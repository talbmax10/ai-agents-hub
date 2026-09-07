# 🏗️ Architecture

```text
ai-agents-hub/
├── agents/              # Agent catalog and evaluation guidance
├── skills/              # Tools, skills and MCP marketplace
├── docs/                # Guides, methodology and interactive website
├── templates/           # Contribution templates
├── .github/workflows/   # GitHub Pages deployment
├── README.md            # English entry point
├── README.ar.md         # Arabic entry point
├── CONTRIBUTING.md
├── SECURITY.md
├── CODE_OF_CONDUCT.md
├── CHANGELOG.md
└── LICENSE
```

## Design principles

- **Upstream-first:** link to original repositories.
- **Transparent:** explain ranking methodology and distinguish facts from opinions.
- **Bilingual:** English and Arabic documentation.
- **Composable:** agents, tools, skills and MCP are cataloged separately so capabilities can be reused across ecosystems.
- **Security-aware:** entries should disclose important permissions and trust boundaries.
- **Community-driven:** contributions are welcome and should be reviewable.

The interactive site is intentionally lightweight HTML/CSS/JavaScript so it can be hosted directly with GitHub Pages without a framework build step.
