# Nutritrack — Nutrition Tracker

A lightweight, offline-first Progressive Web App (PWA) for tracking meals, monitoring daily nutrition, setting goals, and discovering recipes. See your daily intake at a glance.

**Live app:** https://nutritrack-5wk.pages.dev

---

## Features

- **Food log** — record every meal with calories and macros
- **Daily dashboard** — see your nutrition summary at a glance
- **Goal tracking** — set and monitor daily nutrition targets
- **Recipe suggestions** — discover meals that fit your goals
- **Offline support** — works fully without an internet connection (service worker)
- **Installable** — install to your home screen on Android or iOS
- **Dark mode** — follows your system preference
- **No account needed** — all data stays on your device

---

## Tech stack

- Single HTML file — no build step, no dependencies, no framework
- Vanilla JS + CSS
- PWA (Web App Manifest + Service Worker)
- Data stored in `localStorage`

---

## Project structure

```
Nutritrack/
├── index.html       # The entire app
├── sw.js            # Service worker (offline caching)
├── manifest.json    # PWA metadata (name, icons, shortcuts)
├── privacy.html     # Privacy policy page
├── _headers         # Cloudflare Pages HTTP headers config
├── _redirects       # Cloudflare Pages redirect rules
├── robots.txt
├── sitemap.xml
├── icons/           # App icons (72px – 512px)
└── screenshots/     # dashboard, log, goals, recipes, today pages
```

---

## Deployment

The app is hosted on **Cloudflare Pages** and deploys automatically when changes are pushed to the `main` branch.

To make a change:
1. Edit the files locally (or directly on GitHub)
2. Commit and push to `main`
3. Cloudflare Pages picks up the change and redeploys in ~30 seconds

---

## Running locally

No build step needed — just open `index.html` in a browser, or serve the folder with any static server:

```bash
npx serve .
# or
python3 -m http.server 8080
```

---

## License

MIT
