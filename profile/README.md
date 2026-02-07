<div align="center">

# BlockRun

**Pay-per-request AI infrastructure**

No API keys. No accounts. Just fund a wallet and go.

[![Website](https://img.shields.io/badge/blockrun.ai-visit-blue)](https://blockrun.ai)
[![Telegram](https://img.shields.io/badge/Telegram-join-blue?logo=telegram)](https://t.me/blockrunAI)
[![X](https://img.shields.io/badge/X-follow-black?logo=x)](https://x.com/BlockRunAI)

</div>

---

## Featured: ClawRouter

<a href="https://github.com/BlockRunAI/ClawRouter">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=BlockRunAI&repo=ClawRouter&theme=dark" />
</a>

**Save 78% on LLM costs. Automatically.**

```
"What is 2+2?"            → DeepSeek        $0.27/M    saved 99%
"Summarize this article"  → GPT-4o-mini     $0.60/M    saved 99%
"Build a React component" → Claude Sonnet   $15.00/M   best balance
"Prove this theorem"      → o3              $10.00/M   reasoning
```

- **30+ models** — OpenAI, Anthropic, Google, DeepSeek, xAI, Moonshot
- **100% local routing** — 14-dimension weighted scoring in <1ms
- **x402 micropayments** — pay per request with USDC on Base

```bash
openclaw plugins install @blockrun/clawrouter
```

---

## How It Works

```
Your App → ClawRouter (localhost) → BlockRun API → 30+ LLMs
               ↓
         Weighted Scorer    →    Model Selector    →    x402 Signer
        (14 dimensions)        (cheapest tier)          (USDC)
```

**Payment IS authentication.** No API keys to manage — your wallet signature proves you can pay.

---

## SDKs

| Language | Package | Install |
|----------|---------|---------|
| Python | [blockrun-llm](https://github.com/BlockRunAI/blockrun-llm) | `pip install blockrun-llm` |
| TypeScript | [blockrun-llm-ts](https://github.com/BlockRunAI/blockrun-llm-ts) | `npm install blockrun-llm` |
| XRPL | [blockrun-llm-xrpl](https://github.com/BlockRunAI/blockrun-llm-xrpl) | `pip install blockrun-llm-xrpl` |

---

## Why BlockRun?

Traditional LLM access requires:
1. Human creates account
2. Human adds payment method
3. Human generates API key
4. Human pastes key into app

**BlockRun requires:**
1. Agent generates wallet
2. Agent receives funds
3. Agent makes requests

Agents shouldn't need humans to paste API keys. They should pay per request — programmatically.

---

<div align="center">

**[Docs](https://blockrun.ai/docs)** · **[Models](https://blockrun.ai/models)** · **[x402 Protocol](https://x402.org)**

Built for agents. Powered by [x402](https://x402.org).

</div>
