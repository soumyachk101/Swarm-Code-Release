# Third-Party Notices

> **SwarmAI** is built on the shoulders of giants. This document acknowledges the open-source software that makes SwarmAI possible.

---

## Acknowledgement

SwarmAI is released under the **MIT License** and embraces the open-source ecosystem. The app combines native Swift code with carefully selected third-party libraries, each under their own permissive license. We are grateful to the maintainers and contributors of every project listed here.

---

## Core Dependencies

### SwiftTerm

| | |
|---|---|
| **Repository** | [migueldeicaza/SwiftTerm](https://github.com/migueldeicaza/SwiftTerm) |
| **License** | MIT |
| **Copyright** | (c) 2016–2026 Miguel de Icaza |
| **Purpose** | Cross-platform terminal emulator written in Swift. SwarmAI embeds a real PTY terminal inside every thread using SwiftTerm as the rendering layer. |
| **License Text** | [github.com/migueldeicaza/SwiftTerm/blob/master/LICENSE](https://github.com/migueldeicaza/SwiftTerm/blob/master/LICENSE) |

> _"SwiftTerm is the prettiest terminal emulator I have written."_ — Miguel de Icaza

---

## Swift Package Ecosystem

SwarmAI is built with Swift Package Manager. The full dependency manifest is available in `Package.swift` and `Package.resolved`.

### Direct Dependencies

| Package | Maintainer | License | Purpose |
|---------|-----------|---------|---------|
| **SwiftTerm** | Miguel de Icaza | MIT | Terminal emulation inside threads |
| **swift-git** | knownsec | MIT | High-level Git operations (worktrees, commits, status) |
| **swift-argument-parser** | Apple | Apache 2.0 | CLI command parsing for embedded agents |

### Transitive Dependencies

| Package | License | Notes |
|---------|---------|-------|
| SwiftNIO | Apache 2.0 | Async networking (via SwiftTerm) |
| Swift Collections | Apache 2.0 | Optimised data structures |
| swift-system | Apache 2.0 | Low-level system bindings |

---

## System Frameworks

SwarmAI also uses Apple's first-party frameworks, which are covered under the macOS SDK license:

| Framework | Purpose |
|-----------|---------|
| **SwiftUI** | Declarative UI and Liquid Glass rendering |
| **AppKit** | Native macOS window and menu integration |
| **Combine** | Reactive data flow |
| **Foundation** | File system, networking, JSON |
| **UniformTypeIdentifiers** | Modern file type handling |
| **CryptoKit** | Secure Keychain operations |
| **libgit2** | Git plumbing (via Swift bindings) |

---

## Bundled Fonts

| Font | License | Author |
|------|---------|--------|
| SF Pro Display | System (Apple) | Apple Inc. |
| SF Mono | System (Apple) | Apple Inc. |
| Inter | Open Font License | Rasmus Andersson |

System fonts are used wherever possible. Inter is bundled only when needed for the terminal UI.

---

## Design Inspiration

SwarmAI's **Liquid Glass** aesthetic and several interaction patterns draw inspiration from:

- **Apple's Human Interface Guidelines** — Liquid Glass design system
- **Roo Code** — Stream-driven chat UX patterns
- **Claude Code CLI** — Inline approval workflow
- **Codex CLI** — Provider abstraction and session management

---

## AI Provider Acknowledgements

SwarmAI does **not** ship or bundle any AI model. It acts as a unified interface to providers you authenticate with locally:

| Provider | Attribution |
|----------|-------------|
| OpenAI / Codex | OpenAI, Inc. |
| Anthropic / Claude | Anthropic PBC |
| Cursor | Anysphere, Inc. |
| OpenCode | OpenCode contributors |
| xAI / Grok | xAI Corp. |
| Google DeepMind / Antigravity | Google LLC |
| DeepSeek | DeepSeek AI |
| Meta Llama | Meta Platforms, Inc. |

All trademarks are property of their respective owners. SwarmAI is not affiliated with, endorsed by, or sponsored by any of the above providers.

---

## Icons & Assets

- **App Icon:** Original design by Soumya Chakraborty (CC BY 4.0 for the bee motif, trademarked as SwarmAI brand).
- **SF Symbols:** Used under Apple's developer license.

---

## Contribution Notice

If you believe SwarmAI includes software that should be acknowledged here and is not, please open an issue or email **hi@getswarmai.app**. We will add it promptly and correctly attribute the original authors.

---

## Full License Texts

For the complete text of every license referenced above:

- **MIT:** [opensource.org/licenses/MIT](https://opensource.org/licenses/MIT)
- **Apache 2.0:** [apache.org/licenses/LICENSE-2.0](https://www.apache.org/licenses/LICENSE-2.0)
- **OFL 1.1:** [scripts.sil.org/OFL](https://scripts.sil.org/OFL)

---

<div align="center">

_This document was last updated: 2026._

**Built with respect for the open-source community.**

</div>
