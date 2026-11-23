# ClickClarity for ChatGPT

Public **plugin directory** package (MCP + skills) plus older Custom GPT helpers.

## Directory submission package

Folder: [`click-clarity-ai/`](./click-clarity-ai/)  
ZIP: [`click-clarity-ai.zip`](./click-clarity-ai.zip) (regenerate after edits)

```text
click-clarity-ai/
├── plugin.json          # name/version + OpenAI listing (extensions.com.openai)
├── mcp.json             # production MCP URL + OAuth (no secrets)
├── assets/logo.png
└── skills/…/SKILL.md
```

### Important: ignore the local “app ID” step for public submit

ChatGPT / Plugin Creator may ask you to point at a `plugin_asdk_app…` ID from **Add custom MCP**. That ID is for **local testing only**.

For **directory upload**, the ZIP must declare the **public HTTPS MCP** in `mcp.json` (already set to `https://clickclarity.ai/api/plugin/mcp`). **Do not** include `.app.json` in the submission ZIP.

### Upload steps

1. Open [OpenAI Plugins](https://chatgpt.com/) → Plugins → **Upload new or existing plugin** (org with Apps Management Write + verified publisher).
2. Upload `chatgpt/click-clarity-ai.zip`.
3. Fix any **Metadata & Skills** findings; re-ZIP and re-upload if needed.
4. Open **MCPs** → Connect `clickclarity` → complete domain verification + OAuth (client secret stays in the dashboard, not the ZIP).
5. Resolve tool-scan issues, add review cases / video / reviewer account, then **Submit for review**.

OAuth client id in prod: `chatgpt` (secret from `AI_PLUGIN_OAUTH_CLIENTS`).  
Privacy: https://clickclarity.ai/privacy · Terms: https://clickclarity.ai/terms

### Regenerate the ZIP (PowerShell)

```powershell
cd chatgpt
Remove-Item .\click-clarity-ai.zip -ErrorAction SilentlyContinue
Compress-Archive -Path .\click-clarity-ai\* -DestinationPath .\click-clarity-ai.zip
```

## Custom GPT helpers (legacy)

| File | Use |
|------|-----|
| `instructions.md` | Paste into Custom GPT **Instructions** |
| `openapi.example.json` | Shape reference — prefer live `{API}/plugin/openapi.json` |
| `shared-instructions.md` | Shared Co-Worker rules |

Setup: feature toggle `ai_assistant_plugins`; API base `https://clickclarity.ai/api`.
