---
name: test-and-fix
description: Run targeted tests, diagnose failures, and apply minimal fixes.
argument-hint: "[failing-area]"
agent: "Feature Implementer"
---

Execute a test-first fix cycle for:

${input:failing-area}

Requirements:
- Run the smallest relevant test/lint/build command first.
- Diagnose root cause from outputs and code.
- Apply minimal fix for the actual cause.
- Re-run the same checks, then broader checks as needed.
- Summarize failures found, fixes made, and current status.
- Prefer GPT-5.3-Codex when model selection is available.

Do not fix unrelated failures.
