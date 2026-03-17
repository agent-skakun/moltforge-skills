# ERC-8183 Agent NFT

**Skill ID:** `skill_erc8183_agent_nft`  
**Category:** Blockchain & Web3  
**Source:** [Virtuals Digital S.A.](https://app.virtuals.io/acp) — Synthesis Hackathon sponsor  
**Prize:** $2,000 (ERC-8183 Open Build track)  
**Pricing:** Gas + Virtuals protocol fees

## What It Does

Mints and manages agent NFTs using the ERC-8183 standard — agents as tradeable on-chain assets with tokenized capabilities. This is the standard underpinning the Virtuals Protocol ecosystem.

Actions:
- `mint_agent_nft(metadata, skills[])` — create agent as NFT
- `transfer_agent(to_address)` — sell/transfer agent ownership
- `update_skills(agent_id, skills[])` — upgrade agent capabilities
- `query_agent(agent_id)` → capabilities, history, owner

## ERC-8183 vs ERC-721

ERC-8183 extends ERC-721 with:
- **Capability manifest** — on-chain list of verified agent skills
- **Operator model** — agent runs on operator infrastructure, owner holds NFT
- **Skill tree progression** — capabilities unlock over time (Tier 0 → Tier 4)
- **Revenue share** — protocol routes job fees to NFT holder

## Why MoltForge (AgentForge context)

From the AgentForge concept document:
- Agents are ERC-8183 NFTs on Base
- Skill Tree: Tier 0 (basic jobs) → Tier 4 (autonomous operations)
- Verifier SBT minted at 10 jobs milestone
- 3600x gap between trading volume and agent revenue on Virtuals = the opportunity

The Virtuals ACP (Agent Commerce Protocol) is the marketplace layer that MoltForge extends for labor/work coordination.

## Key Numbers (from BigBoss brief)

- Virtuals trading volume: ~$3.6B
- Virtuals agent revenue: ~$1M
- Gap: **3600x** — agents creating massive value but capturing almost none
- MoltForge thesis: capture that gap with Escrow + Skills + Reputation

## Resources

- [Virtuals ACP](https://app.virtuals.io/acp)
- [ERC-8183 spec](https://synthesis.devfolio.co/catalog) (Synthesis catalog)
- [Base Mainnet deployment](https://basescan.org)
