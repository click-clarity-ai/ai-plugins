# ClickClarity AI — assistant plugins

Public packaging for **Claude** (plugin directory) and **ChatGPT** (Custom GPT / MCP).

Runtime OAuth and tools are hosted by ClickClarity (`https://clickclarity.ai/api/plugin/*`). This repository only ships connector metadata, instructions, and skills—no secrets.

| Path | Purpose |
|------|---------|
| [`click-clarity-ai/`](./click-clarity-ai/) | Claude plugin bundle (submit this folder to [claude.ai/directory/manage](https://claude.ai/directory/manage)) |
| [`chatgpt/`](./chatgpt/) | ChatGPT directory ZIP (`click-clarity-ai.zip`) + Custom GPT helpers |

## Claude directory submission

1. Repo must be **public** before the listing goes live.
2. Submit **Plugin bundle** with:
   - Repository: `click-clarity-ai/ai-plugins`
   - Plugin path: `click-clarity-ai`
3. Also submit the remote MCP server as an **MCP connector** pointing at `https://clickclarity.ai/api/plugin/mcp` (OAuth).
4. Privacy: https://clickclarity.ai/privacy

```bash
claude plugin validate ./click-clarity-ai
```

## ChatGPT plugin directory submission

1. Upload [`chatgpt/click-clarity-ai.zip`](./chatgpt/click-clarity-ai.zip) in the OpenAI Plugins dashboard (**Upload new or existing plugin**).
2. Connect MCP `https://clickclarity.ai/api/plugin/mcp` (OAuth client id `chatgpt`; secret only in the dashboard).
3. Do **not** put a `plugin_asdk_app…` local app ID in the public ZIP — that ID is for Plugin Creator / local testing only.

Details: [`chatgpt/README.md`](./chatgpt/README.md).

## Local monorepo checkout

This folder is a separate git clone under the ClickClarity workspace root (`plugins/`). It is not part of the backend/frontend remotes.
