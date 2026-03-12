# Kids Learning Games 🎮

Two standalone HTML5 games for children. No build step, no dependencies, no server required — just open the HTML file in any browser.

## Games

### 🦊 Deutsch Abenteuer — German Language
`german-game/index.html`

Learn German vocabulary across 10 themed levels (Animals, Food, Nature, Home, Transport, Body, Clothes, Colours, School, Adventure).

**Exercise modes:**
- 🖼️ **Picture Match** — see a picture, pick the German word
- 👂 **Listen & Type** — hear the word, type it out
- 🔀 **Mixed** — both types alternating

---

### 🦁 Math Adventure — Numbers & Maths
`math-game/index.html`

Progressive maths practice across 10 levels per mode.

**Exercise modes:**
- 🔢 **Count & Match** — count objects and match numbers to groups (levels scale from 1–3 up to groups of 10)
- ➕ **Calculations** — addition, subtraction, missing numbers, times tables
- ➡️ **Sequences** — complete number patterns (forwards, backwards, skip counting)
- 🔀 **Mixed** — all types together

---

## Features
- ⭐ Star ratings (1–3) per level per mode
- 🔒 Level unlock progression
- 🔊 Text-to-speech audio (browser built-in, works offline)
- 🗑️ Per-mode progress reset
- 🎉 Confetti & sparkle animations
- 💾 Progress saved to sessionStorage
- 📱 Mobile-friendly responsive layout
- ✈️ Fully offline — no internet needed after first load (fonts cache automatically)

## Usage

```bash
# Just open in a browser
open german-game/index.html
open math-game/index.html

# Or serve locally for best font caching
python3 -m http.server 8080
# then visit http://localhost:8080/german-game/
```

## Structure

```
kids-learning-games/
├── README.md
├── german-game/
│   └── index.html        # Complete self-contained game (~45KB)
└── math-game/
    └── index.html        # Complete self-contained game (~50KB)
```

Each game is a **single self-contained HTML file** — all CSS, JS, and game data are inline. No build tools, no npm, no framework dependencies.

## Browser Support
Works in any modern browser: Chrome, Firefox, Safari, Edge. Text-to-speech quality varies by OS and browser.
