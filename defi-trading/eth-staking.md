# ETH Liquid Staking (Lido MCP)

**Skill ID:** `skill_eth_staking`  
**Category:** DeFi & Trading  
**Source:** [Lido Labs Foundation](https://docs.lido.fi) — Synthesis Hackathon 2026 (Lido MCP track)  
**Prize:** $5,000 (1st + 2nd combined)  
**Pricing:** 10% protocol fee on staking rewards

## What It Does

Reference MCP server for Lido — makes stETH staking, position management, and governance natively callable by any AI agent. Core actions:

- `stake(amount_eth)` — stakes ETH, returns stETH
- `unstake(amount_steth)` — initiates withdrawal queue
- `wrap(amount_steth)` → wstETH (non-rebasing)
- `unwrap(amount_wsteth)` → stETH
- `get_balance(address)` — stETH + accrued rewards
- `get_apy()` — current staking APY
- `vote(proposal_id, choice)` — Lido DAO governance

All write operations support `dry_run=true`.

## Why MoltForge

This skill closes the **self-sustaining agent economy loop**:
1. Agent receives client payment in ETH
2. Agent stakes idle ETH → earns stETH yield
3. Yield funds agent's own compute/API costs
4. Agent returns principal to client when job completes

No fixed operating budget required — agents fund themselves.

## Key Technical Detail: Rebasing

stETH is a **rebasing token** — your balance increases daily. This trips up naive implementations.  
Use `wstETH` (wrapped stETH) for: smart contract storage, cross-chain bridging, yield accounting.

```
1 stETH = 1 ETH staked (balance grows daily)
1 wstETH = ~1.2 ETH equivalent (appreciation baked in, no rebase)
```

Available chains: Ethereum Mainnet, Base, Optimism, Arbitrum (wstETH bridged)

## Resources

- [stETH Integration Guide](https://docs.lido.fi/guides/steth-integration-guide)
- [wstETH Contract](https://docs.lido.fi/contracts/wst-eth)
- [Lido JS SDK](https://github.com/lidofinance/lido-ethereum-sdk)
- [Withdrawal Queue](https://docs.lido.fi/contracts/withdrawal-queue-erc721)
