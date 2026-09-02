# CitizenSolar Repository Ecosystem

Status: canon-first map. Implementation repositories are downstream of the public canon.

## Principle

The CitizenSolar ecosystem should not collapse into a single website repository.

A public website can publish doctrine, routes, product pages, resource pages, and investor-safe documents. It must not carry private firmware, device-security details, live orchestration logic, private supplier records, project/customer data, market-settlement internals, or deployment secrets.

## Canon-First Dependency

```text
citizensolar-canon
  ↓ defines public doctrine, claims, maturity, boundaries
citizensolar-site
  ↓ publishes bounded public website surfaces
implementation repos
  ↓ implement only after canon gates are clear
```

## Initial Repositories

| Repository | Visibility | Purpose | Upstream Gate |
|---|---:|---|---|
| `citizensolar-canon` | Public | White Paper, Blue Paper, Light Paper, claim boundaries, source register | Root |
| `citizensolar-site` | Public | Deployed `citizen.solar` website and public routes | Canon |
| `solarint-orchestrator` | Private | Operator-supervised deterministic orchestration | White/Blue/Claim |
| `solareye-edge` | Private | SolarEye controller, device identity, telemetry trust stack | Blue/Security |
| `citizenvault-hardware` | Private initially | Hardware standards, BOM/CAD/test protocols, BESS integration | Blue/Standards |
| `ceb-ledger-core` | Private initially | CEB seven-ledger model and governed shared-capacity accounting | White/Claim/Legal |

## Recommended Next Repositories

| Repository | Visibility | Purpose |
|---|---:|---|
| `citizensolar-energy-packs` | Public/private split | Pack templates, scoring, jurisdiction packaging |
| `citizensolar-finance-fit` | Private initially | Finance-fit workflow, beneficiary evidence model |
| `citizensolar-supplier-registry` | Private initially | Supplier candidate records, intake, diligence state |
| `citizensolar-byos-adapters` | Private initially | Mixed-fleet adapters and compatibility screens |
| `ongrid-security` | Private | Cyber-physical assurance and security controls |
| `citizensolar-mission-control` | Private | Operator console and workflows |
| `citizensolar-simlab` | Public/private split | Simulations, demos, examples, public non-control models |
| `p2p-energy-market-sim` | Private initially | P2P and market simulations; no live settlement claim |
| `citizensolar-infra` | Private | CI/CD, cloud, secrets, deployment, environments |

## Public / Private Rule

Public repositories may contain:

- doctrine;
- public pages;
- non-sensitive schemas;
- mock data;
- public-safe simulations;
- documentation;
- bounded examples;
- claim checks;
- source references.

Private repositories should contain:

- firmware;
- hardware files not ready for disclosure;
- control logic;
- production orchestration;
- private supplier records;
- customer/project records;
- live dispatch integrations;
- real market interfaces;
- secrets and infrastructure configuration.

## Release Rule

No implementation repo may publish public claims that exceed `CLAIM_BOUNDARIES.md`.

No implementation repo may become the authoritative doctrine source. The public doctrine source is `citizensolar-canon`, synchronized with the canonical Google Drive working tree.
