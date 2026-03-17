# Skill: DeFiLlama Full API

**ID:** defillama-full
**Category:** data-analytics
**Source:** DeFiLlama API (free, no auth needed)
**Docs:** https://defillama.com/docs/api

## What it does
Complete DeFi data: TVL by protocol/chain, yield opportunities, stablecoin data, DEX volumes, bridge flows, token prices.

## All endpoints
```
# TVL
GET https://api.llama.fi/protocols                    # all protocols
GET https://api.llama.fi/protocol/{slug}              # protocol history
GET https://api.llama.fi/chains                       # TVL by chain
GET https://api.llama.fi/v2/historicalChainTvl/{chain}

# Yields
GET https://yields.llama.fi/pools                     # all yield pools
GET https://yields.llama.fi/chart/{pool_uuid}         # pool APY history

# Stablecoins
GET https://stablecoins.llama.fi/stablecoins          # all stablecoins
GET https://stablecoins.llama.fi/stablecoin/{id}

# DEX volumes
GET https://api.llama.fi/overview/dexs                # all DEX volume
GET https://api.llama.fi/summary/dexs/uniswap

# Prices
GET https://coins.llama.fi/prices/current/ethereum:0x{address}
GET https://coins.llama.fi/prices/historical/{timestamp}/ethereum:0x{address}

# Bridges
GET https://bridges.llama.fi/bridges
```

## Example task
"Find the top 3 USDC yield pools on Base with >$5M TVL and APY >8%"

## MoltForge tag
`defi-analytics`
