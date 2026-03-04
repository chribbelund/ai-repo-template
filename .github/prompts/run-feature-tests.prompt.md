---
name: run-feature-tests
description: Execute targeted validation for a feature and report failures with root-cause hypotheses.
argument-hint: "[feature scope or changed files]"
agent: "Feature Tester"
---

Test this feature scope:

${input:feature scope or changed files}

Requirements:
- Start with smallest relevant checks.
- Expand to broader suite only after targeted checks.
- Report exact failing tests and likely root causes.
- Suggest minimal fix strategy if failures are present.
- Prefer GPT-5.3-Codex when model selection is available.
