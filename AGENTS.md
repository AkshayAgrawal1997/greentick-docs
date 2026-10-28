# Documentation project instructions

## About this project

- This is the GreenTick documentation site, built on [Mintlify](https://mintlify.com).
- Pages are MDX files with YAML frontmatter.
- Configuration lives in `docs.json`.
- `openapi.json` is generated from `green-tick-backend/services/developer/openApiDocument.js` with origin `https://api.greentick.ai`. Regenerate it when the public API changes. Do not hand-edit endpoint pages that Mintlify generates from that file.
- Product context lives in `.mintlify/product-brief.md`.

## Terminology

- GreenTick, not Greentick or Green Tick, in titles and prose.
- WhatsApp Business account for the connected Meta account. Use WABA only in developer reference when the field name requires it.
- Phone number for a sending line on that account. `phoneNumberRef` is the GreenTick id from `GET /phone-numbers`.
- Live Chat for the inbox. Broadcasts, Templates, Contacts, Flows, Catalogs, Automations, and AI Bot match the dashboard labels.
- Developer for the API key and webhook screens. API keys use the prefix `gt_live_`.
- Template variables are named. Do not document positional `{{1}}` variables as the GreenTick format.
- Plans are Trial, Starter, Standard, and Premium.

## Style preferences

- Use active voice and second person ("you").
- Use sentence case for headings.
- Bold for UI elements: Click **Settings**.
- Code formatting for file names, commands, paths, and code references.
- Describe the dashboard a customer sees. Do not document super-admin tools, internal services, or environment variables.

## Content boundaries

- Document the dashboard at `https://dashboard.greentick.ai` and the public API at `https://api.greentick.ai/v1`.
- Google Sheets is the integration that is available in the dashboard. HubSpot, Make, n8n, Zapier, and Zoho are marked coming soon there. Explain the API they will use, and do not write install steps for tools the dashboard still labels coming soon.
- The MCP server at `https://api.greentick.ai/mcp` has its own docs tab under `mcp/`. Keep those pages aligned with `green-tick-backend/mcp/server.mjs`.
- Do not document All accounts, Change owner, or other super-admin screens.
