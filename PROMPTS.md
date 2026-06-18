# 🤖 Claude Code Prompts — 6 Steps from Idea to Shipped App

> Claude Code is running in your repo folder. Type each prompt below **in order** into the Claude Code chat. Each step starts with **Claude asking you 2-3 quick questions** — that's intentional. Answer them, and Claude writes the result based on your decisions.

By Step 4 you'll have a working app. By Step 6 it's polished and ready to ship.

---

## 0️⃣ Step 0 — Share your idea (2 min)

```
I'm in an AI Build Workshop. We're going to build a small web app together
in about 60 minutes. I'll be your director — you do the heavy work,
but check in with me at each step so the result is mine, not generic.

Here's my idea in one sentence:

> [YOUR ONE SENTENCE IDEA — example:
>  "A daily prayer + gratitude tracker for my mom who is 65 and not super techy."]

Before we start, ask me 3 quick questions to understand my idea deeper:
1. Who exactly will use this? (be specific — name, age, comfort with tech)
2. What's the ONE thing this app should do best?
3. What would make this person smile when they open it?

After my 3 answers, summarize my idea in one short paragraph and ask:
"Approved? Ready to move to requirements?"
```

---

## 1️⃣ Step 1 — Define requirements (5 min)

```
Great. Now let's nail the requirements together.

First, ask me the 3 most important "spec-shaping" questions for my specific
idea — the decisions that will most affect what we build. Format each as a
short choice with 2-3 clear options (a / b / c) so I can answer fast.

Wait for my 3 answers.

Then write a one-page requirement spec to SPEC.md covering:
- The 1 core feature (the must-have)
- 2-3 nice-to-have features (only if time permits)
- Data: what gets saved? (we'll use localStorage in the browser)
- Inputs from the user (text? taps? choices from a list?)
- Constraints: single HTML file, no backend, no login, mobile-first
- One explicit "this app will NOT do X" (helps cut scope)

Then ask me: "Anything to add or remove before we design?"
```

---

## 2️⃣ Step 2 — Design the UI/UX (5 min)

```
Now let's design the UI/UX together.

First, ask me 2-3 design-shaping questions like:
- Mood / vibe (calm pastel? bold dark? playful? serene off-white?)
- One core visual choice (font feel: rounded / sharp / classic — or palette family)
- One small "delight" preference (subtle animation? confetti? gentle pulse? none — keep it quiet?)

Wait for my answers.

Then DO NOT write code yet — describe the design plain words and save to DESIGN.md:
- Overall layout on a phone screen, top to bottom
- Color palette (3-4 hex codes matching the chosen vibe)
- Typography (1 font for headings, 1 for body — web-safe or Google fonts)
- The first thing the user sees and the first thing they tap
- Key interactions (what happens when they tap X, save Y, complete Z)
- One small delightful detail (matching my preference from above)
- Mobile-first sizing (thumb-friendly tap targets)

After saving DESIGN.md, ask me:
"Does this match what you imagined? Want any changes before I build?"
```

---

## 3️⃣ Step 3 — Build the first working version (15-20 min)

```
Now let's build. First a quick check-in:

Ask me: "Should I build ALL of SPEC.md's core + nice-to-haves at once, or
JUST the core first so you can sanity-check before we add more?"

Wait for my answer.

Then build by editing index.html directly. Strict requirements:
- Keep it ONE SINGLE HTML FILE (no build step, no npm, no external files
  except the Tailwind CDN that's already there)
- Tailwind CSS via CDN (already in starter)
- Vanilla JavaScript only (no React, Vue, frameworks)
- localStorage for saving data (use the `store` helper that's already there)
- Mobile-first responsive
- Match the UI/UX from DESIGN.md

When done, show me a summary of what changed.
Then ask: "Want me to open index.html in your browser, or refine first?"
(You can also open it manually — just double-click index.html in your file
explorer, or run `start index.html` (Windows) / `open index.html` (Mac).)
```

---

## 4️⃣ Step 4 — Add features & iterate (10 min)

```
The base works. Now add the nice-to-haves we listed in SPEC.md.

First ask me: "Which nice-to-have should we add first? (give me the SPEC.md list
again, numbered, so I can pick)."

Wait for my pick. Add ONE feature at a time. After each:
1. Show me the diff of what changed
2. Ask "How does this feel? Add the next one, or refine this first?"

Don't add anything we didn't list in SPEC.md. If I think of something new,
I'll tell you.
```

---

## 5️⃣ Step 5 — Polish & make it shine (10 min)

```
The app works fully. Before I polish, ask me:

"Any specific thing that bugs you visually right now that you want me to fix
first? Or shall I do a standard polish pass — transitions, spacing,
typography hierarchy, and a small celebration moment?"

Wait for my answer.

Then polish index.html. Standard pass covers:
1. Smooth transitions on hover, tap, save (200-300ms ease-out)
2. Refine spacing — give breathing room, no cramped feel
3. Typography hierarchy — clear visual difference between title,
   content, actions
4. Add a small celebration or satisfying feedback for the main action
   (subtle — confetti, pulse, gentle color shift)
5. Make sure it's gorgeous on a phone screen
6. Verify it works offline (since we're using localStorage)

Do NOT change the function — just polish.
Show me the diff and the updated file.
```

---

## 6️⃣ Step 6 — Final review & ship (3 min)

```
One last pass on index.html. Run through this checklist out loud:

- Is the visual hierarchy obvious?
- Does the first interaction feel natural?
- Are the colors consistent (no accidental clash)?
- Mobile-friendly with thumb-sized tap targets?
- Does the "delight moment" feel earned, not annoying?
- Is the code clean enough that I could share it without being embarrassed?

For each "no" or "kind of", fix it. Show me the fixes briefly.

When the checklist is clean, ask me one final question:
"Anything else you want to change before we ship?"

If I say no, commit and push:

git add .
git commit -m "my v1 — ready for deploy"
git push

Then tell me: "Done. Pushed to main. Kemal will deploy."
```

---

## ✅ When the push is done

1. Confirm in the Meet chat: *"My app is pushed!"*
2. Kemal sees it, connects Cloudflare Pages, deploys.
3. Within a few hours you get a live URL: `https://buildschool-yourname.pages.dev`
4. Share it with anyone — it's yours forever.

---

## 🆘 Stuck mid-build?

- **Open [COACH.md](./COACH.md)** — the Workshop AI Coach (a separate Claude chat in your browser) knows the workshop format and unsticks you in 2 minutes
- **Type `@Kemal acil`** in the Meet chat — Kemal jumps to your screen-share
- **Ask Claude Code itself** — *"I'm stuck because [X]. Help me think through it."* Be specific about what's not working.

---

## 💡 Pro tips for talking to Claude Code

- **Be specific.** "Make it nicer" → vague. "Add 16px more padding to the card and switch the font to Inter" → clear.
- **Ask to see before changing.** "Show me what you'd change before applying it."
- **Iterate small.** One change at a time = easy to undo if you don't like it.
- **Commit often.** Every time something works, ask Claude to commit. It's a free undo button.
- **Don't fight the flow.** If Claude asks a question you weren't expecting, answer it — those questions usually surface a decision you should be making anyway.
