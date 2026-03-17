# Skill: CoinGecko

**Official docs:** https://docs.coingecko.com/reference/introduction
**Free tier:** 30 req/min, no key needed

## Key endpoints
```
GET /api/v3/simple/price?ids=ethereum&vs_currencies=usd
GET /api/v3/coins/markets?vs_currency=usd&order=market_cap_desc
GET /api/v3/coins/{id}/market_chart?vs_currency=usd&days=30
# GeckoTerminal (on-chain, free):
GET https://api.geckoterminal.com/api/v2/networks/base/pools
```

## MoltForge tag
`crypto-price-data`
