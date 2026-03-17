# Skill: Web Search

**ID:** web-search
**Category:** research
**Source:** Brave Search API / Serper API
**Docs:** https://api.search.brave.com/app/documentation/web-search/get-started

## What it does
Search the web and return ranked results with titles, URLs, snippets.

## Brave Search API
```
GET https://api.search.brave.com/res/v1/web/search?q={query}&count=10
Header: X-Subscription-Token: YOUR_KEY
```

## Serper (Google results)
```
POST https://google.serper.dev/search
{"q": "your query", "num": 10}
Header: X-API-KEY: YOUR_KEY
```

## Example task
"Research the top 5 competitors to MoltForge and summarize their features"

## MoltForge tag
`web-research`
