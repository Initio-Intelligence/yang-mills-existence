# A relative local marginal comparison in the first Wilson normal form

Part of the [scalar-extraction analysis](scalar_extraction.md). This note proves a local
Radon--Nikodym comparison, uniform in total volume, for the actual first-step
normal-form density on a fixed convex product cutoff. It is stronger than an
absolute comparison of expectations: it applies to arbitrarily rare events
measurable in the local set. It does not assert that every later residual
selector is such an event, nor replace the old residual operation by this
first-step law.

The distinction about the cutoff is essential. The Gaussian reference carries
**the same product cutoff** as the interacting law. A fixed larger cutoff on
selected coordinates is allowed on both sides. Additional source selectors,
when they are local, can then be inserted on both sides of the comparison.
They have not been silently removed or linearized.

## 1. The actual free-coordinate input

At the flat first-step retained configuration, put all background maps at
their source values, and use the actual independent coordinates `z` after
the exceptional-bond constraint solve. The exact positive normal form is

\[
 d\mu_1(z)=Z_1^{-1}{\bf1}_{\mathcal K}(z)
  \exp\{-\tfrac12 z^{\mathsf T}K_0z+W(z)\}\,dz .       \tag{RMg.1}
\]

Here `K_0` is the original constrained Wilson-plus-soft-gauge precision.
The complete `W` includes the higher Wilson and soft-gauge terms, the Haar
logarithm, the coarea factor and the exceptional-coordinate Jacobian, each
once. The original critical cancellation has already been made. No new
saddle is substituted and no residual force is discarded. At flat data
the leading precision is exactly the flat one in [first step precision gap](first_step_precision_gap.md).

Group the finitely many real Lie-algebra coordinates stored in a free-bond
block into sites `i`. Their graph has fixed polynomial growth. Matrix norms
below are block norms, with fixed component multiplicities absorbed in
constants. The preceding first-step gap proof gives

\[
 K_0\ge\lambda I,\qquad
 \sup_i\sum_j e^{\nu d(i,j)}\|(K_0)_{ij}\|\le C_K .    \tag{RMg.2}
\]

The precision is in fact finite range in these fluctuation coordinates.
The constants depend on fixed `L`, group dimension, and source geometry;
they do not depend on volume or coupling.

Let `P=P(g)`. Fix constants `b_+>b_->0`. The cutoff `K` is a product of
convex balls (or boxes) centered at zero, with coordinate radii in
`[b_-P,b_+P]`. One can, for example, double the radius on a prescribed local
set and keep the original radius elsewhere. Its membership is fixed during
the interpolation below. All these product domains lie inside the exact
constraint chart when `g` is sufficiently small, because `gP` tends to zero.

### The derivative rows, including their sums

The first-step source description in [local extension kernel](local_extension_kernel.md), Section
3.4, and CMP119 p.249 identifies every non-Gaussian term as a local analytic
function of the actual free coordinates and the local constraint solve.
At flat background the latter changes only the exceptional bond of a
coarse constraint and uses its two adjacent blocks. The Wilson plaquette,
the source soft-gauge contour and the Haar/coarea terms consequently have
fixed finite fluctuation-coordinate stencils. Equivalently one may use the
absolutely localized coefficient representation.

On a fixed larger complex coordinate tube, with radius `b_{++}P` and
`b_{++}>b_+`, their complete coefficient bounds have size

\[
 \epsilon_0=C\{gP^3+g^2P^2\}.                       \tag{RMg.3}
\]

The enlargement is by a fixed factor; it still has `g b_{++}P` inside the
same fixed geometric analytic chart. Cauchy in one independent coordinate
of radius `cP`, and in two independent coordinates successively, gives

\[
 \sup_{z\in\mathcal K}\|\partial_iW\|\le\epsilon_1,
 \qquad \epsilon_1=C\{gP^2+g^2P\},                  \tag{RMg.4}
\]

\[
 \sup_i\sum_j e^{\nu_1d(i,j)}
       \sup_{z\in\mathcal K}\|\partial_i\partial_jW\|
       \le\epsilon_2,
 \qquad \epsilon_2=C\{gP+g^2\}.                     \tag{RMg.5}
\]

The row sum is part of the conclusion. For the literal local stencils it
uses bounded incidence. If one instead writes `W=Σ_X W_X`, Cauchy first
gives `C epsilon_0 P^{-2} exp(-nu |X|)` for each Hessian entry with both
indices in `X`. Summing the second index costs `C|X|`; the carrier contains
both indices, so its exponential pays `exp(nu_1 d(i,j))`. The original
localization slack then sums `|X|` and all carriers containing `i`.
There is no inference of a row sum from the supremum of a completed sum.
Retained-only constants in `W` have zero first and second rows and cancel
from the normalized comparison.

Here is the enlargement check for the density terms. The physical argument
of each group exponential is `g z`. Haar density is analytic and nonzero in
a fixed neighborhood of the identity. The exceptional-coordinate solve is
the finite local implicit solve of CMP119 (1.14), with a uniformly invertible
linear constraint at the origin; its inverse and its coarea Jacobian are
therefore analytic and nonzero on a fixed physical tube. Its determinant
is taken in the actual eliminated coordinates. Any representation as a
trace logarithm uses the branch fixed at zero. After factoring its constant
invertible part, the remaining local matrix is `I+T(gz)` with absolute row
norm `||T||<=C g b_{++}P<1/2`. The series
`Tr log(I+T)=sum_{m>=1}(-1)^{m+1}Tr(T^m)/m` has an absolutely summable
anchored loop representation. Its enlarged-domain and derivative bounds
are therefore uniform in total volume. The higher Wilson and source soft
gauge terms are analytic local traces/contours on the same tube. Thus the
fixed-factor enlargement required for Cauchy concerns every factor in
`W`, including the measure, not just the Wilson polynomial. This assertion
is at the original first step; it is not a claim about a trace logarithm
of an inherited residual integral.

These are real derivatives of the complete normal-form density. They are
not derivatives of a Wilson action evaluated at a modified nonstationary
background. At nonflat native centers the same theorem below applies to
the actual positive precision whenever these same uniform rows hold;
the comparison then uses that center's precision, not a substituted flat
one. Comparing distinct background precisions is a further step.

## 2. A covariance lemma that remains valid at a hard convex boundary

Consider any probability on a product of convex coordinate domains,
with potential

\[
 H(z)=\tfrac12z^{\mathsf T}K_0z-\theta W(z)+\ell(z),
 \qquad 0\le\theta\le1,                              \tag{RMg.6}
\]

where `ell` is linear. Pinning some coordinates changes `ell` and restricts
the Hessian to a principal subspace. By (RMg.2), (RMg.5), all these
conditional potentials have Hessian at least `lambda/2` when
`epsilon_2<lambda/2`. Their off-diagonal Hessian entries have a common
exponentially summable majorant. The same statements hold after pinning
any set, with constants independent of its size and pinned values.

### Lemma RMg.1 -- covariance decay with a common absolute majorant

For sufficiently small fixed `kappa>0`, every measure just described obeys

\[
 |\operatorname{Cov}(f,q)|
 \le C\sum_{i,j}e^{-\kappa d(i,j)}
       \|\partial_if\|_\infty\|\partial_jq\|_\infty. \tag{RMg.7}
\]

The same inequality holds on any remaining coordinates after conditioning
on the others. It does not require a sign condition on the off-diagonal
precision, diagonal dominance, or entrywise positivity of its inverse.

**Proof.** First extend `W` beyond the product domain by composing each
coordinate block with a smooth saturation into its slightly larger
analytic ball. The saturation is identity on the cutoff, has bounded
first derivative and second derivative `O(P^{-1})`. The chain rule and
(RMg.4)--(RMg.5) preserve the gradient and Hessian row bounds, with fixed
constants. This also preserves the fluctuation stencils. Taking `g`
smaller leaves the stated gap on the whole extended space; no extension
of a nonconvex source selector is being made. Now approximate each convex
coordinate boundary by a smooth convex confining potential `b_i(z_i)` on
its own coordinate block.
For a source norm ball other than the Euclidean one, the saturation uses
a sufficiently larger Euclidean chart ball; equivalence of norms in the
fixed coordinate-block dimension only changes the fixed constants.
It may have an arbitrarily large positive Hessian. Its off-block Hessian
is zero. Choose a distance weight `D_a(i)=exp(kappa d(a,i))`, constant on
each coordinate block. It commutes with every `Hess b_i`.

The exponentially summable off-diagonal majorant gives, uniformly in the
position and in every boundary approximation,

\[
 \|D_a\operatorname{Hess}H D_a^{-1}
                      -\operatorname{Hess}H\|_2\le C\kappa .
                                                               \tag{RMg.8}
\]

To see this, an `(i,j)` entry gains a factor bounded by
`exp(kappa d(i,j))-1`; the two absolute row/column sums are `O(kappa)`.
There is no diagonal contribution. Choose `kappa` so the right side is
at most `lambda/4`. The real part of the conjugated Hessian is then at
least `lambda/4`.

For the Langevin generator `L=Delta-grad H dot grad`, the derivative of
its stochastic flow solves the matrix equation

\[
 \dot J_t=-\operatorname{Hess}H(X_t)J_t,
 \qquad J_0=I.
\]

The weighted energy inequality and (RMg.8) imply
`||D_a J_t D_a^{-1}||_2 <= exp(-lambda t/4)`. Applying this with a weight
centered at either endpoint bounds each matrix entry by
`exp(-kappa d(i,j)) exp(-lambda t/4)`. Integrating the stationary
semigroup covariance identity

\[
 \operatorname{Cov}(f,q)
   =\int_0^\infty \mathbb E[\nabla f\cdot\nabla P_tq],dt
                                                               \tag{RMg.9}
\]

gives (RMg.7). The factor `4/lambda` is absorbed into `C`.

For rigor one can first use smooth bounded functions and smooth barriers,
then approximate. Convex block barriers preserve the Hessian gap and
(RMg.8), so all constants are uniform as the barriers tend to the
indicator of the product domain. Dominated convergence passes the
covariance inequality to that domain. Equivalently the limit is the
reflecting diffusion with the Neumann condition; no boundary term has
been discarded in an integration by parts. Principal compression after
pinning preserves the same gap and off-diagonal majorants, and repeats
the proof. \(\square\)

## 3. The local density ratio

Define the full interpolating probabilities

\[
 d\mu_\theta=Z_\theta^{-1}{\bf1}_{\mathcal K}
             e^{-z^{\mathsf T}K_0z/2+\theta W(z)}dz.
                                                               \tag{RMg.10}
\]

Let `D` be any finite set of coordinate blocks and `u=z_D`. Denote its
normalized marginal density by `p_{theta,D}(u)`. Put

\[
 F_\theta(u)=\mathbb E_{\mu_\theta}[W\mid z_D=u].    \tag{RMg.11}
\]

For `i` in `D`, differentiation of the **conditional normalized** integral
gives the exact formula

\[
 \partial_iF_\theta(u)
 =\mathbb E_{\theta,u}(\partial_iW)
   +\operatorname{Cov}_{\theta,u}(W,G_i),
                                                               \tag{RMg.12}
\]

\[
 G_i=\theta\partial_iW-(K_0z)_i .                   \tag{RMg.13}
\]

The terms in `(K_0z)_i` depending only on pinned coordinates cancel from
the covariance. The derivative of the boundary score on an unpinned
coordinate `j` is

\[
 \partial_jG_i=\theta\partial_j\partial_iW-(K_0)_{ij}.
                                                               \tag{RMg.14}
\]

In particular the quadratic coupling across `D` and its complement has
not been omitted. The gradient of this score has a uniformly bounded
absolute weighted row. Combining (RMg.4), (RMg.7), (RMg.14) and the
summability of `exp(-kappa d(i,j))` gives

\[
 \sup_u\|\partial_iF_\theta(u)\|\le C\epsilon_1 .   \tag{RMg.15}
\]

For example the covariance contribution is bounded by
`C epsilon_1 sum_{a,b} exp(-kappa d(a,b))
(|K_{0,ib}|+sup|partial_b partial_i W|)`, which is at most
`C epsilon_1`. This calculation explains why the extensive observable
`W` does not produce an extensive loss.

The convex product marginal domain connects any `u,v` by its straight
segment. Its coordinate diameters are at most `C P`. Hence

\[
 \operatorname{osc}F_\theta
      \le C P\epsilon_1 |D|
      \le C\{gP^3+g^2P^2\}|D|=:\delta_D .           \tag{RMg.16}
\]

The normalized marginal has the exact theta derivative

\[
 \partial_\theta\log p_{\theta,D}(u)
    =F_\theta(u)-\mathbb E_{\mu_\theta}W
    =F_\theta(u)-\int F_\theta(v)p_{\theta,D}(v)dv.  \tag{RMg.17}
\]

The right side is bounded by the oscillation in (RMg.16). Integration
from zero to one proves the following theorem.

### Theorem RMg.2 -- relative local first-step comparison

For the actual first-step product-domain normal form (RMg.1), with its
complete free-coordinate input and sufficiently small coupling,

\[
 \boxed{\quad
 \left|\log\frac{p_{1,D}(u)}{p_{0,D}(u)}\right|
 \le C\{gP^3+g^2P^2\}|D|=\delta_D .\quad}          \tag{RMg.18}
\]

The statement holds almost everywhere on the common marginal support,
including by continuity at interior limiting points. It is uniform in
total volume and the choice of `D`. The reference `mu_0` is the normalized
Gaussian with precision `K_0` and the **same** product cutoff.

Consequently every nonnegative measurable local function `A(z_D)` obeys

\[
 e^{-\delta_D}\mu_0 A\le\mu_1 A\le e^{\delta_D}\mu_0 A.
                                                               \tag{RMg.19}
\]

If `E` is any event measurable in `z_D` with positive Gaussian probability,
the normalized conditional measures restricted to `D` satisfy

\[
 e^{-2\delta_D}\mu_0(A\mid E)
    \le\mu_1(A\mid E)
    \le e^{2\delta_D}\mu_0(A\mid E).                \tag{RMg.20}
\]

No lower bound on the probability of `E` was used. For `|D|<=C R^4`,
the exponent tends to zero because `g` beats every fixed logarithmic
power. This is the desired rare-event stability at a **first-step local
product-domain** level.

## 4. A further local consequence for a quadratic-size mark

The same argument gives spatial influence without a rare-event denominator.
Let `A_x` be a local mark with a fixed coordinate support near `x`, satisfying
`|grad A_x|<=C bP` on the chosen product domain, as the exact first-step
dimensionless Wilson scalar does. For `m_x(u)=E(A_x|z_D=u)`, retain its direct
derivative when its support intersects `D`, and use (RMg.12) with `W`
replaced by `A_x` for the covariance part. The gradient of `A_x` is now
localized. A convolution of the two exponential majorants gives

\[
 |\partial_{u_i}m_x(u)|
       \le CbP e^{-\kappa' d(x,i)},\qquad i\in D,    \tag{RMg.21}
\]

where `0<kappa'<kappa` is fixed. It follows that any event measurable in
`D` has

\[
 |\mu_1(A_x\mid E)-\mu_1A_x|
   \le CbP^2\sum_{i\in D}e^{-\kappa'd(x,i)}.        \tag{RMg.22}
\]

This crude but rigorous estimate localizes the effect of that event. It
does not yet sum over birth locations, and it retains the stated `P^2`
and coordinate-volume costs. The baseline `mu_1 A_x` is its actual
unconditional first-step value, not an arbitrarily reset identity constant.

### A fixed flat reference on a stronger small-link chart

There is a useful actual first-step variant for the innovation comparison.
Suppose the first retained field is in an admitted global small-link chart

\[
 \sup_e\|V_e-I\|\le C_* gP,                         \tag{RMg.23}
\]

with a fixed `C_*`, and keep the same first-step coordinate convention.
This is stronger than merely small plaquette curvature; it is stated as
such. The local lift `Q^fV` has the same bound. Its force is `O(gP)`, and
the source force-resolved minimizing equation used in
[local extension kernel](local_extension_kernel.md), Lemma 3.1, gives
`U_1(V)-I=O(gP)` uniformly. The finite local coefficient formulas for the
actual constrained precision, including the current-dependent constraint
Hessian, then give

\[
 \sup_i\sum_j e^{\nu_1d(i,j)}
           \|K(V)_{ij}-K_{{\rm flat},ij}\|\le CgP.  \tag{RMg.24}
\]

Write the same exact conditional law with the fixed flat precision and
the perturbation

\[
 \widetilde W_V(z)
    =W_V(z)-\tfrac12 z^{\mathsf T}
                     [K(V)-K_{\rm flat}]z.         \tag{RMg.25}
\]

The retained-only determinant/normalization is canceled exactly by
normalization. By (RMg.24), the new quadratic term has first row `O(gP^2)`
and weighted second row `O(gP)`. The remaining source W has the same rows
as (RMg.4)--(RMg.5); its linear critical term is already canceled, not
bounded by `g^{-1}J`. Thus Theorem RMg.2 applies uniformly in (RMg.23),
with the **same flat Gaussian** and the same product cutoff:

\[
 \left|\log\frac{p_{V,D}(u)}{p_{{\rm flat},D}(u)}\right|
       \le C(gP^3+g^2P^2)|D|.                      \tag{RMg.26}
\]

This fixes the Gaussian reference when the first retained field will
subsequently be integrated over such a stronger good event. If a local
birth event `E_s` is independent of `V` in these free coordinates, its
conditional mass has the same relative bound uniformly in `V`. For an
arbitrary positive later measure `pi` and any subset `G` of the chart,

\[
 e^{-\delta_D}\gamma_{\rm flat}(E_s)\,\pi(G)
 \le\int_G \mu_V(E_s)\,\pi(dV)
 \le e^{\delta_D}\gamma_{\rm flat}(E_s)\,\pi(G).     \tag{RMg.27}
\]

The event must really be the same `E_s`. This does not eliminate the
V-dependent approximate Q selector or the geometric masks of a later
quiet event. Nor does it prove that (RMg.23) has high probability in the
full residual law. It supplies a uniform, fixed-reference comparison on
that explicitly narrower chart.

## 5. Source fit and the remaining exchange problem

The following scope facts are part of the theorem.

1. The independent coordinate chart, source critical cancellation and all
   density factors are the actual first-step ones. The proof uses their
   small **summed real Hessian**, derived above from local analyticity.
2. The convex support is a fixed free-coordinate product support. A doubled
   local cutoff is a common comparison domain, not an assertion that the
   source residual law changed its cutoff. Multiplication by the exact local
   birth selector is allowed via (RMg.19)--(RMg.20).
3. A selector depending on retained data through a minimum is measurable in
   `z_D` only after those data are fixed and the full fluctuation stencil is
   included. A selector involving later integrated variables is not thereby
   local in the first-step coordinates.
4. The comparison does not replace an actual nonlinear selector by its
   Gaussian linearization. Such a replacement requires a separate boundary
   estimate, or an exact translation covariance of the selector itself.
5. It does not assert translation invariance of a fixed higher-scale
   conditioning fiber. The h=1 Gaussian innovation identity in
   [birth position dilution](birth_position_dilution.md) translates the first innovation alone and
   keeps the later ones separate.
6. For the complete residual posterior, one must reassemble the actual
   annular integration and quiet selectors and prove that its varying birth
   sectors have the relative comparison needed for the exchange identity.
   An arbitrary earlier `T_h` is not a weakly perturbed convex Gaussian by
   this argument. The theorem is not a replacement for that missing step.

## 6. A flat local reference using only native small curvature

The global link hypothesis in (RMg.23) can be replaced, for a local
marginal, by small curvature and a local gauge on a buffered patch. The
following quadratic comparison makes the boundary price explicit.

### Lemma RMg.3 -- a local comparison of two positive precisions

Let `K_0,K_1>=lambda I` have common exponentially summable absolute rows,
on the same coordinate graph and the same fixed convex product cutoff.
Put `B=K_1-K_0` and `b_i=sum_j ||B_ij||`. For a marginal on D, their
normalized Gaussian product-domain densities obey

\[
 \left|\log\frac{p_{K_1,D}(u)}{p_{K_0,D}(u)}\right|
 \le CP^2\sum_{i\in D}\sum_a e^{-\kappa d(i,a)}b_a.
                                                               \tag{RMg.28}
\]

In particular, if `b_a<=epsilon` on the r-neighborhood of D and
`b_a<=C` everywhere, then

\[
 \left|\log\frac{p_{K_1,D}}{p_{K_0,D}}\right|
 \le C|D|P^2\{\epsilon+e^{-\kappa' r}\}.           \tag{RMg.29}
\]

**Proof.** Use `K_theta=K_0+theta B`, which has the same positive gap by
convexity, and use the potential perturbation `W_B=-z^T B z/2`.
It is not required to have a small global Hessian: positivity is supplied
by the two endpoint precisions. Its coordinate gradient is bounded by
`CP b_a`. The derivative of its conditional expectation at a pinned
coordinate i has the direct term and covariance with
`-(K_theta z)_i`. Retain the spatial weights in (RMg.7), instead of
replacing all `b_a` by their supremum. The covariance term is at most

\[
 CP\sum_{a,b} b_a e^{-\kappa_0 d(a,b)}
                         \|(K_\theta)_{ib}\|
 \le CP\sum_a e^{-\kappa d(i,a)}b_a.               \tag{RMg.30}
\]

The direct term has the same bound. Integrate the pinned variables over
their O(P) coordinate diameters, then use the normalized theta derivative
(RMg.17). This proves (RMg.28). Polynomial graph growth and a fixed
decrease of the exponent prove (RMg.29). The proof applies equally with
the convex boundary barriers and their hard limits. \(\square\)

### Corollary RMg.4 -- flat local first-step comparison on native backgrounds

Consider the actual first globally P/Q-regular source chart, with admitted
retained coarse curvature at most `epsilon=O(gP)`. Let D have diameter
at most `C_*R` in first free-coordinate blocks and `|D|<=C_*R^4`. Let its
R-sized enlarged patch fit in the admitted contractible source domain.
Use the actual gauge-invariant product norm balls, with the same radii
on the interacting and reference sides.

On the enlarged patch choose a coarse axial gauge. Each gauged coarse
link is a product of O(R^2) parallel-transported plaquette holonomies, so
it differs from identity by `C R^2 epsilon`. Extend that coarse gauge
arbitrarily outside the patch. Its block-constant fine lift acts
orthogonally on the actual free coordinates by CMP119 (1.17), preserving
the product cutoff and its measure.

The local raw lift `Q^fV` is correspondingly close to identity in the
patch. Its force is O(epsilon) everywhere, in norm, and the verified
force-resolved variational estimate gives
`||A_bg||_infty<=C||J(Q^fV)||_infty<=C epsilon`.
Thus the actual minimizing field is `O(R^2 epsilon)` from identity in
that local gauge. This step uses the original variational equation; it
does not declare the local raw lift stationary.

The source precision has finite free-coordinate stencils. Its local
analytic formulas, including the constraint Hessian and actual current,
therefore give, on an R-buffer of D,

\[
 \sum_j\|K(V)^u_{ij}-K_{{\rm flat},ij}\|
       \le C R^2\epsilon .                         \tag{RMg.31}
\]

Here the gauge patch contains the fixed stencil halo as well. The same
row is bounded by a fixed constant globally. Both precisions have a
uniform gap by the actual first-step gap theorem; the gauge is
orthogonal. Apply RMg.29, and then RMg.18 for the complete W on this
same gauged chart. It follows that

\[
 \left|\log\frac{p_{V,D}(u)}{p_{{\rm flat},D}(u)}\right|
 \le C|D|\{gP^3+g^2P^2
              +P^2R^2\epsilon+P^2e^{-\kappa R}\}
       =:\Delta_D.                                \tag{RMg.32}
\]

The left side uses the gauged actual free coordinates. For an observable
or selector invariant under the block adjoint transformations, such as
the literal free-coordinate R max-norm test, this is the same event in
the original coordinates. With `epsilon=O(gP)` and `|D|=O(R^4)`,

\[
 \Delta_D\le C\{gP^3R^6+g^2P^2R^4
                            +P^2R^4e^{-\kappa R}\}=o(1).
                                                               \tag{RMg.33}
\]

All constants are independent of total volume and of the native
background within this admitted class. No global small-link event or
global axial gauge is needed. This conclusion concerns local first-step
marginals, not a comparison of a later completed residual integral.

## 7. Canceling the normalization of a locally enlarged cutoff

There is an exact way to compare a local birth defect to a common
all-small baseline without losing a moving partition function. Let
`K_D` have a fixed enlarged radius `bP`, `b>1`, on D and radius P
elsewhere. Let `K_P` have radius P everywhere. Both use the **same**
actual first-step density. Denote their unnormalized partition functions
by `Z_D(V)` and `Z_P(V)`, and the normalized product-domain law on `K_D`
by `mu_{V,D}^{box}`. For any event E measurable in the D coordinates,

\[
 \frac{\int_{\mathcal K_D}{\bf1}_{E}e^{-H_V(z)}dz}
      {Z_P(V)}
   =\frac{\mu_{V,D}^{\rm box}(E)}
          {\mu_{V,D}^{\rm box}(z_D\in\mathcal K_{P,D})}.
                                                               \tag{RMg.34}
\]

This follows because the event in the denominator cuts `K_D` back
exactly to `K_P`; all outside coordinates already have radius P.
The all-P normalization is the same for every translated D.

Apply (RMg.32) to the two local events in (RMg.34). Their ratio to the
corresponding flat Gaussian defect weight lies in

\[
 [e^{-2\Delta_D},e^{2\Delta_D}].                    \tag{RMg.35}
\]

No lower bound on either event mass is needed. If D and E are translated
by a first-coarse-lattice translation, the flat Gaussian defect weight
is exactly unchanged: its precision, all-P baseline, translated product
cutoff and event transform together. This gives a relative comparison
of actual local first-step defect weights at different positions after
division by the one **common** source baseline `Z_P(V)`.

The proof has not assumed that `Z_D(V)` itself is independent of position.
Nor has it replaced the source cutoff by an enlarged one in the final
law: an actual source sector must be identified as the corresponding
event E inside this encompassing product domain.

### Primary sources and companion proofs

- CMP119 (1988), pp.248--251: the first conditional integral, exact local
  free-coordinate constraint solve, Gaussian normal form and its measure.
- CMP109 (1987), (0.8), (0.11): the actual averaged-contour soft gauge.
- [first step precision gap](first_step_precision_gap.md), PG.1--PG.5: the actual constrained positive
  gap, including the source soft gauge and exceptional-coordinate embedding.
- [local extension kernel](local_extension_kernel.md), Sections 3.3--3.4: complete first-step
  normal-form factors, their local analytic stencils and source-free budgets.
- [local coupling source](local_coupling_source.md), Sections 8--11: the original first-clean
  normalized marked construction. The new relative estimate here does not
  follow merely by dividing that note's absolute error by a rare-event mass.
