# Little Life — Version 2 starter

A soft-pink, offline-first Progressive Web App starter.

## Included
- `index.html`: the app dashboard and trackers
- `manifest.webmanifest`: install metadata
- `sw.js`: app-shell caching for offline reopening
- `icons/little-life.svg`: app icon

## Important data note
This version stores personal entries in the browser's local storage for the current site origin. The app shell can be cached for offline use once served over HTTPS and opened online at least once. Browser/site data can still be cleared or lost, so use the app's Backup tab regularly. Keep backups somewhere safe.

## Run locally for testing
Service workers generally require HTTPS or `localhost`; opening `index.html` directly as a `file://` URL will not enable the PWA offline cache.
If you have Python installed, open a terminal in this folder and run:
`python -m http.server 8000`
Then visit `http://localhost:8000`.

## Free hosting option
GitHub Pages can host static files from a public repository on the free plan. The website source will be public, so never put personal journal entries or backup files in the repository. Your app data should remain in your browser and backups should be stored privately.
Official docs: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Long-term safety checklist
1. Export a JSON backup weekly.
2. Keep at least two backup copies in separate places.
3. Test restoring a backup occasionally.
4. Keep a copy of this source ZIP.
5. Before using sensitive journal data, remember this prototype has no app lock or encryption.
