# NDT Study Hub — install guide

This is a Progressive Web App (PWA). Once it's online at a web address, it installs
to a phone's home screen and works offline, with progress that saves permanently.

## Files in this folder (keep them all together)
- index.html               ← the app
- manifest.webmanifest      ← app name, colors, icons
- sw.js                     ← offline support
- icon-192.png / icon-512.png / icon-maskable-512.png
- apple-touch-icon.png / favicon.png

---

## Put it online with GitHub Pages (free, ~5 minutes)

1. Go to github.com and sign in (create a free account if needed).
2. Click the "+" (top right) → "New repository".
3. Name it something like `ndt-study-hub`. Set it to **Public**. Click "Create repository".
4. On the new repo page, click "uploading an existing file".
5. Drag in EVERY file from this folder (index.html, sw.js, manifest.webmanifest,
   and all the .png icons). Click "Commit changes".
6. Go to the repo's **Settings** tab → **Pages** (left sidebar).
7. Under "Build and deployment" → "Source", choose **Deploy from a branch**.
   Set branch to **main** and folder to **/ (root)**. Click **Save**.
8. Wait ~1 minute, then refresh. Pages will show a live URL like:
   `https://YOURNAME.github.io/ndt-study-hub/`

That URL is the app. Share it with Na.

---

## Install on the phone (from that URL)

**iPhone (Safari):**
Open the URL → tap the Share button → "Add to Home Screen" → Add.

**Android (Chrome):**
Open the URL → tap the ⋮ menu → "Install app" (or "Add to Home screen").

It now launches full-screen like a normal app, works offline, and saves progress.

---

## Updating later (adding more decks)
Send new material and I'll extend the app. To publish an update, replace `index.html`
in the repo (Add file → Upload files → drop the new one → Commit). Bump the cache name
in `sw.js` (e.g. `ndt-study-hub-v2`) so phones pick up the change.
