# 🛍️ Capability Catalog

A starter marketplace of reusable capabilities. Entries link to upstream projects; compatibility should be verified before installation.

| Capability | Category | Source | Typical use |
|---|---|---|---|
| Playwright | Browser | https://github.com/microsoft/playwright | Browser automation and testing |
| MCP | Protocol | https://github.com/modelcontextprotocol | Standardized tool/data connections |
| GitHub CLI | Developer | https://github.com/cli/cli | GitHub operations from terminal |
| ripgrep | Search | https://github.com/BurntSushi/ripgrep | Fast repository search |
| Docker | Runtime | https://github.com/moby/moby | Isolated environments |
| uv | Python tooling | https://github.com/astral-sh/uv | Fast Python environments and packages |

## Compatibility matrix

| Capability | Hermes | OpenHands | OpenCode | Cline | Goose |
|---|---|---|---|---|---|
| Git / shell workflows | 🧩 | 🧩 | 🧩 | 🧩 | 🧩 |
| Browser automation | 🧩 | 🧩 | 🧩 | 🧩 | 🧩 |
| MCP | 🔌 | 🔌 | 🔌 | 🔌 | 🔌 |
| Custom scripts | 🛠️ | 🛠️ | 🛠️ | 🛠️ | 🛠️ |

Legend: 🔌 MCP integration, 🧩 agent/tool integration, 🛠️ manual integration. These labels are a discovery aid, not a compatibility guarantee.

## Add a listing

Use the following structure:

```markdown
### Tool name
- Category:
- Source:
- License:
- Installation:
- Compatible agents:
- Permissions:
- Security notes:
- Last reviewed:
```
