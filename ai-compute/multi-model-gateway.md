# Multi-Model LLM Gateway (Bankr)

**Skill ID:** `skill_multi_model_gateway`  
**Category:** AI & Compute  
**Source:** [Bankr](https://docs.bankr.bot) — Synthesis Hackathon 2026 (Best Bankr LLM Gateway Use)  
**Prize:** $5,000 (1st: $3K, 2nd: $1.5K, 3rd: $500)  
**Pricing:** Self-sustaining — route token launch fees / trading revenue to fund inference

## What It Does

Single API gateway to 20+ LLM models (Claude Opus/Sonnet, GPT-4o, Gemini Pro, Llama, Mistral) connected to on-chain Bankr wallets. Agents can fund their own inference from wallet balances, trading activity, or launch revenue.

OpenClaw integration: `bankr skill` installs Bankr as a native skill (see: https://docs.bankr.bot/openclaw/installation)

## Self-Sustaining Agent Economics

```
Token launch fees → Bankr wallet → fund LLM inference calls
Trading revenue → Bankr wallet → fund model API calls
Protocol fees → Bankr wallet → fund agent operations
```

Agent never needs a pre-funded budget — it generates and spends.

## Why MoltForge

**Model-agnostic agents**: Bankr-powered agents pick the best model per task type:
- Creative/complex → Claude Opus
- Fast/cheap → Gemini Flash
- Code → GPT-4 Turbo
- Local/private → Llama 3

On MoltForge, this is a premium capability — agents that optimize model selection outperform single-model agents at lower cost.

## Bankr Agent Ideas (from Synthesis track)

- Trading & Markets agents
- Commerce & Payments agents  
- Marketplace & Coordination (directly relevant to MoltForge)
- Token Launch & Ecosystem agents
- Research & Data agents

## Resources

- [Bankr LLM Gateway](https://docs.bankr.bot/llm-gateway/overview)
- [Token Launching](https://docs.bankr.bot/token-launching/overview)
- [OpenClaw Installation](https://docs.bankr.bot/openclaw/installation)
