# Working agreement — dropship

## Always end with a paste-able status block

**Every response ends with a fenced ``` block headed `STATUS FOR CLAUDE.AI`.** The user pastes it into a
claude.ai chat so that chat can steer this work. Write it standalone — assume the reader has no context
from this session and cannot see the repo.

It must carry, briefly:
- **State** — what phase, what's built, money spent, anything ordered
- **Decided** — confirmed limits and locked choices
- **Open** — decisions waiting on the user, each a clear question
- **Next** — what I do when unblocked
- **Needed** — access or information I'm missing

Keep it under ~40 lines. It is a steering aid, not a re-read of the documents.

## Locked parameters — answer these from here, don't re-ask

Set by the user 2026-09-17. A browser chat with no context may ask for them again; paste these back.

| Parameter | Value |
|---|---|
| Total test budget (X) | **$1,000** all-in — ads, samples, platform |
| Daily ad cap (Y) | **$30 per product** |
| No-sale cutoff (Z) | **$60 spent, zero sales** |
| ROAS read (N) | **3 days AND ≥$90 spent AND ≥3 purchases** — all three, or the read defers |
| Test duration | **10 days per product**, one product at a time, never concurrent |
| Approval limit (W) | **$50** — and any paid tool at any price |
| Target market | **US only** |
| Supplier | **CJdropshipping** primary · DSers / AutoDS backup |
| Ad platform | **Meta first** |
| Samples | Not pre-approved. Each needs sign-off; **the user places every order** |
| Payouts / banking | Never mine, under any instruction |

**Current hero:** felt Desk Set, $75. The $69 desk cable kit was dropped 2026-09-17 — Amazon Prime
already sells the bundle. Dog car kit ($79) is the pivot, pending the niche decision in
`phase2-bundles-and-access.md` §0.

## Standing rules for this project

- **Spend nothing.** No orders, no signups, no subscriptions, no ad spend. Present costs for approval;
  the user places every order. Anything over $50 needs explicit sign-off, and paid tools need sign-off
  at any price.
- **Never touch payouts, banking, or payment settings.** Not at any stage, under any instruction.
- **Label every figure `[EST]` or `[QUOTED]`.** A `[QUOTED]` figure needs a source URL and a date.
  Unmarked guesses are worse than gaps. Never present an estimate as a fact.
- **Don't invent demand signals.** This environment's egress proxy blocks supplier and trend sites, and
  there's no ad-account access. If a number can't be verified from here, say so rather than producing a
  plausible one.
- **Honest copy only** — no fake scarcity, fake reviews, invented claims, or safety/medical claims that
  can't be backed. Flag anything that risks a platform policy strike.
- **Correct errors plainly** in the affected document, not just in chat.

## Where things live

| File | Contents |
|---|---|
| `research/phase1-shortlist.md` | 6 screened candidates, 4 dropped with decision record (rev 3) |
| `research/phase2-bundles-and-access.md` | Economics, break-even math, budget, access plan, niche decision |
| `research/cj-quote-worksheet.md` | Blank worksheet converting `[EST]` → `[QUOTED]` |
| `research/deskset-check-brief.md` | **Current** brief — paste into a browser chat to validate the hero |
| `research/handoff-brief.md` | Superseded by `deskset-check-brief.md`; kept for the check method |

Branch: `claude/affectionate-shannon-5954qk`.
