# 🌊 Wave Art — Interactive Generative Canvas
**VishwaNova 2026 · National Level Weboreel AI Hackathon**

*Move your hand. Watch the ocean respond.*
A meditative, mouse-driven generative art experience where 80+ animated sine waves breathe, bend, and bloom in real time around your cursor — every movement a brushstroke, every second a new painting.

---

## ✨ Features

**🎨 80-Wave Sine Engine:** Eighty independent sine waves are rendered every frame across the full canvas, each with its own amplitude, frequency, and phase offset. Mouse X and Y coordinates are mapped directly to wave amplitude and frequency — moving slowly creates gentle rolling hills, moving fast creates chaotic interference patterns.

**🌈 Continuous Hue Rotation:** Wave stroke colors cycle through a full 360° hue rotation over time via an incrementing HSL value — no two seconds share the same palette. Color mode toggles let users lock into Rainbow, Monochrome, Sunset, or Ocean themes, each constraining the hue range to its mood.

**💫 Cursor Ripple Distortion:** Waves within a 150px radius of the mouse cursor are locally distorted — their phase is pushed outward like a physical ripple in water, creating the sensation that your cursor is an object pressing into a liquid surface.

**🖼️ Trail Fade Persistence:** Each frame is not fully cleared — instead a semi-transparent dark overlay is painted first, causing old wave positions to linger as fading trails. Fast movement leaves bold streaked arcs; stillness lets the canvas breathe into soft glowing lines.

**🎛️ Live Control Panel:** A minimal floating panel houses a Speed slider (controls animation tick rate), a Wave Count slider (20–120 waves), a Color Mode toggle, and a Download PNG button — all updating the canvas in real time without interruption.

**💾 One-Click PNG Export:** The current canvas frame is captured via `canvas.toDataURL()` and silently downloaded as a timestamped PNG — saving whatever accidental masterpiece just appeared on screen.

---

## 🛠️ Tech Stack

**HTML5 Canvas** — Full-screen 2D rendering context, `toDataURL()` PNG export.
**Vanilla CSS3** — Floating glassmorphism control panel, smooth hover transitions, dark backdrop.
**Vanilla JavaScript** — `requestAnimationFrame` render loop, sine wave math per-pixel, mouse event tracking, HSL color cycling, local ripple distortion algorithm.
**Web Audio API** — Subtle ambient drone (layered sine oscillators) that shifts pitch gently with wave density — the canvas breathes sound as well as light.

---

## 📸 Try It Out

Simply double-click the `index.html` file to open it in any modern browser. No servers, build steps, or dependencies required.

---

*Built with 🌊 for VishwaNova 2026*
