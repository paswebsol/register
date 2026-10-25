SCHOOL REGISTER — GITHUB PAGES INSTALL PACKAGE

CONTENTS
- index.html: client app and visible FULL INSTALL APP controls
- manifest.webmanifest: PWA install metadata
- sw.js: service worker for app-shell caching/offline launch
- icons/: app icons for installation

DEPLOY TO GITHUB PAGES
1. Create a GitHub repository (for example: school-register-client).
2. Upload ALL files and folders in this package to the repository root. Do not upload only index.html.
3. In repository Settings > Pages, choose Deploy from a branch, select the main branch and /(root), then Save.
4. Wait for GitHub Pages to publish the site. Use the HTTPS URL it provides.
5. Open that HTTPS link in Chrome/Edge on desktop or a supported mobile browser. The page displays FULL INSTALL APP / INSTALL APP.

INSTALL ON DEVICES
- Android: Chrome generally shows an install prompt; if not, use browser menu (⋮) > Install app or Add to Home screen.
- Windows/macOS/Linux: Chrome or Edge, use the install icon in the address bar or browser menu > Install app.
- iPhone/iPad: open the HTTPS site in Safari > Share > Add to Home Screen. iOS may not show a native web install prompt, so the page explains the manual steps.

IMPORTANT LIMITATIONS
- PWA installation requires HTTPS (GitHub Pages provides HTTPS) or localhost for development. Installation options vary by browser and OS; no website can force installation without the user's approval.
- The service worker caches the app shell so the app can launch offline after the first successful online visit. Any external resources/features still requiring a network may not work offline.
- This is still a browser-installed web app, not a signed native APK/EXE. For native store installation, separate platform-specific builds are needed.
- One-device licensing uses browser storage. Clearing browser/site data or using a different browser/profile may change the generated Device ID and may require issuing a replacement license.
- Keep your private License Issuer separate. Do not upload the issuer or signing private key to the public GitHub repository.
