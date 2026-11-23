---
name: competitor-ad-research
description: Competitor ad research. Use when Ad Library or competitor creative research.
---

# Competitor ad research

Use this skill when Ad Library or competitor creative research.

## Required first step

Call the ClickClarity MCP tool `get_agent_analysis_skill` with:

```json
{ "skill_id": "competitor-ad-research" }
```

Follow the returned playbook before a long tool loop. Prefer evidence from live tools; do not invent metrics. Stay read-only.
