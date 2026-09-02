# CitizenSolar Canon

**Status:** Canon RC0.1 — public doctrine stabilized before implementation.

This repository is the public upstream authority for the CitizenSolar ecosystem. It defines the storage-first thesis, allowed claims, source discipline, maturity boundaries, repo boundaries, and release gates that downstream website and implementation repositories must follow.

CitizenSolar is a storage-first distributed energy infrastructure platform for the software-defined grid. It helps municipalities, C&I operators, energy communities, EPCs, and public-sector buyers evaluate, package, and operate compliant solar-storage systems using trusted hardware, secure telemetry, deterministic orchestration, supplier-risk screening, finance-readiness evidence, and Community Energy Bank reporting.

## Canon-First Rule

```text
CANON
→ WEBSITE / PUBLIC ROUTES
→ SAFE PUBLIC SKELETONS
→ PRIVATE IMPLEMENTATION REPOS
→ SIMULATION
→ PILOT-READY DEVELOPMENT
```

No implementation repo should exceed this canon's public claims, maturity level, safety boundary, or source discipline.

## RC0.1 Canon Files

| File | Role |
|---|---|
| `CANON.md` | Canonical doctrine, claim IDs, system map |
| `WHITEPAPER.md` | Public commercial / investor storage-first white paper |
| `BLUEPAPER.md` | Public-safe technical architecture and control boundary |
| `LIGHTPAPER.md` | Forwardable investor/customer summary |
| `CLAIM_BOUNDARIES.md` | Allowed, restricted, and forbidden claim language |
| `CLAIM_REGISTER.md` | Stable claim IDs and evidence class mapping |
| `SOURCE_REGISTER.md` | Source IDs, live-site anchors, market/regulatory evidence classes |
| `MATURITY_LADDER.md` | M0-M7 maturity definitions and allowed repo behavior |
| `REPO_ECOSYSTEM.md` | Public/private repo split and implementation dependencies |
| `RELEASE_CHECKLIST.md` | RC0.1 gate checks before public/site synchronization |
| `DIAGRAM_BACKLOG.md` | Figure queue for website, white paper, blue paper, and deck |
| `ROADMAP.md` | Canon-first roadmap and next phases |
| `SECURITY.md` | Public repository security policy |
| `LICENSE_POLICY.md` | Content/code licensing policy |

## Current Implementation Hold

The following repos remain downstream and should not receive real control, firmware, trading, or deployment internals until the relevant canon gates are closed:

- `solarint-orchestrator`
- `solareye-edge`
- `ceb-ledger-core`
- `citizenvault-hardware`

`citizenvault-hardware` should be treated as sensitive. If it will contain BOM, CAD, test protocols, component choices, certification files, or manufacturing data, it should be private or split into a public documentation repo plus private engineering repo.

## Public Safety Boundary

This repo must not contain:

- firmware signing keys or device secrets;
- live grid-control logic;
- production dispatch algorithms;
- private supplier diligence files;
- customer/project data;
- P2P settlement credentials;
- live trading or market-dispatch code;
- deployment secrets, tokens, cloud credentials, or private infrastructure configuration.

## Canonical Doctrine

CitizenSolar is not a generic battery reseller.

CitizenSolar is a jurisdiction-fit, finance-aware, sovereign energy-system packager and secured deterministic orchestration layer for storage-first distributed grids.

Current public orchestration boundary:

```text
observe → explain → recommend → simulate → operator review → audit
```

Supervised execution is staged and bounded. Autonomous market action is future-only and disabled unless separately permitted, implemented, reviewed, certified where required, and governed.

## Current Release State

```text
CANON RC0.1:              CLOSED
PUBLIC CANON REPO:        POLISHED
CLAIM IDS:                ASSIGNED
SOURCE IDS:               ASSIGNED
MATURITY LADDER:          ASSIGNED
DIAGRAM BACKLOG:          CREATED
IMPLEMENTATION REPOS:     HOLD
SITE REPO:                NOT EXPOSED TO CONNECTOR
ECOSYSTEM ROOT REPO:      NOT EXPOSED TO CONNECTOR
```

## Next Gate

After RC0.1 review, synchronize the deployed website route:

- `/whitepaper` becomes the canonical storage-first public White Paper.
- `/resources/protocol-archive` preserves legacy SSRL/token/proof/quorum/governance material with boundaries.
- `/resources` cards point to the canonical papers and supporting routes.
- all website claims remain bounded by `CLAIM_BOUNDARIES.md` and `CLAIM_REGISTER.md`.
