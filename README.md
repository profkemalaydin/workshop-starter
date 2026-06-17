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

## 🛠 Setup — Install Claude Code on your machine (15-20 min)

Pick your operating system. Each path ends the same way: Claude Code running in your repo folder.

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

6. **Clone your repo** (Kemal will send you the URL — replace `your-name`):

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

7. **Clone your repo** (replace `your-name` with what Kemal gave you):

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

6. **Clone your repo** (replace `your-name`):

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

## 🆕 No GitHub account yet?

It takes 2 minutes:

1. Go to **[github.com/signup](https://github.com/signup)**
2. Use any email (gmail works fine)
3. Pick a username — choose something you like, it becomes part of your URL
4. Verify your email
5. **Tell Kemal your username in the Meet chat** — he'll create your repo and add you as a collaborator so you can push changes

---

## 🎬 The workflow tonight

1. **You and Kemal are both collaborators** on this repo. You push changes; Kemal handles the Cloudflare deploy.
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
2. **Workshop AI Coach** — open a *second* Claude chat in your browser and paste the Coach prompt Kemal shared. That second Claude knows the workshop structure and unsticks you in 2 minutes
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
