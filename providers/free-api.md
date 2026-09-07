# 🆓 Free / Free-Tier Model API Providers

This page focuses on providers that offer a free tier or free models. **Free does not mean unlimited**: limits, eligible models, rate limits and policies can change. Always check the provider's current dashboard and pricing page before building a production dependency.

## 1. Google AI Studio / Gemini API

**Best for:** an easy first API key and Gemini models.

### Create an API key
1. Open Google AI Studio.
2. Sign in with your Google account.
3. Open the API key section.
4. Create a new API key and copy it immediately.
5. Store it as an environment variable; never commit it to Git.

### Choose a model
Use the model list shown in AI Studio/API documentation. Prefer a current Gemini Flash model for low-latency, lower-cost experiments and choose a stronger Gemini model when quality is more important.

Example environment variable:

```bash
export GEMINI_API_KEY="YOUR_KEY"
```

Official docs: https://ai.google.dev/

## 2. Groq

**Best for:** very fast inference and agent/tool-calling experiments when a supported model is available.

### Create an API key
1. Create/sign in to your Groq account.
2. Open the API keys page in the console.
3. Create a key.
4. Store it as `GROQ_API_KEY`.

```bash
export GROQ_API_KEY="YOUR_KEY"
```

### Choose a model
Select a currently listed model in the Groq console. Model availability and free-tier limits can change, so the live model list is authoritative.

Official docs: https://console.groq.com/docs

## 3. OpenRouter

**Best for:** one OpenAI-compatible endpoint that exposes many providers and models, including models marked free when available.

### Create an API key
1. Create/sign in to an OpenRouter account.
2. Open the Keys page.
3. Create a key.
4. Store it as `OPENROUTER_API_KEY`.

```bash
export OPENROUTER_API_KEY="YOUR_KEY"
```

### Choose a model
Open the Models page and filter for models whose pricing shows zero input/output cost or the current free label. Do not hard-code a model as permanently free; availability can change.

API base URL:

```text
https://openrouter.ai/api/v1
```

Official docs: https://openrouter.ai/docs

## 4. Cerebras

**Best for:** fast inference when an eligible free/developer tier and desired model are available to your account.

### Create an API key
1. Create/sign in to your Cerebras account.
2. Open the developer/API-key area.
3. Create a key.
4. Store it as `CEREBRAS_API_KEY`.

```bash
export CEREBRAS_API_KEY="YOUR_KEY"
```

Check the current model list and limits in the Cerebras documentation before selecting a model.

Official docs: https://inference-docs.cerebras.ai/

## 5. Cloudflare Workers AI

**Best for:** developers already using Cloudflare Workers and wanting hosted model inference inside the Cloudflare platform.

### Setup
1. Create/sign in to a Cloudflare account.
2. Create or select a Workers project.
3. Enable Workers AI and follow the current account/binding setup.
4. Choose a model from the current Workers AI catalog.
5. Keep credentials/bindings server-side; do not expose privileged tokens in browser code.

Official docs: https://developers.cloudflare.com/workers-ai/

## How to choose a free provider

| Need | Start with |
|---|---|
| Easiest first API key | Google AI Studio |
| Fast inference | Groq / Cerebras |
| Many models through one API | OpenRouter |
| Cloudflare-native application | Workers AI |

## Agent configuration principles

- Prefer environment variables for API keys.
- Confirm the agent supports the provider's API format before configuring it.
- For OpenAI-compatible agents, use the provider's documented base URL and model identifier.
- Start with a small/fast model for tool-call and integration tests.
- Move to a stronger model after verifying context length, structured output and tool-calling behavior.
- Track rate limits and quotas; a free tier may stop working after a quota is reached.

## Security

**Never put a real API key in this repository.** Use `.env` locally (and keep it ignored), GitHub Actions Secrets for workflows, or the agent's documented secret store.
