---
name: b2b-seo-ops
description: SEO and content-gap intelligence for B2B marketers. Audits any company's website, compares its content against competitors, maps keyword ideas by funnel stage, scores keywords by Impact × Confidence when data is available, scouts trending topics, and writes content briefs. Works with no paid tools (web research only), gets sharper with exports the user brings (Google Keyword Planner, Semrush, Ahrefs, Search Console CSVs), and uses live Semrush or Search Console connections automatically if they exist. Use whenever the user asks for an SEO audit, keyword research, competitor content gaps, "what should we write about", trending topics in their space, a content brief, a site's positioning or messaging on the web, or an SEO snapshot of a company (e.g. for interview prep or a client pitch).
---

# B2B SEO Ops

SEO and content intelligence for B2B marketing: what a site says, what it's missing, what competitors cover, what's trending, and what to write next.

It works at whatever data level is available, and **it always says which level it's at**, so an estimate is never presented as data.

Reference files:
- `references/data-levels.md`: what each data source gives, how to read exports, and how to label outputs. **Read first, every time.**
- `references/workflows.md`: the seven workflows and their output templates
- `references/scoring.md`: funnel stages, Impact × Confidence scoring, and quick-win rules

---

## Step 0: Check the data level

Before any analysis, work out what data is available (details in `references/data-levels.md`):

| Level | What's available | What it unlocks |
|---|---|---|
| **1. Research** | Web search and reading pages only | Site audits, competitor content gaps, keyword *ideas*, trends, briefs |
| **2. Exports** | The user pastes or attaches keyword data (Keyword Planner, Semrush, Ahrefs, Search Console) | Real volumes, difficulty, and rankings from that file, and full scoring |
| **3. Live** | A working Semrush or Search Console connection in this session | Everything above, pulled directly |

- If a Semrush or Search Console tool is available, try one small call. If it errors or says the plan doesn't include access, fall back and tell the user in one line.
- If the user hasn't shared data and the task needs numbers (e.g. "which keywords should we target"), do the Level 1 version, then say what export would make it sharper and how to get it (see `references/data-levels.md`).
- Put a data-level label at the top of every output, e.g. `Data level: 1 (research only). Volumes and difficulty are estimates.`

---

## Step 1: Get the essentials

1. **Target site**: the domain to analyze.
2. **Whose site**: the user's own or managed site, or an outside company (research).
3. **Competitors**: 2-4 domains. If none are given, propose some from web research, say why, and let the user confirm or swap before the deep comparison.
4. **Focus**: the product category, audience, or topics that matter (e.g. "IT infrastructure monitoring for mid-market IT teams").
5. **Goal**: audit, gap analysis, keyword plan, trends, brief, or company snapshot. Infer from the request.

Infer what you can and state assumptions in one line. Ask only what you truly can't guess.

---

## Step 2: Run the workflow

Pick from `references/workflows.md`:

1. **Site audit**: on-page basics, positioning clarity, and which buyer questions the site answers
2. **Competitor content gap**: topic-by-topic coverage vs competitors, and open gaps
3. **Keyword map**: keyword ideas grouped by funnel stage (TOFU / MOFU / BOFU)
4. **Keyword scoring**: Impact × Confidence ranking and quick wins (needs Level 2 or 3)
5. **Trend scout**: what's rising in the space this week or month
6. **Content brief**: a ready-to-write brief for one gap or keyword
7. **Company SEO snapshot**: a one-page summary of 1-3 (+5), for interview prep or a pitch

Chain them when it helps (e.g. gap analysis → brief for the top gap).

---

## Step 3: Rules that always apply

- **Never invent numbers.** No search volumes, difficulty scores, rankings, or traffic figures unless they come from a tool or a file the user gave you. At Level 1, use words ("likely niche", "competitive term"), not made-up numbers.
- **Cite what you read.** When a finding comes from a specific page, name or link the page.
- **Private data comes with permission.** For a company the user doesn't manage, work from public data by default. Its private analytics (Search Console, Google Analytics, internal reports) can make the analysis much sharper, so it's fine to suggest getting them **through the company's own marketing team or an employee, with their permission**, e.g. "If you're working with their digital marketing team, ask them to share a Search Console export (last 3 months) for a sharper read." Frame it as an authorized request, never as a workaround. Use private data only if the user says it was shared with permission. If the user mentions a former employer, don't bring in confidential knowledge from their time there.
- **Web search results aren't rankings.** If a site shows up (or doesn't) in searches you ran, report it as a spot check, e.g. "appeared in the web searches I ran (not a ranking measurement)". Never state a position or imply a ranking at Level 1.
- **Be specific.** "Add a comparison page: [Product] vs [Competitor]" beats "improve BOFU content".
- **Prioritize.** End every output with the 3-5 highest-value actions, in order.

---

## Step 4: Deliver

1. Data-level label (one line).
2. The workflow output, using the template in `references/workflows.md`.
3. **Top actions**: 3-5, ordered, each with why and expected effort (quick / medium / big).
4. **Sharpen this**: one line on what data would improve the result, only if it would change the recommendations. List what the user can get themselves first (a Semrush free-account export, a Keyword Planner CSV). For a site they don't manage, add the permission-based option if it fits: their own analytics, shared by the company's marketing team.

Offer the natural next step (e.g. "Want a brief for gap #1?" or "Want a LinkedIn post on this trend?" if the personal-brand-writer skill is available).
