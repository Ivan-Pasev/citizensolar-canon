# CitizenSolar Canon Roadmap RC0.1

## Current Decision

Finish and polish the canon before developing sensitive implementation repositories.

```text
CANON
→ WEBSITE / PUBLIC ROUTES
→ SAFE PUBLIC SKELETONS
→ PRIVATE IMPLEMENTATION REPOS
→ SIMULATION
→ PILOT-READY DEVELOPMENT
```

## Phase C0 — Canon Seed

Status: complete.

Seeded public files:

- `README.md`
- `CANON.md`
- `WHITEPAPER.md`
- `BLUEPAPER.md`
- `LIGHTPAPER.md`
- `CLAIM_BOUNDARIES.md`
- `SOURCE_REGISTER.md`
- `REPO_ECOSYSTEM.md`
- `ROADMAP.md`
- `SECURITY.md`
- `LICENSE_POLICY.md`

## Phase C1 — Canon Polish / RC0.1

Status: complete.

R6C added:

- RC0.1 labels;
- reduced duplication between White / Blue / Light papers;
- stable claim IDs;
- source IDs;
- maturity ladder;
- release checklist;
- diagram backlog;
- stronger public/private repo boundaries;
- implementation hold rules.

## Phase C2 — Canon Review

Status: next.

Review checklist:

- read all RC0.1 files as one system;
- verify claim IDs and source IDs are internally consistent;
- verify live-site `/whitepaper` replacement remains public-safe;
- verify `citizenvault-hardware` visibility decision;
- decide whether to create/expose `citizensolar-site` and `citizensolar-ecosystem`;
- decide whether to tag/publish Canon RC0.1 after manual review.

## Phase C3 — Site Synchronization

After canon review:

- update `/whitepaper` route;
- create `/resources/protocol-archive` or `/technical/protocol-reference`;
- update `/resources` cards;
- update metadata, sitemap, llms routing, and assistant routing;
- run public-site validation.

## Phase C4 — Implementation Repo Skeletons

Only after C1/C2:

- seed safe public/private READMEs for implementation repos;
- define each repo's boundary from the canon;
- create private issue boards;
- add security policy and no-secrets guidance;
- add mock-only schemas where safe;
- postpone real control/firmware/P2P internals until review.

## Phase C5 — Simulation Work

Begin controlled non-production technical work:

- SolarINT Orchestrator simulation layer;
- SolarEye telemetry simulator;
- CEB ledger mock model;
- hardware standards checklist;
- BYOS adapter mock catalog;
- Mission Control prototype UI;
- finance-fit workflow prototype.

## Gate

Do not build the sensitive stack before the canon is stable.

The canon tells every repo what it is allowed to say, what it is allowed to expose, and what maturity level it can claim.
