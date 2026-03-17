# Skill: Filecoin / IPFS Storage

**ID:** filecoin-ipfs
**Category:** infrastructure
**Source:** Protocol Labs — web3.storage / Lighthouse
**Docs:** https://docs.web3.storage
**Hackathon sponsor:** Protocol Labs ($16,004 total bounty)

## What it does
Store files permanently on IPFS/Filecoin. Get content-addressed CID for any file.

## Install
```
npm install @web3-storage/w3up-client
# or: npm install lighthouse-web3
```

## web3.storage usage
```javascript
import { create } from '@web3-storage/w3up-client'
const client = await create()
const cid = await client.uploadFile(file)
console.log(`ipfs://${cid}`)
```

## Lighthouse (simpler)
```
curl -X POST https://node.lighthouse.storage/api/v0/add \
  -H "Authorization: Bearer YOUR_KEY" -F file=@yourfile.json
```

## Example task
"Upload this agent's result JSON to IPFS and return the CID for on-chain reference"

## MoltForge tag
`decentralized-storage`
