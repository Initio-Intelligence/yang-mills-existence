# A local smooth bundle reference for admissible SU(N) link fields

This note constructs a regular fine reference directly from raw current links. It does not choose a global small-link gauge and does not interpolate independently chosen gauge representatives. The construction is local in a fixed current neighborhood, works at every fine depth, and preserves the holonomy of each current edge exactly. Its nonlinear block averages need only approximate the prescribed current links: that is the hypothesis used by CMP102 (14).

The theorem concerns a homogeneous current lattice with an admitted fixed halo. Mixed determining geometries and the complete old residual conditional density are not identified with this construction here.

## 1. Statement and geometric conventions

Let the current lattice be a cubical lattice of spacing one in dimension four, with periodic or local boundary conditions. Every fixed neighborhood used below is assumed to be embedded and contractible; on a torus its side lengths can be taken larger than twice the fixed construction radius. Let

\[
 v_{ij}\in SU(N),\qquad v_{ji}=v_{ij}^{-1},\qquad
 \sup_p\|v(\partial p)-I\|\le\varepsilon .
 \tag{BR.1}
\]

All constants below depend on the fixed dimension, N, the fixed interpolation functions, and, where indicated, L. They do not depend on volume or on the fine depth `k`, with `η=L^{-k}`. The construction uses only a fixed number of raw current links near the point or fine bond being evaluated. A local statement uses the corresponding enlarged input halo.

### Theorem BR.1

For sufficiently small fixed `ε`, there is an explicitly constructed smooth rank-N Hermitian bundle with an SU(N) connection over current physical space, and a field `U_ref(v)` of its fine-lattice parallel transports in geometrically selected local frames, with the following properties.

1. `U_ref` is SU(N)-valued for real data. The product along the straight fine subdivision of every current edge `(i,j)` equals exactly `v_ij`.
2. A fine link depends only on raw current links in a fixed current neighborhood of that link. This dependence is analytic in complex SL(N) perturbations of admitted real data, on a uniform local neighborhood. The matrix operations and logarithm branches defining the construction are fixed explicitly below.
3. If `δ_X=Σ_{p⊂X}||v(∂p)−I||` on the fixed input halo of a fine plaquette and its immediate neighbors, then

\[
 \|U_{\rm ref}(\partial p)-I\|\le C\eta^2\delta_X,
 \qquad
 \|D^*\partial U_{\rm ref}\|\le C\eta^3\delta_X .
 \tag{BR.2}
\]

The second expression is the unrescaled covariant lattice difference of neighboring plaquette holonomies. All required fixed higher covariant differences satisfy the corresponding powers of `η`. Thus the source's normalized curvature and first curvature derivative are bounded by `Cε`.
4. For the literal nonlinear k-fold Balaban average,

\[
 \|\mathcal M^k(U_{\rm ref})_c-v_c\|\le C_L\varepsilon
 \tag{BR.3}
\]

uniformly in k. Both sides transform by the same gauge values at current vertices.
5. Coarse gauge transformations act on the fine field through a geometrically fixed block-constant lift. There is no gauge selected by following a path across the full volume.
6. Nearby raw data admit a local, center-fixed analytic bundle identification. In this common frame their connection difference and every required fixed spatial derivative are `O(δ)` when their raw links differ by `O(δ)`. In particular their fine relative field has the native form `exp(iη A)` with source-normalized `A` and first derivatives `O(δ)`. This last assertion is necessary for the source complex field domain; raw matrix analyticity alone would not establish it.

The smooth bundle may be topologically nontrivial. Only a frame at each discrete fine vertex is selected. No global smooth frame is asserted.

## 2. A partition with the exact edge property

Choose a smooth increasing function `θ:[0,1]→[0,π/2]`, constant near both endpoints, such that

\[
 \theta(1-t)=\pi/2-\theta(t).
\]

For a one-dimensional lattice vertex n, define its nonnegative weight on the two adjacent intervals by

\[
 w_n(t)=\cos\theta(t-n)\quad(n\le t\le n+1),
 \qquad
 w_n(t)=\sin\theta(t-n+1)\quad(n-1\le t\le n),
\]

and zero elsewhere. These functions are smooth, with support strictly inside the open two-interval star, and satisfy `Σ_n w_n(t)^2=1`. Tensor products in the four directions give smooth weights `w_i(x)` at current vertices with

\[
 \sum_i w_i^2=1,\qquad \psi_i=w_i^2.
 \tag{BR.4}
\]

At most `2^4` weights are nonzero at one point. On a current edge only its two endpoint weights are nonzero. At a current vertex i, `w_i=1` and all other weights vanish. Every fixed derivative of the weights is uniformly bounded.

Take an open geometric star `O_i` slightly larger than the support of `w_i`. A fine vertex x is assigned one current vertex `i(x)` by a fixed nearest-vertex/block rule, independent of v. This rule can be the original current block convention; on its boundary choose a fixed convention. Its assigned weight is bounded below by a fixed positive number. The later formulas in fact do not require division by this weight.

## 3. Short transports and the approximate projection

For any pair of current vertices whose stars can meet, choose once and for all a bounded-length lattice path from i to j in their fixed neighborhood. Use its reverse for the reversed pair, and use the actual one-edge path on nearest-neighbor edges. Write its transport as `g_ij(v)`. Then

\[
 g_{ji}=g_{ij}^{-1},\quad g_{ii}=I,\quad
 g_{ij}=v_{ij}\ \hbox{on actual current edges}.
 \tag{BR.5}
\]

A bounded loop in these fixed contractible boxes is a product of a bounded number of conjugated elementary plaquette holonomies. Unitarity and telescoping the product give

\[
 \|g_{ij}g_{j\ell}-g_{i\ell}\|
 \le C\sum_{p\subset X}\|v(\partial p)-I\|.
 \tag{BR.6}
\]

Here X is one fixed halo containing the three chosen paths and a fixed plaquette filling. Its size is independent of the lattice volume. Equivalently, a coarse axial gauge on this fixed box makes every relevant `g_ij` differ from I by `Cδ_X`. This gauge is used to prove bounds; it is not part of the definition of the reference field.

On the direct sum of one copy of `C^N` per current vertex, set

\[
 P_{ij}(x)=w_i(x)g_{ij}(v)w_j(x).
 \tag{BR.7}
\]

Only a uniformly bounded number of rows and columns is active at any point. Thus all following matrix operations are finite local operations even though it is convenient to write a single ambient direct sum. The blocks outside that local set vanish identically.

For real data, `P*=P`. Formula (BR.6) and `Σw_ℓ²=1` give

\[
 (P^2-P)_{ij}
 =w_i\sum_\ell w_\ell^2
       (g_{i\ell}g_{\ell j}-g_{ij})w_j,
 \qquad
 \|\partial_x^a(P^2-P)\|\le C_a\delta_X.
 \tag{BR.8}
\]

In a fixed local coarse axial gauge, `P` is `C^a`-close by `C_aδ_X` to
`P_flat=ww^T⊗I_N`, a rank-N projection. Consequently its spectrum has N eigenvalues near one and all the others near zero. For a sufficiently small fixed ε, define

\[
 \Pi(x)=\frac{1}{2\pi i}
     \oint_{|z-1|=1/4}(z-P(x))^{-1}\,dz.
 \tag{BR.9}
\]

The contour lies uniformly in the resolvent set. `Π` is a rank-N orthogonal projection on real data and an idempotent on the complex domain described below. It has the same fixed raw footprint as P. In particular this is not an inversion of a spatial lattice operator: inactive rows contribute only the zero spectral subspace and have no effect on the contour integral. Smooth dependence on x across a change in the active indices follows from the smooth vanishing of the weights.

If the local transports are exactly flat, write `g_ij=g_i g_j^{-1}` and `W_i=w_i g_i`. Then

\[
 P=\Pi=WW^*,\qquad W^*W=I,\qquad W^*dW=0.
 \tag{BR.10}
\]

The induced connection is flat on these local flat data. This exact cancellation, rather than a bound on `dP` alone, is what supplies the small curvature.

## 4. Local frames without division by a vanishing weight

For x in `O_i`, define the column and row

\[
 (V_i)_j=w_j g_{ji},\qquad (L_i)_j=w_j g_{ij},
 \qquad M_i=L_i\Pi V_i.
 \tag{BR.11}
\]

All the required paths remain in one fixed halo. At flat data, `V_i=Wg_i^{-1}`, `L_i=g_iW*`, and `M_i=I`. The preceding local comparison gives
`||M_i−I||_{C^a}≤C_aδ_X`. Define the fixed analytic inverse square root near I and set

\[
 S_i=\Pi V_i M_i^{-1/2},\qquad
 S_i^\vee=M_i^{-1/2}L_i\Pi.
 \tag{BR.12}
\]

For real SU data the dual is the Hermitian adjoint. On complex SL data it is the explicitly displayed analytic row, not a nonholomorphic adjoint. The identities

\[
 S_i^\vee S_i=I,\qquad S_iS_i^\vee=\Pi
 \tag{BR.13}
\]

follow from `Π²=Π` and rank N. These formulas remain valid where `w_i=0`; no quotient by `w_i` is used. On an overlap put

\[
 t_{ij}=S_i^\vee S_j.
 \tag{BR.14}
\]

Then `S_j=S_i t_ij`, `t_ij t_jℓ=t_iℓ`, and `t_ji=t_ij^{-1}` exactly. The transitions are unitary for real data. Locally they differ from the SU transports `g_ij` by `Cδ_X`, so

\[
 |\det t_{ij}-1|\le C\delta_X.
 \tag{BR.15}
\]

This determinant estimate is invariant under coarse SU gauge transformations, and is uniform even when an individual weight approaches zero.

## 5. Exact SU reduction and its connection

Use the logarithm near one to define

\[
 \lambda_{ij}=\log\det t_{ij}.
 \tag{BR.16}
\]

The determinant cocycle is exact. Because all three logarithms on a triple overlap have uniformly small modulus, there is no nonzero `2πi` ambiguity, and

\[
 \lambda_{ij}+\lambda_{j\ell}=\lambda_{i\ell}.
 \tag{BR.17}
\]

Set

\[
 \theta_i=\sum_j\psi_j\lambda_{ij},\qquad
 \theta_i-\theta_\ell=\lambda_{i\ell},\qquad
 \widehat S_i=S_i e^{\theta_i/N}.
 \tag{BR.18}
\]

Only active j enter the sum. Smooth vanishing of `ψ_j` and the uniform frame formulas make the expression smooth at chart boundaries. The new transitions

\[
 \widehat t_{ij}=e^{-\theta_i/N}t_{ij}e^{\theta_j/N}
 \tag{BR.19}
\]

have determinant exactly one. On real data they belong to SU(N). This supplies an SU reduction of the constructed rank-N bundle; it does not assert that the bundle itself is trivial.

The Grassmannian connection has forms `A_i=S_i^∨dS_i`. In the new frames these are `A_i+(dθ_i/N)I`. Their traces agree on overlaps, since the new transitions have determinant one. Denote this global one-form by α and subtract `αI/N`. In the frames `Ŝ_i` the resulting connection is simply

\[
 a_i=A_i-\frac{\operatorname{tr}A_i}{N}I.
 \tag{BR.20}
\]

It is anti-Hermitian and traceless on real data, and obeys the connection transformation law with the exact SU transitions (BR.19). In a local coarse axial gauge the flat comparison (BR.10) yields

\[
 \|a_i\|_{C^q}\le C_q\delta_X,
 \qquad \|F_a\|_{C^q,\mathrm{cov}}\le C_q\delta_X
 \tag{BR.21}
\]

for each required fixed q. The same bounds hold in any smooth local frame after the corresponding covariant interpretation. All constants involve a fixed current patch, not a fine rank.

## 6. Exact coarse edges and fine regularity

Along an actual current edge `(i,j)`, only `w_i=a` and `w_j=b` are nonzero, with `a²+b²=1`. There

\[
 P=\Pi=
 \begin{pmatrix}a^2I&abv_{ij}\\abv_{ij}^{-1}&b^2I\end{pmatrix},
 \qquad
 S_i=\binom{aI}{bv_{ij}^{-1}},\quad S_j=S_i v_{ij}.
 \tag{BR.22}
\]

Its tangent connection is `S_i* dS_i=(a da+b db)I=0`. The only active determinant transition is `det v_ij=1`; hence the restrictions of `θ_i,θ_j` and their tangent derivatives vanish. The SU correction does not change this tangent connection. At a current vertex i the canonical frame is the fixed inclusion `e_i`. The transport from j to i in those vertex frames is therefore exactly `v_ij`, which is the source convention `U(i,j)→u(i)U(i,j)u(j)^{-1}`.

Define each fine link as this connection's transport from its final endpoint to its initial endpoint, in the canonical frames `Ŝ_{i(x)}(x)`. The product along a subdivided edge is the original edge transport by composition. Locality is immediate: the ODE along a fine segment of length at most one uses only the fixed union of the raw footprints met by that segment. Its solution is analytic in those finitely many raw variables.

The holonomy around a fine square is `I+O(η² sup|F|)`. The covariant difference of neighboring such holonomies is `O(η³)` times a fixed bound on F and its first covariant derivative. These estimates can be proved directly by writing parallel transport in a smooth local frame on the square and its neighbor, differentiating the defining ODE, and integrating the curvature identity. Equation (BR.21) proves (BR.2), including the higher fixed differences. Canonical discrete frames may jump between charts; holonomy and covariant comparison remove that change exactly. It creates no curvature error.

At zero plaquette curvature the construction is locally flat and gives zero in these estimates. Consequently the bound is in the actual local defect `δ_X`, not merely the chosen ceiling ε. For example, with the fixed fundamental-trace normalization and `E_X=βΣ_{p⊂X}[N−Re Tr v(∂p)]`,

\[
 \beta\eta^{-4}
  [N-\operatorname{ReTr}U_{\rm ref}(\partial p)]
 \le C E_X.
 \tag{BR.23}
\]

The source-normalized Wilson force satisfies the analogous local square bound. This is a classical reference estimate, not a bound for all the fluctuations of a transported microscopic mark.

## 7. Nonlinear averages: a uniform elementary recurrence

Let `A_j=Μ^j U_ref` and `ℓ_j=L^jη`. CMP98 (53), obtained by iterating its Proposition 1, gives

\[
 \|A_j(\partial p)-I\|\le C\varepsilon\ell_j^2,
 \qquad 0\le j\le k.
 \tag{BR.24}
\]

The initial coefficient in this estimate is the fixed constant in (BR.2); choose ε small enough for the cited averaging theorem with that coefficient. The one-step definition (42) compares each averaging contour with the central straight L-bond path. Their closed difference is filled by at most a fixed number, depending on L, of j-scale plaquettes. The principal logarithms are therefore uniformly near zero, and

\[
 \|A_{j+1}(c)-A_j(\hbox{central straight path }c)\|
       \le C_L\varepsilon\ell_{j+1}^2.
 \tag{BR.25}
\]

Let `T_j(c)` be the original connection's straight transport along the same `ℓ_j` edge and put `e_j=sup_c||A_j(c)−T_j(c)||`. Real unitarity bounds a difference of products of L links by L times their largest difference. Thus

\[
 e_{j+1}\le L e_j+C_L\varepsilon\ell_{j+1}^2,
 \qquad e_0=0.
 \tag{BR.26}
\]

Dividing by `ℓ_{j+1}²` gives a contraction factor `L^{-1}`. Hence
`e_j≤C_L ε ℓ_j²` uniformly in j. At the current scale `T_k(c)=v_c` by (BR.22), proving (BR.3). This argument uses the literal nonlinear average; it does not replace that average by straight holonomy.

## 8. Gauge covariance, holomorphy, and the native complex tube

Under a coarse gauge transformation u, every path transport changes as `g_ij→u_i g_ij u_j^{-1}`. With `D_u=diag(u_i)`, the definitions imply

\[
 P\mapsto D_uPD_u^{-1},\quad
 \Pi\mapsto D_u\Pi D_u^{-1},\quad
 S_i\mapsto D_u S_i u_i^{-1}.
 \tag{BR.27}
\]

The determinant transitions, θ and α are unchanged for SU gauges. Fine transports consequently transform by `u_{i(x)}` at fine vertices x. This is the fixed geometric block lift of the coarse gauge and has no field-selected long path.

For complex data use SL(N,C) matrices on positively oriented links and their inverses on reversed links. All short transports, P, the Riesz contour, the dual frames (BR.11)–(BR.12), the logarithm near one, and the connection ODE are holomorphic. Around any real field satisfying (BR.1), perturbing its finitely many raw links by `exp(iB_e)` with `||B_e||≤δ_*` leaves the required resolvent and Gram spectra separated when `ε+δ_*` is sufficiently small. The constants are uniform in the real center: apply a fixed real coarse axial gauge on the local test patch for the norm estimate, without changing the definition.

There is a further source-domain issue. The canonical block frames need not give a pointwise relative link difference of size `ηδ` between two nearby raw fields. A jump of their frame changes at a block face could give only `O(δ)`. This is removed by an explicit local identification, as follows.

Write `P_0=Π(v)` and `P_1=Π(v')` for their exact projections and set

\[
 T=[P_1P_0+(I-P_1)(I-P_0)]
             [I-(P_1-P_0)^2]^{-1/2}.
 \tag{BR.28}
\]

The inverse square root is taken near I. The algebraic identities
`TP_0=P_1T` and invertibility follow directly; T is unitary when both inputs are real. It is a local analytic function with `T−I=O(δ)` in every fixed spatial derivative. At current vertices both projections equal the same `e_i e_i*`, independently of v, so `T=I` there.

In the two SU frames let
`G_i=Ŝ_i(v')^∨ T Ŝ_i(v)`. On overlaps its determinant is the same, because both transition systems have determinant one. This defines a global scalar function `d=det G_i` close to one, equal to one at current vertices, and local in the same fixed raw halo. Replace the bundle restriction of T by `T d^{-1/N}` using the root near one. The resulting identification respects the SU reductions and still equals identity at every current vertex.

After pulling the second connection back by this identification, the two smooth connection forms differ by `C^q O(δ)` on every fixed local patch. Their fine transports therefore differ by a regular relative field `exp(iη A)` with `A`, its first covariant derivatives, and the fixed higher norms required by the source bounded by `Cδ`. The change from this common smooth frame back to canonical fine frames is a local center-fixed analytic gauge. This proves part 6 of the theorem. It avoids mistaking ordinary raw matrix analyticity for the source's stronger scale-normalized complex domain.

The same comparison and CMP98's uniform averaging/gauge bounds make the mismatch field `log(v [Μ^k U_ref]^{-1})` a local analytic current field on this domain. Its real size is `Cε` by (BR.3), and its derivatives have the uniform current-scale bounds. All dependence on the two adjacent current averaging blocks is included in its raw footprint.

## 9. Application to the homogeneous variational equations

The fine reference just constructed satisfies CMP102 (14): its curvature and divergence satisfy the required scale factors, and its prescribed-average discrepancy is `Cε`. On a larger fixed current patch the local smooth frame bounds have constants depending on that patch; the source localization parameters are fixed before ε is made small. Thus the regularity conditions used for the propagators also hold. This is exactly why a regular approximate reference suffices.

The actual source equation is now the force-containing equation, not the flat special case. With the notation of CMP102 (111)–(112),

\[
 A_1=-\mathcal GJ(U_{\rm ref})
      -\mathcal G\,\mathcal N_{U_{\rm ref},H}
                         (A_1+H_1B),
 \qquad
 A=A_1+H_1B-HD(A_1+H_1B).
 \tag{BR.29}
\]

Here B is the actual local average mismatch, J is the actual Wilson force, and all nonlinear maps are the source maps. The reference is not declared stationary. The input B and J have size `Cε`, their raw dependence is local, and the source nonlinear derivative is quadratic with the bound (98).

The propagator coefficients in the generalized walks are local functions of `U_ref` on their full source domains. Composing with the construction above enlarges these domains by a fixed current halo and leaves no independent global background slot. Choose the source vanishing collar wider than that halo and the averaging stencil. Modify the same walk family by complex decouplers as in CMP116 (1.6)–(1.11). Its enlarged operator bound is `B_R≤B_0 exp(C log R)` on a fixed disc `|s_Δ|≤R` after its block size is chosen.

For fixed R, choose ε small enough that `C B_R ε` lies in the source nonlinear ball and `C B_R^2 ε<1/2`. Equation (BR.29), together with the exact constraint-linearizing equation, then has the same uniform analytic contraction as CMP102 (116)–(121) and CMP116 (1.13)–(1.18). Its regular relative field is bounded by `C_R ε`. At `s=1` it gives the actual constrained minimal orbit. At other s it is the analytic continuation of those equations, not a new assertion of exact physical stationarity.

When decouplers outside a set are zero, the modified kernels vanish across its components with the source collars. The local force, mismatch and nonlinear maps have no larger primitive dependence. The component identity therefore holds in raw v variables, including the fixed halo. Applying the same fundamental-theorem expansion used for FC.1 gives genuine connected raw carriers for the relative Landau correction and local gauge-invariant readouts of the homogeneous minimal orbit. One tag is retained per fundamental-theorem carrier; internal walk and fixed-point indices remain inside that analytic coefficient.

For n new source cubes Cauchy costs `(R−1)^{-n}`. The full raw footprint has volume plus tree size at most `C_M(n+1)`. Choose R above the fixed connected-set entropy, choose the source block buffer, then a positive carrier rate κ with
`A_4 exp(κ C_M)/(R−1)<1`, and finally the geometric ceiling ε. This gives a depth- and volume-uniform absolute carrier sum. Fine gauge-invariant plaquette readouts retain their true `η²` curvature normalization. The source's block-local axial conversion can be included with its actual footprint where that representative is needed.

This closes the homogeneous weak-curvature regular-reference obstruction identified after FC.1. It is not yet a proof of the full residual raw density. For that application one must still identify the mixed determining geometry, its bounded freed core, all old Schur/coarea factors and complete cross action in one exact conditional law. Nor does this construction establish the missing incoming microscopic scalar transport budget.

## 10. What was and was not imported

The partition, approximate projection, local frames, SU reduction, exact edge property and Kato comparison in Sections 2–8 are proved here. They are not attributed to an interpolation paper.

The source input begins with:

- CMP98 (1985), (42), (53) and Propositions 1–2: the literal averaging operation and its depth-uniform curvature bound; Propositions 4–5 and (77), (87), (104)–(106): normalized analytic averaging and block gauge maps.
- CMP102 (1985), p.280 (14); (98), (111)–(121): admission of a regular approximate reference and the actual force-containing variational contraction; Section G and Proposition 9: analytic physical reconstruction.
- CMP99 (1985), generalized random-walk propagators and their localized background dependence, as used explicitly in CMP116 (1.6)–(1.11).
- CMP116 (1988), (1.9)–(1.18): exact component separation and enlarged complex decouplers for the local nonlinear equations.

Any use beyond the homogeneous scope must check those source hypotheses on its actual determining geometry. Neither regularity nor a local reference alone is a replacement for that check.
