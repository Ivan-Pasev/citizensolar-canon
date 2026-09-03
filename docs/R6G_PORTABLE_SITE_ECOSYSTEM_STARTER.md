# R6G — Portable Site + Ecosystem Starter

**Status:** Portable unblock package created.

## Why this exists

The deployed `citizen.solar` site repository and the `citizensolar-ecosystem` root repository are still not exposed through the connector. The available GitHub connector can edit files/issues in exposed repositories, but it does not expose a repository-creation action.

Therefore R6G creates a portable starter pack for manual creation or local application.

## Current accessible repos

- `Ivan-Pasev/citizensolar-canon` — public canon authority.
- `Ivan-Pasev/solarint-orchestrator` — private HOLD skeleton seeded.
- `Ivan-Pasev/solareye-edge` — private HOLD skeleton seeded.
- `Ivan-Pasev/citizenvault-hardware` — public-safe HOLD; visibility action required before engineering content.
- `Ivan-Pasev/ceb-ledger-core` — private HOLD skeleton seeded.

## Still missing

- `Ivan-Pasev/citizensolar-site`
- `Ivan-Pasev/citizensolar-ecosystem`

## Portable pack contents

The local R6G starter pack contains:

```text
README_R6G.md
citizensolar-site-starter/README.md
citizensolar-site-starter/src/app/whitepaper/page.mdx
citizensolar-site-starter/src/app/resources/protocol-archive/page.mdx
citizensolar-site-starter/src/data/citizensolar/resourceCards.patch.ts
citizensolar-site-starter/src/data/citizensolar/claimBoundaries.ts
citizensolar-site-starter/scripts/check-citizensolar-claims.mjs
citizensolar-site-starter/SITE_SYNC_CHECKLIST.md
citizensolar-ecosystem-root/README.md
citizensolar-ecosystem-root/REPO_INDEX.md
citizensolar-ecosystem-root/docs/adr/ADR-0001-canon-first.md
citizensolar-ecosystem-root/docs/boundaries/IMPLEMENTATION_HOLD.md
citizensolar-ecosystem-root/docs/release/R6G_STATUS.md
```

## Application rule

Do not start live implementation in `solarint-orchestrator`, `solareye-edge`, or `ceb-ledger-core` until:

1. deployed site repository is exposed or `citizensolar-site` is created;
2. `/whitepaper` is synchronized to Canon RC0.1;
3. `/resources/protocol-archive` exists;
4. public claim-boundary validation passes;
5. ecosystem root records the dependency graph and HOLD rules.

## Next gate

R6H should either:

- apply this starter pack to newly exposed/created repos; or
- continue improving canon/public documents while site repo remains blocked.
