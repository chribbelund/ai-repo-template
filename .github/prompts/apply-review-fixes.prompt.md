---
name: apply-review-fixes
description: Apply fixes from review findings and re-validate changed scope.
argument-hint: "[review findings]"
agent: "Feature Implementer"
---

Apply fixes based on these review findings:

${input:review findings}

Requirements:
- Implement only fixes required by findings.
- Keep changes minimal and scoped.
- Run targeted validation checks.
- Summarize what was fixed and what remains.
