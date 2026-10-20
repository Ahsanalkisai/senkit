# SENKit — SEN Teacher Toolkit

**Tagline:** Tools that make teaching easier.

SENKit is a static, single-page resource hub for SEN teachers. It includes Dhivehi content, interactive activities, resource cards, and theme controls.

## Project files

- `index.html` — the full website and its original interactive JavaScript.
- `assets/Faruma.woff2` — Faruma font in WOFF2 format.
- `assets/Faruma.woff` — Faruma font in WOFF fallback format.

The website references Faruma locally, so both font files must remain in the `assets` folder. The existing Google Fonts link for Noto Sans Thaana and Amiri is retained as a complementary font source.

## Run locally

Open `index.html` in a modern browser. For a local web server, run `python -m http.server 8000` from this folder, then visit `http://localhost:8000`.

## Deploy to GitHub and Vercel

1. Create a GitHub repository named `senkit`.
2. Upload the contents of this folder to the repository root (make sure `index.html` is at the root and `assets/` is beside it).
3. In Vercel, import the GitHub repository.
4. Choose **Other** as the framework preset; no build command is needed for this static HTML project.
5. Set the output directory to `.` if Vercel asks for one, then deploy.

## Notes

- This project uses plain HTML, CSS, and JavaScript; no npm install or build process is required.
- The educational content and existing JavaScript were preserved. The changes made for this package are the SENKit browser title/brand, a proper HTML document wrapper, local Faruma font loading, and a SENKit-specific theme preference key.
