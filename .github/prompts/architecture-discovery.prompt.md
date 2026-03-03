---
name: architecture-discovery
description: Analyze current repository architecture and identify implementation boundaries, contracts, and risks before coding.
argument-hint: "[feature or problem statement]"
agent: "Architecture Planner"
---

Perform architecture discovery for:

${input:feature or problem statement}

Output:
- Current-state architecture map (frontend/backend/data)
- Proposed change boundaries
- API/data contract impact
- Risk list and sequencing recommendations
- Minimal implementation plan ready for handoff
