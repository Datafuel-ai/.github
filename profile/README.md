<div align="center">
  <a href="https://datafuel.ai">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://dashboard.datafuel.ai/web-app-manifest-192x192.png">
      <img src="https://dashboard.datafuel.ai/web-app-manifest-192x192.png" alt="DataFuel" height="140">
    </picture>
  </a>

  <h3>The fuel for web scraping & AI agents</h3>
  <p>Any page, past any protection, as clean Markdown or JSON.<br>Proxies and web data APIs, owned and operated in Europe.</p>

  <a href="https://datafuel.ai">
    <img src="https://img.shields.io/badge/🚀_Get_Started-0b171a?style=for-the-badge" alt="Get Started">
  </a>
  <a href="https://docs.datafuel.ai">
    <img src="https://img.shields.io/badge/📚_Documentation-335259?style=for-the-badge" alt="Documentation">
  </a>
  <a href="https://scraping-api.datafuel.ai/skill.md">
    <img src="https://img.shields.io/badge/🤖_MCP_&_Agents-22b573?style=for-the-badge" alt="MCP & Agents">
  </a>
</div>

<br>

<div align="center">
  <a href="https://www.npmjs.com/package/@datafuel/sdk"><img src="https://img.shields.io/npm/v/@datafuel/sdk?label=%40datafuel%2Fsdk&color=335259" alt="npm"></a>
  <a href="https://pkg.go.dev/github.com/Datafuel-ai/datafuel-go"><img src="https://img.shields.io/badge/go-datafuel--go-335259?logo=go&logoColor=white" alt="Go"></a>
  <a href="https://status.datafuel.ai"><img src="https://img.shields.io/badge/status-live-22b573" alt="Status"></a>
</div>

---

## Why DataFuel?

Scrapers break. Pages render client-side, anti-bot walls block plain requests, results change by country, and agents waste tokens on navbars and cookie banners.

DataFuel is one account and one balance for the whole stack: **our own proxy network** and **the APIs on top of it**. Send a URL, get clean data back. Pay only for what succeeds.

**Discover → Unlock → Extract → Use**

## What DataFuel does

| API                                                         | Job                                                                                               |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **[Unlocker](https://datafuel.ai/scraping/unlocker)**       | Any page past any protection, as Markdown, HTML, JSON or a screenshot. One request.               |
| **[Crawl](https://datafuel.ai/scraping/crawl)**             | Every page under a start URL as LLM-ready Markdown, in one async job.                             |
| **[Map](https://datafuel.ai/scraping/map)**                 | Every URL of a site, deduplicated and filtered, for one flat credit.                              |
| **[Search](https://datafuel.ai/scraping/serp)**             | Google results as structured JSON, Markdown or HTML, for the country, language and city you pick. |
| **[LLM Scraper](https://datafuel.ai/scraping/llm-scraper)** | What ChatGPT, Gemini, Perplexity and Copilot actually answer, by country, with citations.         |

| Proxies                                                    |                                  |
| ---------------------------------------------------------- | -------------------------------- |
| **[Residential](https://datafuel.ai/proxies/residential)** | Ethically sourced, billed per GB |
| **[Mobile](https://datafuel.ai/proxies/mobile)**           | Real 4G/5G carrier IPs           |
| **[ISP](https://datafuel.ai/proxies/isp)**                 | Dedicated static IPs, yours only |
| **[Datacenter](https://datafuel.ai/proxies/datacenter)**   | Speed at scale, unmetered        |

## Try it in 10 seconds

```bash
curl https://scraping-api.datafuel.ai/api/v1/task \
  -H "X-API-Key: $DATAFUEL_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"type": "unlocker", "attributes": {"url": "https://example.com", "result_format": "markdown"}}'
```

Failed or blocked pages are refunded automatically. No success, no charge.

## Our Ecosystem

### MCP Server

<a href="https://github.com/Datafuel-ai/datafuel-js/tree/main/packages/mcp">
  <img align="right" src="https://img.shields.io/badge/MCP_Server-22b573?style=for-the-badge&logo=anthropic&logoColor=white" alt="MCP Server">
</a>

**[@datafuel/mcp](https://github.com/Datafuel-ai/datafuel-js/tree/main/packages/mcp)** — Model Context Protocol
Give Claude Code, Cursor, VS Code, Windsurf, Claude Desktop, Codex and Gemini CLI an unblockable browser. One command sets it up:

```bash
npx -y @datafuel/mcp init
```

Or point any MCP client at `https://scraping-api.datafuel.ai/mcp` with your `X-API-Key` header.

<br clear="right"/>

### JavaScript / TypeScript SDK

<a href="https://github.com/Datafuel-ai/datafuel-js">
  <img align="right" src="https://img.shields.io/badge/TypeScript-335259?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
</a>

**[datafuel-js](https://github.com/Datafuel-ai/datafuel-js)** — `@datafuel/sdk`
Typed client for the whole API. Zero runtime dependencies.

```bash
npm install @datafuel/sdk
```

<br clear="right"/>

### Go SDK

<a href="https://github.com/Datafuel-ai/datafuel-go">
  <img align="right" src="https://img.shields.io/badge/Go-335259?style=for-the-badge&logo=go&logoColor=white" alt="Go">
</a>

**[datafuel-go](https://github.com/Datafuel-ai/datafuel-go)** — Go client
Standard library only. `client.Markdown(ctx, url)` and you're done.

```bash
go get github.com/Datafuel-ai/datafuel-go
```

<br clear="right"/>

### Agent Skill

<a href="https://scraping-api.datafuel.ai/skill.md">
  <img align="right" src="https://img.shields.io/badge/SKILL.md-0b171a?style=for-the-badge&logo=markdown&logoColor=white" alt="Skill">
</a>

**[skill.md](https://scraping-api.datafuel.ai/skill.md)** — Teach your agent DataFuel
One file that tells an AI agent which endpoint to pick, what it costs and how to read the result. Also served as [`/llms.txt`](https://scraping-api.datafuel.ai/llms.txt).

<br clear="right"/>

### Python SDK

<img align="right" src="https://img.shields.io/badge/Python-coming_soon-lightgrey?style=for-the-badge&logo=python&logoColor=white" alt="Python">

**datafuel-py** — Sync and async client. Coming soon.

<br clear="right"/>

## Built for

- **AI agents that browse** — clean Markdown instead of raw HTML, through one MCP integration.
- **RAG and training data** — crawl whole sites into embed-ready text.
- **GEO / AI visibility** — see how AI engines cite you and your competitors, by country.
- **Price monitoring and SERP tracking** — every market, every city, on a schedule.
- **Lead enrichment and alternative data** — public web signals straight into your pipeline.

## Resources

|                                                                       |                                                  |
| --------------------------------------------------------------------- | ------------------------------------------------ |
| 📚 [Documentation](https://docs.datafuel.ai)                          | Guides and full API reference                    |
| 📄 [OpenAPI spec](https://scraping-api.datafuel.ai/docs/openapi.yaml) | Generate your own client                         |
| 💶 [Pricing](https://datafuel.ai/pricing)                             | Every price on one page, plans and pay-as-you-go |
| 🌍 [Locations](https://datafuel.ai/locations)                         | Proxy inventory by country, city and ASN         |
| 🟢 [Status](https://status.datafuel.ai)                               | Live availability                                |
| 🔒 [Trust center](https://datafuel.ai/trust/security)                 | Security, DPA, compliance                        |

---

<div align="center">
  <sub><a href="https://datafuel.ai/contact">Contact us</a></sub>
</div>
