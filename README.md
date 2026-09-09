# Ohshin Bhat Portfolio Clone (`ohsh.in`)

A pixel-perfect, 1:1 replica of [ohsh.in](https://ohsh.in), the personal website and portfolio of Ohshin Bhat.

## ✨ Features Replicated

- **Hero & Aesthetic**:
  - Retro-futuristic dark mode palette with noise, scanlines, and radial gradient glow.
  - Pixel font headings powered by Google Fonts (`Doto`, `Tektur`, `IBM Plex Mono`, `Lora`).
  - High-resolution hero background (`background.png`) with animated scan-roll and chromatic blur effects.
  - Floating pill navigation bar with active states, backdrop-blur glassmorphism, and pixelated Minecraft avatar/pickaxe icons.
- **About & Lore Section**:
  - Authentic typography, origin tags (`origin`, `taste`, `lore`, `polymath`, `side-quests`).
  - Styled portrait container with angle tilt and gradient blend (`profile.png`).
  - Embedded Spotify playlists (*Playlist 01* & *Playlist 02*).
  - Curated Sci-Fi reading stack with OpenLibrary book covers (*Dune*, *The Three-Body Problem*, *The Martian*, *1984*, *Project Hail Mary*, *Neuromancer*).
- **Work / Projects Section (`/work`)**:
  - Complete project showcase (*Zeno UI*, *Recur Obj Model*, *Prompt Now*) with tags, GitHub links, and live demos.
  - Interactive "Open Channels" contact cards (*Team channel*, *Growth channel*, *Fun channel*) linking to Cal.com, email, and social DMs.
  - Technical skills matrix (*Javascript*, *Typescript*, *React*, *React Native*, *Expo*, *Next.js*, *Tailwind*, *Python*, *GraphQL*, *AWS*, *Figma*, *Vite*, *Framer*, *Spline*, *GitHub*).
  - Career timeline & experience (*Dream11*, *Logitrix*, *Rewire*).
  - Live reach stats counter and animated metric cards.
  - Downloadable resume (`resume.pdf`).
- **Remix Client Hydration & API Routing**:
  - Full client-side navigation support between `/` and `/work`.
  - Built-in data loader endpoints (`?_data=routes%2F_index` and `?_data=routes%2Fwork`).
  - Organic page-view counter endpoint simulation (`/api/page-view`).

---

## 🚀 Quick Start

### 1. Launch with Python (Recommended)

Run the included server script:

```bash
python server.py
```

Or on Windows, simply double-click **`start.bat`**.

The server will automatically start on:
- **Home**: [http://localhost:3000](http://localhost:3000)
- **Work**: [http://localhost:3000/work](http://localhost:3000/work)

### 2. Static Server (Alternative)

You can also serve this folder with any static file server (e.g. `npx serve`, VS Code Live Server, or Python's built-in `http.server`):

```bash
python -m http.server 3000
```

---

## 📁 Directory Structure

```
ohsh-in/
├── index.html                     # Pre-rendered home page
├── work.html                      # Pre-rendered work & experience page
├── work/
│   └── index.html                 # Clean static route for /work
├── server.py                      # Local dev server with Remix loaders & API
├── start.bat                      # 1-click Windows launcher
├── index_data.json                # Home route loader payload
├── work_data.json                 # Work route loader payload
├── background.png                 # Hero background art
├── profile.png                    # Profile portrait
├── favicon.png                    # Site favicon
├── favicon.ico                    # Site icon
├── resume.pdf                     # Original resume document
└── assets/
    ├── tailwind-BLJyI5Uo.css       # Complete Tailwind styling bundle
    ├── entry.client-D5NWadp1.js   # Client hydration entry
    ├── manifest-75827b0d.js       # Remix route manifest
    ├── components-BrecM3Or.js     # Shared UI components
    ├── root-D56Tr3J4.js           # Root layout bundle
    ├── site-nav-DhKSKA3s.js       # Navigation bar bundle
    ├── _index-CG_3XinR.js         # Home page module
    ├── work-Cb3NvFOg.js           # Work page module
    ├── api.page-view-l0sNRNKZ.js  # Page view analytics module
    └── external/                  # Offline backup copies of covers & sprites
```
