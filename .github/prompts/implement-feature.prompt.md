---
name: implement-feature
description: Implement a planned feature with minimal churn and strong verification.
argument-hint: "[implementation-plan]"
agent: "Feature Implementer"
---

Implement this approved plan:

${input:implementation-plan}

Requirements:
- Make targeted, minimal code changes.
- Keep API contracts and frontend types aligned.
- Add/update tests for changed behavior.
- Run relevant checks and summarize outcomes.
- Report changed files, rationale, and follow-ups.
- Prefer GPT-5.3-Codex when model selection is available.

Do not perform unrelated refactors.
