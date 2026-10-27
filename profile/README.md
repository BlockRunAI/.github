<div align="center">

# BlockRun

### Agents spend money. We measure.

BlockRun independently tests AI agents that move money: did they pay the right party the right amount, avoid being scammed, stay within their mandate, and tell the truth afterwards. Scored from the ledger, not by a model judge.

[![Website](https://img.shields.io/badge/blockrun.ai-visit-blue)](https://blockrun.ai)
[![Agent testing](https://img.shields.io/badge/agent%20testing-learn%20more-black)](https://blockrun.ai/agent-testing)
[![Developers](https://img.shields.io/badge/developers-get%20an%20API%20key-brightgreen)](https://blockrun.ai/developers)
[![ClawRouter](https://img.shields.io/github/stars/BlockRunAI/ClawRouter?label=ClawRouter&style=flat&color=green)](https://github.com/BlockRunAI/ClawRouter)
[![Telegram](https://img.shields.io/badge/Telegram-join-blue?logo=telegram)](https://t.me/blockrunAI)
[![X](https://img.shields.io/badge/X-follow-black?logo=x)](https://x.com/BlockRunAI)

</div>

---

## Why we can measure it

We run a gateway where agents pay per call, and every payment settles. So we see every payment an agent gets wrong, and what each dollar actually bought. Everything we build reads those same settled payments.

| | For | What you get |
|---|---|---|
| **[Verified Eval](https://blockrun.ai/benchmark)** | Financial institutions, agent builders | Your own production cases, run across models and harnesses and graded by code. Where the agent moves money, we check it paid the right party the right amount, within its limits, and said so truthfully. You see which setup holds up, and what each completed task costs. |
| **[RL environments](https://blockrun.ai/ai-labs)** | AI labs | Money-moving tasks built to order: agents that pay for real, scored by the settlement ledger instead of a judge. Every task synthesized by us. No customer data. |
| **[Developer API](https://blockrun.ai/developers)** | Developers | One OpenAI-compatible endpoint for models, tools and data, each call priced before it runs. |

**[Talk to us about an evaluation →](https://blockrun.ai/contact)**

---

## Open source

The open-source half of BlockRun runs on your side, not ours.

### [ClawRouter](https://github.com/BlockRunAI/ClawRouter) — the agent-native LLM router

Picks the cheapest model that can do the job on every request, locally, in under a millisecond, with no inference call. One wallet instead of an account at every lab.

```bash
curl -fsSL https://blockrun.ai/ClawRouter-update | bash
```

Built on **[router-core](https://github.com/BlockRunAI/router-core)**: classify, hard-filter on capability, then rank on task fit, cost, speed and reliability. Deterministic. Also powers Franklin and every ClawRouter port below.

| Port | Where it runs |
|---|---|
| [ClawRouter-Hermes](https://github.com/BlockRunAI/ClawRouter-Hermes) | NousResearch Hermes — one provider block replaces an account at every lab |
| [dsh-clawrouter](https://github.com/BlockRunAI/dsh-clawrouter) | DeepSeek Harness — a stronger model reviews dangerous tool calls before they run |
| [clawrouter-codex](https://github.com/BlockRunAI/clawrouter-codex) | OpenAI Codex CLI and Desktop, via the Responses API |
| [XClawRouter](https://github.com/BlockRunAI/XClawRouter) | OKX OnchainOS wallet |

### [Franklin](https://github.com/BlockRunAI/Franklin) — the AI agent with a wallet

An open-source agent that spends from its own budget to get real work done. Any model, switch mid-session, pay only for what it uses.

```bash
npm install -g @blockrun/franklin
franklin
```

Also: [Franklin-Trading](https://github.com/BlockRunAI/Franklin-Trading) (a trading agent with a wallet) · [franklin-canvas](https://github.com/BlockRunAI/franklin-canvas) (image, video and music on an infinite canvas).

### [BlockRun MCP](https://github.com/BlockRunAI/blockrun-mcp) — live data and media inside your agent

Search, research, markets, crypto, X/Twitter, image, video, music and speech as tools for Claude Code, Cursor and ChatGPT.

```bash
claude mcp add blockrun npx -y @blockrun/mcp@latest
```

Plugins with a spend gate and a cost meter: [blockrun-claude-plugin](https://github.com/BlockRunAI/blockrun-claude-plugin) (Claude Code) · [blockrun-codex-plugin](https://github.com/BlockRunAI/blockrun-codex-plugin) (OpenAI Codex).

---

## Developer API

Two ways in: pay per call with no account, or get an API key and a monthly invoice.

**With an API key.** [Get a key](https://user.blockrun.ai), add credits by card, and point any OpenAI client at BlockRun:

```python
import os
from openai import OpenAI

client = OpenAI(api_key=os.environ["BLOCKRUN_API_KEY"], base_url="https://api.blockrun.ai/v1")
response = client.chat.completions.create(
    model="deepseek/deepseek-v4.1-flash",
    messages=[{"role": "user", "content": "Hello!"}],
)
print(response.choices[0].message.content)
```

**With a wallet.** No account and no credential to hand over: the signature that pays also proves who is calling, which is why an autonomous agent can use it. Settled per call in USDC over [x402](https://x402.org), on [Solana](https://sol.blockrun.ai) or [Base](https://blockrun.ai).

Models, tools and live prices: [blockrun.ai/models](https://blockrun.ai/models) · [blockrun.ai/pricing](https://blockrun.ai/pricing) · [`GET /api/v1/models`](https://blockrun.ai/api/v1/models). Some open-weight models are [free](https://blockrun.ai/free), no card and no signup.

### SDKs

| Language | Repo | Install |
|---|---|---|
| Python | [blockrun-llm](https://github.com/BlockRunAI/blockrun-llm) | `pip install blockrun-llm` |
| TypeScript | [blockrun-llm-ts](https://github.com/BlockRunAI/blockrun-llm-ts) | `npm i @blockrun/llm` |
| Go | [blockrun-llm-go](https://github.com/BlockRunAI/blockrun-llm-go) | `go get github.com/BlockRunAI/blockrun-llm-go` |
| LiteLLM | [blockrun-litellm](https://github.com/BlockRunAI/blockrun-litellm) | custom provider or local proxy |
| Native passthrough | [blockrun-llm-vip](https://github.com/BlockRunAI/blockrun-llm-vip) · [blockrun-llm-go-vip](https://github.com/BlockRunAI/blockrun-llm-go-vip) | official Anthropic and OpenAI SDKs, responses verbatim |
| Gas-free batched USDC | [blockrun-nano-client](https://github.com/BlockRunAI/blockrun-nano-client) | via Circle Gateway |

More integrations: [elizaos-plugin-blockrun](https://github.com/BlockRunAI/elizaos-plugin-blockrun) · [lobstercash-blockrun-skill](https://github.com/BlockRunAI/lobstercash-blockrun-skill) · [blockrun-llm-xrpl](https://github.com/BlockRunAI/blockrun-llm-xrpl) · [awesome-blockrun](https://github.com/BlockRunAI/awesome-blockrun) · [awesome-finance-mcp](https://github.com/BlockRunAI/awesome-finance-mcp) · [branding](https://github.com/BlockRunAI/branding)

---

<div align="center">

**[Agent testing](https://blockrun.ai/agent-testing)** · **[For AI labs](https://blockrun.ai/ai-labs)** · **[Developers](https://blockrun.ai/developers)** · **[Docs](https://blockrun.ai/docs)** · **[Live settlements](https://blockrun.ai/live)**

Working with AWS, Circle and the Solana Foundation. Backed by HF0.

</div>
