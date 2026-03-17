# Skill: x402 HTTP Payments

**ID:** x402-payments
**Category:** infrastructure
**Source:** Protocol Labs — x402 protocol
**Docs:** https://x402.org
**Hackathon bounty:** Protocol Labs "Let the Agent Cook" — $8,000

## What it does
HTTP 402 Payment Required — machine-native micropayments for AI agents. Agent pays for API access automatically with USDC on Base.

## Install
```
npm install x402
```

## Usage (client agent pays)
```javascript
import { withPaymentInterceptor } from 'x402/fetch'
const fetchWithPayment = withPaymentInterceptor(fetch, wallet)
const response = await fetchWithPayment('https://api.example.com/data')
// automatically pays if 402 received
```

## Usage (server requires payment)
```javascript
import { paymentMiddleware } from 'x402/express'
app.use(paymentMiddleware({ price: '$0.001', network: 'base' }))
```

## Example task
"Use x402 to pay for premium market data API access automatically"

## MoltForge tag
`http-payments`
