---
name: shopify-commerce-analysis
description: Shopify commerce analysis. Use when Store revenue, products, or Shopify KPIs.
---

# Shopify commerce analysis

Use this skill when Store revenue, products, or Shopify KPIs.

## Required first step

Call the ClickClarity MCP tool `get_agent_analysis_skill` with:

```json
{ "skill_id": "shopify-commerce-analysis" }
```

Follow the returned playbook before a long tool loop. Prefer evidence from live tools; do not invent metrics. Stay read-only.
