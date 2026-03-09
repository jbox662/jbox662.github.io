# jbox662.github.io

This repo serves the **domain root** for `jbox662.github.io` so Apple can load the Universal Links file for SpendSnap (Plaid OAuth).

- **`.well-known/apple-app-site-association`** – required for iOS to open SpendSnap when the user taps "Open in app" on the Plaid redirect page.
- **`apple-app-site-association`** (root copy) – Apple also checks this path; may be served with better behavior.

**Enable GitHub Pages** (Settings → Pages → Source: main branch, / (root)).

**If the link opens as a download in the browser:** GitHub Pages doesn’t set `Content-Type: application/json` for extensionless files, so the browser may download the file instead of showing it. That’s normal. **Universal Links can still work** – iOS fetches the file with its own request. Reinstall the SpendSnap app and try tapping "Open in app" on the Plaid redirect page; if the app opens, Universal Links are working.
