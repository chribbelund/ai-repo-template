---
name: fullstack-react-dotnet
description: Orchestrate fullstack implementation across React frontend and ASP.NET Core backend with aligned API contracts, auth flows, validation, testing, and deployment readiness. Use when delivering end-to-end features.
---

# Fullstack React + .NET Skill

Use this skill for end-to-end feature delivery that touches both frontend and backend.

## When to Use This Skill

- New business feature spanning UI, API, and data storage
- API contract change that impacts frontend behavior
- Authentication/authorization flow across client and server
- End-to-end bug fixes crossing multiple layers

## Execution Plan

1. Define feature contract first (request/response schema + error model)
2. Implement backend endpoint/service/data changes with tests
3. Implement frontend UI + data integration + state/error handling
4. Validate auth and permission boundaries across both layers
5. Run targeted backend/frontend tests and key user-flow checks
6. Confirm non-functional criteria (perf, accessibility, observability)

## Coordination Rules

- Treat API contract as source of truth.
- Keep versioning/backward compatibility explicit.
- Include consistent correlation IDs/log context across layers.
- Ensure UI and API share validation semantics where possible.
- Add at least one end-to-end acceptance path in test coverage.

## Release Readiness

- Feature flags or safe rollout strategy for risky changes
- Migrations are reversible or have rollback guidance
- Monitoring/alerts updated for new critical flows

## References

- [Fullstack delivery checklist](references/fullstack-delivery-checklist.md)
