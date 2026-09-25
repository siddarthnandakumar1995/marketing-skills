# Data levels

The skill works at three levels. Always tell the user which one an output is based on.

---

## Level 1: Research (no paid tools)

**Sources:** web search, reading the target and competitor pages, public trend sources (Google Trends, Reddit, Hacker News, industry news, YouTube).

**Reliable at this level:**
- What a site says: titles, headings, meta descriptions, messaging, page structure, internal links
- What topics a site and its competitors cover, and how deeply
- Which buyer questions are answered or missing
- Keyword *ideas* and funnel stages
- Which topics are being discussed more right now

**Not reliable at this level. Don't state as fact:**
- Search volume, keyword difficulty, cost per click
- Actual rankings or positions
- Traffic, clicks, or traffic changes

**Web search spot checks:** seeing a site in (or missing from) searches you ran is useful, but it isn't a Google ranking. Results come from a different engine, can vary, and have no reliable positions. Word it as "appeared in the web searches I ran for X (not a ranking measurement)".

Use qualitative labels instead: "likely niche", "likely competitive (large vendors and review sites dominate this query)", "appears to be rising (more coverage this month across X, Y)".

---

## Level 2: Exports the user brings

Accept CSV or Excel files, or tables pasted into the chat. Identify the source from the column names, then use only the columns that exist.

| Source | Typical columns | Gives you | Watch out for |
|---|---|---|---|
| **Google Keyword Planner** (free with a Google Ads account) | Keyword, Avg. monthly searches, Three month change, YoY change, Competition, Competition (indexed value), Top of page bid (low/high range) | Search volume (often as ranges), trends, ad bid prices | **"Competition" is ad-bidder competition, not SEO difficulty.** Never treat it as keyword difficulty. High bids suggest commercial intent. |
| **Semrush** (web export) | Keyword, Position, Search Volume, Keyword Difficulty, CPC, URL, Traffic, Intent | Rankings for a domain, difficulty, volume, intent | Traffic is an estimate. Small B2B sites may show few keywords. |
| **Ahrefs** (web export) | Keyword, Volume, KD, CPC, Position, URL, Traffic | Same as Semrush | Same. KD scales differ from Semrush's, so don't mix them in one score. |
| **Google Search Console** (sites the user owns, or shared with permission by the site's team) | Query, Clicks, Impressions, CTR, Position; pages; date ranges | Real clicks and impressions, average position | No difficulty and no competitor data. Needs two date ranges to spot decay. |

**Tips to share with the user when a result would benefit from data:**
- Keyword Planner: Tools → Keyword Planner → "Discover new keywords" → try "Start with a website" with a competitor's URL → Download keyword ideas (CSV).
- Semrush free account: Organic Research on a domain → Positions → Export (if the plan allows), or copy the visible table and paste it.
- Search Console: Performance → Search results → pick a date range → Export. For decay, export the last 28 days and the previous 3 months.

---

## Level 3: Live connections

If a Semrush or Google Search Console tool is available in the session:
1. Make one small test call first.
2. If it works, use it instead of asking for exports, and cite "Semrush (live)" or "Search Console (live)".
3. If it returns a plan or access error, say so in one line ("Semrush is connected but your plan doesn't include access from Claude"), then continue at Level 1 or 2. Don't retry repeatedly.

---

## Combining sources (for a site the user manages)

- **Search Console** is the truth for the user's own site: real clicks, impressions, and positions.
- **Semrush or Ahrefs** is for the market view: competitors, difficulty, gaps.
- When they disagree on the user's own site, trust Search Console.

## Labels

Start every output with one line:
- `Data level: 1 (research only). No volumes or rankings; keyword notes are estimates.`
- `Data level: 2 (Keyword Planner export, 214 keywords). Volumes are ranges; no SEO difficulty.`
- `Data level: 3 (Semrush live, US database).`
