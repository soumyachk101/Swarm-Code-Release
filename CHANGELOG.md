# Changelog

All notable releases, feature additions, bug fixes, and refinements for SwarmAI.

---

## [1.1.2] - 2026-09-17

A release introducing in-picker model search and flexible provider switching in running chats. Apple silicon, macOS 14 or later.

### 🚀 New features
- **In-picker model search:** Instant search and filter across all providers and Hydra pairs directly in the model picker.
- **Provider switching in running chats:** Seamlessly switch models and providers (Codex, Claude, etc.) within ongoing conversation threads while keeping full conversational context and history.

### 🎨 Refinements
- Clearer provider branding and optical icon sizing in the model picker list.

---

## [1.1.1] - 2026-09-17

A polish release ensuring rock-solid chat stability, timeline animations, and license compliance. Apple silicon, macOS 14 or later.

### 🚀 New features
- **In-app Licenses:** `Settings › About › Licenses` shows the app's license, third-party notices, and trademark policy shipped inside the app bundle.

### 🐛 Bug fixes
- Fixed timeline positioning so chat never opens into empty space after turn completions or rapid thread switches.
- Fixed the working line presentation so it flows as a natural timeline row rather than sliding up awkwardly.
- Adjusted window traffic-light buttons alignment when the sidebar is collapsed.

### 🎨 Refinements
- Streamlined About dialog layout without redundant version headers.

---

## [1.1.0] - 2026-09-15

SwarmAI updates itself from here on: Settings › About checks for new versions and installs them with Update & restart. Apple silicon, macOS 14 or later.

### 🚀 New features
- **In-app auto-updates:** About settings checks for updates, displays rich release cards, and installs updates in-place.
- **GitHub Copilot CLI provider:** Copilot CLI integration with models, reasoning efforts, and monthly quota tracking.
- **Antigravity integration:** Direct support for Antigravity AI coding agent and plan limit monitoring.
- **Native DeepSeek & Meta:** Direct API integration with Keychain-secured credentials and real-time usage/credit tracking.
- **26 Tinted-Glass Themes:** System glass, Catppuccin, Claude, Codex, Tokyo Night, Dracula, and window transparency control.
- **Follow-up Queue:** Queue subsequent prompts while an agent is executing; steer running turns or dispatch queued prompts immediately.
- **Interactive Delegation Tabs:** Agent questions and approval requests appear on dedicated tabs above the chat box.
- **Minimap Rail & Previews:** Thread minimap, large photo/file previews, and completion chimes.

### 🐛 Bug fixes
- Native provider turns now properly handle unlimited tool rounds without stalling at 12 steps.
- Changes popover reliably opens on modified files even in complex multi-file edits.
- Fixed DeepSeek tool-call chains through context compaction and interruptions.
- Fixed blank link renders and dark mode scroll veils.

### 🎨 Refinements
- Virtualized row rendering for ultra-smooth scrolling on conversations with hundreds of messages.
- Clean collapsible tool run cards with one-click expansion.
- Native iMessage-style speech bubbles.

---

## [1.0.0] - 2026-09-15

Initial public release of SwarmAI: The native Mac client for your coding agents.

### 🚀 Highlights
- Native multi-agent support: Codex, Claude, Cursor, OpenCode, Grok, DeepSeek, Meta, Devin, Antigravity.
- Git worktree isolation per thread for parallel non-destructive branch execution.
- Command palette (`Cmd+K`) for jumping across threads, projects, and actions.
- Built-in live diff viewer and code review popovers.
- Reasoning effort sliders and provider selectors integrated in composer.
- Built-in terminal under every thread.
