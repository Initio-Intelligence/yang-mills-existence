# First ordinary step: an active geometry pair and a strong-carrier lower bound

This note concerns the actual first ordinary Wilson RG conditional, before
any large-field replacement. Both retained data used below have positive
active neighborhoods. The argument does not use an inactive extension,
an eliminated-energy regulator, a substitute Gaussian law, or a reset
posterior. The Gaussian calculation is a uniform weak-coupling limit of
the complete finite first-step conditional.

The conclusion has an essential representation scope: the declared
source ledger of Annex W §2.2, with the **deterministic construction
footprints** required by Annex Y (M.1). That ledger explicitly constructs
its geometric domains from the primitive selectors. The conclusion
does not apply without further argument to a changed state architecture
which declares derived activation masks to be independent local
primitive coordinates. Section 7 distinguishes these alternatives.

## 1. The literal source operation

Use CMP119, printed pp.247–253, (1.8)–(1.26), at its first step. Choose
all initial plaquette and approximate-fluctuation alternatives good, so
that Ω₁ is the whole torus. Fix the coarse field V₁=1. The global
background U₁ and every local background U₁,□ are then identically one.

Let

\[
 P=\delta _0/g_0.
 \tag{GO.1}
\]

This is a fixed source logarithmic power as g₀ tends to zero. The first
free-field cutoff is unambiguous: (1.18) uses |A₀|<P. It is
not the later printed normalization mismatch discussed in
[M04 Quiet Selector Catalog](M04_Quiet_Selector_Catalog.md). The approximate Q test in (1.19) is
starred and has physical radius 2δ₀. The actual independent coordinates
are all bonds except b₀(c), by (1.9) and the paragraph immediately before
(1.15). The exact constraint reconstruction is

\[
 U(A)=\exp\{i[g_0CA-hD(g_0CA)]\},\qquad QCA=0.
 \tag{GO.2}
\]

Here C differs from the inclusion of the independent entries only on the
exceptional bonds b₀(c). Its stencil, and the nonlinear exceptional solve,
have fixed L-dependent size. These are the literal coarse-average
constraints; no linearized constraint replaces them in the measure.

Let R′₁ be the union of the LMR₁ cubes intersecting R₁. Printed p.251,
(1.20), gives, because Ω₁ is full,

\[
 \Lambda _1=(R'_1{}^{\sim})^c.
 \tag{GO.3}
\]

The tilde adds one layer of these cubes. Small complement components
are subsequently replaced by their smallest rectangular hull. The same
page states explicitly that the conditional integration is with respect
to A restricted to Λ₁. Thus A on Λ₁ᶜ is retained, rather than integrated
in this regular conditional. With the independent-bond incidence
convention understood, put I=Λ₁*.

The localization (1.21)–(1.22) does not alter this example. Both of its
reference minima are exactly one when V₁=1. Consequently H₁,Λ=0,
the coordinate change (1.22) is the identity, and its Jacobian is one,
including at the bad retained witnesses. This is an exact source
identity, not an exponentially small approximation.

## 2. Two actual admitted histories

Work first in coarse current units h=La. An MR₁ cube then has side
MR₁. Take any admissible torus with current side at least CMR₁, where
C is a sufficiently large fixed power of L. There is room to keep the
following rectangles away from their periodic translates. The choice
of side exactly CMR₁ gives the simplest finite-volume comparison in
Section 3. Section 3.1 supplies the same conclusion uniformly on an
arbitrarily larger compatible physical/cofinal torus.

Choose adjacent MR₁ cubes C₁,C₂. The two R patterns have covering sets

\[
 R'_{\rm s}=C_1,
 \qquad R'_{\rm l}=C_1\cup C_2.
 \tag{GO.4}
\]

Their retained holes are

\[
 Y_{\rm s}=C_1^{+1},
 \qquad Y_{\rm l}=(C_1\cup C_2)^{+1},
 \qquad Y_{\rm s}\subset Y_{\rm l}.
 \tag{GO.5}
\]

They are already rectangles, with side lengths respectively
(3,3,3,3) and (4,3,3,3) in MR₁ units after orienting the first coordinate
along C₁,C₂. The source hull operation changes neither one. In
particular their diameters meet the stated 100MR₁ small-component test.

Here is an exact strict realization of (GO.4) on the source's actual
**smoothed gauge** branch. Choose one fine vertex x₀ strictly inside
an L block, away from its center and its faces, deep inside C₁. Put
u(x₀)=exp(i3δ₀T/2) for a fixed unit Lie-algebra generator T and
u(x)=1 elsewhere. Gauge-transform the identity field by u. Exact
endpoint covariance of the source averaging map, CMP98 (11), gives
V₁=1 because u is identity at every block center.

The only nonidentity fine links are the eight incident links at x₀,
with angles ±3δ₀T/2. They are all nonexceptional. Thus the actual
independent coordinates are ±3PT/2 there and zero elsewhere. The
linearized average of this center-fixed gradient is zero, and every
exceptional link is identity. The unique local nonlinear constraint
solve in (GO.2) therefore reproduces this exact pure-gauge field; no
approximate averaging identity is used.

Every physical plaquette is exactly identity. Every actual
center-to-vertex contour is identity except the one at x₀, whose
angle is 3δ₀/2<ε₀ by the source's fixed A₀≫A₁ hierarchy. Their
group mean is the same endpoint gauge matrix, because all those
contours agree for a pure gauge. Consequently the initial plaquette
and smoothed-gauge selectors are strictly good. The starred Q test
sees exactly exp(ig₀A(b)) and has maximal deviation less than 2δ₀.
The R test fails strictly since max|A|=3P/2.

This uses the soft gauge factor of CMP119 (1.5)–(1.16), not a
configuration forbidden by a hard axial slice. The fact that U₁ can
be characterized in an axial representative does not remove the
ordinary soft-gauge integration variables. The physical variance
direction in Section 4 is separate from this geometrical gauge seed.

Alternatively, one independent nonexceptional entry 3PT/2 is enough.
The exact C/hD solve leaves its starred Q value unchanged and
produces full physical links bounded by C_Lδ₀; the fixed source
A₀≫C_LA₁ choice makes its P/soft-gauge tests good. The pure-gauge
seed above avoids needing this last quantitative allowance for the
seed itself. For the integrated entries |A|<P the ordinary source
redundancy argument already supplies the required P/soft-gauge
admission, including the fixed-L boundary stencils.

The actual bad R-test cubes are those whose enlarged test footprints
see this seed. Place it farther from the boundary of C₁ than four
elementary test-cube widths plus the fixed constraint stencil. The
source permits M≫LM₂, so the center of C₁ has this margin. All these
bad test cubes then have precisely the single coarse cover C₁. Put all
other retained free coordinates equal to zero. This gives the small-hole
datum y_s. For y_l add an identical seed deep inside C₂. No other
coordinate value changes. The cover is now exactly C₁∪C₂.

Notice that C₂ itself lies inside Y_s. Thus the extra seed coordinate is
retained in **both** states. The newly retained outer strip

\[
 B=I_s\setminus I_l,
 \qquad I_s=Y_s^c{}^*,\quad I_l=Y_l^c{}^*,
 \tag{GO.6}
\]

has value zero in the large-hole state and padded value zero in the
small-hole state. All current compact coordinates are identity in both
states. Every discrete source choice other than the induced R geometry
is the same. Every changed nonzero numerical coordinate is a distance
at least cMR₁ from the outer face of Y_l adjacent to C₂.

All selectors used to define these retained data have strict margins.
Small open neighborhoods of each datum, in its own retained sector,
therefore have positive density and a strictly positive regular
normalizer. The two data are active, rather than reference values on
inactive fibers. The R pattern can include several elementary bad test
cubes around a seed; the argument uses its actual MR cover, not an
invented single test.

The first R selectors on I_s or I_l are exactly their good product
cutoffs. Their bad selectors are already satisfied by the retained
seeds, and their remaining starred Q factors are retained-only and
strictly good. The source redundancy argument after (1.19), or C7.1
applied to this first step, removes no factor which depends on the
integrated variables besides these literal good cutoffs.

## 3. Uniform reduction of the actual conditional to its flat Gaussian

Write K for the flat first primitive precision in the genuine
independent free coordinates. Formula (1.16) and the underlying
propagator estimates give fixed constants

\[
 0<k_*I\le K\le K_*I.
 \tag{GO.7}
\]

K has fixed finite range. This also follows directly from the Wilson
curl quadratic, the block-local smoothed-gauge quadratic, and the
fixed-L C embedding. The source uniform upper kernel estimate is
CMP99, printed p.428 after (3.158); the gap is the ordinary constrained
regular precision gap. A principal restriction inherits both bounds.

Every nonzero retained seed is separated from its integration boundary
by MR₁ minus a fixed stencil. All retained entries in the finite-range
collar of that boundary vanish. Hence, exactly,

\[
 K_{I I^c}A_{I^c}=0
 \tag{GO.8}
\]

in both histories. Their Gaussian conditional means are zero. No
exponentially small mean estimate or inverse rare-event probability is
needed.

There is also no hidden seed dependence in the primitive nonlinear
density on I. At V₁=1, the Wilson terms, smoothed-gauge terms, Haar
factors, exceptional constraint maps and their Jacobians are fixed-range
functions of the free variables. The boundary relocation is the exact
identity already noted. The retained seed terms are separated from I
by a zero collar and therefore multiply numerator and denominator by
the same retained-only factor.

Let γ_I be the centered Gaussian with precision K_II and let C_P be
the actual product |A(b)|<P. Undoing the first regular integration
identities, including all coarea and gauge factors, gives the actual
conditional in the form

\[
 \nu_I(dA)=
 \frac{e^{-W_I(A)}1_{C_P}(A)\,\gamma_I(dA)}
      {\gamma_I(e^{-W_I}1_{C_P})}.
 \tag{GO.9}
\]

The normalization constants which only depend on I cancel in this
conditional ratio. W_I includes every nonquadratic primitive term; it
is not just the Wilson remainder. Finite-range analyticity of (GO.2),
the Wilson and smoothed-gauge Taylor expansions, and the Haar/coarea
Taylor expansions give

\[
 \|W_I\|_\infty\le Cg_0P^3D,
 \qquad D\le C(L,M)R_1^4
 \quad\hbox{on the optional torus of side }CMR_1.
 \tag{GO.10}
\]

The harmless O(g₀P) or O(g₀²P²) Jacobian terms fit this bound for
P≥1. This elementary finite-volume estimate is sufficient here; no
completed E/B response estimate is assumed. All physical fields in
(GO.9) are in the first admitted regular chart because g₀P→0.

The uniform gap in (GO.7) also gives

\[
 \gamma_I(C_P^c)\le CD e^{-cP^2}.
 \tag{GO.11}
\]

Each source Lie-algebra block has fixed dimension. Its Gaussian norm
tail, followed by a union bound over D blocks, proves (GO.11).

For a scalar whose fixed stencil stays in a fixed-L neighborhood of the
chosen interface, its dimensionless value is O(P²) on C_P. Its Taylor
remainder is O(g₀P³). Equations (GO.9)–(GO.11) consequently imply a
uniform error bounded by

\[
 \eta(g_0)\le
 Cg_0P^5R_1^4+C\,\operatorname{poly}(P,R_1)e^{-cP^2}
 \longrightarrow0.
 \tag{GO.12}
\]

Here and below the Wilson/source dictionary is the specified B-01 one,
g₀⁻²=Nβ₀. In particular β₀g₀²=1/N is a fixed positive constant.
The usual first-step comparison of g₁ and g₀ makes P and R₁ powers
of log(g₀⁻²), up to fixed factors. The source specifies r≥2 and
R₁≥(log g₁⁻²)^r. Thus both terms in (GO.12) tend to zero. This
passes from the actual Wilson conditional to the Gaussian calculation
uniformly even though the torus and the holes grow with R₁.

### 3.1 The same transfer on an arbitrary larger physical torus

There is no need to restrict the theorem to that optional torus size.
The first-step relative marginal theorem RMg.18, in
[first step relative marginal](first_step_relative_marginal.md), applies after arbitrary pinning and
principal compression. The retained values here are at most 3P/2 and
lie in its fixed larger analytic tube. Its complete first-step
derivative rows are unchanged up to fixed constants. The Gaussian
linear force is exactly zero by (GO.8). For the fixed number of free
coordinates D_x on which one root depends, it gives

\[
 e^{-C g_0P^3|D_x|}
 \le\frac{d(\nu_I)_{D_x}}
          {d(\gamma_I(\cdot\mid C_P))_{D_x}}
 \le e^{C g_0P^3|D_x|}.
 \tag{GO.12a}
\]

This comparison retains the complete product cutoff on both sides.
There is no denominator equal to a rare all-good probability.

Here is a volume-uniform cutoff-removal argument for the local quadratic
root. Let f(z)=z*Az, where A is supported on a fixed finite stencil.
For the centered Gaussian γ with precision K_II, solve its quadratic
Ornstein–Uhlenbeck Poisson equation by

\[
 H=\int_0^\infty e^{-tK_{II}}A e^{-tK_{II}}dt,
 \qquad u(z)=-z^*Hz,
 \qquad (\Delta-K_{II}z\cdot\nabla)u=f-\gamma f.
 \tag{GO.12b}
\]

The gap and finite range give a conjugated semigroup estimate
|e^{-tK_II}_{ij}|≤C e^{-c d(i,j)}e^{-k_*t/2}, uniformly for every
principal domain. Hence

\[
 \sum_{i,j}\|H_{ij}\|\le C_A
 \tag{GO.12c}
\]

independently of the volume and the holes. This is also the hypothesis
used in the specified Annex K, Theorem 5.1, cutoff-removal argument.

For clarity the required boundary estimate can be checked directly.
The one-coordinate marginal of the Gaussian restricted to C_P has
unnormalized density

\[
 1_{\{|u|<P\}}e^{-u^*S_i u/2}I_i(m_i(u)),
 \qquad k_*I\le S_i\le K_*I.
 \tag{GO.12d}
\]

Its outside cutoff is a centered symmetric convex product. The exact
Gaussian completion obeys I_i(m)≤I_i(0), while symmetry and Jensen
give I_i(m)≥e^{-m*K_{OO}m/2}I_i(0). Moreover
m_i(u)*K_OO m_i(u)≤K_*|u|². Integrating over a fixed unit ball in u
therefore bounds the normalized marginal density by Ce^{-c|u|²},
with constants independent of every outside coordinate. The upper
completion inequality is the convex symmetric Gaussian inequality
proved in [first schur tilt trial](first_schur_tilt_trial.md) §2; its cutoff is retained exactly.

On a fixed source norm ball the boundary has |u|≥cP and surface area
O(P^{d_G-1}). Integration by parts in (GO.12b) over the product cutoff,
using (GO.12c), consequently gives

\[
 |\gamma(f\mid C_P)-\gamma f|
 \le C_A P^{d_G}e^{-cP^2}.
 \tag{GO.12e}
\]

Indeed the normal derivative of u on coordinate face i is bounded by
CP Σ_j||H_ij||, and the integrated normalized density of that face
has the preceding exponential bound. Summing these absolute boundary
fluxes proves (GO.12e); it never bounds a global failure probability.
Convex smooth approximation gives the same result for a nonsmooth
source norm ball.

Finally the Gaussian law on C_P is centered and has covariance at most
K_II⁻¹, by the convex Gaussian covariance inequality. Its local
nonnegative quadratic root expectation is uniformly bounded. Combine
(GO.12a), (GO.12e), and the O(g₀P³) local Wilson Taylor error. The
local actual-to-full-Gaussian scalar error tends to zero uniformly in
the torus volume. This proves the transfer used in Section 4 on the
actual large physical/cofinal tori as well as on the short illustrative
torus. No relation between a and g₀, or choice of a physical F-01
normalization window, was changed.

## 4. A strictly positive actual scalar gap

Set I=I_l and J=I_s=I⊔B. All Gaussian covariances in this section are
padded to the common independent-coordinate space J. Block inversion
gives the exact identity

\[
 K_{JJ}^{-1}-\operatorname{diag}(K_{II}^{-1},0)
 =R S_B^{-1}R^*,
 \quad
 R=\binom{-K_{II}^{-1}K_{IB}}{I_B},
 \quad
 S_B=K_{BB}-K_{BI}K_{II}^{-1}K_{IB}.
 \tag{GO.13}
\]

The left side is positive semidefinite. Moreover
S_B≤K_BB≤K_*I, so S_B⁻¹≥K_*⁻¹I. For every physical linearized
plaquette map D_pC, its variance in J is at least its variance in I.
This remains true for plaquettes crossing the boundary; one must use
the padded covariance difference, not just its I×I block.

Choose adjacent fine L blocks A and B₀ on the outer face of Y_l, with
A in I and B₀ in B. Choose one tangential fine bond on the B₀-side
face, with a neighboring tangential plaquette wholly inside B₀. Put a
unit Lie-algebra generator on that one actual independent coordinate,
and zero on the other B coordinates. Denote this vector by b, so
||b||=1. Every edge of the selected tangential plaquette is internal
to the block and hence nonexceptional. No additional condition Qb=0
is imposed on the independent-coordinate vector; the actual C map
already solves all the linearized averaging constraints.

The inner-face curl is nonzero:

\[
 \|d_{\rm face}b\|\ge c_L>0.
 \tag{GO.14}
\]

For this single-bond choice c_L can be taken to be a fixed generator
normalization constant. The source L>11 supplies ample room; the local
construction only needs an interior tangential plaquette. It requires
no rank count for Q and no separate physical-gauge decomposition.

Consider the full cochain CRb. Every tangential bond on the B₀-side
face still has its prescribed value b: R leaves B coordinates fixed,
and C changes only the exceptional bonds. The B-side face curl is
therefore exactly d_face b. Each such tangential plaquette is one face
of a fine three-dimensional cube crossing the A/B₀ interface. The
linear lattice Bianchi identity says its curl equals the signed sum of
the curls of the other five faces. Each of those five faces has an
A-side vertex. Cauchy–Schwarz and (GO.14) give

\[
 \sum_{p\in\mathcal P_A}|D_pCRb|^2\ge c_L'>0,
 \tag{GO.15}
\]

where P_A is a fixed finite set of plaquettes with A-side vertices.
All constants are independent of R₁ and of the remote seeds.

Combining (GO.13) and (GO.15) shows that the sum of their physical
plaquette variance increments is at least c_L'/K_*.

The exact F-01 scalar is

\[
 \sigma_a(x)=\frac{2}{\sqrt6}\,
 \frac1{4a^4}
 \sum_{\mu<\nu}\sum_{\epsilon,\epsilon'=\pm1}
 s(P_{\epsilon e_\mu,\epsilon'e_\nu}(x)).
 \tag{GO.16}
\]

Every coefficient in this sum is positive. Every p∈P_A occurs in the
stencil of an A-side vertex. Choose the fixed finite set X_A of these
vertices. All the other plaquette variance increments are nonnegative
by (GO.13). The Gaussian sum of the scalar increments over X_A is
therefore bounded below by a fixed c>0 in units a⁻⁴.

By the actual conditional comparison (GO.12), for all sufficiently
small g₀ at least one x∈X_A satisfies

\[
 a^4\left|
 Q_{\rm s}(\beta_0\sigma_a(x))(y_s)
 -Q_{\rm l}(\beta_0\sigma_a(x))(y_l)
 \right|\ge c_0>0.
 \tag{GO.17}
\]

The root x belongs to the regular interior in both histories. Its
fixed microscopic scalar stencil can cross the integration interface.
Neither the M-04 statement nor M.2/M.12 imposes an MR-depth condition or
requires that this entire stencil lie inside Λ₁. That feature of the
scope is used here. For a family required to remain MR-deep in Λ₁,
(GO.17) would be a different question.

Centering the microscopic scalar subtracts the same number at the two
retained data, so (GO.17) is unchanged for the actual compact-centered
M.13 scalar. Multiplying it by its fixed incoming F-01 coefficient
multiplies both this gap and its input budget by the same factor.

## 5. The native regulator at the two data

The output first-step native list consists of V₁ and the retained
ordinary free coordinates A₀ on the hole. There is no older raw
determining field because Ω₁ is full. Both V₁ fields are identity.
There are at most 4d nonzero independent free coordinates, in the two
strict seeds, and each is O(P). All padded coordinates have their fixed zero
or identity values.

It follows for every carrier X that

\[
 \widehat R_{h,X}(y_s)+\widehat R_{h,X}(y_l)
 \le C_L(1+P^2),\qquad h=La.
 \tag{GO.18}
\]

This includes the shifted regulator (M.6), not only its unshifted part.
A unit native Euclidean perturbation changes one seed/zero coordinate
by at most one. A normalized compact-link perturbation of V₁ affects
only finitely many native plaquettes and contributes O(1) to β₁s.
The external scale and coupling labels are fixed as required by M.3.
A discrete change does not assign new numerical values to the padded
coordinates; activating a zero or identity coordinate does not create
energy. No unobservable eliminated microscopic Wilson energy is put
in (GO.18).

## 6. A supported-carrier lower-bound lemma

Let f=Σ_X f_X be any supported carrier representation with one
insertion anchor x. Suppose two ambient data y,z agree on every
coordinate whose full defining footprint lies in the current ball
B_h(x,r). Suppose also that their shifted regulators are bounded by K
for every X. For every carrier X contained in this ball, support gives
f_X(y)=f_X(z). Every remaining carrier contains x and a block outside
the ball, so its tree length is at least r−1.

The pointwise value part of (M.11) therefore gives, for source order one,

\[
 h^4|f(y)-f(z)|
 \le 2K e^{-\kappa(r-1)}
       \sum_Xw_h(X)v_{h,1,X}(f_X).
 \tag{GO.19}
\]

Adding direct and kernel-current costs only increases the norm. Thus

\[
 \|\mathbf f\|_{h,\kappa}
 \ge \frac{h^4|f(y)-f(z)|}{2K}
                       e^{\kappa(r-1)}.
 \tag{GO.20}
\]

The proof uses absolute activity costs and permits arbitrarily many
tags on the same carrier. It cannot be defeated by cancellation among
different activities or by a different supported decomposition.
An array whose set of active tags changes with the history must first
be placed on the common padded ambient index set. Its activation
indicator is then part of the coefficient and has its actual footprint;
an unrecorded sector-dependent index convention is not a supported
M.1–M.12 representation.

At the two data of Section 2, all differing primitive selector/raw
coordinates are a distance ≥cMR₁ from x. Under the deterministic
footprint rule of Section 7, every changed derived coordinate also has
a defining footprint reaching those remote data. Hence (GO.19) applies
with r=cMR₁ and K=C(1+P²). Equations (GO.17)–(GO.20) yield

\[
 \boxed{
 \|\mathbf QF_x\|_{La,\kappa}
 \ge cL^4\,\frac{e^{c'\kappa MR_1}}{1+P^2}.
 }
 \tag{GO.21}
\]

This lower bound already comes from the value term. No need to divide
by a small continuous increment arises.

The microscopic input has a fixed local carrier and, by compactness
alone, satisfies

\[
 \|\mathbf F_x\|_{a,\kappa}\le C_N(1+\beta_0).
 \tag{GO.22}
\]

Indeed the centered scalar value is O(β₀a⁻⁴), its normalized link
increments are at most that size, and all its finite stencil and
direction counts are fixed. The uniform compact reserve of M.14 would
improve (GO.22), but is unnecessary. Since r≥2 and
R₁≳(log β₀)^r, the ratio of (GO.21) to (GO.22) diverges. Thus even
allowing this much larger finite incoming budget does not give a
scale-uniform linear one-step transport bound with the literal strong
carrier weight.

## 7. What the footprint statement means

Annex Y (M.1) states:

> A coordinate whose definition uses several blocks is assigned its full
> dependency footprint, even if it is stored at one block. A carrier
> must contain that footprint.

It further distinguishes storage from dependency and requires an actual
locality identity before reducing a global history flag's footprint.
The B-01/H-01 selector inventory explicitly lists Ω_j,Λ_j,S_j as
**obtained from the preceding labels and their specified cube layers**;
it cites (1.10), (1.20) and (3.20). C7 retains this live source geometry
while proving fixed product support within a fixed sector. These facts
are relevant to a deterministic construction footprint, rather than to
decay of stochastic correlations.

For example the bit 1{b⊂Λ₁} near the extended face in this construction
changes when the R seed is added deep inside C₂. Every primitive raw
and selector datum in a ball of radius cMR₁ around that bit is the same
at y_s and y_l. Consequently no exact function of those local primitive
data can equal that bit on both admitted histories. This is an explicit
failure of a proposed local identity. Splitting Λ₁ into membership bits
and storing one at every block does not change that fact or its defining
footprint under M.1. The same observation applies to a derived active
rank flag for A₀. The actual padded A₀ values on the newly retained
strip are zero in both states, so they do not distinguish the pair.

By contrast, a **different interface** could choose a mask field m_b as
an independent primitive coordinate at each current block, with the
joint probability law imposing m=1_Λ. Its correlation with remote R
tests would not by itself make its coordinate footprint nonlocal. Such
an interface deliberately discards the source construction footprint
when defining support. With that convention the two states differ in
a local mask coordinate next to x, and (GO.19)'s premise fails.

This is not an off-support continuation of the same norm. It changes
which supported functions may be placed on a small carrier, and hence
changes the strong carrier interface itself. The proof here does not
rule out a uniform theorem for that altered interface. It does require
that such a change be explicit and that the new local-mask current,
rank-change, reconstruction and downstream estimates be proved.

Thus (GO.21) applies specifically to the declared Annex W §2.2 source
history architecture with the literal M.1 deterministic-definition
rule. Its inventory identifies the masks as derived domains, not as
independent local mask primitives. Replacing that inventory and its
support rule by the alternative above is an explicit amended interface.
It is not a missing Gaussian estimate or an automatic freedom to
change the specified norm.

## 8. Scalar and identity extraction do not remove this gap

The M-04 statement and its source analysis ask for an expansion of the same
QF_x in the fixed incoming F-01 basis, into a current scalar, an identity
term, and a localized remainder. F-01 (F.30)–(F.35) specifies numerical
coefficients from the compact law; they do not depend on an individual
retained RG history. A fixed scalar coefficient and fixed
identity coefficient cannot remove (GO.17): the coarse field V₁ is the
same identity field in both data, so every fixed coarse scalar, centered
or uncentered, has the same value there. The identity also has the same
value. Therefore the subtracted remainder has precisely the same pair
gap and obeys the same lower bound (GO.21).

Allowing the coefficients themselves to depend on the history does not
make that dependence free. Such a coefficient is a marked response
function of the retained state. Its full construction footprint and its
direct/kernel current belong to the M.10–M.12 representation. Moving
the pair gap into a history-dependent coefficient moves the same cost
to that coefficient. Declaring it to be an uncharged scalar number
would no longer be the specified supported extraction.

## 9. Versions and the precise conclusion

The points V₁=1 and the specified zero retained fields can be null as
singletons, but they are interior points of positive-density active
sectors. Their actual conditional ratios are continuous there: the
domain is the fixed finite product C_P, the complete density is smooth,
and the normalizer is strictly positive. Any output version with finite
M.03 divided-current norm is continuous in each continuous coordinate
on such a finite compact neighborhood. It agrees everywhere on the
neighborhood with the continuous conditional ratio if it agrees almost
everywhere. Thus changing a version on these isolated retained data
does not evade the lower bound while keeping the current norm finite.

The result is an actual first-step test of the strong carrier interface.
Under its literal deterministic construction-footprint rule, uniform
M-04 transport, including its fixed scalar/identity remainder, fails
already on the two active first-step histories above. The effect is a
change in a local fluctuation variance caused by a remote padded R
geometry decision. Outer rarity is irrelevant to the pointwise part of
M.11. No assertion about Yang–Mills existence, a differently defined
local-mask norm, or a mark confined MR-deep inside the regular region
is a consequence of this result.

### Mathematical sources

* CMP119, printed pp.244–245: fixed source grids, r≥2, and M≫M₂.
* CMP119, pp.247–253: actual first Q/R tests, independent free entries,
  flat constraint chart, domains (1.20), retained exterior, localization
  (1.21)–(1.22), and conditional integration (1.26).
* B-01/H-01, selector inventory and
  coefficient dictionary: deterministic domain construction and
  g₀⁻²=Nβ₀.
* Annex Y, (M.1)–(M.12): footprints, padding, actual native regulator,
  shifted pointwise norms and the exponential carrier weight.
* Annex X/F-01, equivalently [scalar extraction](scalar_extraction.md) (SE.1): exact
  positive Wilson scalar identity.
