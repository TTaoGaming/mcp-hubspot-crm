# mcp-hubspot-crm

TypeScript MCP server for HubSpot contact/deal search and CRUD, associations, workflow enrollment, and the dated 2026-03 sequence enrollment API. Twelve tools plus a status resource and search-first prompt work over stdio or Cloudflare Workers Streamable HTTP.

```bash
git clone https://github.com/TTaoGaming/mcp-hubspot-crm.git
cd mcp-hubspot-crm && npm ci && npm run build
HUBSPOT_ACCESS_TOKEN=... npm run dev
```

Grant only the CRM and automation scopes you need. Workflow and sequence enrollment may trigger external communications and should be confirmed first. Hosted mode uses `/mcp`. `npm run check` and `npm run inspector:list` provide local verification. npm and Registry publication require operator approval.

Live credential-free demo: `https://mcp-hubspot-crm.tommytai3.workers.dev/mcp`. Discovery and status work; HubSpot calls fail closed until a Worker secret is bound.
