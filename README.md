
# 🚀 X (Twitter) Advanced Search Tweet Scraper 𝕏

> **The Ultimate Twitter/X Search & Scraper for Developers, Researchers, AI Teams, Marketers, Journalists, Growth Teams, and Businesses.**

Search, scrape, analyze, and export public Twitter/X data without relying on the official Twitter API. Built for speed, flexibility, and scale with **60+ advanced filters**, structured outputs, and seamless integrations.

---

# Table of Contents

- Features
- Why Choose This Actor
- Use Cases
- Search Examples
- Quick Start
- API Examples
- Search Recipes
- Showcase
- Integrations
- FAQ
- Best Practices
- Roadmap
- Support

---

# ✨ Features

- ✅ No official Twitter/X API required
- ✅ 60+ advanced search filters
- ✅ Search by keyword, hashtag, username, mentions
- ✅ Date, language & location filters
- ✅ Engagement filters (likes, replies, retweets)
- ✅ Verified & Twitter Blue filtering
- ✅ Media search (images, videos, GIFs, Spaces)
- ✅ Conversation & quote tweet support
- ✅ JSON, CSV, Excel & XML export
- ✅ Rich structured metadata
- ✅ Built for AI, analytics & automation

---

# 🚀 Why Choose This Actor?

Unlike basic scrapers, this actor combines Twitter Advanced Search Operators with structured filtering to help you discover exactly the public data you need.

Perfect for:

- AI Training
- Lead Generation
- Social Listening
- Brand Monitoring
- Competitor Analysis
- Market Research
- Journalism
- Academic Research
- Crypto & Stock Monitoring
- Product Research

---

# 💼 Real-World Use Cases

## Marketing

- Brand monitoring
- Campaign tracking
- Trend discovery

## Sales

- Lead generation
- Prospect discovery
- Startup research

## AI & Data Science

- LLM datasets
- RAG pipelines
- Sentiment analysis
- Topic clustering

## Finance

- Crypto sentiment
- Stock discussions
- Market intelligence

## Journalism

- Breaking news
- Event monitoring
- Public opinion analysis

---

# 🔎 Popular Search Examples

```text
ChatGPT
OpenAI
Bitcoin
Tesla
Python
#AI
from:elonmusk
AI since:2025-01-01
AI min_faves:1000
AI filter:images
```

---

# ⚙️ Quick Start

```json
{
  "query": "Artificial Intelligence",
  "queryType": "Latest",
  "numberOfTweets": 100
}
```

Advanced example:

```json
{
  "query":"(ChatGPT OR Claude OR Gemini)",
  "usersVerifiedOnly": true,
  "engagementMinLikes":500,
  "mediaTypes":["image","video"]
}
```

---

# 📤 Example Output

```json
{
  "tweet_id":"123456789",
  "text":"The future of AI is exciting.",
  "author":{
    "username":"example",
    "verified":true
  },
  "stats":{
    "likes":2145,
    "retweets":356
  }
}
```

---

# 💻 API Examples

## Python

```python
from apify_client import ApifyClient

client = ApifyClient("YOUR_TOKEN")

run = client.actor(
    "mikolabs/x-twitter-advanced-search-tweet-scraper"
).call(run_input={
    "query":"OpenAI",
    "numberOfTweets":100
})
```

## Node.js

```javascript
import { ApifyClient } from "apify-client";

const client = new ApifyClient({
  token: process.env.APIFY_TOKEN,
});
```

## cURL

```bash
curl -X POST \
https://api.apify.com/v2/acts/mikolabs~x-twitter-advanced-search-tweet-scraper/run-sync-get-dataset-items
```

---

# 🍳 Search Recipes

## AI Discussions

```json
{
 "query":"ChatGPT OR OpenAI OR Claude OR Gemini",
 "numberOfTweets":500
}
```

## Lead Generation

```json
{
 "query":"\"looking for\" OR \"recommend\"",
 "numberOfTweets":500
}
```

## Brand Monitoring

```json
{
 "query":"Your Brand Name"
}
```

## Viral Tweets

```json
{
 "query":"Artificial Intelligence",
 "engagementLevel":"viral"
}
```

---

# 🖼️ Showcase

Replace these placeholders with screenshots.

- assets/search-config.png
- assets/run-actor.png
- assets/output-json.png
- assets/export-csv.png
- assets/ai-workflow.png

---

# 🔌 Integrations

Works great with:

- OpenAI
- Claude
- Gemini
- LangChain
- LlamaIndex
- Pinecone
- Supabase
- PostgreSQL
- MongoDB
- Power BI
- Tableau
- Zapier
- Make
- n8n

---

# ❓ FAQ

### Does it require the official API?

No.

### Can I export CSV?

Yes.

### Can I collect AI datasets?

Yes.

### Can I automate runs?

Yes, using Apify scheduling and integrations.

---

# 💡 Best Practices

- Combine multiple filters.
- Use date filters.
- Export JSON for AI.
- Export CSV for reporting.
- Schedule recurring runs.

---

# 🛣️ Roadmap

- Faster scraping
- More filters
- Better thread detection
- More integrations
- Improved documentation

---

# ❤️ Support

If you enjoy this actor:

- ⭐ Add to Favorites
- ⭐ Leave a Review
- 🚀 Share with your team
- 💡 Suggest features

---

# 🚀 Ready to Start?

**Mikolabs X (Twitter) Advanced Search Tweet Scraper** helps developers, researchers, marketers, AI teams, and businesses collect high-quality public Twitter/X data quickly and reliably.

**Fast. Structured. Scalable.**
