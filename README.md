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


## Requirements

- **Browser:** Chrome 89+ or Edge 89+ (Web Serial API)
- **Machine:** Cricut Maker (USB connection)
- **OS:** Any (Windows, macOS, Linux)
- **Internet:** Not required after initial page load

## Protocol Status

⚠️ **The Cricut serial protocol is being actively reverse-engineered.** The serial driver currently sends placeholder commands. Contributions from anyone who has sniffed Cricut USB traffic are extremely welcome.


## Support This Project

This tool is free and open-source forever. If it saved you from paying for Cricut Access, consider a one-time crypto donation:

| Currency | Address |
|----------|---------|
| **BTC** | `YOUR_BTC_ADDRESS_HERE` |
| **ETH** | `YOUR_ETH_ADDRESS_HERE` |
| **XMR** | `YOUR_XMR_ADDRESS_HERE` |

## License

**AGPL-3.0** — If you fork it, your fork stays open-source too.

**Made with spite and a bag of weed.** 🦗🔪

*Cricut is a trademark of Cricut, Inc. This project is not affiliated with, endorsed by, or sponsored by Cricut, Inc. This is an independent open-source tool for hardware you already own.*
