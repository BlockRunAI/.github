<div align="center">

# BlockRun

**BlockRun lets agents pay for the outcome — every LLM, tool and data source, best value per dollar.**

Sign up with a credit card and get an API key, or pay per call from a wallet with no account.

[![Website](https://img.shields.io/badge/blockrun.ai-visit-blue)](https://blockrun.ai)
[![Get started](https://img.shields.io/badge/user.blockrun.ai-sign%20up-brightgreen)](https://user.blockrun.ai)
[![Open Source](https://img.shields.io/badge/open--source-index-green)](https://blockrun.ai/open-source)
[![Franklin](https://img.shields.io/npm/v/@blockrun/franklin?label=Franklin&color=cb3837)](https://www.npmjs.com/package/@blockrun/franklin)
[![ClawRouter](https://img.shields.io/npm/v/@blockrun/clawrouter?label=ClawRouter&color=green)](https://www.npmjs.com/package/@blockrun/clawrouter)
[![Telegram](https://img.shields.io/badge/Telegram-join-blue?logo=telegram)](https://t.me/blockrunAI)
[![X](https://img.shields.io/badge/X-follow-black?logo=x)](https://x.com/BlockRunAI)

</div>

---

## Two ways in

Same models, same prices, same OpenAI-compatible endpoint. Pick the door that fits you.

| | **API key** | **Wallet** |
|---|---|---|
| Sign up | [user.blockrun.ai](https://user.blockrun.ai) — email + credit card | None. Fund a wallet and go |
| Auth | Your API key | The payment signature itself |
| Billing | Card top-up or monthly invoice, in dollars | Settled per call in USDC (Base or Solana) |
| Best for | Teams, existing OpenAI-compatible code, finance that wants an invoice | Autonomous agents — they can hold USDC, they can't hold a card |

Either way it's the same deal: every call is quoted in dollars **before it runs** and billed at exact usage. No subscription, no seats, no minimum top-up, no prepaid credits that expire.

---

## Flagship Products

### [Franklin](https://github.com/BlockRunAI/Franklin) — Open-source AI agent with wallet

**Every frontier model. Pay per use. No subscription.**

The open-source alternative to Claude Code and Cursor. Use any model, switch mid-session, pay only for what you use.

| | Claude Code | Cursor | Aider | **Franklin** |
|---|---|---|---|---|
| Models | Claude only | Mixed (limited) | Bring your key | **Every frontier model** |
| Pricing | $200/mo | $20/mo + usage | Free + API costs | **Pay per request** |
| Payment | Credit card | Credit card | Your own API keys | **Credit card or USDC** |
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

**Cut LLM costs automatically — route every request to the cheapest capable model.**

Routes every request to the cheapest model that can handle it — 15-dimension weighted scoring in <1ms. This is where "best value per dollar" is earned, and it's open source.

```bash
curl -fsSL https://blockrun.ai/ClawRouter-update | bash
```

---

## Everything you can pay for, per call

One account or one wallet, one API — text, images, video, music, real-time data, and real-person video IP.

- **Chat** — every frontier LLM (GPT, Claude, Gemini, Grok, Qwen, DeepSeek, Kimi, GLM, MiniMax, Llama) — OpenAI-compatible
- **Images** — gpt-image-2, Nano Banana Pro, CogView-4, Grok Imagine
- **Video** — ByteDance Seedance 2.0 + OpenAI Sora 2, with synced audio
- **Music** — MiniMax Music, full tracks per call
- **RealFace** — enroll a real person's likeness for Seedance video ($0.01, no KYC)
- **Live data** — web/news/X search, neural research (Exa), prediction markets (Polymarket/Kalshi), DEX + crypto prices

---

## Data + Intelligence

### [BlockRun MCP](https://github.com/BlockRunAI/blockrun-mcp) — Real-time data for Claude Code

Markets, research, X/Twitter, crypto, image & video generation — all inside Claude Code.

```bash
claude mcp add blockrun npx -y @blockrun/mcp@latest
```

| Tool | What | Cost |
|------|------|------|
| `blockrun_chat` | GPT, Claude, Gemini, Grok, Qwen, DeepSeek — the full catalog | per token |
| `blockrun_image` | gpt-image-2, Nano Banana Pro, Grok Imagine | $0.02–0.10 |
| `blockrun_video` | Sora 2, Seedance 2.0, with synced audio | per second |
| `blockrun_music` | MiniMax music — full tracks | per track |
| `blockrun_speech` | ElevenLabs TTS + sound effects | from $0.05/1k chars |
| `blockrun_realface` | Real-person video — liveness enrollment | $0.01 |
| `blockrun_search` | Live web + news (Grok) | ~$0.01 |
| `blockrun_exa` | Neural research (Exa) — answers, contents | $0.002–0.012 |
| `blockrun_markets` | Polymarket, Kalshi, sports odds | $0.001 |
| `blockrun_surf` | Crypto data — 80+ on-chain endpoints | from $0.003 |
| `blockrun_price` | Pyth quotes — crypto, FX, stocks | free |
| `blockrun_dex` | Live DEX prices (DexScreener) | free |
| `blockrun_rpc` | Raw JSON-RPC — 40+ chains | $0.004 |
| `blockrun_defi` | DefiLlama — TVL, yields, token prices | per call |
| `blockrun_modal` | Sandboxed code exec — optional GPU | per run |
| `blockrun_phone` | AI voice calls + US/CA numbers | $0.54/call |
| `blockrun_models` | Model catalog & pricing | free |
| `blockrun_wallet` | USDC balance & agent budgets | free |

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
  BlockRun API — one OpenAI-compatible endpoint, priced per call
      ↓
  API key  ────  card top-up or monthly invoice, in dollars
  Wallet   ────  x402 micropayments, USDC on Base & Solana
                 (+ gas-free batched USDC on Polygon / Arbitrum /
                   Optimism / Unichain via Circle Gateway)
      ↓
  every frontier model + real-time data + image / video / music
```

The wallet door is the one most gateways can't offer: **payment is authentication**, so an autonomous agent needs no account and no credential to hand over — the signature that pays also proves who's calling. The card door exists because most teams shouldn't have to care.

---

<div align="center">

**[Get started](https://user.blockrun.ai)** · **[Docs](https://blockrun.ai/docs)** · **[Models](https://blockrun.ai/models)** · **[Enterprise](https://blockrun.ai/enterprise)** · **[x402](https://x402.org)**

Built for agents. Pay for the outcome.

</div>
