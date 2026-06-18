# 🚀 Build Your Idea in 1 Hour — AI Workshop Starter

> Bring an idea. Build it with Claude Code. Ship a working app tonight.

A starter from the **AI Build Workshop** by SafeScreens Initiative. Customize this empty shell into anything — habit tracker, family game, study tool, journal — with the help of Claude Code in your terminal.

---

> ## ⚠️ Heads-up before you start
>
> Tonight's workshop uses **Claude Code**, which requires a **Claude Pro, Max, Team, Enterprise, or Console account** (Pro is $20/month).
> **The free Claude.ai plan does not include Claude Code.**
> → [Check or upgrade your plan](https://claude.ai/settings/billing) before tonight.
>
> *If you can't upgrade right now, you can still attend — just use [claude.ai](https://claude.ai) web (Artifacts) as Plan B. The workflow is similar; you copy-paste HTML instead of editing files directly.*

---

## 📑 Contents

- [✅ Before tonight](#-before-tonight--6-things-10-min-total) — 6 quick things to do before the workshop starts
- [🛠 Setup tonight](#-setup-tonight--install-claude-code-15-20-min-kemal-walks-through-live) — install Claude Code (Mac / Windows / Linux)
- [⚠️ Common setup issues](#%EF%B8%8F-common-setup-issues--quick-fixes)
- [🎬 The workflow tonight](#-the-workflow-tonight)
- [🆘 Stuck during the build?](#-stuck-during-the-build)

**If you only read one section: → [Before tonight](#-before-tonight--6-things-10-min-total).**

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

Knock these out before the workshop starts so the live session can focus on building, not configuring.

1. **Create or confirm your GitHub account** — [github.com/signup](https://github.com/signup) (2 min if you don't have one)
2. **Add yourself to the workshop sign-up sheet** — name + GitHub username + one-sentence idea → **[Workshop sign-up sheet](https://docs.google.com/spreadsheets/d/1lVzVVg_3B4jm5zGTbv3aS50Frn4lhhhoCe8NXc-hxaY/edit)**
3. **Accept the GitHub repository invitation** Kemal sends to your email. He creates `github.com/profkemalaydin/buildschool-yourname` right after he sees your row on the sheet — usually a few minutes. *Your slug is your first name in lowercase: if you signed up as "Sara", your repo is `buildschool-sara`.*
4. **Confirm a Claude Pro account** (see the ⚠️ note at the top of this README)
5. **Bring your laptop charger + ~2 GB of free disk space** — an hour of build + streaming drains a battery fast; Claude Code, Git, and a Node install combined take ~1.5 GB
6. **Use Chrome or another modern browser** — for the GitHub login flow and Claude streaming UI

> 💛 **Don't worry if something fails during setup.** The goal isn't to finish alone — it's to get everyone into the repo and run Claude Code together. Kemal screen-shares every step and unblocks you live.

---

## 🛠 Setup tonight — Install Claude Code (15-20 min, Kemal walks through live)

Pick your operating system. Each path ends the same way: Claude Code running in your repo folder.

> Anthropic's recommended path for Claude Code is the **native installer** — much cleaner than npm. The commands below pipe a remote installer script into your shell — this is the **same one Anthropic publishes** in their official docs.

---

### 🍎 macOS

1. Open **Terminal** (Cmd+Space → "Terminal" → Enter)
2. **Check if you already have Git + GitHub CLI:**

   ```bash
   git --version
   gh --version
   ```

   Both already there? Skip to step 4. Missing either? Install via Homebrew:

   ```bash
   # Install Homebrew first if you don't have it:
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   # Then:
   brew install git gh
   ```

3. **Install Claude Code with the native installer:**

   ```bash
   curl -fsSL https://claude.ai/install.sh | bash
   ```

4. **Verify everything:**

   ```bash
   git --version
   gh --version
   claude --version
   claude doctor
   ```

   `claude doctor` runs a self-check — if anything's off it tells you exactly what.

5. **Set your Git identity** (first time only):

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```

6. **Log in to GitHub** (browser opens):

   ```bash
   gh auth login
   ```

   Choose: GitHub.com → HTTPS → Yes → Login with browser. Then verify:

   ```bash
   gh auth status
   ```

   should show ✓ Logged in.

7. **Clone your repo** (replace `your-name` with your slug from "Before tonight" step 3 — only works *after* you've accepted the invitation):

   ```bash
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

8. **Start Claude Code:**

   ```bash
   claude
   ```

   Log in with your Claude account when prompted. You're ready.

9. **Open the prompts in your browser** (easier to read than in terminal):
   → **[PROMPTS.md](https://github.com/profkemalaydin/workshop-starter/blob/main/PROMPTS.md)** — paste each step into Claude Code, in order.

---

### 🪟 Windows

**Quickest install (Windows 11 with winget):**

```powershell
winget install Git.Git GitHub.cli
```

That's both Git and GitHub CLI in one go. If you're on older Windows or `winget` isn't available, install the two manually:

1. **Git for Windows** → [git-scm.com/download/win](https://git-scm.com/download/win) → run installer (defaults are fine). This gives you Git + Bash-style commands.
2. **GitHub CLI** → [cli.github.com](https://cli.github.com) → run installer

Then:

3. **Open Windows Terminal or PowerShell** (Start menu → "Terminal"). **Use PowerShell, not Git Bash, for the next step** — the installer chokes on Git Bash.
4. **Install Claude Code with the native installer:**

   ```powershell
   irm https://claude.ai/install.ps1 | iex
   ```

5. **Verify everything:**

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

   Choose: GitHub.com → HTTPS → Yes → Login with browser. Then verify:

   ```powershell
   gh auth status
   ```

8. **Clone your repo** (replace `your-name` with your slug — only works after you accepted the invitation):

   ```powershell
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

9. **Start Claude Code:**

   ```powershell
   claude
   ```

   Log in when prompted. You're ready.

10. **Open the prompts in your browser** (easier to read than in terminal):
    → **[PROMPTS.md](https://github.com/profkemalaydin/workshop-starter/blob/main/PROMPTS.md)** — paste each step into Claude Code, in order.

---

### 🐧 Linux (Ubuntu / Debian)

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

4. **Verify everything:**

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

   Choose: GitHub.com → HTTPS → Yes → Login with browser. Then:

   ```bash
   gh auth status
   ```

7. **Clone your repo** (replace `your-name` with your slug — only after accepting the invitation):

   ```bash
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

8. **Start Claude Code:**

   ```bash
   claude
   ```

   Log in when prompted. You're ready.

9. **Open the prompts in your browser** (easier to read than in terminal):
   → **[PROMPTS.md](https://github.com/profkemalaydin/workshop-starter/blob/main/PROMPTS.md)** — paste each step into Claude Code, in order.

---

### 🪟🐧 WSL (Windows Subsystem for Linux)

If you have WSL set up, **run the Linux (Ubuntu) steps above inside your WSL terminal** — not the Windows steps. WSL = Linux on Windows, so the Linux installer is the right one.

If you don't already have WSL working and want to set it up tonight: just use the Windows native path above instead. WSL setup itself takes 15+ minutes — too much for tonight.

---

## ⚠️ Common setup issues — quick fixes

**`git clone` says "Repository not found"** — usually one of:
- You haven't accepted the GitHub invitation yet → check your email or [github.com/notifications](https://github.com/notifications)
- You're logged into the wrong GitHub account → run `gh auth status` to verify
- The repo slug was typed incorrectly → it's your first name in lowercase (e.g. `buildschool-sara`)

**`claude` command not found** — installer ran but your PATH hasn't picked it up yet:
- Close + reopen your terminal
- If it still doesn't work, run `claude doctor` once your new terminal is open

**`gh auth login` won't open browser** — copy the URL it prints, paste into your browser manually.

**Plan B — install fails entirely** — switch to [claude.ai](https://claude.ai) web (Artifacts). You can build the same app in a web chat; Kemal helps you push the final HTML to your repo at the end. You won't fall behind.

**Anything else** — type `@Kemal acil` in the Meet chat. Kemal jumps to your screen-share and fixes it in under 2 minutes.

---

## 🎬 The workflow tonight

1. **You and Kemal are both collaborators** on your repo. You push changes; Kemal handles the Cloudflare deploy.
2. **Claude Code runs in your repo's folder** — it can directly read and edit your files as you talk to it.
3. **Open [PROMPTS.md](./PROMPTS.md)** — paste **one** big prompt into Claude Code. After that, just answer Claude's questions as they come.
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
2. **Workshop AI Coach** — a second Claude chat that knows the workshop structure and unsticks you in 2 minutes → **[Open COACH.md and follow the instructions](./COACH.md)**
3. **Type `@Kemal acil` in the Meet chat** — Kemal jumps into your screen-share and helps personally

---

## 📦 What's in this starter

| File | Purpose |
|---|---|
| `index.html` | Working "hello, your app" page with Tailwind CSS pre-wired, localStorage helpers ready |
| `PROMPTS.md` | The 6-step Claude Code conversation guide |
| `COACH.md` | The Workshop AI Coach prompt (your second Claude chat) |
| `LICENSE` | MIT — yours to keep |

The starter is **deliberately minimal** so Claude has room to make it yours.

---

## 📝 License

MIT — fork it, remix it, build a business with it. Yours to keep.
