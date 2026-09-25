# Platform rules

The same idea needs different packaging on LinkedIn and X. LinkedIn is the default.

---

## LinkedIn

**Length**
- Hard limit: 3,000 characters.
- Sweet spot: 900-1,800 characters for story and opinion posts, 600-1,200 for stat posts.

**The hook lives above "...see more"**
- LinkedIn cuts the post after roughly the first 2-3 lines (fewer on mobile). The hook has to land there on its own.
- Line 1 should work even if it's the only thing someone reads. Don't spend it on setup ("So, last week I...").

**Formatting**
- LinkedIn does **not** render markdown. `**bold**`, `# headings`, and code blocks show up as literal symbols. Never use them in the post.
- Avoid "fancy" unicode bold or italic text generators. Screen readers can't read them and search can't find them.
- Use line breaks for rhythm: 1-3 lines per paragraph, blank line between.
- Lists: start lines with "- " (or the voice profile's list style).
- Tags: write `[@Name]` in the draft. The user converts these into real tags when posting.

**Links**
- A link in the post body is fine, but many creators put it in the first comment instead. If there's a link, add a note in Flags: "Link: put in first comment, or keep in post?"

**Hashtags**
- Follow the voice profile (for Sid: exactly 5 keyword hashtags at the end).
- Keyword hashtags only: real topics people search or follow. No filler like #motivation or #success.

**Ending**
- Story posts: punchline, then sign-off per the voice profile.
- Opinion, stat, tech posts: punchline, then a specific question for the comments.

**Visuals (LinkedIn has no text diagrams)**
Text diagrams made from keyboard characters don't line up on LinkedIn, so don't put them in the post. When a visual would help, add a **visual brief** in the notes instead:

```
Visual brief
Format:     single image | carousel (N slides) | photo suggestion
Focal point: the one thing the eye should hit first
On-image text: exact words (keep under ~12 words per image)
Layout:     e.g. "3 boxes left to right with arrows: Brief → Draft → Review"
Tone:       e.g. clean, brand colors, lots of white space
```

When a visual helps:
- **Stat post**: the stat as the image (big number, one line of context, source).
- **Tech-in-marketing post**: a simple workflow diagram (3-5 boxes with arrows).
- **Opinion post**: optional, a before/after or a two-column comparison.
- **Story post**: usually a real photo from the moment. Suggest what photo, don't design one.

If a Canva connector is available and the user wants the visual made, pass the visual brief as the design brief once the copy is final.

---

## X (Twitter)

**Length**
- Standard post: 280 characters.
- Long posts (X Premium) can run much longer. Only write long-form if the user says they have it.
- Otherwise, if the idea needs more than ~280 characters, write a **numbered thread**:
  - 1/ is the hook and must stand alone
  - each post is one idea, and each makes sense if read alone
  - 5-8 posts is typical, and the last one is the takeaway or question

**Voice adjustments for X**
- Tighter than LinkedIn. Cut the context, keep the punch.
- Fewer emoji (0-2 per post).
- Hashtags: 0-2, only if genuinely useful. Don't carry over the LinkedIn five.
- Asides and CAPS moments still work, just fewer of them.
- Sign-offs usually don't fit X. Only add one if asked.

**Text diagrams on X**
- Keyboard-character diagrams only line up where the text renders in monospace (for example, a code block in a long-form X article). Tell the user to check the preview before posting.
- Keep them under 40 characters wide and simple enough to read in 3 seconds:

```
Brief ──► Draft ──► Review ──► Ship
            ▲          │
            └──────────┘
             (rewrite)
```

- If it won't render cleanly, use a visual brief instead (same format as LinkedIn).

---

## "Both"

Write LinkedIn first, since it's the fuller version. Then adapt for X:
- Pull the sharpest line as the X hook.
- Compress to one post, or split into a thread.
- Swap the 5 hashtags for 0-2.
- Drop the sign-off.
