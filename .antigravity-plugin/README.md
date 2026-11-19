# mowteng

mowteng connects Antigravity to Google Search Console, Bing Webmaster Tools and Yandex Webmaster. Ask about your clicks, queries and indexing in plain language, submit sitemaps and URLs, and run ready-made SEO analyses on live data.

## Before you install

- A Google account with at least one Search Console property. Sign in with Google when Antigravity asks, and leave the Search Console permission ticked.
- Bing Webmaster Tools and Yandex Webmaster are optional. When you ask about them, the assistant gives you a link to connect each one.
- New accounts get a 7-day free trial without a card. After that mowteng needs a subscription, bought on [mowteng.app](https://mowteng.app), not inside Antigravity.

There is no Google Cloud project, API key or OAuth client of your own to set up. The plugin uses one remote MCP server (`https://mowteng.app/mcp`, Streamable HTTP, OAuth 2.1).

## Tools

**Google Search Console:** list and add properties, search analytics by query, page, country, device and date, a performance overview, URL inspection, and listing, submitting or deleting sitemaps.

**Bing Webmaster Tools:** sites, search stats, crawl issues, sitemaps and URL submission.

**Yandex Webmaster:** sites, site summary, search queries, sitemaps and URL submission.

**IndexNow:** set up the key file and ping Bing, Yandex and other engines when pages change.

**Analyses:** pages losing clicks (content decay), queries at positions 11-20 (striking distance), pages competing for the same query (cannibalization), sitemap URLs Google hasn't indexed (index audit), Google vs Bing ranking gaps, and any two periods compared by query, page, country or device.

**Routines:** a daily SEO to-do list for a site, and ready-to-schedule prompts for a first week, daily to-dos, weekly and monthly reports.

**Account:** connected sources, and a link to connect Bing or Yandex or to delete your mowteng account.

Write tools (adding a property, submitting or deleting sitemaps, submitting URLs) are annotated so Antigravity asks before running them. Deleting a sitemap and submitting URLs to Bing are marked destructive. mowteng never edits your site.

## Example workflows

- *Which pages on example.com lost the most Google clicks in the last 28 days?* Then ask for the queries behind the biggest drops.
- *Show queries where I rank 11-20 with the most impressions, and the page ranking for each.* A shortlist of pages to improve.
- *Check the URLs in https://example.com/sitemap.xml and list the ones Google hasn't indexed.* Then inspect the worst ones one by one.
- *Compare example.com in Google and Bing: biggest position gaps and queries only one engine shows.*
- *Compare October with September by country, then resubmit my sitemap to Google and Bing.*

## Data

Search data is fetched live for each request and never stored. mowteng keeps only your encrypted connection, and you can delete your account and revoke access at any time. Bing and Yandex support is experimental.

- Setup guide: https://mowteng.app/integrations/antigravity
- Help: https://mowteng.app/help
- Privacy policy: https://mowteng.app/privacy-policy
- Terms of use: https://mowteng.app/terms-of-use
