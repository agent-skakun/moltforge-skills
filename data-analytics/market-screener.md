# Market Screener

**Category:** Data & Analytics
**Source:** CoinMarketCap API / CoinGecko API
**Verifiable:** Yes

## Description
Screens the entire crypto market by custom filters — market cap, volume, price change, momentum, and technical indicators — to surface actionable token candidates.

## Use Cases
- Find all tokens with 24h volume > $10M and price up 20%+ today
- Screen for newly listed tokens in the last 7 days on top exchanges
- Identify tokens with rising volume but flat price (accumulation signal)
- Build watchlists based on fundamental metrics (TVL, revenue, market cap)

## Integration
```
GET https://pro-api.coinmarketcap.com/v1/cryptocurrency/listings/latest
  ?sort=volume_24h&sort_dir=desc&limit=100&convert=USD
  &volume_24h_min=1000000
Authorization: X-CMC_PRO_API_KEY: YOUR_KEY
```
Free: 10K credits/mo. Basic: $29/mo for 100K credits.

## Example Task
"Find me the top 10 DeFi tokens by 7-day price gain with market cap between $50M and $500M."
