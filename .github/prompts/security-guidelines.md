# Security Guidelines - PRODYNA-YASM

This document provides comprehensive security guidelines for all technology stacks used in the YASM project. Security is everyone's responsibility, and these guidelines help ensure we build secure applications.

## General Security Principles

### Defense in Depth
Implement multiple layers of security controls. Never rely on a single security mechanism.

### Principle of Least Privilege
Grant only the minimum permissions necessary for a task.

### Fail Securely
When errors occur, fail in a way that denies access rather than grants it.

### Security by Default
Secure configurations should be the default, not opt-in.

### Never Trust User Input
All user input is potentially malicious until proven otherwise.

## Common Security Vulnerabilities

### OWASP Top 10 Awareness

1. **Broken Access Control**
2. **Cryptographic Failures**
3. **Injection**
4. **Insecure Design**
5. **Security Misconfiguration**
6. **Vulnerable and Outdated Components**
7. **Identification and Authentication Failures**
8. **Software and Data Integrity Failures**
9. **Security Logging and Monitoring Failures**
10. **Server-Side Request Forgery (SSRF)**

## TypeScript/Frontend Security

### Input Validation and Sanitization

```typescript
// ❌ DANGEROUS: XSS vulnerability
function DisplayUserContent({ content }: { content: string }) {
  return <div dangerouslySetInnerHTML={{ __html: content }} />;
}

// ✅ SAFE: Use text content by default
function DisplayUserContent({ content }: { content: string }) {
  return <div>{content}</div>;
}

// ✅ SAFE: Use a sanitization library when HTML is needed
import DOMPurify from 'dompurify';

function DisplayUserContent({ content }: { content: string }) {
  const sanitized = DOMPurify.sanitize(content, {
    ALLOWED_TAGS: ['b', 'i', 'em', 'strong', 'a'],
    ALLOWED_ATTR: ['href']
  });
  return <div dangerouslySetInnerHTML={{ __html: sanitized }} />;
}
```

### Authentication Token Handling

```typescript
// ✅ CORRECT: Store tokens securely
class AuthService {
  private readonly TOKEN_KEY = 'auth_token';

  // Store in httpOnly cookie (backend-set) - PREFERRED
  // OR sessionStorage (for SPA, cleared on tab close)
  setToken(token: string): void {
    sessionStorage.setItem(this.TOKEN_KEY, token);
    // Never use localStorage for sensitive tokens (XSS vulnerable)
  }

  getToken(): string | null {
    return sessionStorage.getItem(this.TOKEN_KEY);
  }

  clearToken(): void {
    sessionStorage.removeItem(this.TOKEN_KEY);
  }

  // Add token to requests
  async authenticatedFetch(url: string, options: RequestInit = {}): Promise<Response> {
    const token = this.getToken();
    
    if (!token) {
      throw new Error('No authentication token available');
    }

    return fetch(url, {
      ...options,
      headers: {
        ...options.headers,
        'Authorization': `Bearer ${token}`,
      },
    });
  }
}
```

### CSRF Protection

```typescript
// ✅ Include CSRF token in state-changing requests
async function updateUserProfile(data: UserProfile): Promise<void> {
  const csrfToken = document.querySelector<HTMLMetaElement>('meta[name="csrf-token"]')?.content;
  
  if (!csrfToken) {
    throw new Error('CSRF token not found');
  }

  await fetch('/api/user/profile', {
    method: 'PUT',
    headers: {
      'Content-Type': 'application/json',
      'X-CSRF-Token': csrfToken,
    },
    body: JSON.stringify(data),
  });
}
```

### Content Security Policy (CSP)

```typescript
// Set in HTML or via headers
const cspMeta = `
  default-src 'self';
  script-src 'self' 'unsafe-inline' 'unsafe-eval';
  style-src 'self' 'unsafe-inline';
  img-src 'self' data: https:;
  font-src 'self' data:;
  connect-src 'self' https://api.yasm.com;
  frame-ancestors 'none';
  base-uri 'self';
  form-action 'self';
`;

// In React helmet or HTML head:
<meta httpEquiv="Content-Security-Policy" content={cspMeta} />
```

### Sensitive Data Exposure

```typescript
// ❌ DANGEROUS: Logging sensitive data
console.log('User logged in:', { username, password, creditCard });

// ✅ SAFE: Sanitize logs
console.log('User logged in:', { 
  username, 
  userId,
  timestamp: new Date().toISOString() 
});

// ❌ DANGEROUS: Storing sensitive data in localStorage
localStorage.setItem('creditCard', cardNumber);

// ✅ SAFE: Never store sensitive data in browser storage
// Use secure, httpOnly cookies set by backend
```

### API Call Security

```typescript
// ✅ Type-safe API client with validation
import { z } from 'zod';

const UserSchema = z.object({
  id: z.string().uuid(),
  email: z.string().email(),
  name: z.string().min(1).max(100),
  role: z.enum(['admin', 'user', 'guest']),
});

type User = z.infer<typeof UserSchema>;

async function fetchUser(userId: string): Promise<User> {
  // Validate input
  if (!z.string().uuid().safeParse(userId).success) {
    throw new Error('Invalid user ID format');
  }

  const response = await fetch(`/api/users/${encodeURIComponent(userId)}`);
  
  if (!response.ok) {
    throw new Error(`HTTP ${response.status}: ${response.statusText}`);
  }

  const data = await response.json();
  
  // Validate response
  return UserSchema.parse(data);
}
```

### Dependency Security

```json
// package.json - use exact versions for security-critical dependencies
{
  "dependencies": {
    "react": "18.2.0",
    "react-dom": "18.2.0"
  },
  "scripts": {
    "audit": "npm audit",
    "audit-fix": "npm audit fix"
  }
}
```

## Java/Quarkus Security

### Input Validation

```java
import jakarta.validation.constraints.*;
import jakarta.validation.Valid;

public class CreateUserRequest {
    
    @NotBlank(message = "Email is required")
    @Email(message = "Invalid email format")
    @Size(max = 255)
    private String email;
    
    @NotBlank(message = "Name is required")
    @Pattern(regexp = "^[a-zA-Z\\s'-]+$", message = "Name contains invalid characters")
    @Size(min = 2, max = 100)
    private String name;
    
    @NotBlank(message = "Password is required")
    @Size(min = 12, max = 128)
    @Pattern(
        regexp = "^(?=.*[a-z])(?=.*[A-Z])(?=.*\\d)(?=.*[@$!%*?&])[A-Za-z\\d@$!%*?&]+$",
        message = "Password must contain uppercase, lowercase, digit, and special character"
    )
    private String password;
    
    // Getters and setters
}

@POST
@Path("/users")
public Uni<Response> createUser(@Valid CreateUserRequest request) {
    // Validation happens automatically
    return userService.create(request);
}
```

### SQL Injection Prevention

```java
// ❌ DANGEROUS: String concatenation
public Uni<User> findUserByEmail(String email) {
    String query = "SELECT * FROM users WHERE email = '" + email + "'";
    return client.query(query); // SQL INJECTION VULNERABILITY
}

// ✅ SAFE: Parameterized queries
public Uni<User> findUserByEmail(String email) {
    return client.preparedQuery("SELECT * FROM users WHERE email = $1")
        .execute(Tuple.of(email))
        .map(rows -> mapToUser(rows.iterator().next()));
}

// ✅ SAFE: Using Panache
@Entity
public class User extends PanacheEntity {
    public String email;
    
    public static Uni<User> findByEmail(String email) {
        return find("email", email).firstResult();
    }
}
```

### Authentication and Authorization

```java
import io.quarkus.security.Authenticated;
import jakarta.annotation.security.RolesAllowed;
import jakarta.annotation.security.PermitAll;

@Path("/api/users")
public class UserResource {

    // Anyone can access
    @GET
    @Path("/public")
    @PermitAll
    public Uni<Response> getPublicData() {
        return Uni.createFrom().item(Response.ok().build());
    }

    // Must be authenticated
    @GET
    @Path("/profile")
    @Authenticated
    public Uni<Response> getProfile(@Context SecurityContext ctx) {
        String userId = ctx.getUserPrincipal().getName();
        return userService.findById(userId)
            .map(user -> Response.ok(user).build());
    }

    // Requires specific role
    @POST
    @Path("/admin/users")
    @RolesAllowed("admin")
    public Uni<Response> createUser(CreateUserRequest request) {
        return userService.create(request);
    }

    // Custom authorization logic
    @DELETE
    @Path("/{id}")
    @Authenticated
    public Uni<Response> deleteUser(
        @PathParam("id") String userId,
        @Context SecurityContext ctx
    ) {
        String currentUserId = ctx.getUserPrincipal().getName();
        
        // Users can only delete their own account, admins can delete any
        if (!userId.equals(currentUserId) && !ctx.isUserInRole("admin")) {
            return Uni.createFrom().item(
                Response.status(Response.Status.FORBIDDEN).build()
            );
        }
        
        return userService.delete(userId);
    }
}
```

### Secure Password Handling

```java
import at.favre.lib.crypto.bcrypt.BCrypt;

@ApplicationScoped
public class PasswordService {
    
    private static final int BCRYPT_COST = 12;

    public String hashPassword(String plainPassword) {
        return BCrypt.withDefaults()
            .hashToString(BCRYPT_COST, plainPassword.toCharArray());
    }

    public boolean verifyPassword(String plainPassword, String hashedPassword) {
        BCrypt.Result result = BCrypt.verifyer()
            .verify(plainPassword.toCharArray(), hashedPassword);
        return result.verified;
    }

    public boolean isPasswordStrong(String password) {
        // At least 12 characters, with upper, lower, digit, and special char
        return password.length() >= 12
            && password.matches(".*[a-z].*")
            && password.matches(".*[A-Z].*")
            && password.matches(".*\\d.*")
            && password.matches(".*[@$!%*?&].*");
    }
}
```

### Preventing XXE (XML External Entity) Attacks

```java
import javax.xml.parsers.DocumentBuilderFactory;
import javax.xml.parsers.DocumentBuilder;

// ✅ SAFE: Disable external entities
public DocumentBuilder createSafeDocumentBuilder() throws Exception {
    DocumentBuilderFactory factory = DocumentBuilderFactory.newInstance();
    
    // Disable DTDs completely
    factory.setFeature("http://apache.org/xml/features/disallow-doctype-decl", true);
    
    // Disable external entities
    factory.setFeature("http://xml.org/sax/features/external-general-entities", false);
    factory.setFeature("http://xml.org/sax/features/external-parameter-entities", false);
    
    // Disable external DTDs
    factory.setFeature("http://apache.org/xml/features/nonvalidating/load-external-dtd", false);
    
    factory.setXIncludeAware(false);
    factory.setExpandEntityReferences(false);
    
    return factory.newDocumentBuilder();
}
```

### Secure Configuration

```java
// application.properties - Never commit secrets
// Use environment variables or secret management

# ❌ DANGEROUS
quarkus.datasource.password=myP@ssw0rd123

# ✅ SAFE - Use environment variables
quarkus.datasource.password=${DB_PASSWORD}

# ✅ SAFE - Use Vault or secret management
quarkus.vault.url=https://vault.example.com
quarkus.vault.authentication.kubernetes.role=my-role
```

### CORS Configuration

```java
// application.properties
# Restrict CORS to specific origins
quarkus.http.cors=true
quarkus.http.cors.origins=https://app.yasm.com,https://staging.yasm.com
quarkus.http.cors.methods=GET,POST,PUT,DELETE
quarkus.http.cors.headers=Content-Type,Authorization
quarkus.http.cors.exposed-headers=Location
quarkus.http.cors.access-control-max-age=86400
```

## Go Security

### Input Validation

```go
import (
    "errors"
    "regexp"
    "unicode/utf8"
)

var (
    emailRegex = regexp.MustCompile(`^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`)
    ErrInvalidInput = errors.New("invalid input")
)

type CreateUserRequest struct {
    Email    string `json:"email"`
    Name     string `json:"name"`
    Password string `json:"password"`
}

func (r *CreateUserRequest) Validate() error {
    // Email validation
    if r.Email == "" {
        return fmt.Errorf("%w: email is required", ErrInvalidInput)
    }
    if !emailRegex.MatchString(r.Email) {
        return fmt.Errorf("%w: invalid email format", ErrInvalidInput)
    }

    // Name validation
    if r.Name == "" {
        return fmt.Errorf("%w: name is required", ErrInvalidInput)
    }
    if utf8.RuneCountInString(r.Name) > 100 {
        return fmt.Errorf("%w: name too long", ErrInvalidInput)
    }

    // Password validation
    if err := validatePassword(r.Password); err != nil {
        return err
    }

    return nil
}

func validatePassword(password string) error {
    if len(password) < 12 {
        return fmt.Errorf("%w: password must be at least 12 characters", ErrInvalidInput)
    }
    
    var (
        hasUpper   = false
        hasLower   = false
        hasDigit   = false
        hasSpecial = false
    )
    
    for _, char := range password {
        switch {
        case unicode.IsUpper(char):
            hasUpper = true
        case unicode.IsLower(char):
            hasLower = true
        case unicode.IsDigit(char):
            hasDigit = true
        case unicode.IsPunct(char) || unicode.IsSymbol(char):
            hasSpecial = true
        }
    }
    
    if !(hasUpper && hasLower && hasDigit && hasSpecial) {
        return fmt.Errorf("%w: password must contain uppercase, lowercase, digit, and special character", ErrInvalidInput)
    }
    
    return nil
}
```

### SQL Injection Prevention

```go
import "database/sql"

// ❌ DANGEROUS: String concatenation
func getUserByEmail(db *sql.DB, email string) (*User, error) {
    query := "SELECT * FROM users WHERE email = '" + email + "'"
    // SQL INJECTION VULNERABILITY
    row := db.QueryRow(query)
}

// ✅ SAFE: Parameterized queries
func getUserByEmail(ctx context.Context, db *sql.DB, email string) (*User, error) {
    query := "SELECT id, email, name FROM users WHERE email = ?"
    
    var user User
    err := db.QueryRowContext(ctx, query, email).Scan(
        &user.ID,
        &user.Email,
        &user.Name,
    )
    
    if err != nil {
        if errors.Is(err, sql.ErrNoRows) {
            return nil, ErrUserNotFound
        }
        return nil, fmt.Errorf("failed to query user: %w", err)
    }
    
    return &user, nil
}
```

### Secure Password Hashing

```go
import "golang.org/x/crypto/bcrypt"

const bcryptCost = 12

func hashPassword(password string) (string, error) {
    hash, err := bcrypt.GenerateFromPassword([]byte(password), bcryptCost)
    if err != nil {
        return "", fmt.Errorf("failed to hash password: %w", err)
    }
    return string(hash), nil
}

func verifyPassword(password, hash string) error {
    err := bcrypt.CompareHashAndPassword([]byte(hash), []byte(password))
    if err != nil {
        if errors.Is(err, bcrypt.ErrMismatchedHashAndPassword) {
            return ErrInvalidCredentials
        }
        return fmt.Errorf("failed to verify password: %w", err)
    }
    return nil
}
```

### JWT Token Handling

```go
import (
    "github.com/golang-jwt/jwt/v5"
    "time"
)

type Claims struct {
    UserID string `json:"user_id"`
    Role   string `json:"role"`
    jwt.RegisteredClaims
}

func generateToken(userID, role string, secret []byte) (string, error) {
    claims := Claims{
        UserID: userID,
        Role:   role,
        RegisteredClaims: jwt.RegisteredClaims{
            ExpiresAt: jwt.NewNumericDate(time.Now().Add(24 * time.Hour)),
            IssuedAt:  jwt.NewNumericDate(time.Now()),
            NotBefore: jwt.NewNumericDate(time.Now()),
            Issuer:    "yasm-auth",
        },
    }

    token := jwt.NewWithClaims(jwt.SigningMethodHS256, claims)
    return token.SignedString(secret)
}

func validateToken(tokenString string, secret []byte) (*Claims, error) {
    token, err := jwt.ParseWithClaims(tokenString, &Claims{}, func(token *jwt.Token) (interface{}, error) {
        // Verify signing method
        if _, ok := token.Method.(*jwt.SigningMethodHMAC); !ok {
            return nil, fmt.Errorf("unexpected signing method: %v", token.Header["alg"])
        }
        return secret, nil
    })

    if err != nil {
        return nil, fmt.Errorf("failed to parse token: %w", err)
    }

    if claims, ok := token.Claims.(*Claims); ok && token.Valid {
        return claims, nil
    }

    return nil, errors.New("invalid token")
}
```

### CSRF Protection Middleware

```go
import (
    "crypto/rand"
    "encoding/base64"
    "net/http"
)

func generateCSRFToken() (string, error) {
    b := make([]byte, 32)
    if _, err := rand.Read(b); err != nil {
        return "", err
    }
    return base64.URLEncoding.EncodeToString(b), nil
}

func CSRFMiddleware(next http.Handler) http.Handler {
    return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
        // Skip CSRF for GET, HEAD, OPTIONS
        if r.Method == "GET" || r.Method == "HEAD" || r.Method == "OPTIONS" {
            next.ServeHTTP(w, r)
            return
        }

        // Get token from header
        headerToken := r.Header.Get("X-CSRF-Token")
        
        // Get token from session/cookie
        session, err := getSession(r)
        if err != nil {
            http.Error(w, "Invalid session", http.StatusForbidden)
            return
        }

        sessionToken := session.CSRFToken
        
        // Validate tokens match
        if headerToken == "" || sessionToken == "" || headerToken != sessionToken {
            http.Error(w, "Invalid CSRF token", http.StatusForbidden)
            return
        }

        next.ServeHTTP(w, r)
    })
}
```

### Rate Limiting

```go
import (
    "golang.org/x/time/rate"
    "sync"
)

type RateLimiter struct {
    visitors map[string]*rate.Limiter
    mu       sync.RWMutex
    rate     rate.Limit
    burst    int
}

func NewRateLimiter(r rate.Limit, b int) *RateLimiter {
    return &RateLimiter{
        visitors: make(map[string]*rate.Limiter),
        rate:     r,
        burst:    b,
    }
}

func (rl *RateLimiter) getLimiter(ip string) *rate.Limiter {
    rl.mu.Lock()
    defer rl.mu.Unlock()

    limiter, exists := rl.visitors[ip]
    if !exists {
        limiter = rate.NewLimiter(rl.rate, rl.burst)
        rl.visitors[ip] = limiter
    }

    return limiter
}

func (rl *RateLimiter) Middleware(next http.Handler) http.Handler {
    return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
        ip := r.RemoteAddr
        limiter := rl.getLimiter(ip)

        if !limiter.Allow() {
            http.Error(w, "Too many requests", http.StatusTooManyRequests)
            return
        }

        next.ServeHTTP(w, r)
    })
}
```

## Secrets Management

### Never Commit Secrets

```bash
# .gitignore
.env
.env.local
.env.*.local
secrets/
*.pem
*.key
config/local.yaml
```

### Use Environment Variables

```go
// ✅ Load from environment
func loadConfig() (*Config, error) {
    return &Config{
        DBPassword:   os.Getenv("DB_PASSWORD"),
        APIKey:       os.Getenv("API_KEY"),
        JWTSecret:    []byte(os.Getenv("JWT_SECRET")),
    }, nil
}
```

### Use Secret Management Services

- Azure Key Vault
- HashiCorp Vault
- AWS Secrets Manager
- Kubernetes Secrets

## Dependency Security

### Regular Updates

```bash
# TypeScript/Node.js
npm audit
npm audit fix
npm outdated

# Java/Maven
mvn versions:display-dependency-updates
mvn versions:display-plugin-updates

# Go
go list -u -m all
go get -u ./...
```

### Automated Scanning

Enable Dependabot in GitHub:
```yaml
# .github/dependabot.yml
version: 2
updates:
  - package-ecosystem: "npm"
    directory: "/"
    schedule:
      interval: "weekly"
  - package-ecosystem: "maven"
    directory: "/"
    schedule:
      interval: "weekly"
  - package-ecosystem: "gomod"
    directory: "/"
    schedule:
      interval: "weekly"
```

## Logging and Monitoring

### Secure Logging

```go
// ❌ DANGEROUS: Logging sensitive data
log.Printf("User login: %s with password: %s", username, password)

// ✅ SAFE: Sanitized logging
log.Printf("User login attempt: user_id=%s, success=%v", userID, success)
```

### Security Event Logging

```java
@ApplicationScoped
public class SecurityAuditLogger {
    
    private static final Logger log = Logger.getLogger(SecurityAuditLogger.class);

    public void logAuthenticationSuccess(String userId, String ip) {
        log.infof("AUTH_SUCCESS user_id=%s ip=%s", userId, ip);
    }

    public void logAuthenticationFailure(String username, String ip, String reason) {
        log.warnf("AUTH_FAILURE username=%s ip=%s reason=%s", username, ip, reason);
    }

    public void logAuthorizationFailure(String userId, String resource, String ip) {
        log.warnf("AUTHZ_FAILURE user_id=%s resource=%s ip=%s", userId, resource, ip);
    }

    public void logSensitiveDataAccess(String userId, String dataType, String ip) {
        log.infof("SENSITIVE_ACCESS user_id=%s data_type=%s ip=%s", userId, dataType, ip);
    }
}
```

## Security Checklist

### Before Each Release

- [ ] All dependencies updated and scanned
- [ ] No hardcoded secrets or credentials
- [ ] Authentication and authorization properly implemented
- [ ] Input validation on all user inputs
- [ ] SQL injection prevention verified
- [ ] XSS prevention verified
- [ ] CSRF protection enabled
- [ ] HTTPS enforced
- [ ] Security headers configured
- [ ] Error messages don't leak sensitive info
- [ ] Logging doesn't expose sensitive data
- [ ] Rate limiting implemented
- [ ] Security tests passing
- [ ] Code scanning (CodeQL) passed

## Incident Response

### If You Discover a Security Issue

1. **Do not** commit the fix to a public branch
2. **Report** immediately to the security team
3. **Document** the vulnerability privately
4. **Coordinate** the fix with the security team
5. **Test** thoroughly before deploying
6. **Deploy** the fix as soon as possible
7. **Monitor** for exploitation attempts

## Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)
- [CWE Top 25](https://cwe.mitre.org/top25/)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)

## Conclusion

Security is not a one-time task but a continuous process. Stay informed about new vulnerabilities, update dependencies regularly, and always think like an attacker when reviewing code.
