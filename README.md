# ✦ NEON HAND

Draw on a glowing canvas using just your hand. No install, no backend — one HTML file.

---

## How it works

Open the file, allow camera access, and point your hand at the screen.

| Gesture | Action |
|---|---|
| ☝️ Index finger up | Draw — your fingertip is the brush |
| 🤏 Pinch thumb + index | Grab mode — pick up and move strokes |
| ✋ Open hand | Idle — nothing happens |

In grab mode the neon cursor disappears and your mouse works normally.

---

## Run it

Camera needs `localhost` or `https` — just spin up a quick server:

```bash
# Python
python -m http.server 8080

# Node
npx serve .
```

Then open `http://localhost:8080/neon-hand-draw.html` in Chrome or Edge.

Or deploy to **GitHub Pages** and get a live HTTPS link for free.

---

## Stack

- [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands) — hand tracking
- One-Euro Filter — removes jitter without adding lag
- Vanilla JS + HTML5 Canvas — no frameworks, no build step

---

> All processing is local. Your camera feed never leaves your device.
