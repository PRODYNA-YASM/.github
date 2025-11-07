# Knowledge Base Setup Guide - PRODYNA-YASM

This guide explains how to set up and use knowledge bases with GitHub Copilot to provide better context-aware assistance across the YASM organization.

## What is a Knowledge Base?

A knowledge base is a collection of documentation, code examples, and organizational knowledge that GitHub Copilot can reference to provide more accurate and contextually relevant suggestions. It helps Copilot understand:

- Your organization's coding standards
- Project-specific patterns and practices
- Common solutions to recurring problems
- Domain-specific knowledge about YASM

## Benefits

1. **Consistent Code Quality**: Copilot suggestions align with your standards
2. **Reduced Onboarding Time**: New developers get suggestions that follow your patterns
3. **Domain Knowledge**: Copilot understands YASM-specific concepts
4. **Fewer Errors**: Suggestions follow your security and best practices guidelines

## Organization-Level Knowledge Base

### What We've Already Set Up

The PRODYNA-YASM organization has the following knowledge base structure:

```
.github/
├── copilot-instructions.md          # Organization-wide instructions
├── prompts/
│   ├── coding-standards.md          # Language-specific standards
│   ├── code-review-guidelines.md    # Review process
│   └── security-guidelines.md       # Security best practices
├── agents/
│   ├── code-reviewer.md             # Custom code review agent
│   └── documentation-helper.md      # Documentation assistant
└── knowledge-base/
    └── README.md                    # This file
```

### How Copilot Uses These Files

1. **copilot-instructions.md**: Applied to all repositories in the organization
2. **prompts/**: Available as reusable prompts for common tasks
3. **agents/**: Custom agents that can be invoked for specialized help
4. **knowledge-base/**: Documentation and examples for reference

## Repository-Level Knowledge Base

Each repository can extend the organization knowledge base with project-specific information.

### Recommended Repository Structure

```
repository/
├── .github/
│   └── copilot-instructions.md      # Repository-specific instructions
├── docs/
│   ├── architecture/
│   │   ├── README.md
│   │   ├── database-schema.md
│   │   └── api-design.md
│   ├── development/
│   │   ├── setup.md
│   │   ├── testing.md
│   │   └── deployment.md
│   └── examples/
│       ├── common-patterns.md
│       └── code-snippets.md
└── README.md
```

### Creating Repository Instructions

Create `.github/copilot-instructions.md` in each repository:

**Example for yasm-frontend:**

```markdown
# GitHub Copilot Instructions - yasm-frontend

## Project Overview

This is the TypeScript/React frontend for the YASM skill management platform.

## Technology Stack

- React 18+ with functional components and hooks
- TypeScript in strict mode
- React Router for routing
- React Query for server state management
- Tailwind CSS for styling
- Vite as build tool

## Key Patterns

### Component Structure

Use functional components with TypeScript:

```typescript
interface UserCardProps {
  userId: string;
  onUserClick?: (userId: string) => void;
}

export const UserCard: React.FC<UserCardProps> = ({ userId, onUserClick }) => {
  // Component logic
};
```

### Data Fetching

Use React Query for all API calls:

```typescript
import { useQuery } from '@tanstack/react-query';

function useUser(userId: string) {
  return useQuery({
    queryKey: ['user', userId],
    queryFn: () => fetchUser(userId),
  });
}
```

### State Management

Prefer React hooks and context over external state libraries.

## File Organization

- `/src/components` - Reusable UI components
- `/src/pages` - Page components
- `/src/hooks` - Custom React hooks
- `/src/api` - API client functions
- `/src/types` - TypeScript type definitions
- `/src/utils` - Utility functions

## Testing

All components should have tests using React Testing Library.

## Important Notes

- Always use TypeScript strict mode
- Follow accessibility guidelines (WCAG 2.1 AA)
- Use semantic HTML
- Implement proper error boundaries
```

**Example for yasm-backend:**

```markdown
# GitHub Copilot Instructions - yasm-backend

## Project Overview

This is the Java/Quarkus backend for the YASM skill management platform.

## Technology Stack

- Java 21
- Quarkus 3.x
- Reactive programming with Mutiny
- Neo4j graph database
- REST APIs with JAX-RS
- OpenTelemetry for observability

## Key Patterns

### Service Layer

All services use reactive types:

```java
@ApplicationScoped
public class UserService {
    @Inject
    UserRepository repository;

    public Uni<User> findById(String id) {
        return repository.findById(id)
            .onItem().ifNull().failWith(() -> 
                new NotFoundException("User not found: " + id)
            );
    }
}
```

### REST Resources

Use reactive endpoints:

```java
@Path("/api/users")
public class UserResource {
    @Inject
    UserService service;

    @GET
    @Path("/{id}")
    public Uni<Response> getUser(@PathParam("id") String id) {
        return service.findById(id)
            .map(user -> Response.ok(user).build());
    }
}
```

### Graph Database Queries

Use parameterized Cypher queries:

```java
public Uni<List<User>> findUsersBySkill(String skillId) {
    String cypher = "MATCH (u:User)-[:HAS_SKILL]->(s:Skill {id: $skillId}) RETURN u";
    return neo4j.query(cypher)
        .execute(Map.of("skillId", skillId));
}
```

## Important Notes

- Always use Uni/Multi for async operations
- Never block reactive chains
- Use CDI for dependency injection
- Validate all inputs with Bean Validation
- Log with structured logging (JSON)
```

## Creating Effective Prompts

Prompts in `.github/prompts/` should be reusable templates for common tasks.

### Prompt Structure

```markdown
# Prompt Title

## Purpose
What this prompt helps with

## Context
When to use this prompt

## Instructions
Step-by-step guidance

## Example Input
Sample starting code

## Expected Output
What the result should look like

## Variations
Different use cases
```

### Example Prompts

**`.github/prompts/create-api-endpoint.md`:**

```markdown
# Create API Endpoint

## Purpose
Generate a complete REST API endpoint with proper validation, error handling, and tests.

## Instructions

1. Define the request/response DTOs with validation
2. Create the service method with reactive types
3. Implement the REST resource
4. Add error handling
5. Write comprehensive tests

## Example

For a "Get User by Email" endpoint:

Request DTO:
```java
public class GetUserByEmailRequest {
    @NotBlank
    @Email
    private String email;
}
```

Service:
```java
public Uni<User> findByEmail(String email) {
    return repository.findByEmail(email);
}
```

Resource:
```java
@GET
@Path("/by-email/{email}")
public Uni<Response> getUserByEmail(@PathParam("email") String email) {
    return service.findByEmail(email)
        .map(user -> Response.ok(user).build());
}
```
```

## Using Knowledge Base with Copilot

### In the IDE

1. **Context from Files**: Copilot automatically reads relevant files in your workspace
2. **Reference Documentation**: Open documentation files to give Copilot more context
3. **Use Prompts**: Reference prompt files when asking for help

### In Copilot Chat

```
@workspace Use the coding standards from .github/prompts/coding-standards.md 
to review this function
```

```
Based on .github/prompts/security-guidelines.md, is this password 
validation secure?
```

### With Custom Agents

```
@code-reviewer Please review this pull request focusing on 
TypeScript best practices
```

```
@documentation-helper Create a README for this new service based 
on our documentation standards
```

## Best Practices

### Keep It Current

- Update instructions when patterns change
- Review quarterly for accuracy
- Remove outdated examples
- Add new patterns as they emerge

### Be Specific

- Provide concrete examples
- Show both good and bad patterns
- Include rationale for decisions
- Reference authoritative sources

### Make It Discoverable

- Use clear file names
- Organize logically
- Cross-reference related docs
- Include a table of contents

### Maintain Consistency

- Use the same terminology across docs
- Follow a consistent format
- Link to canonical definitions
- Avoid contradicting guidelines

## Knowledge Base Content Ideas

### Architecture Documentation

- System architecture diagrams
- Component interaction flows
- Database schema and relationships
- Deployment architecture
- Integration patterns

### Code Examples

- Common patterns and their usage
- Utility functions
- Complex algorithms explained
- Design pattern implementations
- Test examples

### Domain Knowledge

- YASM-specific terminology
- Business rules and logic
- User workflows
- Data models
- API contracts

### Troubleshooting

- Common errors and solutions
- Debugging strategies
- Performance optimization tips
- Configuration issues
- Environment-specific problems

### Workflows

- Git workflow
- Code review process
- Deployment procedures
- Testing strategies
- Release management

## Measuring Effectiveness

Track these metrics to understand knowledge base impact:

1. **Code Quality**: Fewer bugs in new code
2. **Consistency**: More uniform code patterns
3. **Onboarding Time**: Faster ramp-up for new developers
4. **Review Feedback**: Less repetitive review comments
5. **Developer Satisfaction**: Survey team about Copilot usefulness

## Advanced: Custom Knowledge Sources

### External Documentation

Link to external resources in your instructions:

```markdown
## References

- [Quarkus Guides](https://quarkus.io/guides/)
- [Neo4j Cypher Manual](https://neo4j.com/docs/cypher-manual/)
- [React Documentation](https://react.dev/)
```

### API Specifications

Include OpenAPI/Swagger specs:

```yaml
# .github/knowledge-base/api-spec.yaml
openapi: 3.0.0
info:
  title: YASM API
  version: 1.0.0
paths:
  /api/users/{id}:
    get:
      summary: Get user by ID
      parameters:
        - name: id
          in: path
          required: true
          schema:
            type: string
            format: uuid
```

### Code Templates

Provide templates for common scenarios:

```typescript
// .github/knowledge-base/templates/react-component.tsx
import React from 'react';

interface ComponentNameProps {
  // Props
}

export const ComponentName: React.FC<ComponentNameProps> = (props) => {
  // Implementation
  return <div>{/* JSX */}</div>;
};
```

## Getting Started Checklist

- [ ] Review organization-level instructions in `.github/copilot-instructions.md`
- [ ] Read coding standards in `.github/prompts/coding-standards.md`
- [ ] Familiarize yourself with security guidelines
- [ ] Create repository-specific `.github/copilot-instructions.md`
- [ ] Add project-specific examples to `docs/examples/`
- [ ] Document architecture in `docs/architecture/`
- [ ] Create prompts for common tasks in your project
- [ ] Test Copilot suggestions with your knowledge base
- [ ] Gather team feedback and iterate

## Support

If you have questions or suggestions about the knowledge base:

1. Open an issue in this repository
2. Discuss in team meetings
3. Propose improvements via pull request
4. Share successful patterns with the team

## Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [GitHub Copilot for Business](https://docs.github.com/en/copilot/overview-of-github-copilot/about-github-copilot-for-business)
- [Copilot Best Practices](https://github.blog/2023-06-20-how-to-write-better-prompts-for-github-copilot/)

---

Remember: The knowledge base is only as good as we keep it. Contribute, update, and improve it regularly! 🚀
