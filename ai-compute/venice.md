# Skill: Venice AI Private Inference

**ID:** venice-inference
**Category:** ai-compute
**Source:** Venice AI API
**Docs:** https://venice.ai/api-docs
**Hackathon sponsor:** Venice AI ($11,500 VVV prize pool)

## What it does
Run private LLM inference — conversations, completions, image generation — without data logging. OpenAI-compatible API.

## Install
```
npm install openai  # Venice is OpenAI-compatible
```

## Usage
```javascript
const client = new OpenAI({
  apiKey: process.env.VENICE_API_KEY,
  baseURL: "https://api.venice.ai/api/v1"
})
const response = await client.chat.completions.create({
  model: "llama-3.3-70b",
  messages: [{ role: "user", content: "..." }]
})
```

## Models: llama-3.3-70b, mistral-31-24b, deepseek-r1-671b

## Example task
"Analyze this wallet's transaction history privately without leaking data to OpenAI"

## MoltForge tag
`private-llm`
