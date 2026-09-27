# The Milkman — Website

A modern, earthly single-page website for **The Milkman**, a Goa-based Jersey cow milk D2C brand.

Pure static HTML/CSS/JS — no build step, no dependencies. Ready to host on **GitHub Pages**.

**Live contact details baked in:**
- WhatsApp / Call: `+91 77769 50403`
- Email: `vinodpatil.business@gmail.com`
- Location: Goa, India

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire site (nav, hero, story, products, farm gallery, why us, bulk & subscription, testimonials, FAQ, contact, footer) |
| `styles.css` | Earthly cream + leaf-green + terracotta palette, responsive down to mobile |
| `script.js`  | Mobile nav, footer year, scroll fade-ins, WhatsApp form handoff |
| `README.md`  | This file |

## Sections included

1. **Hero** — headline, CTA, live stats
2. **Trust strip** — quick promises
3. **Our Story** — brand narrative
4. **Menu & Rates** — ₹35 / ₹65 / ₹120 / ₹300 cards + delivery note
5. **The Farm** — 6-tile photo gallery of cows & pastures
6. **Why The Milkman** — 4-point value grid
7. **Bulk orders & Monthly Subscription** — 3 tiered plans:
   - Household monthly subscription (10% off + free delivery on route)
   - Café / hotel / sweet-shop wholesale (₹55–₹58/L tiered)
   - One-time event bulk (weddings, functions)
   - Delivery-charge notice
8. **Testimonials**
9. **FAQ** (incl. delivery-charge question)
10. **Contact** — WhatsApp / Call / Email + a form that opens WhatsApp pre-filled

## Hosting on GitHub Pages

The site is already pushed to https://github.com/justPURU/vpatil_milks.

To enable Pages:

1. Open **Settings → Pages** in your repo.
2. Source: **Deploy from a branch**
3. Branch: `main` / `/ (root)`
4. Save.
5. Wait ~1 minute. Site will be live at:
   `https://justpuru.github.io/vpatil_milks/`

### Custom domain (optional)

If you own a domain:

1. In your DNS provider, add these records:
   - `A` records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` → `justpuru.github.io`
2. In GitHub **Settings → Pages → Custom domain**, enter your domain and tick **Enforce HTTPS**.

## Local preview

Open `index.html` in a browser. Or run any static server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Editing rates

Rates live in the **Menu & Rates** section of `index.html` — search for `product-card`. Each card is a small `<article>` block; change the `<h3>`, `.product-price`, and `.product-size` values.

Bulk / subscription rates live in the **Bulk & Subscription** section — search for `plan-card`.

## Notes

- The contact form does **not** send email. It opens WhatsApp with the visitor's message pre-filled — no server, no backend, no data storage. Perfect for GitHub Pages hosting.
- Images are loaded from Unsplash's CDN (hotlinks). Swap the `src=""` attributes for your own farm photos when you have them.
- The site is fully responsive and accessible (semantic HTML, ARIA where needed, respects `prefers-reduced-motion`).
- Fonts (Fraunces + Inter) load from Google Fonts.

---

Made for The Milkman. 🥛
