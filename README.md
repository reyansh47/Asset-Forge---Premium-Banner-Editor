# ⚡ Asset Forge — Premium Browser-Based Banner Editor

> A fully-featured, zero-dependency social media image editor that runs entirely in a single HTML file. No React. No backend. No build step. Just open and create.

[![License: MIT](https://img.shields.io/badge/License-MIT-gold.svg)](https://opensource.org/licenses/MIT)
[![Single File](https://img.shields.io/badge/Size-Single%20HTML%20File-blueviolet)](./x-banner.html)
[![No Dependencies](https://img.shields.io/badge/Backend-None%20Required-brightgreen)](./x-banner.html)
[![Fonts](https://img.shields.io/badge/Fonts-20%20Google%20Fonts-orange)](./x-banner.html)

---

## 🌐 Live Demo

**[Try it live →](https://reyansh47.github.io/Asset-Forge---Premium-Banner-Editor/)**

---

## ✨ What is Asset Forge?

Asset Forge is a premium, Figma-inspired browser-based image editor built for creating stunning social media banners — Twitter/X headers, Instagram posts, stories, and custom formats — entirely in the browser with no install, no login, and no server.

Everything runs client-side in a **single HTML file** (~200KB). Open it locally or host it anywhere static.

---

## 🎯 Features

### 🖼️ Canvas & Backgrounds
- **Multi-format canvas presets** — Twitter/X (3:1), Instagram Square (1:1), Portrait (4:5), Story (9:16), Custom dimensions
- **Premium gradient backgrounds** — 5 built-in luxury linear gradient presets
- **Stock background library** — High-quality Unsplash CDN backgrounds
- **Background controls** — Opacity, zoom, pan X/Y, blur

### 🧱 Layer System
- **Drag & drop** layers anywhere on the canvas
- **8-point resize handles** with live bounding boxes
- **Rotation handle** — free rotate any layer
- **Layer panel** — visibility toggle, lock, reorder (bring forward/send back)
- **Snap guides** — horizontal and vertical center alignment snapping
- **Duplicate layer** — `Ctrl+D` or button
- **Delete layer** — `Delete` key or button

### ✍️ Text Tools
- **3 text presets** — Headline, Subtitle, Eyebrow
- **3 layout presets** — Minimal Luxury, Editorial Quote, Tech Blueprint
- **20 Google Fonts** in 4 categories (Serif, Modern Sans, Display/Impact, Handwriting)
- **Full typography controls** — size, weight, letter spacing, line height
- **Text alignment** — Left, Center, Right
- **Text transform** — None / UPPERCASE
- **Fill color** picker
- **Glow / ambient light** — color + blur radius slider
- **Text stroke / outline** — color + width slider
- **Inline double-click editing** — edit text directly on canvas

### 🔷 Shapes & Assets
- **Geometric shapes** — Rectangle, Circle, Triangle, Star, Hexagon, Line
- **Vector emblems** — Crown, Lion, Shield, Sword, Spiral, Crosshair, Badge Seal, and more
- **Color accent** control per shape layer

### 🎨 FX & Overlays
- **4 color grade presets** — Stoic Gold, Kintsugi Bronze, Neuro Reset, Ascension
- **Ambient glowing orbs** — size, position, color, opacity controls
- **Tech grid overlay** — color, opacity, density
- **Vignette** — center position, size, color, opacity
- **Film grain noise** — opacity control
- **Luxury border frame** — style, width, color, padding, corner accents

### 📐 Alignment Toolbar
Contextual floating toolbar that appears when a layer is selected:
- Align Left / Center Horizontally / Right
- Align Top / Center Vertically / Bottom
- **One-click "Center on Canvas"** button

### 💾 Save & Load Projects
- **Save Project** — exports full canvas state as a `.json` file
- **Load Project** — restores any previously saved `.json` project instantly
- Sessions are fully portable — share `.json` files between devices

### 📤 Export
- **PNG** (lossless) and **JPEG** (compressed) formats
- **1x / 2x / 3x resolution scaling** (web, Retina/HD, Ultra-HD/Print)
- **Copy to Clipboard** — directly paste into any app
- JPEG quality slider (50–100%)

### ⌨️ Keyboard Shortcuts
| Shortcut | Action |
|---|---|
| `Ctrl+Z` | Undo |
| `Ctrl+Y` | Redo |
| `Ctrl+D` | Duplicate selected layer |
| `Delete` | Delete selected layer |
| `Arrow Keys` | Nudge layer 1px |
| `Shift+Arrow` | Nudge layer 10px |
| `Escape` | Deselect layer |
| `Double-click` | Edit text inline |

---

## 🚀 Getting Started

### Option 1 — Just open it
```bash
# No install needed. Download and open directly:
open x-banner.html
```

### Option 2 — Clone and run locally
```bash
git clone https://github.com/reyansh47/Asset-Forge---Premium-Banner-Editor.git
cd Asset-Forge---Premium-Banner-Editor

# Open directly in browser
start x-banner.html       # Windows
open x-banner.html        # macOS
xdg-open x-banner.html   # Linux
```

### Option 3 — Serve with any static server
```bash
# Python
python -m http.server 8080

# Node
npx serve .
```

---

## 🏗️ Architecture

This is intentionally a **zero-build, zero-dependency** project:

```
x-banner.html        ← The entire application (HTML + CSS + JS)
```

**External dependencies loaded via CDN (no install):**
- [html2canvas](https://html2canvas.hertzen.com/) — Canvas → image export
- [Google Fonts](https://fonts.google.com/) — 20 premium typefaces

**No frameworks. No bundler. No npm. No backend.**

The canvas engine is built on DOM manipulation with a centralized `state` object, a 30-level undo/redo history stack, and a custom transform engine for drag/resize/rotate operations.

---

## 🎨 Design System

| Token | Value |
|---|---|
| Primary Black | `#050505` |
| Card Background | `#121212` |
| Gold Accent | `#d4af37` |
| Bronze Accent | `#cd7f32` |
| Border | `rgba(212, 175, 55, 0.15)` |
| Primary Font | Inter, Cinzel |

---

## 📋 Roadmap

- [ ] Multi-layer group selection
- [ ] Gradient fill on text layers
- [ ] Offline mode (bundled fonts + assets)
- [ ] Mobile touch support
- [ ] Shareable design links (via URL state encoding)
- [ ] More shape libraries (arrows, callouts, icons)

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

1. Fork the repo
2. Create your branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 👤 Author

**Reyansh** — [@reyansh47](https://github.com/reyansh47)

---

<div align="center">
  <sub>Built with vanilla HTML, CSS & JavaScript. No framework required.</sub>
</div>
