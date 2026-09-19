# A Prayer Book — installable app

Six files. Two ways to get a real app on your phone.

## Route 1 — Install as an app (5 minutes, free, no developer account)

1. Create a free GitHub account if you don't have one.
2. Make a new **public** repository, e.g. `prayer-book`.
3. Upload all six files (index.html, manifest.json, sw.js, icon-192.png, icon-512.png, icon-180.png) to the root of the repo.
4. Repo **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
5. Wait a minute, then open the URL it gives you (`https://<your-name>.github.io/prayer-book/`) in Chrome on your phone.
6. Chrome will offer **"Install app"** (three dots → Install app). Not "Add to Home screen" — the real one.

What you get: its own icon in the app drawer, opens full-screen with no address bar, appears in the recent-apps switcher, and works offline once opened.

## Route 2 — A real APK you can sideload

Do Route 1 first, then:

1. Go to **pwabuilder.com** on a computer.
2. Paste your GitHub Pages URL.
3. Choose **Android → Generate Package**.
4. Download the zip, put the `.apk` on your phone, open it, allow install from unknown sources.

This produces a genuine signed Android package. It is not on the Play Store, so Android will warn you before installing.

## Why not a plain .apk from the start?

Building an APK needs the Android SDK and Google's build tools, which aren't reachable from where this was made. PWABuilder does that step for you.
