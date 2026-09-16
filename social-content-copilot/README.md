<!-- cover.png: drop a screenshot here showing a before (calendar row) / after (finished post) -->
![cover](./cover.png)

# Social Content Copilot

A Claude Skill that turns one content-calendar entry into a finished, on-brand social post — headline, supporting line, caption, hashtags, and creative direction — instead of a generic AI-sounding caption.

## The problem it solves

Most AI-generated social copy reads the same regardless of what kind of post it actually is — a stat post, a carousel, and a thought-leadership piece all need different structures, not just different words. This skill treats **post type** (why you're posting — brand awareness, thought leadership, announcement) and **creative type** (the format — carousel, stat post, single static) as first-class inputs, so the output actually matches the format instead of being one-size-fits-all filler text. It also carries over an existing brand voice if you give it a past post as a reference, and it hands off directly to Canva for a mockup once the copy is locked.

This is a rebuilt, genericized version of a workflow I use for real content calendars at work — same logic, fictional example brand ("Sentra AI") below so nothing from an actual employer shows up here.

## How to use it (no coding required)

1. You'll need Claude Code or claude.ai with Skills enabled — see [Anthropic's skills documentation](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) if you're not sure what that means or how to turn it on.
2. Download this folder (`social-content-copilot`) — either clone the whole repo, or click "Download" on just this folder on GitHub.
3. Add it as a skill in Claude following the "Add a skill" steps in the docs linked above (it's a drag-and-drop / upload step, nothing technical).
4. Once added, just talk to Claude naturally — mention your content calendar, a post type, or a creative type, and the skill kicks in automatically.

## Example

**You give it:**
> Post Type: Thought leadership. Creative Type: Stat post. Topic: confidence in AI systems is increasingly tied to how seriously companies take data privacy.

**It gives you back:**

> **Caption:**
> Privacy plays a bigger role in AI trust than most companies realize.
>
> As AI adoption accelerates, user confidence increasingly hinges on one thing: how seriously a company treats data privacy. A strong privacy foundation isn't a compliance checkbox — it's becoming the actual basis for trust.
>
> [source stat + citation would go here — always verify before posting]
>
> **Hashtags:** #AI #DataPrivacy #EnterpriseAI #DigitalTrust #SentraAI #Compliance #DataGovernance #Trust #PrivacyByDesign
>
> **Why no CTA:** this reads as a pure thought-leadership/stat post — the stat stays the visual hero and a CTA block would make it feel like a conversion post wearing a thought-leadership costume. Add one only if there's a specific asset (report, blog) to point to.
>
> **Suggested filename:** `thoughtleadership-statpost-ai-trust-privacy-2026-04.png`

## Built with

Claude (as a Skill), optionally the Canva MCP connector for generating the actual visual mockup once copy is finalized.
