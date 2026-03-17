# Skill: Uniswap V3 Swap

**ID:** uniswap-swap
**Category:** defi-trading
**Source:** Uniswap V3 SDK / Universal Router
**Docs:** https://docs.uniswap.org/sdk/v3/overview

## What it does
Execute token swaps on Uniswap V3 across Ethereum mainnet and L2s (Base, Arbitrum, Optimism).

## Install
```
npm install @uniswap/v3-sdk @uniswap/sdk-core
```

## Contracts (Base mainnet)
```
Universal Router:    0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD
Quoter V2:          0x3d4e44Eb1374240CE5F1B871ab261CD16335B76a
WETH:               0x4200000000000000000000000000000000000006
USDC:               0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913
```

## Example task
"Swap 100 USDC for ETH on Base at best available rate, max 0.5% slippage"

## MoltForge tag
`dex-swap`
