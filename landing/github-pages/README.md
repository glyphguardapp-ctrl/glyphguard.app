# GlyphGuard GitHub Pages Landing

This folder contains a ready landing page for publishing on **GitHub Pages**.

## Files
- `index.html` — main page with:
  - store buttons (App Store, Google Play, AppGallery)
  - official app icon in hero, favicon, and social preview tags
  - language auto-detect (`en`, `ru`, `es`) + manual switch
  - placeholders for your studio page and donate link
- `icon.png` — official GlyphGuard app icon used by `index.html`

## 1) Replace placeholder links
Open `index.html` and find `STORE_LINKS` block. Replace:

- `YOUR_GOOGLE_PLAY_URL`
- `YOUR_APPGALLERY_URL`
- `YOUR_STUDIO_PAGE_URL`
- `YOUR_DONATE_URL`

## 2) Publish in your GitHub repo `glyphguard.app`
If your repo URL is like:
`https://github.com/glyphguardapp-ctrl/glyphguard.app`

Then your Pages URL will be:
`https://glyphguardapp-ctrl.github.io/glyphguard.app/`

### Minimal publish flow
1. Copy `index.html` and `icon.png` into the root of repo `glyphguard.app`
2. Commit + push to `main`
3. In GitHub repo: `Settings -> Pages`
4. Source: `Deploy from a branch`
5. Branch: `main` and folder: `/ (root)`
6. Save and wait 1-3 minutes

## 3) If URL is different
If GitHub username/repo changes, update URL in app share link accordingly.
Current app share link is set in:
`src/screens/MainAppScreen.js`

## 4) Optional improvements
- Add favicon and Open Graph image
- Add analytics (Plausible/GA)
- Add separate page for all your apps
- Add privacy policy and support links
