# Zephyr Automated Solutions — website

Single-page marketing site. Static files, no build step.

## Files
- `index.html` — the whole page (markup, inline styles, and page logic)
- `support.js` — runtime the page loads; keep it alongside index.html
- `assets/` — logo SVGs and favicons

## Running it
Serve the folder over HTTP (opening the file directly with file:// will block the asset loads):

    npx serve .

## Deploying
Push the folder as-is. It works on GitHub Pages, Netlify, Vercel, Cloudflare Pages, or any static host — set the publish directory to this folder.

## Brand
- Magenta `#ff03cf` · Cyan `#03cfff` · Lime `#cfff04` · Navy `#021d50`
- Display: Orbitron · Body: Source Sans 3 (loaded from Google Fonts)

## Notes
- The contact form opens the visitor's email client via `mailto:marketing@zephyrautomation.com`. Point it at a real form endpoint (Formspree, Netlify Forms, your own API) when you're ready.
- Respects `prefers-reduced-motion`: the particle field and logo animations stand down for users who ask for less motion.
