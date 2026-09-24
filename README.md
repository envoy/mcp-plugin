# Envoy MCP plugin

Connect Cursor to Envoy's hosted MCP server using the [Agent Plugins 1.0.0](https://agent-plugins.org/) format.

The plugin connects to `https://mcp.envoy.com/mcp`. After installation, sign in with your Envoy account when Cursor prompts you. Available tools follow your Envoy account permissions. No API key or local server is required.

## Install

Install **Envoy** from the Cursor Marketplace. Cursor reads `plugin.json` and `mcp.json` from this repository and configures the remote server. When prompted, complete the Envoy sign-in and authorization flow.

For a manual MCP connection, add this server to Cursor's MCP configuration:

```json
{
  "mcpServers": {
    "envoy": {
      "url": "https://mcp.envoy.com/mcp"
    }
  }
}
```

The MCP service and its OAuth flow are hosted by Envoy. This repository contains only the public plugin configuration and installation instructions.
