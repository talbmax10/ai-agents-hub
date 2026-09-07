# 🧰 Tools & Skills Catalog

A larger curated catalog for AI-agent workflows. Always verify compatibility and current installation instructions in the upstream project before use.

## Browser & Web

| Capability | Type | Best use | Source |
|---|---|---|---|
| Playwright | Tool | Browser automation, testing, extraction | https://github.com/microsoft/playwright |
| Puppeteer | Tool | Chrome/Chromium automation | https://github.com/puppeteer/puppeteer |
| browser-use | Agent skill/tooling | Website operation by agents | https://github.com/browser-use/browser-use |
| Selenium | Tool | Cross-browser automation/testing | https://github.com/SeleniumHQ/selenium |
| curl | Tool | HTTP APIs, downloads and diagnostics | https://github.com/curl/curl |

## Coding & Developer Tools

| Capability | Type | Best use | Source |
|---|---|---|---|
| GitHub CLI | Tool | Repositories, issues, PRs and Actions | https://github.com/cli/cli |
| Git | Tool | Version control and checkpoints | https://git-scm.com/ |
| ripgrep | Tool | Fast code/text search | https://github.com/BurntSushi/ripgrep |
| fd | Tool | Fast filesystem discovery | https://github.com/sharkdp/fd |
| jq | Tool | JSON processing in pipelines | https://github.com/jqlang/jq |
| Docker | Tool | Isolated execution | https://github.com/docker |
| pytest | Tool/skill | Python testing | https://github.com/pytest-dev/pytest |

## Research & Retrieval

| Capability | Type | Best use | Source |
|---|---|---|---|
| Trafilatura | Tool | Web text extraction | https://github.com/adbar/trafilatura |
| Scrapy | Framework | Crawling and extraction | https://github.com/scrapy/scrapy |
| Beautiful Soup | Library | HTML parsing | https://www.crummy.com/software/BeautifulSoup/ |
| LlamaIndex | Framework/skill | RAG and data connectors | https://github.com/run-llama/llama_index |
| LangChain | Framework/skill | Tool calling and orchestration | https://github.com/langchain-ai/langchain |

## Memory & Data

| Capability | Type | Best use | Source |
|---|---|---|---|
| SQLite | Database/tool | Lightweight local state | https://github.com/sqlite/sqlite |
| PostgreSQL | Database/tool | Durable relational data | https://github.com/postgres/postgres |
| Qdrant | Vector database | Semantic memory/RAG | https://github.com/qdrant/qdrant |
| Chroma | Vector database | Local vector retrieval | https://github.com/chroma-core/chroma |
| Redis | Data store | State, queues and caching | https://github.com/redis/redis |

## Messaging & Automation

| Capability | Type | Best use | Source |
|---|---|---|---|
| Telegram Bot API | Integration | Agent notifications and remote control | https://core.telegram.org/bots/api |
| Discord API | Integration | Agent channels and notifications | https://discord.com/developers/docs |
| cron | Tool | Scheduled jobs | https://github.com/vixie/cron |
| n8n | Automation platform | Visual workflows and webhooks | https://github.com/n8n-io/n8n |

## Computer Use

| Capability | Type | Best use | Source |
|---|---|---|---|
| PyAutoGUI | Tool | Desktop keyboard/mouse automation | https://github.com/asweigart/pyautogui |
| xdotool | Tool | X11 desktop automation | https://github.com/jordansissel/xdotool |

## Recommended skill patterns

- **Browser research:** browser-use + Playwright + extraction + citation checks.
- **Coding:** Git + GitHub CLI + ripgrep + tests + isolated shell.
- **RAG:** LlamaIndex/LangChain + Qdrant/Chroma + document extraction.
- **Remote agent:** Telegram/Discord + webhook + scheduler + least-privilege credentials.
- **Safe execution:** Docker sandbox + explicit approval for destructive commands.

## Compatibility labels

- ✅ Native — documented first-class support by the agent.
- 🔌 MCP — exposed through an MCP server.
- 🧩 Plugin — exposed through an extension/plugin system.
- 🛠️ Manual — callable through shell/API integration.
- ❓ Unverified — not independently checked.

Do not treat a catalog entry as a security endorsement. Review permissions, network access, dependencies and upstream maintenance before installation.
