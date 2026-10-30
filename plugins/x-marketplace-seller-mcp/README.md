# X Marketplace Seller

Sell items on X: create listings with a private floor and ceiling, draft buyer replies with intent and scam detection, run a negotiation engine that never goes below your floor or reveals it, draft pickup/delivery handoffs, and keep a deal ledger. Posting and DMs use your own X token, and every post, DM or deal needs explicit confirmation. Storage is isolated per user.

- Hosted MCP server: `https://x-marketplace-seller-mcp.vercel.app/mcp` (Streamable HTTP)
- Source code: https://github.com/MAASAI-Labs/x-marketplace-seller-mcp
- Free to use. MIT licensed.

## Optional settings

Set these in Cursor under **Plugins**, then **Configure** on this plugin. They are sent to the hosted server as request headers and are never stored by it.

| Variable | Sent as header | What it is |
|---|---|---|
| `X_USER_ACCESS_TOKEN` | `x-x-user-access-token` | Your own X OAuth 2.0 user-context token with tweet.write (and dm.write for DMs). Only needed to post listings or send DMs. |

Leave them blank to use only the tools that need no credentials.

## Use in Cursor

1. Install **X Marketplace Seller** from the Cursor Marketplace (publisher: MAASAI Labs).
2. Open Cursor Settings, then MCP, and check that the `x-marketplace-seller` server is enabled.
3. Ask the agent a question that needs it. See the source README for example prompts.

## Privacy and terms

- Privacy policy: https://maasai.tech/privacy
- Terms of use: https://maasai.tech/terms
- Support: colepresley000@gmail.com
