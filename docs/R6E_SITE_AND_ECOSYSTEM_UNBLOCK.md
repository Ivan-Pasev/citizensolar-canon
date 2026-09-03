# CitizenSolar R6E — Site and Ecosystem Unblock Manifest

**Status:** R6E closed as site/ecosystem binding preparation.

**Date:** 2026-09-03 Europe/Sofia.

## 1. Purpose

R6E attempts to move from Canon RC0.1 into website synchronization and ecosystem-root binding.

The canon is ready. The deployed website repository is not exposed to the connector. The ecosystem-root repository is not exposed to the connector. Therefore, R6E does not mutate the live website and does not start private implementation work.

## 2. Current Verified Repository Surface

Accessible CitizenSolar repositories:

| Repository | Visibility | R6E status |
|---|---:|---|
| `Ivan-Pasev/citizensolar-canon` | Public | Canon RC0.1 authority |
| `Ivan-Pasev/solarint-orchestrator` | Private | Hold; no live control implementation |
| `Ivan-Pasev/solareye-edge` | Private | Hold; no firmware/secrets/public implementation |
| `Ivan-Pasev/citizenvault-hardware` | Public | Public-safe HOLD README added; make private or split before engineering files |
| `Ivan-Pasev/ceb-ledger-core` | Private | Hold; no live settlement/trading claims |

Missing / not exposed to connector:

```text
Ivan-Pasev/citizensolar-site
Ivan-Pasev/citizensolar-ecosystem
```

## 3. Required Binding Decision

Before site synchronization can be applied, one of the following must happen:

1. expose the actual deployed `citizen.solar` repository to the GitHub connector;
2. create `Ivan-Pasev/citizensolar-site` and bind it as the deployed site repository;
3. provide the exact current deployed-site repository full name;
4. apply the R5/R6 site patch locally and return the changed repository for review.

Before ecosystem coordination can be closed, one of the following must happen:

1. create `Ivan-Pasev/citizensolar-ecosystem`;
2. expose the already-created ecosystem root repository;
3. bind another exact repo name as the ecosystem root.

## 4. Canonical Route Patch To Apply Once Site Repo Is Available

```text
/whitepaper
=
canonical public commercial / investor / procurement-safe storage-first CitizenSolar White Paper
```

```text
/resources/protocol-archive
=
bounded archive for SSRL, token utility, proof, quorum, zeta-pi-theta governance, zk/PQ roadmap, and advanced protocol material
```

Required order:

1. read deployed site repository structure;
2. identify current `/whitepaper` route implementation;
3. snapshot or branch before mutation;
4. replace `/whitepaper` with `WHITEPAPER.md` doctrine from `citizensolar-canon`;
5. move legacy protocol material to `/resources/protocol-archive` or `/technical/protocol-reference`;
6. update `/resources` card ordering and related links;
7. update metadata, sitemap, llms routing, and assistant/topic routing;
8. run claim-boundary validation;
9. run build and route validation;
10. report exact files changed and unresolved holds.

## 5. Claim-Boundary Search Strings

The site patch must search deployed output for the following and confirm each use is negated, restricted, archived, or otherwise bounded:

- autonomous grid control
- guaranteed funding
- guaranteed grants
- guaranteed rebates
- guaranteed tax credits
- guaranteed loan approval
- guaranteed savings
- guaranteed grid revenue
- certified compliant
- approved supplier
- live regulated market dispatch
- active token sale
- production mainnet
- regulated settlement
- deposit-taking bank

## 6. Implementation Repo Hold

No private implementation repo should receive real firmware, live control logic, trading logic, settlement logic, secrets, supplier-private records, or customer/project data until:

1. the site repo is bound;
2. `/whitepaper` is synchronized with Canon RC0.1;
3. the protocol archive route is created;
4. the public claim-boundary check passes;
5. the hardware visibility decision is resolved.

## 7. R6E Final State

```text
CANON RC0.1: CLOSED
SITE SYNC: READY BUT BLOCKED BY SITE REPO EXPOSURE
ECOSYSTEM ROOT: READY BUT NOT EXPOSED/CREATED THROUGH CONNECTOR
IMPLEMENTATION REPOS: HOLD
HARDWARE VISIBILITY: ACTION REQUIRED
NEXT TARGET: SITE REPO BINDING OR ECOSYSTEM ROOT CREATION
```
