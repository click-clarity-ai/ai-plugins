---
name: ad-account-changes
description: Ad account changes. Use when Recent Meta or Google Ads change history.
---

# Ad account changes

Use this skill when Recent Meta or Google Ads change history.

## Required first step

Call the ClickClarity MCP tool `get_agent_analysis_skill` with:

```json
{ "skill_id": "ad-account-changes" }
```

Follow the returned playbook before a long tool loop. Prefer evidence from live tools; do not invent metrics. Stay read-only.
