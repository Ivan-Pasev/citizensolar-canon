# CitizenSolar Canon Roadmap

## Current Decision

Finish and polish the canon before developing sensitive implementation repositories.

## Phase C0 — Canon Seed

Status: active.

Deliverables:

- `README.md`
- `CANON.md`
- `WHITEPAPER.md`
- `BLUEPAPER.md`
- `LIGHTPAPER.md`
- `CLAIM_BOUNDARIES.md`
- `SOURCE_REGISTER.md`
- `REPO_ECOSYSTEM.md`
- `ROADMAP.md`

## Phase C1 — Canon Polish

Polish the public papers into investor/reviewer form:

- remove duplicated prose;
- add numbered sections;
- add figure captions;
- add source IDs;
- add claim IDs;
- align route copy with live `citizen.solar` pages;
- preserve older protocol material under archive/reference status.

## Phase C2 — Canon Release Candidate

Create release candidate:

```text
CitizenSolar Canon RC0.1
```

Required checks:

- White Paper matches public website direction;
- Blue Paper does not expose sensitive implementation details;
- Light Paper is forwardable to investor/customer/partner;
- Claim boundaries pass;
- source register is current;
- repo ecosystem map is aligned with created repos;
- no implementation repo claims exceed canon maturity.

## Phase C3 — Site Synchronization

After canon is polished:

- update `/whitepaper` route;
- create `/resources/protocol-archive` or `/technical/protocol-reference`;
- update `/resources` cards;
- update metadata, sitemap, llms routing, and assistant routing;
- run public-site validation.

## Phase C4 — Implementation Repo Skeletons

Only after C1/C2:

- seed safe public READMEs for implementation repos;
- define each repo's boundary from the canon;
- create private issue boards;
- add security policy and no-secrets guidance;
- add mock-only schemas where safe;
- postpone real control/firmware/P2P internals until review.

## Phase C5 — Technical Development

Begin controlled technical work:

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
