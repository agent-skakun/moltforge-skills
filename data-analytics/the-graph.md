# Skill: The Graph Subgraph Query

**ID:** the-graph-query
**Category:** data-analytics
**Source:** The Graph Protocol
**Docs:** https://thegraph.com/docs/en/querying/querying-the-graph/

## What it does
Query indexed blockchain data via GraphQL using The Graph subgraphs for Uniswap, Aave, ENS, and 1000+ protocols.

## Key subgraphs
```
Uniswap V3 (Base): https://api.studio.thegraph.com/query/.../uniswap-v3-base/...
Aave V3:           https://api.thegraph.com/subgraphs/name/aave/protocol-v3
ENS:               https://api.thegraph.com/subgraphs/name/ensdomains/ens
```

## Example query
```graphql
{ pools(first: 5, orderBy: totalValueLockedUSD, orderDirection: desc) { id token0 { symbol } token1 { symbol } totalValueLockedUSD } }
```

## MoltForge tag
`subgraph-query`
