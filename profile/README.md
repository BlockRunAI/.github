<div align="center">

# BlockRun

**AI infrastructure that lets agents pay for themselves**

No API keys. No subscriptions. Fund a wallet and go.

[![Website](https://img.shields.io/badge/blockrun.ai-visit-blue)](https://blockrun.ai)
[![Franklin](https://img.shields.io/npm/v/@blockrun/runcode?label=Franklin&color=cb3837)](https://www.npmjs.com/package/@blockrun/runcode)
[![ClawRouter](https://img.shields.io/npm/v/@blockrun/clawrouter?label=ClawRouter&color=green)](https://www.npmjs.com/package/@blockrun/clawrouter)
[![Telegram](https://img.shields.io/badge/Telegram-join-blue?logo=telegram)](https://t.me/blockrunAI)
[![X](https://img.shields.io/badge/X-follow-black?logo=x)](https://x.com/BlockRunAI)

</div>

---

## Flagship Products

### [Franklin](https://github.com/BlockRunAI/runcode) — Open-source AI coding agent

**41+ models. Pay per use. No subscription.**

The open-source alternative to Claude Code and Cursor. Use any model, switch mid-session, pay only for what you use with USDC.

| | Claude Code | Cursor | Aider | **Franklin** |
|---|---|---|---|---|
| Models | Claude only | Mixed (limited) | Bring your key | **41+ models** |
| Pricing | $200/mo | $20/mo + usage | Free + API costs | **Pay per request** |
| Payment | Credit card | Credit card | API keys | **USDC** |
| Open source | No | No | Yes | **Yes** |

```bash
npm install -g @blockrun/runcode
runcode setup base
runcode
```

**Proxy mode** — use Franklin as a payment proxy behind Claude Code:
```bash
runcode init    # auto-configures Claude Code to route through Franklin
```

---

### [ClawRouter](https://github.com/BlockRunAI/ClawRouter) — Smart LLM router for OpenClaw

**Save 40-92% on LLM costs. Automatically.**

Routes every request to the cheapest model that can handle it. 15-dimension weighted scoring in <1ms.

```bash
curl -fsSL https://blockrun.ai/ClawRouter-update | bash
```

---

## Data + Intelligence

### [BlockRun MCP](https://github.com/BlockRunAI/blockrun-mcp) — Real-time data for Claude Code

Markets, research, X/Twitter, crypto, image generation — all inside Claude Code. No API keys.

```bash
claude mcp add blockrun npx -y @blockrun/mcp@latest
```

| Tool | What | Cost |
|------|------|------|
| `blockrun_search` | Web + news search | ~$0.01 |
| `blockrun_exa` | Neural research (Exa) | $0.01 |
| `blockrun_markets` | Polymarket, Kalshi | $0.001 |
| `blockrun_twitter` | X/Twitter intelligence | per token |
| `blockrun_dex` | DEX prices | free |
| `blockrun_image` | DALL-E 3, Flux | $0.02-0.08 |
| `blockrun_chat` | GPT, Gemini, DeepSeek, 30+ | per token |

---

## Full Ecosystem

| Project | What | Install |
|---------|------|---------|
| [Franklin](https://github.com/BlockRunAI/runcode) | Open-source AI coding agent | `npm i -g @blockrun/runcode` |
| [ClawRouter](https://github.com/BlockRunAI/ClawRouter) | Smart LLM router for OpenClaw | `curl -fsSL https://blockrun.ai/ClawRouter-update \| bash` |
| [blockrun-mcp](https://github.com/BlockRunAI/blockrun-mcp) | Real-time data for Claude Code | `claude mcp add blockrun npx -y @blockrun/mcp@latest` |
| [awesome-finance-mcp](https://github.com/BlockRunAI/awesome-finance-mcp) | Curated finance MCP servers | — |
| [polymarket-agent](https://github.com/BlockRunAI/polymarket-agent) | AI prediction market trading | `git clone` |
| [alpha-mcp](https://github.com/BlockRunAI/alpha-mcp) | Crypto trading signals | `git clone` |
| [blockrun-llm](https://github.com/BlockRunAI/blockrun-llm) | Python SDK | `pip install blockrun-llm` |
| [blockrun-llm-ts](https://github.com/BlockRunAI/blockrun-llm-ts) | TypeScript SDK | `npm i blockrun-llm` |

---

## How It Works

```
Your App / Agent
      ↓
  Franklin (standalone)     OR     ClawRouter (OpenClaw plugin)
      ↓                                ↓
  BlockRun API (x402 micropayments, USDC on Base & Solana)
      ↓
  41+ LLM providers + real-time data sources
```

**Payment IS authentication.** No API keys — your wallet signature proves you can pay.

---

<div align="center">

**[Docs](https://blockrun.ai/docs)** · **[Models](https://blockrun.ai/models)** · **[x402 Protocol](https://x402.org)**

Built for agents. Powered by [x402](https://x402.org).

</div>
