# Repository Agentic Instructions (React + .NET)

This repository is a template for fullstack development with React (frontend) and ASP.NET Core C# (backend).

## Global Priorities

- Prefer minimal, reversible changes over broad refactors.
- Keep contracts explicit and typed across API boundaries.
- Preserve existing style and project conventions when present.
- Fix root causes; avoid superficial patches.
- Validate changes with targeted tests before broad test runs.

## Working Model

1. Discover architecture and relevant files before editing.
2. Propose a short execution plan for non-trivial tasks.
3. Implement in small, reviewable steps.
4. Run build/lint/test checks and report outcomes.
5. Document assumptions, tradeoffs, and follow-up tasks.

## Code Quality Baseline

- Security: validate inputs, protect secrets, least privilege access.
- Reliability: explicit error handling and predictable fallbacks.
- Observability: structured logs and actionable diagnostics.
- Performance: avoid unnecessary allocations/queries/renders.
- Accessibility: keyboard support, semantic markup, contrast-safe UI.

## Fullstack Contract Discipline

- Treat backend API contract as source of truth.
- Keep frontend types aligned with backend response models.
- Ensure auth and validation behavior are consistent end-to-end.
- Cover happy path + failure path in both layers.

## Definition of Done

- Code compiles and checks pass for modified scope.
- Tests for changed behavior are added/updated.
- No unrelated file churn.
- Notes include what changed, why, and how it was verified.
