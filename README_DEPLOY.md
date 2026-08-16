# MAIN "Asli atau AI?" — Deploy & Maintenance Notes

**Live:** https://leofire19.github.io/main-game/
**Repo:** https://github.com/leofire19/main-game (GitHub Pages serves the `main` branch root)

One file, zero build step, zero backend. Every push to `main` redeploys the
site automatically within a minute or two.

## Photo rounds

The game unlocks photo rounds when these four files exist next to `index.html`:

```
assets/ai-01.jpg     AI-generated
assets/ai-02.jpg     AI-generated
assets/real-01.jpg   real photograph (license in CREDITS.md)
assets/real-02.jpg   real photograph (license in CREDITS.md)
```

Spec: JPG, max 800px wide, under 300KB each. To swap an image, replace the
file but keep the exact filename, then commit and push. Only use photos you
own or that are freely licensed (update `CREDITS.md` accordingly), never real
public figures or people who haven't consented.

## Test locally

```
python -m http.server 8000
```

then open http://localhost:8000 — or simply open `index.html` in a browser.

## Editing content

All game text and items live in `index.html`: UI strings in the `STR` object
(Indonesian + English), the card deck in the `ITEMS` array. Keep both
languages in sync when editing.
