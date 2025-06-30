# 🧠 netpeek

**A real-time, high-performance network packet analyser built with Rust and powered by a live browser UI.** Lightweight, fast, and made for sysadmins, pentesters, and network explorers who want to see their traffic — clearly.

---

![netpeek dashboard screenshot](./ui/public/screenshot.png) <!-- Replace with actual screenshot path -->

[🚀 Release v0.1.0](https://github.com/lacham378/netpeek/releases/tag/v0.1.0) • MIT License

---

## ✨ Features

- ⚙️ Native Rust engine built on `libpcap` (fast and memory-safe)
- 📡 Live WebSocket stream to your browser
- 🌐 Realtime IPv4 & TCP/UDP packet parsing
- 🧩 Clean output: JSON line format, ready for piping or saving
- 📊 Easy-to-style dashboard with Socket.IO + HTML
- 🧪 Modular codebase — ready for CLI parsing, protocol extensions, and frontend charts

---

## 🚀 Quickstart

### 🔧 Prerequisites

- [Rust](https://www.rust-lang.org/tools/install)
- [Node.js (v16+)](https://nodejs.org/)
- Linux or WSL2 (libpcap required)

---

### 🦀 Build the Packet Engine

```bash
git clone https://github.com/lacham378/netpeek.git
cd netpeek/analyser
cargo build --release

