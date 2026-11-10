# Broad first-step cutoffs: exact local-mask scalar responses

## Result and scope

After the explicit local-mask amendment, a change of one integrated
free-coordinate block has a bounded exact scalar response. The theorem
below includes the hard product cutoff, its normalizer, changing rank,
and a retained Gaussian force whose unconstrained mean may meet the
cutoff. It gives uniform native-energy bounds and exponential distance
decay, with no inverse cutoff probability and no factor growing like a
power of the cutoff P.

The theorem applies to the complete **first** flat-background Wilson
normal form, including its soft gauge, Haar, constraint and coarea
terms, on the common all-mask chart described below. It also supplies
an explicit positive continuation in the padded retained Lie-algebra
coordinates. It does not yet supply the exponentially weighted
**carrier-volume** expansion of the hard-cutoff output. Distance
decay alone is not that expansion. Nonflat coarse-link currents and
later inherited completed operations are not included.

The untruncated Gaussian full-carrier construction is separate, in
[M04 Gaussian Local Mask Carrier Theorem](M04_Gaussian_Local_Mask_Carrier_Theorem.md). The present result neither
assumes that hard cutoff corrections are uniformly rare at a large
retained force nor inserts a complex zero-free disk for that force.

## 1. The amended common coordinate law

Let J be the present independent free-coordinate index set. There is a
fixed number of real components per native block and a fixed number
of such blocks per current physical block. All constants may depend
on the fixed source L and group, but not on volume or mask geometry.
Distances below use the current block graph; fixed constraint stencils
are included in that distance convention.

An independent bit m_i says whether coordinate i is integrated:

\[
 I=\{i:m_i=1\},\qquad O=J\setminus I.
\]

The stored retained coordinates are r_i for every i in J. On the
actual supported state r_i=0 at integrated slots. The amended ambient
regulator retains the **whole padded list**,

\[
 R_X^{\rm mask}(r)=1+\sum_{i:\operatorname{foot}(i)\subset X}|r_i|^2
       +\text{the stated padded native plaquette energies}.
                                                               \tag{HC.1}
\]

There is no factor 1-m_i in this definition. On actual states this is
the original native energy. Off support it is an explicit extension.
Otherwise many ignored nonzero r_i could contribute to the sum of
mask currents while a one-edit regulator saw only their maximum.

Let D_i=P B_i, where B_i is the fixed symmetric convex unit norm ball
for that independent coordinate, and let D_I be the product. For a
globally defined retained-coordinate continuation choose a blockwise
smooth saturation r -> bar r with bounded first derivative, equal to
r on the actual first-step retained range and with |bar r_i|<=C_+P.
The source's first flat chart permits a fixed larger buffer C_+P
because gP tends to zero. It can be chosen with |bar r_i|<=C|r_i|.
No saturation is made inside the integrated domain D_i.

Assemble a_i=z_i on I and a_i=bar r_i on O. For one common complete
primitive potential V(a), define

\[
 \nu_{I,r}(dz_I)=Z_I(r)^{-1}{\bf1}_{D_I}(z_I)
       e^{-V(z_I,\bar r_O)}\,dz_I.                 \tag{HC.2}
\]

Every Z is the actual finite integral in this formula. A factor
independent of z_I cancels in this individual conditional; it is not
deleted from an outer history mass or a later restoration marginal.
For I empty, the physical old-field law is the point mass at bar r.
Dummy integration variables, if used to put all masks on a product
noise space, are ignored by the physical assembly.

The positive old-field law is the pushforward of (HC.2) by the common
reconstruction U=Phi_g(a). This is the filing explicitly permitted
after (M.28c): the microscopic Wilson mark is a function of the old
physical field, and every new reconstruction/rank response is in the
normalized-kernel current. For that filing B_new=0; the new J is the
actual difference of the two expectations. No total-variation
estimate of the mutually singular physical laws is used.

## 2. Quantitative inputs verified in the first flat chart

Write the common potential as

\[
 V(a)=\tfrac12 a^TKa-W(a),\qquad
 \lambda I\preceq K\preceq K_*I.                   \tag{HC.3}
\]

K is the actual constrained Wilson-plus-soft-gauge precision. It has
fixed finite range and uniformly bounded absolute rows. On the fixed
enlarged product |a_i|<=C_+P, the **complete** first-step perturbation
satisfies

\[
 \sup_i\sup_a|\partial_iW(a)|\le\epsilon_1,
 \qquad
 \sup_i\sum_j e^{\nu d(i,j)}
      \sup_a\|\partial_i\partial_jW(a)\|\le\epsilon_2,
                                                               \tag{HC.4}
\]

where

\[
 \epsilon_1\le C(gP^2+g^2P),\qquad
 \epsilon_2\le C(gP+g^2),\qquad
 \epsilon_1\le1,\quad \epsilon_2\le\lambda/4.
                                                               \tag{HC.5}
\]

The second inequality is a summed row bound, not a bound on a final
sum W without its locality. All mixed retained/integrated rows are
included. At the first flat step the potential actually has fixed
finite fluctuation stencils; an exponentially summable stencil
majorant is more than sufficient.

For the energy-normalized scalar write

\[
 f_x(a)=\alpha\beta\sigma_a(x;\Phi_g(a))-c.
\]

Its free-coordinate footprint S_x has fixed size. There is a fixed
b>=|alpha|+a^4|c| such that on the same enlarged chart

\[
 |f_x(a)|\le Cb a^{-4}\Bigl(1+\sum_{i\in S_x}|a_i|^2\Bigr),
 \qquad
 |\partial_i f_x(a)|\le
 Cb a^{-4}{\bf1}_{i\in S_x}
       \Bigl(\sum_{j\in S_x}|a_j|^2\Bigr)^{1/2}.
                                                               \tag{HC.6}
\]

The constant c has zero derivative. These estimates are for the
actual scalar, not just its quadratic Taylor coefficient.

### Source verification

At the first step with Omega_1 full and V_1=I the background is exactly
identity. For every source-admissible mask the localized minimum in
(1.21) is also identity, so the relocation (1.22) is identity. For an
arbitrary inconsistent or irregular mask, (HC.2) is defined directly
using the common original Phi_g and V. It does not invoke a
geometry-specific localized minimum on an unadmitted domain.
The exceptional-coordinate solve changes only b_0(c), using the two
adjacent fixed-L blocks. The Wilson, averaged soft-gauge, Haar and
coarea functions are therefore actual local analytic functions of a.
Their fixed-factor enlarged tube gives precisely (HC.4)--(HC.5), as
proved with the full measure factors in RMg.3--RMg.5 of
[first step relative marginal](first_step_relative_marginal.md).

The exact reconstruction has physical first derivative O(g), second
derivative O(g^2), and value Phi_g(0)=I. At a plaquette the trace of a
first generator is zero. Consequently beta s(Phi_g(a)_p) is bounded
by C sum_{S_p}|a_i|^2, and its derivative by C times that local norm,
using beta g^2=1/N. The analytic nonlinear correction contributes
only the fixed small factor gP to these same bounds. This proves
(HC.6) for the exact positive Wilson scalar stencil.

On actual first-step data the remaining primitive R/Q factors on
the integrated region are precisely its good product cutoff. The
other first-step factors are retained-only or redundant there, as
in C7 and CMP119 (1.19)--(1.26). On inconsistent ambient masks the
positive extension is (HC.2), without a new consistency selector
that would set its normalizer to zero. Thus it agrees with the
actual regular law on its stated supported flat-background family.
This source fit is not asserted for a general nonflat background or
for an old completed E/B/R density.

## 3. Real covariance and moments with the exact cutoff

For eta>0 define the weighted padded energy

\[
 \mathcal E_{x,\eta}(r)
 =1+\sum_{j\in J}e^{-\eta d(x,j)}|r_j|^2.           \tag{HC.7}
\]

These are useful bounds, not finite physical carriers. Their weights
have a uniform sum on the current graph.

### Lemma HC.1 -- uniform conditional covariance

For some eta>0, every measure (HC.2), every further pinning, and every
linear tilt obey

\[
 |\operatorname{Cov}(F,G)|
 \le C\sum_{i,j\in I}e^{-\eta d(i,j)}
       \|\partial_iF\|_{L^2}\|\partial_jG\|_{L^2}. \tag{HC.8}
\]

The constants are independent of P, the retained force, I and volume.

**Proof.** The potential restricted to I has Hessian at least
3lambda/4 and a fixed exponentially summable off-block majorant.
First extend W by the blockwise smooth saturation into its fixed
larger analytic tube as in RMg.1; its Hessian error stays O(gP).
Approximate the convex product cutoffs by convex block barriers.
Conjugation by the index weight exp(eta d(i,i_0)) changes only the
off-block Hessian and costs O(eta). It commutes with the arbitrarily
large positive diagonal block-barrier Hessian. Choose eta so that
the conjugated real part remains at least lambda/2.

The stationary Langevin-flow derivative then obeys the deterministic
entry bound C exp(-eta d(i,j)) exp(-lambda t/2). In the semigroup
covariance identity, Cauchy--Schwarz and stationarity bound the two
gradient factors by their L2 norms. Integrate in time and pass to the
hard-domain limit. The same argument on a principal subspace proves
the conditional assertion. A linear tilt changes no Hessian. This
is the L2 version of RMg.7, with the same barrier argument; it discards
no boundary term. QED.

### Lemma HC.2 -- local moments, including a large boundary mean

For every i in I and p>=1,

\[
 \|z_i\|_{L^p(\nu_{I,r})}
 \le C\left[\sqrt p+
       \sum_{j\in O}e^{-\eta d(i,j)}|\bar r_j|\right].
                                                               \tag{HC.9}
\]

In particular the square of the bracket at p=2 is bounded by
C E_{i,eta}(r), after reducing eta if needed.

**Proof.** First set W=0 and write h=-K_IO bar r_O. At h=0 the
cutoff Gaussian is even and has mean zero. Differentiating its mean
along the real linear tilt t h gives its covariance matrix. Apply
(HC.8) to coordinate functions and integrate from t=0 to 1. This
gives

\[
 |\mathbb E z_i|\le
 C\sum_{j\in O}e^{-\eta d(i,j)}|\bar r_j|.
                                                               \tag{HC.10}
\]

Now interpolate the complete perturbation theta W. Its mean
derivative is Cov(z_i,W), at most
C sum_j exp(-eta d(i,j)) epsilon_1 <= C epsilon_1.
This is bounded by a fixed constant by (HC.5).

Uniform convexity bounds the covariance of every real linear tilt
by a fixed multiple of the identity. Integrating the second
derivative of its log moment-generating function gives a uniform
sub-Gaussian bound for each coordinate about its mean. Combining
that bound with (HC.10) and the perturbative mean shift proves
(HC.9). All these are normalized cutoff measures throughout. QED.

The estimate is polynomial in the actual retained data. It does not
bound a translated normalization below by exp(-C|mean|^2), nor use
that loss as a moment estimate.

It follows from (HC.6)--(HC.9) that

\[
 |\nu_{I,r}f_x|\le Cb a^{-4}\mathcal E_{x,\eta}(r),
 \qquad
 \|f_x\|_{L^p(\nu_{I,r})}
       \le Cb a^{-4}[p+\mathcal E_{x,\eta}(r)].     \tag{HC.11}
\]

## 4. Exact one-mask restoration, with the completion factor

Let A be the common integrated set and let b be one additional
coordinate block. Write O for all remaining retained blocks. Put
y=bar r_b and keep bar r_O fixed. For w in the admitted enlarged
b-chart, let

\[
 q_A^w(dz_A)
 =Z_A(w)^{-1}{\bf1}_{D_A}e^{-V(z_A,w,\bar r_O)}dz_A.
\]

Let rho_b be the b-marginal of the exact joint q_{A union b}.
Fubini gives, with the same original potential,

\[
 \rho_b(dw)
 =\frac{{\bf1}_{D_b}(w) Z_A(w)\,dw}
        {\int_{D_b}Z_A(u)\,du},
 \qquad
 q_{A\cup b} f=\int \rho_b(dw)\,q_A^w f(\cdot,w).
                                                               \tag{HC.12}
\]

The factor Z_A(w) here includes all w-dependent terms, even those
constant in z_A. They cancel in q_A^w alone but not in rho_b.

For W=0 this has an explicit Schur form. With h=-K_{J O}bar r_O,
J=A union b, define

\[
 S_b=K_{bb}-K_{bA}K_{AA}^{-1}K_{Ab},\quad
 m_b=S_b^{-1}(h_b-K_{bA}K_{AA}^{-1}h_A),\quad
 m_A(w)=K_{AA}^{-1}(h_A-K_{Ab}w).
\]

Then, up to its displayed normalization,

\[
 \rho_b(dw)\ \propto\
 {\mathbf1}_{D_b}(w)
 e^{-\frac12(w-m_b)^T S_b(w-m_b)}
 \mathcal C_A(m_A(w))\,dw,
 \quad
 \mathcal C_A(m)=\Pr_{N(m,K_{AA}^{-1})}(D_A).       \tag{HC.13}
\]

The completion factor C_A is generally not constant and may be very
small. Replacing rho_b by a truncated Gaussian with precision S_b
alone is wrong. The estimates below use rho_b as a marginal of the
full uniformly convex law and hence require no lower bound on C_A.

The exact release response is

\[
 Q_{A\cup b}f_x-Q_A^y f_x
 =\int\rho_b(dw)
   \{q_A^w f_x(\cdot,w)-q_A^y f_x(\cdot,y)\}.     \tag{HC.14}
\]

This identity compares the original rank-changing conditional laws.
It also holds when y lies outside D_b but inside its fixed larger
retained chart. The path from y to w stays in that enlarged convex
chart; the integrated domain D_A stays unchanged.

## 5. The actual response estimate

### Theorem HC.3 -- one-mask value/current bound

Under (HC.3)--(HC.6), for some eta>0,

\[
 |Q_{A\cup b}f_x-Q_A^y f_x|
 \le Cb a^{-4}e^{-\eta d(x,b)}
       [\mathcal E_{x,\eta}(r)+\mathcal E_{b,\eta}(r)].
                                                               \tag{HC.15}
\]

It holds in both directions of the mask flip and is uniform in the
shape and rank of A. Here b before a^{-4} denotes the incoming
coefficient budget; the subscript b denotes the changed coordinate
block. No cutoff P appears in the constant.

**Proof.** For H(w)=q_A^w f_x(.,w), normalized differentiation on the
fixed product domain gives

\[
 D_w H
 =q_A^w D_w f_x
   -\operatorname{Cov}_{q_A^w}(f_x,D_wV).           \tag{HC.16}
\]

The first term is zero unless b belongs to S_x. In the covariance,
the z_A gradient of the score is the exact mixed Hessian row
K_{Ab}-D_A D_b W. Its constant-in-z part has zero covariance.
Use (HC.8), (HC.4), and the local gradient bound (HC.6). Lemma HC.2
then gives, along w_t=(1-t)y+tw,

\[
 |D_w H(w_t)|\le
 Cb a^{-4}e^{-\eta d(x,b)}
 \left[\mathcal E_{x,\eta}(r)^{1/2}
              +e^{-\eta d(x,b)/2}|w|\right],      \tag{HC.17}
\]

after a fixed reduction of eta. The original y contribution is
already included in E_x. Fixed-stencil direct terms obey the same
inequality after changing its constant.

Integrate along this real segment and then against rho_b in
(HC.14). Lemma HC.2 on the joint A union b law gives
rho_b(|w|^2)<=C E_{b,eta}(r), and |y|^2<=C E_{b,eta}(r).
Cauchy--Schwarz controls |w-y| and |w-y||w|. Finally
sqrt(E_x E_b)<= (E_x+E_b)/2. This proves (HC.15).
Its absolute value is unchanged on reversing the flip. QED.

The proof is valid for the complete first Wilson potential, not just
for a quadratic V. The exact covariance score in (HC.16) includes the
mixed coarea/Jacobian and nonlinear Wilson derivatives through W.

If one instead files the coordinate assembly as a separate direct
map, the release response splits exactly into

\[
 B_b^+=q_{A\cup b}
      [f_x(z_A,w)-f_x(z_A,y)],
\]
\[
 J_b^+=\int\rho_b(dw)
        [q_A^w f_x(\cdot,y)-q_A^y f_x(\cdot,y)].    \tag{HC.18}
\]

The first term is supported only when b meets the original free
root stencil. The second is bounded by (HC.8) along the specified-root
path. Each term separately obeys (HC.15), with a changed constant.
The reverse M30 records use the actual opposite rectangular path
and need not be the negatives of these two individual records.
In the physical pushforward filing fixed in Section 1 their sum is
the single new normalized-kernel record J, and B_new=0. This is an
explicit representation choice allowed by (M.28c), not a cancellation
of unestimated records.

### Summed mask response

Exponential convolution on the bounded-growth graph gives

\[
 \sum_b |\Delta_b Q_m f_x(r)|
       \le Cb a^{-4}\mathcal E_{x,\eta/2}(r).      \tag{HC.19}
\]

Indeed sum_b exp(-eta d(x,b)) E_b is bounded by a fixed multiple of
E_{x,eta/2}, by the triangle inequality for distance and exponential
summability. Thus changing an arbitrary number of ranks does not
introduce a total-volume factor into the **summed one-edit envelope**.
All directions in a coordinate block contribute only their fixed
component multiplicity.

## 6. Retained continuous currents

The same normalized derivative (HC.16), with b now a retained
coordinate and no restoration integral, proves

\[
 \sup_{0<|t|\le1}
 \left|\frac{Q_mf_x(r+t e_j)-Q_mf_x(r)}{t}\right|
 \le Cb a^{-4}e^{-\eta d(x,j)}
             [1+\mathcal E_{x,\eta}(r)^{1/2}].     \tag{HC.20}
\]

Only the chosen retained block changes along the path. The local
saturation has bounded derivative and changes its energy by O(1)
under such a shift. If the slot is integrated, the kernel ignores
its stored r_j and the difference is zero. Summing j again has a
constant bound. These are actual finite differences, obtained by
integrating the derivative of the same positive normalized kernel.

Under the physical pushforward convention all these newly generated
responses are J records. Given incoming direct or old-current
records, they would be integrated separately according to (M.30);
the present microscopic scalar has no earlier current to absorb.

If the actual outer law has the stated padded local reserve
||r_j||_{L^{2p}}^2<=Cp uniformly, Minkowski gives
||E_{x,eta}||_{L^p}<=Cp. Consequently (HC.11), (HC.19), and (HC.20)
have the required value grade one and current grade at most one,
hence also the M03 allowed grade 3/2. This last assertion uses that
true outer reserve; a conditional bound does not manufacture it.

## 7. What is genuinely settled, and the remaining carrier question

The one-mask current is finite even when changing rank, even when a
retained value lies above the integrated cutoff, and even when the
unconstrained Gaussian mean lies next to its boundary. The actual
normalized cutoff completion is present throughout (HC.12)--(HC.17).
The geometry counterexample from the preceding analysis is now a
bounded **local** mask response: its changed mask lies next to the
insertion. No remote construction footprint is assigned to that new
primitive mask coordinate in the amended interface.

Nevertheless (HC.19) is not a complete physical-carrier theorem.
A family of ball approximations with error exp(-c radius) would
have carriers of volume proportional to radius^4, and would not
be summable against exp(kappa |X|). The weighted energy E_x and
the pointwise influence kernel in this note are not themselves
an exact finite-carrier decomposition of Qf_x or of its records.

The untruncated Gaussian theorem supplies genuine connected
carrier coefficients for the principal inverse, mean and quadratic
root with independent mask bits. Its blocked-power argument uses
uniform matrix contraction only after grouping a fixed finite number
of powers into locally supported coefficients. It does not imply
an analogous inverse formula for the nonlinear hard-cutoff
completion C_A in (HC.13).

The missing hard-cutoff statement is therefore concrete: construct
an exact connected coefficient family for the normalized cutoff
correction, with a common positive physical carrier rate, its full
padded-energy majorant, and its separate retained/mask records.
One-mask exponential mixing and a bound for a completed logarithm
are not sufficient substitutes. The relevant object is a real
conditional completion of the **same** finite-range uniformly
convex potential; no older residual posterior is involved in this
first-step gate.

## 8. Why a uniform rare-cutoff replacement is invalid here

Already in one dimension let

\[
 q_{P,m}(dz)\propto
 {\mathbf1}_{[-P,P]}(z)e^{-(z-m)^2/2}\,dz.
\]

At m=P, elementary half-Gaussian integration gives

\[
 q_{P,P}z=P-\sqrt{2/\pi}+o(1),\qquad
 q_{P,P}z^2=P^2-2P\sqrt{2/\pi}+1+o(1).             \tag{HC.21}
\]

The full Gaussian second moment is P^2+1. Thus the cutoff correction
is of order P, not exp(-cP^2). It is still bounded by the native
quadratic energy and fully consistent with (HC.15). A precision gap
alone does not put the conditional mean a fixed fraction inside
the cutoff.

Likewise a complex continuation of a mean of size P can have an
absolute Gaussian normalization loss exp(C|Im m|^2). A fixed complex
decoupler radius may therefore cost exp(CP^2). Neither this note nor
the untruncated carrier theorem assumes that cost away. A proof of
the hard completion family must either keep the real normalized
conditional structure used above or establish an actual additional
source margin. The present source support bound |r|<=CP is not such
a margin.

## Sources and companion proofs

* CMP119 (1.9), (1.14)--(1.26): actual first independent coordinates,
  broad cutoff, local reconstruction and complete regular integral.
* [first step precision gap](first_step_precision_gap.md): flat positive precision, its fixed
  range and the actual averaged soft-gauge convention.
* [first step relative marginal](first_step_relative_marginal.md), RMg.3--RMg.9: complete first
  derivative rows, convex-boundary covariance proof and arbitrary
  pinning. This note uses its real covariance mechanism, not an
  unsupported large-force complex disk.
* Annex Y (M.28c)--(M.32): physical pushforward filing and exact
  normalized-kernel finite differences for changing supports/ranks.
* Annex X (F.6)--(F.7), (F.17): exact positive Wilson scalar.
* [M04 Local Mask Interface](M04_Local_Mask_Interface.md): explicit amended local masks,
  padded retained state, regulator and positive common-chart law.

The result is an actual broad first-step local-response theorem on
the stated flat common chart. The full hard-cutoff physical-carrier
bound, nonflat group-coordinate currents and general later source
sectors remain distinct proof obligations.
