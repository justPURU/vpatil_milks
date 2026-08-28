# VPATIL Milks — Website

A modern, earthly single-page website for **VPATIL Milks**, a Goa-based Jersey cow milk D2C brand.

Pure static HTML/CSS/JS — no build step, no dependencies. Ready to host on **GitHub Pages**.

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire site (nav, hero, story, products, farm gallery, why us, testimonials, FAQ, contact, footer) |
| `styles.css` | Earthly cream + leaf + terracotta palette, responsive down to mobile |
| `script.js`  | Mobile nav, footer year, scroll fade-ins, WhatsApp form handoff |
| `README.md`  | This file |

## Before you publish — replace these placeholders

Open the files and search-replace these values:

| Placeholder | Where | Replace with |
|---|---|---|
| `hello@vpatilmilks.com` | `index.html` (3 places) | your real business email |
| `919800000000` | `index.html` (2 links) + `script.js` (`WHATSAPP_NUMBER`) | your WhatsApp number in international format, no `+` or spaces (e.g. `919812345678`) |
| `+91 98XXXXXXXX` | `index.html` (2 places, visible text) | the same number formatted for humans |

All images are loaded from **Unsplash** (free hotlinks). If you'd rather use your own farm photos, drop them into an `images/` folder and swap the `src=""` attributes in `index.html`.

## Hosting on GitHub Pages

1. **Create a new GitHub repo**, e.g. `vpatil-milks`.
2. **Upload these files** (or `git push` them) to the `main` branch. They must sit at the repo root.
3. In GitHub: **Settings → Pages**
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`
   - Save.
4. Wait ~1 minute. Your site will be live at:
   `https://<your-username>.github.io/vpatil-milks/`

### Custom domain (optional)

If you own `vpatilmilks.com`:

1. In your DNS provider, add these records:
   - `A` records for `@` pointing to GitHub Pages IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` → `<your-username>.github.io`
2. In GitHub **Settings → Pages → Custom domain**, enter `vpatilmilks.com` and tick **Enforce HTTPS**.
3. GitHub will create a `CNAME` file in the repo automatically.

## Local preview

Just open `index.html` in a browser. Or run any static server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Editing rates

Prices live in the **Products / Rates** section of `index.html` — search for `product-card`. Each card is a small `<article>` block; change the `<h3>`, `.product-price`, and `.product-size` values.

## Notes

- The contact form does **not** send email. It opens WhatsApp with the visitor's message pre-filled — no server, no backend, no data storage. This is perfect for GitHub Pages hosting.
- The site is fully responsive and accessible (semantic HTML, ARIA where needed, respects `prefers-reduced-motion`).
- Fonts (Fraunces + Inter) load from Google Fonts.

---

Made for the VPATIL family. 🥛
