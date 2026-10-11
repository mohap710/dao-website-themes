# DAO Website Themes

Design previews for the new **Depth Action Organization (منظمة الأثر العميق)** website.

The landing page lists every theme with a screenshot, a live preview (desktop / tablet / phone), a comparison table, and a **Select this theme** button that gives you a link to share your choice.

| # | Theme | Mood |
|---|-------|------|
| 01 | [Architectural Light](theme1/) | Clean, bold, confident |
| 02 | [Bento Dashboard](theme2/) | Modern, data-driven, interactive |
| 03 | [Field Stories](theme3/) | Warm, human, editorial |

## Structure

```
index.html            landing page (plain HTML/CSS/JS, no build step)
assets/previews/      screenshots shown on the landing page
theme1/ theme2/ theme3/   one self-contained index.html per theme
.nojekyll             tells GitHub Pages to serve files as they are
```

Each theme is a single `index.html`. The themes load Tailwind CSS, Alpine.js, Lucide icons and photos from public CDNs, so previews need an internet connection.

## Run locally

Any static server works:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Add or change a theme

1. Create `themeN/index.html`.
2. Add a screenshot at `assets/previews/themeN.jpg` (1200×750).
3. Copy one of the `<article class="card">` blocks in `index.html`, and update its `data-theme`, name, text and links.

## Publishing (GitHub Pages)

Repository **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`**.

## Content and photo notes

Numbers, quotes and partner names in the themes are placeholders. Photos are free-licence images from [Unsplash](https://unsplash.com/license), credited on each page and used for illustration only; replace them with DAO's own photography before launch.
