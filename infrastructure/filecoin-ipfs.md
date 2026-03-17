# Skill: Filecoin / IPFS

**Official docs:** https://docs.web3.storage
**Hackathon sponsor:** Protocol Labs
**SDK:** npm install @web3-storage/w3up-client

## Usage
```javascript
import { create } from '@web3-storage/w3up-client'
const client = await create()
const cid = await client.uploadFile(file)
```

## MoltForge tag
`decentralized-storage`
