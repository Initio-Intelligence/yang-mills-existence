# Actual first-step R-birth weights have a common Gaussian comparison

Part of the [scalar-extraction analysis](scalar_extraction.md). This note concerns the
original first step on the globally P/Q-regular branch, before later
history operations. It proves a relative comparison for the complete
local R selector at a fixed admitted coarse field. It does not restrict
the R selector to a small trial box, and it does not divide an absolute
error by a rare-event probability.

The later residual-class integral still has to be reassembled so that
these first-step weights are integrated against a common later law. This
note does not claim that its geometry-dependent quiet masks have already
been compared.

## 1. Exact first-step density and the R pattern

Put `g=g_0` and `P=delta_0/g_0` in the literal source normalization.
Fix an admitted first coarse field V on the globally P/Q-regular branch
`Omega_1=whole lattice`. CMP119 pp.248--250, (1.11)--(1.18), gives the
complete free-coordinate density

\[
 \mathcal D_V(z)\,dz
  =\exp\{-\tfrac12z^{\mathsf T}K(V)z+W_V(z)\}\,dz . \tag{RB.1}
\]

The retained-only factors, the constant linear-constraint Jacobian and
the displayed powers of g are common to every first R pattern. They
are kept in the original coarse density and cancel in every ratio below.
The full W includes Wilson, soft gauge, Haar, coarea and exceptional-bond
Jacobian factors, in the source's original critical-cancelled form.

Let `mathcal R` specify the exact set of bad R-test cubes. The R tests in
(1.18) are maxima of the norm of the actual independent free coordinates
over the specified enlarged starred cubes, with threshold P. Hence they
are fixed functions of z, independent of the coarse field V. They are
invariant under the block adjoint gauge transformations of CMP119 (1.17).

Assume this R pattern has one bounded h=1 large-field neighborhood. Choose
a coordinate set D containing the complete footprints of all its bad
R tests and the remaining Q tests there, with the source's fixed stencil
halo. It can be chosen with

\[
 \operatorname{diam}D\le C R_1,\qquad |D|\le C R_1^4.
                                                               \tag{RB.2}
\]

Every coordinate outside D is constrained by a good R test to have norm
less than P. The good-test restrictions on coordinates inside D are
retained. Thus on the product domain with radius P off D, the exact
R-pattern event is a measurable event `E_R(z_D)`. It may impose many
overlapping good and bad tests; it is not replaced by a single maximum.
Its key exact property is that it depends only on which coordinate
norms are above or below P. A coordinatewise radial map that preserves
those alternatives preserves the entire R pattern.

This formulation includes a pattern with several bad test cubes whose
source cover/hull is one bounded birth neighborhood. It is not an
assertion about arbitrary bad P/Q regions or an arbitrary old T_h.

## 2. The starred Q test gives a uniform radial sandwich

CMP119 p.247, (1.8)--(1.9), excludes the exceptional bonds `b_0(c)` from
the approximate Q test. The linearizing change in (1.14) changes only
those excluded bonds. Consequently, on a tested free bond e, the exact
reconstruction is

\[
 U_e=\exp(i g z_e)\,U_{1,e},
 \qquad
 U_e U_{1,\square,e}^{-1}
       =\exp(i g z_e)\,E_{\square,e}(V),             \tag{RB.3}
\]

where the source reference comparison gives

\[
 \|E_{\square,e}(V)-I\|
       \le C gP e^{-cR_1}.                         \tag{RB.4}
\]

The constants absorb the fixed hierarchy `A_0/A_1`. This is precisely
the local-reference estimate used to remove the old Q factor on good
R cubes, printed at the first step after (1.18), and at general steps in
(3.17)--(3.19). Its footprint is already included in D.

The original Q threshold is `2delta_0=2gP`. On `||z_e||<=3P`, Taylor's
formula and the triangle inequality give

\[
 \left|g^{-1}\|\exp(i g z_e)E_{\square,e}-I\|
                                  -\|z_e\|\right|
       \le C\{gP^2+P e^{-cR_1}\}.                 \tag{RB.5}
\]

Use the same matrix norm as the source. Norm equivalence in fixed group
dimension changes only constants, and the expansion has the same linear
norm at the origin. Put

\[
 \eta=C\{gP+e^{-cR_1}\},\qquad
 q_\pm=(2\pm\eta)P .                              \tag{RB.6}
\]

For sufficiently weak coupling, `eta<1/8`. The actual remaining Q-good
event therefore lies between the product norm balls of radii `q_-` and
`q_+` on its free coordinates. On good R coordinates the Q test is
automatically true because their radius is P. All original small-field
and axial-cutoff functions dropped in (1.11) are exactly redundant on
this P/Q-regular branch as stated on p.248; their exponential gauge
density remains in W.

Conversely, the original Q-good condition puts each tested free bond in
the principal logarithm chart with `||z_e||<q_+<3P`. The change to z does
not alter those free entries. Thus the product radius `3P` on D
encompasses the entire R-only sector, rather than just a strict trial
subset.

Let `E_act(V)` be the exact remaining first-step Q-good selector together
with `E_R`, on the encompassing product domain `K_D` of radius 3P on D
and P elsewhere. With `B_q` denoting the product norm ball of radius q
on D, the exact inclusions are

\[
 E_R\cap B_{q_-}\ \subset\ E_{\rm act}(V)
                  \subset\ E_R\cap B_{q_+}.        \tag{RB.7}
\]

Coordinates in D on which a good R test already imposes P are harmless
in these inclusions. The local coarse gauge used below preserves all
the norm tests and the sandwich; it does not alter their source meaning.

## 3. A radial transport preserves every R alternative

### Lemma RB.1 -- a relative comparison of the two Q sandwiches

For the flat first-step Gaussian, integrated with radius P off D, let
`I(q)` be the unnormalized integral of `1_{E_R}1_{B_q}`. Then

\[
 e^{-C\eta P^2|D|}I(q_+)
          \le I(q_-)\le I(q_+).                    \tag{RB.8}
\]

The same estimate compares either side with `I(2P)`.

**Proof.** On each coordinate block, map a vector of norm r radially
to norm `psi(r)`, where `psi(r)=r` for `r<=3P/2`, and on
`[3P/2,q_+]` use the increasing affine map taking `q_+` to `q_-` and
fixing `3P/2`. Its derivative and ratio `psi(r)/r` lie in
`[1-C eta,1]`. This map is a bi-Lipschitz bijection between the two
balls. It leaves all norms at most P fixed and maps every norm greater
than P to another norm greater than P. Hence it preserves the exact
event E_R, including every overlapping bad-cube maximum and good-cube
condition.

The Jacobian on one real coordinate block of dimension d is
`psi'(r)(psi(r)/r)^{d-1}` almost everywhere. The same formula follows
from norm-polar coordinates for a non-Euclidean convex norm ball, so no
smoothness of the operator-norm sphere is assumed. The product Jacobian
is bounded below by `exp(-C eta |D|)`.

The displacement is supported in D and has coordinate norm at most
`C eta P`. Before and after transport every coordinate is at most 3P,
and the flat precision has a fixed absolute row bound. Therefore

\[
 \left|\tfrac12(Tz)^{\mathsf T}K_{\rm flat}(Tz)
                   -\tfrac12z^{\mathsf T}K_{\rm flat}z\right|
       \le C\eta P^2|D|.                          \tag{RB.9}
\]

This retains all cross terms between D and its complement; outside
coordinates have radius P. Change variables by T and combine the
Jacobian and action bounds. The upper inequality is inclusion.
\(\square\)

Unlike an absolute Gaussian tail estimate, (RB.8) has no loss depending
on how many bad cubes E_R requires or how small its mass is. It applies
to the full event, not only to a specified seed configuration.

## 4. One common original baseline

Let

\[
 Z_P(V)=\int_{\|z_e\|<P\ \forall e}\mathcal D_V(z)dz
                                                               \tag{RB.10}
\]

be the actual all-R-good first-step integral. Define the exact relative
R-only defect weight

\[
 b_R(V)
   =\frac{\int_{\mathcal K_D}{\bf1}_{E_{\rm act}(V)}
                                     \mathcal D_V(z)dz}
          {Z_P(V)}.                                \tag{RB.11}
\]

This is just an algebraic factoring of the original positive integral.
The same `Z_P(V)` is retained as part of the later coarse density for
every R pattern; it is not a resetting of that density. If one uses the
overall first conditional normalizer instead, the same positive
`Z_P/Z_total` factor multiplies every pattern.

The exact identity RMg.34 expresses (RB.11) as a ratio of two local
probabilities under the product-domain law on K_D. RMg.32--RMg.35 compare
those probabilities relatively to the single flat Gaussian, after a
local block-constant gauge on an R-sized halo of D. The literal R tests
and both radial sandwiches are invariant under that gauge. Thus

\[
 e^{-2\Delta_D}\frac{I(q_-)}{Z_{P,\rm flat}}
    \le b_R(V)\le
 e^{2\Delta_D}\frac{I(q_+)}{Z_{P,\rm flat}},          \tag{RB.12}
\]

where

\[
 \Delta_D\le C\{gP^3R_1^6+g^2P^2R_1^4
                             +P^2R_1^4e^{-\kappa R_1}\}.
                                                               \tag{RB.13}
\]

Define the flat defect weight using the same exact R event and the
radius 2P Q cutoff,

\[
 b_R^G=I(2P)/Z_{P,\rm flat}.                         \tag{RB.14}
\]

### Theorem RB.2 -- conditional first-birth weight comparison

On the stated original globally P/Q-regular first-step chart, uniformly
in the admitted coarse data V and for every bounded local R pattern,

\[
 \boxed{\quad e^{-\varepsilon_R}b_R^G
               \le b_R(V)\le e^{\varepsilon_R}b_R^G,
 \qquad
 \varepsilon_R=2\Delta_D+C\eta P^2|D|=o(1).
 \quad}                                             \tag{RB.15}
\]

The rate is uniform in total volume. It is valid for arbitrarily small
positive R-pattern mass. It does not depend on the optimal Gaussian
large-deviation rate of the pattern.

**Proof.** Combine (RB.8) with (RB.12). Every factor is from the same
first-step integral and its actual free-coordinate chart. The source
cutoffs have only been enclosed in the common product domain; (RB.7)
keeps their actual alternatives. Since g and `exp(-cR_1)` beat the
displayed logarithmic powers, the exponent tends to zero. \(\square\)

If `R'` is an exact translation of the entire R pattern by a vector
preserving the first block and R-test partitions, its footprint D
translates as well. The flat precision, all-P baseline and radius 2P
event translate together, so `b_{R'}^G=b_R^G` exactly. Consequently

\[
 e^{-2\varepsilon_R}\le
          b_{R'}(V)/b_R(V)\le e^{2\varepsilon_R}.     \tag{RB.16}
\]

The whole-cluster translations counted in BD.1a preserve those partitions.
This gives an actual weight comparison at fixed first coarse data for
that family of local first R patterns. It is more than a collection of
young-trial lower bounds.

## 5. A local fluctuation moment for the full first R pattern

The same comparison supplies a useful local energy budget. It still
concerns the first-step R sector, not an arbitrary inherited marked
family.

### Lemma RB.3 -- finite-coordinate insertion lower bound

For every positive R pattern in (RB.2),

\[
 b_R^G\ge e^{-C P^2}.                               \tag{RB.18}
\]

**Proof.** The number of bad R-test cubes in a bounded `MR_1`-sized
birth neighborhood is bounded by a fixed source constant: each test
cube has side a fixed multiple of `R_1`, while the neighborhood has
side at most another fixed multiple of `R_1`. The constant can be large
and depends on the fixed M/M2 hierarchy, but not on g or the volume.

For each bad test cube choose one free coordinate in its tested set
which is not covered by any good-test footprint. Such a coordinate
must exist: otherwise every coordinate in that bad test would be
strictly below P on every nonempty realization of the pattern. Use at
most one chosen coordinate per bad cube, allowing coincidences.

Put each chosen coordinate in a fixed-radius ball about a vector of
norm `5P/4`, and keep all other coordinates below P. For sufficiently
large P this event has exactly the specified R pattern and lies inside
the 2P Q sandwich. No good test contains a chosen coordinate, and every
bad test has its chosen witness. There are at most a fixed number of
modified real coordinate blocks.

For fixed values of the remaining coordinates, all of norm at most P,
the absolute row bound for Kflat bounds the change of its quadratic
action between any selected vector in the all-P box and the stated
insertion balls by `C P^2`. This includes cross terms with every other
coordinate; their absolute row sums, not their number, enter. The ratio
of the finite selected-coordinate volumes costs at worst a fixed power
of P. Comparing those conditional integrals, then integrating the
remaining coordinates, proves (RB.18). \(\square\)

Unlike the earlier young preparation trial, this is a finite-coordinate
insertion into the same first-step product integral. It does not put
all O(R^4) background coordinates in tiny boxes.

Let

\[
 E_D=1+d_D+\sum_{i\in D}|z_i|^2,                    \tag{RB.19}
\]

where `d_D` is the number of real coordinate components in D and the
Euclidean norm is taken in the fixed orthonormal Lie basis. It is
invariant under the block adjoint gauge used in RMg.4.

### Proposition RB.4 -- actual first-birth local fluctuation moments

Let `nu_{R,V}` be the normalized actual first-step R-only sector of
(RB.11). For all `p>=1`,

\[
 \|E_D\|_{L^p(\nu_{R,V})}
       \le C\{p+P^2+|D|\}.                        \tag{RB.20}
\]

The constants are independent of total volume and the particular positive
R pattern within (RB.2).

**Proof.** First use the flat Gaussian on the product domain with 3P
on D and P elsewhere. It is invariant under `z->-z`, so its mean is
zero. Inserting `exp(t sum_D |z_i|^2)` changes its precision to
`Kflat-2t P_D`. For fixed `0<t<lambda/4` the precision and every further
tilted precision have a fixed gap. The convex-domain covariance bound
therefore bounds the derivative of the log partition function by
`C d_D`. Integrating the tilt gives

\[
 \gamma_{\mathcal K_D}\exp\{t\sum_D|z_i|^2\}
       \le e^{C|D|}.                              \tag{RB.21}
\]

The same strongly convex symmetric measure has a uniform coordinate
sub-Gaussian bound. In fixed block dimension,
`gamma_{K_D}(||z_i||>=P)<=C exp(-cP^2)`. Hence
`gamma_{K_D}(z_D notin K_{P,D})<=C|D|exp(-cP^2)<1/2` for sufficiently
weak coupling. Consequently the enlarged Gaussian normalization is at
most twice the all-P normalization, irrespective of total volume.

Apply RMg.32 and RMg.34 to the two local nonnegative functions
`exp(t E_D)` and `1_{z_D in K_{P,D}}`. Drop the additional actual birth
selector only for the upper numerator. This bounds that numerator,
divided by the common actual ZP, by `exp(C|D|+2Delta_D)`.
The actual denominator b_R(V) is at least `exp(-CP^2-epsilon_R)` by
(RB.15), (RB.18). Thus

\[
 \nu_{R,V}e^{tE_D}\le e^{C(P^2+|D|)}.              \tag{RB.22}
\]

The resulting tail is bounded by
`min(1, exp(C(P^2+|D|)-t s))`. Integrating it gives (RB.20).
\(\square\)

This bounds the local free-coordinate fluctuation energy, with its actual
local rank. It does not include an unremoved background Wilson energy
or assert that every already transported microscopic scalar has this
coefficient. The original `a^{-4}` factor of a primitive microscopic
mark remains explicit when this estimate is used.

## 6. What remains before a full residual-class exchange

There are three remaining scope changes; none is contained in RB.15.

First, the completed old law can contain P/Q births and, for h>1,
arbitrary earlier histories. They are not members of the product-domain
R-only first-step family. A comparison of their total contribution to
this R-only family needs the source density and its actual rate; a trial
cost with an unspecified exponential constant is insufficient.

Second, even at h=1, the later quiet/preparation masks depend on the
birth geometry. Their test functions have no direct A0 dependence on
this R-only branch because Omega1 is full and there is no Gamma0, but
their domains and the intermediate averaging constraints vary with the
history. To use (RB.15) in the complete old operation one must prove an
exact common positive reassembly, schematically

\[
 M_{R,r}(F)=\int \Pi(d\zeta)\,
       {\bf1}_{G_{R,r}}(\zeta)\,Z_P(V_1(\zeta))\,
       \int_{E_R}F\,d\mu_{V_1(\zeta)}^{\rm defect}, \tag{RB.17}
\]

with the same measure Pi before the masks and the exact retained
readout for every compared geometry. Formula (RB.17) is the task to
identify from the original annular Fubini identities; it is not asserted
here. The small preparation cutoff with exponent `p_1<p_0` makes an
absolute failed-preparation bound unusable after division by the birth
mass. A relative comparison retaining the birth factor is necessary.

Third, a marked microscopic scalar must retain its incoming coefficient,
thermal identity and already generated annular marks. RB.15 is a weight
theorem. It does not make an arbitrary old-energy-bounded mark dilute,
and it does not supply a depth-uniform replacement of its microscopic
`a^{-4}` coefficient by the current `h^{-4}` coefficient. A localized
centered-root budget and the separate current records remain required.

### Mathematical sources

- CMP119 (1988), pp.247--251, (1.8)--(1.20): starred Q test, exceptional
  solve, complete normal form, independent R test and reference-tail
  comparison.
- CMP119, pp.267--269, (3.15)--(3.19): the same exact distinction between
  the old Q cutoff and new free-coordinate R cutoff at an ordinary step.
- [first step relative marginal](first_step_relative_marginal.md), RMg.18--RMg.35: common-cutoff local
  density ratios, local gauge/precision comparison, and exact normalization
  cancellation. These are quantitative relative comparisons, not a
  replacement of the actual conditional law by a chosen Gaussian.
- [birth position dilution](birth_position_dilution.md), BD.1a--BD.1b: actual compatible positions
  and the single thin-birth geometric witness at a permitted large L.
