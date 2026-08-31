# Sciama gothic metric and bottom-up etherodynamics

This repository contains the original paper and its independently reviewed,
executable scientific companion.

- [Paper (PDF)](2026-08-29_sciama_gothic_metric_bottom_up_etherodynamics_v1.0.pdf)
- [Purpose-aware review](REVIEW.md)
- [Corrected construction](campaigns/P248-sciama-gothic-metric-audit/evidence/solution.md)
- [Complete 34-unit claim inventory](campaigns/P248-sciama-gothic-metric-audit/evidence/claim-inventory.yaml)
- [Claim-by-claim adjudication](campaigns/P248-sciama-gothic-metric-audit/evidence/claim-results.yaml)
- [Primary-source audit](campaigns/P248-sciama-gothic-metric-audit/evidence/literature-audit.md)
- [Independent review record](campaigns/P248-sciama-gothic-metric-audit/reviews/C-GOT-001-C-GOT-006-review.md)

## Result

The paper contains useful exact relaxed-GR and optical-metric structure, but
its full etherodynamic interpretation is not established as written. The
review resolves all 34 argumentative units: 15 are established at their stated
scope, 13 are refuted by a named algebraic or physical mechanism, and 6 remain
blocked by one explicitly named microscopic or empirical construction.

The executable repair preserves the strongest positive result. It adds an
independent positive lapse to obtain a complete ten-field optical ADM chart,
derives the exact harmonic/material compatibility relation, corrects the
Newtonian energy-sign ledger, replaces additive index deviations with an exact
logarithmic unimodular shear, and proves that an invertible optical change of
variables preserves the Euler equations of any supplied covariant metric
action.

This is a complete conditional infrared presentation. It is not a derivation
of a microscopic ether, universal material coupling, Newton's constant, a
preferred foliation, or empirical equivalence with gravity.

## Reproduce the checks

Python 3.11 or newer is required.

```bash
python -m venv .venv
. .venv/bin/activate
python -m pip install -e '.[test]'
python campaigns/P248-sciama-gothic-metric-audit/companion/sympy_checks.py
python campaigns/P248-sciama-gothic-metric-audit/companion/numerical_checks.py
pytest
```

The exact suite runs 31 SymPy checks. The numerical suite runs 18 checks,
including eight independent positive-definite metric round trips, mesh
refinement, a sign mutation, and an independent DOP853 solve. The focused test
suite covers the public API and its domain guards.

The Lean 4.28/mathlib corroboration is pinned under `formal/`:

```bash
cd formal
lake build
lake env lean SubstrateFramework/OpticalGothic.lean
```

The block-map bijection and ten-component Jacobian use exact SymPy as the
primary oracle. Lean independently checks the finite compatibility, sign,
shear, nonzero-Jacobian, cancellation, and theorem-composition statements.

## Provenance

The source PDF has SHA-256
`cfbea3cdebc59da6fd898448cf04088c10b152abdb025702ce807e1c7f54ef89`.
The review was performed as Substrate Framework campaign P248 for
[issue #184](https://github.com/vantasnerdan/substrate-framework/issues/184),
independently approved and merged in
[PR #185](https://github.com/vantasnerdan/substrate-framework/pull/185), and
accepted as claims C-GOT-001 through C-GOT-006 in release `v0.170.0`.

The complete immutable campaign record is included here so the review's
purpose inventory, attempts, evidence, correction history, and validation
receipt remain inspectable beside the paper.
