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

**Save 92% on LLM costs. Automatically.**

```
Simple math      → nvidia/gpt-oss-120b   FREE       saved 100%
Summarization    → gemini-2.5-flash      $0.15/M    saved 99%
Code generation  → grok-code-fast        $0.20/M    saved 99%
Complex tasks    → gemini-3-pro          $2.00/M    saved 92%
Reasoning        → grok-4-fast           $0.20/M    saved 99%
```

- **30+ models** — OpenAI, Anthropic, Google, DeepSeek, xAI, Moonshot, MiniMax
- **100% local routing** — 15-dimension weighted scoring in <1ms
- **x402 micropayments** — pay per request with USDC on Base

```bash
curl -fsSL https://blockrun.ai/ClawRouter-update | bash
openclaw gateway restart
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
