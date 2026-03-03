---
applyTo: "**/*test*.*,**/*.spec.*,**/*.test.*"
---
# Testing Rules

- Test behavior, not implementation details.
- Prefer deterministic tests over timing-sensitive patterns.
- Keep Arrange-Act-Assert clear and concise.
- Cover happy path, edge cases, and expected failures.
- Use descriptive test names that read like scenarios.

## Fullstack Focus

- Backend: validate status codes, error contracts, and authorization outcomes.
- Frontend: validate user interactions, state transitions, and accessibility-critical behavior.
