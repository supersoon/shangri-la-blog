# SHANGRI-LA — restored

Faithful static rebuild of the 2006–2007 travel blog *SHANGRI-LA — "poppetsch on tour"*,
originally at `road.supersoon.net` (WordPress + newspaper-10 theme).

Rebuilt from the BackWPup export (`full_backup/…2017-08-07….zip`). Text encoding
(UTF-8-as-Latin-1 mojibake) repaired with ftfy; the original theme CSS is reused
verbatim with a small responsive block appended for phones.

## Contents
- `index.html` — all 42 posts, newest first
- `post-*.html` — individual posts
- `page-*.html` — the 3 pages (supersoon, herr_schaft, their itinerary)
- `category-*.html`, `archive-YYYY-MM.html` — category & monthly archives
- `images/` — all original uploads
- client-side search via `search-index.json`

## View it
    cd site && python3 -m http.server 8000
    # open http://localhost:8000

100% static — host anywhere (Cloudflare Pages, Netlify) or just open locally.
Regenerate with `scratchpad/build.py`.
