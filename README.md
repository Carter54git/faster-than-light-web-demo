<div align="center">

<img src="ftlicon.png" alt="FTL: Faster Than Light" width="200">

# FTL: Faster Than Light — Browser Demo

**The official FTL demo that runs right in your browser — no installs, no plugins.**

*Save the Federation from the rebels and travel faster than light.*

[![Play now](https://img.shields.io/badge/▶_PLAY_NOW-in_your_browser-e8542a?style=for-the-badge)]([https://USERNAME.github.io/ftldemo/](https://rgc.zone/ports/ftldemo/index.html))

![Emscripten](https://img.shields.io/badge/Emscripten-asm.js-4b8bbe?style=flat-square)
![WebGL](https://img.shields.io/badge/WebGL-990000?style=flat-square&logo=webgl&logoColor=white)
![Build year](https://img.shields.io/badge/build-2014-555?style=flat-square)
![Size](https://img.shields.io/badge/size-~200_MB-555?style=flat-square)
![Developer](https://img.shields.io/badge/by-Subset_Games-2b2b2b?style=flat-square)

</div>

---

## 🚀 About the game

**FTL: Faster Than Light** is a "spaceship simulation roguelike-like" by Subset Games. You command a Federation ship carrying vital data through a randomly generated galaxy, with the rebel fleet hot on your heels. Every jump brings a new encounter, and every decision could be your last.

| | |
|---|---|
| 🧠 **Complex strategic gameplay** | Give orders to your crew, manage ship power distribution and choose weapon targets in the heat of battle. |
| ⏸️ **Play at your own speed** | Pause mid-combat to evaluate your strategy and give orders. |
| 👽 **Unique lifeforms and technology** | Upgrade your ship and unlock new ones with the help of diverse alien races. |
| 📜 **Be the captain you want** | Hundreds of text-based encounters force you to make tough decisions. |
| 🌌 **Randomized galaxy** | Different enemies, events and outcomes every run — no two playthroughs are the same. |
| 💀 **No second chances** | Permadeath: when you die, there's no coming back. |

## 🕹️ About this build

This is the browser demo released by Humble Bundle together with Mozilla in October 2014: the original C++ game compiled to **asm.js** with **Emscripten**. It runs in any modern browser with WebGL support.

- 🎵 34 soundtrack tracks by **Ben Prunty** in OGG format
- 🖥️ Fullscreen mode with proper scaling
- 🔒 Demo mode: once the trial section ends, the game offers to buy the full version

## ▶️ How to play

### Online

Just open **[USERNAME.github.io/ftldemo](https://rgc.zone/ports/ftldemo/index.html)**.

### Locally

The game loads its data via XHR, so opening `index.html` directly from disk (`file://`) won't work — you need any local web server:

```bash
git clone https://github.com/USERNAME/ftldemo.git
cd ftldemo
python -m http.server 8000
```

Then open <http://localhost:8000> in your browser.

### Host your own copy on GitHub Pages

1. Fork this repository.
2. Go to **Settings → Pages → Source:** `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. After a couple of minutes the game will be live at `https://<your-username>.github.io/ftldemo/`.

## 📁 Project structure

```
ftldemo/
├── index.html                    # player page
├── FTL-1413323248.js             # game engine (asm.js)
├── FTL-1413323248.js.mem         # initial memory image
├── FTL-1413323248.data           # graphics and game data (~54 MB)
├── FTL-audio-1413323248.data     # sound effects (~12 MB)
├── music/                        # soundtrack, 34 × .ogg (~130 MB)
├── main.min.js, 19d6f4….js       # Humble loader and player
├── *.css, *.woff2, *.svg, *.png  # UI styles, fonts and icons
└── ftlicon.png                   # icon
```

## 💻 Requirements

- A browser with WebGL support: Chrome, Firefox, Edge or Safari (recent versions)
- ~200 MB download on first launch
- Mouse and keyboard

## ⚖️ Legal

**FTL: Faster Than Light** © [Subset Games](https://subsetgames.com/). All rights to the game, artwork, music and trademarks belong to their respective owners. The browser demo was distributed for free by Humble Bundle.

This repository is not affiliated with or endorsed by Subset Games or Humble Bundle. If you enjoy the game, please support the developers and buy the full **FTL: Advanced Edition**:

<div align="center">

[![Steam](https://img.shields.io/badge/Steam-buy-1b2838?style=for-the-badge&logo=steam&logoColor=white)](https://store.steampowered.com/app/212680/)
[![GOG](https://img.shields.io/badge/GOG-buy-86328a?style=for-the-badge&logo=gogdotcom&logoColor=white)](https://www.gog.com/game/faster_than_light)
[![Humble](https://img.shields.io/badge/Humble-buy-cc2929?style=for-the-badge&logo=humblebundle&logoColor=white)](https://www.humblebundle.com/store/ftlfasterthanlight)

<sub>Made with ❤️ for space captains everywhere</sub>

</div>
