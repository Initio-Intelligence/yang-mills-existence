# Unmarked energy-weighted component logarithms for the regular Q density

This theorem is a conditional analytic tool for the completed-component
part of the regular-Q density. It uses the actual old unmarked energy
reserve. It does not require a localized microscopic old-mark moment.
The construction of the raw-local reference and of the actual supported
density coefficients remains a source-specific task.

## 1. Hypotheses and actual supports

Let D₀ be a connected current core of uniformly bounded physical
cardinality. Let ν₀(v_{D₀},du) be a positive probability kernel whose
dependence on retained raw data is genuinely confined to D₀. Its old
space may contain arbitrarily many variables and a mixture of old
histories. At each finite cutoff it is a common padded measurable space.

Assume a nonnegative old energy/rank envelope E≥1 satisfies

\[
 \nu_0(E^m)\le m!K^m,\qquad m=0,1,\ldots,
 \qquad K\ge1.                                       \tag{UL.1}
\]

There is no deterministic bound on the old rank. For the proposed
source application the actual RT reserve has K=C(1+P²); transferring
that reserve to a constructed reference requires the exact comparison
in EW.2 or a direct proof, not a change of normalization.

Let the complete difference of old log densities, with retained-only
factors consistently removed, have an actual raw carrier expansion

\[
 \Sigma(v,u)=\sum_{X\supset D_0}\sigma_X(v_X,u),
 \qquad |\sigma_X|\le a_XE,
 \qquad
 \epsilon=\sum_X w_\kappa(X)a_X,
 \qquad q=K\epsilon<\tfrac12.                         \tag{UL.2}
\]

All carrier sets are connected and contain D₀. A tag includes every
retained raw, selector, graph, and history coordinate on which its
function actually depends. A global label is not replaced by a core
label without the required locality identity. All suprema over retained
data precede the coefficient sum. For analytic current conclusions the
core datum may remain real while the external/current perturbation
coordinates vary on the common complex contour. The positive reference
then remains the same probability kernel. A complex continuation of the
reference itself instead requires an absolute operator-moment bound;
positivity at the real center alone is not such a bound.

Define the actual relative partition function and its distinguished
logarithm by

\[
 Z(v)=\nu_0(e^\Sigma),\qquad W(v)=\log Z(v),
 \qquad W=0\text{ when }\Sigma=0.                      \tag{UL.3}
\]

The reference is normalized. Thus any reference-only mass has already
been factored consistently out of numerator and denominator; it is not
used again as a small probability.

## 2. Absolute physical-carrier expansion of the logarithm

### Theorem UL.1

Under (UL.1)–(UL.2), W has an absolutely convergent tagged expansion in
actually supported carriers, and

\[
 \boxed{
 \|W\|_{\mathrm{car},\kappa}
 \le \log\frac{1-q}{1-2q}.}
                                                               \tag{UL.4}
\]

In particular its complete carrier budget is O(q) at a fixed margin
q≤q_*<1/2. The constant does not depend on the old rank.

**Proof.** Put d=ν₀(e^Σ−1). Expand the exponential into ordered words
and keep their original carrier tags. The length-n absolute carrier
budget is at most

\[
 \frac{\epsilon^n}{n!}\nu_0E^n\le q^n.
\]

The union of a word's carriers is connected because all contain D₀,
and its weight is bounded by the product of their weights. Therefore

\[
 \|d\|_{\mathrm{car},\kappa}
       \le \frac q{1-q}=:s<1.                         \tag{UL.5}
\]

The same positive series proves absolute integrability, including
ν₀e^{εE}≤(1−q)^{-1}. The series

\[
 W=\sum_{m\ge1}\frac{(-1)^{m+1}}m d^m                \tag{UL.6}
\]

then converges in this carrier algebra. Every product in it again has
the support union of its displayed tags; no cancellation is used to
bound a tag. Its norm is at most −log(1−s), which is (UL.4).
For complex perturbation parameters with the stated absolute bounds,
(UL.5) also proves that Z=1+d is nonzero and
chooses the logarithm in (UL.3). ∎

The result concerns the old scalar density factor. If a present-current
mark f(z,v) is independent of u, it factors exactly through this old
integration:

\[
 \nu_0\{f(z,v)e^\Sigma\}=f(z,v)Z(v).                 \tag{UL.7}
\]

No bound for ν₀(|F_micro|E^n) is needed to justify (UL.7). This is the
specific reason that the unresolved microscopic reset localization
problem EW.13 is not an extra hypothesis of the unmarked regular-Q
boundary-density estimate.

## 3. Current derivatives when the core reference is fixed

Let the differentiated current coordinates be outside D₀, so that ν₀
is independent of them. Assume actual tagged derivative majorants

\[
 \sum_d|D_d\sigma_X|\le a_{1,X}E,
 \qquad
 \sum_{d,e}|D_dD_e\sigma_X|\le a_{2,X}E,
 \qquad
 \epsilon_r=\sum_Xw_\kappa(X)a_{r,X},\quad r=1,2.
                                                               \tag{UL.8}
\]

Directions, endpoint weights and enlarged footprints are those of the
claimed application. For a Hessian row rather than the total displayed
sum, the same proof uses the corresponding rooted/weighted multilinear
majorant and preserves it under carrier convolution.

The separate derivative tags obey

\[
 \boxed{
 \|DW\|_{\mathrm{car},\kappa}
 \le\frac{K\epsilon_1}{(1-q)(1-2q)}.}                \tag{UL.9}
\]

The complete second derivative, with its two contributions kept, obeys

\[
 \boxed{
 \begin{aligned}
 \|D^2W\|_{\mathrm{car},\kappa}
 \le{}&\frac{K\epsilon_2}{(1-q)(1-2q)}\\
 &+\frac{K^2\epsilon_1^2(3-4q)}
 {(1-q)^2(1-2q)^2}.
 \end{aligned}}                                      \tag{UL.10}
\]

**Proof.** The absolute series gives

\[
 \|Dd\|\le\frac{K\epsilon_1}{(1-q)^2},
 \qquad
 \|(1+d)^{-1}\|\le\frac{1-q}{1-2q}.                  \tag{UL.11}
\]

Their product proves (UL.9). For the second derivative,

\[
 \|D^2d\|
 \le\frac{K\epsilon_2}{(1-q)^2}
       +\frac{2K^2\epsilon_1^2}{(1-q)^3}.             \tag{UL.12}
\]

Use the exact identity

\[
 D^2W=(1+d)^{-1}D^2d-(1+d)^{-2}(Dd)(Dd).
\]

Multiplying the absolute carrier bounds, then adding rather than
cancelling the two terms, yields (UL.10). ∎

For the C-08 application, if K=O(P²), ε=o(P^{-2}), and the actual
current contour gives ε₁≤Cε/P and ε₂≤Cε/P², then

\[
 \|DW\|\le C K\epsilon/P,
 \qquad \|D^2W\|\le C(K\epsilon+(K\epsilon)^2)/P^2.
                                                               \tag{UL.13}
\]

This supplies a small rooted scalar prefactor Kε. Neither the contour
nor the actual coefficient inequalities are inferred from this algebra.

## 4. Reference responses in retained core directions

Core retained-data directions can change ν₀. That response must be
included. For a differentiable common-support family write its centered
score as S_d, so ν₀S_d=0. Then

\[
 D_dZ=\nu_0(e^\Sigma D_d\Sigma)
       +\nu_0\{S_d(e^\Sigma-1)\}.                   \tag{UL.14}
\]

The subtraction of one is exact. A reference derivative does not
generate a zero-interaction term.

For example suppose, on the required common rectangular two-copy
paths,

\[
 \sum_d|S_d|\le A_0E,
\]

with its core carrier retained. Then the reference part satisfies

\[
 \begin{aligned}
 \|D_{\rm ref}d\|
 &\le A_0 K\sum_{n\ge1}(n+1)q^n
   =A_0K\frac{q(2-q)}{(1-q)^2},\\
 \|D_{\rm ref}W\|
 &\le A_0K\frac{q(2-q)}{(1-q)(1-2q)}.
 \end{aligned}                                      \tag{UL.15}
\]

This is a sufficient explicit score budget, not a theorem that the
actual reference has it. A smaller square-root-energy score gives the
corresponding gamma-function series and can improve the K power.

A version not requiring a density score uses the signed variation
kernel. If ν₀ is normalized and

\[
 \int E^n\,|\delta_d\nu_0|(du)
      \le A_d n!K^n\quad(n\ge1),
 \qquad A=\sum_d A_d,                                \tag{UL.16}
\]

then normalization again removes its action on one and

\[
 \boxed{\|D_{\rm ref}W\|
       \le\frac{Aq}{1-2q}.}                          \tag{UL.17}
\]

To prove this, apply (UL.16) to the n≥1 exponential words, giving
Aq/(1−q), and multiply by the inverse bound in (UL.11). For genuine
continuous differences (UL.16) is substantive; finite endpoint total
variation alone has a 1/|t| loss and does not prove it.

For a discrete replacement the denominator is one. Endpoint expansions
of W may instead be subtracted directly, on a common universe of
tags, charging the union of their core/interaction footprints. Their
combined absolute budget is at most the sum of their two bounds
(UL.4). This requires no common continuous rank, but it retains the
actual footprint of the changed descriptor and all its affected
interactions. Summing over many discrete directions still incurs the
displayed direction count or a sharper locality estimate.

## 5. Finite differences, ambient versions and the actual gate

All differential estimates above become finite-difference records by
integrating on the corresponding independent insertion/kernel paths,
provided the estimates and energy moments hold on those paths. A
diagonal-only moment theorem does not supply the two-copy assertion.
An inactive reference-point extension can introduce a jump. Any positive
analytic extension used to avoid that jump must be recorded as the
actual ambient version in Annex Y.

To apply UL.1 to the source completed component, it remains to prove:

1. A positive reference whose **raw** retained dependence is confined
   to a bounded current core, with the same old support and exact
   normalizations. Native analyticity in an externally declared (U,J)
   pair is not by itself this assertion.
2. An actual carrier expansion of every old precision, Schur, nonlinear
   action, coarea and reconstruction difference, with energy-weighted
   coefficients satisfying (UL.2) on the complete common data. A
   per-mode perturbation O(g_k poly(P,R)) is enough if it multiplies
   the actual total energy/rank envelope and Kε is small; no
   deterministic bound on the old rank is required.
3. The old hard selectors must be common on that representation, or
   their actual changes must be treated. A hard support difference
   is not an analytic log-density coefficient.
4. The core reference responses and discrete label changes must obey
   their actual current budgets, with complete physical footprints.

The existing RT/EW reserve and the ordinary old-slot geometry are
useful inputs to this calculation. They do not prove these four
identifications. Once those source inputs are established, the
unmarked completed-component logarithm and its current response
follow by the absolute expansions above, without the separate
microscopic reset-mark moment which obstructed the earlier residual
route.
