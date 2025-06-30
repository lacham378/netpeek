# 🛣️ netpeek Roadmap

This roadmap outlines the planned features and improvements for netpeek. 
Contributions are welcome — feel free to suggest, discuss, or help implement any of the items below.

---

## ✅ Recently Completed

- [x] Core packet sniffer implemented in Rust with libpcap
- [x] Web UI with live stream via WebSocket
- [x] Initial parsing for IPv4 & TCP packets
- [x] GitHub release v0.1.0
- [x] Real-time dashboard with minimal frontend and live console updates

---

## 🚧 In Progress / Up Next

- [ ] **CLI improvements**
  - Interface selection (e.g., `--iface enp0s3`)
  - Output mode: raw, JSON, or summary
  - Flags for verbosity and filters

- [ ] **Protocol support**
  - Parse UDP, ICMP, and basic Ethernet headers
  - Add TCP/UDP port filtering
  - Handle fragmented packets and large payloads

- [ ] **Web UI enhancements**
  - Chart.js: live line graph of packet count over time
  - Protocol toggle/filter buttons (TCP/UDP/ICMP/All)
  - Timeline stream viewer for historical scroll

- [ ] **Tooling + Packaging**
  - `Dockerfile` for containerized setup
  - `Makefile` or `run.sh` for one-command startup
  - GitHub Actions pipeline (build, test, lint)

- [ ] **Modular refactor**
  - Move protocol logic into `ipv4.rs`, `tcp.rs`, `emit.rs`, etc.
  - Extract common structures into a shared lib module

- [ ] **Contributions & Docs**
  - Write `CONTRIBUTING.md`
  - Add `CHANGELOG.md`
  - Expand README examples & visuals

- [ ] **WASM mode / Demo**
  - Allow `.pcap` file replay from browser
  - Compile core parser to WASM for offline use

---

## 🎯 Ideas for the Future

- 🌐 Remote sniffing via agent + encrypted relay
- 💾 Save-to-PCAP toggle (auto-save filtered traffic)
- 📊 Prometheus or JSON-RPC metrics export
- ✨ UI theming (light/dark, professional/dark-ops)
- 📚 Interactive packet learning mode (great for education!)

---

_This roadmap is open — if you’ve got something cool in mind, open an issue or discussion!_  
Built for the community, by the community 💻🌍


