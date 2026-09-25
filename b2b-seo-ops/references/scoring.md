# Scoring

Adapted from the Impact × Confidence model in Eric Siu's seo-ops ([ai-marketing-skills](https://github.com/ericosiu/ai-marketing-skills), MIT). The change: volume thresholds are recalibrated for B2B, where good keywords often have tens or hundreds of searches, not thousands.

---

## Funnel stage

Classify every keyword:

- **BOFU (ready to buy):** commercial or transactional intent, or the keyword contains: pricing, cost, price, software, tool(s), platform, vendor, provider, services, company, consultant, best, top, vs, alternative(s), review(s), demo, trial, buy, hire, outsource.
- **MOFU (evaluating):** how to, guide, strategy, framework, checklist, template, examples, case study, ROI, comparison, what is, explained, benefits, use cases, best practices.
- **TOFU (learning):** everything else, i.e. pure informational or problem-aware searches.

If an export includes an intent column, use it (commercial or transactional → BOFU).

---

## Impact × Confidence (Level 2 or 3 only)

Only score when the numbers come from a tool or an export. At Level 1, don't produce scores. Use the funnel stage and qualitative notes instead.

### Impact (0-10)

| Factor | Points |
|---|---|
| Monthly volume (B2B scale) | ≥1,000 → 3 · ≥200 → 2 · ≥50 → 1 |
| Cost per click / top-of-page bid | ≥$15 → 3 · ≥$5 → 2 · ≥$1 → 1 |
| Funnel stage | BOFU → 2 · MOFU → 1 |
| Trend (last 3 months vs earlier) | >+50% → 2 · >+20% → 1 |

Cap at 10. If volume comes as a range (Keyword Planner), use the lower bound.

### Confidence (0-10)

| Factor | Points |
|---|---|
| Keyword difficulty (Semrush or Ahrefs KD) | ≤10 → 4 · ≤20 → 3 · ≤35 → 2 · ≤50 → 1 |
| Current position of the target site | ≤10 → 3 · ≤30 → 2 · ≤50 → 1 |
| Topic authority: the site already has 3+ pages on this topic | +2 |

Cap at 10. **If there's no difficulty data** (e.g. Keyword Planner only), don't guess KD. Score confidence from position and topic authority only, and say so in the output.

### Priority

**Priority = Impact × Confidence** (max 100). Sort descending.

---

## Quick wins

Flag a keyword as a **quick win** when:
- the site ranks in positions 5-20 (close to page 1), and
- KD ≤ 40 (if known), and
- the keyword is MOFU or BOFU.

Action: refresh and expand the existing page, improve the title and headings for the query, and add internal links to it.

## Execution path

| Situation | Suggested path |
|---|---|
| Low difficulty (KD ≤ 20), no existing page | Create a new page. AI drafts, a human reviews. |
| Existing page, KD ≤ 50 | Refresh the existing page. |
| KD 20-40 | AI drafts, a subject-matter expert reviews. |
| KD 40-60 | Expert-written, AI-optimized. |
| KD > 60 | Expert content plus links. A long-term play. |

## Decaying pages (Search Console only)

Compare clicks for the last 28 days with the average 28-day clicks over the previous 90 days. Flag a query or page when clicks dropped more than 30% and the earlier average was above 5 clicks. Suggest: check whether the ranking dropped or demand dropped, then refresh the content or fix the page.
