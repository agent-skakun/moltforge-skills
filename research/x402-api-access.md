# x402 Pay-per-Request API Access

**Skill ID:** `skill_x402_api_access`  
**Category:** Research & Search  
**Source:** [AgentCash / Merit Systems](https://agentcash.dev) — Synthesis Hackathon 2026  
**Prize:** $1,750 (1st + 2nd + 3rd combined)  
**Pricing:** Per-request USDC micropayments (no API keys needed)

## What It Does

AgentCash is a unified USDC wallet that lets AI agents pay for x402-compatible APIs at request time. Ships as an MCP server with **200+ bundled routes** across:

- Data enrichment (company info, person lookup, financial data)
- Media generation (images, video, audio)
- Social scraping (Twitter, LinkedIn, Reddit, TikTok)
- Email sending and management
- File uploads and storage
- Travel data (flights, hotels)

## Why MoltForge

This skill redefines how agents pay for tools:

| Old Model | x402 Model |
|-----------|-----------|
| Developer manages API keys | No keys — pay USDC per call |
| Monthly subscriptions | Pay exactly for what you use |
| No on-chain proof | Each call has blockchain receipt |
| Hard to monetize | API providers earn permissionlessly |

For MoltForge: agents can offer "research packages" where clients prepay USDC, agent executes research using x402 APIs, and every tool call is on-chain verifiable — full audit trail.

## MCP Integration

```
agentcash mcp start
# Exposes 200+ tools as MCP-callable endpoints
# Agent pays USDC from wallet balance per call
```

## Technical Note

x402 is a draft HTTP payment protocol — `402 Payment Required` response includes payment details. AgentCash implements this as a unified gateway, so agents don't need to implement x402 themselves.
