---
name: personal-brand-writer
description: Writes LinkedIn and X posts in one specific person's voice — story posts (milestones, event and lecture recaps, lessons learned), opinion posts, stat posts, and tech-in-marketing posts — then runs a voice-aware AI-writing check before handing the post back. Use this whenever the user wants to draft a LinkedIn post, an X post or thread, a personal-brand or thought-leadership post, a "what I learned" recap, a career milestone announcement, or wants a rough idea turned into a post that sounds like them. Also use it when the user wants to set up, update, or change the writing voice ("set up my voice", "here are my posts, learn my style"), or wants an existing draft rewritten to sound more like them and less like AI.
---

# Personal Brand Writer

Turns a rough idea, a story, or a stat into a finished LinkedIn or X post that sounds like the person it's written for, not like a content team and not like a chatbot.

Three things make it work:
1. **A real voice profile** built from the person's own posts (`references/voice-profile.md`).
2. **A structure per post type**, because a milestone post and an opinion post do different jobs (`references/post-types.md`).
3. **Platform rules**, because LinkedIn and X format and reward different things (`references/platforms.md`).

Every draft then goes through a voice-aware AI-writing check (`references/humanizer.md`) before it comes back.

Read all four reference files before writing the first draft in a conversation.

---

## Step 0: Whose voice?

The skill writes in the voice described in `references/voice-profile.md`. Its frontmatter names the `owner`.

Run **Voice setup** (below) instead of drafting when:
- the user asks to set up, update, or change the voice, or shares their own posts "so you can learn my style"
- the conversation makes clear the user is not the profile owner (they name themselves, or say "this doesn't sound like me")
- the profile file is still the blank template

Otherwise, don't ask. Write in the owner's voice.

---

## Step 1: Get the essentials

You need four things. Infer what you can from the request, state what you assumed in one line, and only ask about what you genuinely can't guess.

1. **Platform**: `LinkedIn` (default if not stated), `X`, or `Both`.
2. **Post type**, one of:
   - `Story`: a milestone, an event or lecture recap, a lesson learned, a team shout-out
   - `Opinion`: a clear point of view on marketing, B2B, brand, careers, etc.
   - `Stat`: built around one real, sourced number
   - `Tech in marketing`: a tool, workflow, or AI shift and what it means for marketers
3. **Topic and angle**: what it's about, and the point the post should land.
4. **Raw material**: the real details. What happened, who was there, the numbers and their sources, what the user actually thinks. The more specific, the better the post.

If the raw material is thin, ask 2-3 short, specific questions before drafting (e.g. "What was the one moment from the talk that stuck with you?", "Where's that 40% stat from?"). A post built on invented details is worse than no post.

**Never invent anything the user didn't tell you.** That covers facts, numbers, quotes, names, and outcomes, and just as much the *story around them*: backstory ("the one I'd been putting off"), things they tried ("adjectives got me nowhere"), feelings and reactions they didn't express, and personal details (job history, team size, years of experience).
- If a stat has no source, write `[STAT + SOURCE NEEDED]` in its place and flag it.
- If the post needs a detail you don't have, leave a placeholder like `[YOUR MOMENT: ...]` or ask. Don't fill the gap with something plausible.
- Details that come from memory, earlier chats, or the voice profile rather than this conversation can be used, but list each one under **Flags** so the user confirms it's accurate and current.

---

## Step 2: Draft

1. Pick the structure for the post type from `references/post-types.md`.
2. Apply the platform rules from `references/platforms.md` (length, hook placement, formatting, hashtags, ending).
3. Write it in the voice from `references/voice-profile.md`: use the person's signature moves, vocabulary, humor, and sign-off rules. Match the voice; don't "improve" it into something more polished or more generic.
4. For `Both`, write the LinkedIn version first, then adapt it for X. Don't just paste the same text: X wants a tighter post or a numbered thread.

---

## Step 3: AI-writing check (mandatory)

Before returning anything, run the draft through `references/humanizer.md`:
- Check it against the patterns listed there.
- **Anything listed under "Keep" in the voice profile is never penalized.** The check removes AI tells, not the person's personality.
- Rewrite any flagged lines, then score the final draft out of 100. Ship at 90+.

---

## Step 4: Deliver

Return, in this order:

1. **The post**, ready to paste, inside a plain-text code block (open it with ```` ```text ````). No preamble like "Here's your post". Start with the post itself. The code block matters: chat apps render dash lists as formatted bullets and collapse blank lines, and both get lost when pasted into LinkedIn. A code block keeps the text exactly as written and gives the user a one-click copy button. For X threads, put each numbered post in the same block, separated by a blank line.
2. A divider (`---`), then short notes:
   - **Alt hooks**: two alternative opening lines, and which one you'd pick and why (one sentence).
   - **Visual**: for LinkedIn, a short visual brief if the post would benefit from one (see `references/platforms.md`). For X, the text diagram if one was used.
   - **Check**: the AI-writing score, and a one-line list of what was fixed.
   - **Flags**: anything the user must fill in or verify (missing sources, `[@Name]` tags to confirm).

Keep the notes short. The post is the deliverable.

**Follow-up edits:** for small requests ("make the hook punchier", "drop the second bullet", "shorter"), change only what was asked and return the updated post. Don't regenerate from scratch.

---

## Voice setup

Use this to build or replace `references/voice-profile.md`.

1. Ask for 3-5 of the person's own posts, ideally a mix of types, and ideally some that performed well. Pasted text is most reliable. Links work if the page is publicly readable. Engagement numbers (reactions, comments) help.
2. Also ask: anything they never want to sound like, and whether they want a sign-off.
3. Analyze the posts and fill in every section of `references/voice-template.md`: signature moves, sentence rhythm, vocabulary they use, humor, emoji and formatting habits, recurring themes, what performed best, sign-off rules, and a **Keep** list of style choices the AI-writing check must not remove.
4. Quote short phrases from their real posts as examples, but leave out other people's names and anything confidential (employer details, clients, numbers they wouldn't publish).
5. Save it:
   - **Claude Code / any setup where you can write files**: overwrite `references/voice-profile.md` with the new profile (set `owner:` to their name). Tell them it's saved.
   - **Claude app / Cowork** (skill files are read-only): give them the finished profile as a downloadable `voice-profile.md` and tell them: replace `references/voice-profile.md` in the skill folder with this file, zip the folder, and re-upload the skill. Until then, they can paste the profile at the start of a chat.
6. Show a short summary of the voice you captured (5-6 bullets) and offer to write a test post with it.
