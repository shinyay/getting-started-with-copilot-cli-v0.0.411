---
layout: step
title: "Setup & Installation"
step_number: 0
permalink: /setup/
---

# 🔧 Setup & Installation

Complete these steps before starting the workshop. Estimated time: **10–15 minutes**.

---

## System Requirements

| Requirement | Details |
|-------------|---------|
| **Operating System** | Linux, macOS, or Windows (PowerShell 6+ / WSL) |
| **Node.js** | Version 22 or later (for npm installation) |
| **Git** | Installed and configured |
| **GitHub Account** | With a valid Copilot subscription (Individual, Business, or Enterprise) |
| **Python** | 3.8+ (for Levels 1–6 sample apps) |
| **Node.js** | 18+ (for Level 7 TypeScript sample app) |

---

## Step 1: Install Copilot CLI

Choose the installation method for your platform:

### npm (All Platforms — Requires Node.js 22+)

```bash
npm install -g @github/copilot
```

### macOS / Linux (Homebrew)

```bash
brew install copilot-cli
```

### macOS / Linux (Install Script)

```bash
curl -fsSL https://gh.io/copilot-install | bash
```

### Windows (WinGet)

```powershell
winget install GitHub.Copilot
```

### Download from GitHub.com

Download executables directly from the [releases page](https://github.com/github/copilot-cli/releases/). Unpack and run the executable for your platform.

> [!NOTE]
> The `gh copilot` extension (via `gh extension install github/gh-copilot`) is a **different tool** from the standalone `copilot` CLI. For the full agent experience used in this workshop, use one of the methods above.

---

## Step 2: Verify Installation

```bash
copilot --version
```

You should see a version number like `0.0.411` or later.

---

## Step 3: Clone This Repository

```bash
git clone https://github.com/shinyay/getting-started-with-copilot-cli-v0.0.411.git
cd getting-started-with-copilot-cli-v0.0.411
```

---

## Step 4: Launch Copilot CLI

```bash
cd workshop/level-1/sample-app
copilot
```

When prompted to **trust the folder**, choose **"Yes, proceed"** (session-only trust).

---

## Step 5: Authenticate

If not already logged in, type `/login` inside Copilot CLI.

Alternatively, set a fine-grained PAT with the **"Copilot requests"** permission:

```bash
export GH_TOKEN=ghp_your_token_here
```

---

## Verification Checklist

Run these commands to confirm everything is ready:

```bash
# Check Copilot CLI
copilot --version

# Check Node.js
node --version

# Check Python (for Levels 1-6)
python3 --version

# Check Git
git --version
```

All commands should return valid version numbers.

---

## Troubleshooting

### "copilot: command not found"

- **npm install:** Ensure `$(npm bin -g)` is in your `PATH`
- **Homebrew:** Run `brew link copilot-cli`
- **Install script:** Check that `~/.local/bin` is in your `PATH`

### "Authentication failed"

- Run `/login` inside Copilot CLI
- Verify your GitHub subscription includes Copilot
- Check that your organization hasn't disabled Copilot CLI

### "Trust failed"

- You must trust the folder before Copilot can read files
- If you accidentally denied, exit (`Ctrl+C`) and relaunch `copilot`

### Python/Node.js version issues

- **Python:** Levels 1–6 need Python 3.8+. Use `pyenv` or your system package manager
- **Node.js:** Level 7 needs Node.js 18+. Use `nvm` or download from [nodejs.org](https://nodejs.org)

---

✅ **You're ready!** Continue to [Level 1: Observe →](../steps/1/)
