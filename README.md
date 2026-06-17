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

## 🛠 Tonight's setup (15 min walkthrough, Kemal helps live)

Pick **one** path. Codespaces is easier if you've never used a terminal.

### 🌐 Path A — GitHub Codespaces (recommended, no local install)

1. **Go to your repo on GitHub** (Kemal sent you the link)
2. Click the green **`<> Code`** button → tab **`Codespaces`** → **`Create codespace on main`**
3. Wait 1-2 minutes — a full coding environment opens in your browser
4. In the terminal at the bottom, paste:

   ```bash
   npm install -g @anthropic-ai/claude-code
   ```

5. Then start Claude Code:

   ```bash
   claude
   ```

6. **Log in when prompted** with your Claude account
7. You're ready — jump to [PROMPTS.md](./PROMPTS.md)

### 💻 Path B — Local Claude Code (if you already use a terminal)

1. **Install Node.js** from [nodejs.org](https://nodejs.org) (LTS version)
2. **Install Claude Code:**

   ```bash
   npm install -g @anthropic-ai/claude-code
   ```

3. **Install GitHub CLI** from [cli.github.com](https://cli.github.com)
4. **Authenticate GitHub:**

   ```bash
   gh auth login
   ```

5. **Clone your repo** (replace `your-name` with what Kemal gave you):

   ```bash
   git clone https://github.com/profkemalaydin/buildschool-your-name.git
   cd buildschool-your-name
   ```

6. **Start Claude Code:**

   ```bash
   claude
   ```

7. Log in when prompted — you're ready. Jump to [PROMPTS.md](./PROMPTS.md)

---

## 🆕 No GitHub account yet?

It takes 2 minutes:

1. Go to **[github.com/signup](https://github.com/signup)**
2. Use any email (gmail works fine)
3. Pick a username — choose something you like, it becomes part of your URL
4. Verify your email
5. **Tell Kemal your username in the Meet chat** — he'll create your repo and add you as a collaborator (so you can push changes; Kemal will deploy)

---

## 🎬 The workflow tonight

1. You and Kemal are **both collaborators** on this repo. You push changes; Kemal handles deploy.
2. Claude Code is running in your repo's folder — it can **directly read and edit your files** as you talk to it.
3. Open [PROMPTS.md](./PROMPTS.md) — type each prompt into Claude Code, in order.
4. By Step 4 you'll have a working app. By Step 6 it's polished.
5. When you're happy: tell Claude Code *"Commit and push my changes"* — it does it.
6. **Kemal sees your push and deploys** to `https://buildschool-yourname.pages.dev` within a few hours.

---

## ✏️ When Claude Code is done — push your work

In Claude Code, just type:

```
Commit my changes with message "my v1" and push to main.
```

Claude Code handles the git commit + push for you.

You can also do it manually if you prefer:

```bash
git add .
git commit -m "my v1"
git push
```

---

## 🔁 After the workshop — build another idea

Click the green **`Use this template`** button at the top of [workshop-starter](https://github.com/profkemalaydin/workshop-starter). That creates a brand-new repo on your account with this same starter. You can keep building independently — no need for Kemal.

---

## 🆘 Stuck during the build?

You have **3 layers of help**:

1. **The prompts themselves** — they're written to anticipate where you might get stuck
2. **Workshop AI Coach** — open a *second* Claude chat in the browser, paste the Coach prompt Kemal shared. That second Claude knows the workshop structure and helps in 2 minutes
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
