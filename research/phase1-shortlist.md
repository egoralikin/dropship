# Phase 1 — Product Shortlist

**Prepared:** 2026-09-17 · **Revised:** 2026-09-17 (rev 3 — Bundle A dropped on Amazon price floor; Desk Set promoted to hero)
**Status:** **Every figure is ESTIMATED. Zero CJ quotes pulled.** See §2.
**Spend to date:** $0 · **Samples ordered:** none

---

## 1. Read this first: two blockers

### 1.1 I do not have the access the brief assumes

The brief grants me "your Shopify store, supplier app, and ad accounts." In this session I have:

| System | Access | Consequence |
|---|---|---|
| Shopify Admin | **None** | Cannot build store, set up pixel/CAPI, or fulfil orders |
| DSers / AutoDS / CJ | **None** | **Cannot read real supplier cost, rating, order volume, or shipping times** |
| Meta / TikTok Ads | **None** | Cannot create campaigns, read spend/ROAS, or query Ad Library |
| Web search | Yes | Category-level research only |
| Direct web fetch | **Mostly blocked** | `cjdropshipping.com`, `trends.google.com` and similar are blocked by this environment's egress proxy — I could not pull cost sheets or trend curves |
| Shell + GitHub repo | Yes | Where this document lives |

So Phases 2–5 cannot start until credentials/integrations are connected. I am not going to pretend otherwise.

### 1.2 Operating limits — CONFIRMED

| Limit | Value |
|---|---|
| Total budget | **$1,000** (all-in: ads + samples + platform) |
| Daily ad cap | **$30 per product** |
| Kill rule A | **$50 spent, no sale** |
| Kill rule B | **Below break-even ROAS after 3 days** |
| Approval threshold | **Anything over $50** |
| Target market | **US only** |
| Supplier | **CJ** primary; DSers / AutoDS backup |
| Ad platform | **Meta first** |
| Samples | **NOT pre-approved.** Each needs explicit OK; you place the orders |
| Payouts / banking | Never mine, under any circumstance |

Two things inside these limits need your sign-off before they happen, because both cross the $50 / paid-tool line:

- **Shopify subscription** (~$39/mo) — a paid tool, so it needs your OK even though it's under $50.
- **Any sample order** — see §7 for the list and estimated cost.

---

## 2. Data limitations — how much to trust this list

I want to be blunt, because the "demand signal" column is the part you'd most want to rely on and it is the weakest.

- **Costs and shipping times are estimates**, from category norms — not quotes pulled from a supplier account. Treat them as ±40%. They must be replaced with real figures before any spend.
- **I could not access Meta Ad Library, TikTok Creative Center, or Google Trends.** "Demand signal" below is therefore reasoning from category-level reporting plus the shape of the product, not a count of live ads or a trend curve.
- **Most sources reachable by search are SEO content farms** run by dropshipping tool vendors. Their "winning product" lists are marketing for the tool and are, by construction, lists everyone else is also reading. I used them for category direction only, and deliberately did not simply copy their picks.
- **No supplier has been vetted.** Ratings, order volumes, and consistency are Phase 2 and require account access.

**Quote-status labels used throughout:**

| Label | Meaning |
|---|---|
| **[EST]** | My estimate from category norms. ±40%. Not from any supplier account. |
| **[QUOTED]** | Pulled from a live CJ listing, with URL and date recorded. |

**Right now every figure in this document is [EST]. There are zero [QUOTED] figures.** `research/cj-quote-worksheet.md` is the blank worksheet that converts them; nothing moves to Phase 3 until it is filled.

---

## 3. Screening applied

Your rules, applied honestly — including where they cut down the field.

**Rejected on your exclusion list**, despite showing up repeatedly as top 2026 sellers in the research:

| Product | Why rejected |
|---|---|
| Red light therapy masks / wands | Medical + health claims; FDA device territory |
| Hydrocolloid pimple patches | Regulated (OTC drug/device); cosmetic compliance |
| Supplements, collagen, "gut health" | Explicitly excluded |
| Haircare / skincare (the 65%-margin category CJ pushes) | Cosmetic regulatory compliance |
| Back-to-school, dorm, kids' items | Children's products excluded (CPSIA/CPC testing) |
| Posture correctors | Implied medical claim |
| Halloween masks, pet costumes | Seasonal dead-end + IP risk on character designs |
| Branded-lookalike anything | Counterfeit/trademark |

**Structural conclusion worth stating up front:** your price band ($25–80) plus "not sold cheaply everywhere" plus 3× markup rules out nearly every single viral commodity gadget, because those all sit at $10–40 on Amazon with the identical unit on Temu for $6. The shapes that survive are:

1. **Kits/systems** — a bundle isn't directly price-comparable to a single SKU on Amazon.
2. **Design-led goods** — where material and colorway carry the price, not function.
3. **Fit-specific goods** — where "does it fit my thing" beats "what does it cost."

Every candidate below is one of those three. That is the thesis of this list.

---

## 4. The shortlist — 6 candidates

**Four products dropped.** Three on the "sold cheaply everywhere" rule in rev 2; the desk cable kit added
in rev 3 after web research found a ~$15 accessory kit and a 26-piece tray-plus-clips kit on Prime.

Sell prices below are the **bundle configurations** from `phase2-bundles-and-access.md`.
**Quote status for every row: [EST] — no CJ quote pulled.**

| # | Product | Landed [EST] | Sell | Contribution | BE ROAS | Ship US [EST] | Competition | Verdict |
|---|---|---|---|---|---|---|---|---|
| 2 | **Wool-felt Desk Set** (mat + mousepad + coasters + cord catch + tray) | $22.00 | **$75** | $48.64 | 1.54× | 7–12d | Medium | **HERO** |
| 3 | **Dog Car Travel Kit** (hammock + door shields + tether + bowl + gap catchers) | $28.20 | **$79** | $42.68 | 1.85× | 8–12d | Medium | **SECOND SKU** |
| 4 | Fit-specific fridge organization set | $13–17 | $42 | — | — | 10–15d | Medium | WATCH |
| 5 | Elevated tilted slow-feeder bowl set (steel/bamboo, not ceramic) | $14–18 | $46 | — | — | 10–14d | Medium | WATCH |
| 6 | Under-monitor light bar, USB-powered | $14–18 | $45 | — | — | 8–14d | High | WATCH |
| 7 | Aluminium monitor riser w/ drawer | $16–21 | $49 | — | — | 12–18d | High | WATCH |

### 4.1 Dropped — decision record

| Product | Dropped | Reason |
|---|---|---|
| **Desk cable-management kit ($69)** | **rev 3** | **Amazon Prime carries a ~$15 accessory kit (clips/ties/holders/sleeves) and single listings such as KHAMAL's 26-piece tray kit bundle a tray with clips and ties. A complete kit at ≤$40 defeats a $69 bundle.** Pending final confirmation of the KHAMAL price; revived only if it lands well above $40. |
| Reusable pet-hair removal set | rev 2 | $8–14 Amazon, ~$5 Temu. No pricing room. |
| Silicone air-fryer liner kit | rev 2 | $9–19 Amazon. Commodity. |
| Sunset / aurora projector lamp | rev 2 | Most-copied dropship SKU of the last 3 years; known LED/motor return rate. |

**The kit thesis took real damage here.** Bundle A was the cleanest expression of "a bundle isn't directly
price-comparable to a single SKU on Amazon," and Amazon turned out to already sell the bundle. That same
test now has to be run against the Desk Set before it inherits hero status — see `deskset-check-brief.md`.

---

## 5. Detail on the two live products

### #2 — Wool-felt Desk Set — $75 — **HERO**

- **Why it's now hero:** design-led, so price is carried by material and colorway rather than function.
  That's a different defence from Bundle A's — a bundle-of-parts can be out-bundled by Amazon, but a
  material-and-finish proposition competes on taste. It's a better thesis, and it's why this survived.
- **Physical:** light, flat, cannot break. **Lowest return risk on the list.**
- **Certification:** none — no battery, no mains power.
- **Creative:** flat-lay and desk-setup content; evergreen, not trend-dependent.
- **Risks:**
  - *Fibre honesty.* Polyester sold as wool is common. **No "wool" claim unless the CJ listing and the
    physical sample both support it.** Otherwise it's "felt", same price, honest description.
  - *Oversized shipping.* An 80×40cm rolled mat is exactly the shape that triggers CJ's oversized-package
    fee. This is now the single biggest cost unknown — see §6.
  - *Amazon floor, unproven.* The test that killed Bundle A has not yet been run against this product.
- **Plain colorways only** — prints are where IP risk enters.

### #3 — Dog Car Travel Kit — $79 — **SECOND SKU**

- **Why:** highest absolute margin among survivors. Fit-specific ("does it fit my car/dog") suppresses raw
  price comparison — the same defence that failed for cable parts works here, because fit isn't a spec you
  can price-match on.
- **Physical:** folds flat, ~700g–1kg, unbreakable.
- **Creative:** real dogs, real cars. No stock footage presented as customer content.
- **Risks:** sizing/fit returns drive the 7% reserve. Needs an explicit vehicle-fit guide, which doubles as
  a moat.
- **Hard limit:** no crash-protection, restraint, or safety claims. Untestable, unbackable, and the exact
  shape of claim that draws a Meta policy strike.
- **⚠ Niche conflict — see `phase2-bundles-and-access.md` §0.** This sits in pet/auto, not desk. Running it
  as a second SKU *inside the same store* contradicts the single-niche principle in §8.

---

## 6. Unit economics

Superseded — see `research/phase2-bundles-and-access.md` §2, which recomputes break-even ROAS and maximum CPA against your confirmed $1,000 / $30-day / $50-kill limits at the $60–80 bundle prices.

The conclusion from the original $39 configuration still holds and is the reason for the redesign: **at $39 the break-even CPA was ~$24, and a realistic cold-traffic Meta CPA of $35–45 makes that unprofitable regardless of creative quality.** Raising AOV is the lever.

---

## 7. Samples — none ordered, none approved

**Correction to the prior version of this document: I wrongly stated the brief pre-approved sample purchases. It does not. Nothing is pre-approved.**

No sample has been ordered and none will be. When we reach that point I will give you a specific list — CJ product URLs, quantities, and cost — and you place the orders yourself. The proposed list and its estimated cost are in `research/phase2-bundles-and-access.md` §4, for your decision, not as a request already granted.

---

## 8. Two honest flags

1. **I still cannot verify demand from here.** Ad libraries and trend tools are unreachable in this
   environment. Rev 3's Bundle A kill came from *your* browser research, not mine — which is precisely the
   pattern that should continue. Until the Desk Set clears the same checks, funding it means funding my
   judgement.
2. **One niche per store.** Rev 3 puts a felt desk mat and a dog car hammock in the same shortlist as hero
   and second SKU. Those are two audiences, not one. Options in `phase2-bundles-and-access.md` §0 — this
   needs a decision before any store gets built.

---

## Sources

Category direction (used with the caveats in §2):

- [Best Dropshipping Products September 2026 — AutoDS](https://www.autods.com/blog/best-items-to-dropship-in-september-2026/)
- [Winning Products, updated September 2026 — Sell The Trend](https://www.sellthetrend.com/blog/winning-products)
- [Top 50 Trending Dropshipping Products 2026 — Dropified](https://www.dropified.com/blog/top-50-trending-dropshipping-products-to-sell-in-2026-with-profit-margins/)
- [Best TikTok Products to Sell in 2026 — Darkroom](https://www.darkroomagency.com/observatory/the-best-tiktok-products-to-sell-in-2026-what-actually-works-on-tiktok-shop)
- [Is Dropshipping Oversaturated? Data across 26,500+ stores — Dropbuild](https://www.dropbuild.com/blog/is-dropshipping-oversaturated)
- [15 Saturated Dropshipping Niches to Avoid — NicheDropshipping](https://nichedropshipping.com/saturated-dropshipping-niches/)
- [Prohibited products — Shopify Help Center](https://help.shopify.com/en/manual/online-sales-channels/shop/eligibility/prohibited-products)
