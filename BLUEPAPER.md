# CitizenSolar Blue Paper RC0.1

**Technical Architecture for Storage-First Sovereign Energy Infrastructure**

**Status:** Canon RC0.1. Architecture-level, implementation-bounded, public-safe.

## 0. Purpose

The Blue Paper defines the CitizenSolar technical architecture without exposing private implementation details, firmware secrets, security-sensitive control logic, supplier-private records, customer/project records, or deployment credentials.

It is the architecture bridge between the public White Paper and downstream private implementation repositories.

## 1. System Layers

| Layer | Function | Public Boundary | Downstream repo |
|---|---|---|---|
| Physical Assets | PV, BESS, PCS/inverter, BMS, EMS, meter, EVSE, sensors | Descriptive only | `citizenvault-hardware`, future pack repos |
| Grid-Edge Trust | SolarEye, device identity, telemetry integrity, firmware/update state | Architecture only; no keys or firmware internals | `solareye-edge`, `ongrid-security` |
| Software Runtime | SolarINT OS, Mission Control, OnGrid Security, Onward Analytics | Product-level only | `solarint-os`, `citizensolar-mission-control`, `ongrid-security` |
| Orchestration | SolarINT Orchestrator, policy-bounded agents, action tiers | No live control code | `solarint-orchestrator` |
| Evidence/Governance | CEB ledgers, audit records, finance-fit records, supplier-risk records | No private data; no regulated settlement claim | `ceb-ledger-core`, `citizensolar-finance-fit`, supplier registry |
| Regional Pack Layer | EU/USA pack templates, AHJ/DSO notes, finance mapping | No final advice/approval | `citizensolar-energy-packs` |

## 2. Action Tiers

**Claim ID:** `CS-CLAIM-007`

| Tier | Name | Canonical Meaning | Current public status |
|---|---|---|---|
| T0 | Observe | Read telemetry and status | Allowed |
| T1 | Explain | Explain conditions, anomalies, and readiness | Allowed |
| T2 | Recommend | Recommend bounded operator actions | Allowed |
| T3 | Simulate | Simulate reserve, dispatch, and pack scenarios | Allowed |
| T4 | Supervised Execute | Requires validation, site review, authorization, and governance | Staged/future |
| T5 | Deterministic Fallback | Local safety fallback concept; no public control code | Staged/future |
| T6 | Autonomous Market Action | Future-only; disabled unless separately governed and permitted | Disabled |

## 3. Agent Taxonomy — Public-Safe

The canon may name agent classes, but not expose control internals.

| Agent | Public role | Boundary |
|---|---|---|
| Grid Sentinel | monitors site/grid posture | no privileged grid access described |
| Reserve Governor | evaluates reserve policies | no autonomous dispatch claim |
| Load Balancer | models load/storage scenarios | simulation/recommendation only |
| Forecast Agent | forecasts production/load/storage conditions | no market revenue guarantee |
| Firmware Quorum Agent | tracks firmware/update posture | no signing keys or procedures |
| BYOS Adapter Agent | classifies adapter readiness | no universal compatibility claim |
| Supplier-Risk Agent | maps supplier evidence and risk flags | no supplier approval claim |
| Community Ledger Agent | organizes CEB ledger records | no banking/settlement claim |
| Audit Scribe | records events and recommendations | no certification claim |
| Operator Relay | routes decisions to human/operator review | no autonomous control claim |
| Market Adapter Watcher | watches future market/flexibility paths | no live market-dispatch claim |

## 4. Event-State Machine

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

No state in this public Blue Paper implies certified engineering approval, procurement approval, funding approval, interconnection approval, cybersecurity certification, or live dispatch authority.

## 5. Minimum Public Data Model

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
  orchestration_tier: T0 | T1 | T2 | T3 | T4_staged | T5_staged | T6_disabled

pack:
  provider_fit: PF_A | PF_B | PF_C | PF_D | PF_X
  sovereign_stack: SOV_A | SOV_B | SOV_C | SOV_D | SOV_X
  finance_fit: FF_A | FF_B | FF_C | FF_D | FF_X
  orchestration_fit: OF_A | OF_B | OF_C | OF_D | OF_X
  ceb_fit: CEB_A | CEB_B | CEB_C | CEB_D | CEB_X
```

## 6. BYOS Interface Contract — Public Skeleton

BYOS adapter records may include the following public-safe fields:

| Field | Meaning | Public boundary |
|---|---|---|
| device_type | battery, inverter, PCS, BMS, EMS, meter, EVSE, sensor, controller | descriptive |
| telemetry_path | API, Modbus, CAN, MQTT, DNP3, IEC 61850, file export, manual evidence | no private credentials |
| control_path | none, advisory, supervised, automated, fallback-only | no live autonomous claim |
| cybersecurity_posture | identity, auth, encryption, firmware path, update authority | no exploit detail or keys |
| cloud_posture | vendor cloud, local gateway, EU-hosted, US-hosted, customer-hosted, unknown | no private config |
| warranty_service_route | supplier/service record | no endorsement |
| supplier_risk_status | candidate, screened, restricted, excluded | no final procurement approval |
| finance_constraints | public funding / credit / beneficiary constraints | no tax/legal advice |

## 7. Security Controls — Public Canon

The public canon may describe:

- device identity goals;
- telemetry integrity goals;
- firmware/update-state posture;
- remote-access review;
- audit records;
- operator approval boundaries;
- supplier-risk evidence;
- maturity labels;
- standards-aware design goals.

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

## 8. Integration Boundary

BYOS adapters normalize heterogeneous third-party assets for readiness review and orchestration classification. They do not imply universal compatibility, final compatibility, final safety approval, or final engineering approval.

## 9. Maturity Mapping

This Blue Paper may describe levels M0-M4 publicly and may reference M5-M7 only as external review/certification dependent. See `MATURITY_LADDER.md`.

## 10. Blue Paper Release Gate

A Blue Paper release is acceptable when it:

- matches `CANON.md` and `WHITEPAPER.md`;
- preserves public/private boundaries;
- avoids live control-code disclosure;
- defines data objects, states, and action tiers;
- maps each implementation domain to a downstream repo;
- keeps all claims bounded by `CLAIM_BOUNDARIES.md`;
- exposes only mock/skeleton schemas unless reviewed.
