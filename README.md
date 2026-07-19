# Proving Ground

> **Status:** live public repo, deploy-ready (`vercel --prod`). Seeded from the internal audit
> trail at `portfolio/programs/2026-07-16-fable-window/T6-proving-ground/LEDGER.md` (private
> vault — that copy is the historical record of how each row was decided; this repo is now the
> canonical public copy going forward).

A public, falsifiable record of claims we make about our own products, each backed by
*executed evidence* — a touchstone dossier, a pre-registered eval with a p-value, or a
machine-verification count re-derivable from a named artifact. It is legally clean
self-attestation (we only attest to our own claims), an FTC-substantiation defense file, an
insurance file, and the distribution brand every launch inherits.

The ledger content (8 rows + 3 pending rows) lives directly in `index.html` here. New rows get
added to this repo going forward — it is the source of truth, not a mirror.

## The one rule

A claim enters this ledger only with evidence a third party can re-derive without trusting
us. No claim rests on model assertion. Same doctrine as `touchstone/dossier@0`: absence of
proof is `UNVERIFIABLE`, never a pass. A claim we can't yet substantiate is listed as
**PENDING** — naming the gap is itself the discipline.

## How a launch inherits this

Every product launch cites the ledger row(s) that substantiate its public claims, and adds
its own claims as new rows *with evidence attached*. A claim in launch copy with no ledger
row is a bug — the copy overclaims. This is the FTC-substantiation posture made mechanical:
we can show the executed evidence for every superlative we ship.

## This directory

- `index.html` — the whole site. Single file, no build step, no framework.
- `vercel.json` — static deploy config. One command away once a repo/domain exists:

  ```bash
  vercel --prod
  ```

- `LEDGER.md` (T6 folder, linked above) — the authored source. Update it there; port new
  rows into `index.html` verbatim when the ledger changes.
