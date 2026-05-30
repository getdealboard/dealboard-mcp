# Dealboard MCP Server

Track every deal without the spreadsheet mess or CRM overhead.

Dealboard is the simple, opinionated deal tracker for salespeople, BD teams,
founders, and small teams. It gives humans one clear sales pipeline with deal
cards, notes, goals, files, and reporting that works out of the box. The
Dealboard MCP server lets AI agents work with that same live pipeline: inspect
deals, add notes, update opportunities, promote leads, move stages, and pull
pipeline summaries.

## Hosted MCP Endpoint

```text
https://app.getdealboard.com/mcp
```

Authentication uses OAuth 2.1 with PKCE and dynamic client registration.

## What AI Agents Can Do

- List, search, create, update, and move deals
- Add notes to a deal's activity feed
- List, qualify, triage, and promote inbound leads
- Fetch active pipeline, weighted pipeline, and stage summaries
- Show out-of-the-box reporting for deal progress, deals won, active deals, and
  this month so far
- Export shareable report images

## Cursor, Cline, Windsurf, VS Code, and Other MCP Clients

Use the hosted remote MCP server:

```json
{
  "mcpServers": {
    "dealboard": {
      "url": "https://app.getdealboard.com/mcp"
    }
  }
}
```

If your client asks for transport, choose Streamable HTTP.

## xAI / Grok

Dealboard can be used as a remote MCP tool from the xAI API:

```json
{
  "type": "mcp",
  "server_url": "https://app.getdealboard.com/mcp",
  "server_label": "dealboard",
  "server_description": "Dealboard tracks sales deals, leads, notes, goals, files, and out-of-the-box pipeline reporting."
}
```

## Example Prompts

```text
Show me my active Dealboard pipeline and summarize what needs attention.
```

```text
Find the Acme deal, summarize what is happening, and add a note that I should
follow up next week on pricing.
```

```text
How am I pacing against my goals this month in Dealboard?
```

```text
Show me my newest inbound leads and help me decide which ones to promote to
deals.
```

## Links

- Website: https://getdealboard.com
- App: https://app.getdealboard.com
- Developer docs: https://getdealboard.com/developers/
- Server card: https://app.getdealboard.com/.well-known/mcp/server-card.json
- Privacy policy: https://getdealboard.com/privacy/
- Support: support@getdealboard.com

## Keywords

MCP, Model Context Protocol, remote MCP, hosted MCP, OAuth MCP, sales pipeline,
deal tracker, sales CRM, lightweight CRM, spreadsheet alternative, sales tools,
BD tools, founder sales, pipeline reporting, sales goals, ChatGPT, Claude,
Cursor, Cline, Windsurf, Grok, xAI.
