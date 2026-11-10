# Composition of mixed kernels on a compact state

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

## 0. Result and exact scope

The alternative in item 3 of the finite-volume mixed-kernel calculation can be
proved: retain a countable family of bounded physical and archived
probes, all their products, and all their pullbacks by the actual
normalized source-free kernels. There is then one compact metrizable
state space on which those kernels have continuous probability-kernel
extensions. One subsequence of the actual Wilson sequence has a joint
limit preserving every finite kernel composition and every bounded
source-jet identity.

The construction uses the kernels themselves, not a proposed common
Lebesgue/Haar density for different cutoffs. A bound on a sum of
functions is never used as a bound on the sum of their absolute values.
Products of archived coefficients are retained jointly before taking a
limit. Tiny canonical masses cause no singularity in complete
mass-retaining expressions.

This proves an enlarged-state composition theorem. The state generally
contains more information than the limiting active raw coordinates.
It does not assert that the canonical limiting RG operation can be
recomputed from those raw coordinates alone. It also does not remove
the truncation of an unbounded physical insertion. The recent separated
hierarchy estimate ER.7, physical normalization/nondegeneracy and the
remaining existence requirements are separate.

The proofs below have the following statuses:

- **P:** the compactification, kernel composition, bounded source
  reweighting and finite analytic-jet theorems are proved here.
- **L/input:** the literal finite-cutoff positive construction,
  complete masses and native comparison are the supplied source
  formulas and the retained C01/C05 scope identified in Section 1.
- **C:** removal of an unbounded-insertion truncation requires its
  actual joint uniform-integrability estimate.
- **O:** identifying the enlarged state with an autonomous raw-field
  RG state, recomputing all hard selectors, ER.7 and Yang--Mills
  existence are not concluded.

## 1. The actual finite-cutoff objects

### 1.1 Full-law kernels and their marginals

Use the actual source-free positive lift of one cofinal Wilson sequence.
At a chosen retained interface, the state contains the actual geometry,
coarse fields, surviving old raw variables, selector/preparation labels,
and all retained action and archive data needed by the next operation.
In particular a recent multiplier
\[
 \tau_b(V_b)=T'_b(Y_b)1
 \tag{MK.1}
\]
is not replaced by its scalar mass or by the age of its explicit
argument. Its already integrated older history remains in its actual
function and in every queried evaluation of that function.

At finite cutoff these states are standard Borel: they are assembled
from the finite source geometry/history labels and the actual
finite-dimensional group and free-coordinate variables. An archive
function can be specified by its literal finite-cutoff construction and
parameters; no topology on all measurable functions is needed here.

Let \(\mu_n^s\) and \(\mu_n^t\) be the actual probability marginals at
two interfaces, and let \(P_n^{st}\) be an actual normalized conditional
kernel, oriented from its conditioning state to the variable it
integrates. Then
\[
 \mu_n^s P_n^{st}=\mu_n^t,\qquad P_n^{st}1=1.
 \tag{MK.2}
\]
The equality of marginals is essential. It makes \(P_n^{st}\) a
well-defined map
\[
 L^\infty(\mu_n^t)\longrightarrow L^\infty(\mu_n^s):
 \qquad \|P_n^{st}f\|_\infty\le\|f\|_\infty.
 \tag{MK.3}
\]
Indeed a \(\mu_n^t\)-null set has zero conditional probability for
\(\mu_n^s\)-almost every conditioning state, by (MK.2).

These are law-level statements. A conditional kernel on a null fiber
can have different versions; this proof does not identify its value at
every arbitrary raw configuration. A prescribed counterfactual query
may be added as its own type, including a deterministic admitted
input, but uncountably many unrestricted raw inputs are not covered
merely by an almost-everywhere conditional law.

The exact source-jet transport CS.5--CS.11 uses these full-law
conditional kernels. Its chronological composition identities are
retained as identities of these operators. Arbitrary conditional
expectations onto nonnested sigma fields do not satisfy a tower
identity and are not substituted for them.

There is no need to enlarge a conditioning sigma field by unknown
future labels in the proof below. We preserve the actual kernels on
their own interface spaces. If a chronology requires further data to
be a sufficient interface, those data are retained before defining
\(P_n^{st}\). A factorization is asserted only at a literal source
cut. In the supplied construction, the ordered operations in
CMP119 (2.19)--(2.22), printed p.258, and the complete retained action
(2.23) specify these interfaces. Gauge restoration is used only after
its integrated gauge-invariant identity, as required on LFR II p.378.

### 1.2 Canonical component kernels are not silently full-law kernels

For a source component the canonical normalized operator is
\[
 \Pi_{n,X}=\tau_{n,X}^{-1}T'_{n,X},\qquad
 \tau_{n,X}=T'_{n,X}1.
 \tag{MK.4}
\]
It is a positive probability kernel at real admitted data. Its
reference law need not be the marginal \(\mu_n^t\) of an independently
chosen physical cut. Therefore it cannot simply be inserted into
(MK.3) with that marginal.

To include such a kernel, give it an auxiliary query type. Draw its
input from the actual input marginal, apply the literal \(\Pi_{n,X}\),
and define the query-output marginal to be precisely that pushforward.
The output retains the input environment whenever a later query needs
it. Repeating this construction for a finite query word gives its
actual iterated reference law. There are countably many finite words
in a countable list of source queries.

Only source-admitted composable query words are included. An
auxiliary pushforward law does not prove that a later canonical
operation is admitted on its outputs; that operation must already
be defined on the declared input law and domain. No new admissible
history class is introduced by this notation.

Thus every added edge again satisfies (MK.2), on its own declared
types. Complete joint component operations are retained as joint
operators. They are not reconstructed by multiplying separately
extracted limiting kernels.

If two query words reach the same kind of raw variable with different
induced laws, keep different output types and copy the literal bounded
test into both. A source equality between the two calculations is then
an equality of their output probe arrays at the common input type.
That equality passes there. The two output reference measures are
not identified, and no kernel is applied to an \(L^\infty\)
equivalence class for the wrong output law.

For the literal component in LFR II (1.71), p.378 allows either the
first or the second component class. The fundamental bound on p.387,
(1.89), gives at the admitted real source data
\[
 0<\tau_{n,X}
 \le \exp\{-2(1+\beta_0)^{-1}p_0(g_{n,k})\}\le1.
 \tag{MK.5}
\]
Absent component slots may be padded by \(\tau=0\) and any fixed
dummy probability kernel. These particular canonical mass coordinates
and their products are uniformly bounded. A broader unnormalized
branch weight is not assigned (MK.5) unless it is literally one of
these source masses.

The complete source grouping is the one on LFR II pp.391--392:
\[
 \left(\prod_i\tau_{n,i}\right)
 \left(\prod_i\Pi_{n,i}\right)F
 =
 \left(\prod_iT'_{n,i}\right)F.
 \tag{MK.6}
\]
The operators on disjoint components have their literal factorization;
overlapping operations retain their chronological order. No mass is
used twice after conditional normalization has canceled it.

### 1.3 A countable diagram, with no common raw reference

Write \(\mathcal T\) for the countable list of interface and auxiliary
query types and \(\mathcal E\) for the countable list of kernel arrows.
Each arrow \(e:s\to t\) is described by
\[
 (S_n^s,\mu_n^s),\quad (S_n^t,\mu_n^t),\quad P_n^e,
 \qquad \mu_n^sP_n^e=\mu_n^t.
 \tag{MK.7}
\]
The state spaces, coordinate dimensions and measures may depend on
\(n\). Their common-reference or total-variation compactness is not
assumed.

We also prescribe countably many uniformly bounded probe arrays
\[
 f=(f_n),\qquad
 \sup_n\|f_n\|_{L^\infty(\mu_n^t)}<\infty.
 \tag{MK.8}
\]
They include:

1. bounded continuous generators of the actual local active-record
   coordinates, using bounded transforms for Euclidean coordinates;
2. the literal discrete labels and bounded archive evaluations;
3. bounded physical Wilson probes, including any fixed truncations
   of the actual microscopic source observables;
4. canonical masses (MK.5), their complete products, and the
   corresponding bounded source moments;
5. any additional bounded probes required by a specified finite
   source calculation.

All finite products and kernel pullbacks will be added by the
construction. There is no assertion that an unbounded physical
field already satisfies (MK.8).

An interface at a fixed physical offset may be absent for finitely
many early cutoffs. It can be padded by a one-point state. Alternatively,
the formulas may be read modulo arrays whose uniform norm tends to
zero as \(n\to\infty\). Section 4 proves that these early choices do
not affect the limiting construction.

## 2. Close the observable algebra before taking a limit

For each type define the commutative normed function space
\[
 \mathcal B_t
 =\left\{(f_n):\
 f_n\in L^\infty(\mu_n^t),\
 \sup_n\|f_n\|_\infty<\infty\right\},
 \qquad
 \|f\|_{\mathcal B_t}=\sup_n\|f_n\|_\infty.
 \tag{MK.9}
\]
With pointwise multiplication and conjugation, this is a unital
commutative \(C^*\)-algebra. In particular products at a fixed cutoff
are part of the object, not operations performed after weak limits
of separate factors.

Every real source kernel induces the positive unital contraction
\[
 \mathsf P^e:\mathcal B_t\to\mathcal B_s,
 \qquad
 (\mathsf P^ef)_n=P_n^ef_n.
 \tag{MK.10}
\]
Equation (MK.2) proves that this definition respects the
almost-everywhere equivalence classes in every component of (MK.9).

Include the cutoff coordinate
\[
 c_t=(1/n)_{n\ge1}
 \tag{MK.11}
\]
among the probes at every type.

### Lemma MK.1 — a separable invariant algebra exists

There are separable unital selfadjoint closed subalgebras
\(\mathcal A_t\subset\mathcal B_t\), containing the prescribed
probes, such that
\[
 \mathsf P^e\mathcal A_t\subset\mathcal A_s
 \quad\text{for every }e:s\to t.
 \tag{MK.12}
\]

**Proof.** At stage zero take the closed unital selfadjoint algebra
generated by the countable prescribed probes. If the stage-\(r\)
algebras have been chosen, choose countable norm-dense subsets in
them and adjoin to the source algebra the images of those subsets
under every incoming operator \(\mathsf P^e\). Generate the next
closed unital selfadjoint algebras.

Every stage is separable because there are only countably many
generators, rational complex polynomials and arrows. Take the norm
closure of the increasing union over all stages. Since every
\(\mathsf P^e\) is a contraction, approximation by a dense subset
and then by finite stages proves (MK.12). \(\square\)

Closing only the initial probe family under a single conditional
expectation would not suffice. A later source operation can act on
a product of earlier conditional moments. The iteration in the proof
adds precisely those products and their further pullbacks, to every
finite depth.

## 3. A compact state and genuine Feller kernels

### Lemma MK.2 — concrete compact realization

For every type \(t\) there is a compact metrizable space \(X_t\)
and an isometric identification
\[
 \mathcal A_t=C(X_t).
 \tag{MK.13}
\]
The probability \(\mu_n^t\) induces a probability
\(\bar\mu_n^t\) on \(X_t\), with
\[
 \int_{X_t}\widehat f\,d\bar\mu_n^t
 =\int_{S_n^t}f_n\,d\mu_n^t
 \quad(f\in\mathcal A_t).
 \tag{MK.14}
\]
Joint products of probes have the same equality.

**Proof.** Enumerate a countable selfadjoint algebraic generating
family \(a_1,a_2,\ldots\), including a norm-dense family in
\(\mathcal A_t\). Choose bounded measurable versions at each \(n\).
All of their countably many algebraic relations hold on one
full-measure subset at that \(n\).

Map the state into the countable product of closed disks by
\[
 y\longmapsto(a_{1,n}(y),a_{2,n}(y),\ldots).
 \tag{MK.15}
\]
Each disk has the corresponding fixed uniform radius. Let \(X_t\)
be the closure of the union, over \(n\), of the supports of the
pushforward probabilities. It is compact and metrizable.

For a polynomial \(p\) in finitely many coordinates and their
conjugates,
\[
 \sup_{X_t}|p|
 =\sup_n\operatorname*{ess\,sup}_{\mu_n^t}
       |p(a_{1,n},a_{2,n},\ldots)|.
 \tag{MK.16}
\]
This is immediate from the definition by supports and closure.
Thus the coordinate algebra is isometric to the corresponding
subalgebra of \(\mathcal B_t\). It separates points, contains
constants and is selfadjoint. Stone--Weierstrass identifies its
uniform closure with \(C(X_t)\), proving (MK.13).
The pushforward probabilities prove (MK.14), first on polynomials
and then by uniform approximation. \(\square\)

### Theorem MK.3 — extension of every actual kernel

For every \(e:s\to t\), there is a probability kernel
\[
 \bar P^e(x,dy),\qquad x\in X_s,\quad y\in X_t,
 \tag{MK.17}
\]
such that
\[
 \widehat{\mathsf P^ef}(x)
 =\int_{X_t}\widehat f(y)\,\bar P^e(x,dy).
 \tag{MK.18}
\]
It is Feller: the right side is continuous in \(x\) for every
\(\widehat f\in C(X_t)\). The finite-cutoff probabilities satisfy
\[
 \bar\mu_n^s\bar P^e=\bar\mu_n^t.
 \tag{MK.19}
\]
Every exact prelimit operator composition identity extends exactly
to these kernels.

**Proof.** Under (MK.13), \(\mathsf P^e\) is a positive unital
linear map \(C(X_t)\to C(X_s)\). At a fixed \(x\), evaluation of
this map is a positive functional of value one on the constant
function. The Riesz representation theorem gives the unique
probability in (MK.17). Equation (MK.18) and membership in
\(C(X_s)\) give the Feller property and weak continuity of the
measure-valued map.

Integrating (MK.18) against \(\bar\mu_n^s\), using (MK.14) and
(MK.2), proves (MK.19). For a countable dense family of continuous
tests, (MK.18) also represents the pushed-forward original kernel
for \(\mu_n^s\)-almost every actual input. Thus it is a representation
of the actual finite-cutoff kernels, not a new choice of their
conditional expectations.

If, for example, \(P_n^{su}P_n^{ut}=P_n^{st}\) holds almost
everywhere at every \(n\), it is an equality in the spaces (MK.9).
Its restriction to \(\mathcal A_t\) is therefore an equality of
continuous functions on \(X_s\). Measures on \(X_t\) are determined
by continuous tests, so
\[
 \bar P^{su}\bar P^{ut}=\bar P^{st}.
 \tag{MK.20}
\]
The same argument treats every specified finite operator diagram.
No new tower identity is asserted for kernels whose original
diagram did not have one. \(\square\)

### 3.1 Why the cutoff fiber is preserved

An actual kernel never changes the cutoff index. Therefore
\[
 \mathsf P^ec_t=c_s,\qquad
 \mathsf P^e(c_t^2)=c_s^2.
 \tag{MK.21}
\]
Both identities are retained in the algebra. Consequently, for
every \(x\in X_s\),
\[
 \int_{X_t}\bigl(c_t(y)-c_s(x)\bigr)^2
                         \bar P^e(x,dy)=0.
 \tag{MK.22}
\]
The kernel is supported on the exact same cutoff fiber. In
particular it restricts to a probability kernel between
\[
 X_t^0=\{x\in X_t:c_t(x)=0\}.
 \tag{MK.23}
\]
This uses the first and second moments, not an unsupported inference
from preservation of a mean at a nonzero fiber.

## 4. One limit preserves the complete bounded calculus

### Theorem MK.4 — simultaneous mixed-kernel limit

Along one subsequence, all \(\bar\mu_n^t\) converge weakly to
probabilities \(\bar\mu_\infty^t\) supported on \(X_t^0\).
They satisfy
\[
 \bar\mu_\infty^s\bar P^e=\bar\mu_\infty^t.
 \tag{MK.24}
\]
All finite path laws built from the retained kernels and all finite
joint bounded-probe expressions converge along this same subsequence.
The limiting conditional kernels obey every retained composition
identity.

**Proof.** Probability measures on each compact metrizable \(X_t\)
are sequentially compact. A diagonal extraction over the countable
types gives one subsequence. Since
\(\int c_t\,d\bar\mu_n^t=1/n\), every limiting measure is supported
on (MK.23). The Feller property permits passage in (MK.19), proving
(MK.24).

For a finite path \(t_0\to\cdots\to t_r\) and continuous bounded
tests \(f_j\), its mixed moment is
\[
 \int f_0\,
 \bar P^{e_1}\!\left[
 f_1\bar P^{e_2}\!\left[
 \cdots f_{r-1}\bar P^{e_r}f_r
 \right]\right]d\bar\mu_n^{t_0}.
 \tag{MK.25}
\]
The integrand is one fixed continuous function on \(X_{t_0}\).
Weak convergence proves its limit. Finite sums of such products
are dense in the continuous functions on the finite path product,
so the whole path law converges.

The expression at finite \(n\) is the exact original path integral
by (MK.18)--(MK.19). The same expression with
\(\bar\mu_\infty^{t_0}\) defines the limiting path law. Identities
(MK.20) hold on the zero fibers and prove the asserted consistency.
\(\square\)

This is more than extracting separate one-step measures. A product
formed during an intermediate normalized operation is already one
element of the invariant algebra before the limit is taken.

### 4.1 Eventual identities and uniform approximation errors

An array \(a\in\mathcal A_t\) vanishes on \(X_t^0\) exactly when
\[
 \|a_n\|_{L^\infty(\mu_n^t)}\longrightarrow0.
 \tag{MK.26}
\]
For the forward implication, if the norms did not tend to zero,
one could choose points in the corresponding supports, pass to a
compact subsequence with cutoff coordinate tending to zero, and
contradict continuity. The reverse implication follows directly
from closure of those supports. Equivalently, \(C(X_t^0)\) is
the quotient of the retained algebra by its vanishing-tail ideal.

Consequently identities holding for all sufficiently large \(n\),
or with an \(o(1)\) uniform error, hold on the zero fiber. A fixed
finite horizon missing at finitely many cutoffs causes no ambiguity.
All real kernels preserve the ideal by contraction.

If a source tail estimate gives
\[
 \sup_n\|F_n-F_n^{[A]}\|_\infty\le\varepsilon_A,
 \qquad \varepsilon_A\to0,
 \tag{MK.27}
\]
then the corresponding continuous functions differ by at most
\(\varepsilon_A\) on the entire compactification, and every real
normalized kernel preserves that error.

This applies, on the fixed finite geometry/native-root scopes
actually stated, to the HS regular \(E/R\) tails and the C05
relative-creation tail FK.7--FK.8. It does not delete an arbitrary
old internal portion of a canonical self multiplier \(\tau_b\).
That multiplier remains a separately retained archive probe.

### 4.2 Literal masses and complete component expressions

A bounded nonnegative mass array \(\tau\) is a nonnegative continuous
coordinate on \(X_s\). The unnormalized operation
\[
 T_nF=\tau_nP_nF
 \tag{MK.28}
\]
therefore extends as the finite positive kernel
\[
 \bar T(x,dy)=\widehat\tau(x)\bar P(x,dy).
 \tag{MK.29}
\]
It vanishes at a zero-mass state. A normalized kernel at that state
can retain additional limiting information, but the complete
mass-retaining expression is unambiguous.

All complete products in (MK.6), and all their bounded numerator
moments, are included before compactification. Thus (MK.6) passes
as an algebraic identity. For a complete canonical connected jet,
the additional finite-moment continuity result in
bounded source jets applies to its joint mass/moment
coordinates. No common raw reference measure is required by that
finite-coordinate application.

One must still use the actual outer measure and the literal
complete source grouping. Multiplying a mass into a coefficient
which did not carry that mass, or counting it again after its
cancellation, is not authorized by this construction.

## 5. Bounded physical sources and analytic parameters

### 5.1 A uniform bounded-source disk

Let \(H_{n,1},\ldots,H_{n,m}\) be actual bounded physical probes,
with \(|H_{n,i}|\le R_i\), inserted on the common source-free
positive space. Put
\[
 W_n(z)=\exp\left(\sum_i z_iH_{n,i}\right),\qquad
 \sum_i|z_i|R_i\le a<\pi/2.
 \tag{MK.30}
\]
Real and imaginary parts may be used to treat complex physical
probes as a finite real family. At every actual conditional cut,
\[
 Z_{n,k}(z)=Q_{n,k}W_n(z)
 \tag{MK.31}
\]
is holomorphic and satisfies
\[
 |Z_{n,k}(z)|\ge e^{-a}\cos a,\qquad
 |Z_{n,k}(z)|\le e^a.
 \tag{MK.32}
\]

**Proof.** For real \(H_{n,i}\), the imaginary part of the exponent
has absolute value at most \(a\), while its real part lies in
\([-a,a]\). The real part of \(W_n\) is at least
\(e^{-a}\cos a\). Integrating against a probability proves the
lower bound. The upper bound and holomorphy follow from the same
uniform bound and the entire exponential. \(\square\)

Thus the source-reweighted conditional law has the actual
normalized kernel
\[
 Q_{n,k}^{\,z}F
 =\frac{Q_{n,k}(W_n(z)F)}{Z_{n,k}(z)},
 \qquad
 |dQ_{n,k}^{\,z}|
 \le \frac{e^{2a}}{\cos a}\,dQ_{n,k}.
 \tag{MK.33}
\]
The numerator, conditional normalizer and its reciprocal belong to
the retained algebra after including the indicated probes: the
reciprocal is continuous functional calculus on the uniform
zero-free range.

For an intermediate chronological kernel the inherited source
factor is \(Z_{n,j}(z)\), and its denominator is \(Z_{n,k}(z)\).
The exact relation \(Z_{n,k}=P_n^{kj}Z_{n,j}\) gives the corresponding
source-reweighted kernel. Its identities pass by the same
construction. A new current-scale stencil is never substituted
for \(H_{n,i}\).

The bound is independent of cutoff depth, the number of earlier
history operations, and individual rare component masses. It
depends on the displayed bounded source amplitudes. It supplies
no bound when the actual physical probes fail to have a uniform
bounded envelope.

### 5.2 The complete finite jet

For bounded actual insertions \(H_i\), the conditional moment
coordinates
\[
 M_{I,k}=Q_k\prod_{i\in I}H_i
 \tag{MK.34}
\]
are among the retained pullbacks. Their joint limiting values
define the finite nilpotent jet
\[
 \mathcal Z_k(\varepsilon)
 =1+\sum_{\varnothing\ne I}\varepsilon_I M_{I,k}.
 \tag{MK.35}
\]
All products in the finite logarithm are continuous functions of
these joint coordinates. The original identity consequently gives
\[
 \mathcal Z_{k+1}=P_{k+1}\mathcal Z_k,\qquad
 \mathcal H_{k+1}=\log P_{k+1}e^{\mathcal H_k}.
 \tag{MK.36}
\]
Every higher source vertex and every outer conditional-mean term
is retained. This is the limiting bounded-source version of
CS.6--CS.11. The complementary moment-cone paper gives the
complete mass-weighted version, including zero-mass branches.

### Theorem MK.5 — native/analytic kernel families

Suppose an actual kernel arrow has an admitted common finite-dimensional
polydomain \(D^+\) and a holomorphic complex family \(P_{n,\zeta}\)
on one fixed real output measurable space \(S_n^t\) at that cutoff.
The real input environment is retained in this raw-reference type
when the integration fiber depends on it. Assume that, uniformly
over its actual real input data,
\[
 P_{n,\zeta}1=1,\qquad
 |dP_{n,\zeta}|\le M\,dP_{n,0}.
 \tag{MK.37}
\]
Use precisely the source family for which this has been proved.
Then the algebras may be chosen to include all its parameter
values. On the compactified state, it extends to normalized complex
kernels \(\bar P_\zeta\) with
\[
 |d\bar P_\zeta(x,\cdot)|
       \le M\,d\bar P_0(x,\cdot).
 \tag{MK.38}
\]
Their bounded analytic probes, all fixed derivatives on a strict
smaller polydomain, and every finite composition of such verified
families pass along the same subsequence.

**Proof.** Repeat the iterative construction of Lemma MK.1 with the
additional bounded linear pullback operators at a countable dense
set of parameter values. Include conjugates of all resulting
functions when forming the selfadjoint algebra. Thus inputs
created by an earlier complex operation also receive all later
pullbacks. For each bounded input,
the uniform bound in (MK.37) and Cauchy's formula give uniform
equicontinuity in the \(\mathcal B_s\) norm on every smaller
polydomain. Approximation by dense parameter values therefore
places every \(P_\zeta f\) in \(\mathcal A_s\).

The same Cauchy estimates prove norm-holomorphy. In particular, if
the contour margin in coordinate \(j\) is \(\delta_j\), then
\[
 \|\partial^\alpha_\zeta P_\zeta f\|_{\mathcal A_s}
 \le M\,\alpha!\prod_j\delta_j^{-\alpha_j}\,
                         \|f\|_{\mathcal A_t}.
 \tag{MK.39}
\]
For a holomorphic bounded input family, apply the same argument
to the complete composed function. The parameter pullback and
kernel response terms are both included by this composition.

At a fixed input point of \(X_s\), evaluation is a bounded linear
functional on \(C(X_t)\). Its norm is at most \(M\), so Riesz gives
a complex measure. The pointwise inequality
\[
 |P_\zeta f|\le M P_0|f|
 \tag{MK.40}
\]
holds in every prelimit \(L^\infty\) space and hence in the compact
algebra. Positivity of the continuous right side and approximation
by continuous test functions imply the variation domination
(MK.38). The mass-one identity also passes.

For a finite operator word, the resulting output is one
holomorphic \(C(X)\)-valued function. Its norm on a common larger
domain is bounded by the product of the displayed finite operator
constants and the input bound. Weak convergence of the initial
measure gives convergence at each parameter. Uniform Cauchy
bounds give local uniform convergence and convergence of every
fixed derivative on a smaller domain. Equivalently one can
integrate the fixed Cauchy contour after the finite path identity.
All original analytic composition identities pass first on the
dense parameter set and then throughout the domain. \(\square\)

For the actual component and stopped-prefix operators, use the
literal real integration atoms as \(S_n^t\), with their fixed
source selectors, constraints and input environment. LFR II
(1.73)--(1.75), pp.379--380, and the C05 common
positive-reference construction supply (MK.37) for that reference
family on the stated native charts.

If a physical output is reconstructed by a parameter-dependent map
\(\Psi_{n,\zeta}\), an insertion must be written as the actual
family \(F_{n,\zeta}(a)\) on those real atoms. The theorem applies
only when this family has its own bounded holomorphic extension
on the admitted chart. It does not assert that
\(f(\Psi_{n,\zeta}(a))\) is holomorphic for an arbitrary bounded
measurable physical-state function \(f\), or that a complex
reconstructed output has a dominated measure on the real physical
state space. The native claim is the composition of the verified
raw-reference kernel with its verified analytic test family.

The whole old canonical archive is already inside that literal
operator. Its internal depth is not counted as the number of
factors in a new finite operator word.

For the literal canonical component covered by LFR II
(1.73)--(1.74), the full unnormalized density change is bounded
by its actual small absolute perturbation \(\sigma\). This
separate comparison also keeps the mass. At a real admitted
center with \(\tau_{n,0}>0\), write
\[
 \tau_{n,\zeta}=\tau_{n,0}\,r_{n}(\zeta).
 \tag{MK.40a}
\]
Here \(r_n=\Pi_{n,0}e^{\sigma_{n,\zeta}}\). If
\(\sup|\sigma_{n,\zeta}|\le s<\log2\), then
\[
 |r_n-1|\le e^s-1,\qquad
 2-e^s\le |r_n|\le e^s.
 \tag{MK.40b}
\]
The source's absolute perturbation bound therefore supplies
fixed upper and lower bounds, uniformly on its working domain.
Together with (MK.5), this makes the complete mass a bounded
holomorphic probe family. Retain \(r_n\), \(\tau_{n,0}\) and the
normalized kernel moments jointly. Their products then pass by
the preceding algebra and Cauchy arguments. If a limiting real
mass is zero, the entire limiting family in (MK.40a) is zero,
so its complete weighted jet vanishes. No logarithm of a
zero-mass branch is taken.

Normalized domination (MK.37), or a phase bound after removing
an arbitrary parameter-dependent scalar, does not by itself
bound an unnormalized mass ratio. For any other stopped-prefix
family the mass-jet conclusion requires a separately verified
full unnormalized comparison. The normalized-kernel theorem
does not require that additional conclusion.

At a fixed finite source geometry/age truncation, use a common
strict native polydomain in the actual current and preparation
slots. Include all relevant finite charts and compact subdomains
in a countable exhaustion. The theorem applies simultaneously.
It does not assert (MK.37) for an arbitrary global complex
conditional law merely because its real normalization is positive.
Any such additional native family must have its own verified
common bound.

## 6. Physical state, labels and symmetries

### 6.1 The active raw state retains its genuine probability limit

At actual physical interface types, include a countable bounded
continuous coordinate embedding of each Polish local active-record
space from LC.1. Its laws are
tight under the actual Wilson/history marginals. Therefore the
projection of \(\bar\mu_\infty^t\) onto these coordinates is
supported on genuine local records, not on escape points of their
compactification.

For clarity, let \(j:S\to[-1,1]^{\mathbb N}\) be a continuous
embedding determined by these probes. Given \(\epsilon>0\), choose
a compact \(C\subset S\) with probability at least \(1-\epsilon\)
at every cutoff. The image \(j(C)\) is closed in the product
cube. Portmanteau gives limiting probability at least
\(1-\epsilon\) on that image. A sequence of compact sets carrying
probabilities at least \(1-2^{-r}\), made increasing by finite
unions, proves support on \(j(S)\). These sets need not exhaust
the entire Polish space.
The inverse embedding supplies a genuine raw record almost surely.

Exact coordinate restriction maps pass as identities of the
retained probe functions. The same one subsequence works for
all finite windows, native depths and fixed physical offsets.
This uses the actual LC tightness estimates, including their
restriction to literal local active footprints.

The additional archive/predictor coordinates need not be
measurable functions of this raw projection in the limit. That
is the information the enlarged state was constructed to keep.
Auxiliary canonical-query output laws do not automatically satisfy
LC.1. Their compact probe states have a raw-state identification
only when their own tightness estimate has been supplied.

### 6.2 Hard selectors

Each literal selector label is retained as a discrete coordinate.
An identity such as \(\chi_n^2=\chi_n\) passes, so its limiting
coordinate is still an indicator. Its role in every bounded
kernel expression passes with the actual joint law.

The identity
\(\chi=\mathbf1_{\{f\le t\}}\) for a recomputed limiting minimizer
test requires the separate convergence and boundary-null
condition of FK.19. It is not a continuous algebraic relation
in the underlying raw variables and is not supplied by this
theorem. The limiting construction is a labeled enlarged-state
construction until that identification is proved.

### 6.3 Physical symmetries and reflection positivity

Include the original physical Wilson state as a separate type,
with its actual marginal and its disintegration to the positive
history lift. Exact physical translations and reflection act
there by deterministic pullback operators. Add a countable
compatible family, together with inverses, to the invariant
algebra. A deterministic pullback preserves products and
conjugation; its extension therefore acts by a continuous map
of the compact state. Exact group identities, including identities
valid for all sufficiently fine lattices, pass on the zero fiber.

For translations one may use the dense compatible subgroup
\(\ell_0\mathbb Z[L^{-1}]^4\). This yields its exact action on the
bounded-probe state. Continuity of that action in an arbitrary
real displacement still requires the appropriate physical test
regularity; it is not inferred from density of the subgroup.

Reflection positivity is passed only on the original physical
positive-time cone. Choose countably many bounded physical
observables \(F_{n,j}\) with the actual finite-cutoff positive-time
support and reflection convention. Include their reflected
partners and all finite products. For every finite complex
vector \(z\), the original Wilson inequality is
\[
 \sum_{i,j}\bar z_i z_j
   \int (\Theta F_{n,i})F_{n,j}\,d\mu_n^{\rm W}\ge0.
 \tag{MK.41}
\]
Every matrix entry is a retained continuous probe expression,
so the same inequality holds in the limiting physical marginal.
This does not assert reflection positivity for a law conditioned
on an arbitrary history label or for every auxiliary archive
observable.

## 7. Why retaining the predictors is necessary

Here is a finite-state example of the obstruction addressed by
the construction. Let \(\xi=\pm1\) be equiprobable and set
\[
 X_{0,n}=\xi,\qquad X_{1,n}=\xi/n,\qquad X_{2,n}=\xi.
 \tag{MK.42}
\]
The finite-cutoff chain is Markov: its middle variable determines
the bit exactly. Its raw weak limit is \((\xi,0,\xi)\), which is
not Markov with the middle raw variable alone. In particular the
conditional past and future remain correlated after that variable
has become constant.

The bounded predictor
\[
 P_n[X_{2,n}\mid X_{1,n}]=nX_{1,n}=\xi
 \tag{MK.43}
\]
is one of the functions generated by Lemma MK.1. Its extra
coordinate survives and restores the actual conditional
information. This demonstrates why an argument based only on
tight raw-coordinate marginals could not prove Theorem MK.4.

Likewise, for the archived-mass example FK.17,
\[
 \tau_n(x)=a\left(1+\tfrac12\cos(2\pi n x)\right),
 \tag{MK.44}
\]
the compact state keeps the cosine coordinate and its square
jointly. The limiting average of \(\tau^2\) is
\(a^2(1+\tfrac18)\), as in the actual sequence, and is not replaced
by the square \(a^2\) of the averaged mass. No raw \(L^1\)
convergence is asserted or needed for this joint calculation.

These examples diagnose general weak-limit losses. They are not
claims that the actual Yang--Mills coefficients have those forms.

## 8. Source-specific closure and remaining obligations

### Theorem MK.6 — bounded mixed-source composition for the retained construction

Use one actual cofinal Wilson/source sequence at the retained
C01 construction scope, with the C05 theorem on its
stated native families. Prescribe countably many bounded actual
physical probes, bounded archived evaluations and exact finite
source-query diagrams. Retain complete canonical masses and
joint component operations.

Then one subsequence has:

1. compact metrizable enlarged interface states and actual
   probability marginals;
2. normalized source-free probability kernels with their exact
   finite composition identities;
3. the complete bounded microscopic source-jet transport,
   including higher vertices and outer conditional means;
4. jointly retained canonical masses, moments and complete
   mass-weighted coefficients, with zero-mass branches handled
   by the moment-cone theorem;
5. convergence of every fixed native derivative for every
   verified common-domain family covered by Theorem MK.5;
6. the actual local active-record marginals and the stated
   bounded physical symmetry/positivity identities.

**Proof.** The real normalized kernels and their correct marginals
are (MK.2) and the auxiliary query construction of Section 1.2.
Canonical masses have (MK.5), and complete grouping is (MK.6).
Apply Lemmas MK.1--MK.2 and Theorems MK.3--MK.4 to the countable
diagram. Equations (MK.34)--(MK.36) pass the complete finite
source jet. The moment-cone theorem treats its literal
mass-retaining coefficients. The supplied common native
comparison permits Theorem MK.5 precisely on those source
families. LC.1 identifies the active raw marginals, and Section
6.3 passes the physical identities. All extractions occur
inside one diagonal sequence. \(\square\)

This closes the enlarged-state alternative in FK Section 8,
item 3, for bounded source calculations. It also provides a
route around a common cross-cutoff raw density for these
measure-level calculations. It does not prove that the common
raw-density parametrization proposed in FK items 1--2 exists.

| Issue | Conclusion of this paper |
|---|---|
| Products of unrelated weak-* archive limits | Replaced by one invariant joint observable algebra before extraction. |
| Loss of normalized-kernel composition | Exact Feller extensions and finite path-law convergence prove composition on the enlarged state. |
| Very small component masses | Literal masses remain in complete expressions; the moment-cone theorem applies at zero mass. |
| Finite bounded source jets | Exact limiting transport and conditional logarithmic update. |
| Native finite jets | Proved for the actual uniform common-domain operator families, with their moving normalizers retained. |
| Raw-state autonomous canonical RG formula | Still requires identification of the extra predictor/archive coordinates with functions of that raw state. |
| Recomputed hard selectors | Still requires their actual boundary-null and convergence statements. |
| Unbounded physically normalized source hierarchy | Still requires joint uniform integrability, including the actual ER.7/F05 input. |
| Global Yang--Mills existence | Not concluded. |

The first three rows are mathematical closures of the specified
bounded composition obstruction. The last four rows identify the
remaining work without turning an enlarged-state limit into an
unproved physical field theory.
