# Óðrerir — the Live Hall

The Ymir fleet's planning glass, on its own deck. A static Astro site
(alpine-cold: a carved `src/index.html` served verbatim) that paints the
fleet's live planning snapshot — one page, one candle, no wandering halls.

Part of the [Ymir](https://github.com/zerwiz/ymir) project. Norse name for the
mead of poetry: the lore is stored in the cauldron, and here it is served.

## What it is

- **The Live Hall board** — the fleet's planning snapshot as a single glass:
  agents, tasks, and the road ahead, read from `livehall.json`
  (written by the Ymir tree's `bin/hall-snapshot.sh` into this repo's
  `public/`; absent, the page paints the saga's own tale and says so).
- **Own origin, own port** — serves on `:4322` (the landing keeps `:4321`).
- **Cloth** — `src/styles/cloth.css` (tokens extracted from the landing's
  `:root`) and `src/styles/livehall.css` (the board kit).

## Run

```bash
npm install
npm run dev        # astro dev, :4322
npm run build      # static build to dist/
npm run preview
```

## Licence

Apache License, Version 2.0 — see `LICENSE` and `NOTICE`.