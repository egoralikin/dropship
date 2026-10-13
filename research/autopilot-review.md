# Review — `dropship-autopilot` handoff, 2026-10-13

**Verification status: NONE.** The system was not inspected. `dropship-autopilot` is not in this repo or
on this machine; the Railway host is blocked by this environment's egress proxy (403 on the CONNECT
tunnel, which is a sandbox restriction and says nothing about whether the app is up). Every statement
below reviews the **described design**, taking the handoff's claims at face value. No claim in it has
been confirmed.

Severity: **S1** act before the first sale · **S2** fix soon · **S3** worth knowing.

---

## S1-1 — The system can take money it cannot fulfil

CJ wallet is **$0**, auto top-up **off**, ads **live**, automatic listing **signed and enabled**.

That combination means the pipeline can publish a product, run ads, and accept a customer's payment while
having no ability to buy the goods. The order sits paid and unfulfilled until the owner notices and funds
CJ by hand.

**The stated plan — "delay funding until the first sale" — may be circular.** New Shopify Payments
merchants typically face a payout hold on early sales (commonly several business days, longer if the
account is reviewed). If the first sale's cash is what funds CJ, and that cash is held, the first customer
waits on a payout that is waiting on them. *Typical practice, not verified for this account — confirm the
actual payout schedule in Shopify before relying on either version.*

Cost of being wrong: a paid, unfulfilled order is a refund, a chargeback, or a complaint — against a store
with no transaction history, which is when payment processors are least forgiving. The original brief
classes chargebacks as immediate-escalation events.

**Do:** fund CJ with the **$25 already authorised** under the supplier allocation *before* any ad spend.
It is inside the existing ceiling and needs no new authorisation. If funding now is genuinely not an
option, disable automatic listing and pause ads until it is — selling is the step that must wait, not
sourcing.

---

## S1-2 — Auto-publish to a live storefront is the unbounded risk

The $100 ceiling bounds the money. It does not bound this.

Discovery rejected **46 of 50** products for safety, IP, unclear-material, unsupported-claim, recall and
compliance reasons. The gates are working — but a 92% rejection rate also says the input stream is
92% unsuitable. The seed pool was then widened from 10 to 40 categories, which raises throughput against
those same gates. More volume past a filter means more opportunities for a false negative, and the new
categories include cleaning tools (chemical and labelling exposure) and pet accessories (safety claims).

A published listing carrying an IP violation, an unsupported claim, or a recalled item produces a
trademark complaint, a platform strike, or a consumer-safety problem. None of those are capped at $100,
and all are on the original brief's escalate-immediately list.

Two further points specific to auto-publish:

- **No sample exists for anything.** Every listing will therefore use supplier-provided imagery — which is
  also where IP problems most often live — and copy written without anyone having handled the product.
  The brief requires original copy, honest descriptions, and real photos where possible. An auto-publish
  pipeline with no physical goods cannot satisfy the third and is structurally prone to failing the second.
- Job `238027` is described as publishing automatically on pass. That is the step to gate.

**Do:** hold publication for owner review for at least the first 5 products. Let the job validate, score
and queue — approve the publish by hand. This costs very little time and removes the only uncapped risk
in the system.

---

## S1-3 — The ad budget cannot produce a learnable result

Against this repo's own validated economics (break-even CPA **$42–48** at a $75 AOV):

| Setting | Value | What it buys |
|---|---|---|
| Per-product test | **$20** | ~0.45 of one break-even conversion |
| Daily ad limit | **$10** | ~0.2 conversions/day |
| Total ads | **$55** | ~1.2 break-even conversions, all products combined |

**A product performing exactly at break-even would most likely return zero sales on a $20 test.** That is
the expected outcome, not a bad sign. So the test cannot distinguish a viable product from a dead one —
whatever it reports, the information content is near zero.

For scale: this repo already concluded that **$30/day for 10 days ($300)** was too small to exit Meta's
learning phase and would yield only directional reads. The live configuration is roughly an order of
magnitude below that.

This is not a money risk — $55 is $55. It is a **decision risk**: products may be killed as losers, or
the whole approach judged unviable, on data that never had the power to say so.

**Do:** treat $55 as buying a smoke test — do the ads serve, does the pixel fire, does checkout complete —
and not a product verdict. Nothing should be concluded about demand from it.

---

## S2-1 — Google Ads works against the product thesis

The locked parameter in this repo is **Meta first**. The live system runs Google Ads with Merchant Center.
That is not a neutral swap:

- **Shopping surfaces price comparison directly.** Our entire screen was built to find products that
  *aren't* price-comparable — design-led goods, fit-specific goods — precisely to avoid competing on
  price. Google Shopping places a $75 listing in a grid beside $25 alternatives. The channel reintroduces
  the exact dynamic the product selection was designed to escape.
- **Merchant Center suspension is a live risk.** New dropshipping merchants with supplier imagery and no
  trading history are a common misrepresentation-suspension profile. A suspension is an account
  restriction — an escalate-immediately event.
- The original creative thesis was short-form video. Shopping doesn't use it.

**Do:** decide deliberately whether the channel changed, and if it did, re-run product selection against
Google's economics rather than inheriting a shortlist built for Meta.

---

## S2-2 — What "285/285 passed" and "READY" actually certify

Tests verify the code does what it was written to do. They do not verify the business is sound, the
supplier real, the product legal, or the ads effective.

Two specific cautions:

1. **"All *currently evaluated* readiness checks pass."** A readiness check that defines its own scope and
   then reports passing that scope is close to circular. The useful question is what the check does *not*
   evaluate — on the evidence of this handoff, that includes every item in §S1-3 and §S2-1.
2. **The Stripe bug is the evidence.** A health monitor checked Stripe Issuing when the signed funding
   method was a card, opened a breaker, and paused discretionary work — found in production, with a green
   suite. The suite didn't cover the class of bug that actually occurred, and that class was *the safety
   system misfiring*. Breaker and pause logic deserves scrutiny the test count doesn't provide.

A related question worth answering: **can the system clear its own breakers?** Scoping that fix to the one
false Stripe breaker was right. But if an agent can diagnose a breaker as false and clear it unsupervised,
the breaker is advisory, not a control.

---

## S2-3 — The real authorisation is $1,100, not $100

"Cumulative base ceiling: $100" reads as the headline. But reinvestment is **80% of realized profit capped
at $1,000**, which compounds without a further human decision. Total authorised exposure is **$1,100**.

Tying reinvestment to *realized, payout-aware* profit is good design — it can't spend money that hasn't
landed. The point is only that the number to hold in mind is $1,100. That does match the brief's original
$1,000 total, so it isn't a breach; it's a framing that undersells itself.

---

## S3 — Smaller items

| Item | Note |
|---|---|
| **DataForSEO $1 balance**, auto top-up off | A research pipeline on $1 will stop shortly. Job `238027` reports no error *yet*; credit exhaustion mid-run is the likely next failure. Check before trusting its output. |
| **Pending reconciliation holds** | Releasing them on evidence of verification failure + zero reported cost is reasonable. Owner's call; low stakes. |
| **Keyword Ideas / vendor permission** | Correctly left disabled. That attestation asserts the vendor's terms permit this commercial automation. Sign it only if DataForSEO's actual terms say so — not to unblock a feature. |
| **Gmail read/send** | An autonomous sender on the owner's mailbox. Confirm it's a dedicated support address, not personal mail. Recommend draft-only until replies have been reviewed for a while — the brief requires honest, timely replies, which is a standard a generated auto-reply can quietly miss. |
| **Plan divergence** | The autopilot shares nothing with this repo: different channel, different budgets, different kill rules, and its own product discovery instead of the shortlist. The Desk Set work isn't feeding it. |

---

## Recommended order

1. **Fund CJ $25** (already authorised) — or pause ads and automatic listing until funded.
2. **Gate first publishes** behind owner review, at least the first 5.
3. **Confirm the Shopify payout schedule**, so the funding plan isn't circular.
4. **Reclassify the $55** as a smoke test, not a product verdict.
5. **Decide Meta vs Google deliberately**, and re-screen products if Google stands.
6. **Check DataForSEO credit** before trusting job `238027`'s output.
7. **Confirm Gmail scope**; set replies to draft-only for now.

## The open question for the owner

Is `dropship-autopilot` the project now? If yes, this repo's plan — Desk Set hero, Meta, the break-even
and kill rules — should be ported in as constraints or explicitly retired, not left to drift as a second
source of truth. If no, the autopilot is publishing to a live storefront on a plan nobody has written down.
