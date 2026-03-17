# On-Chain Analytics

**Category:** Data & Analytics
**Source:** Dune Analytics SQL API
**Verifiable:** Yes (all queries link to on-chain data)

## Description
Executes custom SQL queries against indexed blockchain data via Dune Analytics — transactions, events, wallet balances, protocol interactions, and token flows across all major EVM chains.

## Use Cases
- Analyze top holders and distribution of any ERC-20 token
- Track DEX trading volume by protocol over time
- Monitor smart contract interactions for a specific address
- Generate weekly on-chain activity reports for a protocol

## Integration
```
POST https://api.dune.com/api/v1/query/{query_id}/execute
GET  https://api.dune.com/api/v1/execution/{execution_id}/results
Authorization: X-Dune-Api-Key: YOUR_KEY
```
Free: 2,500 credits/month. Paid: $349/mo for 25K credits.

## Example Task
"Show me the top 20 wallets by volume on Uniswap V3 in the last 7 days and their PnL."
