---
name: plan-feature
description: Plan a fullstack React + .NET feature with contracts, phased steps, and validation.
argument-hint: "[feature-request]"
agent: "Architecture Planner"
---

Create an implementation plan for this feature:

${input:feature-request}

Requirements:
- Define frontend/backend scope and boundaries.
- Propose API request/response and error contracts.
- Provide phased implementation steps in order.
- Include migration/data concerns if needed.
- Include validation commands and expected outcomes.
- Include risks, mitigations, and rollback plan.
- Prefer GPT-5.3-Codex when model selection is available.

Output in concise markdown with checklists.
