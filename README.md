# 🎹 Piano — Interactive Browser Piano

A fully functional, playable piano built with pure HTML, CSS, and JavaScript. No frameworks, no dependencies — just one file that works everywhere.

🌐 **[Live Demo → vibecodegames.org/piano](https://www.vibecodegames.org/piano/)**

---

## ✨ Features

- 🎹 **17 keys** — C4 to E5 (white & black keys)
- 🖱️ **Mouse & Touch** — works on desktop and mobile
- ⌨️ **Keyboard support** — physical keyboard layout shown on keys
- 🔊 **4 timbres** — Triangle, Sine, Sawtooth, Square (Web Audio API)
- 🎚️ **Volume control** — smooth slider
- 🌀 **Reverb effect** — via ConvolverNode
- 🎇 **Synthesia mode** — colorful falling notes animation
- 📊 **Oscilloscope** — real-time sound wave visualization
- ⏺️ **Record & Playback** — record your melody with accurate timing
- 💾 **Save to LocalStorage** — keep recordings in the browser
- ⬇️ **Download as JSON** — save recordings to disk
- 📂 **Load from file** — load any previously saved `.json` recording
- 🥁 **Metronome** — adjustable BPM (40–200)
- 🎵 **5 Demo melodies** — Tetris, Happy Birthday, Twinkle Star, Für Elise, Ode to Joy
- 🎯 **Guess the Note** — ear training game with score counter
- 🎓 **Learn Melody** — step-by-step Für Elise tutorial with key highlighting
- 📱 **Fully responsive** — adaptive key size for any screen width

---

## 🎮 Keyboard Layout

| White keys | `A` `S` `D` `F` `G` `H` `J` `K` `L` `;` |
|---|---|
| Black keys | `W` `E` `T` `Y` `U` `O` `P` |

> Keys use `e.code` so they work regardless of your keyboard language layout.

---

## 🚀 Getting Started

No installation needed. Just open the file in any browser:

```bash
git clone https://github.com/YOUR_USERNAME/piano.git
cd piano
# open index.html in your browser
Or simply play it online — no setup required.

📁 Project Structure
text
piano/
└── index.html    # Everything in one file — HTML + CSS + JS
🛠️ Built With
HTML5 — structure

CSS3 — styling, animations, responsive layout

JavaScript (ES6+) — logic, keyboard & touch events

Web Audio API — sound synthesis, reverb, oscilloscope

LocalStorage API — saving recordings in browser

📱 Mobile Support
touchstart events on every key with e.preventDefault() for zero delay

touch-action: manipulation disables double-tap zoom on keys

Adaptive key width: 32px on small screens, 38px on medium, 46px on desktop

Horizontal scroll on the piano keyboard for small screens

Layout rebuilds automatically on device rotation

💾 Recording Format
Recordings are saved as .json files with the following structure:

json
{
  "name": "piano_2026-03-05T11-45-00",
  "notes": [
    { "freq": 261.63, "note": "C4", "t": 0 },
    { "freq": 329.63, "note": "E4", "t": 312 },
    { "freq": 392.00, "note": "G4", "t": 605 }
  ]
}
t is the timestamp in milliseconds from the start of the recording — used for accurate playback timing.

🌐 Deploy
This is a single static file — deploy anywhere for free:

Platform	Command / Method
GitHub Pages	Push to repo → Settings → Pages → main branch
Netlify	Drag & drop index.html into Netlify dashboard
Vercel	vercel --prod
📄 License
MIT License — free to use, modify, and distribute.

👨‍💻 Author
Made with ❤️ by VibecodeGames

🎮 Check out more games and tools at vibecodegames.org
