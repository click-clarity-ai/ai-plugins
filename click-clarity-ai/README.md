# Click Clarity AI for Claude

Connect Claude to your **ClickClarity** workspace with OAuth. Claude runs the conversation on Anthropic’s side; ClickClarity only supplies **read-only** analytics tools for the integrations you already connected (Meta Ads, Google Ads, GA4, Shopify, HubSpot, Change Intelligence, and related skills).

## What you get

- Remote MCP at `https://clickclarity.ai/api/plugin/mcp`
- Sign-in with your ClickClarity account and pick a workspace
- Live account metrics and diagnostics without giving Claude write access to ad platforms
- Optional analysis skills under `skills/` that tell Claude which MCP skill id to load first

## How to connect

1. Install this plugin (or add the MCP connector URL above in Claude settings).
2. Complete the OAuth consent screen and choose a workspace.
3. Ask about campaigns, creatives, traffic, or store performance for that workspace.

If a platform is not connected in ClickClarity, Claude will say so and continue with available sources.

## Privacy

ClickClarity does not store your Claude chat prompts or replies. Tool calls retrieve data from your workspace; see [Privacy Policy](https://clickclarity.ai/privacy) for retention of operational logs and execution traces.

## Support

- Product: [https://clickclarity.ai](https://clickclarity.ai)
- Email: support@clickclarity.ai

## Developer notes

Feature toggle `ai_assistant_plugins` must be enabled on the ClickClarity deployment. OAuth client id for Claude is `claude` (PKCE, no client secret). Dev MCP URL: `https://dev.clickclarity.ai/api/plugin/mcp`.
