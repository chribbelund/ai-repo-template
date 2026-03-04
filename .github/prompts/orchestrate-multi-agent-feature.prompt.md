---
name: orchestrate-multi-agent-feature
description: Coordinate a full feature lifecycle across planner, implementer, tester, and reviewer agents using parallel worktrees.
argument-hint: "[feature request]"
agent: "Multi-Agent Coordinator"
---

Orchestrate this feature across multiple agents and worktrees:

${input:feature request}

Requirements:
- Use `/fleet` to decompose independent subtasks and run them in parallel.
- Prefer GPT-5.3-Codex for coding subtasks whenever model selection is available.
- Confirm worktree setup (`planner`, `implementer`, `tester`) for feature branch set.
- Run sequence: plan -> implement -> test -> review.
- Capture outputs and decisions from each role.
- Surface blockers and recommended next action.
- End with merge readiness summary.
