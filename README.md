<div align="center">

<img src="assets/icon.png" alt="SwarmAI" width="140" height="140">

# SwarmAI

### Your coding agents. Native on the Mac.

<p>
  <b>Codex</b> · <b>Claude</b> · <b>Cursor</b> · <b>OpenCode</b> · <b>Grok</b> · <b>Antigravity</b> · <b>DeepSeek</b> · <b>Meta</b>
</p>

<p>
  <a href="https://github.com/soumyachk101/SwarmAI-Release/releases/latest"><img src="https://img.shields.io/badge/Download-Free-blue?logo=apple" alt="Download"></a>
  <a href="https://github.com/soumyachk101/SwarmAI-Release"><img src="https://img.shields.io/badge/SwiftUI-Liquid_Glass-orange?logo=swift" alt="SwiftUI"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-success" alt="MIT"></a>
  <a href="https://github.com/soumyachk101/SwarmAI-Release"><img src="https://img.shields.io/badge/macOS-26%2B-999?logo=apple" alt="macOS 26+"></a>
</p>

<p align="center">
  <i>One Liquid Glass window. Your subscriptions. No middleman. No cloud. No compromise.</i>
</p>

---

</div>

## What is SwarmAI?

**SwarmAI** is a native macOS desktop app that unifies all your AI coding agents into one beautiful, powerful interface.

Built entirely in **Swift and SwiftUI** with Apple's **Liquid Glass** design language, SwarmAI drives the coding agents you already have installed — on your own subscriptions, with zero markup, zero cloud, zero compromise.

> **Built by [Soumya Chakraborty](https://github.com/soumyachk101). For Mac, only Mac, forever.**

---

## Screenshots

|  |  |
|:---:|:---:|
| <img src="assets/screenshots/hero.webp" alt="Main window streaming reply" width="100%"><br>**Streaming replies** with live diff | <img src="assets/screenshots/palette.webp" alt="Command palette" width="100%"><br>**Command palette** — ⌘K for everything |
| <img src="assets/screenshots/switcher.webp" alt="Model switcher" width="100%"><br>**Model picker** — any model, any provider | <img src="assets/screenshots/sidebar.webp" alt="Project sidebar" width="100%"><br>**Sidebar** — projects, threads, search |
| <img src="assets/screenshots/plans.webp" alt="Plan mode" width="100%"><br>**Plan mode** — approvals before changes | <img src="assets/screenshots/diff.webp" alt="Diff viewer" width="100%"><br>**Diff** — every turn, a checkpoint |
| <img src="assets/screenshots/themes.webp" alt="Theme picker" width="100%"><br>**26 themes** — System, Catppuccin, Dracula… | <img src="assets/screenshots/question.webp" alt="Question mode" width="100%"><br>**Questions** — inline approvals |

---

## Features

### 8 Agents, One Window

Drive **Codex**, **Claude**, **Cursor**, **OpenCode**, **Grok**, **Antigravity**, **DeepSeek**, and **Meta** from one interface. Sign in once in your terminal — SwarmAI picks it up automatically. No keys to paste, no middleman.

### Hydra: One Chat, Many Heads

Turn a big job into a team. The lead writes the briefs, sends heads out in parallel — each in its own git worktree — and their work lands back in your checkout. Pair a strong lead with quick heads, fuse effort across the team.

### Streaming & Live Diffs

Watch streaming replies arrive in real time — reasoning, reads, edits, to-dos, builds. Every turn gets a checkpoint with a diff. Read the change, revert the turn, or rewind the whole thread.

### Follow-up Queue

Type while it works. Follow-ups line up above the chat box and go out one after another when the turn ends. Never lose a thought mid-turn.

### Inline Approvals

The agent proposes a plan, asks before it pushes, and you approve right in the timeline. Plan mode, model selection, and four permission modes per thread.

### Model Picker with Search

Find any model from any provider instantly. Switch models and providers mid-chat while preserving conversation history and context.

### Terminal Per Thread

Every thread gets its own real PTY terminal. Run commands, check builds, inspect state — right where you need it.

### Git Built In

Worktrees, commits, pushes, pull requests. Every turn creates a hidden git checkpoint. New threads start in their own worktree so several agents can work on one project simultaneously without clashing.

### 26 Tinted-Glass Themes

From System to Catppuccin, Dracula, Tokyo Night, Nord, Gruvbox, and more. Real glass, real code, real you.

### Zero Compromise

No remote access. No mobile apps. No cloud sync. No telemetry. No accounts. No web client. Left out on purpose.

---

## Architecture

```
┌──────────────────────────────────────────────────────────┐
│                   SwarmAI (SwiftUI)                       │
│  ┌────────────────────────────────────────────────────┐  │
│  │              Liquid Glass Window                    │  │
│  │  ┌──────────┐ ┌──────────┐ ┌────────────────────┐  │  │
│  │  │ Sidebar  │ │  Chat    │ │  Detail Panel      │  │  │
│  │  │ Projects │ │ Thread   │ │  Diff / Git        │  │  │
│  │  │ & Search │ │ Stream   │ │  Terminal          │  │  │
│  │  └──────────┘ └──────────┘ └────────────────────┘  │  │
│  └────────────────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────────────────┐  │
│  │  Theme Engine  │  Binary Field  │  Hydra Engine    │  │  │
│  └────────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────────┘
         │                        │
         ▼                        ▼
  ┌──────────────┐      ┌──────────────┐
  │ Your Mac     │      │ Your Agents  │
  │ Swift/SwiftUI│      │ Codex, Claude│
  │ No Electron  │      │ Cursor, etc  │
  │ 1 dependency │      │ Your subs    │
  └──────────────┘      └──────────────┘
```

---

## Tech Stack

| | |
|---|---|
| **Language** | Swift 6 |
| **UI Framework** | SwiftUI + Liquid Glass |
| **Terminal** | SwiftTerm |
| **Git** | libgit2 |
| **Architecture** | MV + async/await |
| **License** | MIT |

**One dependency. Zero telemetry. 100% native.**

---

## Download

### Requirements

- Apple Silicon Mac (M1 / M2 / M3 / M4 or newer)
- macOS 26 or later
- At least one provider installed (`codex login`, `claude auth login`, etc.)
- Git, plus `gh` or `glab` for pull requests

### Install

1. Download `SwarmAI-1.1.2.dmg` from the [Releases](https://github.com/soumyachk101/SwarmAI-Release/releases) page.
2. Double-click the `.dmg` file to open it.
3. Drag **SwarmAI.app** into your `/Applications` folder.
4. Launch from Applications or Spotlight.

> If Gatekeeper blocks it on first launch: right-click → **Open**, or run:
> ```bash
> xattr -cr /Applications/SwarmAI.app
> ```

---

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for the full history.

### v1.1.2
- Model search and provider switching in running chats
- Eliminated all remaining compiler warnings
- Performance improvements and bug fixes

### v1.0.0
- 8 agent providers in one window
- Hydra: parallel agents in separate worktrees
- 26 tinted-glass themes
- Streaming replies with live diff per turn
- Inline approvals and follow-up queuing
- Reasoning slider (Fast to Maximum)
- Built-in terminal per thread
- Zero telemetry, MIT licensed

---

## FAQ

**Is it really free?**
Yes. SwarmAI is free and MIT licensed. You pay your agent providers as you already do; SwarmAI never sits in between.

**Is it open source?**
Yes. The full Swift/SwiftUI source is on [GitHub](https://github.com/soumyachk101/SwarmAI-Release). The code is MIT; the SwarmAI name and icon are trademarks.

**Do I need an API key?**
Not for Codex, Claude, Cursor, OpenCode, Grok or Antigravity — sign in once in your terminal. DeepSeek and Meta need a key stored in your Keychain.

**Which Mac do I need?**
Apple silicon, macOS 26+. Signed and notarized. No Gatekeeper workaround needed.

**Does it send anything anywhere?**
Only what your agents send to their own providers. No telemetry, no analytics, no account, no cloud sync.

**Where do I get help?**
Open an [issue on GitHub](https://github.com/soumyachk101/SwarmAI-Release/issues) or email hi@getswarmai.app.

---

## License

Copyright (c) 2026 Soumya Chakraborty. All rights reserved.

SwarmAI is released under the [MIT License](LICENSE). The SwarmAI name and icon are trademarks of Soumya Chakraborty — see [TRADEMARK.md](TRADEMARK.md).

---

<div align="center">

**Made with love by [Soumya Chakraborty](https://github.com/soumyachk101)**

Built in Swift. For Mac, only Mac, forever.

[⬆ Back to top](#-swarmai)

</div>
