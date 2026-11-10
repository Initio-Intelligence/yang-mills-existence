## Analysis of the first retained Schur cancellation

This note gives the supporting arguments for [first schur tilt trial](first_schur_tilt_trial.md) and
[first energy cancellation](first_energy_cancellation.md). The finite-dimensional cutoff argument in
ST.1–ST.12 and EC0.2–EC0.12 is correct. The statements below identify the
quadratic, the independent coordinates, the source collar and the exact
normalization to which it applies. The scope is the original first step,
globally P/Q regular, with a bounded R-only birth neighborhood. It is not
an assertion about an arbitrary inherited T-operation.

## 1. The literal source quadratic

CMP119, printed p.254, (1.29), has the retained exponent

\[
 -\frac12\langle A,KA\rangle
 +\frac12\langle A,K C^{(0)}(\Lambda_1)K A\rangle,
 \qquad K=C^*\Delta_1C.
 \tag{SA.1}
\]

The sign of the second term is as printed. Put O=Λ₁ and let D be the remaining actual free
coordinates. The covariance in (SA.1) is the Dirichlet inverse K_OO⁻¹,
extended by zero. Thus (SA.1) is exactly −E₀, where

\[
 E_0(a)=\tfrac12a^{\mathsf T}
    (K_{DD}-K_{DO}K_{OO}^{-1}K_{OD})a.
 \tag{SA.2}
\]

It is the untruncated Schur quadratic. The integral in (1.26) also has
the actual complement cutoff after completing the square. That factor
is retained in the complete E/B terms and in the renormalization
identity (1.26)–(1.30). A proof may undo that entire identity, or keep
its completion factor; it may not set the factor to one.

At (2.21), printed p.258, the first component operation keeps its
diagonal Schur block, while cross-component entries are assigned to B.
For a single first retained component this is exactly (SA.2). For
several components, cancellation of the joint Schur quadratic is also
exact if all its cross terms are retained. Replacing it by the sum of
diagonal blocks requires the actual separated geometry. With the source
MR₁ gap, bounded total first rank n_D=O(R₁⁴), and |a|≤CP, exponential
covariance decay gives

\[
 |E_{\rm joint}(a)-E_{\rm diag}(a)|
      \le C n_D P^2e^{-cMR_1}=o(1).
 \tag{SA.3}
\]

This does not authorize dropping a completion force from separately
conditioned external first components. Such a force must be kept or
bounded in the actual conditional density.

## 2. The first relocalization is harmless for this tilt, with its factors kept

CMP119 (1.21)–(1.24), pp.251–252, changes the first retained free
coordinate near the boundary of its Q chart. The reference displacement
H is O(ε₁ exp(−cMR₁)); after division by g₀ the free-coordinate
displacement is O(P exp(−cMR₁)). The source keeps the determinant (1.24)
in B and explicitly says that its free R characteristic functions are
unchanged. These are exact statements about the transformation; no
cutoff approximation is required.

The Schur precision has a fixed upper bound. Consequently on the
actual encompassing domain |a|≤CP,

\[
 |E_0(a_{\rm old})-E_0(a_{\rm new})|
       \le C n_D P^2e^{-cMR_1}=o(1).
 \tag{SA.4}
\]

There is a stronger fact for the lower box in EC0.7: its witnesses have
norm 5P/4 and its other coordinates have a fixed O(1) bound. The smooth
switch in (1.22) is zero below the printed threshold 4P/3. For large P
the change is therefore exactly the identity on that whole box. The
first determinant is one there, rather than an omitted extra factor.
Elsewhere its actual determinant and the inverse pullback of any mark
must still be retained, once only.

## 3. Which entries are genuinely independent

CMP119 p.249, (1.14)–(1.15), defines the free field on Ω₁* after the
exceptional entries have been removed. The embedding C restores those
entries and satisfies QCA=0. Every assignment of the independent
Ω₁* entries is therefore an allowed input to the nonlinear constraint
solve. One must not impose an additional QA=0 on that independent
vector. A proposed assignment to all physical bond entries, before
the embedding, would need a separate constraint check.

The special cochain seed of RT.1 is a convenient physical construction
whose full-bond field already satisfies the linear constraint. It is
not a necessary restriction on the independent-coordinate boxes used
in RB.3 or EC0.7. If an axial tree has been fixed sharply, its entries
are absent from the independent list; if the source uses the soft gauge
integral, those entries receive ordinary small balls.

## 4. Exact R patterns, the source collar, and the bounded domain

For every positive R pattern in the bounded neighborhood, choose in each
bad test a free coordinate not belonging to any good-test footprint.
Such a coordinate exists by nonemptiness of the pattern. A fixed-width
ball about a vector of norm 5P/4 at each chosen coordinate, and fixed
small balls about zero elsewhere, realizes every good and bad alternative
of the pattern. Coincident witnesses can be merged. The number of
bad-test cubes in a bounded MR₁ neighborhood is bounded by a fixed
source constant.

The chosen coordinates lie inside the complete enlarged bad-test
footprints. The source first retained region adds an MR₁ layer beyond
their region cover. The hierarchy M≫LM₂ leaves a positive MR₁ collar
between all such witnesses and the regular complement. Rectangular
hulls only enlarge this buffer. It is wider than the fixed range of
the primitive flat K=C*Δ₁C: C has the fixed block stencil and Δ₁ has the
fixed local action/gauge stencil. Therefore

\[
 K_{OD}a_{\rm witness}=0
 \tag{SA.5}
\]

exactly in the flat first precision. Only the O(1) boundary noise of
the trial box contributes to K_OD a. Its conditional-mean completion
cost is at most C n_D by the uniform gap and row bound. This verifies
the hypothesis ST.5 with no P² cost and no outside-volume factor.

The Q characteristic functions are starred and exclude exceptional
entries. On each remaining free entry either a good R test imposes P,
or the surviving Q test imposes (2+o(1))P, by the local-reference
comparison in (1.19). Thus the whole actual post-cancellation first
integration domain is contained in |a|≤CP. There is no uncanceled,
unbounded exceptional-coordinate direction. Its Lebesgue volume is at
most (CP)^{n_D}; the powers of g and all coarea/normalization factors
remain at their literal positions in (1.29) and (1.71).

## 5. Local flat comparison and normalization

The RMg/RK buffered precision estimate gives, on the first
native regular chart and after its block-adjoint local gauge,

\[
 \|S_D(V)^u-S_{D,\rm flat}\|
       \le C(R_1^2\varepsilon_1+e^{-cR_1}),
 \quad
 |E_0(V,a)-E_0^G(a)|
       \le C n_DP^2(R_1^2\varepsilon_1+e^{-cR_1})=o(1).
 \tag{SA.6}
\]

Block-adjoint rotations preserve the literal R norms and the product
balls. Combining (SA.1)–(SA.6) with the exact symmetric outside-cutoff
lemma proves EC0.12:

\[
 b_R(V;e^{E_0})\ge e^{-C n_D-o(1)}.
 \tag{SA.7}
\]

The definition of b_R is crucial: its numerator is the actual first
R-sector integral and its denominator is the same all-small first
integral Z_P(V) used in RB.10–RB.14. The extensive complement-cutoff
factor cancels through that denominator. It is not an independent
all-Q-good probability normalization. In the annular reassembly Z_P
must remain a factor of the later measure before (SA.7) is used.

**Conclusion.** The weighted first-step lower bound and its identification
with the literal retained Schur energy hold at this scope.
The complete later-energy upper and the comparison of two geometric
quiet masks are separate theorems. The analysis supplies no uniform
microscopic marked-carrier assertion.

## Primary sources

- CMP119 pp.249–254, (1.14)–(1.29), and p.258, (2.21).
- [first birth relative weights](first_birth_relative_weights.md), RB.1–RB.16, for the actual Q
  sandwich, R pattern and common Z_P denominator.
- [first step relative marginal](first_step_relative_marginal.md), RMg.28–RMg.35, and the RK Schur
  estimate for the quantitative local gauge comparison.
- [first schur tilt trial](first_schur_tilt_trial.md), ST.1–ST.12, and
  [first energy cancellation](first_energy_cancellation.md), EC0.1–EC0.12, for the
  finite-dimensional cutoff and weighted-defect proof.
