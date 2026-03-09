# jbox662.github.io

This repo serves the **domain root** for `jbox662.github.io` so Apple can load the Universal Links file for SpendSnap (Plaid OAuth).

- **`.well-known/apple-app-site-association`** – required for iOS to open SpendSnap when the user taps "Open in app" on the Plaid redirect page.

Enable **GitHub Pages** (Settings → Pages → Source: main branch, / (root)) so the file is available at:

`https://jbox662.github.io/.well-known/apple-app-site-association`
