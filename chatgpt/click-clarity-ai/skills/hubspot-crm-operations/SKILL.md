---
name: hubspot-crm-operations
description: HubSpot CRM operations. Use when CRM contacts, companies, or deals reads.
---

# HubSpot CRM operations

Use this skill when CRM contacts, companies, or deals reads.

## Required first step

Call the ClickClarity MCP tool `get_agent_analysis_skill` with:

```json
{ "skill_id": "hubspot-crm-operations" }
```

Follow the returned playbook before a long tool loop. Prefer evidence from live tools; do not invent metrics. Stay read-only.
