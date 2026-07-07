# Cyberfrequency Labs — Landing Page

Static landing page for **cyberfrequencylabs.com**, an independent software studio.
Built to satisfy Google Play developer account website verification.

## Files

- `index.html` — the entire site. Single static page, no build step, no dependencies beyond Google Fonts (CDN).
- `car-night.png` — AI-generated hero background (2048×1152). Rear view of an 80s wedge car driving into a cyberpunk city.

## Design

- Direction: "cinematic cyberpunk night drive" — chrome 80s logo over a photoreal night-city image.
- Fonts (Google Fonts): **Orbitron** (900 for the chrome wordmark, 500 for "LABS"), **Chakra Petch** (body/UI).
- Palette: dark navy `#05071c` base, teal `#35e0d0` primary accent, violet `#9a7bff`, pink `#ff4a7a` (reserve accents), body text `#d4daf5`.
- Chrome logo effect: Orbitron 900 with a vertical metallic gradient via `background-clip: text` + drop-shadows.
- Layout: full-viewport flex column (nav / hero / footer), background image `cover`-cropped, top+bottom scrims for text legibility. Responsive via `clamp()`; tested down to mobile widths.

## Contact / links

- Email everywhere: `hello@cyberfrequencylabs.com` (mailto on CONTACT nav link, GET IN TOUCH button, footer).
- Google Play / GitHub buttons were intentionally removed until those URLs exist. To re-add, copy the `.cta` anchor style.

## Deploying

Any static host works (HTTPS + custom domain is all Google Play verification needs):

- **GitHub Pages**: push this folder's contents to a repo root → Settings → Pages → deploy from `main` → set custom domain `cyberfrequencylabs.com` (add a `CNAME` file or use the UI) → point DNS (A records to GitHub Pages IPs, or `www` CNAME).
- **Firebase**: `firebase init hosting` (public dir = this folder), `firebase deploy`.
- **Vercel/Netlify**: drag-and-drop the folder.

## Future ideas (not built)

- Apps/portfolio section once Play Store listings exist
- Re-add Google Play + GitHub buttons
- OG image sized 1200×630 for cleaner link previews
