---
name: review-changes
description: Review implementation quality across correctness, security, performance, accessibility, and tests.
argument-hint: "[change-summary-or-diff]"
agent: "Quality Reviewer"
---

Review these changes:

${input:change-summary-or-diff}

Provide:
1. Must-fix issues
2. Should-fix improvements
3. Nice-to-have refinements
4. Verification confidence and rationale

Focus on React + .NET fullstack quality and contract correctness.
