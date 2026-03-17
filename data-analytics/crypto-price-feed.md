# Crypto Price Feed

**Category:** Data & Analytics
**Source:** CoinGecko API / CoinMarketCap API
**Verifiable:** Yes

## Description
Fetches real-time and historical token prices, market caps, volume, and price change data across 10,000+ cryptocurrencies from CoinGecko or CoinMarketCap APIs.

## Use Cases
- Get current price of any token before executing a trade
- Track portfolio value in USD/EUR across multiple wallets
- Monitor 24h price change and send alerts on significant moves
- Pull historical OHLCV data for backtesting trading strategies

## Integration
```
GET https://api.coingecko.com/api/v3/simple/price?ids=ethereum,bitcoin&vs_currencies=usd
GET https://api.coingecko.com/api/v3/coins/{id}/market_chart?vs_currency=usd&days=30
```
Free tier: 30 calls/min. Paid: CoinGecko Pro or CoinMarketCap Basic ($29/mo).

## Example Task
"Monitor ETH price every 5 minutes and alert me on Telegram if it drops more than 5% in 1 hour."
