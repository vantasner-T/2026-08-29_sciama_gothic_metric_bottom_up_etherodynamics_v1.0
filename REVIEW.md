# Purpose-aware scientific review

## Overall assessment

The manuscript's useful core is a harmonic-coordinate dictionary between the
gothic inverse metric density and a determinant-constrained optical block
metric. That core is exact on its actual nine-field image. It does not by
itself establish a microscopic ether, universal coupling, or equivalence to
general relativity as a physical theory.

The repaired construction adds the missing lapse degree of freedom and yields
a genuine ten-to-ten optical ADM chart. Because its component Jacobian is
nonzero on the positive-lapse, positive-definite spatial domain, pulling back a
supplied covariant metric action loses no Euler equation. This supplies the
paper's intended conditional infrared role without relabeling an invertible
field redefinition as microscopic emergence.

Verdicts below are route-scoped. `Established` means the manuscript unit is
supported at the stated mathematical, historical, or conditional scope.
`Refuted` names a contradiction or counterexample under the stated premises.
`Blocked` identifies a missing construction without claiming the underlying
physical idea is false.

## Claim and purpose ledger

| Unit | Argumentative purpose | Verdict | Decisive result |
| --- | --- | --- | --- |
| S01 | Bound the paper as a dictionary, not a microscopic theory | Established | The source expressly does not vary a constitutive action or propose a new microscopic field equation. |
| S02 | Use Maxwell theory as the wave/gauge/conservation template | Established | Commuting flat derivatives gives current conservation once the Lorenz condition and wave equation hold. |
| S03 | Introduce the gothic relaxed Einstein equation | Established | The metric-density wave pair is standard in a fixed convention; it does not supply an optical material realization. |
| S04 | Separate harmonic gauge from total-source conservation | Established | Gauge and conservation are distinct exact implications, not interchangeable assumptions. |
| S05 | Type gothic and stress variables under coordinate changes | Established | Gothic inverse and densitized matter stress have contravariant density weight one; the gravitational complex is not a general tensor. |
| S06 | Explain why density weight one is useful | Established | It gives ordinary divergence, trace-reversed linearization, and coordinate-volume pairing, without proving uniqueness. |
| S07 | Bound the covariance of the relaxed presentation | Established | The written system is background-Poincare covariant, not generally diffeomorphism covariant in that form. |
| S08 | Motivate a gravitational pseudotensor | Established | Normal coordinates exclude a nonzero local first-derivative metric tensor; curvature and quasi-local constructions remain outside that no-go. |
| S09 | Interpret density factors as volume conversion | Established | The positive tetrad determinant equals metric volume density, but the determinant is not the full metric. |
| S10 | Select continuum mechanics and a preferred chart as ontology | Blocked | A typed microscopic continuum action and observable map selecting that chart are missing. |
| S11 | Import lump mechanics, worldlines, and universal free fall | Refuted | A cited metric inverse fails multiplication, a rigid translate does not yield an all-orders square root, and a null cone does not imply universal massive-lump coupling. |
| S12 | Separate wave-speed matching from gravitational back-reaction | Refuted | Determinant normalization does not match anisotropic interface impedance by direction and polarization, and it cannot determine Newton's constant. |
| S13 | Interpret density stress as a Piola transform | Refuted | First Piola stress also needs the inverse-transpose deformation gradient; volume multiplication alone is insufficient. |
| S14 | Recast equivalence principle as medium co-deformation | Blocked | Universal matter coupling, operational observables, and a derived substrate stress action are missing. |
| S15 | Define the optical block metric | Established | Positive spatial tensor, determinant-slaved lapse, and real flow give a Lorentzian metric on a nine-field constrained image. |
| S16 | Calibrate a mechanical stress with Newtonian energy | Refuted | No common action is supplied, and the printed positive gradient energy has the opposite sign from the required negative Newtonian energy. |
| S17 | Import the Landau-Lifshitz complex as nonlinear closure | Refuted | The advertised weak closure inherits the energy-sign contradiction; a coordinate self-source is not a microscopic stress. |
| S18 | Explain the flat operator, total source, and coupling | Blocked | A constitutive slow-field equation deriving the operator and lump-medium coupling is missing. |
| S19 | Identify material balance with covariant conservation | Blocked | One substrate action whose Noether current supplies both balances is missing. |
| S20 | Evaluate the Planck-cutoff dimensional ledger | Established | The printed numbers reproduce, while inserting the Planck length makes the result a consistency check rather than a prediction of Newton's constant. |
| S21 | Relate the coupling to Sciama's cosmic estimate | Established | This remains a conditional order-of-magnitude model with explicit cosmic matter and boundary assumptions. |
| S22 | Define a retarded nonlinear iteration | Established | The recurrence is valid for a conserved source with convergence retained as a hypothesis. |
| S23 | Argue bootstrap uniqueness and full metric equivalence | Refuted | Nine fields cannot cover ten metric components, and the cited bootstrap result does not derive a substrate spin-two mode or the printed polynomial. |
| S24 | Treat the background as physical rather than gauge | Blocked | A microscopic action and empirical observable map distinguishing physical background structure are missing. |
| S25 | Claim invertibility of the optical-metric dictionary | Refuted | `diag(-4,1,1,1)` with unit spatial block lies outside the determinant-slaved image; adding an independent lapse repairs the map. |
| S26 | Define the vacuum self-source on shell | Established | The on-shell identity is valid; using it as an off-shell definition cancels the field operator and leaves only the matter equation. |
| S27 | Substitute the optical variables into harmonic gauge | Refuted | The printed mixed-metric sign conflicts with the later continuity equation and mixes time-coordinate factors. |
| S28 | Reconcile gothic and material continuity | Refuted | The expansion drops an overall factor; with material-flow sign, joint continuity requires incompressibility rather than optical homogeneity. |
| S29 | Infer global homogeneity and other consequences | Refuted | A static spatially inhomogeneous profile with zero flow satisfies both local continuity equations. |
| S30 | Propose a weak isotropic mechanical closure | Refuted | Equation (55) gives positive Newtonian field energy, opposite to equation (18); the stress coefficient alone cannot repair a missing action. |
| S31 | Extend the closure with additive trace-free shear | Refuted | The `(4,2,1)` witness has nonzero additive trace; mean-subtracted logarithmic eigenvalues give an exact unimodular repair. |
| S32 | Claim a unique exact nonlinear optical closure | Refuted | The map is incomplete, the uniqueness premise is too strong, and the weak sector retains the sign contradiction. |
| S33 | Compose the dictionary into bottom-up etherodynamics | Blocked | A microscopic substrate action deriving universal matter, spin-two, constitutive stress, and observables is missing. |
| S34 | Declare the paper's open problems | Established | The source accurately leaves the constitutive action, coupling selection, residual gauge, expansion, and double-solution sector open. |

## Corrected positive construction

For coordinates `x^0 = c t`, dimensionless flow `v = V/c`, orientation
`s = +/-1`, positive lapse `N`, and symmetric positive-definite `gamma`, define

```text
g_00 = -N^2 + gamma_ij v^i v^j
g_0i = s gamma_ij v^j
g_ij = gamma_ij.
```

Then

```text
det(g) = -N^2 det(gamma)
g^00 = -1/N^2
g^0i = s v^i/N^2
g^ij = gamma^-1^ij - v^i v^j/N^2.
```

The inverse reconstruction is

```text
gamma = g_spatial
v = s gamma^-1 g_mixed
N^2 = -(g_00 - g_mixed^T gamma^-1 g_mixed).
```

Its component Jacobian is `-2 s N det(gamma)`, so it is nonsingular on the
declared domain. The paper's original map is recovered by the extra constraint
`N = det(gamma)^(-1/6)` and is therefore a valid codimension-one slice, not a
general chart.

For the compatibility, energy-sign, logarithmic-shear, and action-pullback
results, see the [full corrected construction](campaigns/P248-sciama-gothic-metric-audit/evidence/solution.md)
and the executable module in [optical_gothic.py](src/substrate_framework/optical_gothic.py).

## Accepted result boundary

The independent review accepted six results in Substrate Framework release
`v0.170.0`: constrained optical-gothic map (C-GOT-001), complete optical ADM
bijection (C-GOT-002), material-harmonic compatibility (C-GOT-003), Newtonian
sign ledger (C-GOT-004), logarithmic conformal/shear split (C-GOT-005), and the
conditional optical action-pullback theorem (C-GOT-006).

These results exclude microscopic substrate emergence, universal matter
coupling, selection of Newton's constant, preferred-background observables,
ether ontology, and empirical equivalence. Those are open scientific frontier,
not consequences of the corrected field chart.
