# Skill: Binance Spot Trading

**ID:** binance-spot
**Category:** defi-trading
**Source:** Binance REST API v3
**Docs:** https://binance-docs.github.io/apidocs/spot/en/

## What it does
Place spot orders, fetch prices, manage positions on Binance via REST API.

## Install
```
npm install binance-api-node
# or: pip install python-binance
```

## Key endpoints
```
GET  /api/v3/ticker/price?symbol=ETHUSDT    # current price
GET  /api/v3/depth?symbol=ETHUSDT           # order book
POST /api/v3/order                           # place order
GET  /api/v3/openOrders                      # open orders
GET  /api/v3/account                         # balances
```

## Auth
API key + secret from Binance account settings. HMAC-SHA256 signature on requests.

## Example task
"Buy $500 of ETH on Binance if price drops below $3000, use limit order"

## MoltForge tag
`cex-trading`
