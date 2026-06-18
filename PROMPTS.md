# 🤖 The One Prompt — Paste This Into Claude Code

> Paste the prompt below into Claude Code **once**. Replace the bracketed idea on line 6 with your own. After that, just **answer Claude's questions** as they come — Claude paces the journey for you.
>
> By the end of the conversation (about 50 minutes), you'll have a working, polished app pushed to your repo.

---

```
I'm in an AI Build Workshop. We'll build a small web app together in
about 60 minutes. I'll be your director — you do the heavy work, but
check in with me at each phase so the result is mine, not generic.

Here's my idea in one sentence:

> [REPLACE THIS BRACKET WITH YOUR ONE-SENTENCE IDEA — example:
>  "A daily prayer + gratitude tracker for my mom who is 65 and not super techy."]

We'll go through 6 phases. After each phase, you stop and ask me to
approve before moving on. Don't skip the check-ins.

═══════════════════════════════════════════════════════════════════════
PHASE 0 — UNDERSTAND (2 min)

Ask me 3 quick questions to understand the idea deeper:
1. Who exactly will use this? (name, age, comfort with tech)
2. What's the ONE thing this app should do best?
3. What would make this person smile when they open it?

After my 3 answers, summarize my idea in one short paragraph and ask:
"Approved? Ready to move to requirements?"

WAIT for my "approved" before starting Phase 1.

═══════════════════════════════════════════════════════════════════════
PHASE 1 — REQUIREMENTS (5 min)

Ask me the 3 most important "spec-shaping" questions for MY specific idea —
the decisions that will most affect what we build. Format each as a short
choice with 2-3 options (a / b / c) so I can answer fast.

WAIT for my 3 answers.

Then write a one-page spec to SPEC.md covering:
- The 1 core feature (the must-have)
- 2-3 nice-to-have features (only if time permits)
- Data: what gets saved (we'll use localStorage)
- Inputs from the user (text? taps? choices?)
- Constraints: single HTML file, no backend, no login, mobile-first
- One explicit "this app will NOT do X" (cut scope)

Show me the spec. Ask: "Anything to add or remove before we design?"
WAIT for my "looks good" before Phase 2.

═══════════════════════════════════════════════════════════════════════
PHASE 2 — DESIGN (5 min)

Ask me 2-3 design-shaping questions, e.g.:
- Mood / vibe (calm pastel? bold dark? playful? serene off-white?)
- One visual choice (font feel: rounded / sharp / classic — or palette family)
- One delight preference (subtle animation? confetti? gentle pulse? none?)

WAIT for my answers.

Then DO NOT write code yet — describe the design in plain words and save
to DESIGN.md:
- Overall layout on a phone screen, top to bottom
- Color palette (3-4 hex codes matching the chosen mood)
- Typography (1 heading font + 1 body font, web-safe or Google fonts)
- The first thing the user sees + the first thing they tap
- Key interactions (what happens when they tap X, save Y, complete Z)
- One small delightful detail (matching my preference)
- Mobile-first sizing (thumb-friendly tap targets)

Ask: "Does this match what you imagined? Want changes before I build?"
WAIT for my "approve" before Phase 3.

═══════════════════════════════════════════════════════════════════════
PHASE 3 — BUILD (15-20 min)

Ask me one thing: "Build the FULL spec (core + nice-to-haves) at once,
or just the CORE first so you can sanity-check before we add more?"

WAIT for my answer.

Then build by editing index.html in place. Strict requirements:
- Keep it ONE SINGLE HTML FILE (no build step, no npm, no external files
  except the Tailwind CDN already in the starter)
- Tailwind CSS via CDN
- Vanilla JavaScript only (no React, Vue, frameworks)
- localStorage for saving data (use the `store` helper already in the file)
- Mobile-first responsive
- Match the UI/UX from DESIGN.md

When done, show me a brief summary of what changed and ask:
"Want to open index.html in your browser to test it, or refine first?"
(I can open it by double-clicking the file, or running `start index.html`
on Windows / `open index.html` on Mac.)
WAIT for my response before Phase 4.

═══════════════════════════════════════════════════════════════════════
PHASE 4 — ITERATE (10 min)

If we only built the core in Phase 3, now add the nice-to-haves.

First ask: "Which nice-to-have from SPEC.md should we add first?"
(List them again, numbered, so I can pick.)

WAIT for my pick. Add ONE feature at a time. After each:
1. Show me a short diff of what changed
2. Ask "How does this feel? Add the next one, or refine this first?"
3. WAIT for my answer

Don't add anything that isn't in SPEC.md. If I think of something new,
I'll tell you.

When I say I'm satisfied, move to Phase 5.

═══════════════════════════════════════════════════════════════════════
PHASE 5 — POLISH (10 min)

Ask me: "Anything bugging you visually right now that you want me to fix
first? Or shall I do a standard polish pass — smooth transitions, spacing,
typography hierarchy, and a small celebration moment?"

WAIT for my answer.

Then polish index.html. Standard pass covers:
1. Smooth transitions on hover, tap, save (200-300ms ease-out)
2. Refine spacing — breathing room, no cramped feel
3. Typography hierarchy — clear visual difference between title, content, actions
4. A small celebration / satisfying feedback for the main action
   (subtle — confetti, pulse, gentle color shift; NOT loud)
5. Make sure it's gorgeous on a phone screen
6. Verify it works offline (since we're using localStorage)

Do NOT change the function — only polish.
Show me the diff. Ask: "Approve, or any last tweaks?"
WAIT for my approval before Phase 6.

═══════════════════════════════════════════════════════════════════════
PHASE 6 — SHIP (3 min)

Run through this checklist out loud, one item at a time:

- Is the visual hierarchy obvious?
- Does the first interaction feel natural?
- Are the colors consistent (no accidental clash)?
- Mobile-friendly with thumb-sized tap targets?
- Does the "delight moment" feel earned, not annoying?
- Is the code clean enough that I could share it without being embarrassed?

For each "no" or "kind of," fix it. Show me each fix briefly.

When the checklist is clean, ask me one final question:
"Anything else you want to change before we ship?"

If I say no, commit and push:

git add .
git commit -m "my v1 — ready for deploy"
git push

Then tell me: "Done. Pushed to main. Kemal will deploy."

═══════════════════════════════════════════════════════════════════════

START WITH PHASE 0 NOW. Don't skip ahead.
```

---

## ✅ When the push is done

1. Confirm in the Meet chat: *"My app is pushed!"*
2. Kemal sees it, connects Cloudflare Pages, deploys.
3. Within a few hours you get a live URL: `https://buildschool-yourname.pages.dev`
4. Share it with anyone — it's yours forever.

---

## 💛 Pay it forward

This workshop is a **SafeScreens Initiative fundraiser** — every donation funds the next round of kids learning to **make** instead of just consume.

If tonight helped you, share **[build.safescreensinitiative.org](https://build.safescreensinitiative.org)** with one friend who would build something too. Or join the next tier:

- **Studio Cohort 1** (4 weeks · starts Friday June 27) — take your app from Tier 1 to Tier 2 (real LLM-powered, your own domain)
- **One-time donation** — $25, $100, $500, or your choice. Tax-deductible under SafeScreens' 501(c)(3) status.

Children grow into who they're surrounded by. Surround them with creators.

---

## 🆘 Stuck mid-build?

- **Open [COACH.md](./COACH.md)** — the Workshop AI Coach (a separate Claude chat in your browser) knows the workshop format and unsticks you in 2 minutes
- **Type `@Kemal acil`** in the Meet chat — Kemal jumps to your screen-share
- **Ask Claude Code itself** — *"I'm stuck because [X]. Help me think through it."* Be specific about what's not working.

---

## 💡 Pro tips

- **Just answer Claude's questions.** Don't search the prompt for "what do I do next" — Claude will tell you.
- **Be specific in answers.** "Calm and quiet" → vague. "Off-white background, serif headings, no animations" → clear.
- **If Claude skips a check-in,** type: *"Wait — I want to approve before you move to the next phase."*
- **Commit often.** When something works, type: *"Commit this with a short message."* — it's a free undo button.
- **Don't fight the flow.** If Claude asks something you didn't expect, answer it. Those questions surface decisions you should be making anyway.
