<div align="center">

<img src="assets/icon.svg" width="88" alt="Résham monogram" />

# Résham

**A Paris house since 1987: handwoven sarees, sherwanis, panjabis and tailoring, with pieces selected from London, Milan and Seoul.**

The complete online house, built end to end: a storefront for Bangladesh and France, an Atelier console for the owner and staff, and a rider portal for doorstep delivery.

**Opens February 1, 2027** · [**Live site**](https://project-mauve-kappa-92.vercel.app) · [**Watch the film**](media/resham-film.mp4)

![Next.js 16](https://img.shields.io/badge/Next.js-16-000?logo=nextdotjs) ![React 19](https://img.shields.io/badge/React-19-149eca?logo=react) ![TypeScript](https://img.shields.io/badge/TypeScript-strict-3178c6?logo=typescript&logoColor=fff) ![Supabase](https://img.shields.io/badge/Supabase-Postgres%20%2B%20Auth-3ecf8e?logo=supabase&logoColor=fff) ![Vercel](https://img.shields.io/badge/Vercel-hosted-000?logo=vercel) ![Tests](https://img.shields.io/badge/automated%20checks-380-c9a96e)

<a href="media/resham-film.mp4"><img src="media/film-poster.jpg" alt="The Résham film: click to watch" width="100%" /></a>

</div>

> **About this repository.** This is the public showcase of Résham: what it does, how it is built, the screenshots and the film. Résham is a real shop, so its code stays in a private repository.
>
> **Full source code available on request.**

---

## Contents

1. [What it is](#what-it-is)
2. [Film and cards](#film-and-cards)
3. [Screenshots](#screenshots)
4. [Features](#features)
5. [Tech stack](#tech-stack)
6. [Architecture](#architecture)
7. [Security](#security)
8. [Testing](#testing)
9. [Status](#status)
10. [About](#about)

---

## What it is

Résham is a production web shop built from scratch, with three parts that share one codebase and one database:

| Who | Where | What they do |
| --- | --- | --- |
| **Customers** | the shop (`/`) | Browse, search, ask the assistant, order for themselves or as a gift, pay, track the delivery live, collect points and a VIP card |
| **Owner and staff** | the Atelier console (`/atelier`) | Run orders, hand deliveries to riders or couriers, manage products, discounts, stock, customers and points, fees and the team |
| **Riders** | the rider portal (`/rider`) | See only the deliveries handed to them, call and navigate, and confirm each delivery with the customer's 4-digit code |

The shop sells in **two markets**: Bangladesh (prices in BDT; bKash, Nagad, Rocket, Upay, cards, banks or cash on delivery; riders) and France (prices in euros; card, Apple Pay and Google Pay; tracked courier). Visitors can view prices in 18 currencies.

---

## Film and cards

A 42-second film for the opening on **February 1, 2027**, made from the live site (with sample orders):

[**Watch the film (MP4, 1080p)**](media/resham-film.mp4)

Seven cards for LinkedIn (1080 × 1350), also as one PDF carousel: [`media/linkedin`](media/linkedin).

<p>
<img src="media/linkedin/01-cover.jpg" width="13.5%" alt="Card 1: cover" />
<img src="media/linkedin/02-the-shop.jpg" width="13.5%" alt="Card 2: the shop" />
<img src="media/linkedin/03-order-to-door.jpg" width="13.5%" alt="Card 3: order to door" />
<img src="media/linkedin/04-the-console.jpg" width="13.5%" alt="Card 4: the console" />
<img src="media/linkedin/05-the-rider-portal.jpg" width="13.5%" alt="Card 5: the rider portal" />
<img src="media/linkedin/06-under-the-hood.jpg" width="13.5%" alt="Card 6: under the hood" />
<img src="media/linkedin/07-see-it-live.jpg" width="13.5%" alt="Card 7: see it live" />
</p>

---

## Screenshots

### The shop

| | |
| :---: | :---: |
| <img src="screenshots/home.jpg" alt="Home" /> **Home**: a WebGL hero that melts one photograph into the next | <img src="screenshots/shop.jpg" alt="Shop" /> **The wardrobe**: departments and collections, live stock |
| <img src="screenshots/product.jpg" alt="Product page" /> **Product page**: price, live stock per size, delivery dates for every speed | <img src="screenshots/product-layers.jpg" alt="What it's made of" /> **"What it's made of"**: every material named, with its origin |
| <img src="screenshots/product-provenance.jpg" alt="Provenance" /> **Provenance**: from raw material to the customer's door | <img src="screenshots/home-craft.jpg" alt="Craft on the home page" /> **Craft**: the anatomy of a piece, on the home page |
| <img src="screenshots/gift-atelier.jpg" alt="Gift wrapping" /> **Gift wrapping**: six wraps in 3D (Three.js) and a card of up to 200 words | <img src="screenshots/bag.jpg" alt="Bag" /> **The bag**: quantities, undo, gift wrap and totals |
| <img src="screenshots/search.jpg" alt="Search" /> **Search**: press `/` anywhere | <img src="screenshots/assistant.jpg" alt="Shopping assistant" /> **Shopping assistant**: answers in the customer's language |
| <img src="screenshots/france.jpg" alt="France" /> **Two markets**: France with euro prices | <img src="screenshots/verify.jpg" alt="Verify a receipt" /> **Verify a receipt**: catches forged receipts |

### Ordering and after

| | |
| :---: | :---: |
| <img src="screenshots/checkout-details.jpg" alt="Checkout" /> **Checkout**: for yourself or as a gift, delivery speed, payment | <img src="screenshots/checkout-review.jpg" alt="Review" /> **Review**: the server's own total, the best single offer applied |
| <img src="screenshots/order-confirmed.jpg" alt="Order confirmed" /> **Order confirmed**: a scroll-driven 3D moment with the delivery code | <img src="screenshots/tracking.jpg" alt="Live tracking" /> **Live tracking**: journey, rider, delivery code |
| <img src="screenshots/receipt.jpg" alt="E-receipt" /> **E-receipt**: with a verification code and QR | <img src="screenshots/account.jpg" alt="Account and VIP card" /> **Account**: points, rewards and the VIP card (tilts in 3D) |

### The Atelier console (owner and staff)

| | |
| :---: | :---: |
| <img src="screenshots/console-overview.jpg" alt="Overview" /> **Overview**: today, the to-do list, low stock, which services are connected | <img src="screenshots/console-orders.jpg" alt="Orders" /> **Orders**: every order, gifts, flagged payments, rider hand-over |
| <img src="screenshots/console-products.jpg" alt="Products" /> **Products**: add, edit, hide; photos, BDT and euro prices, sizes, markets | <img src="screenshots/console-sections.jpg" alt="Sections" /> **Sections**: departments, collections and houses |
| <img src="screenshots/console-discounts.jpg" alt="Discounts" /> **Discounts**: sale prices, piece codes, order codes | <img src="screenshots/console-customers.jpg" alt="Customers and points" /> **Customers and points**: find by account, VIP card, email or mobile; in-store sales |
| <img src="screenshots/console-stock.jpg" alt="Stock" /> **Stock**: per size | <img src="screenshots/console-delivery.jpg" alt="Delivery and payments" /> **Delivery and payments**: fees, cash on delivery, France, connected services |
| <img src="screenshots/console-team.jpg" alt="Team" /> **Team**: roles, add a rider, set a rider's password | <img src="screenshots/console-orders-phone.jpg" width="48%" alt="Console on a phone" /> <img src="screenshots/console-menu-phone.jpg" width="48%" alt="Console menu on a phone" /><br>**On a phone** |

### The rider portal

| Sign in | Deliveries | Wrong code | Delivered |
| :---: | :---: | :---: | :---: |
| <img src="screenshots/rider-signin.jpg" alt="Rider sign-in" /> | <img src="screenshots/rider-deliveries.jpg" alt="Rider's deliveries" /> | <img src="screenshots/rider-wrong-code.jpg" alt="Wrong code refused" /> | <img src="screenshots/rider-delivered.jpg" alt="Delivered" /> |

### On a phone

| Home | Product |
| :---: | :---: |
| <img src="screenshots/home-phone.jpg" width="300" alt="Home on a phone" /> | <img src="screenshots/product-phone.jpg" width="300" alt="Product on a phone" /> |

> The shop's screenshots are taken from the live site by the workflow in `.github/workflows/screenshots.yml`. The console, account, checkout and rider screenshots use made-up demo data (no real customer appears anywhere).

---

## Features

### For customers

- **Storefront**
  - Departments (Women, Men, Accessories) and collections (Privé, Traditional, Classic, Modern, Western, Selections). The owner can open or close each of them, and add departments, such as Beauty with shades instead of sizes.
  - Live stock per size, and sale prices and piece codes shown on the cards.
  - Search with `/` or `Ctrl K`.
- **Product pages**: a long story for each piece:
  - every side of it;
  - "What it's made of", with each material and where it comes from;
  - close-ups;
  - provenance, from raw material to the door;
  - a buy bar that follows down the page.
- **Two markets**
  - Bangladesh and France, each with its own pieces, prices, delivery and ways to pay.
  - France is opened by the owner. Until then, its prices show in euros at today's rate.
- **18 currencies**, shown at the live exchange rate. Orders are always charged in BDT or euros.
- **Gifts**
  - Six gift wraps drawn in 3D, and a card of up to 200 words.
  - Order for someone else: the receiver gets the delivery SMS and code, and the sender gets the receipt.
- **Checkout**
  - Delivery speeds (Regular, Fast, Express 24 in Dhaka), with their dates.
  - Cash on delivery and online payment.
  - Promo codes and points rewards. Only the single best offer applies.
- **After ordering**
  - A 3D packing film and an "order confirmed" scene.
  - Live tracking with the rider's name and location.
  - A 4-digit delivery code, given only to the rider at the door.
- **E-receipt** with a 12-character verification code and a QR code. `/verify` tells anyone whether a receipt is genuine.
- **Loyalty**
  - 10 points per delivered order or visit to the atelier, and 10% off one piece per 100 points.
  - VIP Level 1 (10% off) at 1,000 lifetime points and Level 2 (20%) at 2,000, with a numbered VIP card.
- **Shopping assistant**
  - Answers prices, sizes, stock, fabrics and delivery in the customer's language.
  - Uses Claude when a key is set, and the built-in catalogue answers otherwise.
  - It cannot see orders or accounts.

### For the owner and staff: the Atelier console

- **Overview**: today's and the week's sales, what needs doing, low stock, and which outside services are connected.
- **Orders**
  - Search by order, name, phone or email; filters, and pages for older orders.
  - Confirm, pack, then hand to a rider (Bangladesh) or a courier with tracking (France).
  - Print packing slips.
  - Cancel: stock and points go back, and online payments are marked "refund due".
- **Flags**: risky or mismatched payments and failed delivery attempts are held for a person to check.
- **Products and sections**
  - Add or edit pieces with photos (re-encoded to WebP), BDT and euro prices, sizes and markets.
  - Departments, collections and houses.
  - No code or deploy is needed for any of it.
- **Discounts**: sale prices, codes for one piece, and codes for the whole order (percent or fixed, minimum spend, dates, use limits).
- **Customers and points**
  - Find a customer by account, VIP card, email or mobile.
  - Record in-store sales with the VIP discount, and change points or roles.
- **Delivery and payments**: delivery fees, cash on delivery, the France shop (fee, free-delivery threshold, euro rate, rounding, days), and which services are connected.
- **Team**: who can do what, add a rider login, set a rider's new password, remove someone.
- **Roles**
  - The **owner** can do everything.
  - **Staff** can do orders, customers, in-store sales, piece codes and stock.

### For riders: the rider portal

- **A separate sign-in.** The portal has its own session cookie, kept apart from the shop's. A rider login can't shop or open the console, and the owner's sign-in never opens the rider portal.
- **Only their own deliveries**, showing only what the door needs: name, phone, address, map, and the cash to collect.
- **Start delivery**: the customer gets an SMS with the rider's name and number.
- **Confirm with the customer's code**. A wrong code never marks an order delivered, and tries are limited.
- **"Couldn't deliver"** with a reason, which goes straight to the console.
- **Delivered today**, with the cash collected.

---

## Tech stack

| Layer | Used |
| --- | --- |
| **Framework** | [Next.js 16](https://nextjs.org) (App Router, Turbopack), [React 19](https://react.dev), TypeScript (strict) |
| **Frontend** | Hand-written CSS (no UI kit); [Three.js](https://threejs.org) for the 3D gift wraps; raw WebGL shaders for the hero and the order-confirmed scene; [GSAP](https://gsap.com) for animation; [Lenis](https://lenis.darkroom.engineering) for smooth scrolling; Jost and Tenor Sans fonts (self-hosted via Fontsource); the logo and wordmark drawn as SVG paths |
| **Backend** | Next.js route handlers on Node.js (Vercel functions); [Zod](https://zod.dev) validation on every input; [sharp](https://sharp.pixelplumbing.com) for photo uploads; [qrcode](https://github.com/soldair/node-qrcode) for receipts |
| **Database and accounts** | [Supabase](https://supabase.com): Postgres with Row Level Security, Postgres functions for stock, points and rate limits, Supabase Auth (email and password) through `@supabase/ssr` with httpOnly cookies, and Storage for product photos |
| **Payments** | [SSLCommerz](https://sslcommerz.com) (Bangladesh: bKash, Nagad, Rocket, Upay, cards, banks) and [Stripe Checkout](https://stripe.com) (France: cards, Apple Pay, Google Pay) |
| **Messages** | [Resend](https://resend.com) for receipt email and [Twilio](https://twilio.com) for SMS (either can be swapped for a local provider in one function) |
| **AI** | [Claude](https://www.anthropic.com/claude) through the Anthropic Messages API, with tool use over the catalogue |
| **Hosting** | [Vercel](https://vercel.com) (Singapore region), with long-lived CDN caching for photos and static pages |
| **Quality** | 380 automated checks: API, security probe, browser and unit tests (see [Testing](#testing)); pages checked with axe (WCAG 2 A and AA) during development; a pre-commit secret scanner |

---

## Architecture

```mermaid
flowchart LR
  subgraph Browser
    S["Shop<br/>/"]
    A["Atelier console<br/>/atelier"]
    R["Rider portal<br/>/rider"]
  end
  subgraph Vercel["Vercel: Next.js 16"]
    P["Pages<br/>(static where possible)"]
    API["Shop API<br/>/api/*<br/>shop session cookie on /"]
    RAPI["Rider API<br/>/rider/api/*<br/>rider session cookie on /rider"]
  end
  subgraph Supabase
    DB[("Postgres<br/>RLS on every table")]
    AU["Auth"]
    ST["Storage<br/>(photos)"]
  end
  S --> P
  A --> P
  R --> P
  S -->|fetch| API
  A -->|fetch| API
  R -->|fetch| RAPI
  API --> DB
  API --> AU
  API --> ST
  RAPI --> DB
  RAPI --> AU
  API --> SSL["SSLCommerz<br/>Bangladesh payments"]
  API --> STR["Stripe<br/>France payments"]
  API --> TW["Twilio<br/>SMS"]
  RAPI --> TW
  API --> RS["Resend<br/>email"]
  API --> CL["Anthropic<br/>assistant"]
  SSL -.->|callbacks and IPN| API
  STR -.->|webhook| API
```

**Principles**

- **The browser never talks to the database.**
  - Every read and write goes through the site's own API, which checks who is asking.
  - Only the server holds the database's secret key.
- **The server decides every price.** The browser only previews. On every order the server:
  - recomputes the total (offers, VIP, rewards, delivery, gift wrap);
  - reserves stock atomically;
  - refuses the order if anything changed.
- **Two separate sign-ins.**
  - The shop and console share one session cookie, on `/`.
  - The rider portal has its own, only on `/rider`.
  - Each refuses the other's logins, so a login belongs to exactly one place.
- **Payments count only when the provider confirms them.**
  - SSLCommerz: through its validation API, for the right order, currency and amount.
  - Stripe: through a signed webhook.
  - A "failed" message never cancels an order by itself: the provider is asked first.
- **Static where possible.** Shop, department, collection and product pages are built ahead of time and served from the CDN. Live stock and prices arrive separately (`/api/live`).

---

## Security

- **Secrets**
  - Keys live only in Vercel's environment variables, marked Sensitive.
  - A check before every commit refuses any change that contains a key, token, private key or the database address.
- **Sessions**
  - httpOnly, Secure, SameSite=Lax cookies that page scripts can't read.
  - Two separate sign-ins, for the shop and for the rider portal.
  - Signing out ends only that browser's session.
- **Requests from other sites**
  - Every request that changes something must come from the site's own pages (`Sec-Fetch-Site`, then `Origin`).
  - The checkout also sends the account number: an order is refused if the browser has since signed in as someone else.
- **Roles on the server**
  - Every console action checks the role on the server.
  - Money going back to a customer, owner-only settings and team changes are owner-only.
- **Database**
  - Row Level Security is on every table, and the browser roles have no table rights at all.
  - Stock, points and limits change only through server-only functions.
- **Prices and stock**
  - The server recomputes every total.
  - Stock is reserved atomically, so a size can't be oversold.
  - A points reward is used only once, and codes keep to their use limits.
- **Payments**
  - Validated with SSLCommerz for the right order, currency and amount, or through Stripe's signed webhook.
  - Risky payments are held for a person to check.
  - Unpaid online orders are released after 30 minutes.
- **Delivery codes**
  - Checked against a keyed hash, in constant time, with 5 tries per 15 minutes.
  - The code itself is kept only encrypted, and only the customer who ordered can see it again.
- **Privacy**
  - Riders see only what the door needs.
  - Tracking and receipts open only for the account that ordered, or for staff.
  - The public receipt check shows no personal details.
- **Abuse limits**, shared across all servers: sign-in (per network and per account), sign-up, password reset, orders, delivery codes and the assistant.
- **Headers**: a strict Content-Security-Policy, HSTS, frame denial, `nosniff`, a referrer policy and a permissions policy.
- **Checked by tests** on every run (see [Testing](#testing)):
  - requests from another site, and private routes without a session;
  - tampered prices, junk input, and script injection on the search and verify pages;
  - secrets in the pages and code bundles;
  - another person's orders, receipts and deliveries;
  - forged payment callbacks.

---

## Testing

Every run builds the site, starts it next to a **stand-in database** that imitates Supabase, and runs:

| Suite | Checks | What it covers |
| --- | ---: | --- |
| API suite | 213 | Every console action by owner, staff, rider, customer and nobody; orders and hand-over; the rider portal; the two sign-ins (real password sign-in, cookies, sign-out of one door only); team changes; points and VIP |
| Security probe | 71 | Security headers, private routes without a session, requests from other sites, price tampering and junk input, script injection, wrong methods, assistant limits, secrets in bundles |
| Browser test | 18 | The owner in the console and a rider in the portal in one browser, neither touching the other |
| Unit tests | 78 | Pricing and offers, gift orders and phone numbers, payment settling and forged SSLCommerz callbacks, Stripe webhooks and returns, SMS numbers |

No real key or service is used: every value in the runner is a fake one.

---

## Status

The shop, the Atelier console and the rider portal are complete and running live. Before the opening on **February 1, 2027**, the owner connects the business accounts: online payments (SSLCommerz for Bangladesh, Stripe for France), email, SMS, the Claude assistant and the shop's own domain. The code for each is already in place.

---

## About

- **Owner, brand and product:** Miraz Ahmed ([@miraz2003](https://github.com/miraz2003)).
- **Development:** built with Claude (Anthropic) as an AI pair programmer.
- **Photography:** [Unsplash](https://unsplash.com) (sample photos until the studio photography is in).
- **Fonts:** Jost and Tenor Sans (SIL Open Font License).

© 2026 Miraz Ahmed. All rights reserved. The text, images and film here may be viewed on GitHub; they may not be copied, reused or published elsewhere without written permission. See [LICENSE](LICENSE).
