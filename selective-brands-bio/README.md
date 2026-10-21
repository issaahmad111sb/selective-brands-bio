# Selective Brands — Link in Bio

Single-page, mobile-first "link in bio" landing page for Selective Brands (cosmetics distributor, Iraq).

## Files

- `index.html` — the complete self-contained page (inline CSS/JS, company logo embedded as base64)
- `logos/` — brand logo images referenced by the page (must be uploaded next to `index.html`)

## Editing

- All links, card colors (`bg`/`fg`) live in the `LINKS` config at the top of the `<script>` block in `index.html`.
- Brand card button labels are generated automatically as "اشتري " + brand name.
- Brand URLs get UTM parameters appended automatically (`utm_source=tiktok&utm_medium=bio&utm_campaign=linkinbio`); social links are left untouched.
- Click tracking is handled by Umami via `data-umami-event` attributes — no extra code needed.

## Deploy

Upload `index.html` and the `logos/` folder together to any static host (Netlify, Vercel, GitHub Pages…). No build step required.
