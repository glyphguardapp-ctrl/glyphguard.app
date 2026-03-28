# GlyphGuard GitHub Pages Landing

This folder contains a ready landing page for publishing on **GitHub Pages**.

## Files
- `index.html` — main page with:
  - store buttons (App Store, Google Play, AppGallery)
  - official app icon in hero, favicon, and social preview tags
  - language auto-detect (`en`, `ru`, `es`) + manual switch
  - GEO/AEO improvements: FAQ, structured product facts, Schema.org JSON-LD
- `icon.png` — official GlyphGuard app icon used by `index.html`
- `llms.txt` — compact map of the most important pages for AI systems
- `robots.txt` and `sitemap.xml` — crawl hints for search engines and indexers

## 1) Replace placeholder links
Open `index.html` and find `STORE_LINKS` block. Replace:

- `YOUR_GOOGLE_PLAY_URL`
- `YOUR_APPGALLERY_URL`
- `YOUR_STUDIO_PAGE_URL`
- `YOUR_DONATE_URL`

Current live URLs already configured in this repo:

- landing: `https://glyphguardapp-ctrl.github.io/glyphguard-landing/`
- privacy policy: `https://glyphguardapp-ctrl.github.io/glyphguard-landing/privacy-policy.html`
- App Store: `https://apps.apple.com/app/glyphguard/id6740001394`
- Google Play: `https://play.google.com/store/apps/details?id=com.glyphguard.offline`

## 2) Publish in your public landing repo
You can publish this landing from any public GitHub Pages repository.

Example:
`https://github.com/your-org/your-landing-repo`

Then your Pages URL will usually be:
`https://your-org.github.io/your-landing-repo/`

### Minimal publish flow
1. Copy landing files into the root of your public landing repo
2. Commit + push to `main`
3. In GitHub repo: `Settings -> Pages`
4. Source: `Deploy from a branch`
5. Branch: `main` and folder: `/ (root)`
6. Save and wait 1-3 minutes

## 3) If URL is different
If the public landing URL changes, update app builds to use the new URL.

Current app share link is configured through:
- env var `EXPO_PUBLIC_LANDING_PAGE_URL`
- fallback helper `src/utils/publicSiteUrl.js`

## 4) Optional improvements
- Add favicon and Open Graph image
- Add analytics (Plausible/GA)
- Add separate page for all your apps
- Add privacy policy and support links
