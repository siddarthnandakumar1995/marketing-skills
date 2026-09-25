# AI-writing check (voice-aware)

The last step before any post goes back to the user. It catches the patterns that make a post read as machine-written.

Adapted from Eric Siu's 24-pattern humanizer rubric in [ai-marketing-skills](https://github.com/ericosiu/ai-marketing-skills) (MIT), which draws on Wikipedia's "Signs of AI writing" guide. The change here: **the person's voice wins.** The original rubric penalizes emoji, dashes, lists of three, and corporate vocabulary outright. This version checks the voice profile first, because for many real people those are part of how they write.

---

## Rule zero: check the Keep list first

Before flagging anything, read the **Keep list** and **Vocabulary** in `voice-profile.md`. Anything on them is not an AI tell for this person, so don't penalize it and don't rewrite it.

The goal is a post that sounds like *them*, not a post that sounds like nobody.

---

## Always flag (these are never anyone's voice)

| # | Pattern | Example | Fix | Penalty |
|---|---------|---------|-----|---------|
| 1 | **Invented facts or story** | numbers, quotes, names, or results the user didn't give; also made-up backstory, things they "tried", feelings they didn't express, or personal details not from this conversation | remove, use a `[placeholder]`, or list under Flags for the user to confirm | -20 |
| 2 | **Vague attributions** | "Experts say", "Studies show", "Industry reports suggest" | name the source or cut it | -8 |
| 3 | **Chatbot leftovers** | "I hope this helps", "Certainly!", "Here's a post about..." | delete | -10 |
| 4 | **Knowledge-cutoff hedges** | "As of my last update", "based on available information" | delete | -10 |
| 5 | **Sycophancy** | "Great question!", "What an amazing insight!" | delete | -8 |
| 6 | **Filler phrases** | "In order to", "It is important to note that", "Due to the fact that" | "To", just say it, "Because" | -5 each |
| 7 | **Hedging stacks** | "could potentially possibly help" | commit, or say what's uncertain | -8 |
| 8 | **Empty significance inflation** | "a pivotal moment that marks a new era" | say what actually happened | -10 |
| 9 | **Fake-depth -ing tails** | "..., highlighting the importance of X and showcasing Y" | end the sentence, then add a real detail | -8 |
| 10 | **Generic conclusions** | "The future looks bright", "Exciting times ahead" (unless it's one of the owner's listed sign-offs) | end on the punchline or a question | -10 |
| 11 | **Synonym cycling** | "the CEO... the business leader... the company head" | pick one term | -5 |
| 12 | **False ranges** | "From content to culture, from SEO to storytelling..." | list what matters, plainly | -5 |
| 13 | **"Despite challenges..." formula** | "Despite these challenges, X continues to thrive" | name the challenge and the actual response | -10 |
| 14 | **Markdown on LinkedIn** | `**bold**`, `#` headings, code blocks in a LinkedIn post | remove (LinkedIn doesn't render it) | -5 |

## Flag unless the voice profile keeps it

| # | Pattern | Default fix | Penalty |
|---|---------|-------------|---------|
| 15 | **"Not X, it's Y" constructions** | allowed once per post as a punchline. More than once, rewrite as a direct statement | -5 |
| 16 | **AI-vocabulary clustering**: 3+ of these in one paragraph: delve, tapestry, realm, multifaceted, paramount, synergy, holistic, paradigm, embark, meticulous, commendable, intricate, interplay, garner, fostering, vibrant, profound, groundbreaking, cutting-edge, "ever-evolving landscape" | swap for plain words, **except** words in the voice profile's vocabulary | -10 |
| 17 | **Copula avoidance**: "serves as", "stands as", "boasts" instead of "is" or "has" | use "is" or "has" | -5 |
| 18 | **Emoji overload**: emoji on every line, or mid-sentence | trim to the profile's emoji habits | -5 |
| 19 | **Rule-of-three on autopilot**: *every* list or sentence is a triple | vary it. A single dash list of three takeaways is fine | -5 |
| 20 | **Dash overload**: dashes in most sentences | keep the ones that are real pauses in the person's rhythm | -3 |
| 21 | **Title Case In Every Line** | sentence case | -3 |
| 22 | **Hype words in tech posts**: game-changer, revolutionary, "the future is here", unlock, supercharge | describe the actual result | -8 |
| 23 | **Wall of text**: paragraphs over 3-4 lines on LinkedIn or X | break it up | -5 |
| 24 | **Hashtag spam**: more hashtags than the profile allows, or filler tags | trim to the profile's rule | -3 |

---

## Scoring

Start at 100. Deduct per pattern found. Repeats of the same pattern stack up to 2× the base penalty.

- **90-100**: sounds like the person. Ship it.
- **75-89**: a few tells. Fix them and re-score.
- **Below 75**: rewrite the flagged sections from the raw material, not by patching phrases.

Report the final score and a one-line summary of what you fixed, e.g. `Check: 94/100. Fixed: 1 vague attribution, cut "It is important to note".`

## What good looks like

- A real moment, detail, or number in the first 2 lines
- The person's own asides, humor, and vocabulary intact
- Varied rhythm: short punches mixed with fuller sentences
- A clear point of view
- Nothing invented
