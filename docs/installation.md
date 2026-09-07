# 📦 Installation Guide

AI Agents Hub is a directory; the agents are installed from their upstream projects. Always prefer upstream installation instructions because commands change over time.

## 1. Choose your agent

Start at [`../agents/README.md`](../agents/README.md) and select by use case.

## 2. Prepare your environment

For most CLI agents:

```bash
# Check common prerequisites
python3 --version
node --version
git --version
```

Use the runtime required by the upstream project. Do not install arbitrary global packages just because another agent uses them.

## 3. Install from upstream

Typical patterns include:

```bash
# Python project
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

# Node project
npm install

# Clone a source repository
git clone https://github.com/OWNER/PROJECT.git
cd PROJECT
```

These are generic examples only. **Use the agent's official README for its exact command.**

## 4. Configure a model

Most agents need an API key or a locally hosted model. Prefer environment variables or the agent's documented secret store:

```bash
export OPENAI_API_KEY="..."
```

Never commit secrets to Git.

## 5. Add tools and skills

Browse [`../skills/README.md`](../skills/README.md). Verify compatibility and permissions before installing a third-party integration.

## 6. Run in a sandbox when possible

For agents capable of executing shell commands, start with a dedicated workspace and least-privilege credentials. Consider containers, VMs, or OS-level sandboxing for untrusted tasks.

## 7. Verify

After installation, test:

- model connectivity
- filesystem access
- tool permissions
- browser/network access
- Git credentials
- logs and error reporting

## Mobile / Termux

Many CLI agents can be adapted to Android through Termux, proot containers, or remote Linux hosts, but compatibility is agent-specific. Check architecture, Node/Python versions, native dependencies, and browser requirements before attempting installation.
