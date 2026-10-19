# MagAnchor Pro Store

A responsive multi-page storefront built with plain HTML, CSS, and JavaScript. No build step or package dependencies are required.

## Pages and assets
- `index.html` — home / landing page
- `shop.html` — product gallery, pack selector, quantity control, and sticky buy box
- `why.html` — benefits and use cases
- `faq.html` — product, shipping, returns, and support FAQs
- `styles.css` — shared responsive design, wave dividers, hover states, and reduced-motion support
- `app.js` — shared localStorage cart, drawer, variant selection, and gallery controls

## Preview locally
Open `index.html`, or run `python -m http.server 8000` in this folder and visit http://localhost:8000.

## Deploy with GitHub Pages
1. Open repository **Settings → Pages**.
2. Under Build and deployment, choose **GitHub Actions** if a Pages workflow is configured, or select `main` and `/(root)` for branch deployment.
3. Visit the Actions tab to verify the deployment completes.

## Important before accepting orders
- The cart is a front-end demo using browser localStorage. The checkout button intentionally does not take payments yet. Connect a verified Stripe Checkout Session or equivalent backend; a static Payment Link alone will not automatically carry the cart's chosen variant and quantity.
- Confirm product specifications, bundle contents, surface compatibility, pricing, fulfillment, shipping times, tax handling, returns, and privacy policy.
- Replace the support email placeholder in the footer with a monitored inbox.
- The product page includes an Unsplash cable-management photo plus Unsplash desk/workspace photography. These are illustrative editorial photos, not verified photos of the exact MagAnchor Pro item. Replace them with your supplier's actual product images before launch so customers see the item they will receive.
- Do not publish invented testimonials or unverified performance claims.

## Technical notes
The cart state is shared between pages through localStorage. The drawer opens when an item is added, supports quantity changes/removal, and updates the subtotal. Product prices in the front-end are display values only and must be validated by a real checkout backend.
