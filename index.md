---
layout: workshop
---

## 🎓 Workshop Overview

A progressive **8-level curriculum** for mastering GitHub Copilot CLI, from first launch to advanced automation and delegation. **96 exercises** across **9–13 hours**, designed for hands-on learning.

## How to Use This Workshop

1. **[Complete the Setup](setup/)** — Install Copilot CLI, clone the repo, verify your environment
2. **Click a level in the sidebar** (or the table below) to read the exercises
3. **Follow along in your terminal** — Each exercise tells you exactly what to type
4. **Use the 📋 Cheatsheet** links for quick reference while working
5. **Track your progress** with the sidebar progress bar

> [!TIP]
> Each level has its own **sample application** in the `workshop/level-N/sample-app/` directory. Navigate there in your terminal while reading the exercises on this site.

---

## Skill Progression

```
Level 1   Level 2    Level 3    Level 4    Level 5    Level 6     Level 7      Level 8
Observe → Understand → Plan → Create → Execute → Workflow → Customize → Advanced
  🟢        🟢         🟢      🟡       🟡        🟠         🟢          🔴
 read     ask & learn  think   write    run cmds   full cycle  configure   automate
 only     code Q&A    before   first    tests &    plan→test   instruct.   delegate
                      coding   edits    linters    →review     MCP/ctx     agent/CI
```

| Risk | Levels | What happens |
|------|--------|-------------|
| 🟢 Zero | 1, 2, 3 | Nothing is modified — read-only exploration, questions, planning |
| 🟡 Low | 4, 5 | First writes and command execution — all reversible with `git checkout` |
| 🟠 Medium | 6 | Full plan → execute → review workflows across multiple files |
| 🔴 High awareness | 8 | Autonomous delegation, permissions, and CI/CD integration |

---

## Curriculum

| Level | Title | Exercises | Sample App | Time |
|-------|-------|:---------:|------------|------|
| [**Setup**](setup/) | Setup & Installation | — | — | 10–15 min |
| [**1**](steps/1/) | Observe — Read-Only Exploration | 12 | Python Task Manager CLI | 45–60 min |
| [**2**](steps/2/) | Understand — Ask Questions | 12 | Python Bookmark Manager API | 60–80 min |
| [**3**](steps/3/) | Plan — Think Before Acting | 12 | Python Quick Notes CLI (bugs) | 60–80 min |
| [**4**](steps/4/) | Create — Make Your First Changes | 12 | Python Quick Notes CLI (writable) | 60–90 min |
| [**5**](steps/5/) | Execute — Run Commands | 12 | Python Math Utilities (pytest) | 75–100 min |
| [**6**](steps/6/) | Workflow — Full Cycle | 12 | Python URL Shortener CLI | 90–120 min |
| [**7**](steps/7/) | Customize — Make It Yours | 12 | TypeScript Event API (Express) | 75–100 min |
| [**8**](steps/8/) | Advanced — Delegation | 12 | Multi-service DevOps Toolkit | 90–120 min |

**Total: 96 exercises across 8 levels — estimated 9–13 hours**

---

## What is Copilot CLI?

**GitHub Copilot CLI** is a terminal-based **AI agent** that lets you have conversations while reading your codebase, editing files, and executing commands — all with approval steps in between. Beyond simple Q&A, Copilot CLI enables a complete **plan → execute → verify → review** workflow entirely within the terminal.

### Key Characteristics

- 🖥️ **Cross-platform** — Works across Linux, macOS, and Windows (PowerShell / WSL)
- 🎯 **Interactive UI** — Rich terminal interface with plan mode and tool approval
- 📝 **Editor-agnostic** — Edit in the terminal, confirm in any editor
- 🔗 **GitHub integration** — Native access to issues, PRs, and repos
- 🔌 **Extensible** — MCP servers, custom agents, skills, and plugins
- 🛡️ **Safe by design** — Every tool call requires your approval (Allow / Deny / Allow-for-session)

---

## Quick Start

```bash
# 1. Install
npm install -g @github/copilot    # or: brew install copilot-cli

# 2. Clone this workshop
git clone https://github.com/shinyay/getting-started-with-copilot-cli-v0.0.411.git
cd getting-started-with-copilot-cli-v0.0.411

# 3. Navigate to Level 1 sample app
cd workshop/level-1/sample-app

# 4. Launch Copilot CLI
copilot

# 5. Trust the folder → Authenticate → Try your first prompt:
#    "What does this project contain?"
```

For detailed setup instructions, see the **[Setup & Installation](setup/)** page.

---

## Key Commands Cheat Sheet

| Syntax | Purpose | Token Cost |
|--------|---------|------------|
| `!command` | Run shell command directly (no AI) | **Free** |
| `@ filename` | Inject file contents into context | Adds input tokens |
| `text + Enter` | Send prompt to AI model | Input + output tokens |
| `/help` | Show all commands and shortcuts | **Free** |
| `/plan` | Enter Plan mode (think before acting) | **Free** |
| `/diff` | Show changes since session start | **Free** |
| `/model` | View or switch AI model | **Free** |
| `/compact` | Compress conversation to free tokens | **Free** |
| `/context` | Visualize context window usage | **Free** |

---

## Requirements

- **GitHub Copilot subscription** (Individual, Business, or Enterprise)
- **Node.js 22+** (for npm installation)
- **Python 3.8+** (for Levels 1–6)
- **Git** installed and configured

👉 **[Start the Setup →](setup/)**
