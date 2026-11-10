# Birth-position dilution: exact geometry and the remaining weight comparison

Part of the [scalar-extraction analysis](scalar_extraction.md).

There are three separate statements in a birth-position argument: the number
of positions that produce the same fresh-reference class, an exchange identity
for their complete weights, and a centered microscopic marked estimate. This
note proves the rectangular position count, gives an admitted arithmetic
exception, records an exact first-innovation Gaussian exchange, and states a
quantitative positive-measure exchange lemma. It does not identify the full
old residual law with a Gaussian innovation law.

## 1. Source conventions and the complete reference class

CMP109, printed p.251, fixes `L` to be an odd integer greater than 11.
Thus `L=3` and `L=11` are unavailable examples. The literal condition does
allow `L=21`; no arithmetic nonresonance condition is printed there.
Taking a fixed odd `L>21` is a possible parameter choice when `L` has not
already been fixed numerically. It is a choice that must be recorded.

CMP119 pp.264--265 and p.269 gives the quiet map `S`: take the next-grid
cover and then add ten layers of that grid, followed by the actual
rectangular-hull convention. For a single rectangular chain the hull does
nothing. The source half-open cube convention fixes the floor and ceiling
rules below. Work away from torus wrapping; the compatible torus may be
chosen larger than the component.

Write

\[
 h=k-N,\quad k_0=k-N_0,\quad n=k_0+1,
 \qquad a_j=L^{j-k}MR_j,
 \qquad a_n=M.                                      \tag{BD.1}
\]

Here `a_j` is the physical side of a region cube. The source chooses `N>N0`.
On a constant-radius plateau `R_j=R`, put `a=a_h` and
`m=n-h=N-N0+1`, so `M=L^m a`.

For all ancestors of a fixed final component, the source geometry identity
CG.6a--CG.8 in [M04 Bounded Core Source Map](M04_Bounded_Core_Source_Map.md) is

\[
 S_0=C+B_8,\quad \Lambda=S_0\ominus B_4,
 \quad C+B_{10}=\Lambda+B_6,
 \quad Y=\mathscr D_k(\Lambda).                     \tag{BD.2}
\]

This is an exact erosion/dilation identity; no cancellation of arbitrary
erosion with dilation is needed. When `C` itself is a rectangle it reduces
to `Lambda=C+B4`.

The fresh-factor analysis FS.4 in
[M04 Fresh Support Class Cancellation](M04_Fresh_Support_Class_Cancellation.md) verifies that, after fixing the
fresh graph/orientation, source cutoff choice and representative conventions,
the fresh `h/H` depends on `Lambda`, `Y`, the retained shell and the fixed
scales. It does not use the old `T_h`, old mixed determining set or old
annular tree. These remain in the complete old mass. Consequently a change
of early birth position that preserves `Lambda` and `Y` preserves that
complete fresh class, with those choices fixed. The old weights need not be
equal. A free choice of the source cutoff `zeta_Y` must be fixed too, rather
than omitted from the class.

## 2. The exact one-dimensional endpoint formula

Start with an `h`-scale interval `[t,t+w)`, where `t,w` are multiples of
`a` and `0<w<=C_*a`. Apply the quiet maps through scale `k0`, and finally
take their next-grid cover `C` on mesh `M` without its new ten-layer padding.
The endpoints of that cover are

\[
 \ell_C=M\left\lfloor\frac{t-A}{M}\right\rfloor,
 \qquad r_C=M\left\lceil\frac{t+w+A}{M}\right\rceil,
                                                               \tag{BD.3}
\]

\[
 A=10\sum_{j=h+1}^{k_0}a_j
   =\frac{10}{L-1}M-\frac{10L}{L-1}a.              \tag{BD.4}
\]

**Proof.** At a quiet step the left endpoint is rounded down to the next
mesh and then decreased by ten next-mesh units; the right endpoint is
rounded up and increased by the same amount. The meshes are nested.
For `b` dividing `B`, and for a shift which is an integer multiple of `b`,
rounding to `b`, applying that shift, and then rounding to `B` equals
rounding the shifted original endpoint to `B`. Successive application
collapses all earlier roundings and gives (BD.3). The geometric sum gives
(BD.4). The same proof works for coordinate extrema of a union of all
ancestors: taking connected rectangular hulls changes none of its extrema.
Every ancestor that eventually joins this final component is included at
the start. \(\square\)

Fix a cover `[pM,(p+d)M)`, and put

\[
 y=\frac{t-A}{M}-p,\qquad
 \delta=\frac{w+2A}{M}
       =\frac{20}{L-1}
          +\left(\frac wa-\frac{20L}{L-1}\right)\frac aM.
                                                               \tag{BD.5}
\]

Exactly the allowed positions have

\[
 y\in[0,1)\cap(d-1-\delta,d-\delta].               \tag{BD.6}
\]

This gives an explicit count: intersect that interval with the affine
`a/M` lattice. The number differs from its length times `M/a` by at most
two. In four dimensions the counts multiply coordinatewise.

### Proposition BD.1 -- nonresonant rectangular translation count

On a constant-R plateau, suppose `L` is fixed and
`20/(L-1)` is not an integer. For every fixed upper bound `C_*` on the
birth side lengths in h-region cubes, all nonempty endpoint fibers in
(BD.6) have, for sufficiently large `M/a`, between
`c_L M/a` and `C_L M/a` h-grid positions. The four-dimensional count is
therefore comparable to `(M/a)^4`, uniformly over those rectangular shapes.

**Proof.** Let `theta` be the fractional part of `20/(L-1)` and let
`eta=min(theta,1-theta)>0`. The error in (BD.5) is `O_{L,C_*}(a/M)`.
For large `M/a`, the fractional part of `delta` stays in
`[eta/2,1-eta/2]`. The only possible cover widths have position intervals
of lengths `frac(delta)` and `1-frac(delta)`. Both are at least `eta/2`.
Use the lattice count following (BD.6). \(\square\)

For odd `L>11`, the only resonance of this formula is `L=21`.
The proposition is a geometric count, not a statement that the complete
mass of every position is comparable. The following extension handles
the actual radius variation without assuming it is monotone.

### Proposition BD.1a -- broad fibers for every literal prepared geometry

Choose a source-allowed fixed odd `L>=43`. On the admitted sufficiently
weak window `N=O(poly(log g_k^{-2}))`, every literal rectangular-chain
fresh class has at least

\[
 c_L(M/a_{h+1})^4                                    \tag{BD.6a}
\]

different whole-cluster h-birth positions giving the same prepared core
and the same fixed-rule fresh class. The statement is geometric; each
position can be realized by a bounded young R-only trial. It does not
claim equality of their masses or a translated-state map for arbitrary
old continuous payloads.

**Proof of the radius premise.** CMP119 p.255, (2.6), gives, for `j<k`,

\[
 \frac{g_k}{\sqrt{1+\beta' g_k^2(k-j)}}
       \le g_j\le(1+\beta_0)g_k .                  \tag{BD.6b}
\]

Consequently `x_j=log g_j^{-2}` lies in
`[x_k-2log(1+beta0), x_k+log(1+beta' g_k^2 N)]`.
This is a bounded interval, while `x_k` tends to infinity. Its fixed
power `x_j^r` has a ratio tending to one. Therefore the least powers of
`L` above these numbers take at most two adjacent values, denoted `R_-`
and `R_+=L R_-`. No monotonicity of the sequence is used.

**Reduction to one rectangle.** MW.1 and the literal inner preparation
rectangle put every h-ancestor into one actual rectangular component at
scale `s=h+1`. Its widths are at most `100 a_s`. Translate the entire
collection of h-ancestor rectangles by a vector in `a_s Z^4`. Every old
h shape remains on its own grid. The first cover, padding, joining and
hull commute with that shift, so the entire first merger pattern is
unchanged. From scale `s` onward there is one rectangle. The calculation
therefore starts with a translated interval of width `w<=100 a_s`.

Nested-grid endpoint collapse still gives (BD.3), now with

\[
 A=10\sum_{j=s+1}^{n-1}a_j,\qquad
 x:=\frac{2A}{M}
 =20\sum_{q=1}^{n-s-1}L^{-q}\frac{R_{n-q}}{R_n}.
                                                               \tag{BD.6c}
\]

For `n-s>=3` the following three cases exhaust every two-level radius
sequence, including an arbitrarily oscillating one:

\[
 \begin{array}{c|c}
 \text{radius data}&\text{interval containing }x\\ \hline
 R_n=R_+&[20/L^2,\ 20/(L-1)]\\
 R_n=R_-,\ R_{n-1}=R_-&[20/L,\ 20/L+20/(L-1)]\\
 R_n=R_-,\ R_{n-1}=R_+&20+[20/L^2,\ 20/(L-1)] .
 \end{array}                                       \tag{BD.6d}
\]

For the last case the first summand is exactly 20; the displayed lower
bound on its tail comes from `q=2`. For the other cases the first term
gives the lower bound. Extending each positive tail to an infinite
geometric series gives the upper bounds. Thus the distance to an integer
is at least the fixed positive number

\[
 \delta_L=\min\left\{\frac{20}{L^2},\
             1-\frac{20}{L}-\frac{20}{L-1}\right\}>0.
                                                               \tag{BD.6e}
\]

The initial width contributes `w/M<=100 L^{1-(n-s)}`, so the distance of
`(w+2A)/M` from an integer is at least `delta_L/2` for sufficiently large
age. Formula (BD.6) gives an interval of length at least
`(delta_L/2)M` for every nonempty final-cover fiber. Its `a_s`-grid count
is at least `c_L M/a_s` in every coordinate, proving (BD.6a).

**Eligibility and matching.** The physical consecutive mesh ratio is
one of `1,L,L^2`. If the first mesh is repeated, translation by `a_s`
commutes with that step exactly and preserves the original admitted
width. After the first genuine coarsening a width of at most 100 units
becomes at most `100/L+22<25` units. A repeated-mesh step adds at most
20 units. Repeated-mesh steps cannot occur consecutively when the radii
have only two adjacent values. All subsequent widths are consequently
below 100. The original h geometries have merely been shifted, so their
own size tests persist.

The same final M-cover gives the same prepared core and final Y by
(BD.2). All shifted descendants are inside that Y by physical nesting;
foreign components have their own disjoint final components and cannot
join this shifted chain. The source inner rectangle and its later
annular construction are preserved. Fixing the same orientation
reconstructs the corresponding old tree for each chain; it imposes no
new birth endpoint. The bounded-young-trial construction MW.2 realizes
each shifted h collection with the same fixed fresh factor. This proves
the assertion at its stated geometric scope. \(\square\)

The source hierarchy first fixes L and then chooses `M=L^m` sufficiently
large. The choice `L>=43` is available if no numerical L has previously
been specified. If L has already been fixed, its actual value must be used;
the next proposition explains why a silent nonresonance assumption would
be incorrect.

### Proposition BD.1b -- one thin R birth realizes every such fresh class

Under the hypotheses of BD.1a, every complete fixed-rule fresh class has
a young witness with just one bad `MR_h` covering cube. Thus its initial
large-field rectangle has side `3a_h`; a single strict R seed of RT.1
suffices. The statement concerns source admission and exact class matching,
not an asymptotically optimal Gaussian lower mass for that seed.

**Proof.** Set `s=h+1` and keep the same later radius sequence. Put
`x=2A/M` as in (BD.6c). By (BD.6e), and because all existing s-scale
widths are at most `100a_s`, the integer part of `x+w/M` equals the
integer part of `x` for every possible initial width, at sufficiently
large age. Hence every side of the desired final cover has one of the
two lengths

\[
 \{\lfloor x\rfloor+1,\ \lfloor x\rfloor+2\}\,M. \tag{BD.6f}
\]

A single bad covering cube at scale h has one-layer enlargement of side
`3a_h`. If `a_s>a_h`, put that three-cube rectangle wholly inside one
s-grid cube; this is possible because the ratio is `L` or `L^2`. Its
first quiet descendant has side `21a_s`. If the meshes are equal, its
first descendant has side `23a_s`. Fix one such initial placement and
then translate it by arbitrary `a_s` grid vectors. In either case the
new width divided by M is also smaller than the gap in (BD.6e). Its two
possible final cover lengths are exactly (BD.6f).

For each coordinate choose the cover length of the original class. The
corresponding position interval from (BD.6) has length at least `c_LM`,
and therefore contains an allowed `a_s`-grid translation. Choose those
four shifts independently. This gives the exact desired M-cover, hence
the original prepared core and final component by (BD.2). Its widths
remain below the source size ceiling throughout, by the same calculation
as in BD.1a. The R-only seed has strict actual Q/P margins and a positive
free-coordinate trial neighborhood by RT.1. The source test cube and
the covering cube are different: CMP119 (1.18) uses test cubes of side
`L^2 M_2 R_1` in the first fine units, while their region cover has side
`L M R_1`. The ratio is `M/(L M_2)`, chosen sufficiently large in the
fixed hierarchy. Choose one test cube whose full two-layer enlargement
lies strictly inside a single region-cover cube, and place the finite
free-coordinate seed stencil strictly inside that test cube. Every bad
R test whose enlarged footprint can meet that stencil is then inside
the same region-cover cube, and at least one such test is bad. The
nonlinear constraint correction changes only exceptional coordinates;
the R tests see the actual free coordinates. Thus the bad test set has
exactly one nonempty MR covering cube, rather than being identified
with one test cube. This is the strict placement mechanism of RT.1,
with an extra fixed test-layer collar if needed, allowed by
`M>>L M_2`. The identity-centered
preparation in RT.9b--RT.16 admits the remaining old variables. Fix the
same fresh graph, orientation and cutoff rule. FS.4 then gives exactly
the same complete fresh class. \(\square\)

This improves the geometric part of the lower trial at a permitted large
fixed L: its birth cost uses one seed, rather than the bounded number
needed when the entire earlier geometry is cloned. The complete numerator
still sums all actual old histories. In particular this lemma alone
does not replace that numerator by one-seed histories.

## 3. An admissible resonance pins the entire early ancestry

### Proposition BD.2 -- the L=21 narrow-core class

Let `L=21` and keep the constant-R plateau. In each coordinate take the
birth interval

\[
 I_h=\left[\frac M2-\frac{21}2a,
                 \frac M2+\frac{21}2a\right).
                                                               \tag{BD.7}
\]

Its endpoints belong to the h grid: `M/a=21^m` is odd. Its quiet
descendants before the final M-cover have width `21 a_j` and the same
center `M/2`. The final cover is the single cube

\[
 C=[0,M)^4,
 \qquad \Lambda=[-4M,5M)^4.                         \tag{BD.8}
\]

Every other h-scale ancestral union producing this same cover is contained
in the box `I_h^4`. In particular there are only a fixed number of h-region
cube positions in that class, independent of `N` and `M/a`.

**Proof.** Since `21 a_{j-1}=a_j`, the old interval is exactly one cube of
the next grid, centered at `M/2`. Adding ten layers gives width `21 a_j`.
This proves the indicated chain and its final one-cube cover. At and after
scale `n`, the subsequent intervals have width at most 22 region cubes;
they remain rectangular and satisfy the literal size ceiling 100.

For any competing ancestral union let `t_min,t_max` be its extrema in one
coordinate. Equation (BD.4) gives
`A=M/2-(21/2)a`. If its final cover is contained in `[0,M)`, (BD.3) forces

\[
 t_{\min}\ge A,\qquad t_{\max}\le M-A.              \tag{BD.9}
\]

The same assertion holds in every coordinate. It does not assume that
the old union had only one ancestor or remained unmerged. There are at
most a fixed number, bounded for example by `22^4`, of possible region
cube positions inside this box.

One can realize the stated birth rectangle by the actual R-only seeds
of RT.1, one in every cube of its one-layer erosion. Their number is a
fixed source constant, independent of coupling. The fixed-source seed
margins give positive-volume admission, and all later sets are the
displayed quiet rectangular chain. This is within the literal inner
rectangular-chain preparation examined in MW.1--MW.2.

Finally, if one specifies the same prepared core in (BD.8), rather than
the cover, (BD.2) gives `C+B8=[-8M,9M)^4`. A nonempty union of M-cubes
whose eight-layer enlargement is this 17-cube box must be the central
single cube in every coordinate. Thus the same conclusion holds for
the complete fresh class, not only for an artificially fixed cover.
\(\square\)

This is a rigorous failure of the assertion that `N>>N0` alone supplies
exponentially many same-class h-region positions. It does not prove that
M-04 is impossible: a permissible nonresonant fixed `L` avoids this
particular obstruction, and a different averaging mechanism could exist.
The `L=21` class still has polynomially many finer positions inside its
small h-region box; it lacks the exponential-in-age position gain.

Constant-R windows are compatible with arbitrarily weak couplings and
the admitted polynomial-logarithmic quiet depth: choose the coupling in
the interior of a rounded-radius plateau. Its change over such a depth
is much smaller than the distance to the plateau endpoints. No claim is
made for every coupling without that selection.

## 4. Counting positive young trials is not a numerator comparison

Suppose `J` distinct same-class histories each contain a positive trial
whose mass is at least `exp(-C K)`, where

\[
 K=P^2+R^6\log(1+R)+R^5\log g^{-1}.                 \tag{BD.10}
\]

Their disjoint history labels give the valid denominator lower bound

\[
 m_r\ge J e^{-C K}.                                 \tag{BD.11}
\]

Combining it with an unrelated upper bound for a pinned numerator gives
`e^{C K}/J`, not `C/J`. In this problem `log J=O(N)` while `P^2` is much
larger. The extra count does not cancel the rare-event exponent by itself.
A matching exchange or a relative comparison is necessary.

The native comparison RT.19 changes `(U,J)` at a fixed old integration
problem. It preserves its old hard support and history sum. It is not a
comparison of two different translated histories. At `(U,J)=(1,0)` the
old law still contains nonlinear positive `S` and the full old `T_h`; it
does not become a Gaussian merely because those native slots are flat.

## 5. The exact Gaussian first-innovation identity

There is nevertheless a precise special case where the first coarse grid
does not obstruct exchange. Work in the flat quadratic model, with the
actual first averaging constraint and source gauge convention. Let `y`
be the first coarse variable and let `z_0` be the independent first
fluctuation. Quadratic completion in the actual constraint chart gives

\[
 x=H_1y+C_0z_0,\qquad
 S_0(x)=\tfrac12z_0^{\mathsf T}K_0z_0+S_1(y),
 \qquad Q_1C_0=0.                                  \tag{BD.12}
\]

The cross term is zero by the constrained critical identity. The constant
linear-coordinate Jacobian cancels in normalized probabilities. One may
repeat the completion for `y` and its later coarse variables. After a
fixed final coarse constraint this gives a product of Gaussian innovation
laws. In particular `z_0` remains independent of all later innovations.
The first-step gap makes its normalized Gaussian nondegenerate; coarse
gauge directions are carried by the later variables and their prescribed
gauge factors, rather than counted as Wilson energy in `z_0`.

Let `T_s` be translation by an **entire first coarse lattice unit** (or
an integer vector of such units). It permutes the actual free coordinates,
the exceptional-bond convention and the block gauge contours. Thus

\[
 T_s^{\mathsf T}K_0T_s=K_0,
 \qquad T_s\ker Q_1=\ker Q_1.                       \tag{BD.13}
\]

Translation of `z_0` alone is an exact measure-preserving transformation
of the Gaussian innovation product, even though this small translation
need not preserve any later block partition. Those later variables have
not been translated.

For every first-innovation event `E`, every later-innovation event `G`
and every integrable translation-covariant first-innovation mark `A_x`,

\[
 \begin{split}
 (\gamma_0\otimes\gamma_+)(T_sE\times G)
     &=\gamma_0(E)\gamma_+(G),\\
 (\gamma_0\otimes\gamma_+)(A_x;T_sE\times G)
     &=\gamma_0(A_{x-s};E)\gamma_+(G).
 \end{split}                                       \tag{BD.14}
\]

These are exact finite-dimensional changes of variables, not approximate
translation invariance of the original constrained fine field.

A common global good event for a finite family of later Gaussian test
functionals can also be estimated directly. If each has variance at most
`Sigma^2`, their number is at most `exp(CN)`, and the required bounds are
`cP`, the union bound gives

\[
 \gamma_+(G^c)\le 2\exp\{CN-c'P^2\}.               \tag{BD.15}
\]

Independence makes this a **relative** bound after conditioning on any
first-innovation event. To identify it with the actual source quiet
restrictions, one must verify the common linear test family and that
membership in `G` forces those restrictions for every compared geometry.
The source's masked local minima, gauge choices and P/Q tests are not
automatically those global linear tests. Formula (BD.15) alone is not
that identification.

Likewise a literal translation of the entire fine field is generally
wrong. CMP98 (11) gives exact gauge covariance at the fixed coarse sites.
Take a small pure gauge `u` equal to identity at all those sites but not
at one translated site. Its fine field has coarse average identity; an
arbitrary sub-coarse translation need not. A proposed corrected
translation must keep its compensating map and Jacobian. The innovation
identity avoids this issue at the first quadratic step by using (BD.13).

## 6. A quantitative exchange lemma, including energy-weighted errors

Let a positive sector decomposition have positions `s` in a set `P` of
cardinality `J`, a common payload measure `rho`, and positive weights
`w_s(eta)`. Put

\[
 \mu(d\eta,s)=\frac{w_s(\eta)\rho(d\eta)}
                   {\sum_t\int w_t\,d\rho}.        \tag{BD.16}
\]

Choose one reference weight `w_*` and normalize `rho_*=w_*rho/rho(w_*)`.
Suppose a positive payload energy `E` has

\[
 \rho_* e^{cE/K}\le C_0,\qquad
 \rho_*(E e^{cE/K})\le C_0K,                        \tag{BD.17}
\]

and the exact pulled-back likelihoods obey

\[
 e^{-\epsilon E-\delta}\le w_s/w_*
                       \le e^{\epsilon E+\delta},
 \qquad \epsilon\le c/K.                           \tag{BD.18}
\]

Assume a nonnegative localized root satisfies
`A_x(s,eta)<=b E(eta) a_x(s)` with
`sum_s a_x(s)<=I`. Then

\[
 \mu A_x\le C bK e^{2\delta+C\epsilon K}\frac I J .
                                                               \tag{BD.19}
\]

**Proof.** The numerator is at most
`b I exp(delta) rho(w_*) rho_*(E exp(epsilon E))`.
The denominator is at least
`J exp(-delta) rho(w_*) rho_*(exp(-epsilon E))`.
Jensen bounds the last expectation below by
`exp(-epsilon rho_*E)`, and (BD.17) controls the numerator and `rho_*E`.
Cancel the common mass. \(\square\)

This lemma pays a small energy-dependent exchange error; it does not
require pointwise likelihoods bounded independently of every old state.
RT.20--RT.21 can supply a bound of the form (BD.17) for a correctly matched
reference sector. What remains to prove is the actual likelihood estimate
(BD.18) and an exhaustive, bounded-multiplicity sector decomposition.
A family of young trial subsets does not cover arbitrary earlier histories.

For a core-supported mark the h-region translation count in BD.1 only
gives `(a/M)^4=(R_h L^{h-k})^4`. It leaves the displayed polynomial `R_h^4`.
Finer first-coarse-lattice translations of a localized first-step birth
can in principle add the internal positions within its region cube. They
must preserve the literal P/Q/R test alternatives. They have not been
inserted into BD.19 merely by counting points in an MR cube.

## 7. What the new relative marginal theorem supplies

[first step relative marginal](first_step_relative_marginal.md) proves, for the actual first-step
normal-form product law and its Gaussian law with the same cutoff,

\[
 \left|\log\frac{p_{1,D}(u)}{p_{0,D}(u)}\right|
       \le C(gP^3+g^2P^2)|D|.                      \tag{BD.20}
\]

It uses the actual positive gap, the full W gradient/Hessian rows and a
weighted covariance estimate on the convex product support. It gives a
relative comparison for any equally selected event measurable in D,
without dividing an absolute error by its rare probability. For a birth
neighborhood with `|D|=O(R^4)`, its exponent is `o(1)`.

This proves the missing kind of local comparison at the original first
step. It is not yet an exchange theorem for the completed residual class.
The Gaussian reference in (BD.20) carries the same cutoff; it cannot be
replaced by the untruncated independent innovation law in (BD.14) without
controlling the intervening cutoff event. Extra nonlinear selectors must
be kept as the same event or compared by a separate boundary calculation.

There are also two genuine microscopic bookkeeping issues.

First, a native current-scale plaquette is not the already transported
microscopic scalar. A surviving bare mark still carries its original
`h_0^{-4}` coefficient; no dictionary in the source replaces it with
`h_h^{-4}` just because its old state is stored at scale h. A translation
by h-region cubes therefore only supplies the full physical improvement
when the incoming h-scale marked budget has independently been established,
or when the corresponding finer-history averaging has also been proved.
For the first reset `h=1`, the first-innovation route addresses this issue
directly; for arbitrary `T_h` it does not.

Second, the scalar has a thermal identity contribution. A bound on an
uncentered local energy gives a nonvanishing thermal value at every
position. The dilution estimate must be applied to the defect from the
actual transported identity coefficient, together with its scalar part
and separate direct/kernel records. The first-clean coefficient LC.57--LC.59
does not itself pay an additional rare local P^2 factor. Marks generated
by the preliminary annular integrations need their own exact transport;
they are not all supported in the remaining prepared core.

## 8. Current proof boundary

The following are established here: the exact endpoint/position count,
the admitted `L=21` exception to automatic geometric dilution, the exact
Gaussian first-innovation exchange, the energy-weighted positive exchange
lemma, and the first-step relative local comparison in the companion note.

To finish the proposed first-reset route one must identify an exhaustive
same-class decomposition of the actual h=1 old law, use actual source
reconstruction to match its quiet restrictions to the independent-innovation
calculation or a controlled alternative, and transport the centered scalar
through the removed annuli. For arbitrary older histories the same task
also includes the surviving pre-h microscopic normalization and the genuine
old-weight exchange. None of these obligations is removed by a large
denominator count alone.

### Mathematical sources

- CMP109 (1987), p.251: fixed odd L>11 and nested lattice conventions.
- CMP98 (1985), pp.17--20, (1)--(15): blocks, exact averaging and gauge
  covariance; the fixed coarse sites matter for a translation.
- CMP119 (1988), pp.264--269: exact quiet region cover/padding rules and
  the R birth. Its original density includes all Haar/coarea factors.
- LFR I (1989), pp.179--180, 192--201: N0, the prepared rectangle and
  annular preparation; fresh versus old factors are examined in FS.4.
- LFR II (1989), pp.379--380: relative native continuation; it does not
  compare translated old geometries.
- [residual merger witness](residual_merger_witness.md), MW.1--MW.2, and
  [residual trial mass](residual_trial_mass.md), RT.17--RT.21: bounded young same-class trial
  and old-energy reserve, with their actual literal-chain scope.
