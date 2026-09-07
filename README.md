# 🤖 AI Agents Hub

<p align="center"><strong>A curated home for AI agents, tools, skills, MCP servers, and model APIs.</strong><br><sub>Built for people who love AI agents — discover, compare, install, extend, and build with them.</sub></p>

<p align="center"><a href="README.md"><strong>🇬🇧 English</strong></a> · <a href="README.ar.md"><strong>🇸🇦 العربية</strong></a> · <a href="docs/index.html"><strong>🌐 Hub Website</strong></a></p>

> **AI Agents Hub was created for people who love AI agents.** A community-driven directory and knowledge base for agents, capabilities, MCP integrations, and model APIs.

## ✨ What is AI Agents Hub?

Use one place to discover agents, compare them, find tools/skills/MCP, learn installation, and choose a model provider. The goal is not to declare one universal winner: the best agent depends on your workflow.

## 🏆 Featured Agent Ranking

| Rank | Agent | Primary type | Best for | Score |
|---:|---|---|---|---:|
| 1 | [Hermes Agent](https://github.com/NousResearch/hermes-agent) | Personal / coding / autonomous | Persistent agent workflows | ⭐ 9.7 |
| 2 | [OpenHands](https://github.com/All-Hands-AI/OpenHands) | Coding / autonomous | Software engineering | ⭐ 9.6 |
| 3 | [OpenCode](https://github.com/anomalyco/opencode) | Coding / terminal | Provider-agnostic development | ⭐ 9.5 |
| 4 | [Cline](https://github.com/cline/cline) | Coding / IDE | Human-in-the-loop coding | ⭐ 9.4 |
| 5 | [Goose](https://github.com/block/goose) | General / coding | MCP workflows | ⭐ 9.3 |
| 6 | [Aider](https://github.com/Aider-AI/aider) | Coding / terminal | Git pair programming | ⭐ 9.2 |
| 7 | [SWE-agent](https://github.com/SWE-agent/SWE-agent) | Coding / research | GitHub/SWE tasks | ⭐ 9.0 |
| 8 | [Gemini CLI](https://github.com/google-gemini/gemini-cli) | Coding / terminal | Gemini workflows | ⭐ 8.9 |
| 9 | [Qwen Code](https://github.com/QwenLM/qwen-code) | Coding / terminal | Open-model workflows | ⭐ 8.8 |
| 10 | [OpenClaw](https://github.com/openclaw/openclaw) | Personal / automation | Messaging and automation | ⭐ 8.8 |

The ranking is editorial, not an official benchmark.

## 🧰 Tools, Skills & MCP

The marketplace now covers browser automation, coding, research/RAG, memory/vector databases, messaging, automation and computer use.

- 📚 [Expanded Tools & Skills catalog](skills/catalog.md)
- 🔌 [MCP servers & integrations](skills/mcp.md)
- 🧰 [Marketplace overview](skills/README.md)

Featured capabilities include Playwright, Puppeteer, browser-use, GitHub CLI, Git, ripgrep, Docker, LlamaIndex, LangChain, Qdrant, Chroma, Redis, Telegram, Discord, n8n, PyAutoGUI and more.

Compatibility labels distinguish Native, MCP, Plugin, Manual and Unverified integrations. These labels are discovery aids, not guarantees.

## 🆓 Free / Free-Tier Model APIs

The Hub now includes a practical guide for getting API keys, choosing models, configuring agents, and handling quotas safely.

- 🆓 [Free / free-tier model API guide](providers/free-api.md)

Providers covered:

| Provider | Best starting point | Key variable |
|---|---|---|
| Google AI Studio / Gemini | Easy first API key and Gemini experiments | `GEMINI_API_KEY` |
| Groq | Fast inference | `GROQ_API_KEY` |
| OpenRouter | Many models through one API | `OPENROUTER_API_KEY` |
| Cerebras | Fast inference where eligible | `CEREBRAS_API_KEY` |
| Cloudflare Workers AI | Cloudflare-native applications | Account/binding configuration |

Free availability, model lists and quotas can change. The provider's current dashboard is authoritative.

## 🔑 How to create and use an API key

1. Create an account with the provider.
2. Open its API-key/developer section.
3. Create a key and copy it securely.
4. Store it in an environment variable or documented secret manager.
5. Choose a currently available model from the provider's live model list.
6. Configure the agent with the provider's documented API format/base URL/model ID.
7. Test tool calling and context length before using the model for long autonomous tasks.

Example:

```bash
export OPENROUTER_API_KEY="YOUR_KEY"
```

**Never commit a real API key to GitHub.**

## 📚 Documentation

- 📋 [Agent catalog](agents/README.md)
- 🧰 [Tools & Skills Marketplace](skills/README.md)
- 🔌 [MCP ecosystem](skills/mcp.md)
- 🆓 [Free model APIs](providers/free-api.md)
- 📦 [Installation guides](docs/installation.md)
- 📊 [Ranking methodology](docs/ranking.md)
- 🏗️ [Architecture](docs/architecture.md)
- 🤝 [Contribution guide](CONTRIBUTING.md)
- 🔐 [Security policy](SECURITY.md)

## 🌍 Bilingual by Design

The English and Arabic documentation are kept aligned in scope: agents, tools/skills, MCP, free model APIs, setup, security and contribution guidance.

- 🇬🇧 English: `README.md`
- 🇸🇦 Arabic: `README.ar.md`
- 🌐 Interactive bilingual hub: `docs/index.html`

## 🔐 Security First

Agents can execute commands, edit files, access networks and sometimes control computers. Review permissions and use least privilege. Never put API keys, passwords, private tokens or SSH keys in issues, pull requests or source code.

## 🤝 Contributing

Contribute agents, tools, skills, MCP servers, provider guides, compatibility reports, benchmarks, translations and documentation. See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## 📜 License

This directory and its original documentation are MIT licensed. Third-party projects retain their own licenses and trademarks. AI Agents Hub is an independent community directory.
