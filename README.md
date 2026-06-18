# 🚀 Build Your Idea in 1 Hour — AI Workshop Starter

> Bring an idea. Build it with Claude Code. Ship a working app tonight.

A starter from the **AI Build Workshop** by SafeScreens Initiative. Customize this empty shell into anything — habit tracker, family game, study tool, journal — with the help of Claude Code in your terminal.

> 💛 **Don't worry if something fails during setup.** The goal isn't to finish alone — it's to get everyone into the repo and run Claude Code together. Kemal screen-shares every step and unblocks you live.

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

## ✅ Before tonight — 6 things (10 min total)

Knock these out before the workshop starts so the live session can focus on building, not configuring:

1. **Create or confirm your GitHub account** — [github.com/signup](https://github.com/signup) (2 min if you don't have one)
2. **Add yourself to the workshop sign-up sheet** — name + GitHub username + one-sentence idea → **[Workshop sign-up sheet](https://docs.google.com/spreadsheets/d/1lVzVVg_3B4jm5zGTbv3aS50Frn4lhhhoCe8NXc-hxaY/edit)**
3. **Accept the GitHub repository invitation** Kemal will send to your email (the repo is `github.com/profkemalaydin/buildschool-yourname`). Without accepting, you can't push code.
4. **Create or confirm a Claude account** that has Claude Code access. **Claude Code requires Pro, Max, Team, Enterprise, or Console** — the free Claude.ai plan does **not** include Claude Code. Check or upgrade at [claude.ai](https://claude.ai).
5. **Bring your laptop charger** — an hour of build + AI streaming drains a battery fast.
6. **Use Chrome or another modern browser** — for the GitHub login flow and Claude streaming UI.

---

## 🛠 Setup tonight — Install Claude Code (15-20 min, Kemal walks through live)

Pick your operating system. Each path ends the same way: Claude Code running in your repo folder.

> Anthropic's recommended path for Claude Code is the **native installer** — much cleaner than npm. We'll use that below.

---

### 🍎 macOS

1. Open **Terminal** (Cmd+Space → "Terminal" → Enter)
2. **Install Homebrew** (skip if you already have it):

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

3. **Install Git + GitHub CLI** (Node.js is optional — only needed for our project later):

   ```bash
   brew install git gh
   ```

4. **Install Claude Code with the native installer:**

   ```bash
   curl -fsSL https://claude.ai/install.sh | bash
   ```

5. **Verify installs:**

   ```bash
   git --version
   gh --version
   claude --version
   claude doctor
   ```

   `claude doctor` runs a self-check — if anything's missing it tells you exactly what.

6. **Set your Git identity** (first time only):

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```

7. **Log in to GitHub** (browser opens):

   ```bash
   gh auth login
   ```

   Choose: GitHub.com → HTTPS → Yes → Login with browser. After it finishes:

   ```bash
   gh auth status
   ```

   should show ✓ Logged in.

8. **Clone your repo** (replace `your-name` with the slug Kemal gave you — only works *after* you've accepted the invitation from "Before tonight" step 3):

   ```bash
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

9. **Start Claude Code:**

   ```bash
   claude
   ```

   Log in with your Claude account when prompted. You're ready → open the prompts file:

   ```bash
   cat PROMPTS.md
   ```

   (or if you have VS Code: `code .` to open the whole folder)

---

### 🪟 Windows

1. **Install Git for Windows** — [git-scm.com/download/win](https://git-scm.com/download/win) → run installer (defaults are fine). This gives you Git + Bash-style commands Claude Code can use.
2. **Install GitHub CLI** — [cli.github.com](https://cli.github.com) → run installer
3. **Open Windows Terminal or PowerShell** (Start menu → "Terminal"). **Use PowerShell, not Git Bash, for the next step** — Git Bash chokes on the installer.
4. **Install Claude Code with the native installer (in PowerShell):**

   ```powershell
   irm https://claude.ai/install.ps1 | iex
   ```

5. **Verify installs:**

   ```powershell
   git --version
   gh --version
   claude --version
   claude doctor
   ```

6. **Set your Git identity** (first time only):

   ```powershell
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```

7. **Log in to GitHub** (browser opens):

   ```powershell
   gh auth login
   ```

   Choose: GitHub.com → HTTPS → Yes → Login with browser. Then check:

   ```powershell
   gh auth status
   ```

8. **Clone your repo** (replace `your-name` — only works after you accepted the invitation):

   ```powershell
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

9. **Start Claude Code:**

   ```powershell
   claude
   ```

   Log in when prompted → ready. Open prompts:

   ```powershell
   type PROMPTS.md
   ```

   (or if you have VS Code: `code .`)

---

### 🐧 Linux / WSL (Ubuntu / Debian)

1. Open a **terminal**
2. **Install Git + GitHub CLI:**

   ```bash
   sudo apt update
   sudo apt install -y git gh
   ```

3. **Install Claude Code with the native installer:**

   ```bash
   curl -fsSL https://claude.ai/install.sh | bash
   ```

4. **Verify installs:**

   ```bash
   git --version
   gh --version
   claude --version
   claude doctor
   ```

5. **Set your Git identity** (first time only):

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```

6. **Log in to GitHub** (browser opens):

   ```bash
   gh auth login
   ```

   Choose: GitHub.com → HTTPS → Yes → Login with browser. Then check:

   ```bash
   gh auth status
   ```

7. **Clone your repo** (replace `your-name` — only works after accepting the invitation):

   ```bash
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

8. **Start Claude Code:**

   ```bash
   claude
   ```

   Log in when prompted → ready:

   ```bash
   cat PROMPTS.md
   ```

   (or `code .` for VS Code)

---

## ⚠️ Common setup issues — quick fixes

**`git clone` says "Repository not found"** — usually one of:
- You didn't accept the GitHub invitation yet → check your email or [github.com/notifications](https://github.com/notifications)
- You're logged into the wrong GitHub account → `gh auth status` to verify
- The repo slug was typed incorrectly → double-check the URL Kemal sent

**`claude` command not found** — installer ran but PATH isn't updated yet:
- Close + reopen your terminal
- Run `claude doctor` once your terminal is open again

**`gh auth login` won't open browser** — copy the URL it prints and paste into your browser manually.

**Anything else** — type `@Kemal acil` in the Meet chat. Kemal jumps to your screen-share and fixes it in under 2 minutes.

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
