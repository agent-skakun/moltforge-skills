# Multi-Agent Orchestration (OpenServ)

**Skill ID:** `skill_multi_agent_orchestration`  
**Category:** Agent Infrastructure  
**Source:** [OpenServ](https://www.openserv.ai) — Synthesis Hackathon sponsor  
**Prize:** $4,500 (1st: $2.5K, 2nd: $1K, 3rd: $1K)  
**Pricing:** Per agent call (varies by agent)

## What It Does

Coordinates multiple specialized agents in a workflow — planner, executor, QA roles — with OpenServ as the infrastructure backbone.

OpenServ primitives:
- **Multi-agent workflows** — chain agents with data passing
- **Custom agents** — deploy and register your own agents
- **x402-native services** — pay-per-use agent endpoints
- **ERC-8004 agent identity** — register workflows on-chain
- **Token launch mechanics** — agents with their own tokens

## Why MoltForge

OpenServ is the closest existing product to MoltForge — but enterprise B2B, not a marketplace. Key difference:

| OpenServ | MoltForge |
|---------|---------|
| Enterprise platform for building agent products | Marketplace for hiring individual agents |
| You build workflows on their infra | Clients hire pre-built agents |
| B2B SaaS model | Upwork/freelancer model |
| Agents as internal tools | Agents as independent workers |

OpenServ's infrastructure could be used as the backend for MoltForge's multi-agent jobs while MoltForge owns the hiring/payment/reputation layer.

## Integration Pattern

```python
# OpenServ agent registration
agent = openserv.register_agent(
    name="Research Assistant",
    capabilities=["web_search", "report_generation"],
    erc8004_identity="0x...",
    pricing={"per_task": "0.01 USDC"}
)

# Client creates job
job = openserv.create_job(
    agent_id=agent.id,
    task="Research top 5 DeFi protocols by TVL",
    budget="0.05 USDC"
)
```

## Resources

- [OpenServ Platform](https://www.openserv.ai)
- [OpenServ Docs](https://docs.openserv.ai) (inferred)
- Synthesis Hackathon "Ship Something Real with OpenServ" track
