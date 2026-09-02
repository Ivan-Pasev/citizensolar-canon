# CitizenSolar Repository Ecosystem RC0.1

Status: canon-first map. Implementation repositories are downstream of the public canon.

## 1. Principle

The CitizenSolar ecosystem should not collapse into a single website repository.

A public website can publish doctrine, routes, product pages, resource pages, and investor-safe documents. It must not carry private firmware, device-security details, live orchestration logic, private supplier records, project/customer data, market-settlement internals, or deployment secrets.

## 2. Canon-First Dependency

```text
citizensolar-canon
  ↓ defines public doctrine, claims, maturity, boundaries
citizensolar-site / deployed website repo
  ↓ publishes bounded public website surfaces
implementation repos
  ↓ implement only after canon gates are clear
```

## 3. Current Accessible Repositories

| Repository | Visibility observed | RC0.1 role | Action |
|---|---:|---|---|
| `Ivan-Pasev/citizensolar-canon` | Public | public doctrine authority | Polish first |
| `Ivan-Pasev/solarint-orchestrator` | Private | orchestration implementation | Hold until canon/site sync |
| `Ivan-Pasev/solareye-edge` | Private | edge controller / telemetry trust | Hold until Blue/Security gate |
| `Ivan-Pasev/citizenvault-hardware` | Public | hardware standards/dev surface | Make private or split sensitive engineering |
| `Ivan-Pasev/ceb-ledger-core` | Private | CEB ledger/accounting implementation | Hold until legal/claim gate |

The connector has not yet exposed separate `citizensolar-site` or `citizensolar-ecosystem` repositories.

## 4. Recommended Repositories

| Repository | Visibility | Purpose | Upstream Gate |
|---|---:|---|---|
| `citizensolar-canon` | Public | White Paper, Blue Paper, Light Paper, claim boundaries, source register | Root |
| `citizensolar-site` | Public | Deployed `citizen.solar` website and public routes | Canon RC0.1 |
| `citizensolar-ecosystem` | Public after sanitization | Federation map, repo index, roadmap, cross-repo ADRs | Canon RC0.1 |
| `solarint-orchestrator` | Private | Operator-supervised deterministic orchestration | White/Blue/Claim |
| `solareye-edge` | Private | SolarEye controller, device identity, telemetry trust stack | Blue/Security |
| `citizenvault-hardware` | Private initially | Hardware standards, BOM/CAD/test protocols, BESS integration | Blue/Standards |
| `ceb-ledger-core` | Private initially | CEB seven-ledger model and governed shared-capacity accounting | White/Claim/Legal |

## 5. Recommended Next Repositories

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

## 6. Public / Private Rule

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

## 7. Sensitive Domain Rules

### Hardware

`citizenvault-hardware` should be private if it will contain BOM, CAD, component choices, assembly procedures, testing procedures, manufacturing files, certification evidence, lab notes, or supplier-specific details.

Safe public hardware content may include high-level standards posture, non-sensitive diagrams, public product briefs, and claim-bounded roadmaps.

### Orchestration

`solarint-orchestrator` should remain private. Public canon may define action tiers, agent taxonomy, and operator-supervised boundaries, but not real dispatch logic, production control code, market-control code, or privileged integrations.

### P2P / CEB / trading

`ceb-ledger-core` and any `p2p-energy-market-sim` repo must avoid live settlement claims. Public material should say simulation, future pathway, governed allocation, or reporting unless there is a separately regulated, permitted, reviewed, and operational system.

## 8. Release Rule

No implementation repo may publish public claims that exceed `CLAIM_BOUNDARIES.md`.

No implementation repo may become the authoritative doctrine source. The public doctrine source is `citizensolar-canon`, synchronized with the canonical Google Drive working tree.

## 9. Next Structural Need

Create or expose:

```text
Ivan-Pasev/citizensolar-site
Ivan-Pasev/citizensolar-ecosystem
```

or explicitly bind their real repository names in this file.
