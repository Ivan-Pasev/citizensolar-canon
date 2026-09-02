# CitizenSolar Site Synchronization Plan — RC0.1

This plan is downstream of Canon RC0.1.

## Target Route Decision

```text
/whitepaper
=
canonical public commercial / investor / procurement-safe storage-first CitizenSolar White Paper
```

## Archive Route Decision

```text
/resources/protocol-archive
=
bounded technical archive for SSRL, token utility, proof, quorum, governance, zk/PQ roadmap, and advanced protocol material
```

## Required Website Tasks

1. Replace `/whitepaper` hero and body with the RC0.1 storage-first White Paper.
2. Move legacy protocol/token/proof/quorum/governance content into an archive/reference route.
3. Update `/resources` so the White Paper is the canonical commercial paper.
4. Link supporting resources:
   - Energy System Packs
   - Five-Score Pack Screening
   - Finance-Fit Review
   - Supplier Candidate Registry
   - Supplier Candidate Intake
   - SolarINT Orchestrator
   - Orchestration Readiness Review
   - Storage Bank
   - Community Energy Bank
   - BYOS
   - BESS
   - Security
5. Update metadata, sitemap, llms routing, assistant routing, and related links.
6. Run claim-boundary review against `CLAIM_BOUNDARIES.md`.

## Required Public Boundary

```text
CitizenSolar describes a storage-first platform, product architecture, and pilot-ready packaging model. It does not represent a live regulated market-dispatch system, certified financial infrastructure, active token sale, production mainnet, autonomous grid-control system, or final engineering/procurement/tax/legal approval authority.
```

## Site Sync Hold

The live site repo is not currently exposed to the connector as `citizensolar-site`. Until the exact deployed website repo is bound, this canon repo is the authoritative source for the replacement content but not proof of live-site mutation.
