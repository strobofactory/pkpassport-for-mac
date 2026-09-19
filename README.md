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

## Current screenshot sources
The first implementation uses the existing STROBOFACTORY Shopify CDN screenshots so the LP can be reviewed before final asset packaging:

- `PKcapture_01.png` — Drop
- `PKcapture_02.png` — Create
- `PKcapture_03.png` — Destination / settings
- `PKcapture_04.png` — Windows Preview

Before final production lock, copy these screenshots into `assets/screens/`, optimize them for web, and change the HTML references to local paths. This avoids coupling the standalone LP to Shopify CDN asset URLs.

## Publishing flow
`main` push → Vercel production deployment → `pkpassport.strobofactory.net`

The existing `pkpassport-license` repository / Vercel project is a separate license service and must not be modified for this LP.
