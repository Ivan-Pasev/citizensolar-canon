# CitizenSolar Claim Boundaries RC0.1

This file defines allowed language, restricted language, forbidden language, maturity language, and repo-boundary rules for the public CitizenSolar canon.

## 1. Allowed Public Claim Pattern

Use:

- storage-first distributed energy infrastructure;
- software-defined grid;
- standards-aware;
- designed for review;
- readiness classification;
- evidence package;
- supplier-risk screen;
- finance-fit review;
- beneficiary compliance mapping;
- operator-supervised;
- deterministic orchestration;
- policy-bounded;
- pilot-ready where applicable;
- roadmap toward stronger assurance.

## 2. Restricted Claims

These may be used only with explicit maturity and scope boundaries:

| Phrase | Required boundary |
|---|---|
| autonomous | Use only as future-only or explicitly disabled for current market action |
| execution | Use only as supervised/staged, never implied as live grid dispatch |
| compliance | Use standards-aware / designed-for-review unless certified by a named authority |
| finance-ready | Use as readiness/evidence packaging, not funding/tax/loan approval |
| supplier approved | Use only if a documented partnership or approval exists |
| Community Energy Bank | Must state it is not deposit banking, investment, or regulated settlement |
| P2P energy trading | Use only as simulation/research/future pathway unless regulated system exists |
| token / SSRL | Archive/reference only; not active sale or production mainnet |

## 3. Forbidden / Unsupported Current Claims

Do not claim:

- certified compliant unless a named certification exists;
- autonomous grid control as a current product;
- guaranteed funding;
- guaranteed grants;
- guaranteed rebates;
- guaranteed tax credits;
- guaranteed loan approval;
- guaranteed savings;
- guaranteed grid revenue;
- approved supplier status unless documented;
- final engineering approval;
- final procurement approval;
- tax advice;
- legal advice;
- accounting advice;
- cybersecurity certification;
- live regulated market dispatch;
- active token sale;
- production mainnet;
- regulated settlement service;
- deposit-taking banking service.

## 4. Required Boundary Text

Use this public boundary when describing current platform maturity:

```text
CitizenSolar describes a storage-first platform, product architecture, and pilot-ready packaging model. It does not represent a live regulated market-dispatch system, certified financial infrastructure, active token sale, production mainnet, autonomous grid-control system, or final engineering/procurement/tax/legal approval authority.
```

Use this boundary for scores:

```text
Scores are readiness classifications for review, planning, and partner handoff. They are not approvals, certifications, funding guarantees, tax-credit qualifications, engineering approvals, procurement approvals, savings guarantees, or grid-revenue guarantees.
```

Use this boundary for suppliers:

```text
Supplier inclusion means candidate or screened status only unless a documented partnership exists. It does not mean approval, certification, procurement approval, funding eligibility, endorsement, or final compatibility.
```

Use this boundary for the Community Energy Bank:

```text
The Community Energy Bank is not a deposit-taking bank, investment product, speculative token system, guaranteed-return product, or regulated settlement service.
```

Use this boundary for P2P / market material:

```text
P2P energy trading and market-adapter material is treated as simulation, research, or future-pathway architecture unless a separate regulated, permitted, reviewed, and operational system exists.
```

## 5. Repo Boundary

The public canon repo may describe architecture and maturity boundaries. It must not expose implementation secrets, control code, credentials, private customer data, private supplier data, or live market-settlement logic.

## 6. Enforcement Rule

Downstream repositories must reference this file before publishing public claims. If a claim is not listed in `CLAIM_REGISTER.md` or cannot be mapped to an allowed claim pattern here, the claim must remain internal until reviewed.
