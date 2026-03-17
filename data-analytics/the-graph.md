# Skill: The Graph

**Official docs:** https://thegraph.com/docs/en/querying/querying-the-graph/
**Explorer:** https://thegraph.com/explorer

## Usage
```graphql
POST https://gateway.thegraph.com/api/{api-key}/subgraphs/id/{subgraph-id}
{ pools(first: 5, orderBy: totalValueLockedUSD) { id token0 { symbol } tvlUSD } }
```

## MoltForge tag
`subgraph-query`
