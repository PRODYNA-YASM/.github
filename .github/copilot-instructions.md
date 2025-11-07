# GitHub Copilot Organization Instructions - PRODYNA-YASM

## About YASM (Yet Another Skill Management)

YASM is a comprehensive skill management platform built by PRODYNA, designed to help organizations track, manage, and visualize employee skills, projects, and competencies. The platform is built on a modern microservices architecture with a Graph Database foundation.

### Core Components

- **yasm-frontend**: TypeScript/React-based user interface
- **yasm-backend**: Java/Quarkus-based REST API and business logic
- **Supporting Services**: Go-based microservices for integration, metrics, geocoding, and more
- **Infrastructure**: Kubernetes-based deployment with comprehensive observability

## Technology Stack Overview

### Frontend (yasm-frontend)
- **Language**: TypeScript
- **Framework**: React with modern hooks
- **State Management**: React Context/Hooks
- **Build Tool**: Webpack/Vite
- **Testing**: Jest, React Testing Library

### Backend (yasm-backend)
- **Language**: Java 21+
- **Framework**: Quarkus (reactive microservices)
- **Architecture**: Reactive programming with Mutiny
- **Database**: Graph Database (Neo4j)
- **API**: RESTful services with JAX-RS
- **Testing**: JUnit 5, Quarkus Testing Framework

### Supporting Services (Go Projects)
- **Language**: Go 1.23+
- **Projects**: yasm-integration, yasm-metrics, yasm-github, yasm-geocoding, yasm-proxy-odbc, yasm-mainproject, yasmctl
- **Common Libraries**: Standard library, Gorilla Mux/Chi routers, OpenTelemetry
- **Testing**: Go testing package, testify

## General Coding Standards

### Code Quality Principles
1. **Readability First**: Write code that is self-documenting and easy to understand
2. **SOLID Principles**: Follow single responsibility, open/closed, Liskov substitution, interface segregation, and dependency inversion
3. **DRY (Don't Repeat Yourself)**: Extract common functionality into reusable components
4. **YAGNI (You Aren't Gonna Need It)**: Implement only what is needed now
5. **Boy Scout Rule**: Leave code better than you found it

### Error Handling
- Never silently ignore errors
- Provide meaningful error messages with context
- Use appropriate error types for the language/framework
- Log errors with sufficient detail for debugging

### Testing Requirements
- Write unit tests for all business logic
- Aim for >80% code coverage
- Include integration tests for critical paths
- Write tests before fixing bugs (test-driven debugging)

### Documentation Standards
- Document public APIs with clear, concise comments
- Include examples for complex functionality
- Keep README files up-to-date
- Document architectural decisions

### Version Control
- Write clear, descriptive commit messages
- Use conventional commits format: `type(scope): description`
- Types: feat, fix, docs, style, refactor, test, chore
- Keep commits atomic and focused

## Security Guidelines

### Authentication & Authorization
- Always validate user permissions before operations
- Use secure token-based authentication (JWT, OAuth2)
- Never store credentials in code or logs
- Implement proper session management

### Data Protection
- Encrypt sensitive data at rest and in transit
- Use parameterized queries to prevent SQL injection
- Validate and sanitize all user inputs
- Implement proper CORS policies

### Dependency Management
- Keep dependencies up to date
- Review security advisories regularly
- Use dependency scanning tools
- Minimize third-party dependencies

## Code Review Expectations

### As a Reviewer
- Review code within 24 hours
- Provide constructive, actionable feedback
- Focus on logic, security, and maintainability
- Approve only when truly satisfied

### As an Author
- Self-review before requesting review
- Keep pull requests focused and reasonably sized
- Respond to feedback promptly
- Add tests and documentation

### Review Checklist
- [ ] Code follows language-specific standards
- [ ] Tests are included and pass
- [ ] No security vulnerabilities introduced
- [ ] Documentation is updated
- [ ] No unnecessary dependencies added
- [ ] Error handling is appropriate
- [ ] Performance considerations addressed

## Observability

All services must implement:
- **Structured Logging**: Use appropriate log levels (DEBUG, INFO, WARN, ERROR)
- **Metrics**: Expose Prometheus-compatible metrics
- **Tracing**: Implement OpenTelemetry tracing
- **Health Checks**: Provide readiness and liveness endpoints

## Performance Considerations

- Optimize database queries (avoid N+1 queries)
- Implement caching where appropriate
- Use asynchronous processing for long-running tasks
- Monitor and optimize memory usage
- Consider horizontal scalability in design

## Accessibility

For frontend code:
- Follow WCAG 2.1 AA guidelines
- Use semantic HTML
- Ensure keyboard navigation works
- Provide appropriate ARIA labels
- Test with screen readers

## CI/CD Practices

- All code must pass CI checks before merging
- Automated tests must pass
- Code must be formatted according to standards
- Security scans must pass
- Documentation must build successfully

## Language-Specific Guidance

For detailed coding standards specific to each language, refer to:
- `.github/prompts/coding-standards.md` - Comprehensive standards for TypeScript, Java/Quarkus, and Go
- `.github/prompts/security-guidelines.md` - Security best practices for each stack
- `.github/prompts/code-review-guidelines.md` - Detailed code review process

## Getting Help

- Use GitHub Copilot prompts in `.github/prompts/` for guidance
- Consult the knowledge base in `.github/knowledge-base/`
- Ask the custom agents defined in `.github/agents/` for specialized help
- Refer to project-specific README files for component details

## Continuous Improvement

These guidelines are living documents. If you find areas for improvement:
1. Open a discussion in the repository
2. Propose changes via pull request
3. Document lessons learned from incidents
4. Share knowledge with the team
