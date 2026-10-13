# Publish-gate checklist

Use before approving any product the autopilot wants to publish. One pass per product.
Built from the original brief's rules plus what the autopilot's own gates, as described, do **not** cover.

**Any single HARD REJECT ends it.** Everything else must be answered, not assumed.

---

## A. Hard rejects — any one, stop

- [ ] Counterfeit, branded, trademarked, or character/IP design
- [ ] Supplement, medical device, or anything carrying a health claim
- [ ] Cosmetic requiring regulatory compliance
- [ ] Children's product (CPSIA certificate territory)
- [ ] Electronic without a safety certification on file
- [ ] Weapon, or weapon-adjacent
- [ ] Restricted by Shopify **or** Google Merchant Center
- [ ] Category with an active recall history
- [ ] Material composition unclear → **honest copy is impossible, so it cannot ship**

## B. The gate the autopilot probably doesn't have

The described gates screen safety, IP, materials, claims, recalls, compliance. None of those catch a
product that is simply **sold cheaply everywhere** — the test that killed both products in this repo.

- [ ] Cheapest equivalent on Amazon Prime: `$________`
- [ ] Cheapest equivalent on Temu: `$________`
- [ ] Our price: `$________`
- [ ] **Is our price within ~1.5× the Prime floor?** → if yes, **reject**: there's no room to pay for ads
- [ ] If this is a bundle: does a comparable bundle already exist below our price?

## C. Honest-copy gate

- [ ] Every claim in the listing traces to the supplier spec sheet
- [ ] No health, medical, or safety claim of any kind
- [ ] Material named **exactly** as the supplier states it — no upgrade words
      (not "wool" for polyester, not "leather" for PU, not "steel" for coated alloy)
- [ ] Shipping time stated honestly, matching the **actual** warehouse and method for this SKU
- [ ] No countdown timer, fake scarcity, fake review count, or invented testimonial
- [ ] Copy is original, not the supplier's listing text pasted in

## D. Imagery

- [ ] Images licensed for resale use
- [ ] **No other brand's logo, watermark, or packaging visible in any image** — the most common
      auto-publish IP failure
- [ ] No model's face without a release
- [ ] Images match the SKU actually being shipped

## E. Economics — quoted, not estimated

- [ ] Product cost `[QUOTED]`: `$________`
- [ ] Shipping to US `[QUOTED]`: `$________`
- [ ] CJ fulfilment fee + per-extra-item: `$________`
- [ ] Oversized/volumetric fee, if any: `$________`
- [ ] **Landed total:** `$________`
- [ ] Sell price: `$________` → **Contribution:** `$________`
- [ ] **Break-even CPA:** `$________` — is that achievable on this channel, honestly?

## F. Operations

- [ ] Supplier rating ≥4.5 and ≥100 orders
- [ ] US warehouse stock confirmed (not China-direct, if under-10-day is promised)
- [ ] All components in **one** warehouse, if it's a bundle
- [ ] Backup supplier identified
- [ ] **CJ wallet holds enough to buy this order the moment it sells**
- [ ] Return path exists and matches the published refund policy

## G. Google Shopping specific

- [ ] Category permitted by Merchant Center policy
- [ ] GTIN present, or correctly declared absent — missing GTINs are a common disapproval
- [ ] Brand field populated consistently
- [ ] Landing page price matches the feed price exactly (mismatch = misrepresentation flag)

---

## Sign-off

```
Product:            ____________________
Approved / Rejected:  ____________________
If rejected, which gate: ____________________
Date / by:          ____________________
```

**Keep the rejections.** The autopilot rejected 46 of 50 on its first run. If the ones you reject here
cluster on a gate the autopilot lacks — section B especially — that's the gate to go add to its code,
rather than catching the same thing by hand every time.
