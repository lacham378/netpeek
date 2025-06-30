# 🧠 netpeek

**A real-time, high-performance network packet analyser built with Rust and powered by a live browser UI.** 
Lightweight, fast, and made for sysadmins, pentesters, and network explorers who want to see their traffic — clearly.

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


Make sure you have required libraries installed:

sudo apt install build-essential pkg-config libpcap-dev

🌐 Launch the Web UI

cd ../ui
npm install
node server.js

Then visit: http://localhost:3000

💡 The server auto-spawns the Rust analyser on browser connect.

🧠 Architecture

┌────────────┐     stdout     ┌────────────┐     socket.io     ┌─────────────┐
│  Rust Sniffer │ ───────────▶│  Node Server │ ───────────────▶│   Browser UI │
└────────────┘                └────────────┘                   └─────────────┘
libpcap                      WebSocket bridge                Live JSON feed

📷 Screenshot
<!-- You can swap this with an actual GIF/demo --> <img src="./ui/public/screenshot.png" width="700" alt="netpeek UI example">

🛠 Developer Notes

All parsing is in analyser/src/ — you can extend it with more protocol layers

UI uses minimal HTML/JS — great for custom skins, metrics, or timeline graphs

CLI parsing, filters, and PCAP ingest planned for future releases

🤝 Contributing

Want to make netpeek even better? PRs are welcome!

# Clone your fork and make changes in a new branch
git checkout -b feature/your-feature-name


✅ Please include:

Clear feature/fix description

Clean commits and formatting

Any new dependencies added to Cargo.toml or package.json

💬 Open issues for discussion, suggestions, or bugs.

📦 License

MIT

🙌 Acknowledgements
Built with love by @lacham378 Made possible by: Rust, libpcap, Socket.IO, and the open source community ❤️

📍 Roadmap
[ ] Add CLI support for selecting interfaces and output format
[ ] Parse TCP/UDP headers with port filtering
[ ] Add Chart.js for live visualizations
[ ] Build Docker container for standalone deployment
[ ] WASM frontend decoder for .pcap replay mode


---

Let me know when you’ve got a screenshot (or if you'd like help capturing one in the browser), and I’ll make sure
it slots in beautifully. When you’re ready, we can do `CONTRIBUTING.md`, `CHANGELOG.md`, or even generate a `Makefile`
for one-command launch.

netpeek is looking like the kind of tool that gets bookmarked and starred — now it’s going to *read* like it too 🚀














