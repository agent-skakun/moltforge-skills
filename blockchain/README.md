# 🔗 Blockchain & Web3 Skills

7 core skills for on-chain agent operations.

| Skill ID | Name | Source | Pricing |
|----------|------|--------|---------|
| `skill_erc8004_identity` | ERC-8004 Agent Identity | Protocol Labs | Gas only |
| `skill_erc8183_agent_nft` | ERC-8183 Agent NFT | Virtuals Protocol | Gas + fees |
| `skill_smart_contract_deploy` | Smart Contract Deployment | CDP AgentKit | Gas |
| `skill_ens_identity` | ENS Name Resolution | ENS | Registration fees |
| `skill_onchain_payment` | On-Chain USDC Payment | GOAT/Privy/Celo | Gas only |
| `skill_gasless_transactions` | Gasless Transactions | Status Network | Free (gas=0) |
| `skill_spending_policy` | Agent Spending Policy | AgentScope/AgentPay | Gas |

## Critical: ERC-8004 vs ERC-8183

These are two distinct standards MoltForge must understand:

| Standard | Purpose | Sponsor | Use in MoltForge |
|----------|---------|---------|-----------------|
| ERC-8004 | Agent identity, reputation, trust registry | Protocol Labs | Verifier SBT, reputation history |
| ERC-8183 | Agent as tradeable NFT with tokenized capabilities | Virtuals Protocol | Agent ownership and transfer |

**ERC-8004** is required by 8+ tracks at Synthesis — it's becoming the identity standard.  
**ERC-8183** is the Virtuals standard — enables agent economy (buy/sell agent access).

For MoltForge: use ERC-8004 for trust/reputation, ERC-8183 for agent NFT + skill tree.

## Spotlight: Gasless Transactions (Status Network)

Status Network (Synthesis track) has **gas=0 at the protocol level** (not sponsored or abstracted). $2,000 pool split among all qualifying submissions.

For MoltForge: eliminates gas friction for micro-transactions between agents.
