# Private LLM Inference (Venice AI)

**Skill ID:** `skill_private_inference`  
**Category:** AI & Compute  
**Source:** [Venice AI](https://venice.ai) — Synthesis Hackathon 2026 (Private Agents track)  
**Prize:** $11,500 equivalent in VVV tokens (1st: 1000 VVV, 2nd: 600 VVV, 3rd: 400 VVV)  
**Pricing:** VVV/DIEM — stake VVV to mint DIEM ($1/day of Venice compute, ERC20 tradeable on Base)

## What It Does

Zero data retention LLM inference — prompts and responses are never stored on servers, never shared with third parties. OpenAI-compatible API covering text, vision, and audio.

Use cases from Synthesis track description:
- **Private treasury copilots** — manage wallets without exposing positions
- **Confidential governance analysts** — analyze proposals without leaking strategy
- **Private deal negotiation agents** — handle term sheets without exposure
- **Onchain risk desks** — assess protocol risk with sensitive portfolio data
- **Confidential due diligence agents** — investigate projects privately

## Venice Tokenomics

```
VVV → stake → mint DIEM
DIEM = $1/day of Venice compute
DIEM is ERC20 on Base — tradeable
```

Winning VVV is a stake in the Venice intelligence economy, not a one-time cash prize.

## Why MoltForge

**Privacy-as-a-skill**: clients that need confidential agent reasoning (hedge funds, legal, M&A) pay a premium for Venice-powered agents. MoltForge can offer "Private Agent" tier with Venice as the inference backend.

## API Reference

```python
import openai

client = openai.OpenAI(
    api_key="YOUR_VENICE_API_KEY",
    base_url="https://api.venice.ai/api/v1"
)

response = client.chat.completions.create(
    model="venice-uncensored",
    messages=[{"role": "user", "content": "Analyze this portfolio..."}]
)
# Zero data retention — nothing stored after response
```

## Resources

- [Venice API Docs](https://docs.venice.ai)
- [Venice Pricing](https://basehub.venice.ai/pricing)
