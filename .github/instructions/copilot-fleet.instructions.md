---
applyTo: ".github/agents/*.md,.github/prompts/*.md"
---
# Copilot Fleet + Model Routing Rules

- For agent and prompt files, explicitly state "Prefer GPT-5.3-Codex when model selection is available."
- If model frontmatter is supported in your environment, keep `gpt-5.3-codex` first and include fallbacks.
- For orchestration prompts/agents that coordinate multiple roles, instruct use of `/fleet` when subtasks are independent.
- Keep orchestration deterministic: decompose work, assign per-role subtasks, then aggregate outputs into one status summary.
- Preserve existing agent names and workflow handoffs unless explicitly changing workflow design.
