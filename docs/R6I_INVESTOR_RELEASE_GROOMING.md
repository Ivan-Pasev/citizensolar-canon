# R6I - Investor Release Grooming

Status: completed as an export/polish lane because the deployed site repo and ecosystem root repo remain unavailable through the connector.

## Scope

R6I does not mutate the live CitizenSolar website and does not start private implementation development. It packages the current Canon RC0.1 material into a more serious investor-ready export pack.

## Repository exposure check

Accessible CitizenSolar repositories remain:

- `Ivan-Pasev/citizensolar-canon`
- `Ivan-Pasev/solarint-orchestrator`
- `Ivan-Pasev/solareye-edge`
- `Ivan-Pasev/citizenvault-hardware`
- `Ivan-Pasev/ceb-ledger-core`

Still not exposed:

- `Ivan-Pasev/citizensolar-site`
- `Ivan-Pasev/citizensolar-ecosystem`

## Export pack contents

The local R6I export pack contains:

- `CitizenSolar_White_Paper_RC0.1_R6I.docx`
- `CitizenSolar_White_Paper_RC0.1_R6I.pdf`
- `CitizenSolar_Blue_Paper_RC0.1_R6I.docx`
- `CitizenSolar_Blue_Paper_RC0.1_R6I.pdf`
- `CitizenSolar_Light_Paper_RC0.1_R6I.docx`
- `CitizenSolar_Light_Paper_RC0.1_R6I.pdf`
- `figures/fig_stack.png`
- `figures/fig_loop.png`
- `figures/fig_gate.png`
- `figures/fig_ceb.png`
- `README_R6I.md`
- `R6I_RELEASE_GATE.md`

## Additions over R6H

R6I adds:

- polished title pages;
- embedded diagrams;
- claim appendix;
- source appendix;
- release gate file;
- visual render QA across all pages.

## Diagram set

1. Storage-first operating stack.
2. SolarINT operator-supervised loop.
3. Five-score pack gate.
4. Community Energy Bank seven-ledger map.

## Gate state

PASS:

- Canon RC0.1 basis verified from `WHITEPAPER.md`, `BLUEPAPER.md`, `LIGHTPAPER.md`, `CLAIM_REGISTER.md`, and `SOURCE_REGISTER.md`.
- DOCX exports rendered to PDFs.
- Visual contact sheets generated and inspected.
- No visible clipping, overlap, broken tables, or missing footer boundary observed.

HOLD:

- live `/whitepaper` replacement not applied;
- `citizensolar-site` not exposed;
- `citizensolar-ecosystem` not exposed;
- implementation repos remain HOLD;
- `citizenvault-hardware` remains public-safe only unless made private before engineering content.

## Next recommended cycle

R6J - either bind/apply the missing site and ecosystem repositories, or promote this release pack into Drive-distributed investor materials with a source appendix and diagram backlog for the pitch deck.
