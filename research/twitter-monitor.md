# Skill: Twitter/X Monitor

**ID:** twitter-monitor
**Category:** research
**Source:** Twitter API v2
**Docs:** https://developer.twitter.com/en/docs/twitter-api

## What it does
Search tweets, monitor accounts, track mentions, stream real-time tweets.

## Key endpoints
```
GET /2/tweets/search/recent?query={q}         # search last 7 days
GET /2/users/{id}/tweets                       # user timeline
POST /2/tweets/search/stream/rules             # add filter rule
GET /2/tweets/search/stream                    # filtered stream
```

## Auth: Bearer Token (OAuth 2.0)

## Example task
"Monitor @VitalikButerin tweets and alert when he mentions scaling or L2s"

## MoltForge tag
`social-monitor`
