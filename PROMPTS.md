# 🤖 Claude Code Prompts — 6 Steps from Idea to Shipped App

> Claude Code is running in your repo folder. Type each prompt below **in order** into the Claude Code chat. Claude Code reads and edits your files directly — no copy-pasting HTML between tabs.

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
Great. Now let's nail the requirements.

Write a one-page requirement spec for my idea covering:

- The 1 core feature (the must-have)
- 2-3 nice-to-have features (only if time permits)
- Data: what gets saved? (we'll use localStorage in the browser)
- Inputs from the user (text? taps? choices from a list?)
- Constraints: single HTML file, no backend, no login, mobile-first

Save this spec into a new file called SPEC.md in the repo.

Then ask me: "Want to add or remove anything before we design?"
```

---

## 2️⃣ Step 2 — Design the UI/UX (5 min)

```
Now design the UI/UX. DO NOT write code yet — describe in plain words and
save to a new file called DESIGN.md:

- Overall layout on a phone screen, top to bottom
- Color palette (3-4 hex codes matching the user's vibe — calm, playful,
  serene, bold)
- Typography (1 font for headings, 1 for body — web-safe or Google fonts)
- The first thing the user sees and the first thing they tap
- Key interactions (what happens when they tap X, save Y, complete Z)
- One small delightful detail that will make them smile
- Mobile-first sizing (thumb-friendly tap targets)

After saving DESIGN.md, ask me:
"Does this match what you imagined? Want any changes before I build?"
```

---

## 3️⃣ Step 3 — Build the first working version (15-20 min)

```
Now build the app by editing index.html directly. Strict requirements:

- Keep it ONE SINGLE HTML FILE (no build step, no npm, no external files
  except the Tailwind CDN we already have)
- Tailwind CSS via CDN (already in starter)
- Vanilla JavaScript only (no React, Vue, frameworks)
- localStorage for saving data (use the store helper that's already there)
- Mobile-first responsive
- Match the UI/UX from DESIGN.md
- Build the ONE core feature first — nice-to-haves come later

Edit index.html in place. When done, show me a summary of what changed.
Then ask: "Want me to open index.html in your browser so you can see it?"
(You can open it manually too — just double-click index.html in the file explorer.)
```

---

## 4️⃣ Step 4 — Add features & iterate (10 min)

```
The base works. Now add the nice-to-haves we listed in SPEC.md.

Add them ONE AT A TIME. After each:
1. Show me the diff of what changed
2. Ask "How does this feel? Add the next one, or refine this first?"

Don't add anything we didn't list. If I think of something new, I'll tell you.
```

---

## 5️⃣ Step 5 — Polish & make it shine (10 min)

```
The app works fully. Now polish index.html. Do these specifically:

1. Smooth transitions on hover, tap, save (200-300ms ease-out)
2. Refine spacing — give breathing room, no cramped feel
3. Typography hierarchy — clear visual difference between title,
   content, actions
4. Add a small celebration or satisfying feedback for the user's
   main action (subtle — confetti, pulse, gentle color shift)
5. Make sure it's gorgeous on a phone screen
6. Verify it works offline (since we're using localStorage)

Do NOT change the function — just polish.
Show me the diff and the updated file.
```

---

## 6️⃣ Step 6 — Final review & ship (3 min)

```
One last pass on index.html. Check:

- Is the visual hierarchy obvious?
- Does the first interaction feel natural?
- Are the colors consistent (no accidental clash)?
- Mobile-friendly with thumb-sized tap targets?
- Does the "delight moment" feel earned, not annoying?
- Is the code clean enough that I could share it without being embarrassed?

If anything still needs work, fix it first. Then commit and push:

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

- **Open a second Claude chat** in your browser (not in Claude Code) and paste the **Workshop AI Coach prompt** Kemal shared in the Meet chat. That second Claude knows the workshop format and helps in 2 minutes.
- **Type `@Kemal acil`** in the Meet chat — Kemal jumps to your screen-share.
- **Ask Claude Code itself** — *"I'm stuck because [X]. Help me think through it."* Be specific about what's not working.

---

## 💡 Pro tips for talking to Claude Code

- **Be specific.** "Make it nicer" → vague. "Add 16px more padding to the card and switch the font to Inter" → clear.
- **Ask to see before changing.** "Show me what you'd change before applying it."
- **Iterate small.** One change at a time = easy to undo if you don't like it.
- **Commit often.** Every time something works, ask Claude to commit. It's a free undo button.
