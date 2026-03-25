<!-- BlackRoad SEO Enhanced -->

# ulackroad roadworld

> Part of **[BlackRoad OS](https://blackroad.io)** — Sovereign Computing for Everyone

[![BlackRoad OS](https://img.shields.io/badge/BlackRoad-OS-ff1d6c?style=for-the-badge)](https://blackroad.io)
[![BlackRoad-Interactive](https://img.shields.io/badge/Org-BlackRoad-Interactive-2979ff?style=for-the-badge)](https://github.com/BlackRoad-Interactive)

**ulackroad roadworld** is part of the **BlackRoad OS** ecosystem — a sovereign, distributed operating system built on edge computing, local AI, and mesh networking by **BlackRoad OS, Inc.**

### BlackRoad Ecosystem
| Org | Focus |
|---|---|
| [BlackRoad OS](https://github.com/BlackRoad-OS) | Core platform |
| [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc) | Corporate |
| [BlackRoad AI](https://github.com/BlackRoad-AI) | AI/ML |
| [BlackRoad Hardware](https://github.com/BlackRoad-Hardware) | Edge hardware |
| [BlackRoad Security](https://github.com/BlackRoad-Security) | Cybersecurity |
| [BlackRoad Quantum](https://github.com/BlackRoad-Quantum) | Quantum computing |
| [BlackRoad Agents](https://github.com/BlackRoad-Agents) | AI agents |
| [BlackRoad Network](https://github.com/BlackRoad-Network) | Mesh networking |

**Website**: [blackroad.io](https://blackroad.io) | **Chat**: [chat.blackroad.io](https://chat.blackroad.io) | **Search**: [search.blackroad.io](https://search.blackroad.io)

---


BlackRoad Earth street-level exploration module built with MapLibre GL.

## Features

### Core Features
- **Globe View**: Start from space and zoom down to street level
- **5 Map Styles**: Satellite, Streets, Dark, Terrain, Hybrid
- **Location Search**: Search any location worldwide using Nominatim
- **Quick Locations**: 6 pre-configured famous landmarks
- **User Location**: Find and navigate to your current location
- **Responsive UI**: Works on desktop and mobile

### Advanced Features (NEW!)
- **3D Buildings 🏢**: Vector-based building extrusion with height data
- **Custom Markers 🎯**: Create categorized markers (favorite, work, home, travel, food, custom)
- **Measurement Tools 📏**: Measure distances and areas with Haversine formula
- **URL Sharing 🔗**: Generate shareable links with exact position and view
- **Saved Locations 💾**: Save and manage favorite locations
- **Tools Panel 🛠️**: Comprehensive tools menu with organized sections
- **Real-time Stats**: Live altitude, resolution, and coordinate display
- **Notifications**: Toast-style user feedback system

### Technical Features
- **LocalStorage**: Persistent markers and settings
- **URL Parameters**: Deep linking support
- **Geospatial Calculations**: Accurate distance and area measurements
- **Interactive Panels**: Tools, markers, and saved locations UI
- **History Tracking**: Track search and navigation history

## Technology Stack

- **MapLibre GL**: Open-source mapping library
- **Vanilla JavaScript**: Modular ES6+ architecture
- **LocalStorage**: Client-side data persistence
- **Nominatim**: OpenStreetMap geocoding service

## Project Structure

```
roadworld/
├── public/
│   └── index.html          # Main HTML file
├── src/
│   ├── css/
│   │   └── main.css        # Styles
│   └── js/
│       ├── main.js         # Application entry point
│       ├── config.js       # Configuration and constants
│       ├── mapManager.js   # Map initialization and control
│       ├── uiController.js # UI updates and interactions
│       ├── searchService.js # Location search
│       ├── storageManager.js # Local storage management
│       ├── buildingsManager.js # 3D buildings layer
│       ├── markerManager.js # Custom markers system
│       ├── measurementTools.js # Distance/area measurement
│       └── urlManager.js   # URL sharing and parameters
├── package.json
├── wrangler.toml
└── README.md
```

## Development

Run locally:

```bash
cd ~/roadworld
npm run dev
```

Open http://localhost:8000/public in your browser.

## Deployment

Deploy to Cloudflare Pages:

```bash
npm run deploy
```

Or deploy via Git:

```bash
git init
git add .
git commit -m "Initial RoadWorld module"
gh repo create blackroad-roadworld --public --source=. --remote=origin
git push -u origin main

# Then connect to Cloudflare Pages dashboard
```

## Configuration

### Map Styles

Edit `src/js/config.js` to add or modify map tile sources:

```javascript
export const STYLES = {
  // Add your custom style here
}
```

### Default Settings

Modify `MAP_CONFIG` in `src/js/config.js`:

```javascript
export const MAP_CONFIG = {
  center: [0, 20],
  zoom: 1.5,
  minZoom: 0,
  maxZoom: 22,
  projection: 'globe',
  antialias: true
};
```

## Usage

### Search Locations

Type any location name, address, or coordinates in the search bar and click "FLY TO".

### Quick Navigation

Click any of the quick location buttons on the right side for instant travel to famous landmarks.

### 3D View

Click the 🏢 button to toggle 3D building mode and tilt the map.

### Save Locations

Click the 💾 button to save the current view to your favorites.

### Keyboard Shortcuts

- **Drag**: Pan and rotate
- **Scroll**: Zoom in/out
- **Ctrl+Drag**: Tilt the map
- **Right-click drag**: Rotate the view

## API Usage

The application uses free tile providers and the Nominatim geocoding service. No API keys required.

## BlackRoad Integration

Part of the BlackRoad Earth infrastructure. Integrates with:

- BlackRoad OS Operator
- Cloudflare Pages deployment
- GitHub repository system

## License

MIT License - BlackRoad Systems

---

## 📜 License & Copyright

**Copyright © 2026 BlackRoad OS, Inc. All Rights Reserved.**

**CEO:** Alexa Amundson | **PROPRIETARY AND CONFIDENTIAL**

This software is NOT for commercial resale. Testing purposes only.

### 🏢 Enterprise Scale:
- 30,000 AI Agents
- 30,000 Human Employees
- CEO: Alexa Amundson

**Contact:** blackroad.systems@gmail.com

See [LICENSE](LICENSE) for complete terms.
