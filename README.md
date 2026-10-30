# TigrushDecor

A demo furniture e-commerce storefront: browse a 100-product catalog, filter it down to exactly what you want, build a cart, and start a multi-step checkout. Every interaction is animated with Motion.

> This is a frontend demo. There's no backend, and no real orders or payments are processed.

## Features

**Shop**
- **100 products across 20 categories**, from sofas and beds to bar stools and wardrobes.
- **Combined filters** that all work together: category, color, material, a price range slider, minimum star rating, availability, and live search by name.
- **Sorting** by price, customer rating or name.
- **Filters that persist.** Your filters, sort order and search are saved, so the shop looks the same when you come back.

**Cart**
- Add and remove items, with animated pill buttons that expand on hover to show details.
- Choose standard (5–7 days) or fast (2–3 days) shipping, and see the subtotal and total update instantly.
- The cart is saved between visits.

**Checkout**
- Three steps: **Address → Billing → Confirmation**, with an animated progress bar that fills as you move through them.
- Contact and shipping address forms.
- Payment by credit card or PayPal, with a form that changes depending on the method.
- The confirmation step is still in progress.

**Design**
- Staggered entrance animations on every page, a hero with a scale-in image, and a navbar that animates between pages.

## Tech stack

| Area | Tools |
|---|---|
| Framework | React 19, TypeScript, Vite |
| Routing | React Router |
| Styling | Tailwind CSS 4 |
| Animation | Motion |
| UI | rc-slider (price range) |
| State | Cookies (js-cookie) for cart and filter persistence |
| Data | Local JSON product catalog |

## Project structure

```
src/
  pages/
    Home.tsx       landing page
    Shop.tsx       catalog, filters, search and sorting
    Cart.tsx       cart, shipping options and totals
    CheckOut.tsx   multi-step checkout with progress bar
    About.tsx
  crossPageComponents/
    NavBar.tsx     animated navigation
  data/json/
    products.json  100-product catalog
```

## Running locally

```bash
npm install
npm run dev
```

Other scripts: `npm run build` (type-check and build), `npm run preview` (serve the build), `npm run lint`.

## Roadmap

- [ ] Confirmation step with an order summary
- [ ] Form validation in checkout
- [ ] Quantities in the cart
- [ ] Product detail pages

## Author

**Tigran Agekyan** · [tigranagekyan.com](https://tigranagekyan.com) · [LinkedIn](https://www.linkedin.com/in/tigran-agekyan)
