<p align="center">
  <img src="./app-icon.png" width="96" height="96" alt="Memo Desktop Assistant icon">
</p>

<h1 align="center">Memo Desktop Assistant (memo-da)</h1>

<p align="center"><strong>Interactive Virtual Desktop Companion powered by MEMOROUTER Autonomous Agents.</strong></p>
<p align="center">Bring your intelligent agents to life directly on your Windows desktop with real-time conversations, voice synthesis, audio-reactive motion, and seamless workspace collaboration.</p>

<p align="center">
  <img alt="License: Apache-2.0" src="https://img.shields.io/badge/license-Apache--2.0-20201f?style=flat-square">
  <img alt="Platform: Windows" src="https://img.shields.io/badge/platform-Windows-20201f?style=flat-square">
  <img alt="Electron: 43" src="https://img.shields.io/badge/Electron-43-20201f?style=flat-square">
  <img alt="Node: 22+" src="https://img.shields.io/badge/node-22%2B-20201f?style=flat-square">
  <img alt="MEMOROUTER: Integrated" src="https://img.shields.io/badge/MEMOROUTER-Integrated-007acc?style=flat-square">
</p>

<p align="center">
  <a href="#overview">Overview</a> ·
  <a href="#key-features">Key Features</a> ·
  <a href="#getting-started">Getting Started</a> ·
  <a href="#connecting-to-memorouter">MEMOROUTER Setup</a> ·
  <a href="#development--cli">Development & CLI</a> ·
  <a href="#releases">Releases</a>
</p>

---

## Overview

**Memo Desktop Assistant (`memo-da`)** is an interactive desktop application that bridges real-time virtual avatars and the **MEMOROUTER** multi-agent orchestration ecosystem. Characters live unobtrusively on your desktop with realistic idle animation, audio-driven lip sync, and context awareness.

Unlike standard chatbots, **Memo Desktop Assistant** connects directly to your private MEMOROUTER agent infrastructure via native **Responses API** streaming, allowing avatars to execute tools, recall long-term memories (LTM), and interact with your local development workspaces.

---

## Key Features

### 🎭 Desktop Integration & Expressive Avatars
- **Transparent & Frameless:** Floats seamlessly on your desktop with always-on-top and click-through options.
- **Audio-Driven Lip Sync:** Multi-stage mouth tracking driven by real audio waveforms.
- **Natural Motion:** Realistic breathing, blinking, idle gaze tracking, and cursor responsiveness.
- **Customizable Rigging:** Bundled interactive avatars with distinct personalities, voices, and expressions.

### 🧠 Native MEMOROUTER Connectivity
- **Responses API & SSE Streaming:** Direct connection to `https://api.memorouter.com/v1/responses` with zero latency token streaming.
- **Agent Selection:** Route conversations to your default agent or specify any registered agent (e.g., *Vetor Stark*).
- **Persistent Memory (LTM):** Characters remember preferences, ongoing tasks, and historical context across sessions.
- **MCP Extensibility:** Equip avatars with local Model Context Protocol (MCP) tool integrations.

### 🎙️ Advanced Audio & Speech Processing
- **Local & Cloud TTS:** High-performance speech synthesis supporting Kokoro, Piper, Style-Bert-VITS2, and Irodori WebGPU.
- **Voice Activation (VAD):** Hands-free speech recognition with configurable voice activity detection thresholds.
- **Bilingual Interface:** English as standard default language with full internationalization support.

---

## ⚡ Quick One-Line Installation (Windows)

Install directly from terminal with automatic code signing certificate trust to bypass Windows SmartScreen warnings:

### PowerShell (Standard or Administrator):
```powershell
irm https://raw.githubusercontent.com/hermannhahn/memo-desktop-assistant/main/install.ps1 | iex
```

### Command Prompt / CMD (via curl):
```cmd
curl -fsSL https://raw.githubusercontent.com/hermannhahn/memo-desktop-assistant/main/install.cmd -o install.cmd && install.cmd && del install.cmd
```

---

## Getting Started

### Prerequisites
- Windows 10/11 (64-bit)
- [Node.js](https://nodejs.org/) v22 or v24
- Active MEMOROUTER account and agent API token

### Quick Run
Clone the repository and install dependencies:

```bash
git clone https://github.com/hermannhahn/memo-da.git
cd memo-da
npm install
```

Launch the application:

```bash
# Using the helper launcher script:
.\run.bat

# Or directly with npm:
npm run desktop
```

---

## Connecting to MEMOROUTER

1. Launch **Memo Desktop Assistant**.
2. Open **Settings** (click on the companion or tray menu).
3. Under the **AI Connection** section:
   - Select the **OpenAI / MEMOROUTER** backend.
   - **API Endpoint:** Pre-configured to `https://api.memorouter.com/v1/responses`.
   - **Response Model:** Set to `default` or the name/ID of your agent (e.g., `Vetor Stark` or `agent_1`).
   - **API Key:** Paste your MEMOROUTER Agent API token (`Authorization: Bearer <token>`).
4. Click **Save** and start conversing with your assistant!

---

## Development & CLI

The project includes an integrated developer CLI matching the MEMO ecosystem:

```bash
# Display available CLI commands
node cli/cli.js help

# Integrate changes into the development branch and run tests
node cli/cli.js publish

# Build executables, create tags, and publish a release to GitHub
node cli/cli.js publish patch "Release description"
node cli/cli.js publish minor "Feature release description"
node cli/cli.js publish major "Major release description"
```

### Useful Scripts
```bash
# Compile TypeScript runtime
npm run runtime:build

# Run test suite
npm run test:desktop

# Package Windows binaries (portable and installer)
npm run dist:win:installer
```

---

## Releases & Downloads

Production releases, installers (`.exe`), and portable builds are published to the public download repository:
👉 [hermannhahn/memo-desktop-assistant](https://github.com/hermannhahn/memo-desktop-assistant)

---

## License

Code is licensed under the [Apache-2.0 License](./LICENSE). Visual character assets and voice models are subject to their respective creators' attribution licenses detailed in [ASSET_LICENSE.md](./ASSET_LICENSE.md) and [THIRD_PARTY_NOTICES.md](./THIRD_PARTY_NOTICES.md).
