# Ven_ Entertainment

A free + legal entertainment dashboard for laptops, built as a single-file
web app with live previews. It organizes 40 curated services across
8 categories: **Movies, TV, Music, Podcasts, Books, Games, Documentaries,
Learning**.

Features:
- **App shell** — sidebar navigation with per-category counts.
- **Live preview** — click any tile to open the service embedded in a
  preview pane (with an open-in-new-tab fallback for sites that block
  embedding).
- **Search** — press `/` and filter all 40 platforms by name, tag, or
  description.
- **Favorites** — star platforms into a persistent Favorites shelf
  (stored in localStorage).
- **Surprise me** — opens a random platform from the current view.
- Every platform includes **what it's best for** and a **"premium move"**
  tip for using the free tier like a paid service.

## Run it

Either open `index.html` directly in a browser, or serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Files

- `index.html` — the entire dashboard (no build step, no dependencies).
