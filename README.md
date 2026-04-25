🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

<div align="center">

# 🎯 Soc Ops

### Social Bingo for in-person mixers

*Find people who match the questions. Get 5 in a row. Win the room.*

[![Play Game](https://img.shields.io/badge/🎮%20Play%20Now-Live%20Demo-4f46e5?style=for-the-badge)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)
[![Lab Guide](https://img.shields.io/badge/📚%20Lab%20Guide-Workshop-0ea5e9?style=for-the-badge)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)

[![.NET](https://img.shields.io/badge/.NET-10.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![Blazor](https://img.shields.io/badge/Blazor-WebAssembly-7C3AED?logo=blazor)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![Deploy](https://img.shields.io/badge/Deploy-GitHub%20Pages-22c55e?logo=github)](https://pages.github.com/)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

</div>

---

## 🎲 What is Soc Ops?

**Soc Ops** is a mobile-friendly Social Bingo web app designed for networking events, team mixers, and icebreakers. Players roam the room, find real people who match each square ("bikes to work", "has a hidden talent", "speaks 2+ languages"), and race to get **5 in a row**.

But it's also more than a game — it's the **starting point for a GitHub Copilot hands-on workshop** where you'll use AI agent mode to redesign, extend, and ship new features in under an hour.

```
┌─────────┬─────────┬─────────┬─────────┬─────────┐
│  bikes  │  lived  │  has a  │  prefers│  plays  │
│ to work │ abroad  │   pet   │   tea   │ guitar  │
├─────────┼─────────┼─────────┼─────────┼─────────┤
│ speaks  │  ran a  │  born   │   met   │   can   │
│ 2 langs │marathon │ diff st.│celebrity│ juggle  │
├─────────┼─────────╔═════════╗─────────┼─────────┤
│  been   │  loves  ║  FREE   ║  has a  │traveled │
│ skydive │cooking  ║  SPACE  ║ garden  │  Asia   │
├─────────┼─────────╚═════════╝─────────┼─────────┤
│  left-  │  has a  │  plays  │  does   │ hidden  │
│ handed  │  twin   │ videogm │  yoga   │ talent  │
├─────────┼─────────┼─────────┼─────────┼─────────┤
│  loves  │ been on │ collects│  read a │  knows  │
│ spicy   │   TV    │ unique  │  book   │   ASL   │
└─────────┴─────────┴─────────┴─────────┴─────────┘
```

---

## 🚀 Quick Start

**Prerequisites:** [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher

```bash
# Clone your fork (replace with your repository URL)
git clone https://github.com/your-username/your-fork.git
cd your-fork/SocOps
dotnet run
```

Then open **http://localhost:5000** in your browser. 🎉

> **Prefer the cloud?** Open in GitHub Codespaces — everything is pre-configured.  
> Click **Code → Codespaces → Create codespace on main** and you're ready in minutes.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Framework | [Blazor WebAssembly](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor) |
| Runtime | .NET 10 |
| Styling | Custom CSS utilities (app.css) |
| Hosting | GitHub Pages (auto-deploy on push to `main`) |

---

## 🤖 Workshop: Build with GitHub Copilot Agent Mode

This repo is the foundation for a **~1 hour hands-on lab** where you'll use VS Code's Agent Mode with GitHub Copilot to transform the app. No previous Copilot experience required.

### What you'll learn

| # | Skill | What you'll do |
|---|-------|----------------|
| 1 | **Context Engineering** | Teach the AI your codebase with `.github/instructions` |
| 2 | **Agentic Primitives** | Run background agents, cloud agents & custom workflows |
| 3 | **Design-First Development** | Let AI iterate on UI while you guide the creative vision |
| 4 | **Test-Driven Development** | Use TDD agents to build new features reliably |

### Lab guide

| Part | Title | Time |
|------|-------|------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview & Checklist | — |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup & Context Engineering | 15 min |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-First Frontend | 15 min |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master | 10 min |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-Agent Development | 20 min |

> 📝 Lab guides are also available offline in the [`workshop/`](workshop/) folder.

---

## 🏗️ Build & Deploy

```bash
# Run locally
cd SocOps && dotnet run

# Build for production
cd SocOps && dotnet build
```

Push to `main` → GitHub Actions builds and deploys automatically to GitHub Pages.
