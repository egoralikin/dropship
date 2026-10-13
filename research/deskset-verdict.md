# Desk Set — Check 1 partial result and verdict

**Date:** 2026-10-13 · **Method:** WebSearch only. Amazon, CJ and Google Trends are all blocked by this
environment's egress proxy, so no product page was opened and no price was read off a live listing.

**New label used here: `[SNAPSHOT]`** — a price surfaced in search results, not read from the product page.
Weaker than `[QUOTED]` (which needs a URL *and* a verified read) and stronger than `[EST]` (my guess).
Amazon prices move daily. Nothing below should be treated as settled.

---

## What came back

**Single felt desk mats [SNAPSHOT]:**

| Size | Price |
|---|---|
| 47.2 × 23.6" | $31.34 |
| 35" × 17" (Nordik) | $24.97 |
| 40 × 16" (DAWNTREES) | $18.05 |
| 40 × 16" | $9.98 |
| 35.4 × 15.7" | $11.99 |
| 23.6 × 11.8" | $14.10 |

Category pages span $3–$350 (felt desk pad) and $8–$96 (wool felt desk pad).

**Multi-piece desk mat sets [SNAPSHOT]:**

| Item | Price |
|---|---|
| Desk mat + coasters (cat design) | **$18.99** |
| 35.4 × 15.7" set + keyboard wrist rest + coaster | **from $23.66** |
| XXL mat + coaster (Walmart) | from $8.99 |
| Mousepad + coaster sets (Etsy) | ~$8.48 |

No premium multi-piece **felt** set was found at any price. Grovemade appears on Amazon but no price surfaced.

---

## Verdict against the brief's own thresholds

| Test | Threshold | Result |
|---|---|---|
| Hard kill — comparable multi-piece **felt** set ≤$40 | Ends the product | **Not conclusively met.** Sets at $18.99 and $23.66 exist, but they read as gaming/PU mats with a coaster added, not felt sets. |
| Warning — good single felt mat ≤$25 | Set must justify +$50 on presentation alone | **Met, clearly.** Large felt mats at $24.97–$31.34; smaller at $9.98–$18.05. |
| Support — premium felt mats well above $75 | Would prove the price point | **Not found.** Grovemade exists but no price confirmed. |

**Verdict: the $75 Desk Set is in serious trouble, though not formally dead.**

The arithmetic a customer does: a large felt mat is **$25–31**, coasters are **~$8**, a mousepad is a few
dollars. Our $75 bundle asks roughly **+$45 over assembling the same thing from Prime**, and multi-piece
mat-and-coaster sets already exist under $25.

That premium can only be carried by brand and presentation. We have **no brand, no sample, no photographs,
and no confirmed fibre content**. The one defence that made this product hero — "design-led, so price is
carried by material and finish" — requires exactly the assets that don't exist. And the supportive
evidence that would have justified $75 (an established premium tier) did not appear in the results.

**Recommendation: retire the Desk Set at $75.** If it's revived, it is at $39–45 as a single
better-than-average mat with a real brand behind it — which is a different business, with different
economics than anything in `phase2-bundles-and-access.md`.

**Caveat:** this rests on search snapshots, not opened pages. If the browser checks ever run, they could
overturn it. But they would have to overturn a wide margin, not a narrow one.

---

## This is mostly moot now, and that is the bigger point

`dropship-autopilot` isn't selling the Desk Set. It is running its own discovery over 40 seed categories
and auto-publishing whatever passes its gates. So a month of product research is **not feeding the live
system at all**.

Two consequences:

1. The careful screen in this repo — the exclusions, the $25–80 band, the 3× markup rule, the
   "not sold cheaply everywhere" test that just killed this very product — is not applied to anything the
   autopilot publishes, unless it was separately built into those gates.
2. The one test that mattered most here is the one most likely missing there: **a published product can
   still be a commodity sold for $12 on Temu.** The autopilot's gates, as described, screen for safety,
   IP, materials, claims, recalls and compliance. Nothing in the handoff says they screen for
   *price-floor viability*.

That's worth checking in the autopilot's gate code before it publishes anything.
