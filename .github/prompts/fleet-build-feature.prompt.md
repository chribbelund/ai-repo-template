---
name: fleet-build-feature
description: Use /fleet to decompose and execute a feature in parallel across specialized agents.
argument-hint: "[feature request]"
---

/fleet ${input:feature request}

Decompose and execute this feature across specialized subagents in parallel where dependencies allow:

- Use the **Architecture Planner** agent to define API contracts, boundaries, and a phased implementation plan.
- Use the **Feature Implementer** agent to build backend (.NET) and frontend (React) changes per the approved plan.
- Use the **Feature Tester** agent to run targeted tests, triage failures, and confirm coverage.
- Use the **Quality Reviewer** agent to check correctness, security, performance, and accessibility.

Apply quality gates throughout:
- API contract fidelity across frontend and backend.
- Tests updated for all changed behavior.
- No unrelated file churn.
- Security, performance, and accessibility validated before merge.
