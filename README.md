# 🚀 Build Your Idea in 1 Hour — AI Workshop Starter

> Bring an idea. Build it with Claude Code. Ship a working app tonight.

A starter from the **AI Build Workshop** by SafeScreens Initiative. Customize this empty shell into anything — habit tracker, family game, study tool, journal — with the help of Claude Code in your terminal.

---

## 👋 What this is

A blank-slate web app. Same starter for any idea you bring:

- A daily habit tracker
- A family chore wheel
- A kids' story generator
- A budget tool
- A study quiz
- ...whatever you bring

The structure is the same; **your idea makes it yours**.

---

## ✅ Before tonight — 3 things (10 min total)

Do these **before the workshop starts** so the live session can focus on building, not configuring:

### 1. Get a GitHub account (2 min)

Skip if you already have one. Otherwise:

1. Go to **[github.com/signup](https://github.com/signup)**
2. Use any email (gmail works fine)
3. Pick a username — choose something you like, it becomes part of your URL
4. Verify your email

### 2. Send your GitHub username to Kemal (1 min)

Send via WhatsApp or in the workshop Meet chat: **"My GitHub username is `your-username`"**.

Kemal will use it to:
- Create your personal repo at `github.com/profkemalaydin/buildschool-yourname`
- Add you as a **collaborator** with push access (so you can save your changes)

### 3. Accept the collaboration invitation (1 min)

After Kemal creates your repo, you'll get a **GitHub email** with a "View invitation" button — click it and accept. Without this, you can't push code to your repo.

You can also accept directly at: **[github.com/notifications](https://github.com/notifications)**

✅ Done — you're set up before the live session even starts.

---

## 🛠 Setup tonight — Install Claude Code (15-20 min, Kemal walks through live)

We'll do this together in the first 20 minutes of the workshop. Don't worry about doing it perfectly alone — Kemal screen-shares and helps.

Pick your operating system. All paths end the same way: Claude Code running in your repo folder.

### 🍎 macOS

1. Open **Terminal** (Cmd+Space → "Terminal" → Enter)
2. **Install Homebrew** (skip if you already have it):

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

3. **Install Node.js, Git, GitHub CLI:**

   ```bash
   brew install node git gh
   ```

4. **Install Claude Code:**

   ```bash
   npm install -g @anthropic-ai/claude-code
   ```

5. **Log in to GitHub** (browser will open):

   ```bash
   gh auth login
   ```

   Choose: GitHub.com → HTTPS → Yes → Login with browser.

6. **Clone your repo** (replace `your-name` with the slug Kemal gave you — only works after you've accepted the invitation from "Before tonight" step 3):

   ```bash
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

7. **Start Claude Code:**

   ```bash
   claude
   ```

   Log in with your Claude account when prompted. You're ready → jump to [PROMPTS.md](./PROMPTS.md).

---

### 🪟 Windows

1. **Install Node.js LTS** — download from [nodejs.org](https://nodejs.org) → run installer (defaults are fine)
2. **Install Git** — download from [git-scm.com](https://git-scm.com/download/win) → run installer (defaults are fine)
3. **Install GitHub CLI** — download from [cli.github.com](https://cli.github.com) → run installer
4. **Open PowerShell or Windows Terminal** (Start menu → search "Terminal")
5. **Install Claude Code:**

   ```powershell
   npm install -g @anthropic-ai/claude-code
   ```

6. **Log in to GitHub** (browser will open):

   ```powershell
   gh auth login
   ```

   Choose: GitHub.com → HTTPS → Yes → Login with browser.

7. **Clone your repo** (replace `your-name` with the slug Kemal gave you — only works after you've accepted the invitation from "Before tonight" step 3):

   ```powershell
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

8. **Start Claude Code:**

   ```powershell
   claude
   ```

   Log in when prompted → ready → jump to [PROMPTS.md](./PROMPTS.md).

---

### 🐧 Linux (Ubuntu / Debian / WSL)

1. Open a **terminal**
2. **Install Node.js + npm + Git:**

   ```bash
   sudo apt update
   sudo apt install -y nodejs npm git
   ```

   *(If `nodejs --version` shows older than 18, use NodeSource: `curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash - && sudo apt install -y nodejs`)*

3. **Install GitHub CLI:**

   ```bash
   sudo apt install -y gh
   ```

4. **Install Claude Code:**

   ```bash
   sudo npm install -g @anthropic-ai/claude-code
   ```

5. **Log in to GitHub** (browser will open):

   ```bash
   gh auth login
   ```

   Choose: GitHub.com → HTTPS → Yes → Login with browser.

6. **Clone your repo** (replace `your-name` with the slug Kemal gave you — only works after you've accepted the invitation from "Before tonight" step 3):

   ```bash
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

7. **Start Claude Code:**

   ```bash
   claude
   ```

   Log in when prompted → ready → jump to [PROMPTS.md](./PROMPTS.md).

---

## 🎬 The workflow tonight

1. **You and Kemal are both collaborators** on your repo. You push changes; Kemal handles the Cloudflare deploy.
2. **Claude Code runs in your repo's folder** — it can directly read and edit your files as you talk to it.
3. **Open [PROMPTS.md](./PROMPTS.md)** — paste each prompt into Claude Code, in order.
4. **By Step 4** you'll have a working app. **By Step 6** it's polished.
5. **When you're happy:** tell Claude Code *"Commit and push my changes"* — it does it.
6. **Kemal sees your push and deploys** to `https://buildschool-yourname.pages.dev` — link by email.

---

## ✏️ When Claude Code is done — push your work

In Claude Code, just type:

```
Commit my changes with message "my v1" and push to main.
```

Claude Code handles the git commit + push for you.

---

## 🔁 After the workshop — build another idea

Click the green **`Use this template`** button at the top of [workshop-starter](https://github.com/profkemalaydin/workshop-starter). That creates a brand-new repo on your account with this same starter — keep building independently.

---

## 🆘 Stuck during the build?

You have **3 layers of help**:

1. **The prompts themselves** — written to anticipate where you might get stuck
2. **Workshop AI Coach** — open a *second* Claude chat in your browser (claude.ai, NOT Claude Code) and paste the prompt below. That second Claude knows the workshop structure and unsticks you in 2 minutes:

   ```
   You are my AI build coach for the SafeScreens "Build Your App in 1 Hour"
   workshop. Workshop is happening live — June 17, 2026, 21:30–22:30 ET.

   YOUR JOB
   - Help me ship a working prototype in 60 minutes
   - When I'm stuck, ask 1-2 clarifying questions first (which block am I in,
     which tool, what error)
   - Answers: short, action-oriented, baby-step
   - "Ship over polish" — working beats perfect
   - Reject features that won't fit in 60 min ("note for v2")
   - Tone: encouraging but honest. No fluff.

   WORKSHOP BLOCKS
   0–3 min   Welcome
   3–10 min  Frame: why AI now
   10–15 min Spec your app (1 sentence)
   15–20 min Claude Code setup
   20–50 min Build — this is where most help is needed
   50–57 min Show & Tell
   57–60 min Close + next

   START WITH
   "Hey! I'm your workshop coach 👋 Tell me three things:
    1) What are you building, in one sentence?
    2) Which block are you in? (e.g. 'spec' or 'build, 15 min in')
    3) Which tool? (Claude Code, claude.ai web, other)
   Let's go."

   EMERGENCY ESCAPE
   If we can't solve it in 5 minutes, tell me to type "@Kemal acil" in
   the Meet chat — Kemal will jump on directly.

   10 STARTER IDEAS (show if my answer to #1 is blank)
   1.  Family chore tracker (gamified, kid-friendly)
   2.  Recipe finder (paste ingredients, get meal idea)
   3.  Daily Quran/Bible verse + reflection
   4.  Spelling/vocab quiz
   5.  Habit streak counter
   6.  Family chore wheel (random assignment)
   7.  Newsletter draft assistant (TR + EN)
   8.  Gratitude journal
   9.  Water intake reminder
   10. Kids story maker (pick hero + plot)

   BACKGROUND
   Workshop is a SafeScreens fundraiser — proceeds support children's
   screen-health initiatives. https://build.safescreensinitiative.org

   Now, ask me your first three questions.
   ```

3. **Type `@Kemal acil` in the Meet chat** — Kemal jumps into your screen-share and helps personally

---

## 📦 What's in this starter

| File | Purpose |
|---|---|
| `index.html` | Working "hello, your app" page with Tailwind CSS pre-wired, localStorage helpers ready |
| `PROMPTS.md` | The 6-step Claude Code conversation guide |
| `LICENSE` | MIT — yours to keep |

The starter is **deliberately minimal** so Claude has room to make it yours.

---

## 📝 License

MIT — fork it, remix it, build a business with it. Yours to keep.
