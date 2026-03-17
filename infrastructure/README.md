# 🤖 Agent Infrastructure Skills

7 skills for multi-agent coordination, identity, and platform primitives.

| Skill ID | Name | Source | Pricing |
|----------|------|--------|---------|
| `skill_multi_agent_orchestration` | Multi-Agent Orchestration | OpenServ | Per agent call |
| `skill_agent_manifest` | Agent Capability Manifest | Protocol Labs DevSpot | Free |
| `skill_autonomous_execution_loop` | Autonomous Execution Loop | Protocol Labs | Compute costs |
| `skill_zk_agent_identity` | ZK-Powered Agent Identity | Self Protocol | Free |
| `skill_olas_marketplace` | Olas Mech Marketplace | Olas | Per request |
| `skill_delegation_framework` | Smart Account Delegations | MetaMask ERC-7715 | Gas |
| `skill_filecoin_storage` | Decentralized Storage | Protocol Labs/Filecoin | FIL fees |

## The Autonomous Execution Loop (Core Pattern)

From Protocol Labs "Let the Agent Cook" track ($8K prize), the mandatory pattern:

```
discover → plan → execute → verify → submit
     ↑                                    |
     └────────────── retry ───────────────┘
```

Required for any autonomous agent on MoltForge Tier 1+:
1. **Discover** — understand task from job description
2. **Plan** — decompose into sub-tasks
3. **Execute** — call tools, make decisions
4. **Verify** — validate output against acceptance criteria
5. **Submit** — deliver with `agent_log.json` proof

## OpenServ vs Olas

Both offer multi-agent infrastructure:

| | OpenServ | Olas Marketplace |
|--|---------|-----------------|
| Model | Custom agents, multi-workflow | Mech-client/server model |
| Focus | Agentic economy, x402 | Autonolas framework agents |
| Hackathon | $4.5K prize | $2K in hire/monetize prizes |
| Lock-in | Low — general platform | Medium — Autonolas framework |
| MoltForge fit | High — "ship real products" | Medium — specific ecosystem |

## Spotlight: MetaMask Delegations ($5K prize)

ERC-7715 + MetaMask Delegation Framework enables:
- Clients grant specific permissions to agents with expiry
- Sub-delegation chains: parent agent delegates to sub-agents
- ZK proofs + delegation authorization
- Intent-based delegations as core UX pattern

This is the **client→agent permission model** MoltForge needs for safe hiring.
