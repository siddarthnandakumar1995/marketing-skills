# Workflows

Seven workflows. Each ends with **Top actions** (3-5, ordered). Keep outputs scannable: tables and short lines, not essays.

---

## 1. Site audit

**Read:** the homepage, 3-5 key product or solution pages, the pricing or contact page, and the blog or resources index. Check the sitemap (`/sitemap.xml`) to see the site's size and sections.

**Check each key page:**
- Title tag and meta description: present, specific, under ~60 / ~155 characters, includes the term a buyer would search
- One clear H1, and a logical H2 structure
- **Positioning clarity:** can a stranger tell *what it is, who it's for, and why it's different* within 5 seconds of the top of the page?
- Proof: customer logos, numbers, case studies, reviews
- Next step: is there one clear call to action?
- Internal links: do product pages link to supporting content, and the other way round?

**Buyer-question coverage:** list the questions a buyer asks at each stage (TOFU: "what is X / why does it matter"; MOFU: "how to choose X, X vs Y, ROI"; BOFU: "pricing, implementation, security, integrations, reviews") and mark each one ✅ answered / ⚠️ thin / ❌ missing, with the page that answers it.

**Output:**
```
Data level: ...
Site: [domain]: [one-line summary of what it sells, to whom]

Page scorecard
| Page | Title/meta | H1 | Positioning clarity | Proof | CTA | Notes |

Buyer questions
| Stage | Question | Status | Where |

Top actions
1. ...
```

---

## 2. Competitor content gap

**Read** each site's main navigation, solution pages, and resources or blog index (titles are enough; skim a few representative posts).

**Build a topic matrix:** rows are topics or questions buyers care about, columns are sites. Mark coverage depth: ● deep (dedicated page or series) · ◐ some (mentioned or thin) · ○ none.

**Then call out:**
- **Open gaps:** topics no one covers well. The best opportunities.
- **Catch-up gaps:** competitors cover it, the target doesn't.
- **Strengths:** where the target leads. Protect and link to these.
- **Positioning contrast:** one line per competitor on how they position vs the target.

At Level 2 or 3 with competitor keyword data, add a **keyword gap** table: keywords competitors rank for (top 20) that the target doesn't, with volume, KD, and funnel stage.

**Output:**
```
Data level: ...
Sites: target vs [A], [B], [C]

Topic matrix
| Topic | Target | A | B | C |

Open gaps · Catch-up gaps · Strengths · Positioning contrast

Top actions
```

---

## 3. Keyword map

Group keyword ideas by funnel stage (see `scoring.md`), around the focus topics.

- 10-20 ideas per stage for a focused category, fewer if the niche is narrow.
- Include "vs", "alternative", and "pricing" terms for known competitors (BOFU gold in B2B).
- For each idea: stage, intent note, the page type it needs (blog, guide, comparison page, landing page), and whether the target already has a page for it.
- **Level 1:** no numbers. Add a column "Likely demand" with values like niche / moderate / broad, and a note that it's an estimate.
- **Level 2 or 3:** add volume, KD, and CPC from the data.

**Output:**
```
Data level: ...
| Stage | Keyword idea | Page type | Existing page? | Demand (estimate or data) |

Top actions
```

---

## 4. Keyword scoring (Level 2 or 3 only)

1. Read the export (see `data-levels.md` for columns).
2. Classify the funnel stage, and score Impact, Confidence, and Priority (see `scoring.md`).
3. Flag quick wins and assign an execution path.

**Output:**
```
Data level: ...
Top 20 by priority
| # | Keyword | Stage | Vol | KD | Pos | Impact | Conf | Priority | Path |

Quick wins (positions 5-20)
Notes on missing data (e.g. "No KD in Keyword Planner export; confidence uses position only")

Top actions
```

If the user asks for scoring at Level 1, explain in one line why real numbers are needed, give the Level 1 keyword map instead, and say which export would unlock scoring.

---

## 5. Trend scout

Scan for what's rising in the focus area over the last 2-4 weeks:
- Google Trends (rising related queries for the core terms)
- Reddit (relevant subreddits, top posts this week or month)
- Hacker News (for tech and AI topics)
- Industry news and analyst coverage
- YouTube (recent videos getting unusually high views for their channel)

**Output:** 5-8 trends, each with:
```
Trend: ...
Signal: what you saw, with links
Why it matters for [focus audience]: ...
Angle: a content idea: blog / landing page / LinkedIn post
Shelf life: flash (days) · wave (weeks) · shift (months+)
```
Close with the 2-3 trends worth acting on now.

---

## 6. Content brief

For one gap, keyword, or trend:

```
Working title: (include the target term)
Target query + funnel stage:
Reader: who, what they're trying to do
Search intent: what the searcher needs to walk away with
Angle: what makes this better or different from what currently ranks (read the top results first)
Outline: H2s and H3s, with a one-line note each
Must answer: the specific questions to cover
Proof to include: data, examples, screenshots (only real ones, or placeholders)
Internal links: existing pages to link to and from
Title tag (≤60 chars) · Meta description (≤155 chars)
CTA: the next step for the reader
```

---

## 7. Company SEO snapshot

A one-page summary, e.g. for interview prep or a client pitch. Combine the short versions of 1 and 2, plus 5:

```
Data level: ...
[Company]: [what they sell, to whom], in one line

What's working (3 bullets)
Biggest gaps (3 bullets, specific)
Competitor contrast (1 line each)
Trend to ride (1-2)
If I were running content here, first 90 days:
1. ...
2. ...
3. ...
```

Keep it to one screen, factual, and respectful. It may be shown to people at that company.
