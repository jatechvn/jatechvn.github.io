# 🤖 Johnny's Developer Hub & Automation Portal

<p align="center">
  <a href="https://jatechvn.github.io/">
    <img src="assets/logo.png" alt="JA-HUB Logo" width="120" height="120" style="border-radius: 20px; box-shadow: 0 8px 24px rgba(0, 169, 201, 0.25);">
  </a>
</p>

<p align="center">
  <i>The official personal homepage and automated system gateway for <b>Johnny (jatechvn)</b>, built around the <b>JA-HUB</b> architecture.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Online-00ff87.svg?style=flat-square&logo=statuspage" alt="System Status">
  <img src="https://img.shields.io/badge/Theme-Obsidian_BilloDesign-00AFCD.svg?style=flat-square&logo=tailwindcss" alt="Theme">
  <img src="https://img.shields.io/badge/Tech-HTML5_/_CSS3_/_ES6-purple.svg?style=flat-square&logo=javascript" alt="Technology">
  <img src="https://img.shields.io/badge/Deploy-GitHub_Pages-orange.svg?style=flat-square&logo=github" alt="Deployment">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" alt="License">
</p>

<p align="center">
  <a href="#introduction">🚀 Introduction</a> • 
  <a href="#premium-billodesign-aesthetics">🎨 Design System</a> • 
  <a href="#key-features">💡 Key Features</a> • 
  <a href="#system-architecture">🏗️ Architecture Map</a> • 
  <a href="https://jatechvn.github.io/">🌐 Visit Portal</a>
</p>

<p align="center">
  🇻🇳 <a href="i18n/README.vi.md">Tiếng Việt Bản dịch</a>
</p>

---

## 🚀 Introduction

> *"Trong hệ sinh thái JA-HUB, không có dòng code nào hoạt động đơn độc. AHK là đôi tay, Python là trí tuệ, và Node.js là ý chí của người kiến trúc sư."* 🦞

**jatechvn.github.io** is the central dashboard portal designed to monitor, organize, and showcase Johnny's multi-technology automation ecosystem (**JA-HUB**). Rather than displaying static portfolio cards, this hub acts as an interactive system configuration explorer, giving a complete structural overview of all custom scripts and servers running across local workstations and cloud VPS instances.

---

## 🎨 Premium BilloDesign Aesthetics

Inspired by the dark cyber-minimalism of [billodesign.webflow.io](https://billodesign.webflow.io/), the portal features an **Obsidian Glass** theme system:

*   **Interactive 3D Spline Orb**: The hero section background embeds an interactive WebGL 3D glass orb. It captures cursor hover movements to rotate dynamically, providing a premium futuristic visual center.
*   **Curtained Welcome Preloader**: When the page loads, dark curtains lock scrolling and run a typed welcome greeting `"Welcome to JA-HUB"` along with a glowing progress bar, sliding open smoothly when ready.
*   **Rotating Gradient Borders**: All core dashboard cards (Player, Map, Terminal, Projects) and call-to-action buttons feature glowing borders that rotate infinitely, powered by CSS custom properties (`@property --angle` and `linear-gradient` overlays).
*   **Pulsing Status Indicators**: Integrated pulsing indicator dots next to panel titles to emphasize active processes.
*   **Adaptive Light & Dark Modes**:
    *   **Dark Mode (Default)**: Deep obsidian black `#010101`, frosted panels with thin cyan glow outlines, and high-tech typography.
    *   **Light Mode**: Frosted white glass layout (`rgba(245, 245, 247, 0.85)`), high-contrast gray text (`#111111`), and refined dark boundaries.
*   **Harmonious Typography**: Importing `Lato` (fordisplay/headings) paired with `IBM Plex Mono` / `JetBrains Mono` for code blocks and text outputs.

---

## 💡 Key Features

### 1. Interactive SVG System Map
An interactive vector graph visualizing the **JA-HUB (Central Brain)** connected to various worker nodes. Moving your mouse over nodes triggers animated flow indicators, representing real-time communication, and displays system details on a dedicated diagnostic panel.

### 2. Workspace Project Browser
Browse through all automation directories:
*   **Technology Filters**: Group by technology (Python, AHK, Node.js, PowerShell, Windows Batch, C#, VPS configurations).
*   **Live Search**: Real-time matching against project names, technology stacks, descriptions, and file path markers.
*   **Exploration Modal**: Expands to display code trees, allowing directories to collapse and expand dynamically.

### 3. Diagnostic Sandbox Terminal
A built-in simulated CLI terminal at the bottom of the portal. It lets users run diagnostic tasks locally:
*   `help`: Review available commands.
*   `status`: Scan active connections and monitor worker heartbeats (Watchdog log).
*   `list`: List technology roles in the Spokes structure.
*   `about`: Show the developer profile and design philosophy.
*   `clear`: Wipe console diagnostics.

### 4. Apple Music (iOS 16 style) Player
A glassmorphic audio player pinned to the left sidebar representing ambient workspace music:
*   **Dynamic Album Art**: Uses `jsmediatags` CDN to parse the playing MP3 metadata on-the-fly and extract the embedded album artwork to display as a circular spinning disk.
*   **Toggleable Volume Slider Panel**: Clicking the volume toggle button expands/collapses a matching seek-bar volume controller with mute/unmute and max shortcuts.
*   **Robust Setup**: Optimized scripts prioritize static page and project Explorer loading to bypass any CORS restrictions on local `file:///` protocols, with seamless autoplay fallbacks.

---

## 🏗️ System Architecture

| Node Spokes | Stack | Operational Role | Key Projects |
| :--- | :--- | :--- | :--- |
| **JA-HUB (Brain)** | Node.js / WS | Task Orchestrator, REST APIs, Websocket Server | `server.js`, `web_ui` |
| **Python Spokes** | Python 3.13 | Data mining, log analysis, local AI engines, GUI tools | `JA_AUTO_GIT`, `JA_KEY_CREATOR` |
| **AHK Spokes** | AutoHotkey v1/v2 | Windows UI clicks, hardware hooks, background controls | `TRAYSYSTEM.ahk`, `USB_Debug_detect` |
| **PowerShell** | WinRM / PS1 | Windows administrative control, LAN port scanner | `Network_Scanner.ps1` |
| **Batch Spokes** | Command Scripts | Quick environment builders, elevated privileges | `NSudo_8.2` |
| **C# Core** | C# / Sockets | High-performance socket routers, multi-threaded retest | `LVI_LX_RETEST_CHECK` |
| **VPS Spoke** | CentOS 7 | Host routing scripts, secure SFTP setups, cloud backup | `backup_agent.sh` |

---

## 📦 Directory Structure

```text
jatechvn.github.io/
├── index.html                 # Main entry point (Portal Page)
├── README.md                  # Documentation (This file)
├── ABOUT.txt                  # Simple system card
├── LICENSE                    # MIT license details
│
├── assets/                    # Static resources
│   ├── logo.png               # Brand icon (Lobster AI co-pilot logo)
│   ├── images/                # System graphic assets
│   │   └── icon.ico           # Website favicon icon
│   └── sounds/                # Playback audio and extracted arts
│       ├── *.mp3              # Playlist songs
│       └── *.jpg              # Extracted album artworks
│
└── i18n/                      # International readmes folder
    ├── README.vi.md           # Vietnamese version
    ├── README.zh-CN.md        # Chinese version
    └── README.ja-JP.md        # Japanese version
```

---

## 🌐 Quick Start & Local Run

To open the portal locally on your computer:

1.  Simply double-click the [index.html](index.html) file, or start a lightweight server in the workspace folder using python:
    ```bash
    python -m http.server 8000
    ```
2.  Open your browser and navigate to:
    ```text
    http://localhost:8000
    ```

---

## 📄 License

This repository is licensed under the **MIT License**. Check [LICENSE](LICENSE) for more details.
