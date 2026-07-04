# Samson Challenge Tracker — PWA

A self-contained installable web app. No build step, no dependencies. Adaptive
strongman-endurance tracker for the JCC Samson Challenge (Masters 50+): logs each
session and prescribes the next from your last performance, with shoulder-pain
gating on all overhead events.

## Files
- `index.html` — the entire app
- `manifest.webmanifest` — home-screen install config
- `sw.js` — offline caching
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` — app icons

## Put it on your phone (GitHub Pages — free)
1. Create a new GitHub repo, e.g. `samson-tracker`.
2. Upload all the files in this folder to the repo root (drag-and-drop in the
   GitHub web UI works, or push with git).
3. Repo **Settings → Pages → Build and deployment**: Source = "Deploy from a
   branch", Branch = `main`, folder = `/root`. Save.
4. Wait ~1 minute. Your app is live at
   `https://<your-username>.github.io/samson-tracker/`.
5. Open that URL on your phone:
   - **iPhone (Safari):** Share → Add to Home Screen.
   - **Android (Chrome):** menu → Install app / Add to Home Screen.
6. Launch it from the new icon — full-screen, works offline.

## Backups (do this occasionally)
Your log lives on the device. In the app: **Settings → Export backup** saves a
`.json` file. **Import backup** restores it — handy when switching phones or if
iOS ever clears site storage. Export after a few sessions and keep the file
somewhere safe (email it to yourself, drop it in cloud storage).

## Notes
- Starting loads are conservative estimates; log honestly and the engine
  calibrates from your real numbers.
- Set your true race date in Settings once you register.
- Overhead progression only advances when the shoulder-pain field is 0. Clear any
  overhead pain with whoever manages your rehab before pushing those events.
