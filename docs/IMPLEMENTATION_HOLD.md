# CitizenSolar Implementation Hold — RC0.1

The implementation repositories are intentionally downstream of the canon.

## Hold Applies To

- `solarint-orchestrator`
- `solareye-edge`
- `ceb-ledger-core`
- `citizenvault-hardware`
- future `citizensolar-byos-adapters`
- future `citizensolar-finance-fit`
- future `citizensolar-supplier-registry`
- future `p2p-energy-market-sim`
- future `ongrid-security`
- future `citizensolar-infra`

## Allowed Before Canon Review

- public-safe README files;
- repo boundary statements;
- mock-only schemas;
- architecture references back to `citizensolar-canon`;
- non-sensitive issue planning;
- local-only prototypes not pushed to public surfaces.

## Not Allowed Before Canon Review

- production dispatch logic;
- live grid-control integrations;
- firmware signing keys;
- customer/project/site data;
- private supplier diligence;
- market-settlement credentials;
- regulated trading claims;
- final hardware BOM/CAD/test files in public repos;
- unsupported claims beyond `CLAIM_BOUNDARIES.md`.

## Resume Conditions

Implementation repos may move when:

1. Canon RC0.1 is reviewed;
2. website `/whitepaper` is aligned or scheduled for alignment;
3. repo boundaries are accepted;
4. security/no-secrets policies exist in each implementation repo;
5. claims map to `CLAIM_REGISTER.md`;
6. maturity labels map to `MATURITY_LADDER.md`.

## Canon Link

The upstream public doctrine source is:

```text
Ivan-Pasev/citizensolar-canon
```

No downstream repo should become the authoritative doctrine source.
