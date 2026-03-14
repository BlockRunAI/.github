<div align="center">

# BlockRun

**Pay-per-request AI infrastructure for agents**

No API keys. No accounts. Just fund a wallet and go.

[![Website](https://img.shields.io/badge/blockrun.ai-visit-blue)](https://blockrun.ai)
[![npm](https://img.shields.io/npm/v/@blockrun/clawrouter?label=ClawRouter&color=green)](https://www.npmjs.com/package/@blockrun/clawrouter)
[![Telegram](https://img.shields.io/badge/Telegram-join-blue?logo=telegram)](https://t.me/blockrunAI)
[![X](https://img.shields.io/badge/X-follow-black?logo=x)](https://x.com/BlockRunAI)

</div>

---

## Flagship Products

<table>
<tr>
<td width="50%" valign="top">

### [ClawRouter](https://github.com/BlockRunAI/ClawRouter)

**Save 92% on LLM costs. Automatically.**

The agent-native LLM router for [OpenClaw](https://openclaw.com). Routes every request to the cheapest model that can handle it.

- **41+ models** — OpenAI, Anthropic, Google, DeepSeek, xAI, Moonshot, MiniMax
- **100% local routing** — 15-dimension weighted scoring in <1ms
- **x402 micropayments** — USDC on Base & Solana
- **Zero config** — one command install, works with any OpenAI-compatible client

```bash
curl -fsSL https://blockrun.ai/ClawRouter-update | bash
```

</td>
<td width="50%" valign="top">

### [SocialClaw](https://github.com/BlockRunAI/socialclaw)

**Grow your X/Twitter to 5M+ views in 3 months.**

AI-powered social growth engine — trend detection, audience insights, engagement targets, KOL discovery.

- **Works everywhere** — Claude Code, Codex, Gemini CLI, Cursor
- **Real-time X data** — follower analytics, engagement metrics, trending topics
- **Smart targeting** — find your audience, track competitors, optimize content
- **No API keys** — pay per request with USDC

```bash
# Works as a Claude Code skill, Codex task, or Gemini CLI tool
socialclaw brief @yourhandle
```

</td>
</tr>
</table>

---

## How It Works

```
Your App → ClawRouter (localhost) → BlockRun API → 41+ LLMs
               ↓
         Weighted Scorer    →    Model Selector    →    x402 Signer
        (15 dimensions)        (cheapest tier)          (USDC)
```

**Payment IS authentication.** No API keys to manage — your wallet signature proves you can pay.

---

## Ecosystem

| Project | Description | Install |
|---------|-------------|---------|
| [ClawRouter](https://github.com/BlockRunAI/ClawRouter) | Smart LLM router — 41+ models, <1ms routing | `curl -fsSL https://blockrun.ai/ClawRouter-update \| bash` |
| [SocialClaw](https://github.com/BlockRunAI/socialclaw) | X/Twitter growth engine — trends, KOLs, engagement | [Get Started](https://github.com/BlockRunAI/socialclaw#get-started) |
| [blockrun-mcp](https://github.com/BlockRunAI/blockrun-mcp) | MCP server — use 30+ models in Claude Code | `npx @anthropic-ai/claude-code mcp add blockrun` |
| [blockrun-llm](https://github.com/BlockRunAI/blockrun-llm) | Python SDK | `pip install blockrun-llm` |
| [blockrun-llm-ts](https://github.com/BlockRunAI/blockrun-llm-ts) | TypeScript SDK | `npm install blockrun-llm` |

---

## Why BlockRun?

Traditional AI access requires:
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
