# Call Anyone in Any Language

Plan and place outbound phone calls in the callee's language with your own Bland or Twilio account: language detection, goal-based script, cost estimate and a preview you must confirm before any call. Then fetch transcript and summary. The caller always discloses it's an AI; emergency and premium numbers are blocked.

- Hosted MCP server: `https://call-anyone-mcp.vercel.app/mcp` (Streamable HTTP)
- Source code: https://github.com/MAASAI-Labs/call-anyone-mcp
- Free to use. MIT licensed.

## Optional settings

Set these in Cursor under **Plugins**, then **Configure** on this plugin. They are sent to the hosted server as request headers and are never stored by it.

| Variable | Sent as header | What it is |
|---|---|---|
| `BLAND_API_KEY` | `x-bland-api-key` | Your own Bland AI API key. Needed only to place calls through Bland. |
| `TWILIO_ACCOUNT_SID` | `x-twilio-account-sid` | Your own Twilio Account SID. Use instead of Bland. |
| `TWILIO_AUTH_TOKEN` | `x-twilio-auth-token` | Your own Twilio auth token. |
| `TWILIO_FROM_NUMBER` | `x-twilio-from-number` | A Twilio number you own, in E.164 format. |

Leave them blank to use only the tools that need no credentials.

## Use in Cursor

1. Install **Call Anyone in Any Language** from the Cursor Marketplace (publisher: MAASAI Labs).
2. Open Cursor Settings, then MCP, and check that the `call-anyone` server is enabled.
3. Ask the agent a question that needs it. See the source README for example prompts.

## Privacy and terms

- Privacy policy: https://maasai.tech/privacy
- Terms of use: https://maasai.tech/terms
- Support: colepresley000@gmail.com
