# 🔴⚫ AC Milan — Wallpaper Engine Live Wallpaper

A stunning animated desktop wallpaper celebrating **AC Milan's glorious history**, built with HTML/CSS/JS for [Wallpaper Engine](https://store.steampowered.com/app/431960/Wallpaper_Engine/).

> *Sempre il Milan · Forza Rossoneri*

---

## ✨ Features

- **Classic Red & Black Stripes** — Iconic Rossoneri stripes as an elegant dark background layer
- **Photo Carousel** — Auto-rotating showcase of classic squad photos with year captions and crossfade transitions
- **Honours Timeline** — Infinite-scrolling gold-on-black palmares with custom SVG trophy icons for each competition
- **Gold Particle System** — Floating gold dust particles with glow and flicker effects
- **Audio Visualizer** — System audio-reactive gold frequency bars at the bottom edge (works with any music player)
- **Badge Display** — Pulsing glow animation for the AC Milan crest
- **Corner Ornaments & Decorative Lines** — Gold filigree details throughout
- **Fully Responsive** — Adapts to any resolution: 1080p, 2K, 4K, ultrawide (21:9, 32:9)
- **FPS Limiter** — Respects Wallpaper Engine's performance settings
- **Customizable** — Accent color, particle density adjustable via Wallpaper Engine properties

## 🏆 Honours Displayed

| Competition                           | Count | Trophy Icon     |
| ------------------------------------- | ----- | --------------- |
| Champions League                      | 7     | Big Ears Cup    |
| Serie A / Scudetto                    | 19    | Shield          |
| Intercontinental Cup / Club World Cup | 4     | Globe           |
| UEFA Super Cup                        | 5     | Super Cup       |
| Cup Winners' Cup                      | 2     | Classic Cup     |
| Coppa Italia                          | 5     | Italian Cup     |
| Supercoppa Italiana                   | 7     | Star Cup        |
| Latin Cup                             | 2     | Hexagonal Medal |

All trophy icons are hand-drawn SVG in a unified gold wireframe style.

---

## 📸 Demo

[![AC Milan Wallpaper Demo](https://img.youtube.com/vi/LgbcvUa3PS0/maxresdefault.jpg)](https://youtu.be/LgbcvUa3PS0)

▶️ **[Watch on YouTube](https://youtu.be/LgbcvUa3PS0)**

---

## 📁 Project Structure

```
ac-milan-wallpaper/
├── index.html          # Main wallpaper (single-file, all CSS/JS inline)
├── project.json        # Wallpaper Engine configuration
├── badge.png           # AC Milan badge — YOU provide this
├── preview.jpg         # Optional: preview image for WE browser
├── photos/             # Classic squad photos — YOU provide these
│   ├── 1988-89.jpg     # Sacchi's Grande Milan
│   ├── 1989-90.jpg     # Back-to-back European Cups
│   ├── 1993-94.jpg     # 4-0 vs Barcelona in Athens
│   ├── 1995-96.jpg     # Capello's Invincibles
│   ├── 2002-03.jpg     # Old Trafford — Shevchenko, Pirlo, Maldini
│   ├── 2006-07.jpg     # Revenge in Athens — Inzaghi's Brace
│   ├── 2010-11.jpg     # Allegri's Scudetto
│   └── 2021-22.jpg     # Pioli's Title after 11 Years
└── README.md
```

> ⚠️ **Photos and badge are NOT included** in this repo due to copyright. The wallpaper works without them (shows placeholders), but looks best with your own images.

---

## 🚀 Installation

### Prerequisites

- [Wallpaper Engine](https://store.steampowered.com/app/431960/Wallpaper_Engine/) on Steam

### Steps

1. **Clone or download** this repository

   ```bash
   git clone https://github.com/huxiaoming274/ac-milan-wallpaper.git
   ```

2. **Add your own media files** (not included due to copyright):

   - `badge.png` — AC Milan badge (PNG, transparent background, 512×512+ recommended)
   - `photos/*.jpg` — Squad photos for each era (any resolution, the frame auto-adapts)

3. **Import into Wallpaper Engine**:

   - Open Wallpaper Engine Editor
   - Drag `index.html` onto the **"Create Wallpaper"** button
   - Done!

---

## ⚙️ Customization

### Via Wallpaper Engine Settings

| Setting                   | Description                             |
| ------------------------- | --------------------------------------- |
| **Gold Accent Color**     | Change the gold to any color you like   |
| **Gold Particle Density** | Adjust floating particle count (10–200) |

### Via Code

Edit the `PHOTO_SLIDES` array near the top of `index.html` to add, remove, or reorder photos:

```javascript
const PHOTO_SLIDES = [
  {
    file: 'photos/1988-89.jpg',
    year: '1988–89',
    desc: "Sacchi's Grande Milan — Gullit, Van Basten, Rijkaard"
  },
  // Add more slides here...
];
```

Other configurable constants:

| Constant         | Default     | Description                      |
| ---------------- | ----------- | -------------------------------- |
| `SLIDE_INTERVAL` | `8000`      | Photo rotation interval in ms    |
| `PARTICLE_COUNT` | `60`        | Default gold particle count      |
| `HONORS`         | Full list   | Honours with SVG icons and years |
| `BADGE_IMAGE`    | `badge.png` | Path to badge file               |

---

## 🎵 Audio Visualization

The wallpaper reacts to **system audio** via Wallpaper Engine's audio API — it does NOT play audio itself.

To see it in action: play any music on your computer. The gold frequency bars at the bottom will pulse with the beat.

For the full Rossoneri experience, play *"Milan Milan"* (the official anthem) 🎶

---

## 🛠 Technical Details

- **Single-file architecture** — All HTML, CSS, JS in one `index.html`
- **Canvas-based particles** — Performant 2D canvas particle system
- **CSS animations** — Glow pulses, stripes, corner ornaments
- **requestAnimationFrame** — Delta-time animations for frame-rate independence
- **FPS limiter** — Wallpaper Engine `applyGeneralProperties` integration
- **Audio API** — `wallpaperRegisterAudioListener` with exponential smoothing
- **Inline SVG trophies** — Hand-crafted, zero dependencies
- **Fully offline** — No CDN, no frameworks, no external requests

---

## 📜 License

The wallpaper code (HTML/CSS/JS) is released under the [MIT License](LICENSE).

AC Milan name, badge, and related imagery are trademarks of **AC Milan S.p.A.** Player photos are subject to their respective copyrights. These assets are **not included** in this repository.

---

## 🤝 Contributing

PRs welcome! Some ideas:

- Additional animation effects (parallax, mouse interaction)
- Alternative color themes (away kit, third kit, retro)
- More configurable Wallpaper Engine properties
- Screenshot contributions for the demo section

---

<p align="center">
  <strong>Forza Milan! 🔴⚫</strong><br>
  <em>Made with ❤️ by a Rossonero</em>
</p>

