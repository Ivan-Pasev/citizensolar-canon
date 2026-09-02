# CitizenSolar Site Sync Queue R6D

**Status:** site-sync ready queue; deployed site repo still not exposed to connector.

## 1. Canonical Route Decision

```text
/whitepaper
=
canonical public commercial / investor / procurement-safe storage-first CitizenSolar White Paper
```

```text
/resources/protocol-archive
=
bounded archive for SSRL, token utility, proof, quorum, ζπθ governance, zk/PQ roadmap, and advanced protocol material
```

## 2. Required Site Patch Order

1. Read current deployed site repository structure.
2. Identify route implementation for `/whitepaper`.
3. Replace top-level `/whitepaper` body with `WHITEPAPER.md` doctrine.
4. Create `/resources/protocol-archive` or equivalent route for legacy protocol material.
5. Update `/resources` card order so canonical White Paper is first-class.
6. Update related-route cards on Finance-Fit, Five-Score, Orchestrator, BYOS, BESS, Storage Bank, CEB, Security, Suppliers, and Intake pages.
7. Update page metadata, OpenGraph, sitemap, llms routing, and assistant/topic routing.
8. Run claim-boundary validation.
9. Run build and route validation.
10. Report exact files changed and unresolved holds.

## 3. Required Public Copy Kernel

CitizenSolar is a storage-first distributed energy infrastructure platform for the software-defined grid.

It helps municipalities, C&I operators, energy communities, EPCs, and public-sector buyers evaluate, package, and operate compliant solar-storage systems using trusted hardware, secure telemetry, deterministic orchestration, supplier-risk screening, finance-readiness evidence, and Community Energy Bank reporting.

CitizenSolar does not present the current platform as a live regulated market-dispatch system, certified financial infrastructure, autonomous grid-control system, token sale, or final engineering/procurement/tax/legal approval authority.

## 4. Required Validation Strings

Search deployed output for these terms and confirm each use is negated, restricted, archived, or otherwise bounded:

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

## 5. Blocker

R6D blocker:

```text
DEPLOYED SITE REPOSITORY NOT EXPOSED TO CONNECTOR
```

Unblock by exposing or naming the actual deployed `citizen.solar` repository, or by applying the site patch locally and returning the changed repo for review.
