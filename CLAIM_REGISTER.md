# CitizenSolar Claim Register RC0.1

Stable claim IDs for the CitizenSolar public canon.

| Claim ID | Claim | Evidence class | Public status | Boundary |
|---|---|---|---|---|
| `CS-CLAIM-001` | CitizenSolar is a storage-first distributed energy infrastructure platform for the software-defined grid. | `SOURCE-LIVE`, `SOURCE-INTERNAL` | Allowed | Identity claim, not performance guarantee |
| `CS-CLAIM-002` | CitizenSolar packages compliant solar-storage systems using trusted hardware, secure telemetry, deterministic orchestration, supplier-risk screening, finance-readiness evidence, and CEB reporting. | `SOURCE-LIVE`, `SOURCE-INTERNAL` | Allowed | Use `designed for review` / `readiness` language where compliance is not certified |
| `CS-CLAIM-003` | CitizenSolar is not a generic battery reseller; it is a jurisdiction-fit, finance-aware energy-system packager and secured deterministic orchestration layer. | `SOURCE-INFERENCE`, `SOURCE-LIVE` | Allowed | Strategic positioning, not market-share claim |
| `CS-CLAIM-004` | Storage is the operating layer of the next distributed grid. | `SOURCE-MARKET`, `SOURCE-OFFICIAL`, `SOURCE-INFERENCE` | Allowed | Timing thesis only; no revenue/savings guarantee |
| `CS-CLAIM-005` | Energy System Packs combine compliant hardware, CitizenSolar software, supplier-risk screen, regulatory map, finance-fit record, EPC handoff, orchestration boundary, and CEB readiness. | `SOURCE-LIVE`, `SOURCE-INTERNAL` | Allowed | Pack candidate/review language only |
| `CS-CLAIM-006` | Every serious pack should carry five readiness scores: provider fit, sovereign stack, finance fit, orchestration fit, and CEB fit. | `SOURCE-LIVE`, `SOURCE-INTERNAL` | Allowed | Scores are not approvals/certifications/guarantees |
| `CS-CLAIM-007` | SolarINT Orchestrator is operator-supervised and policy-bounded with observe/explain/recommend/simulate/operator-review/audit as current public boundary. | `SOURCE-LIVE`, `SOURCE-INTERNAL` | Allowed | No current autonomous grid-control claim |
| `CS-CLAIM-008` | Community Energy Bank is a governed shared-storage operating model with seven ledgers. | `SOURCE-LIVE`, `SOURCE-INTERNAL` | Allowed | Not a bank, investment product, token system, return product, or regulated settlement service |
| `CS-CLAIM-009` | Finance-Fit Review maps funding routes, tax-credit evidence, beneficiary compliance, ownership options, supplier-risk posture, and readiness evidence. | `SOURCE-LIVE`, `SOURCE-OFFICIAL`, `SOURCE-INTERNAL` | Allowed | Not tax/legal/procurement/accounting/funding authority |
| `CS-CLAIM-010` | Supplier Candidate Registry and Intake support supplier evidence review and five-score screening. | `SOURCE-LIVE`, `SOURCE-INTERNAL` | Allowed | Candidate/screened status only unless documented partnership exists |
| `CS-CLAIM-011` | The public canon repo is upstream doctrine and must not contain secrets, control code, customer data, private supplier files, or live settlement logic. | `SOURCE-INTERNAL` | Allowed | Repository safety rule |
| `CS-CLAIM-012` | Implementation repos remain downstream until canon gates close. | `SOURCE-INTERNAL` | Allowed | Development governance rule |
| `CS-CLAIM-013` | P2P energy trading is currently a simulation/future-pathway architecture unless separately regulated, permitted, and implemented. | `SOURCE-INTERNAL`, `SOURCE-OFFICIAL` | Restricted | No live market/settlement claim |
| `CS-CLAIM-014` | Hardware standardization and CitizenVault development are architecture domains, not public certified product claims until reviewed. | `SOURCE-INTERNAL`, `SOURCE-OFFICIAL` | Restricted | Treat BOM/CAD/test/certification details as sensitive |

## Review Rule

Any new public claim must be either:

1. mapped to an existing claim ID;
2. added here with evidence class and boundary; or
3. held until review.
