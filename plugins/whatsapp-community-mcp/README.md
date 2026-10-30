# WhatsApp Community Manager

Run WhatsApp groups with your own Green API instance (optional WhatsApp Cloud API): list groups, read recent messages, summarise activity (top posters, busiest hours, unanswered questions, links), draft announcements, and post or schedule messages. Every send needs explicit confirmation; per-user isolated storage.

- Hosted MCP server: `https://whatsapp-community-mcp.vercel.app/mcp` (Streamable HTTP)
- Source code: https://github.com/MAASAI-Labs/whatsapp-community-mcp
- Free to use. MIT licensed.

## Optional settings

Set these in Cursor under **Plugins**, then **Configure** on this plugin. They are sent to the hosted server as request headers and are never stored by it.

| Variable | Sent as header | What it is |
|---|---|---|
| `GREEN_API_ID_INSTANCE` | `x-green-api-id-instance` | Your own Green API idInstance. Needed to list groups, read messages and post. |
| `GREEN_API_TOKEN_INSTANCE` | `x-green-api-token-instance` | Your own Green API apiTokenInstance. |

Leave them blank to use only the tools that need no credentials.

## Use in Cursor

1. Install **WhatsApp Community Manager** from the Cursor Marketplace (publisher: MAASAI Labs).
2. Open Cursor Settings, then MCP, and check that the `whatsapp-community` server is enabled.
3. Ask the agent a question that needs it. See the source README for example prompts.

## Privacy and terms

- Privacy policy: https://maasai.tech/privacy
- Terms of use: https://maasai.tech/terms
- Support: colepresley000@gmail.com
