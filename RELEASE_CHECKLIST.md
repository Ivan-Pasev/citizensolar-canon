# CitizenSolar Canon RC0.1 Release Checklist

This checklist must pass before the canon is used to drive website synchronization or implementation repo work.

## 1. Canon Coherence

- [x] `README.md` identifies the repo as the public upstream doctrine authority.
- [x] `CANON.md` defines identity, category, pack formula, five-score gate, CEB boundary, finance-fit boundary, and repo boundary.
- [x] `WHITEPAPER.md` is storage-first, investor-readable, and procurement-safe.
- [x] `BLUEPAPER.md` defines architecture without exposing private implementation details.
- [x] `LIGHTPAPER.md` is concise and forwardable with boundary.
- [x] `CLAIM_BOUNDARIES.md` defines allowed, restricted, and forbidden claim language.
- [x] `CLAIM_REGISTER.md` assigns stable claim IDs.
- [x] `SOURCE_REGISTER.md` assigns source IDs and refresh rules.
- [x] `MATURITY_LADDER.md` defines M0-M7 levels.
- [x] `REPO_ECOSYSTEM.md` defines public/private repo roles.
- [x] `DIAGRAM_BACKLOG.md` defines figure queue.

## 2. Required Website Synchronization

- [ ] Replace live `/whitepaper` with storage-first canonical White Paper.
- [ ] Move legacy SSRL/token/proof/quorum/governance content to `/resources/protocol-archive` or `/technical/protocol-reference`.
- [ ] Update `/resources` cards so the canonical White Paper is first-class.
- [ ] Update metadata, sitemap, llms routing, assistant routing, and related links.
- [ ] Run public claim-boundary search on the deployed site.

## 3. Required Repo Synchronization

- [x] Seed `citizensolar-canon` with public canon files.
- [ ] Confirm/create `citizensolar-site` or identify the deployed live-site repo.
- [ ] Confirm/create `citizensolar-ecosystem` root repo.
- [ ] Make `citizenvault-hardware` private or split public docs from private engineering if it will contain BOM/CAD/test/certification details.
- [ ] Keep `solarint-orchestrator`, `solareye-edge`, and `ceb-ledger-core` private until implementation gates close.

## 4. Claim Boundary Checks

Search public files for unsupported unbounded phrases before release:

- `autonomous grid control`
- `guaranteed funding`
- `guaranteed grants`
- `guaranteed tax credits`
- `guaranteed savings`
- `guaranteed grid revenue`
- `certified compliant`
- `approved supplier`
- `live regulated market dispatch`
- `production mainnet`
- `active token sale`
- `regulated settlement`
- `deposit-taking bank`

Allowed when explicitly negated or marked as forbidden/restricted in `CLAIM_BOUNDARIES.md`.

## 5. Source Refresh Checks

Refresh source evidence before any public/investor release:

- storage additions / market scale;
- IEA grid/flexibility evidence;
- EU CRA implementation dates and obligations;
- EU battery regulation and battery passport status;
- EU high-risk inverter/PCS public-funding restrictions;
- U.S. §48E / domestic content / PFE / FEOC guidance;
- DOE/USDA funding programs;
- supplier current status;
- competitor current positioning.

## 6. RC0.1 Decision

```text
CANON RC0.1: CLOSED
SITE SYNC: PENDING
IMPLEMENTATION REPOS: HOLD
P2P/TRADING: SIMULATION/FUTURE ONLY
HARDWARE ENGINEERING: PRIVATE OR PUBLIC-SAFE ONLY
```
