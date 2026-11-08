# byteblisk

Three hosted MCP servers for AI agents, running on [Apify](https://apify.com/byteblisk). Nothing to install: connect
over Streamable HTTP with your Apify API token, and pay per use. Every tool states its cost, and failed calls are free.

| | Server | What your agent gets | Store page |
|---|---|---|---|
| <img src="https://raw.githubusercontent.com/ByteBlisk/mcp-servers/main/logos/sitereader.png" width="48"> | **Web Scraper & Crawler for RAG** | Any page or whole site as clean Markdown or JSON, site maps, fields you describe in plain words | [apify.com/byteblisk/sitereader](https://apify.com/byteblisk/sitereader) |
| <img src="https://raw.githubusercontent.com/ByteBlisk/mcp-servers/main/logos/app-reviews.png" width="48"> | **App Store & Google Play Reviews** | Reviews from both stores in one format, complaint themes with real quotes, competitor comparison | [apify.com/byteblisk/app-reviews-insights](https://apify.com/byteblisk/app-reviews-insights) |
| <img src="https://raw.githubusercontent.com/ByteBlisk/mcp-servers/main/logos/toolkit.png" width="48"> | **Google Play Scraper & SERP Rank Checker** | Google Play apps, reviews and search, top-100 rank on Google, Bing and Yandex | [apify.com/byteblisk/google-play-search-toolkit](https://apify.com/byteblisk/google-play-search-toolkit) |

## Connect

Endpoints (Streamable HTTP, header `Authorization: Bearer <YOUR_APIFY_TOKEN>`):

```
https://byteblisk--sitereader.apify.actor/mcp
https://byteblisk--app-reviews-insights.apify.actor/mcp
https://byteblisk--google-play-search-toolkit.apify.actor/mcp
```

Claude Desktop, Cursor or any MCP client (`mcp.json`):

```json
{
  "mcpServers": {
    "byteblisk-sitereader": {
      "url": "https://byteblisk--sitereader.apify.actor/mcp",
      "headers": { "Authorization": "Bearer YOUR_APIFY_TOKEN" }
    },
    "byteblisk-app-reviews": {
      "url": "https://byteblisk--app-reviews-insights.apify.actor/mcp",
      "headers": { "Authorization": "Bearer YOUR_APIFY_TOKEN" }
    },
    "byteblisk-google-play-search": {
      "url": "https://byteblisk--google-play-search-toolkit.apify.actor/mcp",
      "headers": { "Authorization": "Bearer YOUR_APIFY_TOKEN" }
    }
  }
}
```

Get a token at [console.apify.com/settings/integrations](https://console.apify.com/settings/integrations). Prices
are on each Store page; Apify's free plan includes monthly credit to try them.

## Support

Open an issue on the actor's Store page; we answer every one.
