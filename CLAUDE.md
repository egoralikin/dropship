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
| `research/phase1-shortlist.md` | 7 screened candidates, 3 dropped with decision record |
| `research/phase2-bundles-and-access.md` | $60–80 bundles, break-even math, budget, access plan, Chrome playbook |
| `research/cj-quote-worksheet.md` | Blank worksheet converting `[EST]` → `[QUOTED]` |
| `research/handoff-brief.md` | Standalone brief to paste into a browser-capable Claude chat |

Branch: `claude/affectionate-shannon-5954qk`.
