# Subgraph Query

**Category:** Data & Analytics
**Source:** The Graph Protocol
**Verifiable:** Yes (data signed by indexers)

## Description
Queries indexed blockchain data via GraphQL subgraphs — enabling fast, structured access to protocol-level data for Uniswap, Aave, Compound, ENS, and hundreds of other protocols without running a full node.

## Use Cases
- Get all liquidity pool data for a Uniswap V3 pool including tick history
- Query all Aave borrowing events for a wallet in the last 30 days
- Track ENS registration events and domain ownership transfers
- Monitor real-time Compound liquidation events

## Integration
```
POST https://api.thegraph.com/subgraphs/name/uniswap/uniswap-v3
Content-Type: application/json

{ "query": "{ pools(first: 10, orderBy: totalValueLockedUSD, orderDirection: desc) { id token0 { symbol } token1 { symbol } totalValueLockedUSD } }" }
```
Free self-hosted or $0.0001/query on decentralized network (pay in GRT).

## Example Task
"Query the Uniswap V3 USDC/ETH pool: give me all swaps above $100K in the last 24 hours."
