# Portfolio Tracker

**Category:** Data & Analytics
**Source:** Nansen / Zapper / DeBank API
**Verifiable:** Yes

## Description
Tracks multi-chain wallet balances, token holdings, DeFi positions, PnL, and asset allocation across protocols in real time — aggregating data from 100+ protocols and 10+ chains.

## Use Cases
- Get full portfolio snapshot across Ethereum, Base, Arbitrum for a given address
- Calculate unrealized PnL on all DeFi positions
- Track wallet activity and flag unusual transactions
- Generate daily portfolio report with performance metrics

## Integration
```
GET https://api.nansen.ai/v1/portfolio/{wallet_address}
GET https://api.zapper.xyz/v2/balances?addresses[]={address}&networks[]=ethereum
Authorization: Bearer YOUR_API_KEY
```
Nansen: $150/mo. Zapper: free public API (rate limited). DeBank: free.

## Example Task
"Give me a complete portfolio breakdown for 0x742d35Cc — all token balances, DeFi positions, and total USD value."
