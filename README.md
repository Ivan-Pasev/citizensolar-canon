# CitizenSolar Canon

Canonical public doctrine, whitepaper spine, claim boundaries, and repo-governance surface for the CitizenSolar ecosystem.

CitizenSolar is a storage-first distributed energy infrastructure platform for the software-defined grid. It helps municipalities, C&I operators, energy communities, EPCs, and public-sector buyers evaluate, package, and operate compliant solar-storage systems using trusted hardware, secure telemetry, deterministic orchestration, supplier-risk screening, finance-readiness evidence, and Community Energy Bank reporting.

## Current Status

```text
CANON-FIRST PHASE: ACTIVE
PUBLIC CANON REPO: SEEDED
IMPLEMENTATION REPOS: HOLD UNTIL CANON GATE
```

This repository is the public doctrine layer. It is not the deployed website repo, firmware repo, orchestration-control repo, hardware-CAD repo, trading engine repo, infrastructure repo, or supplier/private diligence database.

## Canon-First Rule

Before developing the sensitive implementation repositories, finish and stabilize the canon:

1. White Paper: public commercial/investor storage-first thesis.
2. Blue Paper: technical architecture and bounded implementation design.
3. Light Paper: concise investor/customer narrative.
4. Claim Boundaries: phrases allowed, phrases forbidden, maturity limits.
5. Repo Ecosystem Map: public/private repo responsibilities.
6. Source Register: evidence anchors and refresh discipline.

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

## Canonical Repositories

Initial ecosystem split:

| Repository | Visibility | Role |
|---|---:|---|
| `citizensolar-canon` | Public | Doctrine, papers, claim boundaries, source register |
| `citizensolar-site` | Public | Deployed website and public routes |
| `solarint-orchestrator` | Private | Operator-supervised deterministic orchestration |
| `solareye-edge` | Private | Edge controller and telemetry trust stack |
| `citizenvault-hardware` | Private initially | Hardware standards, BOM/CAD/test protocols |
| `ceb-ledger-core` | Private initially | Community Energy Bank ledger model and accounting logic |

## Canonical Doctrine

CitizenSolar is not a generic battery reseller. It is a jurisdiction-fit, finance-aware, sovereign energy-system packager and secured deterministic orchestration layer for storage-first distributed grids.

## Release Discipline

No implementation repo should claim production readiness until the canon defines:

- maturity level;
- allowed public claims;
- forbidden claims;
- external evidence anchors;
- integration boundaries;
- safety and legal review requirements.
