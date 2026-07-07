# 7 — CRM System

## 7.1 Tool choice

| Tool | Verdict | Why |
|------|---------|-----|
| **Airtable** | ✅ **Recommended (start here)** | Spreadsheet-simple, but a real relational DB. Free tier is enough at your volume. Views for orders/leads/repeat, automations built-in, connects to WhatsApp/email via Make/Zapier. Grows with you. |
| Notion | ⚠️ Fine alternative | Great if you already live in Notion; weaker automations than Airtable. |
| HubSpot | ❌ Overkill now | Powerful but heavy and pricey for a solo home baker. Revisit past $10k/mo. |
| Shopify (built-in) | ✅ **Use alongside** | Already stores customers/orders + abandoned-cart. Let Shopify own transactions; Airtable owns the *relationship* + drops/waitlist. |

**Decision:** **Shopify for orders/checkout + Airtable as the CRM brain.** Sync purchases into
Airtable (Zapier/Make). Don't build a custom CRM — you'd be maintaining software instead of baking.

## 7.2 Airtable schema (3 core tables)

**`Contacts`** — every human
`Name · WhatsApp · Email · Instagram · Source (Reel/Ads/Referral/Drop) · Status (Lead / Customer /
Repeat / VIP) · Tags (tiramisu-buyer, cake-buyer, corporate) · First order date · Last order date ·
Lifetime value · Birthday month · Notes`

**`Orders`** — every transaction
`Order # · Contact (link) · Product(s) · Amount · Delivery date · Status (Enquiry / Confirmed /
Baking / Delivered / Cancelled) · Channel · Drop (link) · Add-ons · Delivery address`

**`Drops`** — every limited batch
`Drop name · Date · Units offered · Units sold · Revenue · Waitlist count · Sold out? (Y/N) ·
Flavour · Notes/learnings`

**Key views:** *This week's deliveries* (calendar) · *Leads to follow up* · *Repeat customers*
(LTV desc) · *Birthdays this month* (proactive outreach) · *Waitlist for next drop*.

## 7.3 Automations (set these up in order of ROI)

| # | Trigger | Action | Why it pays |
|---|---------|--------|-------------|
| 1 | **Cart abandoned** (Shopify) | Email + WhatsApp @1h and @24h: "Your cake's still waiting — this week's slots are almost gone 🍰" | Recovers 5–15% of lost orders. Highest ROI automation. |
| 2 | **Order delivered** | +2 days: WhatsApp "How was it? A photo/review makes our week 💛" + review link | Generates the social proof that sells the next cake |
| 3 | **New lead / waitlist join** | Instant welcome + "next drop is Saturday, you're on the list" | Converts interest before it cools |
| 4 | **Birthday month** (from Contacts) | Email/WhatsApp 2 weeks before: "It's nearly your birthday — shall we bake?" | Turns a yearly occasion into a reliable repeat |
| 5 | **Post-purchase +30 days** | "Miss us? This week's drop…" to one-time buyers | Reactivation, lifts repeat rate |
| 6 | **VIP tag** (3+ orders) | Early access to drops, occasional freebie | Protects your best customers, drives referrals |

**Channel note:** WhatsApp is the highest-open channel in SG — use the **WhatsApp Business** app
(catalogue, quick replies, labels, broadcast lists) as the front line; email for receipts,
newsletters, and cart recovery. For automation glue, **Make.com** (cheaper than Zapier at volume)
between Shopify → Airtable → WhatsApp/email.

**Privacy:** get explicit opt-in for WhatsApp/email marketing (PDPA applies in Singapore). One
checkbox at checkout: "Send me drop alerts & offers." Keep the consent record in Airtable.

## 7.4 The weekly CRM ritual (15 min, every Monday)
1. Follow up all `Leads` from last week's drop waitlist.
2. Message `Birthdays this month`.
3. Log last week's `Drop` result (units, sold-out, learnings) — this data drives batch sizing.
4. Thank/flag any new `VIP`.
