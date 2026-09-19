# PKPassport for Mac LP Specification

## Purpose

PKPassport for Mac is a static landing page for a macOS utility that prepares ZIP archives for Windows recipients. The page must remain deployable as repository-root static files with no build step.

## Required sections

The page order and section anchors are:

1. Hero (`#top`)
2. Why (`#why`)
3. Feature Slider (`#features`)
4. Sticky Story (`#how-it-works`)
5. PK Story (`#story`)
6. FAQ (`#faq`)
7. Final CTA

## Required interactions

- Scroll reveal uses `IntersectionObserver` and respects `prefers-reduced-motion`.
- The feature carousel supports horizontal scrolling and previous / next controls.
- Sticky Story keeps the product capture pinned while four chapters update the active screen and status label.
- FAQ uses native `details` elements and keeps only one item open at a time.
- The mobile navigation toggles with the menu button and closes after selecting a link.

## Responsive contract

- Desktop: multi-column hero, Why, PK Story, and sticky product story.
- Tablet/mobile (`820px` and below): mobile navigation, stacked purchase panel, and single-column story layout.
- Narrow mobile (`520px` and below): compact hero composition suitable for approximately `390px` viewport width.

## Asset contract

- `assets/brand/pkpassport-icon.webp` — lime-background app icon.
- `assets/brand/pkpassport-icon-transparent.webp` — transparent-background app icon.
- `assets/hero/pkpassport-flow.webp` — wide Mac-to-Windows concept visual.
- `assets/screens/PKcapture_01.webp` through `PKcapture_04.webp` — optimized captures rendered by the feature and story sections.
- `assets/original/` — original PNG captures and extracted source WebP assets.

Production HTML must reference the files above with relative paths. Base64 image data and Shopify CDN image dependencies are not part of the production contract.
