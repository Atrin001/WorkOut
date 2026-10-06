# Iron Log

Strength tracker as a static web page: rest timer, plate calculator, weight suggestions, per-exercise swap, JSON import/export. No server or build step.

## Put it on GitHub Pages
1. Create a repo and upload all files in this folder to the repo root: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, `README.md`.
2. Repo **Settings → Pages → Build and deployment**: Source "Deploy from a branch", branch `main`, folder `/ (root)`, Save.
3. Open `https://<your-username>.github.io/<repo-name>/` (takes about a minute the first time).
4. On your phone, use "Add to Home Screen" / "Install app".

## First use
Settings → **Import JSON** → pick your `atrin-performance-coach-export.json`. Sessions are merged (no duplicates by id); you are asked whether to replace the program too.

## Notes
- Data lives in your browser's localStorage on that device only. Use **Export JSON** as a backup.
- Notifications need HTTPS (GitHub Pages provides it) and your permission. They only fire while the app is open or running in the background; a static site cannot push to a fully closed app.
- Weight suggestions are a simple double-progression rule (all sets at the top of the rep range with at least 1 rep in reserve = add the increment). Use your own judgement.
