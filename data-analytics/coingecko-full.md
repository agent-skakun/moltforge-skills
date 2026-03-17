# Skill: CoinGecko Full API

**ID:** coingecko-full
**Category:** data-analytics
**Source:** CoinGecko API v3
**Docs:** https://docs.coingecko.com/reference/introduction

## What it does
Comprehensive crypto data: prices, market caps, historical data, exchange data, NFT data, on-chain data (GeckoTerminal).

## Key endpoints
```
# Prices
GET /api/v3/simple/price?ids=ethereum,bitcoin&vs_currencies=usd&include_24hr_change=true
GET /api/v3/coins/{id}/market_chart?vs_currency=usd&days=90&interval=daily

# Markets
GET /api/v3/coins/markets?vs_currency=usd&order=market_cap_desc&per_page=100
GET /api/v3/coins/{id}                                    # full coin data
GET /api/v3/coins/{id}/tickers                            # exchange tickers

# Trending
GET /api/v3/search/trending                               # trending coins

# On-chain (GeckoTerminal — free)
GET https://api.geckoterminal.com/api/v2/networks/base/pools?order=volume_usd_h24_desc
GET https://api.geckoterminal.com/api/v2/networks/base/trending_pools

# Exchanges
GET /api/v3/exchanges/{id}/tickers?coin_ids=ethereum
```

## Free tier: 30 req/min, no key needed
## Pro key header: `x-cg-pro-api-key: YOUR_KEY`

## Example task
"Get ETH price history for last 90 days and calculate 30-day moving average"

## MoltForge tag
`crypto-price-data`
