# Storeva

<p align="center">
  <img src="assets/storeva-banner.svg" width="960" alt="Storeva — storefront software for Egyptian brands" />
</p>

**Storeva helps small businesses in Egypt run an online storefront.** Merchants manage their catalog, shipping, and orders from one dashboard. Shoppers browse the store, place an order, and can send its details to the merchant on WhatsApp.

Subscription-based · No sales commissions · Private application source

[Official website](https://storeva.vercel.app/) · [Live customer storefront](https://storeva.vercel.app/ghazal) · [Architecture](#architecture) · [GitHub contact](#contact)

## The product

### Storeva homepage

<p align="center">
  <img src="assets/screenshots/storeva-home.jpg" width="630" alt="Storeva’s public homepage headline and calls to action" />
</p>

![Storeva’s public feature section highlighting products, orders, shipping, and WhatsApp](assets/screenshots/storeva-features.jpg)

### Ghazal · Live customer storefront

Ghazal is a real Storeva customer. Its public store shows how a merchant’s branding, product photography, and catalog appear to shoppers.

![Ghazal’s desktop storefront with its own brand banner](assets/screenshots/ghazal-storefront.jpg)

![Ghazal’s public product grid and category filters](assets/screenshots/ghazal-catalog.jpg)

![Ghazal product detail with photography, description, and public price](assets/screenshots/ghazal-product.jpg)

<details>
<summary>View the mobile storefront</summary>
<p align="center">
  <img src="assets/screenshots/ghazal-mobile.jpg" width="390" alt="Ghazal’s storefront at mobile width, showing the banner and the start of the catalog" />
</p>
</details>

## How it works

**Merchant journey.** Add product photos, prices, size and color variants, and stock quantities. Configure shipping rates by Egyptian governorate. Review incoming orders and update their status.

**Customer journey.** Browse the catalog, select a product option, and add it to the cart. Enter delivery details and review the shipping charge at checkout. After placing the order, open the prefilled WhatsApp message and send it to the merchant.

## Architecture

| Layer | Responsibility |
| --- | --- |
| Storefront | Next.js App Router serves store-specific catalog and product pages. React handles cart and checkout interactions. |
| Merchant dashboard | Signed-in merchants manage products, stock, delivery rates, and orders. |
| Data and media | Supabase Auth handles sign-in, PostgreSQL stores records, and Supabase Storage holds product images. |
| Order handoff | Checkout saves the order through a database function. The confirmation page opens a prefilled WhatsApp message at the shopper’s request. |

**Stack** · Next.js App Router, React, TypeScript, Tailwind CSS, Supabase, and Zustand with browser persistence for the cart.

## Contact

[Find Mohamed Mamdouh on GitHub](https://github.com/mohamedmamdouh1805) for portfolio inquiries.
