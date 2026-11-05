# Sergej Braznikov — personal website

One-page personal site: profile, focus areas, experience and contact.

Plain HTML and CSS in a single file. No build step and no external dependencies. The Inter Tight font is self-hosted, and analytics run on Plausible (cookieless). The page supports light and dark mode and is responsive.

## Structure

```
index.html                   the whole page (markup + styles)
assets/sergej-braznikov.jpg  portrait
assets/icon.svg              favicon
assets/apple-touch-icon.png  home screen icon
assets/og-image.jpg          link preview image (1200×630)
assets/fonts/                Inter Tight, self-hosted (SIL OFL)
```

## Local preview

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

## Editing

All content and styles live in `index.html`. Colours are CSS variables in `:root`, and the dark theme overrides them in the `prefers-color-scheme: dark` block.

## Deploy

Any static host works: GitHub Pages, Netlify, Cloudflare Pages. Publish the repository root as is.
