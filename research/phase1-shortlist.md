# Phase 1 — Product Shortlist

**Prepared:** 2026-09-17 · **Revised:** 2026-09-17 (limits set; NO-verdict products dropped; quote status labelled)
**Status:** Hypothesis list. **Every figure is ESTIMATED. Zero CJ quotes pulled.** See §2.
**Spend to date:** $0

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

## 4. The shortlist — 7 candidates

Three products (reusable pet-hair set, silicone air-fryer liner kit, sunset projector lamp) have been **dropped** per your instruction. All three failed the "not sold cheaply everywhere" rule and were the most-copied SKUs in the category. They are recorded in §4.1 so the decision stays auditable, not to keep them alive.

Sell price = my proposed price. Cost = product + shipping to US.
**Quote status for every row below: [EST] — no CJ quote pulled.**

| # | Product | Cost [EST] | Sell | GM $ | GM % | Markup | Ship US [EST] | Competition | Verdict |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Desk cable-management **kit** (tray + magnetic clips + sleeve + channels) | $11–14 | $39 | $25–28 | 64–72% | 2.8–3.5× | 7–10d | High on parts, **low on kits** | **GO — hero** |
| 2 | Wool-felt desk mat set (mat + coaster + cord catch) | $13–16 | $45 | $29–32 | 64–71% | 2.8–3.5× | 7–12d | Medium | **GO — same niche as #1** |
| 3 | Dog car seat hammock + door shields + seatbelt tether | $15–19 | $54 | $35–39 | 65–72% | 2.8–3.6× | 8–12d | Medium | **GO — held as pivot** |
| 4 | Fit-specific fridge organization set (bins + labels + liners) | $13–17 | $42 | $25–29 | 60–69% | 2.5–3.2× | 10–15d | Medium | WATCH |
| 5 | Elevated tilted slow-feeder bowl set (steel/bamboo, **not ceramic**) | $14–18 | $46 | $28–32 | 61–70% | 2.6–3.3× | 10–14d | Medium | WATCH |
| 6 | Under-monitor light bar, USB-powered | $14–18 | $45 | $27–31 | 60–69% | 2.5–3.2× | 8–14d | High | WATCH |
| 7 | Aluminium monitor riser w/ drawer | $16–21 | $49 | $28–33 | 57–67% | 2.3–3.1× | 12–18d | High | WATCH |

The $39–54 prices above are the **original single-kit configurations**. They are superseded by the $60–80 bundle redesign in `research/phase2-bundles-and-access.md`, which is the version to actually price against. This table is kept as the baseline the redesign is measured from.

### 4.1 Dropped — decision record

| Product | Verdict | Reason |
|---|---|---|
| Reusable pet-hair removal set | DROPPED | $8–14 on Amazon, ~$5 Temu. No pricing room. |
| Silicone air-fryer liner + accessory kit | DROPPED | $9–19 on Amazon. Commodity; repeat-purchase upside doesn't survive the CPA. |
| Sunset / aurora projector lamp | DROPPED | Most-copied dropship SKU of the last 3 years; known LED/motor return rate. |

---

## 5. Detail on the three GO products

### #1 — Desk cable-management kit — **hero**

- **Problem:** genuinely felt, visible, universal among desk/WFH buyers.
- **Creative:** before/after is the entire ad. Strongest short-form hook here; near-zero scripting risk.
- **Why it survives the Amazon test:** individual trays are $15–28 and commoditised. A kit solving the whole desk in one purchase isn't directly comparable, which is what lets you hold a price point.
- **Physical:** ~400–600g, steel/plastic/velcro, effectively unbreakable. Low return risk.
- **Certification:** none required — no battery, no mains power. Keeps you clear of your own electronics exclusion.
- **Risks:** adhesive failure on textured desks will be complaint #1 → clamp-mount over adhesive-only, and say so honestly in the copy.

### #2 — Wool-felt desk mat set — **same store as #1**

- **Why:** design-led, so price is carried by material and colorway rather than function. Highest brand potential here and the natural AOV-raiser next to #1.
- **Physical:** light, flat, cheap to ship, cannot break. **Lowest return risk on the list.**
- **Creative:** flat-lay and desk-setup content; evergreen, not trend-dependent.
- **Risks:** felt quality varies sharply — polyester passed off as wool is common. Sample check essential. **No "wool" claim in copy unless the sample and CJ spec both support it.**
- **Note:** plain colorways only — prints are where IP risk creeps in.

### #3 — Dog car seat hammock kit — **held in reserve**

- **Why:** highest absolute margin, and pet has real audience loyalty. Fit-specific ("does it fit my car/dog") suppresses raw price comparison.
- **Physical:** folds flat, ~700g–1kg, unbreakable.
- **Creative:** dog-in-car footage performs and is cheap to shoot — **real dogs, real cars only**. No stock footage presented as customer content.
- **Risks:** sizing/fit returns are the main driver; needs an explicit vehicle-fit guide, which doubles as a moat.
- **Hard limit:** no crash-protection or restraint-safety claims. Untestable, unbackable, and precisely the kind of claim that draws a Meta policy strike.
- **Why reserve and not test:** it's a different niche from #1/#2, so testing it means a second store, second pixel, second audience. At $1,000 that's unaffordable. It's the pivot if the desk niche fails.

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

1. **I cannot verify demand from here.** Ad libraries and trend tools are unreachable in this environment. This list is reasoning, not evidence. The Claude-in-Chrome checks in the companion document are what convert it — until those are run, funding a test on this list means funding my judgement.
2. **Pick the niche before the product.** #1 and #2 form a coherent desk/home-office store; #3 and #5 form a pet store. Mixing them makes the store read as a generic dropshipper, which is what kills conversion rate. **Recommendation: desk/home-office, #1 as hero, #2 as the AOV-raising second SKU, #3 held as the pivot.**

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
