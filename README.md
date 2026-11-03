# Egrisi — egrisi.ge

Website for **Egrisi (ეგრისი)**, a Megrelian restaurant with a garden near Senaki, Georgia.
Static site, no build step: open `index.html` in a browser or serve the folder from any static host.

## Pages

| Language | Path |
|---|---|
| Georgian (default) | `/index.html` |
| English | `/en/index.html` |
| Russian | `/ru/index.html` |

## Structure

```
index.html          Georgian page
en/index.html       English page
ru/index.html       Russian page
styles.css          All styles (shared by the three pages)
favicon.svg
images/             Hero, dish and about photos
images/menu/        Menu thumbnails
robots.txt, sitemap.xml
```

## Sections

Hero with live open/closed status · About · Dishes · Menu (cold dishes, hot dishes, breads, sauces, with prices in GEL) · Google reviews · Visit (hours, phone, map).

## Before launch

- Remove the draft banner (`<div class="draft …">`) from all three pages once the restaurant approves the site.
- **Google reviews:** the reviews section shows live Google reviews once a Google Maps Platform API key
  (Places API (New), restricted to the site's domain) is set in `var KEY = ""` inside each page.
  Without a key it shows the "Write a review" and "Read all reviews on Google" buttons only.
- Have a native speaker proofread the Georgian and Russian text, and confirm menu prices with the restaurant.

## Hosting

Works on GitHub Pages (Settings → Pages → deploy from the `main` branch, root folder), Netlify or Cloudflare Pages.
The canonical and sitemap URLs point to `https://egrisi.ge/`.
