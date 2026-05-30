# Dealboard MCP Installation Notes

Dealboard provides a hosted remote MCP server at:

```text
https://app.getdealboard.com/mcp
```

Use Streamable HTTP transport. The server uses OAuth 2.1 with PKCE and dynamic
client registration, so users should authenticate through the client-provided
OAuth flow instead of supplying an API key manually.

Recommended MCP client configuration:

```json
{
  "mcpServers": {
    "dealboard": {
      "url": "https://app.getdealboard.com/mcp"
    }
  }
}
```

After connection, refresh the tool list. A successful connection exposes tools
for deals, leads, notes, pipeline summaries, goals, reporting cards, and report
image export.

Do not ask the user for secrets. If the user is not authenticated, instruct the
client to start the OAuth flow for the Dealboard MCP server.

