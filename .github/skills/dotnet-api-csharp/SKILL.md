---
name: dotnet-api-csharp
description: Build and evolve ASP.NET Core Web APIs in C# for production. Use when creating endpoints, application services, EF Core data access, authentication/authorization, validation, logging, testing, and performance hardening in .NET backend code.
---

# .NET API (C#) Skill

Use this skill for backend work in ASP.NET Core and C#.

## When to Use This Skill

- Creating or updating ASP.NET Core APIs (controllers or minimal APIs)
- Implementing business logic in services and clean boundaries
- Working with EF Core, migrations, and query performance
- Adding authN/authZ, validation, error handling, and observability
- Writing backend unit/integration tests for reliable changes

## Prerequisites

- Use the project’s existing .NET SDK and solution structure
- Prefer existing architecture conventions over introducing new patterns
- Validate by running local build/tests before finalizing

## Workflow

1. Discover architecture boundaries (`Api`, `Application`, `Domain`, `Infrastructure`, etc.)
2. Implement feature with clear contracts (DTOs, interfaces, typed responses)
3. Add validation and consistent error mapping (400/401/403/404/409/422/500)
4. Add/update persistence with EF Core patterns used by the repo
5. Add tests (unit + integration where applicable)
6. Verify build, tests, and static checks pass

## Implementation Rules

- Prefer async all the way; avoid sync-over-async.
- Use DI with proper lifetimes (`Singleton`, `Scoped`, `Transient`).
- Keep controllers/endpoints thin; move logic to application services.
- Use `CancellationToken` on I/O-bound operations.
- Use structured logging with correlation/trace context.
- Never expose secrets; use environment/config providers.
- Avoid broad `catch (Exception)` unless converting to known API error contract.
- Keep API contracts stable and versioned when introducing breaking changes.

## Data and EF Core Guidance

- Use explicit projections for read paths; avoid over-fetching.
- Use `AsNoTracking()` for read-only queries.
- Keep migrations small and reviewable.
- Prefer idempotent, transactional write flows.
- Prevent N+1 query patterns and unbounded result sets.

## Security and Reliability

- Validate all inbound DTOs.
- Enforce authorization policies close to endpoints.
- Use rate limiting and input-size safeguards for public endpoints when applicable.
- Return safe error payloads; don’t leak internals.

## Testing Expectations

- Unit-test business logic and edge cases.
- Integration-test endpoint contracts and auth behavior.
- Cover failure paths (validation, not found, conflict, forbidden).

## References

- [Backend checklist](references/backend-checklist.md)
- [API error contract](references/api-error-contract.md)
