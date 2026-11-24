# V4.4.2 QA Report

Date: 2026-11-24
Scope: Single Hero main image replacement only.

## Change boundary
- Replaced only `hero-main.webp` as the visible website asset.
- Kept the separate overlapping fabric-sample image (`hero-detail.webp`) and its page overlay unchanged.
- Kept “QUALITY COORDINATION” and “GLOBAL TRADE” as live website text in `module-hero.js`; neither phrase is embedded in the new Hero image.
- No website copy, page markup, CSS, navigation, product images, Admin logic, or other functionality changed.

## Validation
- Hero image: WebP, 900 × 900, successfully decoded.
- Node.js syntax, JSON parsing, asset references, page section mappings, product image mappings, CSS brace balance and Admin boundary checked with `node qa-check.mjs`.
- Public package contains no `admin/` directory.
- ZIP archive integrity checked after packaging.

## Not certified
- Pixel-perfect rendering across every browser, device and zoom level was not certified by automated Chromium testing.
- Live hosting, DNS, HTTPS configuration and email delivery were not tested.
