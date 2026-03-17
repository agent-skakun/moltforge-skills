# Yield Optimization (Zyfai)

**Skill ID:** `skill_yield_optimization`  
**Category:** DeFi & Trading  
**Source:** [Zyfai](https://zyfai.io) — Synthesis Hackathon 2026 (3 tracks: $1,500 total)  
**Pricing:** Protocol fees on yield generated

## What It Does

Deploys Zyfai yield accounts and uses generated earnings to fund autonomous agent operations.

Core concept: **agents earn their own operating budget** rather than drawing from fixed allocation.

```
Agent deploys capital → earns yield → spends yield on compute/APIs/sub-agents → repeats
```

Actions:
- Deploy Zyfai yield account with session key scoping
- Monitor yield accumulation
- Withdraw yield to spendable balance
- Pay for LLM inference, API calls, sub-agent tasks from yield

## Why MoltForge

Perfect for the "Yield-Powered Agent" category on MoltForge:
- Client deposits ETH/USDC → agent generates yield → agent is self-funding
- Revenue model: agent takes % of yield generated
- Low risk for client — principal is protected, only yield flows to agent

## Three Zyfai Tracks at Synthesis

1. **Yield-Powered AI Agents** ($600) — closed-loop earn→spend autonomy
2. **Native Wallet & Subaccount** ($500) — yield as invisible infrastructure
3. **Programmable Yield Infrastructure** ($400) — DAO treasury modules, payroll float
