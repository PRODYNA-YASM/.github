# Code Review Guidelines - PRODYNA-YASM

This document outlines the code review process and best practices for the YASM project. Effective code reviews are essential for maintaining code quality, sharing knowledge, and preventing bugs.

## Code Review Philosophy

Code reviews are:
- **Collaborative**, not confrontational
- **Educational** for both reviewer and author
- **Quality gates** that protect our codebase
- **Knowledge sharing** opportunities
- **Team building** exercises

Code reviews are NOT:
- Personal criticism
- Gatekeeping mechanisms
- Opportunities to show superiority
- Excuses to delay important work

## Responsibilities

### As a Code Author

#### Before Requesting Review

- [ ] **Self-review your code**: Review your own changes first as if you were the reviewer
- [ ] **Run all tests**: Ensure all tests pass locally
- [ ] **Run linters**: Fix all linting issues
- [ ] **Update documentation**: Update README, API docs, and comments as needed
- [ ] **Keep changes focused**: Each PR should address one logical change
- [ ] **Write a clear description**: Explain what, why, and how
- [ ] **Add tests**: Include unit tests for new functionality
- [ ] **Check for secrets**: Ensure no credentials or sensitive data are committed

#### Writing PR Descriptions

A good PR description includes:

```markdown
## What
Brief description of the changes made.

## Why
Explanation of why this change is necessary. Link to related issues/tickets.

## How
Technical explanation of how the change works.

## Testing
- [ ] Unit tests added/updated
- [ ] Integration tests pass
- [ ] Manual testing performed (describe what you tested)

## Screenshots (if UI changes)
Before: [image]
After: [image]

## Checklist
- [ ] Code follows style guidelines
- [ ] Self-reviewed the code
- [ ] Commented complex parts
- [ ] Updated documentation
- [ ] No new warnings
- [ ] Tests pass locally
- [ ] Dependent changes merged
```

#### During Review

- [ ] **Respond promptly** to feedback (within 24 hours)
- [ ] **Be open to feedback**: Don't take it personally
- [ ] **Ask questions** if feedback is unclear
- [ ] **Explain your reasoning** if you disagree
- [ ] **Mark conversations** as resolved when addressed
- [ ] **Push updates** quickly to keep the review moving

#### After Approval

- [ ] **Merge promptly** after approval
- [ ] **Delete the branch** after merging
- [ ] **Monitor** the deployment for any issues
- [ ] **Follow up** on any post-merge comments

### As a Code Reviewer

#### General Guidelines

- [ ] **Review within 24 hours** of the request
- [ ] **Be respectful and constructive** in all feedback
- [ ] **Explain the "why"** behind your suggestions
- [ ] **Distinguish between** must-fix issues and nice-to-have suggestions
- [ ] **Approve when ready**: Don't approve with major concerns
- [ ] **Test the changes** when appropriate

#### Review Checklist

##### Functionality
- [ ] Does the code do what it's supposed to do?
- [ ] Are edge cases handled appropriately?
- [ ] Are there any obvious bugs or logic errors?
- [ ] Is error handling comprehensive and appropriate?

##### Code Quality
- [ ] Is the code readable and self-documenting?
- [ ] Are variable and function names clear and descriptive?
- [ ] Is the code properly formatted according to style guides?
- [ ] Are there any code smells (long functions, deep nesting, etc.)?
- [ ] Is the code DRY (not repeating logic)?

##### Testing
- [ ] Are there adequate unit tests?
- [ ] Do tests cover edge cases and error conditions?
- [ ] Are tests meaningful and not just for coverage?
- [ ] Do all tests pass?

##### Security
- [ ] Are user inputs validated and sanitized?
- [ ] Are there any SQL injection vulnerabilities?
- [ ] Are credentials or secrets hardcoded?
- [ ] Are authentication and authorization implemented correctly?
- [ ] Are dependencies from trusted sources?

##### Performance
- [ ] Are there any obvious performance issues?
- [ ] Are database queries optimized?
- [ ] Is caching used appropriately?
- [ ] Are there any memory leaks?

##### Documentation
- [ ] Is the code adequately commented?
- [ ] Are complex algorithms explained?
- [ ] Is API documentation updated?
- [ ] Are README files current?

#### Providing Feedback

##### Use Clear Communication

**Good feedback:**
```
Consider extracting this into a separate function for better testability:

function validateAndSaveUser(userData) {
  const errors = validateUser(userData);
  if (errors.length > 0) {
    return { success: false, errors };
  }
  return saveUser(userData);
}

This would allow you to test validation logic independently.
```

**Poor feedback:**
```
This is wrong.
```

##### Use Conventional Comments

Use prefixes to clarify the intent of your comment:

- **nitpick:** (or `nit:`) Minor style suggestion that doesn't affect functionality
- **suggestion:** Improvement idea but not required
- **question:** Asking for clarification
- **issue:** Problem that should be fixed
- **security:** Security-related concern
- **performance:** Performance-related concern
- **thought:** Sharing an idea or alternative approach

Examples:
```
nitpick: Consider using const instead of let here since the value doesn't change.

suggestion: You might want to consider using a Map instead of an object for O(1) lookups.

question: What happens if the user is null here?

issue: This will throw an error if the array is empty. Please add a check.

security: This input should be sanitized before being used in the database query.

performance: This loop could be replaced with a single database query to reduce N+1 queries.
```

##### Positive Feedback

Don't forget to highlight good things:
```
✨ Nice refactoring! This is much more readable than before.

👍 Great test coverage for edge cases.

💡 Clever solution to avoid the race condition!
```

## Review Size and Timing

### Optimal PR Size

- **Small PRs** (< 200 lines): Ideal, easy to review thoroughly
- **Medium PRs** (200-500 lines): Acceptable, may need more time
- **Large PRs** (> 500 lines): Should be split when possible

### When to Split PRs

Split large PRs into smaller ones when:
- Changes are logically independent
- Refactoring can be separated from feature work
- Multiple files/modules can be updated independently

Exception: Don't split if it would leave the codebase in a broken state.

### Review Turnaround Time

- **Initial response**: Within 24 hours
- **Full review**: Within 48 hours
- **Follow-up reviews**: Within 24 hours
- **Urgent fixes**: Same day

## Common Review Scenarios

### Scenario 1: Too Many Changes

**Reviewer:**
```
This PR includes refactoring, bug fixes, and a new feature. Could you split this into:
1. Refactoring changes
2. Bug fix
3. New feature

This will make review easier and allow us to deploy changes independently.
```

### Scenario 2: Missing Tests

**Reviewer:**
```
issue: I don't see tests for the new error handling logic. Could you add tests covering:
- Invalid input
- Network timeout
- Partial failure scenarios
```

### Scenario 3: Security Concern

**Reviewer:**
```
security: This user input is being directly interpolated into the SQL query. This creates a SQL injection vulnerability. Please use parameterized queries instead:

const query = 'SELECT * FROM users WHERE email = ?';
db.query(query, [userEmail]);
```

### Scenario 4: Disagreement

**Author:**
```
I understand your concern about performance, but premature optimization can make the code harder to maintain. The current approach handles our expected load, and we can optimize later if needed. What do you think?
```

**Reviewer:**
```
That's a fair point. Let's go with the current approach but add a TODO comment to revisit if we see performance issues.
```

## Language-Specific Review Points

### TypeScript Reviews

- [ ] Type safety: No `any` types without justification
- [ ] Proper use of React hooks (dependencies, cleanup)
- [ ] Props interfaces defined for all components
- [ ] Proper error boundaries for components
- [ ] Accessibility: ARIA labels, keyboard navigation
- [ ] No console.log in production code

### Java/Quarkus Reviews

- [ ] Reactive types used correctly (Uni, Multi)
- [ ] Proper dependency injection (@Inject, scopes)
- [ ] Exception handling with proper types
- [ ] RESTful API design (proper HTTP methods and status codes)
- [ ] Transaction boundaries defined correctly
- [ ] Null safety (Optional usage)

### Go Reviews

- [ ] Errors properly handled (no ignored errors)
- [ ] Context propagation for cancellation
- [ ] Proper use of goroutines and channels
- [ ] No goroutine leaks
- [ ] Deferred cleanup (defer close())
- [ ] Exported functions have documentation
- [ ] Table-driven tests where appropriate

## Anti-Patterns to Watch For

### Code Smells

```javascript
// ❌ God object - too many responsibilities
class UserManager {
  validateUser() {}
  saveUser() {}
  sendEmail() {}
  generateReport() {}
  processPayment() {}
}

// ✅ Single Responsibility Principle
class UserValidator {}
class UserRepository {}
class EmailService {}
class ReportGenerator {}
class PaymentProcessor {}
```

```java
// ❌ Overly complex conditionals
if (user != null && user.isActive() && user.hasPermission("admin") && 
    !user.isLocked() && user.getLastLogin() != null) {
  // do something
}

// ✅ Extract to well-named method
if (canAccessAdminPanel(user)) {
  // do something
}
```

```go
// ❌ Ignored errors
data, _ := fetchData()

// ✅ Proper error handling
data, err := fetchData()
if err != nil {
    return fmt.Errorf("failed to fetch data: %w", err)
}
```

## Automation and Tools

### Automated Checks

Before manual review, ensure these automated checks pass:
- [ ] Linting (ESLint, Checkstyle, golangci-lint)
- [ ] Unit tests
- [ ] Integration tests
- [ ] Code coverage meets threshold
- [ ] Security scanning (Dependabot, CodeQL)
- [ ] Build succeeds

### Useful Tools

- **GitHub Suggestions**: Use the suggestion feature for code changes
- **CodeQL**: For security vulnerability detection
- **Copilot**: For code explanation and review assistance
- **SonarQube**: For code quality metrics

## Metrics and Goals

### Team Metrics to Track

- Average time to first review
- Average time to merge
- Number of review iterations
- PR size distribution
- Test coverage trends

### Individual Goals

- Review at least as many PRs as you create
- Provide constructive feedback on 100% of reviews
- Respond to all feedback within 24 hours

## Conflict Resolution

### When Reviewer and Author Disagree

1. **Have a discussion**: Comment on the PR, explain perspectives
2. **Involve a third party**: Ask another team member for input
3. **Escalate if needed**: Bring to tech lead or team meeting
4. **Document the decision**: Add a comment explaining the final choice

### When to Override a Reviewer

Very rarely. Only if:
- The concern is clearly out of scope
- There's unanimous agreement from other reviewers
- The issue is blocking critical work and can be addressed later

## Special Cases

### Emergency Hotfixes

For critical production issues:
1. Create the fix
2. Get expedited review (same day)
3. Deploy immediately after approval
4. Create follow-up issue for additional testing/refactoring

### Dependency Updates

- Review the changelog for breaking changes
- Check for security vulnerabilities
- Verify compatibility with our codebase
- Run the full test suite

### Infrastructure Changes

- Review for security implications
- Check resource limits and quotas
- Verify rollback procedures
- Test in staging environment first

## Learning from Reviews

### For Authors

- **Track patterns**: If you get similar feedback repeatedly, learn from it
- **Ask questions**: Use reviews as learning opportunities
- **Share knowledge**: If you learned something, document it

### For Reviewers

- **Be consistent**: Apply the same standards to all code
- **Stay current**: Keep up with best practices and new patterns
- **Give context**: Explain not just what, but why

## Templates

### PR Template

Create `.github/pull_request_template.md`:

```markdown
## Description
<!-- Describe your changes -->

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
- [ ] Unit tests pass
- [ ] Integration tests pass
- [ ] Manual testing completed

## Screenshots
<!-- If applicable -->

## Checklist
- [ ] Code follows style guidelines
- [ ] Self-reviewed my code
- [ ] Commented complex code
- [ ] Updated documentation
- [ ] No new warnings
- [ ] Added tests
```

### Review Comment Templates

Save these as GitHub saved replies:

**Request changes:**
```
Thanks for the PR! I've left some comments that need to be addressed before we can merge. Please take a look and let me know if you have questions.
```

**Approval:**
```
LGTM! 🚀 Great work on this feature. The tests look comprehensive and the code is clean.
```

**Needs discussion:**
```
I have some architectural concerns about this approach. Could we discuss this in our next team meeting before proceeding?
```

## Conclusion

Effective code reviews require:
- **Mutual respect** between authors and reviewers
- **Clear communication** about expectations and concerns
- **Consistent standards** applied fairly
- **Timely feedback** to keep work flowing
- **Continuous learning** from each review

Remember: The goal is to ship quality code, not to be right. Work together to find the best solution.
