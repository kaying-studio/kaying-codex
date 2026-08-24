# KayingCodex

**English** | **[简体中文](README.zh-CN.md)** | **[日本語](README.ja.md)**

---

**An intelligent agent workbench built for game development — so AI actually ships the game, not just code that "looks like it compiles."**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> Desktop version: **1.5.0** · Default work mode: **Game Development**

---

## What Is This

KayingCodex is a desktop application for game creators. It combines a powerful AI agent with a "quality assurance framework": when you say "build me a side-scrolling platformer," it won't just tweak a few files and declare "done." Instead, it follows the complete pipeline of **Design → Scene → Gameplay → Integration → Testing**, step by step, to actually build the thing — and build it right.

Ordinary AI coding tools treat projects as text repositories, but a game is a graph of interwoven **scenes, assets, bindings, and gameplay logic**. The key differences of KayingCodex:

- **Compiles ≠ Playable**: It checks whether assets are truly bound and whether the player can actually see something on screen — not just run a type check.
- **Declared ≠ In Effect**: Referencing a texture doesn't mean that texture was actually published into the game. The framework demands "evidence" before it accepts anything.
- **Long Tasks Don't Lose the Thread**: A game spans multiple stages. KayingCodex persists task progress at every step, so closing and reopening picks up right where you left off.
- **No Passing on Self-Reported Success**: When the AI says it's done, that doesn't count. Only verifiable evidence on disk opens the quality gate.

In short: **Judgment goes to the AI; memory, constraints, and acceptance go to the workbench.**

---

## Core Capabilities

### 1. Complete Game Development Pipeline

KayingCodex breaks a game project into clear stages, automatically advancing, recording, and accepting each one:

```
Requirements → Discovery → Capability Audit → Planning → Contract Freeze
     → Scene Planning → Scene Building → Scene Gate
     → Gameplay Planning → Gameplay Building → Integration Gate
     → Testing → Decision → Release → Done
```

Every stage has clear deliverables and acceptance criteria. You can check progress at any time and know "where we are now and what comes next."

### 2. Assets That Actually Land

The easiest way to trip up in game development is "the art never got bound." KayingCodex has a built-in **semantic asset layer** that treats assets as reviewable, publishable packages: from discovery, import, and annotation to binding into scenes, validation, and publishing — every step is traceable. It tells you explicitly which assets are truly bound into the game and which were merely "declared."

### 3. Role-Based Collaboration

Inside the workbench, four specialist "roles" relay the work, each with its own responsibility:

| Role | Responsible for |
|---|---|
| **Game Director** | Requirements & acceptance criteria, overall planning, key decisions |
| **Scene Builder** | Scenes, interfaces, UI, asset binding |
| **Gameplay Engineer** | Gameplay logic, modules, state machines |
| **Quality Tester** | Acceptance scoring, feeding issues back to the Director |

Work flows between roles like a baton, with clean handoffs — no "who's supposed to own this?" mid-task confusion.

### 4. Built-in Knowledge Base (Offline)

No need for the AI to guess engine APIs. KayingCodex ships with a versioned, validated API knowledge base (covering 26 domains and 166 operations), fully available offline, ensuring generated code follows known, correct usage.

### 5. Two Runtime Options

| | **LocalRuntime** | **TapTap Runtime (Official)** |
|---|---|---|
| What it is | The app's built-in cross-platform Lua UI runner | TapTap's official local runner |
| Platforms | Cross-platform (macOS / Windows / Linux) | Windows only |
| Use case | Interactive design preview, instant local preview | TapTap platform builds & publishing |

LocalRuntime lets you see real rendered scene output directly in the app — no internet or external tools required.

---

## What Can You Do With It

- **Build a game from scratch**: Describe your idea, and the workbench will plan and progressively implement a playable prototype.
- **Visual design canvas**: Preview and adjust scenes and UI directly in the Design tab — what you see is what you get.
- **Manage your asset library**: Import, annotate, and bind art and audio assets, making sure they actually make it into the game.
- **Publish to TapTap**: Validate release readiness through the built-in flow and submit your build.

---

## Getting Started

### Installation

Download the installer for your platform (macOS / Windows / Linux) from the releases page, install, and launch. The app starts in Game Development mode by default.

### First Run

1. Launch KayingCodex to enter the game development workspace.
2. Create a new project or open an existing one.
3. Describe the game you want in natural language (e.g., "Make a 2D side-scrolling platformer where the player is a block that can jump and collect coins").
4. The workbench advances through the pipeline: confirming requirements first, then planning scenes and gameplay, building and accepting each step.
5. Preview results in real time on the design canvas; once satisfied, publish.

### Key Entry Points

- **Design tab**: Interactive preview of local-runtime scenes and UI.
- **Asset library**: View, import, and bind project assets.
- **Publish panel**: Validate release readiness and submit to TapTap.
- **"Run" tab in sidebar** (Windows): Run via TapTap Runtime.

---

## System Requirements

- **LocalRuntime (local preview)**: macOS / Windows / Linux all supported.
- **TapTap Runtime (official runs / publishing)**: Requires Windows.
- Internet connection required to download and update runtimes and asset resources.

---

## FAQ

**Q: How is this different from an ordinary AI coding assistant?**
Ordinary assistants finish editing files and "declare success" without verifying whether the game runs or the art got bound. KayingCodex uses persistent task flows and evidence-driven quality gates to make sure every step actually lands.

**Q: Where are my project files stored?**
Task progress and evidence inside a game project live in `.project/` within the project directory — portable, collaboration-friendly, easy to back up. The app's own config and logs live in `~/.KayingCodex/` under your user directory.

**Q: Do I need an internet connection?**
The knowledge base and local preview are fully offline-capable. Internet is required when integrating with TapTap platform builds and publishing.

**Q: Which platforms are supported?**
Local development and preview are cross-platform; official TapTap runs and publishing currently require Windows.

---

## License

[MIT](LICENSE) © Kaying Studio.
