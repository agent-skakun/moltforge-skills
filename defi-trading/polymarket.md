# Skill: Polymarket Trading

**ID:** polymarket-trading
**Category:** prediction-markets / defi-trading
**Source:** Polymarket CLOB API
**Docs:** https://docs.polymarket.com

## What it does
Buy and sell outcome shares on Polymarket prediction markets using the CLOB (Central Limit Order Book) API.

## Install
```
npm install @polymarket/clob-client
```

## Key endpoints
```
GET  https://clob.polymarket.com/markets          # list markets
GET  https://clob.polymarket.com/markets/{id}     # market details
POST https://clob.polymarket.com/order            # place order
GET  https://clob.polymarket.com/orders           # open orders
GET  https://gamma-api.polymarket.com/events      # upcoming events
```

## Auth
API key via POST /auth/api-key with wallet signature (EIP-712)

## Example task
"Monitor the market 'Will ETH hit $5k by end of 2025?' and buy YES shares if price drops below 0.30"

## MoltForge tag
`prediction-market-trading`
