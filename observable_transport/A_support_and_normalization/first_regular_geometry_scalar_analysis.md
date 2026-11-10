# Scalar analysis of the first regular geometry test

## Scope and conclusion

The proposed test compares two active first-step histories with the same
flat coarse field, full determining domain Omega_1, and nested retained
R holes. The common integrated domain contains an insertion next to the
larger hole. The histories differ through an additional R seed a distance
of order MR from that insertion.

The physical Gaussian variance gap, the exact positive Wilson scalar
stencil, and the first-step perturbative transfer are valid. The source
does not require a regular insertion or its whole stencil to be MR-deep
inside Lambda_1. The distinction between Lambda_1 and Omega_1 is essential.

Annex W Section 2.2 identifies Omega_j, Lambda_j and S_j as domains
**obtained from the preceding primitive labels**. Combined with the
original full defining-footprint convention of M.1, this gives a
spatial-norm obstruction in that specified ledger. It is not a no-go theorem
for every different augmented state. A geometry-dependent identity
coefficient also has to retain its own current; treating such a
coefficient as an unrestricted number would evade, rather than satisfy,
the requested matching estimate.

## 1. The actual scalar and its signs

Annex X (F.6), (F.7), and (F.17) give exactly

\[
 \sigma_a(x)=\langle e_S,\widetilde q_a(x)\rangle
 =\frac{1}{2\sqrt6\,a^4}
   \sum_{\mu<\nu}\sum_{\epsilon,\epsilon'=\pm1}
      s(P_{\epsilon e_\mu,\epsilon'e_\nu}(x)).       \tag{GS.1}
\]

All 24 coefficients in this expression are positive. Although the matrix
repair contains the subtraction of the clover trace, that subtraction
cancels in the scalar projection. There is no signed clover remainder
in (GS.1). Every elementary plaquette occurs in the scalar stencil at
each of its four vertices, with the appropriate signed orientation; its
Wilson energy is unchanged by reversal or a change of starting vertex.

For the actual F01 field, write

\[
 F_a(x)=\alpha_a\beta_a\sigma_a(x)-c_a,
 \qquad \alpha_a=z_{S,a}/\beta_a>0.                 \tag{GS.2}
\]

The coefficient is strictly positive both on the nondegenerate branch
(F.33) and on the explicitly labelled totalization (F.35). Its size is
not assumed uniform. The input budget exposes it. The centering c_a is
a real number obtained from the full compact Wilson law and cancels in
the difference between two histories at the same cutoff.

With Hermitian tangent fields and Hilbert--Schmidt norm,

\[
 s(\exp(i g_0 f))=\frac{g_0^2}{2}\|f\|_{\rm HS}^2
                 +O(g_0^3\|f\|^3).
\]

Thus the quadratic scalar is

\[
 a^4\beta_a\sigma_a^{(2)}(x)
 =\frac{\beta_a g_0^2}{4\sqrt6}
       \sum_{p\in\mathcal P_x}\|(d C_0 z)_p\|^2.  \tag{GS.3}
\]

The exact source normalization fixes the positive number beta_a g_0^2;
no varying fine-scale power is hidden in it. Keeping this number exposed
also makes the argument independent of a choice of normalized trace.

## 2. Source geometry and the admitted flat centers

CMP119 (1.18) partitions the actual independent first-step free
coordinates at the broad threshold P=delta_0/g_0. Its elementary tests
use L^2 M_2 R_1 cubes. The union of the intersected LMR_1 cubes is a
different set, denoted R'_1 in the source. One must first place the seed
strictly within a test neighborhood whose entire footprint lies inside
one such larger covering cube. The fixed hierarchy M much larger than
M_2 permits this; neither test cubes nor their enlargements are silently
identified with covering cubes.

For Omega_1 equal to the full torus, (1.20) surrounds this cover by one
covering-cube layer in Lambda_1^c. Start with one covering cube and then
add its neighbor across a fixed face. The corresponding holes are
nested rectangles; both are among the components of side less than
100 LMR_1 for which the source rectangular completion is prescribed.
The added seed lies inside the original one-cube-plus-one-layer hole.
Consequently its old free coordinate can be retained in both histories:
set it to zero in the first and to 3P/2 in the second. The added outer
strip of the larger hole has zero retained free coordinates.

The nonzero seeds are a distance cMR_1 from either integration boundary.
The original seed can be chosen the same in both histories. At the two
centers take V_1=I and every other retained free coordinate to be zero.
The initial P/Q selectors have strict margins: on actual free entries
the approximate Q threshold is 2P, while P curvature and soft gauge
ceilings have the fixed larger A_0/A_1 allowance. The exceptional bond
solve and reconstruction have fixed-L bounds, so choosing the source
constant hierarchy first gives the required P/gauge margins. The R
test at each chosen seed is strictly bad, and all other R test cubes
are good. The exact list of test cubes triggered by one seed is kept;
its fixed number does not grow with R.

The two global minimizing backgrounds are identity. The localized
background U_1(Omega_1 intersect Lambda_1^c,V) used in (1.21) is also
identity. Hence H_{1,Lambda_1}=0 in (1.21), and every relocation (1.22)
and its Jacobian is exactly the identity at these retained centers.

These are active fixed-history fibers, rather than values imposed by
an inactive extension. Strictness gives positive neighborhoods of each
center in its own fixed geometry. They can be made as small as needed
when comparing conditional expectations.

## 3. An exact covariance identity

Use the common actual flat independent free-coordinate precision K.
It includes the constrained Wilson Hessian and the source soft gauge
quadratic. Its fixed-L gap and row bound are proved in
[first step precision gap](first_step_precision_gap.md):

\[
 \lambda I\le K\le K_* I.                            \tag{GS.4}
\]

K has fixed finite range. Because the retained seeds are MR-deep and
the boundary collar is zero, K_{IO}y=0 for both integrated index sets.
The conditional Gaussian means are therefore exactly zero.

Let A be the smaller integrated set, namely the complement of the
larger hole. Let B be the strip integrated only in the other history.
All common retained exterior coordinates are held fixed. On A union B,
put

\[
 S_B=K_{BB}-K_{BA}K_{AA}^{-1}K_{AB},\qquad
 \mathcal R=\binom{-K_{AA}^{-1}K_{AB}}{I_B}.
\]

Block inversion gives the padded covariance identity

\[
 K_{A\cup B,A\cup B}^{-1}
   -\begin{pmatrix}K_{AA}^{-1}&0\\0&0\end{pmatrix}
 =\mathcal R S_B^{-1}\mathcal R^T\succeq0.           \tag{GS.5}
\]

Moreover S_B is positive and S_B <= K_BB <= K_* I, so
S_B^{-1} >= K_*^{-1} I. Formula (GS.5) implies nonnegativity of
the covariance difference for every linear plaquette curvature,
including a plaquette crossing the A/B interface. Nonzero K_AB by
itself is not a sufficient scalar-gap argument; the next construction
supplies the missing physical curvature.

## 4. A finite Bianchi patch forces a Wilson gap

Choose a coarse-block face in the extended flat face of the larger
hole, away from its corners. On its B side take an elementary
tangential plaquette whose edges are intrablock. Choose one of its
bonds e and let b be the unit vector of that independent free
coordinate, in a fixed unit Hilbert--Schmidt Lie-algebra color. These
four plaquette edges are not exceptional bonds b_0(c), since those
cross coarse-block interfaces. The source L>11 supplies this small
patch; no dimensional nullspace construction or larger L is needed.

Consider the constrained cochain C_0 R b. The inner-face bond e has
value one, and its other three edges have value zero. The A extension
cannot change independent entries in B, and C_0 changes only
exceptional entries. Hence its curvature on this inner plaquette is
exactly a unit color:

\[
 |(d C_0\mathcal Rb)_{p_{\rm in}}|^2=1.            \tag{GS.6}
\]

It is unnecessary to impose Qb=0 separately: the actual embedding C_0
already gives Q C_0 Rb=0 for every free vector Rb. Attach the elementary
3-cell which crosses the interface in its normal direction. Linear
Bianchi expresses the inner-face curl as the signed sum of the other
five face curls. Each of those other plaquettes has a vertex on the
A side. Cauchy--Schwarz yields

\[
 \sum_{p\in\mathcal P_{\rm patch}}
       |(d C_0\mathcal R b)_p|^2\ge \frac15.        \tag{GS.7}
\]

The patch contains exactly those five plaquettes, independent of R,
L and the torus.
Combining (GS.5)--(GS.7) gives

\[
 \sum_{p\in\mathcal P_{\rm patch}}
  \left[\mathbb E_{A\cup B}|(d C_0z)_p|^2
               -\mathbb E_A|(d C_0z)_p|^2\right]
       \ge \frac1{5K_*}.                              \tag{GS.8}
\]

For each patch plaquette choose one A-side vertex. Its exact scalar
stencil (GS.1) contains that plaquette with positive coefficient. The
variance differences for all additional plaquettes in these stencils
are nonnegative by (GS.5). Summing the finitely many chosen scalar
stencils proves that at least one insertion anchor x in A satisfies

\[
 a^4\left[\mathbb E_{A\cup B}(\beta_a\sigma_a^{(2)}(x))
           -\mathbb E_A(\beta_a\sigma_a^{(2)}(x))\right]
       \ge c_{L,N}>0.                                 \tag{GS.9}
\]

Its stencil is allowed to cross the integration boundary. Annex Y
(M.2), (M.12), and the M04 statement require its actual support in the
carrier; they impose no condition that the whole stencil lie in A.
CMP119's Omega/Lambda separation concerns the determining-field
boundary. It is not a separation from the conditional Gaussian
boundary partial Lambda.

## 5. Transfer to the actual broad first-step law

Take a compatible torus with side a fixed multiple of MR_1. Its
independent coordinate count is O(R_1^4). On the actual broad product
cutoff, all integrated entries are bounded by P and all retained seed
entries by 3P/2. The fixed local constraint reconstruction bounds all
full tangent entries by C_L P. At the flat reference the complete
primitive Wilson, soft gauge, Haar and coarea expansion has a uniform
relative log-density error

\[
 \epsilon_g\le C g_0\,\operatorname{poly}(P,R_1)=o(1).
                                                               \tag{GS.10}
\]

There is no inherited completed activity at this first step. The
reference and relocation constants cancel exactly in the conditional
ratio. The actual scalar differs from its quadratic scalar by another
g_0 times a fixed polynomial in P. Choose the small-coupling tail so
that these errors, even after multiplication by the local P^2 bound,
are smaller than one fourth of the fixed gap (GS.9).

The centered Gaussian product-cutoff removal error is also o(1).
For example the gap (GS.4) bounds every coordinate variance uniformly;
a union bound over O(R_1^4) coordinates gives a failure probability
O(R_1^4 exp(-cP^2)). Gaussian Cauchy--Schwarz bounds the error for a
fixed quadratic root. The actual source P grows faster than the
square root of log R_1, so this error tends to zero. This argument is
being used on the chosen finite torus; it does not assert a
volume-uniform global cutoff removal theorem.

Thus the exact conditional outputs at the two active centers obey

\[
 a^4\left|Q_{\rm small\ hole}F_a(x)
                -Q_{\rm large\ hole}F_a(x)\right|
       \ge c_{L,N}\,|\alpha_a|                       \tag{GS.11}
\]

after reducing the positive constant. The initial microscopic input
has its ordinary fixed-stencil M03 budget, with the given alpha_a and
c_a exposed. No claim about F05 or a depth-uniform M07 budget enters.

### 5.1 A volume-uniform version on the actual physical torus

The polynomial-size torus above is not required. The same conclusion
holds on an arbitrarily large admitted torus, by the already proved
first-step relative marginal lemma and Gaussian cutoff-removal theorem.
Here are their actual hypotheses in this application.

Pin all retained entries, including the seeds of size at most 3P/2.
The free-coordinate perturbation W is still the complete local first-step
Wilson/soft-gauge/Haar/coarea function. Its fixed-factor complex tube
contains every such pinned value. The real derivative rows of
[first step relative marginal](first_step_relative_marginal.md), (RMg.4)--(RMg.5), remain

\[
 \sup_i|\partial_iW|\le C(g_0P^2+g_0^2P),\qquad
 \sup_i\sum_j e^{\nu d(i,j)}
       \sup|\partial_i\partial_jW|
       \le C(g_0P+g_0^2).                           \tag{GS.10a}
\]

Pinning gives a principal compression of K, preserving (GS.4) and its
finite range. The linear Gaussian force is exactly zero, as proved in
Section 3. Thus RMg.18 applies on either actual Lambda product support.
If D is the fixed finite free-coordinate stencil of a local quadratic
scalar, its actual marginal and same-cutoff Gaussian marginal obey

\[
 \left|\log\frac{p_{\rm actual,D}}{p_{\rm G,P,D}}\right|
       \le C(g_0P^3+g_0^2P^2)|D|.                  \tag{GS.10b}
\]

All density terms are retained. There is no volume-sized Taylor error
and no division by the probability of a complete R history.

For clarity, the volume-uniform Gaussian cutoff theorem is also
applicable to these holes. If H=K_II, conjugation by the diagonal
weight exp(kappa d(i,i_0)) changes H in operator norm by O(kappa),
uniformly in I, because H is finite range with bounded rows. Choose
kappa so that this is at most lambda/2. The energy estimate for the
conjugated semigroup gives

\[
 |(e^{-tH})_{ij}|
       \le C e^{-\kappa d(i,j)}e^{-\lambda t/2}.
                                                               \tag{GS.10c}
\]

Summing over the polynomial-growth fine graph and integrating in t
verifies Annex K assumption (2.3), with the same constant for either
principal domain. Its Theorem 5.1 therefore removes the product cutoff
from any fixed local quadratic with error
`C (1+P)^C exp(-cP^2)`, independently of the torus volume and hole size.

If the source unit norm ball is not Euclidean, the same proof applies
directly: its one-block effective potential is even and satisfies
lambda I <= v_i'' <= H_ii by the covariance formula and Prekopa's
theorem. A fixed convex norm ball has boundary area O(P^{d_G-1}) and
every boundary point has Euclidean norm at least cP. The normalized
boundary flux is therefore O(P^{d_G-1} exp(-cP^2)); the divergence and
semigroup proof of Annex K is unchanged. Fixed nonsmooth norm balls
are handled by convex approximation or their Lipschitz-boundary
divergence theorem. No probability of a global cutoff event occurs.

The nonnegative quadratic scalar has uniformly bounded Gaussian
moments by (GS.4). Equation (GS.10b) compares its two expectations with
an o(1) error. The local exact-root Taylor error is at most Cg_0P^3
on its finite stencil, hence also o(1). Combining these comparisons
with (GS.9) proves (GS.11) uniformly in every admitted total volume.
The physical torus and a cofinal relation between a and g may therefore
be retained.

The displayed centers need not be atoms of the retained law. The C7
conditional integral specifies its value at each strictly admitted
center. It is continuous in a neighborhood in its fixed-history
chart, so the nonzero gap persists in neighborhoods. Moreover any
alternative version with finite M03 continuous-current bound is
locally Lipschitz there and agrees with that version everywhere if
it agrees almost everywhere. Modifying only the two center values
cannot remove the conclusion within the finite-current class.

## 6. Scalar and identity subtraction cannot delete a current

F01 (F.30)--(F.35) specifies numerical coefficients from the actual
compact law. They are constant in spacetime and do not depend on an
individual retained RG history. In an expansion over the fixed
incoming scalar and identity basis with numerical matching
coefficients,

\[
 QF_a=a_k\varphi_{La}+c_k+\mathcal E_k,               \tag{GS.12}
\]

the two centers have the same current coarse field V_1=I. Both basis
functions consequently have the same value at the two centers. The
entire difference (GS.11) remains in E_k. The same conclusion holds
if the scalar basis is centered: its value at identity is another
fixed numerical constant.

If instead a proposed matching permits a_k(r) and c_k(r), where r is
a retained geometry or history coordinate, these are new functions,
not the numerical F01 normalization. Their finite differences obey
the exact product rule. At flat coarse data the discrepancy moves
into the history-dependent identity combination

\[
 c_k(r)+a_k(r)\varphi_{La}(I).                         \tag{GS.13}
\]

It still has the same geometry dependence and full footprint. Its
current must be retained as a marked output record by (M.10),
(M.24), (M.30) and SR20.15--SR20.19. Assigning no budget to (GS.13)
would allow any output to be called an identity coefficient and would
make the matching test vacuous. The M-04 statement does not explicitly
prescribe a unique projector, but neither does a choice of projector
erase a nonconstant coefficient's actual current.

## 7. Consequence in the declared source-derived coordinate ledger

The two centers have identical coarse fields and identical retained
free entries near the root. Their changes in source seed data and
elementary R tests lie a distance cMR_1 away. Annex W Section 2.2
explicitly calls P/Q/R the primitive selector labels and says that
Omega_j, Lambda_j and S_j are obtained from those labels by their
specified covers, layers and rectangular hulls. This is the
defining-coordinate convention used here.

M.1 says explicitly that a coordinate whose definition uses several
blocks has that entire dependency footprint, even when stored at one
block. A derived Lambda membership flag therefore cannot be assigned
only its storage point while its actual definition still uses the
distant R seeds. Every coordinate which differs between the active
centers either is in the seed neighborhood or has such a far defining
footprint. Consequently every supported tagged value whose values at
the two centers differ must have a carrier joining the insertion
anchor to distance cR_1 in output units.

There is a direct lower bound using the value part of M03; no
off-support telescoping path is necessary. At these centers all raw
current links are identity, all inactive slots have their reference
values, and only a fixed number of retained seed coordinates have
size O(P). One allowed normalized elementary shift changes their
native regulator by at most a fixed polynomial. With the first-step
native list this gives

\[
 \widehat R_{La,X}(v_s)+\widehat R_{La,X}(v_l)
       \le C(1+P^2)                                 \tag{GS.14}
\]

for every carrier X; allowing a harmless fixed polynomial in R would
give the same conclusion. Fixed coordinate/scale labels in (M.3)
prevent an elementary history edit from changing a coupling label.
All other padded raw variables remain identity or zero.

Let A_X be any exact supported output representation. Tags whose
carriers do not reach a changed defining footprint have equal values
at the two centers. Apply the pointwise value term of (M.11) to the
remaining tags and use their weight at least exp(kappa cR_1). It
follows that

\[
 \sum_X w_{La}(X)v_{La,1,X}(A_X)
 \ge
 \frac{c(La)^4\,|Q_sF_a(x)-Q_lF_a(x)|}
      {1+P^2}\,e^{\kappa cR_1}
 \ge c L^4|\alpha_a|
      \frac{e^{\kappa cR_1}}{1+P^2}.                \tag{GS.15}
\]

The same bound applies to a remainder after numerical scalar/identity
subtraction by Section 6. If geometry-dependent coefficients are
permitted, it applies to the total represented coefficient/remainder
family which carries the same difference; their support/current is
not omitted.

For the actual F01 centering, (F.31) and (M.14) give

\[
 a^4|c_a|=|\alpha_a|\,a^4\beta_a|m_{a,T}|
       \le C|\alpha_a|,
 \qquad b_a=|\alpha_a|+a^4|c_a|\le C'|\alpha_a|.    \tag{GS.16}
\]

This uses exactly the admitted initial energy reserve, not F05.
Thus even if alpha_a varies with the cutoff, dividing (GS.15) by the
genuine microscopic input budget leaves a factor
exp(kappa cR_1)/poly(P,R_1) tending to infinity. The initial scalar
stencil and all fixed-L conversions contribute only fixed constants.
If one uses only compactness, b_a is at most C|alpha_a|(1+beta_a);
that weaker bound also suffices because the source radius exponent
is r>=2 and exp(kappa cR_1) dominates beta_a.

The resulting obstruction is to a uniform regular M04 transport
estimate in this declared source-derived full-footprint ledger. It
does not assert a no-go theorem for every possible augmented state.
Introducing redundant local membership flags as *independent*
padded primitives, with their consistency only imposed in the law,
would be a changed coordinate presentation. Its compatibility,
pullback and selector interface must be specified and examined
explicitly; it is not the derived-coordinate convention of Annex W.

Likewise, one cannot compare two different physical reconstructions
by holding only their stored arrays equal and ignoring the changing
pullback. At the two flat centers considered here the source (1.22)
is exactly identity, which removes that particular ambiguity. The
coordinate convention in the preceding argument is the declared
Annex W/M.1 one, not an inference from a flag's storage address.

## Summary

Established here: the positive exact scalar stencil; the
single-bond constrained Bianchi construction; the padded Schur
monotonicity identity; zero conditional means at the flat admitted
centers; the first-step volume-uniform perturbative transfer; and the
scope of numerical versus history-dependent scalar/identity
subtraction.

Established for the declared Annex W/M.1 convention: the resulting
supported-value norm obstruction. Still outside the conclusion: a
different local-mask augmentation with a separately proved interface,
and a norm which changes the treatment of live boundary geometry.
This note neither changes the source nor proves M04.
