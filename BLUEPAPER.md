# CitizenSolar Blue Paper

**Technical Architecture for Storage-First Sovereign Energy Infrastructure**

Status: Canon draft. Architecture-level, implementation-bounded, public-safe.

## Purpose

The Blue Paper defines the CitizenSolar technical architecture without exposing private implementation details, firmware secrets, security-sensitive control logic, supplier-private records, or deployment credentials.

## System Layers

| Layer | Function | Public Boundary |
|---|---|---|
| Physical Assets | PV, BESS, PCS/inverter, BMS, EMS, meter, EVSE, sensors | Descriptive only |
| Grid-Edge Trust | SolarEye, device identity, telemetry integrity, firmware/update state | Architecture only |
| Software Runtime | SolarINT OS, Mission Control, OnGrid Security, Onward Analytics | Product-level only |
| Orchestration | SolarINT Orchestrator, policy-bounded agents, action tiers | No live control code |
| Evidence/Governance | CEB ledgers, audit records, finance-fit records, supplier-risk records | No private data |
| Regional Pack Layer | EU/USA pack templates, AHJ/DSO notes, finance mapping | No final advice/approval |

## Action Tiers

| Tier | Name | Canonical Meaning |
|---|---|---|
| T0 | Observe | Read telemetry and status |
| T1 | Explain | Explain conditions, anomalies, and readiness |
| T2 | Recommend | Recommend bounded operator actions |
| T3 | Simulate | Simulate reserve, dispatch, and pack scenarios |
| T4 | Supervised Execute | Future/staged, requires validation and authorization |
| T5 | Deterministic Fallback | Local safety fallback, not public control code |
| T6 | Autonomous Market Action | Future-only, disabled unless separately governed |

## Agent Taxonomy

- Grid Sentinel
- Reserve Governor
- Load Balancer
- Forecast Agent
- Firmware Quorum Agent
- BYOS Adapter Agent
- Supplier-Risk Agent
- Community Ledger Agent
- Audit Scribe
- Operator Relay
- Market Adapter Watcher

## Event-State Machine

```text
SITE_REGISTERED
→ ASSET_DISCOVERED
→ TELEMETRY_BASELINED
→ SUPPLIER_SCREENED
→ FINANCE_FIT_REVIEWED
→ ORCHESTRATION_READINESS_CLASSIFIED
→ PACK_PROPOSED
→ OPERATOR_APPROVED_FOR_PILOT
→ PILOT_MONITORED
→ REPORT_ISSUED
```

No state in this public Blue Paper implies certified engineering approval, procurement approval, funding approval, interconnection approval, or live dispatch authority.

## Minimum Public Data Model

```yaml
site:
  jurisdiction: string
  buyer_class: municipality | c_i | sme | cooperative | epc | public_sector
  use_case: backup | peak | self_consumption | community_storage | resilience | congestion
  maturity: concept | review | proposed_pack | pilot | operational_review

asset:
  asset_type: pv | bess | inverter | pcs | bms | ems | meter | evse | controller | gateway
  supplier_status: candidate | screened | partner | restricted | excluded
  telemetry_status: unknown | observed | baselined | degraded | unavailable
  orchestration_tier: T0 | T1 | T2 | T3 | T4 | T5 | T6_disabled

pack:
  provider_fit: PF_A | PF_B | PF_C | PF_D | PF_X
  sovereign_stack: SOV_A | SOV_B | SOV_C | SOV_D | SOV_X
  finance_fit: FF_A | FF_B | FF_C | FF_D | FF_X
  orchestration_fit: OF_A | OF_B | OF_C | OF_D | OF_X
  ceb_fit: CEB_A | CEB_B | CEB_C | CEB_D | CEB_X
```

## Security Controls — Public Canon

The public canon may describe:

- device identity goals;
- telemetry integrity goals;
- firmware/update-state posture;
- remote-access review;
- audit records;
- operator approval boundaries;
- supplier-risk evidence;
- maturity labels.

The public canon must not expose:

- signing keys;
- key rotation procedures;
- private firmware builds;
- exploit details;
- production dispatch code;
- private credentials;
- private site diagrams;
- customer telemetry;
- privileged infrastructure configuration.

## Integration Boundary

BYOS adapters normalize heterogeneous third-party assets for readiness review and orchestration classification. They do not imply universal compatibility or final safety approval.

## Blue Paper Release Gate

A Blue Paper release is acceptable when it:

- matches the White Paper doctrine;
- preserves public/private boundaries;
- avoids live control-code disclosure;
- defines data objects, states, and action tiers;
- maps to the repository ecosystem;
- keeps all claims bounded.
