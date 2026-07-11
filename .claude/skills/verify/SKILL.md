---
name: verify
description: Build/launch/drive recipe for verifying SkyWheels (single-file three.js game) changes end-to-end.
---

# Verifying SkyWheels

Single-file game: `index.html` + `vendor/three.module.js`, no build step.

## Launch

```bash
python3 -m http.server 8899   # serve from repo root (importmap needs ./vendor/)
```

## Drive (headless Chromium + Playwright)

- `npm install playwright` in a scratch dir, then launch with
  `chromium.launch({ executablePath: '/opt/pw-browsers/chromium' })`
  (installed Playwright version may not match the pre-fetched browser build).
- Tablet emulation: context `{ viewport: {width: 1180, height: 820}, hasTouch: true, isMobile: true }`
  → `(pointer: coarse)` matches → game enters touch mode.
- The touch joystick/buttons listen to Pointer Events; drive them by dispatching
  synthetic `PointerEvent`s (`pointerType: 'touch'`, stable `pointerId`) on
  `#stickArea`, `#lookArea`, `#touchFlyUp/#touchFlyDown/#touchBrake/#touchWalk/#touchUse`.
  `page.touchscreen` has no drag, and `page.tap` can hang while shaders compile —
  fall back to `evaluate(() => btn.click())`.
- Observe via HUD text: `#speedVal` (mph), `#altVal`, `#modeBadge` (DRIVE/FLY/WALK),
  `#hintBar` (toasts). Game state itself is module-scoped, not reachable.

## Gotchas

- Headless uses SwiftShader (~3–10 fps). `frame()` caps dt at 0.1s, so game time
  runs slower than wall time — allow generous holds and loose speed thresholds;
  distances walked/driven will be ~0.3–0.5× the real-hardware value.
- Flying near birds/AI cars can legitimately crash the player (game rule).
  Check `#gameover` visibility and tap `#retryBtn` before continuing a flow.
- Service worker caches aggressively (`sw.js` `CACHE` const). Bump the version
  string on any shipped change or installed tablets keep the old build.
- Fresh browser contexts avoid stale SW/localStorage saves between scenarios
  (a save changes the START button text and spawn state).
