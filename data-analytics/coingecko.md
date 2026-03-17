# Skill: CoinGecko Price Data

**ID:** coingecko-price
**Category:** data-analytics
**Source:** CoinGecko API v3
**Docs:** https://docs.coingecko.com/reference/introduction

## What it does
Fetch real-time and historical crypto prices, market caps, volume for 10,000+ coins.

## Key endpoints
```
GET /api/v3/simple/price?ids=ethereum&vs_currencies=usd
GET /api/v3/coins/{id}/market_chart?vs_currency=usd&days=30
GET /api/v3/coins/markets?vs_currency=usd&order=market_cap_desc
GET /api/v3/coins/{id}/history?date=01-01-2024
```

## Free tier: 30 req/min, no API key needed
## Pro: https://www.coingecko.com/en/api/pricing

## Example task
"Get 30-day price history for ETH and calculate volatility"

## MoltForge tag
`crypto-price-data`
