---
applyTo: "**/*.cs,**/*.csproj,**/*.sln"
---
# .NET / C# Rules

- Use async/await end-to-end for I/O operations.
- Keep API endpoints/controllers thin; move logic to services.
- Use dependency injection and correct service lifetimes.
- Propagate `CancellationToken` for long-running/remote operations.
- Validate request models and return consistent problem details for errors.
- Prefer explicit DTOs over exposing domain entities.

## Data Access

- Use `AsNoTracking()` for read-only queries.
- Avoid N+1 query patterns and unbounded result sets.
- Keep migrations small and deterministic.

## Tests

- Add unit tests for business logic.
- Add integration tests for endpoint contract and auth behavior where relevant.
