# Breach Radar

Passive, public-data security checks: Have I Been Pwned breach lookups (email lookups only when the server operator has set an HIBP key), k-anonymous password checks, NIST CVE search, CISA Known Exploited Vulnerabilities, and a domain's public attack surface (security headers, TLS, SPF/DMARC/DNSSEC/CAA, certificate-transparency subdomains). No scanning or probing.

- Hosted MCP server: `https://breach-radar-mcp.vercel.app/mcp` (Streamable HTTP)
- Source code: https://github.com/MAASAI-Labs/breach-radar-mcp
- Free to use. MIT licensed.

## Use in Cursor

1. Install **Breach Radar** from the Cursor Marketplace (publisher: MAASAI Labs).
2. Open Cursor Settings, then MCP, and check that the `breach-radar` server is enabled.
3. Ask the agent a question that needs it. See the source README for example prompts.

## Privacy and terms

- Privacy policy: https://maasai.tech/privacy
- Terms of use: https://maasai.tech/terms
- Support: colepresley000@gmail.com
