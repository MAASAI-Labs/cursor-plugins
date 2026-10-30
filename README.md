# MAASAI Labs plugins for Cursor

Ten free, open-source (MIT) plugins from MAASAI Labs. Each one connects Cursor to a hosted remote MCP server. There is nothing to install locally and no account with us is needed.

| Plugin | Name | Credentials | Server code |
|---|---|---|---|
| [SAFE & Cap Table Calculator](plugins/safe-cap-table-mcp) | `safe-cap-table-mcp` | None | [source](https://github.com/MAASAI-Labs/safe-cap-table-mcp) |
| [Space Launch & Starlink Tracker](plugins/space-launch-tracker-mcp) | `space-launch-tracker-mcp` | None | [source](https://github.com/MAASAI-Labs/space-launch-tracker-mcp) |
| [Orbital Watch](plugins/orbital-watch-mcp) | `orbital-watch-mcp` | None | [source](https://github.com/MAASAI-Labs/orbital-watch-mcp) |
| [Breach Radar](plugins/breach-radar-mcp) | `breach-radar-mcp` | Optional server-side HIBP key (operator) | [source](https://github.com/MAASAI-Labs/breach-radar-mcp) |
| [Chip Intel](plugins/chip-intel-mcp) | `chip-intel-mcp` | None | [source](https://github.com/MAASAI-Labs/chip-intel-mcp) |
| [WhatsApp Community Manager](plugins/whatsapp-community-mcp) | `whatsapp-community-mcp` | Optional, your own keys | [source](https://github.com/MAASAI-Labs/whatsapp-community-mcp) |
| [Call Anyone in Any Language](plugins/call-anyone-mcp) | `call-anyone-mcp` | Optional, your own keys | [source](https://github.com/MAASAI-Labs/call-anyone-mcp) |
| [Prediction Market Odds](plugins/prediction-odds-mcp) | `prediction-odds-mcp` | None | [source](https://github.com/MAASAI-Labs/prediction-odds-mcp) |
| [X Marketplace Seller](plugins/x-marketplace-seller-mcp) | `x-marketplace-seller-mcp` | Optional, your own keys | [source](https://github.com/MAASAI-Labs/x-marketplace-seller-mcp) |
| [Domain Hunter](plugins/domain-hunter-mcp) | `domain-hunter-mcp` | None | [source](https://github.com/MAASAI-Labs/domain-hunter-mcp) |

## Install in Cursor

**From the Cursor Marketplace (once approved):**

1. Open the Cursor Marketplace at https://cursor.com/marketplace and search for "MAASAI Labs", or the plugin's name.
2. Click **Install**.
3. For WhatsApp Community Manager, Call Anyone or X Marketplace Seller, open **Plugins**, then **Configure**, and add your own keys if you want the tools that post, message or call. Everything else works with no setup.
4. Check the server shows as enabled under Cursor Settings, then MCP. Plugin servers appear with a `plugin-` prefix, for example `plugin-safe-cap-table-mcp-safe-cap-table`.

**Manually, without the Marketplace:** add the server URL to your `~/.cursor/mcp.json`, for example:

```json
{
  "mcpServers": {
    "safe-cap-table": { "url": "https://safe-cap-table-mcp.vercel.app/mcp" }
  }
}
```

## Safety by design

- Read-only tools fetch public data and say where it came from and when.
- Anything that posts, sends a message, places a call or prepares a purchase link returns a preview first and needs explicit confirmation.
- Your own keys are sent per request and are never stored.

## Privacy and terms

- Privacy policy: https://maasai.tech/privacy
- Terms of use: https://maasai.tech/terms
- Support and data requests: colepresley000@gmail.com

## Repository layout

```
.cursor-plugin/marketplace.json   lists all 10 plugins
plugins/<name>/.cursor-plugin/plugin.json
plugins/<name>/mcp.json           remote MCP server URL (and optional headers)
plugins/<name>/assets/logo.png
plugins/<name>/README.md
```

MIT License. Copyright (c) 2026 Segun Cole.
