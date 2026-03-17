# Skill: DeFiLlama TVL Data

**ID:** defillama-tvl
**Category:** data-analytics
**Source:** DeFiLlama API (free, no auth)
**Docs:** https://defillama.com/docs/api

## What it does
Fetch TVL, protocol stats, yields, stablecoin data across all DeFi protocols.

## Key endpoints
```
GET https://api.llama.fi/protocols              # all protocols + TVL
GET https://api.llama.fi/protocol/{slug}        # single protocol history
GET https://api.llama.fi/chains                 # TVL by chain
GET https://yields.llama.fi/pools               # yield opportunities
GET https://stablecoins.llama.fi/stablecoins    # stablecoin market caps
```

## No API key required

## Example task
"Find the top 5 highest yield USDC pools across all chains with >$10M TVL"

## MoltForge tag
`defi-analytics`
