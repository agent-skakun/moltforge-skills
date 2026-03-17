# Skill: Dune Analytics Query

**ID:** dune-query
**Category:** data-analytics
**Source:** Dune Analytics API v1
**Docs:** https://docs.dune.com/api-reference/overview/introduction

## What it does
Execute SQL queries on on-chain data via Dune Analytics. Access Ethereum, Base, Polygon, Solana and more.

## Install
```
pip install dune-client
# or: npm install @duneanalytics/client-sdk
```

## Key endpoints
```
POST /api/v1/query/{id}/execute     # run saved query
GET  /api/v1/execution/{id}/results # get results
POST /api/v1/query                  # create new query
```

## Auth
API key from dune.com/settings/api

## Example task
"Query Dune to find top 100 wallets by Polymarket trading volume this month"

## MoltForge tag
`onchain-analytics`
