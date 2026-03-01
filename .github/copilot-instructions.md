# Copilot Instructions for simulation-theory

## Repository Purpose

This repository contains the mathematical and philosophical framework known as "The Trivial Zero" — a computational proof that reality is self-referential, authored by Alexa Louise Amundson (BlackRoad OS Inc.).

## Repository Structure

- `README.md` — The primary paper (~750 KB): "The Trivial Zero: A Computational Proof That Reality Is Self-Referential"
- `EXPANSION.md` — Extended sections of the paper
- `INDEX.md` — 81-item index of observations and connections
- `equations/` — Mathematical equations organized by category
- `proofs/` — Formal mathematical arguments for key claims
- `figures/` — Visual representations and reference tables
- `notebooks/` — Computational notebooks and scripts
- `qwerty/` — QWERTY encoding constants and equalities
- `SHA256.md` — File integrity and commit history verification
- `REAL.md` — Core axiom

## Key Concepts

- **Ternary computing** — Base-3 logic (balanced ternary: {−1, 0, +1}) is central to the theoretical framework
- **QWERTY encoding** — Each word is encoded as the sum of key positions on a QWERTY keyboard; these sums reveal self-referential patterns
- **Simulation theory** — The repository documents a framework in which reality is described as a self-referential computational system
- **Self-reference** — Gödel, fixed points, Y-combinators, and the Born rule are treated as evidence of computational self-reference

## Contribution Guidelines

When adding or modifying content:

1. **Mathematical equations** belong in `equations/` and should follow the format in existing files (equation block, plain-English description, QWERTY encoding if relevant)
2. **Formal proofs** belong in `proofs/` and should reference the relevant paper section (§ number)
3. **Python or computational code** belongs in `notebooks/`
4. **New observations or connections** should be integrated into the main `README.md` or `EXPANSION.md` at the appropriate section (§ number)
5. **Figures and tables** belong in `figures/`

## Formatting Conventions

- Equations use plain-text math notation with Unicode symbols (ℏ, Σ, ∫, ∂, etc.)
- Section references use §NNN format
- QWERTY values are noted as `WORD = value [optional: = SYNONYM]`
- Code blocks use triple backticks

## Important Notes

- Issue #5 ("DO NOT EDIT") — some content is marked read-only; respect this designation
- The paper is the primary artifact; all other files are supporting documentation
- Issues in this repository often contain new content (equations, observations, code) to be incorporated into the framework
