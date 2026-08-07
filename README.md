# 🏜️ Lost Dune

> **A Godot 4 browser-based survival adventure**  
> Explore the endless dunes, survive the harsh desert, and uncover the mysteries of a forgotten world — all from your browser.

[![Play Now](https://img.shields.io/badge/🎮-Play%20Now-brightgreen)](https://mindfoldz0-spec.github.io/lost-dune/)
[![Godot 4](https://img.shields.io/badge/Godot-4-blue?logo=godot-engine)](https://godotengine.org/)
[![WebAssembly](https://img.shields.io/badge/WebAssembly-Enabled-orange)](https://webassembly.org/)
[![PWA](https://img.shields.io/badge/PWA-Ready-purple)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)

---

## 🚀 Quick Start

### ▶ Play Online
Visit **[Lost Dune on GitHub Pages](https://mindfoldz0-spec.github.io/lost-dune/)** to play instantly in your browser.

### 💻 Local Development
```bash
git clone https://github.com/mindfoldz0-spec/lost-dune.git
cd lost-dune

# Serve locally (required for WASM)
python3 -m http.server 8000

# Open in browser: http://localhost:8000
```

> ⚠️ **Important:** The game cannot run via `file://` due to WebAssembly cross-origin policies. Always use a local HTTP server.

---

## ✨ Features

- 🌍 **Browser-Native**: No downloads required — plays directly in modern browsers
- 📱 **PWA Support**: Install as an app on desktop or mobile for offline play
- 🎮 **Godot 4 Power**: Built with the latest Godot engine features
- 🏜️ **Immersive Desert Survival**: Dynamic weather, resource management, and exploration
- 🔊 **Spatial Audio**: 3D positional audio using Web Audio API worklets
- 🚀 **Optimized WASM**: Fast loading with side-module architecture

---

## 🛠️ Technical Stack

| Component | Technology |
|-----------|------------|
| **Game Engine** | Godot 4.x |
| **Runtime** | HTML5 + WebAssembly |
| **Audio** | Web Audio API + Audio Worklets |
| **Offline** | Service Worker + Cache API |
| **PWA** | Web App Manifest + Icons |

### Key Files

| File | Purpose |
|------|---------|
| `index.html` | Entry point for the game |
| `LostDune.js` | Godot engine loader & bootstrap |
| `LostDune.wasm` | Core WebAssembly runtime |
| `LostDune.side.wasm` | GDExtension side module |
| `LostDune.pck` | Game data pack (~85 MB) |
| `LostDune.service.worker.js` | Offline caching logic |
| `LostDune.offline.html` | Fallback page when offline |
| `LostDune.manifest.json` | PWA installation manifest |

---

## 📦 Installation & Deployment

### Deploy to GitHub Pages

1. Push this repository to GitHub
2. Navigate to **Settings → Pages**
3. Configure:
   - **Source**: Deploy from branch
   - **Branch**: `main` (or `master`)
   - **Folder**: `/ (root)`
4. Your game will be live at:  
   `https://<username>.github.io/lost-dune/`

### Alternative Hosting

Works with any static hosting service:
- Netlify
- Vercel
- Cloudflare Pages
- Apache/Nginx servers

**Server Requirements:**
- Must serve files over HTTP/HTTPS
- Should support `.wasm` MIME type (`application/wasm`)
- Recommended: Enable gzip/brotli compression for `.pck` and `.wasm` files

---

## 🎯 Browser Compatibility

| Browser | Status |
|---------|--------|
| Chrome 90+ | ✅ Fully Supported |
| Firefox 88+ | ✅ Fully Supported |
| Safari 15+ | ✅ Fully Supported |
| Edge 90+ | ✅ Fully Supported |

**Required Features:**
- WebAssembly
- Service Workers
- Web Audio API
- Offscreen Canvas (recommended)

---

## 🤝 Contributing

This is a personal project, but feel free to:
- 🐛 Report bugs via Issues
- 💡 Suggest features or improvements
- 🍴 Fork and experiment with your own versions

---

## 📄 License

© [Mayuresh](https://github.com/mindfoldz0-spec). All rights reserved.

This project is a personal game build. The code and assets are not licensed for redistribution or commercial use without explicit permission.

---

## 🙏 Acknowledgments

- Built with ❤️ using [Godot Engine](https://godotengine.org/)
- Inspired by classic survival games and desert exploration adventures
- Thanks to the amazing Godot community for continuous support

---

<div align="center">

**Ready to explore the dunes?**  
[🏜️ Launch Lost Dune](https://mindfoldz0-spec.github.io/lost-dune/)

*Made with Godot 4 • Powered by WebAssembly*

</div>
