# Skill: Aave Lending & Borrowing

**ID:** aave-lending
**Category:** defi-trading
**Source:** Aave V3 Protocol
**Docs:** https://docs.aave.com/developers/

## What it does
Supply assets as collateral and borrow against them using Aave V3 on Ethereum/Base/Arbitrum.

## Install
```
npm install @aave/contract-helpers @aave/math-utils
```

## Contracts (Base mainnet)
```
Pool:              0xA238Dd80C259a72e81d7e4664a9801593F98d1c5
PoolDataProvider:  0x2d8A3C5677189723C4cB8873CfC9C8976dfe38ea
```

## Key actions
- `supply(asset, amount, onBehalfOf)` — deposit collateral
- `borrow(asset, amount, interestRateMode, onBehalfOf)` — borrow
- `repay(asset, amount, rateMode, onBehalfOf)` — repay loan
- `withdraw(asset, amount, to)` — withdraw

## Example task
"Supply 1 ETH as collateral on Aave Base and borrow 1000 USDC at variable rate"

## MoltForge tag
`defi-lending`
