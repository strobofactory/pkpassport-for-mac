# PKPassport for Mac — Landing Page

Static HTML / CSS / JavaScript landing page for PKPassport for Mac.

## Current status
- LP v0.2 implementation complete
- Hero / Why / Feature carousel / Sticky product story / PK story / FAQ / Final CTA implemented
- Responsive CSS and `prefers-reduced-motion` support included
- SEO meta, canonical, Open Graph/Twitter metadata, SoftwareApplication JSON-LD, favicon, robots.txt and sitemap.xml included
- Purchase CTA points to the existing STROBOFACTORY product page
- GitHub → Vercel production deployment connected and verified on 2026-09-19

## Deployment target
- GitHub repository: `strobofactory/pkpassport-for-mac`
- Vercel project: `pkpassport-for-mac`
- Framework preset: `Other`
- Build command: none
- Root directory: repository root
- Production branch: `main`
- Intended production domain: `https://pkpassport.strobofactory.net`

## Product page
https://strobofactory.net/products/pkpassport-for-mac

## Asset layout

- `assets/brand/` — production app icons
- `assets/hero/` — production hero / flow visual
- `assets/screens/` — optimized WebP product captures used by the LP
- `assets/original/` — source images retained for future export work

All images rendered by `index.html` are local files. The four product captures no longer depend on the Shopify CDN, and the previously embedded Base64 images have been extracted to `assets/`.

See `docs/LP_SPEC.md` for the section and interaction contract, and `docs/DEPLOYMENT.md` for the publishing flow.

## Publishing flow
`main` push → Vercel production deployment → `https://pkpassport-for-mac.vercel.app/`

The existing `pkpassport-license` repository / Vercel project is a separate license service and must not be modified for this LP.
