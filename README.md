# 🏜️ Lost Dune

A Godot 4 game exported to the web — play directly in your browser.

## 🎮 Play

**[▶ Play Now](https://mindfoldz0-spec.github.io/lost-dune/)** (after enabling GitHub Pages)

Or clone and open `LostDune.html` in a browser:
```bash
git clone https://github.com/mindfoldz0-spec/lost-dune.git
cd lost-dune
# Serve locally (required for WASM)
python -m http.server 8000
# Open http://localhost:8000/LostDune.html
```

> ⚠️ Cannot be opened via `file://` — must be served over HTTP due to WASM cross-origin policies.

## 🛠️ Built With

- **Godot 4** — Game engine
- **HTML5 / WebAssembly** — Browser runtime
- **Service Worker** — Offline support & caching

## 📁 Project Structure

```
LostDune.html                 # Entry point
LostDune.js                   # Godot engine loader
LostDune.wasm                 # WebAssembly runtime
LostDune.side.wasm            # GDExtension side module
LostDune.pck                  # Game data pack (85 MB)
LostDune.service.worker.js    # Offline caching
LostDune.manifest.json        # PWA manifest
LostDune.offline.html         # Offline fallback page
LostDune.icon.png             # App icon
LostDune.png                  # Splash screen
icons/                        # PWA icons (144, 180, 512px)
```

## 🚀 Deploy to GitHub Pages

1. Push to GitHub
2. Go to **Settings → Pages**
3. Set source to **Deploy from branch → main → / (root)**
4. Game will be live at `https://<username>.github.io/lost-dune/LostDune.html`

## 📜 License

This project is a personal game build. All rights reserved.

---

**Author:** [Mayuresh](https://github.com/mindfoldz0-spec)
