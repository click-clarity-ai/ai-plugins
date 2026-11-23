---
name: marketing-audit
description: Marketing audit. Use when Broad account health or audit-style reviews.
---

# Marketing audit

Use this skill when Broad account health or audit-style reviews.

## Required first step

Call the ClickClarity MCP tool `get_agent_analysis_skill` with:

```json
{ "skill_id": "marketing-audit" }
```

Follow the returned playbook before a long tool loop. Prefer evidence from live tools; do not invent metrics. Stay read-only.
