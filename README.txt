
Tile Hero — PWA Build
=====================

How to run locally (with install prompt support):
1) Serve the folder over HTTP(S). Opening index.html from a file:// URL won't register the service worker.
2) Quick way: Python 3 -> from this folder run:
   python -m http.server 8080
   Then visit: http://localhost:8080

Deploy options (free, easy):
- GitHub Pages: push this folder into a repo and enable Pages (root).
- Netlify / Vercel: drag-and-drop the folder; no build step needed.

Install to Home Screen:
- iOS (Safari): open the URL, tap Share -> Add to Home Screen.
- Android (Chrome): open the URL; look for "Install app" prompt or use ⋮ -> Install app.

Notes:
- Game saves best score to localStorage; if blocked, it will still run, just without saving best score.
- Service worker caches core files for offline play after first load.
