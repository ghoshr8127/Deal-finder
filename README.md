# Black Friday 2026 Deal Finder 🇺🇸 🇨🇦

A free, fast page for finding Black Friday and Cyber Monday 2026 deals in the **USA and Canada**: electronics, home, clothing, shoes and more, from Amazon, Walmart, Best Buy, Target, Costco, Nordstrom, Lululemon, Canadian Tire and others.

**Live site:** https://YOUR-SITE.netlify.app

## Features

- **USA / Canada switch:** Canadian prices are shown in CAD and never converted.
- **Search that forgives typos:** "airpod", "macbok" or "lulu" all find what you mean.
- **Filters:** category, store, live or upcoming, sold in stores, has a coupon.
- **Sorting:** by biggest % off, biggest $ off, lowest price or newest.
- **Store comparison:** see the same item's price at every store tracked.
- **My list:** mark deals Buy, Maybe, Skip or Bought, set a target price and track a budget. Your list is saved in your own browser only.
- **Deal drop alerts:** upcoming sale start dates, which you can add to your calendar with a reminder.
- **Store dates:** early sale, Black Friday and Cyber Monday dates and hours for each store.
- **CSV export:** download the deals you're viewing.

## How the data works

Deals are gathered from retailer sale pages and newsrooms and from trusted deal sites (9to5Toys, NBC Select, RedFlagDeals, SmartCanucks, CostcoGuides and others). Every deal lists its source and the date it was found.

All deal data lives in `deals-data.js` and is refreshed during the sale season. Prices change quickly, so **always confirm the price on the store's site before buying.**

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app: one page with no build step |
| `deals-data.js` | Deals, alerts and store dates (`window.BF_SNAPSHOT`) |
| `netlify.toml` | Netlify settings: publish the folder as-is and never cache the data file |

## Run it locally

No install needed. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

Hosted on Netlify from this repo. Every push to `main` redeploys the site automatically.

## Disclaimer

This is an independent project, not affiliated with any retailer. Some store links may be affiliate links; if you buy through them, this site may earn a small commission at no extra cost to you. Prices and availability can change at any time.
