<p align="center">
  <a href="https://mowteng.app/?utm_source=github&utm_medium=readme"><img src="https://mowteng.app/icon-512.png" width="96" alt="mowteng"></a>
</p>

# mowteng

Google Search Console, Bing Webmaster Tools, Yandex Webmaster and IndexNow in your AI assistant, with live SEO analyses.

mowteng is a hosted remote MCP server. Add one URL to Claude, ChatGPT, GitHub Copilot, Gemini or any MCP client, sign in with Google, and ask about your sites in plain language.

> This repository holds documentation and the Antigravity plugin manifest only (`.antigravity-plugin/`, `mcp_config.json`, `assets/`). mowteng is a hosted, proprietary service at `https://mowteng.app/mcp`; its source code is not published here, and there is nothing to build.

## Connect

**Server URL:** `https://mowteng.app/mcp` (Streamable HTTP, OAuth 2.1)

**VS Code / GitHub Copilot** (`.vscode/mcp.json`):

```json
{
  "servers": {
    "mowteng": { "type": "http", "url": "https://mowteng.app/mcp" }
  }
}
```

**Claude Code:**

```bash
claude mcp add --transport http mowteng https://mowteng.app/mcp
```

**Antigravity:**

```bash
agy plugin install https://github.com/erayendes/mowteng-mcp
```

**Claude, ChatGPT, Gemini:** add `https://mowteng.app/mcp` as a custom connector, then sign in with Google.

On first use you sign in with Google and pick the Search Console access to grant. Bing Webmaster Tools and Yandex Webmaster connect later through a link the assistant gives you (`mowteng_sources`).

## What you can ask

- "Which pages on example.com lost the most Google clicks in the last 28 days?"
- "Show queries where I rank 11-20 with the most impressions, and the page ranking for each."
- "Check the URLs in https://example.com/sitemap.xml and list the ones Google hasn't indexed."
- "Compare example.com in Google and Bing: biggest position gaps and queries only one engine shows."
- "Compare October with September by country, then resubmit my sitemap to Google and Bing."
- "What are today's SEO tasks for example.com?"

## Tools

| Area | Tools |
|---|---|
| Google Search Console | `gsc_list_sites`, `gsc_add_site`, `gsc_search_analytics`, `gsc_performance_overview`, `gsc_inspect_url`, `gsc_list_sitemaps`, `gsc_submit_sitemap`, `gsc_delete_sitemap` |
| Bing Webmaster Tools | `bing_list_sites`, `bing_search_stats`, `bing_crawl_issues`, `bing_list_sitemaps`, `bing_submit_sitemap`, `bing_submit_urls` |
| Yandex Webmaster | `yandex_list_sites`, `yandex_site_summary`, `yandex_search_queries`, `yandex_list_sitemaps`, `yandex_submit_sitemap`, `yandex_submit_urls` |
| IndexNow | `indexnow_setup`, `indexnow_submit` |
| Analyses | `insights_content_decay`, `insights_striking_distance`, `insights_cannibalization`, `insights_index_audit`, `insights_google_vs_bing`, `insights_compare_periods` |
| Daily work | `todo_list`, `mowteng_routines` |
| Account | `mowteng_sources` |

Write tools (adding a property, submitting or deleting sitemaps, submitting URLs) are annotated, and the destructive ones are marked so your client asks before running them. Bing and Yandex support is experimental.

## Guides

- [Google Search Console MCP server](https://mowteng.app/google-search-console-mcp): what mowteng does with Search Console data
- [Bing Webmaster Tools MCP server](https://mowteng.app/bing-webmaster-tools-mcp)
- [Yandex Webmaster MCP server](https://mowteng.app/yandex-webmaster-mcp)
- [IndexNow MCP server](https://mowteng.app/indexnow-mcp) and the free [IndexNow key generator](https://mowteng.app/indexnow-key-generator)
- [Bulk URL inspection](https://mowteng.app/analyses/bulk-url-inspection) and [how to inspect 10,000 URLs on a 2,000-a-day quota](https://mowteng.app/blog/inspect-10000-urls-url-inspection-quota)
- [Setup guides](https://mowteng.app/guides) and [ready-made prompts](https://mowteng.app/prompts)

## Data and privacy

Search data is fetched live for each request and never stored. mowteng keeps only your encrypted connections and subscription status. You can delete your account and revoke access at any time from the link `mowteng_sources` gives you.

- [Privacy policy](https://mowteng.app/privacy-policy)
- [Terms of use](https://mowteng.app/terms-of-use)

## Pricing

New accounts get a 7-day free trial. After that mowteng needs a subscription, bought on [mowteng.app](https://mowteng.app/?utm_source=github&utm_medium=readme).

## Support

- Website and guides: [mowteng.app](https://mowteng.app/?utm_source=github&utm_medium=readme)
- Email: hi@milowda.com

mowteng is proprietary software by milowda. The server's source code is not published.
