# chess
# ♟️ 3D Wizard's Chess — Sanctuary Edition

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-Play_Now-D0BCFF?style=for-the-badge)](https://raghvendradubey01.github.io/chess/)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)
![WebGL](https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white)
![Material Design 3](https://img.shields.io/badge/Material_Design_3-757575?style=for-the-badge&logo=material-design&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)

A playable, full-featured **3D Wizard's Chess** web application built entirely with procedural WebGL geometry and textures. Set inside a minimalist Gothic cathedral sanctuary, **Ivory Marble** and **Volcanic Obsidian** armies clash with custom combat choreography, real-time shatter physics, synthesized cathedral acoustics, and a sleek **Material Design 3** single-level HUD.

🔗 **Live Demo:** [https://raghvendradubey01.github.io/chess/](https://raghvendradubey01.github.io/chess/)  
📦 **Repository:** [https://github.com/raghvendradubey01/chess](https://github.com/raghvendradubey01/chess)

---

## ✨ Key Features

### 🏛️ Minimalist Gothic Cathedral Environment
* **Architectural Sanctuary**: Surrounded by 8 clustered Gothic columns with warm flickering sconce point lights, a stepped octagonal sanctuary altar, and a bronze-framed chess table.
* **North-Nave Rose Window**: Custom procedural rose window with geometric stone tracery and stained-glass illumination.
* **Atmospheric Lighting & Particles**: Dynamic shadows, volumetric fog, moonlight shafts, and 260+ drifting arcane dust motes.

### 🗿 Procedural Marble vs. Obsidian Pieces
* **100% Procedural Assets**: Zero external 3D models or image dependencies. All 32 pieces are sculpted at runtime using `THREE.LatheGeometry`, custom crowns, battlements, mitres, and arcane runes.
* **Canvas-Generated Materials**:
  * **Marble (White)**: Polished stone with procedural gold and grey mineral veining (`clearcoat` + `physical` shaders).
  * **Obsidian (Black)**: Dark volcanic glass with crimson/violet fracture veins and glowing magma runes.

### ⚔️ Custom Animations & Shatter Physics
* **Idle & Hover**: Floating arcane finials/crowns gently bob and rotate; selected pieces levitate above their square with an arcane ring indicator.
* **Locomotion**: Smooth ease-in-out sliding across the board for standard pieces and high parabolic leaps for Knights.
* **Melee Strike & Shatter**: Capturing pieces approach the target, wind back, and cleave forward—shattering the defeated piece into **34 physics-simulated stone and rune shards** that bounce and settle across the altar floor alongside an expanding shockwave ring.
* **Dynamic Action Cam**: Automatically swoops in during captures for a cinematic close-up before returning to your chosen view.

### 🧠 Full Chess Engine & Wizard AI
* **Complete FIDE Ruleset**: Powered by `chess.js`—supports castling, *en passant*, pawn promotion (with an interactive 3D promotion modal), check, checkmate, stalemate, and insufficient material detection.
* **Wizard AI Opponent**: Built-in Minimax AI with alpha-beta pruning and positional piece-square evaluation tables for single-player duels, plus a **2-Player Pass & Play** mode.

### 🎨 Material Design 3 Single-Level HUD
* **Zero Nested Menus**: All controls are accessible from a single-level floating Material Design 3 glassmorphic interface.
* **Camera Presets**: Instant transitions between **Marble**, **Obsidian**, **Vault (Top-Down)**, and **Action Cam** toggle, alongside full `OrbitControls` support.
* **Collapsible Algebraic Chronicle**: Live move history drawer and real-time captured piece counters.
* **Synthesized Cathedral Audio**: Built with the **Web Audio API**—stone slides, heavy marble impacts, crystalline shatter bursts, and low brass check horns with zero external audio files required.

---

## 🚀 Getting Started

Because the entire application uses procedural geometry, canvas textures, and Web Audio synthesis, **no build step or bundler is required**.

### Option 1: Direct Browser Launch
1. Clone this repository:
   ```bash
   git clone [https://github.com/raghvendradubey01/chess.git](https://github.com/raghvendradubey01/chess.git)
   cd chess
### option 2: Local Development Server
# Using Python 3
python -m http.server 8000

# OR using Node.js (npx)
npx serve .

# Tech Stack
>Three.js (r128) — 3D WebGL rendering, procedural lathe geometry, PBR materials, lighting, and shadow mapping.
>Chess.js — Legal move generation, board state management, and game-over validation.
>Web Audio API — Real-time procedural sound effects (stone friction, melee impact, glass/stone shatter, check horn).
>HTML5 Canvas API — Runtime procedural generation of veined marble, fractured obsidian, and board tile textures.
>Material Design 3 (Dark Theme) — Custom CSS variables, elevation tokens, and glassmorphic surface styling.

# Project Structure
chess/
├── index.html       # Complete self-contained 3D application (HTML, MD3 CSS, Three.js & AI Engine)
└── README.md        # Project documentation


