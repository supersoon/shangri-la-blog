# SHANGRI-LA — restored

Faithful static rebuild of the 2006–2007 travel blog *SHANGRI-LA — "travel diary of
herr_schaft and supersoon"*, originally at `road.supersoon.net` (WordPress).

Rebuilt from the BackWPup export (`full_backup/…2017-08-07….zip`). The **original
custom 2007 theme** was recovered from the backup's customized `wp-content/themes/
newspaper-10/` templates (style.css v2.0 by supersoon) — a dark charcoal (#484848),
three-column travel-diary design with the "shangri / we're back!" logo, the "ON THE
ROAD AGAIN" banner, grey rounded-corner heading bars and light-blue metadata. The
database's plain black-on-white default was the *degraded* look after a later WP
upgrade; this restores the real design. Text encoding (UTF-8-as-Latin-1 mojibake)
repaired with ftfy; dead 2007 widgets (Plazes, Flickr/Skype badges, PayPal, ShinyStat)
dropped, layout made responsive.

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
