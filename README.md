[README.md](https://github.com/user-attachments/files/29266567/README.md)
# 🦗🔪 Stick-it-too-Cricut

**Free, open-source, browser-based Cricut Maker controller. No cloud. No subscription. No paywall.**

![Logo](assets/logo.png)

## What Is This?

Stick-it-too-Cricut is a complete Cricut Maker design-and-cut application that runs entirely in your browser. No Cricut Design Space. No Cricut Access subscription. No internet required after initial load. No data collection. No account needed. **Your machine, your rules.**

## Features

### Design Canvas
- Full SVG design canvas with pan, zoom, and grid
- Shape tools: rectangle, circle, polygon, star, line
- Text tool with live editing
- SVG and image (PNG/JPG) import via drag-and-drop or file dialog
- Selection, move, resize, flip, and transform
- Layers panel with visibility and lock
- Undo/Redo (Ctrl+Z / Ctrl+Y)
- Keyboard shortcuts for all tools
- Rulers with inch markings
- Snap-to-grid

### Cut Dashboard
- Material presets database (vinyl, cardstock, fabric, etc.)
- Custom pressure/speed/passes/blade settings
- Mat preview with auto-nesting (WIP)
- Test cut, load/unload mat controls

### Machine Connection
- Web Serial API — connect directly to your Cricut Maker via USB
- Serial console with command history
- Real-time TX/RX monitoring with timestamps

### Bonus
- 🦗 Cricket Splat — Chrome-dino-style mini-game while your cuts run
- Export to SVG and PNG
- Project save/load (IndexedDB + JSON download)

## Quick Start

1. Clone or download this repo
2. Open `index.html` in Chrome/Edge (Web Serial requires Chromium)
3. Design your project
4. Connect your Cricut Maker via USB
5. Select material, set parameters, cut

**Or visit the live site:** `https://YOUR_USERNAME.github.io/stick-it-too-cricut/`

## Requirements

- **Browser:** Chrome 89+ or Edge 89+ (Web Serial API)
- **Machine:** Cricut Maker (USB connection)
- **OS:** Any (Windows, macOS, Linux)
- **Internet:** Not required after initial page load

## Protocol Status

⚠️ **The Cricut serial protocol is being actively reverse-engineered.** The serial driver currently sends placeholder commands. Contributions from anyone who has sniffed Cricut USB traffic are extremely welcome.

## Project Structure

```
stick-it-too-cricut/
├── index.html          # Entry point
├── css/
│   └── theme.css       # CV-01.37 dark neon theme
├── js/
│   ├── app.js          # App shell & init
│   ├── canvas.js       # SVG canvas engine
│   ├── tools.js        # Drawing & selection tools
│   ├── layers.js       # Layer management
│   ├── history.js      # Undo/redo stack
│   ├── serial.js       # Web Serial driver
│   ├── console-terminal.js  # Serial debug terminal
│   ├── materials.js    # Material presets
│   ├── storage.js      # IndexedDB persistence
│   ├── shortcuts.js    # Keyboard shortcuts
│   └── cricket-game.js # 🦗 Mini-game
├── assets/
│   └── logo.png        # The psychotic cricket
├── README.md
└── LICENSE
```

## Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "initial commit"
git remote add origin git@github.com:YOUR_USERNAME/stick-it-too-cricut.git
git push -u origin main
```

Then enable GitHub Pages in repo Settings → Pages → Source: main branch, root `/`.

## Support This Project

This tool is free and open-source forever. If it saved you from paying for Cricut Access, consider a one-time crypto donation:

| Currency | Address |
|----------|---------|
| **BTC** | `YOUR_BTC_ADDRESS_HERE` |
| **ETH** | `YOUR_ETH_ADDRESS_HERE` |
| **XMR** | `YOUR_XMR_ADDRESS_HERE` |

Every sat, wei, and piconero keeps this project alive. 🦗🔪

## License

**AGPL-3.0** — If you fork it, your fork stays open-source too.

## Roadmap

- [ ] Path boolean operations (weld, slice, attach, flatten)
- [ ] Pen/bezier tool
- [ ] Node editing
- [ ] Full Cricut protocol reverse-engineering
- [ ] G-code generation from SVG paths
- [ ] Auto-nesting algorithm
- [ ] Multi-mat support
- [ ] Print-then-cut calibration
- [ ] DXF import/export
- [ ] Plugin system

---

**Made with spite and a soldering iron.** 🦗🔪

*Cricut is a trademark of Cricut, Inc. This project is not affiliated with, endorsed by, or sponsored by Cricut, Inc. This is an independent open-source tool for hardware you already own.*
