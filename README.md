# Ven_ Entertainment

A free + legal entertainment dashboard for laptops, built as a single-file
web app with live previews. It organizes 50 curated services across
10 categories: **Movies, TV, Music, Podcasts, Books, Games, Documentaries,
Learning, Live TV & News, Anime & Kids**.

Features:
- **App shell** — sidebar navigation with per-category counts.
- **Live preview** — click any tile to open the service embedded in a
  preview pane (with an open-in-new-tab fallback for sites that block
  embedding).
- **Search** — press `/` and filter every platform by name, tag, or
  description.
- **Favorites** — star platforms into a persistent Favorites shelf
  (stored in localStorage), with **export/import as JSON** to back up
  or share your list.
- **Recently Viewed** — the last 8 platforms you previewed, one click away.
- **Sort** — toggle any view between curated order and A–Z.
- **Light / dark theme**, persisted across visits.
- **Keyboard navigation** — arrow keys move between tiles, `/` jumps to
  search, `Esc` closes the preview.
- **Copy link** — grab a platform's URL straight from the preview pane.
- **Surprise me** — opens a random platform from the current view.
- Every platform includes **what it's best for** and a **"premium move"**
  tip for using the free tier like a paid service.

## Deploy to Railway

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/new/template?template=https%3A%2F%2Fgithub.com%2Farihov%2Fentertainment)

The repo is pre-configured for Railway (`railway.json` + `package.json`):
Nixpacks detects Node, installs [`serve`](https://www.npmjs.com/package/serve),
and `npm start` binds it to Railway's injected `$PORT`.

1. Click the button above (or go to [railway.com/new](https://railway.com/new)
   → **Deploy from GitHub repo** → pick `arihov/entertainment`).
2. After the first deploy, open the service → **Settings → Networking →
   Generate Domain** to get your public `*.up.railway.app` URL.
3. Every push to the default branch auto-redeploys.

## Run it

Either open `index.html` directly in a browser, or serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Files

- `index.html` — the entire dashboard (no build step, no dependencies).
