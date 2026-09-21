# ammielbowen.com (v2.0)

Personal portfolio for Ammiel Bowen. A static site: plain HTML, one CSS file, and a small script for the mobile menu. No build step, no dependencies.

## Structure

```
index.html                  All page content
assets/css/site.css         All styles (colors and fonts are set at the top in :root)
assets/js/site.js           Mobile menu toggle only
assets/fonts/               IBM Plex Sans and Serif, self-hosted (SIL Open Font License)
images/                     Optimized photos and project screenshots (WebP)
resume/                     Professional and school resume PDFs, linked from the nav, hero, and contact section
docs/                       Research and project posters (PDF)
favicon.svg, apple-touch-icon.png, og-image.jpg     Browser icon and link-preview card
CNAME                       Custom domain for GitHub Pages
```

## Updating

- **Text:** edit `index.html`. Each section is marked with a comment.
- **Resumes:** export the PDFs and replace `resume/Ammiel_Bowen_Professional_Resume.pdf` and `resume/Ammiel_Bowen_School_Resume.pdf` (keep the file names so links keep working).
- **Colors:** change the variables at the top of `assets/css/site.css`.
- **New project:** copy an `<article class="project">` block, add a screenshot to `images/projects/` (WebP or PNG), and update the text.

## Deploying (GitHub Pages)

1. Delete the old site's files from the repository (the old template's `assets/sass`, `assets/js`, `assets/webfonts`, `index-demo.html`, and `images/gallery` are no longer used).
2. Copy the contents of this folder into the repository root and commit. Keep `CNAME` so `ammielbowen.com` keeps working.
3. In the repository settings, Pages should serve from the `main` branch root.

## Preview locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000. Open it over http rather than double-clicking `index.html`, so the fonts load the same way they do in production.
