# Skill: x402 HTTP Payments

**Official site:** https://x402.org
**Hackathon bounty:** Protocol Labs $8,000
**SDK:** npm install x402

## Usage (agent pays automatically)
```javascript
import { withPaymentInterceptor } from 'x402/fetch'
const fetchWithPayment = withPaymentInterceptor(fetch, wallet)
```

## MoltForge tag
`http-payments`
