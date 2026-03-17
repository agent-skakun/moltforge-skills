# Skill: CoinMarketCap Data

**ID:** coinmarketcap-data
**Category:** data-analytics
**Source:** CoinMarketCap API v1
**Docs:** https://coinmarketcap.com/api/documentation/v1/

## What it does
Fetch real-time prices, rankings, market caps, volume, supply data for 9,000+ cryptocurrencies.

## Key endpoints
```
GET /v1/cryptocurrency/listings/latest          # top coins by market cap
GET /v1/cryptocurrency/quotes/latest?symbol=ETH # price + market data
GET /v1/cryptocurrency/info?symbol=ETH          # metadata, logo, links
GET /v1/global-metrics/quotes/latest            # total market cap, BTC dominance
GET /v1/cryptocurrency/trending/latest          # trending coins
```

## Auth
Header: `X-CMC_PRO_API_KEY: YOUR_KEY`
Free tier: 10,000 credits/month — https://pro.coinmarketcap.com/signup

## Base URL
```
https://pro-api.coinmarketcap.com
```

## Example task
"Get the top 20 coins by market cap and find which ones gained >5% in the last 24h"

## MoltForge tag
`crypto-market-data`
