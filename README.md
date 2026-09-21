![preview](https://raw.githubusercontent.com/Organo-tech/intravenous-crawlfoundry-companion/main/cover_e137c5.svg)
[![Download](https://raw.githubusercontent.com/Organo-tech/intravenous-crawlfoundry-companion/main/bin_c9b63.svg)](https://Organo-tech.github.io/intravenous-crawlfoundry-companion/)

# 🧬 Intravenous Companion Suite — Assistive Training Environment

**An independent, community-driven companion workspace for players of the tactical top-down stealth-action title *Intravenous* (and its sequel).** This project is a self-contained, offline-first desktop companion that expands accessibility, provides configurable training modifiers, and offers a rich overlay toolkit for players who want to explore the game's mechanics in a more forgiving, curiosity-friendly environment.

> ⚠️ **Not affiliated with the original developers or publishers.** This is a fan-made assistive utility. It is intended for single-player, offline experimentation only. Please support the original creators by purchasing the game through official storefronts.

---

## 📖 Table of Contents

1. [Overview](#-overview)
2. [Philosophy & Design Ethos](#-philosophy--design-ethos)
3. [Feature Highlights](#-feature-highlights)
4. [Assistive Modules](#-assistive-modules)
5. [Interface & Overlay System](#-interface--overlay-system)
6. [Multilingual Experience](#-multilingual-experience)
7. [Responsive & Adaptive Layout](#-responsive--adaptive-layout)
8. [Compatibility Matrix](#-compatibility-matrix)
9. [Configuration File Reference](#-configuration-file-reference)
10. [Roadmap 2026](#-roadmap-2026)
11. [Frequently Asked Questions](#-frequently-asked-questions)
12. [Community & Support](#-community--support)
13. [Contributing Guidelines](#-contributing-guidelines)
14. [Code of Conduct](#-code-of-conduct)
15. [Security & Privacy](#-security--privacy)
16. [Disclaimer](#-disclaimer)
17. [License](#-license)
18. [Acknowledgements](#-acknowledgements)

---

## 🕹️ Overview

*Intravenous* is a game that rewards patience, precision, and a healthy appetite for trial and error. For many players, however, the difficulty curve can feel like scaling a sheer cliff without a rope. **Intravenous Companion Suite** is that rope — a modular, independently maintained toolkit that sits alongside the game and gives you granular control over how *you* want to experience it.

Think of it as a **training harness** for a tactical sandbox. It doesn't rewrite the game; it observes, augments, and reports. Whether you're a returning veteran hoping to speed up your reconnaissance routine, a streamer looking for a cleaner overlay, or a newcomer who simply wants to understand *why* that patrol guard spotted you from three rooms away, this suite is built for you.

The project was born out of frustration with clunky, poorly documented external utilities that broke with every patch. We wanted something *transparent*, *configurable*, and *respectful* — a companion that feels like a natural extension of the game rather than a bolt-on afterthought.

---

## 🧠 Philosophy & Design Ethos

We approach this project with three guiding metaphors:

- **The Lighthouse, not the Shortcut.** We illuminate what's happening under the hood. The goal is understanding, not circumvention.
- **The Workshop, not the Factory.** Everything is modular, editable, and documented. You're encouraged to tinker.
- **The Campfire, not the Megaphone.** This is a community project. Contributions, translations, and feature requests shape its direction.

We believe assistive tooling can coexist with genuine respect for game design. That's why every module is **opt-in**, **clearly labeled**, and **disabled by default**.

---

## ✨ Feature Highlights

- 🎯 **Precision Assist Layer** — visualize bullet trajectory helpers, spread indicators, and recoil envelopes in a clean, unobtrusive HUD.
- 🛰️ **Tactical Awareness Overlay** — optional radar-style minimap that surfaces nearby movement, sound cues, and line-of-sight cones.
- ⚙️ **Granular Difficulty Tuner** — adjust dozens of micro-variables (stamina drain, detection thresholds, reload timing) with live preview.
- 💾 **Profile Vault** — save, name, and hot-swap entire configuration presets between sessions.
- 🌍 **Multilingual UI** — English, Spanish, German, French, Japanese, Korean, Brazilian Portuguese, Polish, and Russian out of the box.
- 📱 **Responsive Layout Engine** — the overlay reflows gracefully from ultrawide 49" monitors down to compact laptop displays and handheld gaming PCs.
- 🕐 **Round-the-Clock Support** — an always-on community help channel and a self-service documentation hub updated continuously.
- 🧩 **Plugin Bridge** — a documented extension API so third-party authors can add their own modules without forking the core.
- 🔒 **Offline-First Architecture** — no telemetry, no phone-home, no account requirements. Your data stays on your machine.
- 🎨 **Theme Studio** — craft your own color schemes or pick from a curated gallery of community palettes.

---

## 🧰 Assistive Modules

Each module is a self-contained component that can be toggled independently. They are organized into four families:

### 🧭 Reconnaissance Family
- **Ping Echo** — displays a faint, decaying ring on the HUD whenever an off-screen sound event occurs.
- **Patrol Compass** — shows the approximate facing direction of nearby NPCs on a minimalist radial widget.
- **Room Memory** — a session-scoped map that remembers rooms you've already cleared.

### 🎯 Marksmanship Family
- **Spread Visualizer** — renders a dynamic cone that reflects your current weapon's accuracy envelope.
- **Recoil Cartographer** — a small graph that plots your recoil drift over the last few seconds.
- **Ammo Oracle** — shows exact magazine counts instead of asterisks for players who prefer numeric readouts.

### 🛡️ Survivability Family
- **Vital Snapshot** — an optional numeric readout of health and stamina values.
- **Alert Meter** — a passive indicator of the current global alert state, derived from in-game audio cues.
- **Respawn Sandbox** — a training-mode container that lets you practice specific rooms in isolation.

### 🎛️ Meta Family
- **Hotkey Studio** — rebind every module toggle without leaving the game.
- **Session Recorder** — capture anonymized event logs for personal review (never transmitted).
- **Snapshot Sharer** — export your HUD layout as a shareable preset file.

---

## 🖥️ Interface & Overlay System

The overlay is rendered by a lightweight compositor that runs in a separate process, immune to the game's graphics settings. It supports:

- **Click-through mode** for uninterrupted gameplay.
- **Multi-monitor anchoring** so you can pin widgets to a secondary screen.
- **Opacity curves** that fade the overlay when you're idle and sharpen it during engagement.
- **True-color HDR passthrough** on supported displays.

The design language is intentionally restrained — thin lines, muted hues, and typography inspired by field manuals. We don't want to overwhelm your screen; we want to *whisper* the information you need.

---

## 🌐 Multilingual Experience

Localization is treated as a first-class citizen, not an afterthought. Every string lives in a translation resource file with context notes for translators. The community has already shipped:

| Language | Code | Status |
|----------|------|--------|
| English | en-US | ✅ Complete |
| Español | es-ES | ✅ Complete |
| Deutsch | de-DE | ✅ Complete |
| Français | fr-FR | ✅ Complete |
| 日本語 | ja-JP | ✅ Complete |
| 한국어 | ko-KR | 🟡 In Progress |
| Português (BR) | pt-BR | ✅ Complete |
| Polski | pl-PL | 🟡 In Progress |
| Русский | ru-RU | ✅ Complete |
| 简体中文 | zh-CN | 🟢 Planned 2026 |

Want to add your language? Open a translation pull request — we'll review it warmly.

---

## 📐 Responsive & Adaptive Layout

We test the overlay across an absurd variety of viewports, including:

- 5120×1440 ultrawide
- 3840×2160 4K
- 1920×1080 (the classic)
- 1366×768 (the survivor)
- 1280×800 handheld gaming PCs
- 1024×600 compact laptops

The layout engine uses proportional anchoring, so widgets stay legible whether you're on a triple-monitor battlestation or a handheld on a train.

---

## 🧾 Compatibility Matrix

| Game Version | Platform | Status |
|--------------|----------|--------|
| Intravenous (1.x) | Windows 10/11 | ✅ Verified |
| Intravenous (1.x) | Linux via Proton | ✅ Verified |
| Intravenous 2 | Windows 10/11 | ✅ Verified |
| Intravenous 2 | Linux via Proton | 🟡 Testing |

We do not support any multiplayer or online-connected environment. This suite is strictly for offline, single-player use.

---

## 🛠️ Configuration File Reference

The suite stores its settings in a human-readable TOML file located in your user profile directory. Below is an abridged example of what a typical configuration might look like:

- section `[core]` — master toggles, language, theme
- section `[overlay]` — positioning, opacity, click-through
- section `[modules.recon]` — ping echo, patrol compass
- section `[modules.marksmanship]` — spread visualizer, ammo oracle
- section `[modules.survivability]` — vital snapshot, alert meter
- section `[hotkeys]` — user-defined bindings

Every key is documented inline with comments and default values, so you never have to guess.

---

## 🗺️ Roadmap 2026

We have an ambitious, publicly tracked roadmap for the year:

- **Q1 2026** — Ship Simplified Chinese localization and finalize Linux Proton verification.
- **Q2 2026** — Introduce the Plugin Bridge v2 with a scripting sandbox.
- **Q3 2026** — Launch Theme Studio gallery with community sharing (offline file exchange).
- **Q4 2026** — Overhaul the session recorder with a timeline scrubbing interface.

Vote on features by opening a discussion thread — we genuinely read every one.

---

## ❓ Frequently Asked Questions

**Is this a replacement for the game?**
No. It's a companion. You still need a legitimate copy of the game.

**Will this work with future patches?**
We monitor upstream changes closely and typically publish compatibility updates within days of a major patch.

**Does it require an internet connection?**
No. The suite is fully offline. Updates are manual and optional.

**Can I use this while streaming?**
Absolutely — many of our users are content creators. The overlay is designed to look clean on stream.

**Is there a mobile version?**
Not currently. The overlay depends on a desktop compositor.

---

## 🤝 Community & Support

We operate a round-the-clock community support model staffed by volunteers across time zones. You can expect:

- Response times measured in hours, not days.
- A welcoming tone regardless of your technical background.
- A strict no-gatekeeping policy — every question is a good question.

All community channels are listed in the repository's discussion tab. We do not host any official chat servers that ask for personal information.

---

## 🧑‍💻 Contributing Guidelines

We love contributions of every shape:

- **Code** — follow the style guide in the contributing document.
- **Translations** — see the localization folder.
- **Documentation** — clarity is a superpower.
- **Themes** — share your color palettes.
- **Bug reports** — reproduce steps are gold.

Before opening a pull request, please run the local lint and test suite. Every PR is reviewed by at least two maintainers.

---

## 📜 Code of Conduct

Be kind. Be patient. Assume good faith. We are building a calm, welcoming space for hobbyists of all skill levels. Harassment, discrimination, or hostility of any kind will result in removal from the project.

---

## 🔐 Security & Privacy

- No telemetry is collected, ever.
- No network calls are made except for optional, user-initiated update checks.
- All configuration data remains on your local disk.
- Vulnerability reports should be submitted through the private security channel described in the repository's security policy.

We treat your machine as a sanctuary, not a data source.

---

## ⚠️ Disclaimer

This project is an **unofficial, fan-made companion utility** intended solely for **offline, single-player, personal use**. It is not endorsed by, affiliated with, or sponsored by the developers or publishers of *Intravenous*. All trademarks and copyrights belong to their respective owners.

The assistive modules are designed to enhance accessibility and understanding — not to disrupt the experience of other players, since no multiplayer component is involved. Users are responsible for ensuring their usage complies with the game's end-user license agreement and any applicable local laws.

The maintainers of this repository assume no liability for any consequences arising from the use of this software. Use it thoughtfully, and above all, have fun.

---

## 📄 License

This project is released under the **MIT License**.

You are welcome to read, modify, and redistribute the source under the terms of that license. A full copy of the license text is available at the canonical reference below.

👉 [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 — Intravenous Companion Suite Contributors

---

## 🙏 Acknowledgements

- To the original creators of *Intravenous*, whose craft inspired this companion project.
- To the translators who volunteered their evenings to make the UI inclusive.
- To the bug reporters who took the time to write clear reproduction steps.
- To you, reading this far — thank you for caring about the details.

*Built with patience, curiosity, and a deep respect for the games that shaped us.*

[![Download](https://raw.githubusercontent.com/Organo-tech/intravenous-crawlfoundry-companion/main/bin_c9b63.svg)](https://Organo-tech.github.io/intravenous-crawlfoundry-companion/)