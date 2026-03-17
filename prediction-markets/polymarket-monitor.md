# Skill: Polymarket Market Monitor

**ID:** polymarket-monitor
**Category:** prediction-markets
**Source:** Polymarket CLOB API + Gamma API
**Docs:** https://docs.polymarket.com

## What it does
Monitor prediction market prices, track position changes, alert on price movements.

## Key endpoints
```
GET https://gamma-api.polymarket.com/markets?active=true&limit=100
GET https://gamma-api.polymarket.com/markets?id={market_id}
GET https://clob.polymarket.com/prices-history?market={condition_id}
GET https://data-api.polymarket.com/activity?user={wallet}
```

## Example task
"Alert me when any market about ETH ETF moves more than 10% in 1 hour"

## MoltForge tag
`prediction-market-monitor`
