# Security Policy

**Status:** RC0.1 public canon security policy.

This repository is public doctrine and documentation only.

Do not place secrets, firmware keys, infrastructure credentials, customer records, private telemetry, supplier-private diligence, live dispatch code, market-settlement credentials, or production control logic in this repository.

## Sensitive Domains

The following domains belong in private repositories unless explicitly sanitized:

- SolarEye firmware and device trust;
- SolarINT orchestration internals;
- OnGrid Security controls;
- CitizenVault hardware CAD/BOM/test files before release review;
- Community Energy Bank implementation internals;
- P2P/market simulation and settlement-adjacent logic;
- supplier evidence and private finance-fit files;
- deployment and CI/CD secrets.

## Hardware Visibility Warning

`citizenvault-hardware` is currently visible as a public repository in the accessible GitHub surface. If that repository will contain BOM, CAD, component choices, assembly procedures, testing protocols, supplier details, certification artifacts, lab data, or manufacturing files, it should be made private or split into:

```text
citizenvault-hardware-docs      public-safe brief/docs only
citizenvault-hardware-engineering private engineering files
```

## Reporting

For security issues, use private maintainer channels. Do not publish exploit details, keys, credentials, site-specific vulnerabilities, or third-party supplier-sensitive material in public issues.

## Canon Boundary

Public documentation may describe the security posture as standards-aware, evidence-oriented, operator-supervised, policy-bounded, and roadmap-driven. It must not claim cybersecurity certification unless a specific external certification exists.

## Implementation Hold

Until the canon advances beyond RC0.1 review, private implementation repositories should use placeholders, public-safe README files, and mock/simulation-only examples. No production secrets, live dispatch logic, firmware keys, or market-settlement code should be added through this public canon flow.
