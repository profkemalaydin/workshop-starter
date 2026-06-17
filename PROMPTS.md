# 🤖 Claude Prompts — 6 Steps from Idea to Shipped App

> Open **claude.ai** in a new browser tab and start a fresh conversation.
> Paste each prompt below **in order**. Answer Claude's questions, then move to the next prompt.
> By Step 4 you'll have a working app. By Step 6 it'll be polished and ready to ship.

---

## 0️⃣ Step 0 — Share your idea (2 min)

```
I'm in an AI Build Workshop. We're going to build a small web app together
in about 60 minutes. I'll be your "director" — you do the heavy work,
but you'll check in with me at each step so the result is mine, not generic.

Here's my idea in one sentence:

> [YOUR ONE SENTENCE IDEA HERE — example:
>  "A daily prayer + gratitude tracker for my mom who is 65 and not super techy."]

Before we start, ask me 3 quick questions to understand it deeper:
1. Who exactly will use this? (be specific — name, age, comfort with tech)
2. What's the ONE thing this app should do best? (resist the urge to add features)
3. What would make this person smile when they open it?

After my 3 answers, summarize my idea back to me in one short paragraph
and ask: "Approved? Ready to move to requirements?"
```

---

## 1️⃣ Step 1 — Define requirements (5 min)

```
Great. Now let's nail the requirements.

Based on my idea, write a one-page requirement spec covering:

- The 1 core feature (the must-have)
- 2-3 nice-to-have features (only if time permits)
- Data: what gets saved? (we'll use localStorage in the browser)
- Inputs from the user (text? taps? choices from a list?)
- Constraints (single HTML file, no backend, no login, mobile-first)

Then ask me: "Want to add or remove anything before we design?"
```

---

## 2️⃣ Step 2 — Design the UI/UX (5 min)

```
Now design the UI/UX. DO NOT write code yet. Describe in plain words:

- Overall layout on a phone screen, top to bottom
- Color palette (3-4 hex codes that match the user's vibe — calm, playful,
  serene, bold — pick what fits)
- Typography (1 font for headings, 1 for body — both web-safe / Google fonts)
- The first thing the user sees and the first thing they tap
- Key interactions (what happens when they tap X, save Y, complete Z)
- One small delightful detail that will make them smile
- Mobile-first sizing (thumb-friendly tap targets)

Show me the design as a clear plan. Then ask:
"Does this match what you imagined? Want any changes before I build?"
```

---

## 3️⃣ Step 3 — Build the first working version (15-20 min)

```
Now build the app. Strict requirements:

- ONE SINGLE HTML FILE (no build step, no npm, no external files except CDN)
- Tailwind CSS via CDN: <script src="https://cdn.tailwindcss.com"></script>
- Vanilla JavaScript (no React, Vue, frameworks)
- localStorage for saving data
- Mobile-first responsive
- Match the UI/UX design from step 2
- Build the ONE core feature first — nice-to-haves come later

Show me the FULL HTML.
After I see it, I'll tell you what to adjust or what feature to add next.
```

---

## 4️⃣ Step 4 — Add features & iterate (10 min)

```
The base works. Now let's add the nice-to-haves we discussed in step 1.

Add them ONE AT A TIME. After each, show me the updated full HTML and ask:
"How does this feel? Add the next one, or refine this first?"

Don't add anything we didn't list. If I think of something new, I'll tell you.
```

---

## 5️⃣ Step 5 — Polish & make it shine (10 min)

```
The app works fully. Now polish it. Do these specifically:

1. Smooth transitions on hover, tap, save (200-300ms ease-out)
2. Refine spacing — give breathing room, no cramped feel
3. Typography hierarchy — clear visual difference between title, content, actions
4. Add a small celebration or satisfying feedback for the user's main action
   (subtle, not annoying — confetti, pulse, gentle color shift)
5. Make sure it's gorgeous on a phone screen
6. Verify it works offline (since we're using localStorage)

Do NOT change the function — just polish.
Show me the updated full HTML.
```

---

## 6️⃣ Step 6 — Final review & ship (3 min)

```
One last pass. Check:

- Is the visual hierarchy obvious?
- Does the first interaction feel natural?
- Are the colors consistent (no accidental clash)?
- Mobile-friendly with thumb-sized tap targets?
- Does the "delight moment" feel earned, not annoying?
- Is the code clean enough that I could share it without being embarrassed?

If yes, give me the FINAL CLEAN HTML.
If anything still needs work, fix it first, THEN give me the final HTML.

This is the version I'll commit to my GitHub repo for deployment.
```

---

## ✅ When you have the final HTML

1. Go to your GitHub repo (Kemal sent you the link)
2. Click `index.html` → pencil icon → select all → paste your final HTML
3. Commit with a small message ("my app, v1")
4. Tell Kemal in Meet chat that you're done
5. Kemal deploys → you get a live URL within 24 hours

---

## 🆘 Stuck mid-build?

- **Workshop AI Coach** — open a *second* Claude chat, paste the Coach prompt Kemal shared
- **Type `@Kemal acil`** in the Meet chat — Kemal will help directly
- **Ask Claude itself** — *"I'm stuck because [X]. Help me think through it."* Claude is good at unsticking when you describe the problem clearly.
