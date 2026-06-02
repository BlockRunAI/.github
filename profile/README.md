<div align="center">

# BlockRun

**AI infrastructure that lets agents pay for themselves**

No API keys. No subscriptions. Fund a wallet and go.

[![Website](https://img.shields.io/badge/blockrun.ai-visit-blue)](https://blockrun.ai)
[![Franklin](https://img.shields.io/npm/v/@blockrun/franklin?label=Franklin&color=cb3837)](https://www.npmjs.com/package/@blockrun/franklin)
[![ClawRouter](https://img.shields.io/npm/v/@blockrun/clawrouter?label=ClawRouter&color=green)](https://www.npmjs.com/package/@blockrun/clawrouter)
[![Telegram](https://img.shields.io/badge/Telegram-join-blue?logo=telegram)](https://t.me/blockrunAI)
[![X](https://img.shields.io/badge/X-follow-black?logo=x)](https://x.com/BlockRunAI)

</div>

---

## Flagship Products

### [Franklin](https://github.com/BlockRunAI/Franklin) — Open-source AI coding agent

**60+ models. Pay per use. No subscription.**

The open-source alternative to Claude Code and Cursor. Use any model, switch mid-session, pay only for what you use with USDC.

| | Claude Code | Cursor | Aider | **Franklin** |
|---|---|---|---|---|
| Models | Claude only | Mixed (limited) | Bring your key | **60+ models** |
| Pricing | $200/mo | $20/mo + usage | Free + API costs | **Pay per request** |
| Payment | Credit card | Credit card | API keys | **USDC** |
| Open source | No | No | Yes | **Yes** |

```bash
npm install -g @blockrun/franklin
franklin setup base
franklin
```

**Proxy mode** — use Franklin as a payment proxy behind Claude Code:
```bash
franklin init    # auto-configures Claude Code to route through Franklin
```

---

### [ClawRouter](https://github.com/BlockRunAI/ClawRouter) — Smart LLM router for OpenClaw

**Save 40-92% on LLM costs. Automatically.**

Routes every request to the cheapest model that can handle it. 15-dimension weighted scoring in <1ms.

```bash
curl -fsSL https://blockrun.ai/ClawRouter-update | bash
```

---

## Everything you can pay for, per call

One wallet, one API — text, images, video, music, real-time data, and real-person video IP.

- **Chat** — 60+ LLMs (GPT, Claude, Gemini, Grok, DeepSeek, Kimi, GLM, MiniMax, Llama) — OpenAI-compatible
- **Images** — gpt-image-2, Nano Banana Pro, Flux, Grok Imagine
- **Video** — ByteDance Seedance 2.0 + OpenAI Sora 2, with synced audio
- **Music** — MiniMax Music, full tracks per call
- **RealFace** — enroll a real person's likeness for Seedance video ($0.01, no KYC)
- **Live data** — web/news/X search, neural research (Exa), prediction markets (Polymarket/Kalshi), DEX + crypto prices

---

## Data + Intelligence

### [BlockRun MCP](https://github.com/BlockRunAI/blockrun-mcp) — Real-time data for Claude Code

Markets, research, X/Twitter, crypto, image & video generation — all inside Claude Code. No API keys.

```bash
claude mcp add blockrun npx -y @blockrun/mcp@latest
```

| Tool | What | Cost |
|------|------|------|
| `blockrun_search` | Web + news search | ~$0.01 |
| `blockrun_exa` | Neural research (Exa) | $0.01 |
| `blockrun_markets` | Polymarket, Kalshi | $0.001 |
| `blockrun_x` | X/Twitter intelligence | per token |
| `blockrun_dex` | DEX prices | free |
| `blockrun_price` | Crypto price data | free |
| `blockrun_image` | gpt-image-2, Nano Banana Pro, Flux | $0.02-0.10 |
| `blockrun_video` | AI video generation | per second |
| `blockrun_music` | AI music generation | per track |
| `blockrun_chat` | GPT, Claude, Gemini, DeepSeek, 60+ | per token |
| `blockrun_wallet` | Wallet balance & history | free |
| `blockrun_modal` | Run code on Modal | per run |
| `blockrun_models` | Model catalog & pricing | free |

---

## Full Ecosystem

| Project | What | Install |
|---------|------|---------|
| [Franklin](https://github.com/BlockRunAI/Franklin) | Open-source AI coding agent | `npm i -g @blockrun/franklin` |
| [Franklin-Trading](https://github.com/BlockRunAI/Franklin-Trading) | Autonomous trading agent with a wallet | `git clone` |
| [franklin-canvas](https://github.com/BlockRunAI/franklin-canvas) | Chat + node-canvas workflow UI for Franklin | — |
| [ClawRouter](https://github.com/BlockRunAI/ClawRouter) | Smart LLM router for OpenClaw | `curl -fsSL https://blockrun.ai/ClawRouter-update \| bash` |
| [XClawRouter](https://github.com/BlockRunAI/XClawRouter) | LLM router powered by OKX OnchainOS wallet | `git clone` |
| [ClawRouter-Hermes](https://github.com/BlockRunAI/ClawRouter-Hermes) | ClawRouter plugin for NousResearch Hermes | `git clone` |
| [blockrun-mcp](https://github.com/BlockRunAI/blockrun-mcp) | Real-time data for Claude Code | `claude mcp add blockrun npx -y @blockrun/mcp@latest` |
| [blockrun-llm](https://github.com/BlockRunAI/blockrun-llm) | Python SDK | `pip install blockrun-llm` |
| [blockrun-llm-ts](https://github.com/BlockRunAI/blockrun-llm-ts) | TypeScript SDK | `npm i @blockrun/llm` |
| [blockrun-llm-go](https://github.com/BlockRunAI/blockrun-llm-go) | Go SDK | `go get` |
| [blockrun-litellm](https://github.com/BlockRunAI/blockrun-litellm) | LiteLLM adapter (custom provider / proxy) | — |
| [blockrun-nano](https://github.com/BlockRunAI/blockrun-nano) | Gas-free batched USDC via Circle Gateway | — |
| [Prompt-Case-Hub](https://github.com/BlockRunAI/Prompt-Case-Hub) | Unified image/video/text prompt-case library | — |
| [awesome-finance-mcp](https://github.com/BlockRunAI/awesome-finance-mcp) | Curated finance MCP servers | — |
| [polymarket-agent](https://github.com/BlockRunAI/polymarket-agent) | AI prediction market trading | `git clone` |
| [alpha-mcp](https://github.com/BlockRunAI/alpha-mcp) | Crypto trading signals | `git clone` |
| [branding](https://github.com/BlockRunAI/branding) | Official brand kit — logos, colors, usage | — |

---

## How It Works

```
Your App / Agent
      ↓
  Franklin (standalone)     OR     ClawRouter (OpenClaw plugin)
      ↓                                ↓
  BlockRun API (x402 micropayments, USDC on Base & Solana
                + gas-free batched USDC on Polygon / Arbitrum /
                  Optimism / Unichain via Circle Gateway)
      ↓
  60+ models + real-time data + image / video / music
```

**Payment IS authentication.** No API keys — your wallet signature proves you can pay.

---

<div align="center">

**[Docs](https://blockrun.ai/docs)** · **[Models](https://blockrun.ai/models)** · **[x402 Protocol](https://x402.org)**

Built for agents. Powered by [x402](https://x402.org).

</div>
