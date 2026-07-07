# 🤖 Johnny's Developer Hub & Software Ecosystem (JA-HUB)

<p align="center">
  <a href="https://jatechvn.github.io/">
    <img src="assets/logo.png" alt="JA-HUB Logo" width="120" height="120" style="border-radius: 20px; box-shadow: 0 8px 24px rgba(255, 255, 255, 0.1);">
  </a>
</p>

<p align="center">
  <i>The official personal homepage and digital software showcase for <b>Johnny (jatechvn)</b>, built around the <b>JA-HUB</b> architecture.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Online-00ff87.svg?style=flat-square&logo=statuspage" alt="System Status">
  <img src="https://img.shields.io/badge/Theme-Infinity_Carbon-black.svg?style=flat-square&logo=tailwindcss" alt="Theme">
  <img src="https://img.shields.io/badge/Tech-HTML5_/_CSS3_/_ES6-purple.svg?style=flat-square&logo=javascript" alt="Technology">
  <img src="https://img.shields.io/badge/Deploy-GitHub_Pages-orange.svg?style=flat-square&logo=github" alt="Deployment">
  <img src="https://img.shields.io/badge/Version-v6.1.0-blue.svg?style=flat-square" alt="Version">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" alt="License">
</p>

<p align="center">
  <a href="#introduction">🚀 Introduction</a> • 
  <a href="#infinity-style-design-system">🎨 Design System</a> • 
  <a href="#ecosystem-flagships">📦 Flagships</a> • 
  <a href="#key-features">💡 Key Features</a> • 
  <a href="https://jatechvn.github.io/">🌐 Visit Portal</a>
</p>

<p align="center">
  🇻🇳 <a href="i18n/README.vi.md">Tiếng Việt Bản dịch</a>
</p>

---

## 🚀 Introduction

> *"Trong hệ sinh thái JA-HUB, không có dòng code nào hoạt động đơn độc. AHK là đôi tay, Python là trí tuệ, và Node.js là ý chí của người kiến trúc sư."* 🦞

**jatechvn.github.io** is the central showcase portal designed to organize, document, and host compiled binary executables and scripting ecosystems built under the **JA-HUB** workspace. 

Adapting the premium, developer-focused architecture of **infinitytechstack.uk**, the portal presents Johnny's utilities as a high-performance, single-page bento dashboard, providing clear technical specs, offline documentation, and download hubs for both Dart and Python ecosystems.

---

## 🎨 Infinity-Style Design System

The portal adopts a technical, neomorphic dark-glass look with cutting-edge visual elements:

*   **Stage Curtains Welcome Preloader**: On initial page load, split-curtains cover the screen with an elegant center seam line, parting horizontally with a custom theatre-ease transition (`cubic-bezier(0.85, 0, 0.15, 1)`) to reveal the website.
*   **Translucent 3D Glass Portal**: The landing screen features a blurred glass sheet overlaying the active WebGL canvas, displaying the 3D shapes as a gaseous, abstract neomorphic dreamscape behind the text.
*   **Radial Background Glows**: Soft cyan, magenta, and purple radial gradients float at various depths, slowly drifting and scaling over time.
*   **Scroll-Driven WebGL Parallax**: Integrates four adjustable 3D WebGL background themes (Glass Orbs, 3D Waves, Gallery, Showroom). Scrolling vertically down the page drives the camera depth down the Z-axis, flying past the 3D geometries in real time.
*   **Bento Grid Card outlines**: Glass cards feature thin transparent borders that grow in brightness on hover, projecting an emerald glow for Dart tools and a purple glow for Python tools.
*   **iPhone-style Dynamic Island Music Widget**: Merges ambient track metadata and playback indicators into a responsive capsule in the header navigation that dynamically auto-stretches its width based on text length. Smoothly morphs on hover to reveal playback controls (play/pause, next/prev) and a spinning album CD containing the active track's cover art.
*   **Sound FX Triggers**: Satisfying clicking sounds (beep.mp3) and hover highlights (hover.mp3) trigger on interactive elements to mimic physical interface control.
*   **Typography**: Clean `Inter` font paired with `JetBrains Mono` for tech metadata tags and versions.

---

## 🏗️ Stacks & Structure

The portal categorizes the 14 ecosystem tools into two distinct core stacks:

### 🟢 Dart Compiler Stack (9 Stacks)
Compiled, optimized standalone Windows executables replacing manual connects, device mirrors, and git synchronizers:
*   `ja_adb_tool`: Device mirroring and ADB command interface.
*   `ja_auto_git`: Git initializer and repository templates publisher.
*   `ja_connect`: Tunnel manager and proxy sockets.
*   `ja_key_creator`: Cryptographic license key generators.
*   `ja_qrcode`: Local CLI and GUI barcode makers.
*   `ja_ssh_monitor`: Server shell monitor and remote telemetry.
*   `ja_symlink`: NTFS directory junctions controller.
*   `ja_sync`: Backup mirroring and incremental folder syncer.
*   `ja_wifi_manager`: LAN Wi-Fi profile and credentials checker.

### 🟣 Python Script Ecosystem (5 Stacks)
Rich GUI toolkits and DevOps modules running PySide6 architectures:
*   `CLONE_VOICE_TOOL`: Neural AI voice cloner and speech synthesis.
*   `JA_AutoBuild`: PyInstaller standalone executable wrapper.
*   `JA_AUTO_GIT`: Concurrently managing git trees via desktop panels.
*   `JA_SMART_BK`: Background folder watcher backups.
*   `JA_TRANSLATE`: Database dictionary translator GUI.

---

## 💡 Key Features

### 1. Dynamic Search & Filters
Filter the bento layout instantly by clicking tags, search terms, or stack tabs (`All Stacks`, `Dart Stack`, `Python Stack`). Cards shift and arrange smoothly using client-side layout adjustments.

### 2. Apple Music style Player
A custom iOS-style music player pinned to the header playing Johnny's 5 local ambient tracks, complete with animative audio visualizer bars, volume seek slider, and toggleable mute/unmute actions.

### 3. Detailed Manual Modals
Clicking any bento card launches a detailed overlay guide showcasing custom key features, markdown README guides, and compiled release zip/exe direct downloads.

---

## 🌐 Quick Start & Local Run

Simply open [index.html](index.html) in any modern browser, or run a local web server:
```bash
python -m http.server 8000
```
Open browser and navigate to:
```text
http://localhost:8000
```

---

## 📄 License
This portal is licensed under the **MIT License**.
