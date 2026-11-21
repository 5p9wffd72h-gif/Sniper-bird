# Bird Sniper — iPhone-friendly edition

A free, offline-capable browser game converted from the original Python/Pygame project. This is a Progressive Web App (PWA): publish it to a static HTTPS host, then add it to your iPhone Home Screen from Safari.

## Features
- Mobile touch controls: tap left side or JUMP to jump; hold right side or DUCK to duck
- Desktop keyboard: Space / Up = jump, Down = duck, P = pause
- 20 bird types; a hit changes species
- Endless scrolling, increasing difficulty, aimed bullets and synthesized shot sounds
- High score saved locally on the device
- Offline support after the first visit
- No external assets, analytics, accounts, or network calls from the game

## Test locally
You need Python installed. In this folder run:

```bash
python -m http.server 8000
```
Then open `http://localhost:8000` in your browser. (A server is used because service workers require HTTPS or localhost.)

## Publish free with GitHub Pages
1. Sign in to GitHub and create a **public** repository, e.g. `bird-sniper`.
2. Upload all files from this folder into the repository's root.
3. Open the repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main`, folder `/ (root)`, and Save.
6. Wait for the published link, usually `https://YOUR-USERNAME.github.io/bird-sniper/`.

## Add to iPhone Home Screen
1. Open the published link in **Safari** on your iPhone.
2. Tap **Share**.
3. Scroll and choose **Add to Home Screen**.
4. Enable **Open as Web App** if shown, then tap **Add**.

This installs a Home Screen web-app shortcut that launches in app-like mode. It is not an App Store app. App Store publishing requires Apple's developer program and fees; this PWA route is free.
