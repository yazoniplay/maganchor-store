# MagAnchor Pro Store

Responsive single-product storefront built with plain HTML, CSS, and JavaScript. No build step or dependencies are required.

## Preview locally
Open `index.html` in a browser, or run `python -m http.server 8000` in this folder and visit http://localhost:8000.

## Deploy with GitHub Pages
1. Open repository **Settings → Pages**.
2. Under Build and deployment, select **Deploy from a branch**.
3. Select `main` and `/ (root)`, then save.

## Before launch
- Replace `CHECKOUT_URL` in the script in `index.html` with your real Stripe Payment Link.
- Important: this frontend cart does not send item variants or quantities to Stripe. A single Payment Link needs to be configured for the intended product, or replace it with a proper Checkout Session integration to support dynamic cart contents.
- Replace sample review placeholders with real, permissioned customer feedback. They are clearly labeled as illustrative and are not verified testimonials.
- Confirm supplier product specifications, magnet compatibility, packaging, shipping timelines, returns, taxes, contact details, and privacy policy.
- Test checkout and the complete order flow before accepting real orders.

## Included
- Responsive premium-style product landing page, product illustration, benefits, FAQ, and mobile purchase bar.
- 1-pack and 2-pack bundle selector with quantity controls.
- Slide-out cart with quantity editing, removal, subtotal, and localStorage persistence.
- Checkout placeholder guard: payment navigation is intentionally disabled until a valid Stripe Payment Link is added.

## Production limitations
This is a storefront frontend, not a full ecommerce backend. It is not connected to inventory, fulfillment, analytics, or a database.