---
name: meta-ads-diagnostic
description: Meta Ads diagnostic. Use when Meta creative, video, hook rate, ThruPlay, or learning-phase questions.
---

# Meta Ads diagnostic

Use this skill when Meta creative, video, hook rate, ThruPlay, or learning-phase questions.

## Required first step

Call the ClickClarity MCP tool `get_agent_analysis_skill` with:

```json
{ "skill_id": "meta-ads-diagnostic" }
```

Follow the returned playbook before a long tool loop. Prefer evidence from live tools; do not invent metrics. Stay read-only.
