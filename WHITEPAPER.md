# CitizenSolar White Paper RC0.1

**Storage-First Sovereign Energy Infrastructure for the Software-Defined Grid**

**Status:** Canon RC0.1. Public, commercial, investor-readable, procurement-safe.

## 0. Scope Boundary

CitizenSolar describes a storage-first platform, product architecture, and pilot-ready packaging model. It does not represent a live regulated market-dispatch system, certified financial infrastructure, active token sale, production mainnet, autonomous grid-control system, or final engineering/procurement/tax/legal approval authority.

## 1. Executive Thesis

**Claim ID:** `CS-CLAIM-001`, `CS-CLAIM-002`, `CS-CLAIM-003`

CitizenSolar is a storage-first distributed energy infrastructure platform for the software-defined grid.

It helps municipalities, C&I operators, energy communities, EPCs, and public-sector buyers evaluate, package, and operate compliant solar-storage systems using trusted hardware, secure telemetry, deterministic orchestration, supplier-risk screening, finance-readiness evidence, and Community Energy Bank reporting.

CitizenSolar is not a generic battery reseller. It is a software-led infrastructure company that turns fragmented hardware, fragmented financing, fragmented regulation, fragmented installer capacity, and fragmented grid-edge telemetry into jurisdiction-fit, finance-aware, software-attached storage-first energy infrastructure.

## 2. Why Storage First

**Claim ID:** `CS-CLAIM-004`

Solar generation alone is no longer the decisive infrastructure unit. The decisive unit is the governed solar-storage system: PV, BESS, inverter or PCS, BMS, EMS, meters, edge controllers, telemetry, software, cybersecurity, supplier-risk evidence, financing documentation, installer/EPC handoff, and post-installation operating governance.

Storage is not an accessory to solar. Storage is the operating layer of the next distributed grid.

Market evidence supports a storage-first timing thesis, but does not guarantee CitizenSolar revenue, adoption, savings, project approval, interconnection approval, or public-funding success.

## 3. Market and Grid Transition

**Source classes:** `SOURCE-MARKET`, `SOURCE-OFFICIAL`

Current public evidence supports the timing thesis:

- global energy storage has entered a 100-GW annual additions era;
- grid congestion, project queues, and interconnection delays are material constraints;
- battery storage, demand flexibility, co-location, and grid-enhancing approaches are increasingly treated as system levers;
- buyers need finance-ready, supplier-screened, cyber-aware packaging rather than isolated hardware procurement.

CitizenSolar should use market data as evidence of timing and category relevance, not as a direct forecast of company revenue.

## 4. Regulatory and Financing Shift

Energy infrastructure is becoming a cyber-physical, supplier-risk, and finance-documentation domain.

In the EU, battery regulation, cyber-resilience rules, NIS2 posture, high-risk inverter/PCS restrictions in public financing, public procurement, Modernisation Fund channels, and Net-Zero Industry Act industrial direction all push buyers toward documented, supplier-screened, compliant, and supportable systems.

In the USA, energy-storage credits, domestic-content bonus paths, FEOC/PFE material-assistance screens, DOE grid-resilience channels, USDA REAP routes, state-level storage incentives, AHJ/fire review, interconnection requirements, and remote-access scrutiny all push projects toward finance-ready evidence and supplier-origin clarity.

CitizenSolar turns regulation and financing into product inputs.

## 5. Platform Architecture

CitizenSolar’s platform has six public architecture layers:

| Layer | Function | Public Boundary |
|---|---|---|
| Physical energy assets | PV, BESS, inverter/PCS, BMS, EMS, meters, EVSE, switchgear, sensors | Descriptive; no final engineering approval |
| Grid-edge trust | SolarEye controllers/gateways, device identity, telemetry integrity, firmware/update posture | Architecture-level; no keys/secrets |
| Software fabric | SolarINT OS, SolarINT Orchestrator, Mission Control, OnGrid Security, Onward Analytics, Community Bank Portal | Product-level; no internal control code |
| Deterministic orchestration | policy-bounded observe/explain/recommend/simulate/operator-review/audit loop | No live autonomous control claim |
| Governance and evidence | CEB ledgers, audit records, finance-fit records, supplier-risk records, beneficiary records | No regulated banking/settlement claim |
| Regional execution | EU/USA pack templates, AHJ/DSO/interconnection notes, financing map, installer/EPC handoff | No legal/tax/procurement/permit guarantee |

## 6. Energy System Packs

**Claim ID:** `CS-CLAIM-005`

```text
CitizenSolar Energy System Pack
=
compliant local/native/allied hardware
+ CitizenSolar software stack
+ supplier-risk screen
+ regional regulatory map
+ finance-fit record
+ beneficiary compliance file
+ installer/EPC handoff
+ deterministic orchestration boundary
+ Community Energy Bank readiness
```

Pack naming grammar:

```text
CS-[MACRO]-[JURISDICTION]-[BUYER]-[USE]-[SIZE]-SOV-FIN
```

Example pack classes:

| Pack | Initial role |
|---|---|
| `CS-EU-BG-MUNI-CEB-250-SOV-FIN` | Bulgarian municipal CEB pilot candidate |
| `CS-EU-BG-SME-RESERVE-100-SOV-FIN` | SME reserve / weak-grid resilience candidate |
| `CS-EU-DE-COMMUNITY-STORAGE-250-SOV-FIN` | German community storage candidate |
| `CS-EU-NL-GRID-CONGESTION-500-SOV-FIN` | Netherlands congestion-relief storage candidate |
| `CS-US-TX-INDUSTRIAL-BACKUP-500-SOV-FIN` | Texas industrial backup candidate |
| `CS-US-CA-CI-PEAK-250-SOV-FIN` | California C&I peak/storage candidate |
| `CS-US-NY-MUNI-RESILIENCE-250-SOV-FIN` | New York municipal resilience candidate |
| `CS-US-RURAL-SME-REAP-50-SOV-FIN` | U.S. rural/agricultural REAP-aligned candidate |

## 7. Five-Score Pack Gate

**Claim ID:** `CS-CLAIM-006`

Every serious Energy System Pack must carry:

| Score | Screens |
|---|---|
| `CS-PROVIDER-FIT` | supplier, warranty, service, documentation, installation, integration readiness |
| `CS-SOV-STACK` | cyber/control-chain, firmware, cloud, remote access, jurisdiction, supplier-risk posture |
| `CS-FINANCE-FIT` | grants, loans, rebates, tax credits, domestic content, leases, PPAs, ESCO options, beneficiary evidence |
| `CS-ORCHESTRATION-FIT` | telemetry, device identity, reserve policy, audit trail, operator approval, action-tier readiness |
| `CS-CEB-FIT` | asset, capacity, reserve-policy, dispatch/event, allocation-report, assurance, governance ledger readiness |

Scores are readiness classifications for review, planning, and partner handoff. They are not approvals, certifications, funding guarantees, tax-credit qualifications, engineering approvals, procurement approvals, savings guarantees, or grid-revenue guarantees.

## 8. SolarINT Orchestrator

**Claim ID:** `CS-CLAIM-007`

SolarINT Orchestrator is CitizenSolar's deterministic orchestration layer for storage-first distributed energy systems.

It coordinates telemetry, reserve policy, BYOS assets, operator workflows, supplier-risk state, and Community Energy Bank ledgers. Its current public model is operator-supervised and policy-bounded.

Current action boundary:

```text
observe → explain → recommend → simulate → operator review → audit
```

Supervised execution is staged and bounded. Autonomous market action is future-only and disabled unless separately permitted, implemented, reviewed, governed, and certified where required.

## 9. Storage Bank and Community Energy Bank

**Claim ID:** `CS-CLAIM-008`

The Storage Bank is the commercial center of gravity: storage capacity is treated as an operating asset that can support resilience, self-consumption, public-benefit reporting, and future flexibility paths where allowed.

The Community Energy Bank is a governed shared-storage operating model with seven ledgers:

1. Asset Ledger
2. Capacity Ledger
3. Reserve-Policy Ledger
4. Dispatch/Event Ledger
5. Allocation-Report Ledger
6. Assurance Ledger
7. Governance Ledger

The Community Energy Bank is not a deposit-taking bank, investment product, speculative token system, guaranteed-return product, or regulated settlement service.

## 10. BYOS and Supplier Candidate Screening

**Claim ID:** `CS-CLAIM-010`

BYOS means Bring Your Own Storage. It is a controlled adapter model for third-party batteries, inverters, BMS, meters, EMS, EVSE, telemetry systems, and mixed fleets.

BYOS is not a universal compatibility claim. Each asset must be screened for device type, telemetry path, control path, cybersecurity posture, cloud dependency, remote-access capability, warranty route, service route, supplier-risk status, financing constraints, and orchestration tier.

Supplier pages and registries must treat suppliers as diligence candidates unless a documented partnership exists. Supplier inclusion does not mean approval, certification, procurement approval, funding eligibility, endorsement, or final compatibility.

## 11. Finance-Fit and Beneficiary Compliance

**Claim ID:** `CS-CLAIM-009`

CitizenSolar's Finance-Fit Energy System Review maps grants, loans, leases, tax-credit evidence, supplier-risk screening, beneficiary compliance, ownership options, and readiness evidence for a storage-first deployment.

It is a bounded readiness and packaging service. It does not provide tax advice, legal advice, accounting advice, procurement advice, final engineering advice, funding approval, grant awards, rebate confirmation, tax-credit qualification, loan approval, permit approval, interconnection approval, savings guarantee, or revenue guarantee.

## 12. Priority Strategy

EU priority markets:

- Bulgaria municipal Community Energy Bank pilots;
- Bulgaria SME reserve and weak-grid resilience packs;
- Germany community storage and cooperative finance;
- Netherlands grid-congestion storage packs;
- Spain co-located solar-storage and curtailment-reduction packs;
- France PV-storage hybrid and public resilience packs;
- Italy C&I self-consumption and lease/ESCO packs;
- Portugal grid-control and BESS modernization watch;
- Modernisation Fund country belt for future expansion.

USA priority markets:

- Texas industrial backup and ERCOT-readiness packs;
- California C&I peak and storage packs;
- New York municipal resilience packs;
- Florida hurricane resilience packs;
- Hawaii island storage and microgrid-readiness packs;
- rural/agricultural USDA REAP-aligned packs.

## 13. Partner and Pilot Pathways

Near-term commercial loop:

```text
Finance-Fit Review
→ Orchestration Readiness Review
→ jurisdiction-fit pack design
→ supplier/EPC partner quote
→ pilot deployment
→ monitoring subscription
→ Community Energy Bank reporting where applicable
```

Long-term scale path:

```text
screened partner hardware
→ co-branded compliant packs
→ licensed assembly
→ regional production cells
→ CitizenSolar-native SolarEye / controller / gateway production
→ software-attached storage fleet operations
```

## 14. Technical Archive Boundary

Earlier SSRL, token-utility, proof, quorum, governance, zk/PQ, and advanced roadmap material belongs in a bounded technical archive. It is not the canonical commercial White Paper and must not be presented as an active token sale, production mainnet, regulated settlement system, certified financial infrastructure, or live autonomous grid-control system.

Recommended live route:

```text
/resources/protocol-archive
```

## 15. RC0.1 Release Gate

This White Paper is RC0.1-ready when:

- it remains synchronized with `CANON.md`;
- every strategic claim maps to `CLAIM_REGISTER.md`;
- every current market/regulatory claim maps to `SOURCE_REGISTER.md`;
- claim boundaries are preserved;
- it can replace the live `/whitepaper` route without leading with protocol/token material;
- a reviewer can understand the product, boundary, first commercial wedge, and implementation hold.
