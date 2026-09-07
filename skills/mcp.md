# 🔌 MCP Servers & Integrations

Model Context Protocol (MCP) lets compatible agents connect models to external tools, data and services. Treat each server as code with permissions: inspect its source, credentials, network access and filesystem scope before enabling it.

## Featured MCP ecosystem

| MCP / integration | Category | What it can provide | Source |
|---|---|---|---|
| Official MCP servers ecosystem | Protocol / servers | Standard tool and data connections | https://github.com/modelcontextprotocol |
| GitHub MCP Server | Developer | Repositories, issues, pull requests and GitHub workflows | https://github.com/github/github-mcp-server |
| Filesystem MCP | Files | Controlled filesystem operations | https://github.com/modelcontextprotocol/servers |
| Fetch MCP | Web | Retrieve web resources for agent workflows | https://github.com/modelcontextprotocol/servers |
| Git MCP | Developer | Git repository operations | https://github.com/modelcontextprotocol/servers |
| PostgreSQL MCP | Database | Query approved PostgreSQL databases | https://github.com/modelcontextprotocol/servers |
| SQLite MCP | Database | Local SQLite access | https://github.com/modelcontextprotocol/servers |
| Puppeteer MCP | Browser | Browser interaction through Puppeteer | https://github.com/modelcontextprotocol/servers |
| Slack integrations | Messaging | Team messaging workflows | https://github.com/modelcontextprotocol/servers |

## Installation pattern

1. Read the upstream server README and inspect its source.
2. Check required environment variables and credentials.
3. Restrict filesystem paths, repositories, databases and network destinations where possible.
4. Add the server to the agent's documented MCP configuration.
5. Start with read-only permissions when supported.
6. Test one harmless operation before granting write or destructive capabilities.

## Security checklist

- Never commit API keys or OAuth tokens.
- Prefer environment variables or the agent's secret manager.
- Avoid unrestricted filesystem access.
- Avoid exposing a database with write permissions unless required.
- Pin versions where practical and review updates.
- Remove unused MCP servers and credentials.

Compatibility is agent-specific. The table is a discovery catalog, not a guarantee that every listed server works unchanged with every agent.
