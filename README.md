# The Reading Desk - installable app

These files make your reading tracker an installable, offline Android app.
Everything runs on your device; no server code, no accounts.

## Put it online once (free, ~5 minutes, no coding)
1. Sign in at github.com and click "New repository". Name it e.g. `reading-desk`,
   set it Public, and create it.
2. On the repo page: "Add file" -> "Upload files". Drag in ALL of these files
   (index.html, manifest.webmanifest, sw.js, and the four icon PNGs). Commit.
3. Go to Settings -> Pages. Under "Build and deployment", set Source to
   "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
4. Wait about a minute, then open the URL it shows:
   https://YOUR-USERNAME.github.io/reading-desk/

## Install on Android
- Open that URL in Chrome. You'll get an "Install app" prompt (or use the
  menu -> "Install app" / "Add to Home screen"). It installs as a standalone
  app with its own icon, works offline after the first load.

## Your data
- Saves on the device automatically. It is per-device: your phone and desktop
  do NOT sync. Use "Save backup" on one and "Load backup" on the other to move
  a snapshot. Keep a backup before clearing browser data.

## Updating later
- Re-upload a changed index.html and bump the version in sw.js
  (change `reading-desk-v1` to `-v2`) so devices refresh the cached copy.
