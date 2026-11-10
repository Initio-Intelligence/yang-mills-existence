# Analysis of the residual strata construction
## 1. Scope

The proposed finite-cutoff construction is consistent with the literal source
coordinates after the representative, mixed-tree, and inner-boundary corrections
recorded below. It gives the hypotheses of Proposition RS.1 for the native old
current Wilson scalar on the **descriptor-erased** residual output. Thus that
particular erased output has no ambient continuous version of this native
conditional mark. A value assigned only on an inactive or null fiber cannot
repair the two different active limiting values.

This conclusion has two essential limits.

* The input in this construction is a local Wilson scalar of the old current
  field immediately before the replacement. It has not been identified with
  the scalar obtained by transporting the original microscopic F-01 field
  through the preceding history.
* The HS20 output can retain a newly sampled support-class descriptor. The two
  singular strata can then have different discrete labels. They need not be
  limits in a single fixed-label continuous chart. The exact lift in RS.4 is a
  legitimate repair of this particular topological obstruction. Its old
  normalized quotients, their extensions, and the full physical carrier cost of
  changing that label remain quantitative obligations.

Consequently this analysis does not supply a counterexample to all admissible M-03
augmentations, to the specific transported microscopic M-04 scalar, or to a
continuum Yang--Mills construction.

## 2. Source facts that matter for the preparation

### 2.1 The old current field is an actual retained variable

LFR I, printed pp.193--194, explicitly describes the operation as integration of
the current density with respect to the variables `V_k` on the prepared domain
`Λ`. It then regards the integrated expression as a function independent of
those variables. Formula (1.76) writes the resulting old integral in the mixed
coordinates `V''`; this coordinate change does not turn the former current
variable into an auxiliary fresh test variable. The block-average constraints
in CMP119 (2.21) give the same identification before their removal.

At fixed descriptor, the fresh factor therefore cancels from the old conditional
quotient exactly as in RS.1. Between descriptors it remains in the posterior.
The full output reference is shell Haar measure together with the fresh graph
slice, not a pointwise product of unrelated gauge delta functions.

### 2.2 The exact annular domain

The primary image of LFR I p.195 gives

\[
 \Lambda_0=\Lambda\cap\Omega_{h+1}^{\prime\prime\,\sim2},
 \qquad \mathbb B_0=\mathbb B''_k\cap\Lambda_0,
 \qquad V''=V'V_0,\quad V_0=M_{\mathbb B''_k}U_0.
 \tag{RSA.1}
\]

The source explicitly puts bonds crossing the outer boundary `∂Λ` in
`B_0`, and excludes bonds crossing the inner boundary. The excluded inner
region contains the padded old core. An informal replacement of `Λ_0` by
`Λ\Z_h`, or by `Λ∩Ω_{h+1}^c`, is not the literal formula and is unnecessary.
The birth seed is supported strictly farther inside the old core, with its gauge
transformation equal to the identity near the boundary. It is absent from the
relative coordinate (RSA.1).

### 2.3 Same-fine-lattice nesting, including representatives

CMP98 (42)--(43) defines higher averaging by successive composition. CMP119
p.255, (2.2), assigns the determining fields to the actual nested shells. The
source's domain convention assigns bonds intersecting a domain to that domain;
the averaging of a coarse bond uses its two adjacent fine blocks. With these
aligned blocks, a readout wholly outside the next regular region uses already
fixed lower-scale data, and a crossing readout belongs to the next shell.
Induction consequently gives the fiber inclusion stated in RS.3.

This argument compares constraints on one fine lattice. It does not compare
minimizers reconstructed on different lattices. The C-05 issue does not enter.

There is, however, a representative condition: uniqueness of a minimum **orbit**
does not identify arbitrary axial representatives. Choose the backward
stationary chain `V_{j-1}=M^{j-1}U_j(V_j)`, or keep the actual center-fixed
compensating gauges. They preserve the already fixed higher averages. With
these representatives the true old fluctuations vanish. CMP119
(3.17)--(3.19) controls the difference to the local test minimizers. The
center-fixed birth gauge can be inserted afterward, since it preserves the
complete first average and hence every higher average.

### 2.4 One mixed tree, with an additive path estimate

LFR I p.196 constructs one detoured coordinate tree in each rectangular
annulus, adds one bond joining it to the next annulus, and joins the outer tree
to its exterior anchor. Its union is the single tree `T_0`. A simple root path
cannot repeatedly leave and return to an annulus: the quotient of the annular
trees is a chain. The portion of the path in the `j`-scale annulus has length
at most `C M R_j`.

CMP98 Proposition 6, (164), is the needed uniform averaging estimate. Rescaled
to the `j`th intermediate average in final current units, it gives a bond
difference bounded by `C L^{j-k}a` when the fine normalized relative potential
is bounded by `a`. This is stronger than citing composition or gauge covariance
alone.

Tree transport of two unitary fields telescopes. In particular, the ratio of
their old and reference path transports obeys

\[
 \|u-I\|_\infty
 \le CM a\sum_{j=h}^{k}R_jL^{j-k}
 \le C_M R_k a .                                      \tag{RSA.2}
\]

The last inequality holds immediately on the constant-`R` plateau used in the
construction. It also follows from the polynomial comparison of neighboring
old `R_j` and the geometric factor. No product of `R_j` factors is present.
The same estimate handles the source's twisted relative field: the relevant
gauge is the ratio of the two path transports, and unitarity still gives the
additive telescoping bound.

For `a≤C_M ε_k exp(-cD)` and `D≥c_0 M R_k`, (RSA.2) is strictly smaller
than the actual preparation cutoff `δ'_k`. This proves the claimed `χ'`
margin without an unverified uniform bound on a succession of large gauges.

### 2.5 The reference tail and the literal artificial seam

LFR I (1.77)--(1.78) defines the classical reference minimum on the current
core. LFR II (1.7)--(1.9) gives a strictly positive axial Hessian there, with
constant depending on the fixed core size `M`, not the chronological age.
CMP102 Proposition 9, (190), gives the normalized local response of the
same-fine-lattice minimal configuration. Differentiating the Wilson action
with a pulse far from the core pairs a pulse-localized curvature with a
core-localized curvature response. In four dimensions the two factors of
`η²` cancel the fine plaquette count `η^{-4}`. Reserving part of the
exponential decay pays the convolution polynomial. Thus

\[
 \|\nabla_a\mathscr A_\Lambda(0,s)\|
       \le C_M|s|e^{-cD},\qquad
 \|a_*(s)\|\le C_M|s|e^{-cD}.                         \tag{RSA.3}
\]

The second estimate follows directly from strong convexity along the segment
to the reference minimum. It is a statement about the classical source
minimum, not about a reference Gaussian or an old conditional mean. The
current-core graph has a fixed finite number of edges, so (RSA.3) also bounds
the gauge adjustment needed for the literal fresh graph and the fresh
`M_0 ε_k` cutoff.

LFR I p.197, (1.85)--(1.87), changes the reference to its axial/Landau
representative and explicitly requires the corresponding compensating
transformations of `V_h` and of the relative variable. These transformations
must be retained. Their inputs in the core are of the small size (RSA.3),
and the source analytic map has the same local bound on that fixed chart.

The remaining characteristic function `χ_{h,1/2}` tests the **filled field
`(1,V_h)`**, not the original field alone. The artificial boundary seam is
therefore part of the check. The birth gauge is one near that seam. The
physical annular links and their compensating gauge differ from the identity
there by the localized tail and (RSA.2). Hence seam plaquettes also have a
strict small-field margin; applying the local variational regularity estimate
gives the literal `χ_{h,1/2}` test. Finally LFR I p.198, (1.89), removes
the original `χ''_k` only after these replacement characteristic functions
are present. This is the source-supported implication used here.

## 3. Positivity and singular support

The no-new-field geometry in CMP119 pp.265 and 269 gives, with `C` the
next-grid cover of the preceding old hole,

\[
 \Omega_k^c=C^{+8},\qquad Y=C^{+10},
\]

and tests new `P_k` only outside `C^{+4}`. Equal final rectangles therefore
have the same current hole, although the older prepared cores can be disjoint.
The nested floor/ceiling construction in RS.2 permits separated prepared
cores with this common final rectangle. A final moderate pulse in the common
interior can violate the fresh residual threshold `ε_k` and obey the
exterior-extension threshold `2ε_k`. Local variational response controls its
effect near both cores. Earlier thresholds have the additional scale-square
margin; the true fluctuations vanish by the compatible representative chain.
The strict pure-gauge birth seed gives the desired old bad selector without
introducing physical curvature.

All inequalities used for this construction are strict. At a fixed admitted
cutoff a small physical perturbation of an old current plaquette in the first
core can therefore be reconstructed while keeping the exterior fixed and
preserving every selected cutoff. The regular coarea chart has positive
density. An open set of such perturbations has strictly positive Wilson
scalar, which supplies a positive old numerator. Compactness on the chosen
finite chart and the source finite unnormalized bounds give the finite
denominator bound needed for a positive posterior share. This argument does
not infer an old normalized lower bound from a fresh reference lower bound,
and it needs no uniform ultraviolet lower constant.

For the second stratum, a descriptor that resets the chosen stencil has a
prepared core disjoint from the second core. Its full shell measure has an
absolutely continuous local gauge orbit inside the second core. Its own graph
conditions remain intact under that gauge transformation, by covariance and
disjointness. The anchored graph of the second descriptor fixes this gauge and
is Haar-null along the orbit. Gauge-orbit disintegration therefore proves that
every descriptor resetting the stencil has zero measure on the generic second
stratum. Freezing arbitrary raw shell links and asserting that a
shell-dependent reference is unchanged would not prove this fact.

Only finitely many descriptors occur at fixed cutoff and finite volume. Their
generic strata may be separated after coinciding support classes are grouped.
On the first stratum the positive own-descriptor contribution gives a positive
lower bound; other contributions are nonnegative. On the second stratum every
surviving descriptor retains the native current stencil, so the conditional
mark is exactly its current value. The two strata approach a common field
flat on that stencil. This is precisely RS.1.

## 4. What the native construction does not prove about microscopic energy

The F-01 scalar is exactly a fixed multiple of the microscopic Wilson action.
With the incoming coefficient exposed, the sum of its microscopic insertions
is

\[
 h^4\sum_x(\alpha\beta_0\sigma_h(x)-c)
   =\frac{2\alpha}{\sqrt6}\,\beta_0 S(U)
       -h^4 c\,\#\{x\}.                              \tag{RSA.4}
\]

For a fixed residual descriptor, define the actual old source integral by

\[
 M_\gamma(t;v_\gamma)
  =\int e^{t\beta_0S(U)}\,\rho_\gamma(dU,d\xi;v_\gamma).
 \tag{RSA.5}
\]

All source-free maps, selectors, history weights, coarea factors and current
couplings are specified in this identity. The normalized conditional microscopic
energy is `∂_t log M_γ(0;v_γ)`. On a common support class of the erased
output one must first sum the old source integrals with their actual fresh
densities and only then differentiate its logarithm. Differentiating an
adaptively changed running coupling is not this source identity.

The native reset/retain argument supplies no comparison of these derivatives.
In particular, a strict Wilson minimum gives each individual conditional
energy a positive excess over its own minimum; it does not order two different
conditional laws or subtract their common thermal contribution.

### 4.1 Exact Gaussian calculation: why two flat total energies can agree

Let the gauge-fixed physical microscopic variable `X` have Gaussian density
proportional to `exp(-X^T K X/2)`, with `K>0`. Let `Q` be surjective onto
`r` retained physical coordinates, and put

\[
 H=(QK^{-1}Q^{\mathsf T})^{-1}.
\]

The conditional mean and covariance are

\[
 \bar X=K^{-1}Q^{\mathsf T}Hy,\qquad
 C_{\rm cond}=K^{-1}-K^{-1}Q^{\mathsf T}HQK^{-1}.
\]

Taking the trace of `K C_cond` gives the exact identity

\[
 \mathbb E\!\left[\tfrac12X^{\mathsf T}KX\mid QX=y\right]
       =\tfrac12(n-r)+\tfrac12y^{\mathsf T}Hy.          \tag{RSA.6}
\]

Now forget `r_C` of the current coordinates in a core `C`, retaining its
complement. The second Gaussian conditioning gives

\[
 \mathbb E\!\left[\tfrac12X^{\mathsf T}KX\mid y_o\right]
   =\tfrac12(n-r)+\tfrac12r_C
     +\tfrac12y_o^{\mathsf T}
       (H_{oo}-H_{oC}H_{CC}^{-1}H_{Co})y_o.             \tag{RSA.7}
\]

Two translated cores releasing the same number of physical coordinates have
the same total microscopic conditional energy at flat exterior. Their local
microscopic energy profiles can differ, and (RSA.7) is nonconstant along
retained physical directions, but positivity of a native reset scalar alone
does not imply a discrepancy of the two flat total energies. A soft-gauge
factor is treated separately before applying this calculation to the physical
quotient; counting gauge directions as physical Wilson modes is incorrect.

### 4.2 The common-patch nonconstancy route

A useful stronger criterion avoids comparing the two flat constants. At a
fixed first descriptor the old microscopic quotient is independent of the
newly sampled physical field inside the first core. The same is true after
summing a generic first support class if its fresh kernel is common, as in
RS.4; if coincident-support classes have different fresh kernels, their
within-class posterior must also be checked. The second stratum retains those
physical variables. Gauge covariance lets one vary them on a common stratum
patch while readjusting only the graph gauge inside the disjoint second core.
Under that cancellation condition, an erased-output continuous version would
force the second microscopic quotient to be constant along the patch.

For the Gaussian law, (RSA.7) proves the required nonconstancy: the relevant
Schur complement is strictly positive on a nonzero retained physical
direction. For the actual Wilson old law, a proof that at least one microscopic
scalar conditional mean is nonconstant on this patch would therefore complete
this particular erased-output argument for that family.

That proof is not supplied by the variational minimum alone. It also does not
follow merely from analytic dependence on a new specified source temperature:
nonconstancy at some source temperature need not hold at the actual one. If
the actual coupling is varied instead, the sharp old selectors, preparation
domains and eligibility rules vary too. Continuing a specified-geometry formula
to a convenient temperature requires a justified continuation of those
integrals and a nonidentity argument for their actual derivative. A crude
error proportional to the number of fine variables is insufficient when the
chronological age is `N≈R(g)`.

At present the exact next missing comparison is therefore a **local old
microscopic source response**, with the old positive history weights left in
place, or an alternative finite-geometry proof of the stated nonconstancy.
Neither B-03, F-05 nor the desired all-history M-04 estimate has been used to
replace that comparison.

## 5. Fixed-basis scalar extraction is a separate algebraic issue

The M-04 statement asks for expansion in the fixed incoming F-01 basis. F-01
normalizes that basis by separated Gram forms; it does not prescribe a unique
projection functional for every transported scalar. The symmetry-averaged
identity/single-pulse projection in LC.7 therefore supplies the requested
scalar/identity algebraic extraction on any domain where the actual carrier
bound has already been proved. Its coefficient is converted using the exposed
incoming scalar normalization. No unknown final `Z` is used.

Comparison to a later particular F-03 channel-matrix prescription is a
downstream matching question, not an additional condition silently imposed on
M-04. The unresolved all-history issue lies in the actual output norm and its
current records, not in an invented uniqueness requirement for this finite
projection.

## 6. Further geometric check: the prepared core determines the final quiet component

The geometry in [M04 Bounded Core Source Map](M04_Bounded_Core_Source_Map.md), CG.2, passes with the
following union-level proof. It is not necessary to assume that separate
ancestors never merged, nor to invert an arbitrary dilation.

Let `k_0=k-N_0`, and let `C` include the next-grid covers of **all**
`k_0` ancestors of one final eligible component `Y`. The source formulas
are understood after their stated restriction to this component. Physical
nesting ensures that each connected piece of `C^{+10}` belongs wholly to
`Y`; these pieces, and their smaller enlargements, are not clipped by the
intersection with `Y`.

Put `S=C+B_8`, where `B_q` is the integer sup-norm ball of cube indices.
The quiet hole is `S`, and the literal complement/enlargement formulas in
(1.10), (1.73) give `Z''_k=S\ominus B_5` and
`\Lambda=S\ominus B_4`. For an arbitrary union `C`, erosion cannot be
canceled against dilation to infer `Z''_k=C+B_3` or `\Lambda=C+B_4`.
The exact substitute is

\[
 C+B_{8-q}\subset S\ominus B_q,\qquad
 (S\ominus B_q)+B_q\subset S\quad(0\le q\le8).
\]

Dilating the first inclusion by `B_q` gives the reverse of the second,
because `B_{8-q}+B_q=B_8`. Consequently

\[
 S=(S\ominus B_q)+B_q,\qquad
 C+B_{10}=S+B_2=\Lambda+B_6.                        \tag{RSA.8}
\]

This equality is valid for disconnected unions. The two-layer regular
collar between the hole and the component boundary prevents an outside
hole from changing these componentwise erosions. This corrects the
stronger inverse-erosion assertion in the initial version of this analysis;
only the displayed exact identity is needed.

The source explicitly states on p.192 that the prepared domain on one
eligible component is a rectangle of side at most `100M`. Thus the region
on the right of (RSA.8) is already one rectangle. Subsequent quiet steps
take its next-grid cover and add ten layers; the rectangular-hull rule of
CMP119 p.269 makes no further change. Any old ancestor that later joins
`Y` was already included in `C`, so there is no omitted later arrival.
This proves CG.8 and the redundancy of `Y` once `Λ` and the fixed scale
parameters are specified, at the literal eligible-component scope.

This identity is useful but does not prove that a resampled `Λ` label has
a bounded physical dependency footprint. Its selection, allowed old-history
set, posterior and reference map may still depend on remote data. Nor does
it remove the preliminary annular integrations: the bounded integration
core applies to the **remaining prepared operation**, after those
integrations and their marked records have been performed. These locality
and transport distinctions in CG.1--CG.9 should be retained.
