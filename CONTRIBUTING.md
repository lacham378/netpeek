# 🤝 Contributing to netpeek

Thanks for your interest in improving **netpeek** — a fast, real-time network analyser powered by Rust and WebSockets!  
This project thrives on community ideas, fixes, and enhancements. Here’s how to get started:

---

## 🚀 Setup Guide

### 1. Clone the Repo

```bash
git clone https://github.com/lacham378/netpeek.git
cd netpeek

2. Build the Rust Engine

cd analyser
cargo build --release

Requires: libpcap-dev, build-essential, pkg-config

3. Start the Web UI

cd ../ui
npm install
node server.js

Visit http://localhost:3000 to view live packets.

💻 Contribution Types
We welcome:

🛠️ Bug fixes and code improvements
✨ New features (e.g. CLI flags, protocol parsing)
📖 Docs: tutorials, diagrams, or README updates
🧪 Tests and validation scripts
🎨 UI/UX improvements

📦 How to Contribute

Fork the repo and clone your fork
Create a new branch:

git checkout -b feature/my-awesome-feature

Make your changes

Commit clearly:
git commit -m "Add: TLS protocol parser for port 443"

Push and open a pull request 🎉

✅ Code Style & Notes
Format Rust with cargo fmt

Format JavaScript with Prettier (npx prettier --write .)
Keep logic modular — e.g., src/ipv4.rs, src/tcp.rs, src/emit.rs

Avoid breaking output structure or logs without discussion
Be kind in PRs and Issues — netpeek is a learning-first community

💬 Need Help?
Open an Issue

Suggest features in Discussions
Or @mention @lacham378 in your PR

Thanks for contributing to netpeek — you’re helping build a faster, clearer window into the networked world 🌐⚡


---

### ➕ Bonus: Link It in Your `README.md`
Near the bottom of `README.md`, add:

```markdown
---

## 🧠 Get Involved

Want to dive in, improve netpeek, or build something new?
See [CONTRIBUTING.md](./CONTRIBUTING.md) for how to get started.

View future plans in the [ROADMAP.md](./ROADMAP.md).
