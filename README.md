# Ward Round Dashboard (PWA)

Installable, offline-capable clinical nutrition ward-round tool.

- **App URL:** https://iashahussain.github.io/rounds-dashboard/
- **Install (Android Chrome):** open the URL → Chrome menu (⋮) → **Add to Home screen / Install app**.
- Works offline after the first load.

## Privacy

- The app is **100% client-side**. There is **no server and no backend.**
- **No patient data is ever sent anywhere.** All data lives only in the browser's
  local storage on the device that entered it. Nothing in this repository contains
  patient data — only the blank application.

## How it's built / deployed

- `index.html` is a copy of the single-file master kept alongside this repo
  (`TTH_Ward_Round_Dashboard-NN.html`, highest number = latest).
- `sw.js` caches the app shell + font for offline use (bump `CACHE` on each deploy).
- `manifest.webmanifest` + `icon-*.png` make it installable.

**To redeploy after editing the master:** copy the latest `TTH_Ward_Round_Dashboard-NN.html`
over `index.html`, bump the `CACHE` version in `sw.js`, then commit & push.
