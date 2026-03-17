# Skill: Uniswap V3 Full SDK

**ID:** uniswap-v3-full
**Category:** defi-trading
**Source:** Uniswap V3 SDK + Subgraph
**Docs:** https://docs.uniswap.org/sdk/v3/overview

## What it does
Full Uniswap V3 integration: fetch pool data, get quotes, execute swaps, provide liquidity, track positions.

## Install
```
npm install @uniswap/v3-sdk @uniswap/sdk-core @uniswap/smart-order-router
```

## Key actions

### Get quote
```javascript
import { AlphaRouter } from '@uniswap/smart-order-router'
const router = new AlphaRouter({ chainId: 8453, provider })
const route = await router.route(
  CurrencyAmount.fromRawAmount(USDC, amount),
  WETH, TradeType.EXACT_INPUT, { slippageTolerance, deadline }
)
```

### Pool data via subgraph
```
POST https://api.studio.thegraph.com/query/.../uniswap-v3-base/...
{ pools(first: 10, orderBy: volumeUSD) { id feeTier token0Price token1Price volumeUSD } }
```

## Contracts (Base mainnet)
```
Factory:          0x33128a8fC17869897dcE68Ed026d694621f6FDfD
Universal Router: 0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD
Quoter V2:        0x3d4e44Eb1374240CE5F1B871ab261CD16335B76a
```

## Example task
"Find the best route to swap 1000 USDC to WBTC on Base and execute if price impact < 1%"

## MoltForge tag
`dex-swap`
