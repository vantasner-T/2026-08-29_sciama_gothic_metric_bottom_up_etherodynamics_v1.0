# Standalone validation receipt

Validated on 2026-08-31 against target base
`807fc05c2bf10c15d8ef87de61b82dcf9dabf692` and the unchanged P248 source
boundary merged upstream at
`cdc09f90fd6f5922ea33d6751f923a4b719774b3`.

| Gate | Command | Result |
| --- | --- | --- |
| Editable package | `python -m pip install -e . --no-deps` | Pass; standalone package imports from `src/substrate_framework` |
| Exact verification | `python campaigns/P248-sciama-gothic-metric-audit/companion/sympy_checks.py` | Pass; 6 relaxed + 11 metric + 14 compatibility checks |
| Numerical verification | `python campaigns/P248-sciama-gothic-metric-audit/companion/numerical_checks.py` | Pass; 18 checks including eight SPD round trips, refinement, mutation, and DOP853 cross-check |
| Focused API tests | `python -m pytest` | Pass; 17 tests |
| Formal source | `lake env lean <target>/formal/SubstrateFramework/OpticalGothic.lean` in the identical pinned Lean 4.28/mathlib environment | Pass; no diagnostics |
| PDF identity | `sha256sum 2026-08-29_sciama_gothic_metric_bottom_up_etherodynamics_v1.0.pdf` | Pass; `cfbea3cdebc59da6fd898448cf04088c10b152abdb025702ce807e1c7f54ef89` |
| Patch hygiene | `git diff --check` | Pass |

The included upstream immutable receipt additionally records the full
Substrate Framework boundary: 8,090 Lean jobs, empty axiom footprint for
`commonMetricComposition`, 62 affected-consumer tests, and the 2,471-test full
repository suite. That broader receipt is provenance for accepted claims
C-GOT-001 through C-GOT-006; the table above is the independent standalone
replay performed in this repository.
