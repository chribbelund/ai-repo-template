# AGENTS.md

Operational guide for coding agents in this repository.

## Project Intent

Template repository for fullstack development with React frontend and ASP.NET Core backend.

## Default Workflow

1. Discover relevant files and architecture boundaries.
2. Create a short plan for non-trivial tasks.
3. Implement minimal scoped changes.
4. Run targeted checks, then broader checks.
5. Summarize what changed and how it was verified.

## Quality Gates

- No unrelated file churn.
- Contract fidelity across frontend/backend.
- Tests updated for changed behavior.
- Security, performance, and accessibility considered for relevant changes.

## Common Commands (adapt as project evolves)

Backend:
- `dotnet restore`
- `dotnet build`
- `dotnet test`

Frontend:
- `npm install`
- `npm run build`
- `npm test`
- `npm run lint`

## Multi-Agent Parallel Workflow (Worktrees)

Use VS Code Tasks (Terminal -> Run Task) with built-in `git worktree`:

- `worktree:create-multi-agent` — creates planner/implementer/tester branches and worktrees under `.worktrees/<feature>/`
- `worktree:list` — lists all worktrees
- `worktree:status-multi-agent` — shows status for planner/implementer/tester worktrees
- `worktree:remove-multi-agent-safe` — removes cleanly merged worktrees/branches
- `worktree:remove-multi-agent-force` — force-removes worktrees/branches

Recommended branch naming is automatic in tasks:

- `feature/<feature>/planner`
- `feature/<feature>/implementer`
- `feature/<feature>/tester`

Suggested role mapping:

- planner worktree -> `Architecture Planner`
- implementer worktree -> `Feature Implementer`
- tester worktree -> `Feature Tester`
- any worktree as needed -> `Quality Reviewer`

## Repo Conventions

- Keep API contracts explicit and typed.
- Keep controllers thin and logic in services.
- Keep React components composable and state transitions explicit.
- Use structured logs and safe error contracts.

## Handoff Format

- Scope completed
- Files changed
- Verification run and outcomes
- Open risks / follow-up items
