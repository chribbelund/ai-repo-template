# Agentic Development Template (React + .NET)

This `.github` folder is a production-grade baseline for agentic software development with GitHub Copilot.

## Included Primitives

- `copilot-instructions.md` — repository-wide behavior and quality baseline
- `instructions/*.instructions.md` — path-specific coding rules
- `agents/*.agent.md` — specialist personas for planning, implementation, and review
- `prompts/*.prompt.md` — reusable task workflows
- `skills/*/SKILL.md` — on-demand domain capabilities with references
- `workflows/copilot-setup-steps.yml` — deterministic environment bootstrap for coding agents

## Recommended Usage Pattern

1. Start with `/plan-feature` to define scope and contracts.
2. Execute with `/implement-feature`.
3. Run `/run-feature-tests` (or `/test-and-fix`) for stabilization.
4. Validate quality with `/review-changes`.

For full orchestration, run `/orchestrate-multi-agent-feature` with the `Multi-Agent Coordinator` agent.

## Parallel Multi-Agent Setup (VS Code + Git Worktree)

This template uses native `git worktree` via VS Code tasks in `.vscode/tasks.json`.

- Run `worktree:create-multi-agent` to create isolated planner/implementer/tester worktrees for a feature.
- Open each worktree in its own VS Code window and run different agents in parallel.
- Use `worktree:status-multi-agent` to track branch state quickly.
- Clean up with `worktree:remove-multi-agent-safe` (or force variant if needed).

## Folder Structure

- `.github/instructions/`
  - `general.instructions.md`
  - `dotnet.instructions.md`
  - `react.instructions.md`
  - `testing.instructions.md`
  - `security.instructions.md`
  - `documentation.instructions.md`
- `.github/agents/`
  - `architect.agent.md`
  - `implementer.agent.md`
  - `tester.agent.md`
  - `reviewer.agent.md`
  - `multi-agent-coordinator.agent.md`
- `.github/prompts/`
  - `plan-feature.prompt.md`
  - `implement-feature.prompt.md`
  - `run-feature-tests.prompt.md`
  - `test-and-fix.prompt.md`
  - `review-changes.prompt.md`
  - `orchestrate-multi-agent-feature.prompt.md`
- `.github/skills/`
  - `dotnet-api-csharp/`
  - `react-frontend-modern/`
  - `modern-ui-ux-web/`
  - `fullstack-react-dotnet/`

## Customization Checklist

- Align runtime versions in `copilot-setup-steps.yml` with your project.
- Add real build/test/lint commands once app code exists.
- Expand skill references with team standards and examples.
- Keep instructions short, specific, and conflict-free.
- Review all generated outputs before merge.
