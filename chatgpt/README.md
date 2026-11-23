# ClickClarity for ChatGPT

Packaging helpers for ChatGPT Custom GPTs / custom MCP plugins. Runtime is the same ClickClarity OAuth + tools API as Claude.

## Files

| File | Use |
|------|-----|
| `instructions.md` | Paste into Custom GPT **Instructions** |
| `openapi.example.json` | Shape reference — prefer live `{API}/plugin/openapi.json` |
| `shared-instructions.md` | Shared Co-Worker rules (ChatGPT + Claude) |

## Setup (production)

1. Enable feature toggle `ai_assistant_plugins`.
2. MCP / Actions base: `https://clickclarity.ai/api`
3. OAuth client id `chatgpt` with your client secret from `AI_PLUGIN_OAUTH_CLIENTS`.
4. Privacy URL: https://clickclarity.ai/privacy

See the repo root README for Claude directory submission (sibling folder `click-clarity-ai/`).
