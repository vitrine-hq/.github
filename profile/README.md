<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/vitrine-hq/.github/main/profile/assets/vitrine-mark-white.png">
    <img src="https://raw.githubusercontent.com/vitrine-hq/.github/main/profile/assets/vitrine-mark-teal.png" alt="Vitrine logo" width="96">
  </picture>
</p>

<h1 align="center">Vitrine</h1>

<p align="center">
  <strong>Online catalogs with WhatsApp checkout for jewelry and accessory stores, synced with Bling ERP.</strong>
</p>

## Why Vitrine

Small jewelry and accessory stores sell mostly through Instagram and WhatsApp. Keeping an online catalog in step with the ERP is manual work: stock drifts, photos go missing, and customers message the store asking for pieces that are already sold out.

Vitrine keeps the catalog in sync with the store's ERP automatically and turns a shopping bag into a ready-to-send WhatsApp message, so a customer can go from browsing to ordering in about a minute.

## How it works

1. **Sync.** Products, variants, stock and photos come from Bling ERP in near real time.
2. **Curate.** The store decides what appears: only pieces with photos, only items in stock, selected categories, featured products.
3. **Browse.** Customers explore a fast, mobile-first catalog in Portuguese or English and add pieces to their bag.
4. **Order.** Checkout opens WhatsApp with the complete order, and the store follows it up in the admin dashboard.

## Highlights

- Mobile-first storefront, installable as a web app
- Real-time updates from Bling ERP through webhooks, with scheduled reconciliation as a safety net
- Visibility rules with a clear explanation of why each product is shown or hidden
- Batch photo import from local files, ZIP archives or a shared Google Drive folder
- Portuguese (Brazil) and English from day one
- API-first backend, ready for a future native app

## Repositories

| Repository | What it is | Visibility |
|---|---|---|
| `vitrine-api` | Backend API and worker: ERP sync, catalog publishing, image processing and orders | Private |
| `vitrine-web` | Storefront and merchant admin, multilingual and responsive | Private |

## Built with

Python, FastAPI and PostgreSQL on Google Cloud Run. React, TypeScript and Vite on Cloudflare Workers, with images and catalog files on Cloudflare R2. Tested, built and deployed with GitHub Actions.

## Principles

- **Fast for shoppers.** The catalog is served from the edge and keeps working even if the backend is unavailable.
- **The ERP is the source of truth.** Prices and stock come from Bling; the store only adds presentation on top.
- **Private by default.** Customers share only what is needed to place an order, in line with Brazil's LGPD.

## Status

Vitrine is in early development. The first release is being built together with a jewelry store in Brazil.

- [ ] Foundation: infrastructure, CI/CD and authentication
- [ ] Bling ERP sync
- [ ] Published catalog
- [ ] Bag and WhatsApp checkout
- [ ] Admin dashboard
- [ ] Batch photo import
- [ ] Hardening and launch

<p align="center"><sub>Built in Brazil.</sub></p>
