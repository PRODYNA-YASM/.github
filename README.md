# PRODYNA-YASM Organization Repository

This repository contains organization-wide configurations, documentation, and GitHub Copilot setup for the YASM (Yet Another Skill Management) ecosystem.

## About YASM

YASM is a comprehensive skill management platform built by PRODYNA, designed to help organizations track, manage, and visualize employee skills, projects, and competencies. The platform is built on a modern microservices architecture with a Graph Database (Neo4j) foundation.

### Technology Stack

- **Frontend (yasm-frontend)**: TypeScript, React
- **Backend (yasm-backend)**: Java 21, Quarkus (Reactive)
- **Supporting Services**: Go (yasm-integration, yasm-metrics, yasm-github, etc.)
- **Database**: Neo4j Graph Database
- **Infrastructure**: Kubernetes, Azure, Terraform

## GitHub Copilot Configuration

This repository provides organization-wide GitHub Copilot configuration to ensure consistent, high-quality code across all YASM projects.

### 📚 What's Included

#### Organization-Wide Instructions

**[`.github/copilot-instructions.md`](.github/copilot-instructions.md)**

The main configuration file that GitHub Copilot uses for all repositories in the PRODYNA-YASM organization. Includes:

- Overview of YASM and its architecture
- Technology stack details (TypeScript, Java/Quarkus, Go)
- General coding standards and principles
- Security guidelines overview
- Code review expectations
- Observability requirements
- CI/CD practices

#### Coding Standards

**[`.github/prompts/coding-standards.md`](.github/prompts/coding-standards.md)**

Comprehensive coding standards for all three tech stacks:

- **TypeScript/React**: Component patterns, hooks, state management, testing
- **Java/Quarkus**: Reactive programming, CDI, REST APIs, graph database queries
- **Go**: Idiomatic patterns, concurrency, error handling, HTTP services

Each section includes:
- Naming conventions
- Code examples (good and bad)
- Best practices
- Testing patterns
- Common pitfalls to avoid

#### Code Review Guidelines

**[`.github/prompts/code-review-guidelines.md`](.github/prompts/code-review-guidelines.md)**

Complete code review process documentation:

- Responsibilities of authors and reviewers
- Review checklist by category (functionality, security, performance, etc.)
- How to provide constructive feedback
- PR size and timing recommendations
- Language-specific review points
- Templates for PRs and review comments

#### Security Guidelines

**[`.github/prompts/security-guidelines.md`](.github/prompts/security-guidelines.md)**

Security best practices for all technology stacks:

- OWASP Top 10 awareness
- Input validation and sanitization
- Authentication and authorization
- Secure password handling
- SQL injection prevention
- XSS and CSRF protection
- Secrets management
- Dependency security

Includes specific examples for TypeScript, Java, and Go.

#### Custom Agents

**[`.github/agents/code-reviewer.md`](.github/agents/code-reviewer.md)**

A specialized code review agent that understands:
- YASM technology stack
- TypeScript/React, Java/Quarkus, and Go best practices
- Security vulnerabilities
- Performance optimization
- Our coding standards

**[`.github/agents/documentation-helper.md`](.github/agents/documentation-helper.md)**

A documentation assistant that helps with:
- README creation
- API documentation
- Architecture diagrams
- User guides
- Code comments

#### Knowledge Base

**[`.github/knowledge-base/README.md`](.github/knowledge-base/README.md)**

Guide for setting up and maintaining knowledge bases:
- How GitHub Copilot uses knowledge bases
- Organization-level vs repository-level knowledge
- Creating effective prompts
- Best practices for documentation
- Examples and templates

## How to Use This Configuration

### For All Developers

1. **GitHub Copilot is automatically configured** for all repositories in the PRODYNA-YASM organization using the files in this repository.

2. **Reference the coding standards** when writing code:
   - Before starting a new feature, review the relevant language standards
   - Use the examples as templates for your code
   - Follow the patterns established in the standards

3. **Use the code review guidelines** when reviewing PRs:
   - Follow the review checklist
   - Use the conventional comments (issue:, suggestion:, etc.)
   - Be constructive and educational

4. **Follow security guidelines** for all code:
   - Validate all inputs
   - Use secure authentication
   - Handle errors properly
   - Keep dependencies updated

### Using Copilot Chat

Ask Copilot to reference our standards:

```
@workspace Using the coding standards from .github/prompts/coding-standards.md,
help me write a React component for displaying user skills
```

```
Based on .github/prompts/security-guidelines.md, review this password
validation function for security issues
```

### Using Custom Agents

Invoke our specialized agents:

```
@code-reviewer Please review this pull request focusing on 
Java/Quarkus reactive patterns
```

```
@documentation-helper Create API documentation for this endpoint
following our standards
```

### For Repository Maintainers

1. **Add repository-specific instructions** by creating `.github/copilot-instructions.md` in your repository

2. **Create project-specific prompts** in `.github/prompts/` for common tasks

3. **Document architecture** in `docs/architecture/` with diagrams and explanations

4. **Maintain examples** in `docs/examples/` showing common patterns

See [`.github/knowledge-base/README.md`](.github/knowledge-base/README.md) for detailed guidance.

## Repository Structure

```
.github/
├── copilot-instructions.md           # Organization-wide Copilot configuration
├── prompts/
│   ├── coding-standards.md          # TypeScript, Java, Go standards
│   ├── code-review-guidelines.md    # Review process and best practices
│   └── security-guidelines.md       # Security best practices
├── agents/
│   ├── code-reviewer.md             # Custom code review agent
│   └── documentation-helper.md      # Documentation assistant
├── knowledge-base/
│   └── README.md                    # Knowledge base setup guide
└── workflows/
    └── ...                          # GitHub Actions workflows

profile/
└── README.md                        # Organization profile (deployment overview)

README.md                            # This file
```

## YASM Projects

The PRODYNA-YASM organization includes these main projects:

### Core Platform

- **[yasm-frontend](https://github.com/PRODYNA-YASM/yasm-frontend)** - React/TypeScript frontend
- **[yasm-backend](https://github.com/PRODYNA-YASM/yasm-backend)** - Java/Quarkus backend
- **[yasm-api](https://github.com/PRODYNA-YASM/yasm-api)** - API definitions and schemas

### Supporting Services (Go)

- **[yasm-integration](https://github.com/PRODYNA-YASM/yasm-integration)** - Microsoft 365 integration
- **[yasm-metrics](https://github.com/PRODYNA-YASM/yasm-metrics)** - Metrics collection service
- **[yasm-github](https://github.com/PRODYNA-YASM/yasm-github)** - GitHub integration
- **[yasm-geocoding](https://github.com/PRODYNA-YASM/yasm-geocoding)** - Geocoding service
- **[yasm-mainproject](https://github.com/PRODYNA-YASM/yasm-mainproject)** - Main project service
- **[yasm-proxy-odbc](https://github.com/PRODYNA-YASM/yasm-proxy-odbc)** - ODBC proxy service
- **[yasmctl](https://github.com/PRODYNA-YASM/yasmctl)** - CLI tool

### Infrastructure

- **[yasm-infrastructure-staged](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged)** - Staged environments
- **[yasm-infrastructure-common](https://github.com/PRODYNA-YASM/yasm-infrastructure-common)** - Common infrastructure

### Additional Projects

- **[fox-and-hound](https://github.com/PRODYNA-YASM/fox-and-hound)** - Consultant skills matcher
- **[sales-copilot](https://github.com/PRODYNA-YASM/sales-copilot)** - Sales assistant
- **[yasm-test](https://github.com/PRODYNA-YASM/yasm-test)** - E2E tests
- **[yasm-data](https://github.com/PRODYNA-YASM/yasm-data)** - Data management

See the [organization profile](profile/README.md) for deployment status and release information.

## Contributing

### To This Repository

1. **Propose improvements** to coding standards or guidelines via pull request
2. **Add new prompts** for common tasks or patterns
3. **Update documentation** when best practices evolve
4. **Share knowledge** by documenting solutions to common problems

### To YASM Projects

Each project has its own contribution guidelines. Generally:

1. Follow the coding standards in this repository
2. Write tests for all new code
3. Update documentation
4. Submit a pull request for review
5. Address review feedback promptly

## Support

- **Issues**: Open an issue in the relevant repository
- **Discussions**: Use GitHub Discussions for questions and ideas
- **Security**: Report security issues privately to the security team

## Continuous Improvement

These guidelines and configurations are living documents. We encourage:

- Regular review and updates
- Feedback from the development team
- Documentation of lessons learned
- Sharing of best practices

## License

See [LICENSE](LICENSE) file for details.

## Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Quarkus Documentation](https://quarkus.io/)
- [React Documentation](https://react.dev/)
- [Go Documentation](https://go.dev/doc/)
- [Neo4j Documentation](https://neo4j.com/docs/)

---

**Maintained by the PRODYNA YASM Team**

For questions or suggestions, please open an issue or contact the team.
