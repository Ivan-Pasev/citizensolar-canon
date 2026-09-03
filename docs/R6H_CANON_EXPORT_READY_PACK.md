# R6H Canon Export-Ready Pack

**Status:** CLOSED / export-ready fallback lane.

## Why this exists

`citizensolar-site` and `citizensolar-ecosystem` remain unavailable to the connector. Therefore R6H did not mutate the live website and did not create the missing repositories.

Instead, R6H advances the valid fallback: polished investor/customer review exports from Canon RC0.1.

## Output pack

Local sandbox artifact:

```text
CitizenSolar_R6H_CANON_EXPORT_READY_PACK.zip
```

Pack contents:

```text
CitizenSolar_White_Paper_RC0.1_R6H.docx
CitizenSolar_White_Paper_RC0.1_R6H.pdf
CitizenSolar_Blue_Paper_RC0.1_R6H.docx
CitizenSolar_Blue_Paper_RC0.1_R6H.pdf
CitizenSolar_Light_Paper_RC0.1_R6H.docx
CitizenSolar_Light_Paper_RC0.1_R6H.pdf
README_R6H.md
R6H_RELEASE_GATE.md
```

## Visual QA

DOCX files were rendered to page PNGs and PDFs. Render check passed:

- White Paper: 3 pages
- Blue Paper: 3 pages
- Light Paper: 2 pages

No visible clipping, overlap, broken tables, missing boundary footer, or unreadable table defects were found in the contact-sheet review.

## Source basis

The exports are condensed from Canon RC0.1 public files:

- `WHITEPAPER.md`
- `BLUEPAPER.md`
- `LIGHTPAPER.md`
- `CLAIM_BOUNDARIES.md`
- `CLAIM_REGISTER.md`
- `SOURCE_REGISTER.md`
- `REPO_ECOSYSTEM.md`

## Boundary

These documents are canon-stage investor/customer review materials. They are not legal, tax, accounting, engineering, procurement, interconnection, banking, settlement, cybersecurity-certification, market-dispatch, or funding-approval advice.

## Still blocked

- deployed `citizen.solar` site repo not exposed;
- `citizensolar-ecosystem` root repo not exposed;
- live `/whitepaper` still needs replacement;
- `citizenvault-hardware` remains public and must not receive engineering artifacts until visibility is fixed.

## Next valid cycle

R6I should either:

1. bind/expose/create `citizensolar-site` and `citizensolar-ecosystem`, then apply the R6G starter and site-sync queue; or
2. continue Drive-side investor-pack polish: diagrams, title pages, source appendix, and final PDF/DOCX release grooming.
