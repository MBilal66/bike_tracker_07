BIKE TRACKER — PWA PACKAGE

Files
- index.html: your supplied Bike Tracker HTML, with PWA metadata and service-worker registration added.
- manifest.webmanifest: install/app display settings.
- sw.js: caches the local app shell for repeat/offline opening.
- icon-192.png and icon-512.png: app icons.

Deploy to GitHub Pages
1. Extract this ZIP.
2. Create or open a GitHub repository.
3. Upload all five files in the repository root (index.html, manifest.webmanifest, sw.js, both icons, plus this README).
4. In Settings → Pages, choose deploy from the main branch and the root folder.
5. Open the published HTTPS URL on your phone. In Chrome, use ⋮ → Add to Home screen / Install app.

Notes
- Keep the app on the same site URL so its local browser data remains available. Existing data stored in another browser or on the Claude artifact does not automatically migrate; use the app's Backup/Restore feature if needed.
- The app loads external Google Fonts and the SheetJS Excel library from CDNs; those functions may need internet access.
- A PWA/service worker does not guarantee GPS tracking with the screen off. The HTML currently advises keeping the page open and screen on during a ride; Android battery and browser restrictions may pause GPS in the background.
- Test the deployed app and make a backup before relying on it.
