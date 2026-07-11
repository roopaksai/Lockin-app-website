# Lockin-app-website

Landing page for LockIn — a lock screen countdown wallpaper app.

## Structure

```
Lockin-app-website/
├── assets/          (9 files: 1.jpg, 2.jpg, v1.jpg, v2.jpg, normal.jpg, progress.jpg, settings.jpg, widget.jpg, icon.png)
├── index.html       (single-page static site, all CSS/JS inline)
├── vercel.json      (Vercel static site config)
└── README.md
```

## Sections

1. **NAV** — glassmorphism, sticky, logo + BGM toggle (♪) + Download CTA
2. **HERO** — split layout with text + phone comparison slider (v1.jpg ↔ v2.jpg), Three.js 3D dot grid background
3. **FEATURES** — Setup Mode, Progress Mode (asymmetric bento grid rows)
4. **HOW IT WORKS** — 6-step vertical timeline with staggered reveal
5. **CUSTOMIZATION** — standalone section (settings.jpg), two-column grid with badge row
6. **WIDGET SHOWCASE** — widget.jpg centered, feature badges
7. **CTA** — primary download button with pulse animation
8. **FOOTER** — minimal Logo + credit

## Audio

- **BGM** — auto-play epic orchestral loop (Dm → Bb → F → C), synthesized via Web Audio API (kick, rim, hi-hat, bass, string pad, lead). ♪ button toggles stop/start. Respects browser autoplay policy (AudioContext resumed on first interaction).
- **Success chime** — 3-oscillator ascending arpeggio (C5→E5, 0.6s) on download button clicks, also Web Audio API.

## Deploy

[![Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/roopaksai/Lockin-app-website)

Connected to Vercel via GitHub — pushes to `main` auto-deploy.
