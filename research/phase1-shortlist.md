# Phase 1 — Product Shortlist

**Prepared:** 2026-09-17
**Status:** Hypothesis list. Not validated. See "Data limitations" before acting on any number here.
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

### 1.2 Every limit in the brief is still a placeholder

Nothing below spends money, so Phase 1 proceeds. But I cannot run Phase 4 without these:

| Placeholder | Needed for | Suggested default if you want me to just pick |
|---|---|---|
| `$X` total test budget | Overall go/no-go | $1,500 |
| `$Y` daily ad cap | Launch | $50/day |
| `$Z` kill threshold, no sale | Kill rules | 2× break-even CPA (~$55 at $39 AOV) |
| `[N]` days before reading results | Kill rules | 4 days |
| `$W` approval threshold | Escalation | $100 |
| `[target countries]` | **Shipping times + this entire shortlist** | Assumed **US-only** below |
| `[DSers/AutoDS/CJ]` | Sourcing | — |
| `[Meta/TikTok]` | Creative format + testing | — |

**The target-country assumption is material.** I assumed US. If you're targeting UK/EU/AU, sourcing changes (EU warehouses, VAT/IOSS registration, GPSR — which since Dec 2024 requires a named EU Responsible Person on general consumer products), and at least three items below become unviable on shipping time.

---

## 2. Data limitations — how much to trust this list

I want to be blunt, because the "demand signal" column is the part you'd most want to rely on and it is the weakest.

- **Costs and shipping times are estimates**, from category norms — not quotes pulled from a supplier account. Treat them as ±40%. They must be replaced with real figures before any spend.
- **I could not access Meta Ad Library, TikTok Creative Center, or Google Trends.** "Demand signal" below is therefore reasoning from category-level reporting plus the shape of the product, not a count of live ads or a trend curve.
- **Most sources reachable by search are SEO content farms** run by dropshipping tool vendors. Their "winning product" lists are marketing for the tool and are, by construction, lists everyone else is also reading. I used them for category direction only, and deliberately did not simply copy their picks.
- **No supplier has been vetted.** Ratings, order volumes, and consistency are Phase 2 and require account access.

Anything marked **[EST]** is my estimate. Nothing in this document is a verified figure.

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

## 4. The shortlist

Sell price = my proposed price. Cost = product + shipping to US **[EST]**. Margin = gross, before ads, fees, refunds.

| # | Product | Cost [EST] | Sell | GM $ | GM % | Markup | Ship (US) [EST] | Competition | Verdict |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Desk cable-management **kit** (tray + magnetic clips + sleeve + channels) | $11–14 | $39 | $25–28 | 64–72% | 2.8–3.5× | 7–10d | High on parts, **low on kits** | **GO** |
| 2 | Wool-felt desk mat set (mat + coaster + cord catch) | $13–16 | $45 | $29–32 | 64–71% | 2.8–3.5× | 7–12d | Medium | **GO** |
| 3 | Dog car seat hammock + door shields + seatbelt tether | $15–19 | $54 | $35–39 | 65–72% | 2.8–3.6× | 8–12d | Medium | **GO** |
| 4 | Fit-specific fridge organization set (bins + labels + liners) | $13–17 | $42 | $25–29 | 60–69% | 2.5–3.2× | 10–15d | Medium | WATCH |
| 5 | Elevated tilted slow-feeder bowl set (steel/bamboo, **not ceramic**) | $14–18 | $46 | $28–32 | 61–70% | 2.6–3.3× | 10–14d | Medium | WATCH |
| 6 | Under-monitor light bar, USB-powered | $14–18 | $45 | $27–31 | 60–69% | 2.5–3.2× | 8–14d | High | WATCH |
| 7 | Aluminium monitor riser w/ drawer | $16–21 | $49 | $28–33 | 57–67% | 2.3–3.1× | 12–18d | High | WATCH |
| 8 | Reusable pet-hair removal set (no electronics) | $7–9 | $29 | $20–22 | 69–76% | 3.2–4.1× | 7–10d | **Very high** | NO |
| 9 | Silicone air-fryer liner + accessory kit | $7–10 | $27 | $17–20 | 63–74% | 2.7–3.9× | 7–12d | **Very high** | NO |
| 10 | Sunset/aurora projector lamp | $9–13 | $34 | $21–25 | 62–74% | 2.6–3.8× | 8–14d | **Very high** | NO |

### Why the three NOs are still on the list

You asked for ten, so here are ten — but padding a shortlist with items I'd refuse to launch would be dishonest. #8–10 are the ones every tool-vendor list is currently pushing. All three fail your own "not sold cheaply everywhere" rule: identical units sit at $8–19 on Amazon and roughly half that on Temu. #10 additionally has a known return-rate problem (LED/motor failure) and is the single most-copied dropshipping SKU of the last three years. I'd drop all three rather than test them.

---

## 5. Detail on the three recommended

### #1 — Desk cable-management kit — $39

- **Problem:** genuinely felt, visible, and universal among desk/WFH buyers.
- **Creative:** before/after is the entire ad. Strongest short-form hook on this list; near-zero scripting risk.
- **Why it survives the Amazon test:** individual trays are $15–28 on Amazon and commoditised. A *kit* that solves the whole desk in one purchase is not directly comparable, and lets you own a price point.
- **Physical:** ~400–600g, steel/plastic/velcro, effectively unbreakable. Low return risk.
- **Certification:** none required — no battery, no mains power. This matters; it keeps you clear of your own electronics exclusion.
- **Risks:** adhesive failure on textured desks is the likely #1 complaint → must be addressed honestly in the copy, and clamp-mount preferred over adhesive-only.

### #2 — Wool-felt desk mat set — $45

- **Why:** design-led, so price is carried by material and colorway rather than function. Highest brand-building potential here, and the most natural fit for a single-niche store alongside #1.
- **Physical:** light, flat, cheap to ship, literally cannot break. **Lowest return risk on the list.**
- **Creative:** flat-lay and desk-setup content; evergreen, not trend-dependent.
- **Risks:** felt quality varies sharply between suppliers (polyester passed off as wool). Sample check is essential, and the copy must state the actual fibre content — no "wool" claim unless the sample and supplier spec support it.
- **Note:** colorway/print selection is where IP risk would creep in. Plain colorways only.

### #3 — Dog car seat hammock kit — $54

- **Why:** highest absolute margin on the list, and pet is repeatedly cited as a category with margins plus real audience loyalty. Fit-specific ("does it fit my car/dog") suppresses raw price comparison.
- **Physical:** folds flat, ~700g–1kg, unbreakable.
- **Creative:** dog-in-car footage is high-performing and cheap to produce — but **only with real dogs and real cars**. No stock footage passed off as customer content.
- **Risks:** sizing/fit returns are the main driver. Needs an explicit vehicle-fit guide, which is a real content asset and a competitive moat.
- **Watch:** anchor-strap safety claims. Do **not** claim crash protection or restraint safety — that is a testable safety claim you cannot back, and it is exactly the kind of thing that draws a platform policy strike.

---

## 6. Unit economics you should sanity-check before funding anything

Worked at #1's numbers ($39 sell, $12.50 landed cost):

```
Sell price                     $39.00
Landed cost (product+ship)    -$12.50
Payment fees (2.9% + $0.30)    -$1.43
Est. refunds/replacements @4%  -$1.56
--------------------------------------
Contribution before ads         $23.51

Break-even CPA                  $23.51
Break-even ROAS                  1.66x
Target ROAS for real profit      2.5x+
```

**This is the number that decides the business, not the product.** At a 1.66× break-even, you need a sub-$24 CPA. If your real-world CPA lands at $35–45 — common for a cold-traffic single-product store on either platform — this product cannot be profitable at $39 no matter how good the creative is. The fixes are a higher AOV (bundle/upsell to $59–79) or a lower CPA, and the honest time to discover which is *before* spending, not after.

I'd want your read on this before Phase 4.

---

## 7. What I need from you

**To finish validating this list (no spend, but needs access):**
- Supplier app credentials, or export me a cost/shipping sheet for #1–#7 so I can replace every **[EST]** with a real figure.

**To proceed past Phase 1:**
1. Fill the placeholders in §1.2 (or tell me to use my suggested defaults).
2. **Target countries** — confirm US, or tell me otherwise; several picks change if not.
3. Which supplier app and which ad platform.
4. Shopify + ad account access.

**Sample purchases:** the brief pre-approves these. I'd order #1, #2, #3 — roughly $120–140 delivered for all three including duplicates from backup suppliers. I have **not** ordered anything, because I have no supplier account and no shipping address for you.

---

## 8. Two honest flags

1. **I cannot verify demand.** With the ad libraries and trend tools unreachable from here, this list is reasoning, not evidence. It is a good starting hypothesis set and it is screened hard against your rules — but if you fund a test on it without the Phase 2 verification, you are funding my judgement, not data. Say so out loud now rather than discover it at $400 spent.
2. **Pick the niche before the product.** #1 and #2 form a coherent desk/home-office store; #3 and #5 form a coherent pet store. Mixing them makes the store read as a generic dropshipper, which is precisely what kills trust and conversion rate. My recommendation: **desk/home-office, hero product #1, #2 as the AOV-raising second SKU.**

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
