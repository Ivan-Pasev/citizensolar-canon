# CitizenSolar R6F — Downstream Skeletons and Site Block

**Status:** R6F closed as site-blocked / downstream-skeleton pass.

**Date:** 2026-09-03 Europe/Sofia.

## 1. Purpose

R6F rechecked whether the deployed `citizen.solar` site repository or ecosystem root repository had become accessible. It then initialized only safe downstream implementation skeletons because the deployed site repository remains unbound.

## 2. Repository Exposure

Accessible CitizenSolar repositories:

| Repository | Visibility | R6F action |
|---|---:|---|
| `Ivan-Pasev/citizensolar-canon` | Public | added this R6F report |
| `Ivan-Pasev/solarint-orchestrator` | Private | added HOLD README |
| `Ivan-Pasev/solareye-edge` | Private | added HOLD README |
| `Ivan-Pasev/citizenvault-hardware` | Public | public-safe HOLD README already exists |
| `Ivan-Pasev/ceb-ledger-core` | Private | added HOLD README |

Still not exposed:

```text
Ivan-Pasev/citizensolar-site
Ivan-Pasev/citizensolar-ecosystem
```

## 3. Site Sync Status

The canon is ready to drive website synchronization, but the deployed site repository remains unidentified / unexposed to the connector.

No live site route was changed in R6F.

Required next site actions remain:

1. bind or expose the deployed `citizen.solar` repository;
2. replace `/whitepaper` with Canon RC0.1 storage-first White Paper;
3. create `/resources/protocol-archive` for legacy SSRL/token/proof/quorum/governance material;
4. update `/resources`, related route cards, metadata, sitemap, llms routing, and assistant routing;
5. run public claim-boundary validation and build checks.

## 4. Downstream Skeleton Rule

Implementation repositories are allowed to hold only public-safe governance material until gates close.

Forbidden before gates close:

- live grid-control code;
- dispatch integrations;
- firmware, keys, credentials, secure-element material;
- real telemetry, customer/site data, supplier-private records;
- BOMs, CAD, Gerbers, schematics, manufacturing files;
- live trading, settlement, token-sale, production-mainnet logic;
- safety bypasses or unreviewed control policies.

## 5. R6F Final Gate

```text
SITE REPO: NOT EXPOSED
ECOSYSTEM ROOT: NOT EXPOSED
CANON: CLOSED
PRIVATE IMPLEMENTATION README SKELETONS: SEEDED
IMPLEMENTATION CONTENT: HOLD
HARDWARE PUBLIC VISIBILITY: ACTION REQUIRED BEFORE ENGINEERING CONTENT
```

## 6. Next Recommended Cycle

R6G should either:

1. bind the exact deployed website repository and apply the site-sync queue; or
2. if still blocked, create a complete local `citizensolar-site` starter patch pack and `citizensolar-ecosystem` root skeleton pack for manual GitHub creation/application.
