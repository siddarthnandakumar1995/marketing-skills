---
name: social-content-copilot
description: Turns a content calendar entry (topic, post type, creative type) into ready-to-use social copy — headline/hook options, supporting line, full caption, and hashtags — plus creative direction for the visual. Use this whenever the user is planning social media posts from a content calendar, needs copy for a carousel/stat post/thought-leadership post, wants help going from a rough topic to a finished LinkedIn or social caption, or mentions a content pillar, post type, or creative type for a marketing post. Also use it to A/B two caption or creative directions and get a reasoned recommendation, to polish existing copy ("make this crisper", "sentence case not caps"), or to hand off finished copy to Canva for a mockup.
---

# Social Content Copilot

Turns one content-calendar entry into finished, on-brand social copy — the same shape of work a product marketer does dozens of times a month, just faster and more consistent.

## Why this exists

Most AI-assisted social copy reads generic because it's generated from a bare topic with no sense of *format* or *voice*. This skill fixes that by treating "what kind of post is this" as a first-class input, not an afterthought — a stat post and a carousel need fundamentally different structures, and matching an existing brand voice matters more than writing "good" copy in the abstract.

## Step 1: Get the essentials

Before generating anything, make sure you know:

1. **Post Type** (the *why* — pick one): `Brand awareness` / `Thought leadership` / `Announcement` (e.g. speaking at an event, a launch, a milestone)
2. **Creative Type** (the *how* — pick one): `Carousel` / `Thought post` (single static) / `Stat post`
3. **Topic / content pillar** — what the post is actually about, in a sentence
4. **Style reference (optional but valuable)** — a previous post, screenshot, or brand voice description. If the user provides one, match its tone, sentence rhythm, and structure rather than defaulting to generic marketing voice. If they don't provide one, ask once whether they have a reference; don't block on it if they say no.

If the user gives you a topic but no Post Type / Creative Type, make your best guess from context and say what you assumed (e.g. "Since this is about a conference talk, I'm treating this as an Announcement / Thought post — let me know if you meant something else") rather than stopping to ask — momentum matters more than precision here, and it's a one-line correction if you guessed wrong.

## Step 2: Build it using the right template

Each Creative Type has a different job. Don't use one generic caption shape for all three.

### Carousel (multi-slide)

Every slide earns its place — no slide should just restate the previous one. Default shape, adapt as needed:

1. **Hook slide** — curiosity-led, not a dry title. A question or provocative statement beats a label (e.g. "What is Fully Homomorphic Encryption?" is weaker than "The encryption trick that lets AI compute on data it can never see").
2. **Explainer slide** — the real substance. This is where you actually teach the thing.
3. **Why it matters slide** — connects the concept to a consequence the reader cares about.
4. **Proof/stat slide** — a real, citable number if one exists. Stats build credibility a claim alone can't.
5. **Closer slide** — a forward-looking or values statement, not a repeat of the hook.
6. **Optional CTA slide** — only add if there's a genuine next action (read the blog, register, follow). A CTA slide bolted onto a pure-awareness carousel makes it feel like two posts stitched together — flag this tension to the user if it's an awareness post and they want a hard CTA.

Keep individual slides short. If a slide is doing two jobs, split it.

### Stat post (single visual, stat is the hero)

1. Find or confirm one real, specific, citable statistic. Never invent a number — if the user hasn't supplied a source, ask for one or flag that it needs verification before publishing.
2. The stat itself is the visual focal point — the caption's job is to give it context, not compete with it for attention.
3. Caption structure: one line framing why this matters right now → the stat with its source → one line on the implication.
4. Decide (or offer both, see A/B below) whether to add a CTA. A pure stat/thought-leadership post is often stronger *without* one — a CTA can make it feel like a sales post wearing a thought-leadership costume.

### Thought post (single static)

1. **Headline** — the main visual text, short enough to read in under 2 seconds.
2. **Supporting line** — one short line that adds a second beat (e.g. "Secure Cloud. Smarter AI." → "Trust starts with secure infrastructure.").
3. **Caption** — expands on the headline in full sentences, ends with a CTA if there's somewhere for the reader to go (a blog post, a resource).
4. **Hashtags** — see below.

**Text-only variant:** not every thought post needs a visual. A short, punchy text-only post (2-3 lines, no image) is a valid, lighter-weight version of this format — especially for LinkedIn. It often works best as a contrast structure: state one thing that matters, then pivot to something that matters *more*. For example: "Model performance matters. 🚀 But secure AI adoption depends on more than intelligence alone." A sparing emoji at the end of a line (not mid-sentence) can add visual rhythm without looking unprofessional. Ask the user whether they want a visual or a text-only post if it's not specified — the copy structure differs slightly either way.

## Step 3: Hashtags

Real-world usage runs heavier than most people assume — 8-13 hashtags is normal for a LinkedIn post, not 3-4. Mix three tiers: 2-3 broad category tags (#AI #Cybersecurity), a branded tag if one exists (#CompanyNameAI), and several single-word tags tied to the specific topic (#DataSovereignty #Compliance #Control) — these narrower tags do more work for discoverability than the broad ones. Skip only pure filler that could apply to literally any post in the industry with zero connection to this one's actual topic.

## Step 4: When producing multiple options, recommend one

If you generate 2+ variants (which is often useful for a stat post or headline), don't just dump them and ask the user to pick — that pushes the work back on them. State which one you'd pick and *why*, using concrete reasoning tied to the post's actual goal, e.g.:

> "I'd go with option 2 — it keeps the stat as the visual hero and reads cleaner without a CTA block. Option 1 works if you specifically want this to double as a campaign/conversion post, but for a pure awareness stat post the CTA makes it feel like two goals fighting each other."

Reasoning should reference the post's Post Type and Creative Type, not just "this one sounds better."

## Step 5: Handle polish requests fast

Once copy exists, expect (and handle gracefully) small iterative requests like:
- "make this crisper" — cut words, don't just rephrase; a crisper version should almost always be *shorter*.
- "sentence case not caps" — a formatting change, don't second-guess the content.
- "remove this line" / "remove the CTA" — just do it, don't argue for keeping it unless there's a real risk (e.g. removing the only source citation from a stat post — flag that specifically).

Small requests deserve small, fast responses — don't regenerate the whole post from scratch when one line changed.

## Step 6: Suggest a filename

End each finished post with a suggested filename/title, using this pattern so a whole month's assets stay organized and sortable:

`[posttype]-[creativetype]-[short-topic-slug]-[YYYY-MM].png`

Example: `thoughtleadership-statpost-ai-phishing-2026-04.png`

## Step 7 (optional): Hand off to Canva

If the user has the Canva MCP connector available and wants an actual visual mockup (not just copy), use the Canva tools to generate a draft design once the copy is finalized — pass the headline/supporting line/stat and Creative Type (carousel slide count, single static, etc.) as the design brief. Confirm the copy is locked before generating, since regenerating a Canva design is more expensive than editing text. If no Canva connector is available, just deliver the copy and describe the visual direction in words (layout, what should be the focal point, tone of imagery) so the user can brief a designer or build it themselves.

## A note on voice-matching

If the user shares a past post as a reference, resist the urge to "improve" its voice — match it. A brand's inconsistency is worse than a brand's imperfection. Only deviate from the reference style if the user explicitly asks for a new direction.
