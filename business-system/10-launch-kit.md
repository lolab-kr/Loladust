# 10 — Launch Kit (Wix vs Shopify + how to go live)

## 10.1 Platform decision: **Shopify** (for your goals)

You asked for whichever is *profitable* for the Singapore market. For a premium brand aiming at
$5k/month with paid ads, retargeting and weekly drops, **Shopify wins** — not because it's cheaper
(it isn't) but because it makes **more money per visitor**, which at your AOV outweighs the fee.

| Factor | Shopify | Wix | Why it matters for you |
|--------|---------|-----|------------------------|
| Checkout conversion | ✅ Best-in-class | ⚠️ Good | At $157 AOV, a few % more conversions > the fee difference |
| Abandoned-cart recovery | ✅ Built-in | ⚠️ Add-on | Recovers 5–15% of lost orders — pays the subscription by itself |
| Ads pixel + retargeting | ✅ Native, clean | ⚠️ Workable | Your whole paid plan depends on this |
| Drops / pre-order apps | ✅ Strong ecosystem | ⚠️ Limited | The drop model is core to your brand |
| PayNow (SG) | ✅ Via app / Stripe | ✅ Native-ish | Both fine; Wix slightly easier here |
| Ease for non-tech | ⚠️ Moderate | ✅ Easiest | Wix's one real edge |
| Cost | ~SGD 39/mo (Basic) | ~SGD 22–34/mo | Wix cheaper, but see conversion above |

**Verdict:** **Shopify Basic.** Choose **Wix only if** budget is the hard constraint and you want
the simplest possible drag-and-drop — then use the same content and design from this kit.

> Honest note: the difference only matters *once you have traffic*. Until the Instagram feed is
> active (see §9), either platform sells the same $0. Get the store up on Shopify, then spend your
> energy on Reels.

## 10.2 What's in this kit

| File | Use |
|------|-----|
| `website/index.html` | A complete, working storefront — the exact design, copy, product set, cart and WhatsApp-checkout to replicate. Open it in any browser; it runs with no server. |
| `website/shopify-products.csv` | **Importable** into Shopify (Products → Import). Loads all 5 products with variants, prices, tags and SEO fields. |
| `ads-bundle.csv` | Editable ad bundle (open in Sheets/Excel). Meta + Google, copy + keywords + budgets. Edit and paste into Ads Manager. |
| `05-website.md` | Page-by-page structure + SEO copy if you build pages by hand on Wix. |

## 10.3 Go-live checklist (Shopify — an afternoon)

1. **Create store** → Shopify Basic. Set currency **SGD**, timezone **Singapore**.
2. **Theme** → install **Dawn** (free, minimalist, fast). Set brand colours (ivory `#F3ECE3`,
   cocoa `#3B2C22`, gold `#B08A2E`) and fonts (a light serif for headings, clean sans for body).
   Upload **logo #1** (wordmark) + the **LD monogram** as favicon.
3. **Import products** → Products → Import → upload `website/shopify-products.csv`. Add your real
   photos to each (the storefront uses placeholders for now).
4. **Payments** → enable Shopify Payments (cards) + a **PayNow** app (e.g. via Stripe/HitPay for SG).
5. **Shipping** → flat **$15** delivery; **free over $150** (Settings → Shipping → add a rate + a
   free-over-threshold rule). Add delivery-date picker app for lead times.
6. **Pages** → Home, About, How to Order, Contact/WhatsApp — copy from `05-website.md`.
7. **Apps** → abandoned-cart email (built in), a **countdown/drop** app, product reviews app.
8. **Pixels** → connect Meta pixel + Google tag (needed before ads — see `04-paid-ads.md`).
9. **Domain** → connect `loladust.sg` (buy same day you clear the name — see `01-brand.md`).
10. **Test** → place a test order end-to-end, confirm the WhatsApp/PayNow flow, then go live.

## 10.4 Replace before you launch
- **WhatsApp number** in `website/index.html` (search `var WA = "6591234567"`) → your real number.
- **Placeholder illustrations** → your own cake photography (the single biggest conversion lift).
- **Estimated prices** (tiramisu $58, cups $42, bento $52, loaf $17) → confirm against your
  ingredient cost × 3–4 (see `06-sales-strategy.md`).
- **Reviews** are sample copy → swap for real ones after the Founder's Drop.
