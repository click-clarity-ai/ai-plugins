---
name: ga4-analysis
description: GA4 analysis. Use when Site traffic, sessions, or GA4 reports.
---

# GA4 analysis

Use this skill when Site traffic, sessions, or GA4 reports.

## Required first step

Call the ClickClarity MCP tool `get_agent_analysis_skill` with:

```json
{ "skill_id": "ga4-analysis" }
```

Follow the returned playbook before a long tool loop. Prefer evidence from live tools; do not invent metrics. Stay read-only.
