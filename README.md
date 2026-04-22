# 🔥 Ember

**Warm up. Loosen up. Feel better.**

A dark-mode stretching app that meets you where the tightness is. Tap any muscle group on an interactive body map and get curated stretches with a guided-session mode that talks you through every step.

**[Play it live](https://ephox1.github.io/Ember-Stretching-App/)**

> ⚠ **For demonstration purposes only.** This is a portfolio project — not medical advice. The exercises are not reviewed by a licensed professional. Consult a doctor or physical therapist before starting any routine. You perform any stretch at your own risk.

---

## How to use

1. Open the app — you'll land on the body map.
2. **Tap any muscle group** (red glow on hover) or toggle between **Back** / **Front** views.
3. Pick a stretch from the list to see full instructions.
4. Hit **Start Guided Session** — the timer, voice coach, and chimes take over from there.
5. Finish the session to build your 🔥 streak.

## Features

- **Interactive body map** — click any muscle group on a white anatomical figure to get stretches that target it
- **Voice coach** — built-in browser speech reads every step aloud (no API keys, no external services)
- **Guided-session timer** — animated progress ring, auto-advancing steps, chime between transitions
- **Haptic feedback** on mobile — subtle vibration when steps change
- **Streak tracking** — localStorage-backed day counter that rewards consistency
- **Favorites** — save the stretches that work for you
- **Body scan** — not sure what's tight? Get a smart recommendation
- **Fully offline** — no server, no tracking, no build step

## Stack

- Vanilla HTML, CSS, JavaScript — single file, no dependencies
- Web Speech API for the voice coach
- Web Audio API for chime sounds
- LocalStorage for streak, favorites, and session history
- SVG body map with positioned hotspots

## Design system

| Token | Value |
|-------|-------|
| Background | `#0d0d0d` |
| Primary | `#ff7a1a` (warm orange) |
| Hotspot gradient | `#b91c1c` → `#f97316` → `#fbbf24` |
| Gentle difficulty | `#22c55e` |
| Moderate difficulty | `#fbbf24` |
| Intense difficulty | `#ef4444` |

## Assets

Drop these files next to `index.html`:

```
body-back.png         # back-view anatomical figure (pure black bg)
body-front.png        # front-view anatomical figure (pure black bg)
stretches/
  neck-side.jpg
  neck-tuck.jpg
  shoulder-cross.jpg
  thread-needle.jpg
  cat-cow.jpg
  thoracic-rotation.jpg
  childs-pose.jpg
  supine-twist.jpg
  pigeon.jpg
  butterfly.jpg
  forward-fold.jpg
  low-lunge.jpg
  chest-doorway.jpg
```

Missing images fall back to a placeholder glyph, so the app works without them.

## Run locally

```bash
git clone https://github.com/Ephox1/Ember-Stretching-App
cd Ember-Stretching-App
# open index.html directly, or:
python -m http.server 8000
# then visit http://localhost:8000
```

## License

[MIT](LICENSE) © Nevin Bruce
