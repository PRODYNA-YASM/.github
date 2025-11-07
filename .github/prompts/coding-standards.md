# Coding Standards - PRODYNA-YASM

This document provides comprehensive coding standards for the three primary technology stacks used in the YASM project: TypeScript (frontend), Java/Quarkus (backend), and Go (supporting services).

## TypeScript Coding Standards (yasm-frontend)

### General Principles

- **Strict Mode**: Always use TypeScript strict mode (`"strict": true` in tsconfig.json)
- **Type Safety**: Avoid `any` type; use `unknown` when type is truly unknown
- **Explicit Types**: Prefer explicit return types for functions
- **Modern ES Features**: Use ES2020+ features (async/await, optional chaining, nullish coalescing)

### Naming Conventions

```typescript
// PascalCase for types, interfaces, classes, and React components
interface UserProfile {}
class DataService {}
type ApiResponse = {};
const UserCard: React.FC = () => {};

// camelCase for variables, functions, and methods
const userName = "John";
function fetchUserData() {}

// UPPER_SNAKE_CASE for constants
const API_BASE_URL = "https://api.example.com";
const MAX_RETRY_COUNT = 3;

// Prefix interfaces with 'I' only when needed for disambiguation
interface Props {} // Preferred
interface IUserService {} // Only when clarifying interface vs implementation
```

### React Best Practices

```typescript
// Use functional components with hooks
import React, { useState, useEffect, useCallback, useMemo } from 'react';

interface UserCardProps {
  userId: string;
  onUserClick?: (userId: string) => void;
}

export const UserCard: React.FC<UserCardProps> = ({ userId, onUserClick }) => {
  const [user, setUser] = useState<User | null>(null);
  const [loading, setLoading] = useState(true);

  // Use useCallback for event handlers
  const handleClick = useCallback(() => {
    onUserClick?.(userId);
  }, [userId, onUserClick]);

  // Use useEffect for side effects
  useEffect(() => {
    let cancelled = false;
    
    async function loadUser() {
      try {
        const data = await fetchUser(userId);
        if (!cancelled) {
          setUser(data);
        }
      } catch (error) {
        if (!cancelled) {
          console.error('Failed to fetch user:', error);
        }
      } finally {
        if (!cancelled) {
          setLoading(false);
        }
      }
    }

    loadUser();

    // Cleanup function
    return () => {
      cancelled = true;
    };
  }, [userId]);

  // Use useMemo for expensive calculations
  const displayName = useMemo(() => {
    return user ? `${user.firstName} ${user.lastName}` : 'Unknown';
  }, [user]);

  if (loading) return <LoadingSpinner />;
  if (!user) return <ErrorMessage />;

  return (
    <div onClick={handleClick}>
      <h3>{displayName}</h3>
    </div>
  );
};
```

### State Management

```typescript
// Use React Context for shared state
interface AppState {
  user: User | null;
  theme: 'light' | 'dark';
}

interface AppContextValue {
  state: AppState;
  updateUser: (user: User) => void;
  toggleTheme: () => void;
}

const AppContext = React.createContext<AppContextValue | undefined>(undefined);

export function useAppContext() {
  const context = React.useContext(AppContext);
  if (!context) {
    throw new Error('useAppContext must be used within AppProvider');
  }
  return context;
}

// Custom hooks for reusable logic
export function useDebounce<T>(value: T, delay: number): T {
  const [debouncedValue, setDebouncedValue] = useState<T>(value);

  useEffect(() => {
    const handler = setTimeout(() => {
      setDebouncedValue(value);
    }, delay);

    return () => {
      clearTimeout(handler);
    };
  }, [value, delay]);

  return debouncedValue;
}
```

### Error Handling

```typescript
// Define custom error types
class ApiError extends Error {
  constructor(
    message: string,
    public statusCode: number,
    public response?: unknown
  ) {
    super(message);
    this.name = 'ApiError';
  }
}

// Use proper error handling in async functions
async function fetchData<T>(url: string): Promise<T> {
  try {
    const response = await fetch(url);
    
    if (!response.ok) {
      throw new ApiError(
        `HTTP ${response.status}: ${response.statusText}`,
        response.status,
        await response.json().catch(() => null)
      );
    }
    
    return await response.json();
  } catch (error) {
    if (error instanceof ApiError) {
      throw error;
    }
    throw new ApiError('Network request failed', 0, error);
  }
}

// Error boundaries for React components
class ErrorBoundary extends React.Component<
  { children: React.ReactNode },
  { hasError: boolean; error?: Error }
> {
  state = { hasError: false, error: undefined };

  static getDerivedStateFromError(error: Error) {
    return { hasError: true, error };
  }

  componentDidCatch(error: Error, errorInfo: React.ErrorInfo) {
    console.error('Uncaught error:', error, errorInfo);
  }

  render() {
    if (this.state.hasError) {
      return <ErrorFallback error={this.state.error} />;
    }
    return this.props.children;
  }
}
```

### Testing

```typescript
// Use React Testing Library
import { render, screen, waitFor, fireEvent } from '@testing-library/react';
import userEvent from '@testing-library/user-event';
import { UserCard } from './UserCard';

describe('UserCard', () => {
  it('should display user name when loaded', async () => {
    const mockUser = { id: '1', firstName: 'John', lastName: 'Doe' };
    jest.spyOn(api, 'fetchUser').mockResolvedValue(mockUser);

    render(<UserCard userId="1" />);

    await waitFor(() => {
      expect(screen.getByText('John Doe')).toBeInTheDocument();
    });
  });

  it('should call onUserClick when clicked', async () => {
    const handleClick = jest.fn();
    render(<UserCard userId="1" onUserClick={handleClick} />);

    await waitFor(() => {
      expect(screen.getByText('John Doe')).toBeInTheDocument();
    });

    await userEvent.click(screen.getByText('John Doe'));
    expect(handleClick).toHaveBeenCalledWith('1');
  });
});
```

## Java/Quarkus Coding Standards (yasm-backend)

### General Principles

- **Reactive Programming**: Prefer reactive types (Uni, Multi) over blocking operations
- **Dependency Injection**: Use CDI (@Inject, @ApplicationScoped, etc.)
- **Immutability**: Prefer immutable objects where possible
- **Null Safety**: Use Optional<T> instead of null returns

### Naming Conventions

```java
// PascalCase for classes, interfaces, enums
public class UserService {}
public interface UserRepository {}
public enum UserRole { ADMIN, USER, GUEST }

// camelCase for methods and variables
public User findUserById(String userId) {}
private String userName;

// UPPER_SNAKE_CASE for constants
public static final String DEFAULT_ROLE = "USER";
public static final int MAX_RETRY_ATTEMPTS = 3;

// Package names in lowercase
package com.prodyna.yasm.backend.service;
```

### Reactive Programming with Quarkus

```java
import io.smallrye.mutiny.Uni;
import io.smallrye.mutiny.Multi;
import jakarta.ws.rs.*;
import jakarta.ws.rs.core.MediaType;
import jakarta.ws.rs.core.Response;
import org.eclipse.microprofile.openapi.annotations.Operation;

@Path("/api/users")
@Produces(MediaType.APPLICATION_JSON)
@Consumes(MediaType.APPLICATION_JSON)
public class UserResource {

    @Inject
    UserService userService;

    @GET
    @Path("/{id}")
    @Operation(summary = "Get user by ID")
    public Uni<Response> getUser(@PathParam("id") String userId) {
        return userService.findById(userId)
            .onItem().ifNotNull().transform(user -> Response.ok(user).build())
            .onItem().ifNull().continueWith(Response.status(Response.Status.NOT_FOUND).build())
            .onFailure().recoverWithItem(throwable -> {
                log.error("Failed to fetch user: " + userId, throwable);
                return Response.status(Response.Status.INTERNAL_SERVER_ERROR).build();
            });
    }

    @GET
    @Operation(summary = "List all users")
    public Multi<UserDTO> listUsers(
        @QueryParam("page") @DefaultValue("0") int page,
        @QueryParam("size") @DefaultValue("20") int size
    ) {
        return userService.findAll(page, size);
    }

    @POST
    @Operation(summary = "Create new user")
    public Uni<Response> createUser(CreateUserRequest request) {
        return userService.create(request)
            .onItem().transform(user -> 
                Response.status(Response.Status.CREATED)
                    .entity(user)
                    .build()
            );
    }
}
```

### Service Layer

```java
import io.smallrye.mutiny.Uni;
import io.smallrye.mutiny.Multi;
import jakarta.enterprise.context.ApplicationScoped;
import jakarta.inject.Inject;
import org.jboss.logging.Logger;

@ApplicationScoped
public class UserService {

    private static final Logger log = Logger.getLogger(UserService.class);

    @Inject
    UserRepository repository;

    @Inject
    ValidationService validationService;

    public Uni<User> findById(String userId) {
        return repository.findById(userId)
            .onItem().ifNull().failWith(() -> 
                new NotFoundException("User not found: " + userId)
            );
    }

    public Multi<UserDTO> findAll(int page, int size) {
        return repository.findAll()
            .select().where(user -> user.isActive())
            .skip((long) page * size)
            .select().first(size)
            .map(this::toDTO);
    }

    public Uni<User> create(CreateUserRequest request) {
        return validationService.validate(request)
            .chain(() -> repository.persist(toEntity(request)))
            .invoke(user -> log.infof("Created user: %s", user.getId()));
    }

    private UserDTO toDTO(User user) {
        return UserDTO.builder()
            .id(user.getId())
            .email(user.getEmail())
            .name(user.getName())
            .build();
    }

    private User toEntity(CreateUserRequest request) {
        return User.builder()
            .email(request.getEmail())
            .name(request.getName())
            .build();
    }
}
```

### Exception Handling

```java
// Custom exception hierarchy
public class YasmException extends RuntimeException {
    public YasmException(String message) {
        super(message);
    }

    public YasmException(String message, Throwable cause) {
        super(message, cause);
    }
}

public class NotFoundException extends YasmException {
    public NotFoundException(String message) {
        super(message);
    }
}

public class ValidationException extends YasmException {
    private final List<String> errors;

    public ValidationException(List<String> errors) {
        super("Validation failed: " + String.join(", ", errors));
        this.errors = errors;
    }

    public List<String> getErrors() {
        return errors;
    }
}

// Global exception mapper
@Provider
public class GlobalExceptionMapper implements ExceptionMapper<Exception> {

    private static final Logger log = Logger.getLogger(GlobalExceptionMapper.class);

    @Override
    public Response toResponse(Exception exception) {
        log.error("Unhandled exception", exception);

        if (exception instanceof NotFoundException) {
            return Response.status(Response.Status.NOT_FOUND)
                .entity(new ErrorResponse(exception.getMessage()))
                .build();
        }

        if (exception instanceof ValidationException) {
            ValidationException ve = (ValidationException) exception;
            return Response.status(Response.Status.BAD_REQUEST)
                .entity(new ValidationErrorResponse(ve.getErrors()))
                .build();
        }

        return Response.status(Response.Status.INTERNAL_SERVER_ERROR)
            .entity(new ErrorResponse("Internal server error"))
            .build();
    }
}
```

### Testing

```java
import io.quarkus.test.junit.QuarkusTest;
import io.quarkus.test.InjectMock;
import io.restassured.RestAssured;
import org.junit.jupiter.api.Test;
import org.junit.jupiter.api.BeforeEach;
import org.mockito.Mockito;

import static io.restassured.RestAssured.given;
import static org.hamcrest.Matchers.*;
import static org.mockito.ArgumentMatchers.any;

@QuarkusTest
class UserResourceTest {

    @InjectMock
    UserService userService;

    @BeforeEach
    void setup() {
        Mockito.reset(userService);
    }

    @Test
    void testGetUser() {
        User mockUser = User.builder()
            .id("123")
            .email("test@example.com")
            .name("Test User")
            .build();

        Mockito.when(userService.findById("123"))
            .thenReturn(Uni.createFrom().item(mockUser));

        given()
            .when().get("/api/users/123")
            .then()
            .statusCode(200)
            .body("id", equalTo("123"))
            .body("email", equalTo("test@example.com"))
            .body("name", equalTo("Test User"));
    }

    @Test
    void testGetUserNotFound() {
        Mockito.when(userService.findById("999"))
            .thenReturn(Uni.createFrom().failure(new NotFoundException("User not found")));

        given()
            .when().get("/api/users/999")
            .then()
            .statusCode(404);
    }
}
```

## Go Coding Standards (Supporting Services)

### General Principles

- **Simplicity**: Keep code simple and idiomatic
- **Error Handling**: Always check and handle errors
- **Concurrency**: Use goroutines and channels appropriately
- **Standard Library**: Prefer standard library over external dependencies

### Naming Conventions

```go
// PascalCase for exported identifiers
type UserService struct {}
func NewUserService() *UserService {}

// camelCase for unexported identifiers
type userCache struct {}
func fetchUserData() error {}

// ALL_CAPS for constants (when needed for clarity)
const (
    MaxRetries = 3
    DefaultTimeout = 30 * time.Second
)

// Interface names often end with 'er'
type Reader interface {
    Read(p []byte) (n int, err error)
}
```

### Project Structure

```
.
├── cmd/
│   └── service/
│       └── main.go              # Application entry point
├── internal/
│   ├── api/
│   │   ├── handlers.go          # HTTP handlers
│   │   └── middleware.go        # Middleware
│   ├── service/
│   │   └── user_service.go      # Business logic
│   └── repository/
│       └── user_repository.go   # Data access
├── pkg/
│   └── client/
│       └── api_client.go        # Reusable packages
├── go.mod
└── go.sum
```

### HTTP Handlers and Routing

```go
package api

import (
    "encoding/json"
    "log/slog"
    "net/http"
    
    "github.com/go-chi/chi/v5"
    "github.com/go-chi/chi/v5/middleware"
)

type Server struct {
    router  *chi.Mux
    logger  *slog.Logger
    service UserService
}

func NewServer(logger *slog.Logger, service UserService) *Server {
    s := &Server{
        router:  chi.NewRouter(),
        logger:  logger,
        service: service,
    }
    s.setupRoutes()
    return s
}

func (s *Server) setupRoutes() {
    s.router.Use(middleware.RequestID)
    s.router.Use(middleware.RealIP)
    s.router.Use(middleware.Logger)
    s.router.Use(middleware.Recoverer)

    s.router.Get("/health", s.handleHealth)
    s.router.Route("/api/v1", func(r chi.Router) {
        r.Get("/users/{id}", s.handleGetUser)
        r.Post("/users", s.handleCreateUser)
        r.Get("/users", s.handleListUsers)
    })
}

func (s *Server) handleGetUser(w http.ResponseWriter, r *http.Request) {
    ctx := r.Context()
    userID := chi.URLParam(r, "id")

    if userID == "" {
        s.respondError(w, http.StatusBadRequest, "user ID is required")
        return
    }

    user, err := s.service.GetUser(ctx, userID)
    if err != nil {
        s.logger.ErrorContext(ctx, "failed to get user",
            slog.String("user_id", userID),
            slog.String("error", err.Error()),
        )
        s.respondError(w, http.StatusInternalServerError, "failed to fetch user")
        return
    }

    s.respondJSON(w, http.StatusOK, user)
}

func (s *Server) respondJSON(w http.ResponseWriter, status int, data interface{}) {
    w.Header().Set("Content-Type", "application/json")
    w.WriteStatus(status)
    
    if err := json.NewEncoder(w).Encode(data); err != nil {
        s.logger.Error("failed to encode response", slog.String("error", err.Error()))
    }
}

func (s *Server) respondError(w http.ResponseWriter, status int, message string) {
    s.respondJSON(w, status, map[string]string{"error": message})
}
```

### Service Layer

```go
package service

import (
    "context"
    "errors"
    "fmt"
    "log/slog"
)

var (
    ErrUserNotFound = errors.New("user not found")
    ErrInvalidInput = errors.New("invalid input")
)

type User struct {
    ID    string `json:"id"`
    Email string `json:"email"`
    Name  string `json:"name"`
}

type UserRepository interface {
    GetByID(ctx context.Context, id string) (*User, error)
    Create(ctx context.Context, user *User) error
    List(ctx context.Context, limit, offset int) ([]*User, error)
}

type UserService struct {
    repo   UserRepository
    logger *slog.Logger
}

func NewUserService(repo UserRepository, logger *slog.Logger) *UserService {
    return &UserService{
        repo:   repo,
        logger: logger,
    }
}

func (s *UserService) GetUser(ctx context.Context, id string) (*User, error) {
    if id == "" {
        return nil, fmt.Errorf("%w: user ID is empty", ErrInvalidInput)
    }

    user, err := s.repo.GetByID(ctx, id)
    if err != nil {
        return nil, fmt.Errorf("failed to get user from repository: %w", err)
    }

    if user == nil {
        return nil, ErrUserNotFound
    }

    return user, nil
}

func (s *UserService) CreateUser(ctx context.Context, email, name string) (*User, error) {
    if email == "" || name == "" {
        return nil, fmt.Errorf("%w: email and name are required", ErrInvalidInput)
    }

    user := &User{
        Email: email,
        Name:  name,
    }

    if err := s.repo.Create(ctx, user); err != nil {
        return nil, fmt.Errorf("failed to create user: %w", err)
    }

    s.logger.InfoContext(ctx, "user created",
        slog.String("user_id", user.ID),
        slog.String("email", user.Email),
    )

    return user, nil
}
```

### Concurrency Patterns

```go
// Worker pool pattern
func processItems(ctx context.Context, items []Item, workers int) error {
    jobs := make(chan Item, len(items))
    results := make(chan error, len(items))

    // Start workers
    for w := 0; w < workers; w++ {
        go worker(ctx, jobs, results)
    }

    // Send jobs
    for _, item := range items {
        jobs <- item
    }
    close(jobs)

    // Collect results
    for range items {
        if err := <-results; err != nil {
            return err
        }
    }

    return nil
}

func worker(ctx context.Context, jobs <-chan Item, results chan<- error) {
    for job := range jobs {
        select {
        case <-ctx.Done():
            results <- ctx.Err()
            return
        default:
            results <- processItem(job)
        }
    }
}

// Context-aware operations
func fetchDataWithTimeout(ctx context.Context, url string) ([]byte, error) {
    ctx, cancel := context.WithTimeout(ctx, 10*time.Second)
    defer cancel()

    req, err := http.NewRequestWithContext(ctx, http.MethodGet, url, nil)
    if err != nil {
        return nil, fmt.Errorf("failed to create request: %w", err)
    }

    resp, err := http.DefaultClient.Do(req)
    if err != nil {
        return nil, fmt.Errorf("failed to fetch data: %w", err)
    }
    defer resp.Body.Close()

    return io.ReadAll(resp.Body)
}
```

### Error Handling

```go
// Wrap errors with context
func (s *UserService) UpdateUser(ctx context.Context, id string, updates map[string]interface{}) error {
    user, err := s.repo.GetByID(ctx, id)
    if err != nil {
        return fmt.Errorf("failed to get user %s: %w", id, err)
    }

    if err := s.validateUpdates(updates); err != nil {
        return fmt.Errorf("invalid updates: %w", err)
    }

    if err := s.repo.Update(ctx, user); err != nil {
        return fmt.Errorf("failed to update user %s: %w", id, err)
    }

    return nil
}

// Check for specific errors
func handleUserError(err error) {
    if errors.Is(err, ErrUserNotFound) {
        // Handle not found
    } else if errors.Is(err, context.Canceled) {
        // Handle cancellation
    } else {
        // Handle other errors
    }
}
```

### Testing

```go
package service

import (
    "context"
    "errors"
    "testing"

    "github.com/stretchr/testify/assert"
    "github.com/stretchr/testify/mock"
    "github.com/stretchr/testify/require"
)

// Mock repository
type MockUserRepository struct {
    mock.Mock
}

func (m *MockUserRepository) GetByID(ctx context.Context, id string) (*User, error) {
    args := m.Called(ctx, id)
    if args.Get(0) == nil {
        return nil, args.Error(1)
    }
    return args.Get(0).(*User), args.Error(1)
}

func TestUserService_GetUser(t *testing.T) {
    tests := []struct {
        name    string
        userID  string
        setup   func(*MockUserRepository)
        want    *User
        wantErr error
    }{
        {
            name:   "success",
            userID: "123",
            setup: func(m *MockUserRepository) {
                m.On("GetByID", mock.Anything, "123").
                    Return(&User{ID: "123", Email: "test@example.com"}, nil)
            },
            want:    &User{ID: "123", Email: "test@example.com"},
            wantErr: nil,
        },
        {
            name:   "user not found",
            userID: "999",
            setup: func(m *MockUserRepository) {
                m.On("GetByID", mock.Anything, "999").
                    Return(nil, nil)
            },
            want:    nil,
            wantErr: ErrUserNotFound,
        },
        {
            name:   "empty user ID",
            userID: "",
            setup:  func(m *MockUserRepository) {},
            want:   nil,
            wantErr: ErrInvalidInput,
        },
    }

    for _, tt := range tests {
        t.Run(tt.name, func(t *testing.T) {
            repo := new(MockUserRepository)
            tt.setup(repo)

            service := NewUserService(repo, slog.Default())
            got, err := service.GetUser(context.Background(), tt.userID)

            if tt.wantErr != nil {
                require.Error(t, err)
                assert.ErrorIs(t, err, tt.wantErr)
            } else {
                require.NoError(t, err)
                assert.Equal(t, tt.want, got)
            }

            repo.AssertExpectations(t)
        })
    }
}
```

## Summary

These coding standards ensure:
- **Consistency** across all YASM projects
- **Maintainability** through clear, readable code
- **Reliability** through comprehensive testing
- **Security** through best practices
- **Performance** through appropriate patterns

Always refer to these standards when writing code, and update them as the team learns and grows.
