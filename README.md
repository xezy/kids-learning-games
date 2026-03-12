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

---

## Sharing the Games

Each game is a single HTML file, which makes sharing straightforward. Here are all the options from simplest to most scalable.

### Option 1 — Send the file directly (simplest)
Just send `german-game/index.html` or `math-game/index.html` as an email attachment or via WhatsApp/Telegram. The recipient saves it and double-clicks to open. No internet needed after that.

**Best for:** sharing with a few people you know personally.

---

### Option 2 — Share via Google Drive / Dropbox / OneDrive
1. Upload the HTML file(s) to your cloud storage folder
2. Right-click → **Share** → set to "Anyone with the link can view"
3. Send the link

The recipient downloads the file and opens it locally. They do **not** need a Google/Dropbox account to download.

**Best for:** sharing a download link without hosting anything.

---

### Option 3 — Host on GitHub Pages (free, permanent URL)
This gives you a real URL like `https://yourname.github.io/kids-learning-games/german-game/` that anyone can open directly in their browser — no download required.

```bash
# 1. Push the repo to GitHub (if you haven't already)
git remote add origin https://github.com/yourname/kids-learning-games.git
git push -u origin master

# 2. In GitHub: go to Settings → Pages
#    Source: Deploy from branch → branch: master → folder: / (root)
#    Click Save

# 3. After ~1 minute your games are live at:
#    https://yourname.github.io/kids-learning-games/german-game/
#    https://yourname.github.io/kids-learning-games/math-game/
```

**Best for:** sharing with many people, linking from a message or email, permanent access.

---

### Option 4 — Host on Netlify (free, drag-and-drop, no git required)
1. Go to [netlify.com](https://netlify.com) and sign up free
2. Drag the entire `kids-learning-games` folder onto the Netlify dashboard
3. You instantly get a URL like `https://random-name-123.netlify.app`
4. Optional: rename it to something like `kids-games-yourname.netlify.app` in site settings

```
Your games will be at:
https://your-site-name.netlify.app/german-game/
https://your-site-name.netlify.app/math-game/
```

**Best for:** quickest way to get a shareable URL without using git.

---

### Option 5 — Run a local server on your network (LAN sharing)
Share with people on the same Wi-Fi (e.g. in a classroom or home) without any internet hosting.

```bash
cd kids-learning-games
python3 -m http.server 8080

# Find your local IP address:
# Mac/Linux:  ifconfig | grep "inet "
# Windows:    ipconfig | findstr "IPv4"

# Others on the same Wi-Fi open:
# http://192.168.x.x:8080/german-game/
# http://192.168.x.x:8080/math-game/
```

**Best for:** classroom use, no internet required, works on tablets and phones on the same network.

---

### Quick comparison

| Method | Setup | Needs internet to play | Best for |
|--------|-------|----------------------|----------|
| Email / WhatsApp file | None | No | 1–2 people |
| Cloud drive link | None | No (after download) | Small group |
| GitHub Pages | ~5 min | Yes | Permanent public URL |
| Netlify drag-drop | ~2 min | Yes | Quickest hosted URL |
| Local server | ~1 min | No | Classroom / home Wi-Fi |
