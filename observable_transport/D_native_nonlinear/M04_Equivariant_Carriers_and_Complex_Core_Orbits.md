# Equivariant physical carriers and the gauge-orbit continuation of real core integrals

This note supplies a concrete representation theorem for the actual finite-depth coefficient families. Complete scalar carriers can be made gauge invariant individually, with no enlargement of their raw support and no loss of their analytic carrier norm. The construction also applies to the background angles and Gram factors from which the fixed-target frames and the common Gaussian family are built. It permits a gauge chosen on a larger box to be used to estimate one invariant scalar carrier without assigning that box as its support.

A second result removes an arbitrary finite product of block-constant gauges from a **complete** core integral before taking complex absolute values. Its definition keeps the real core domain fixed and continues the entire transformed integrand. It is not a complex characteristic function. This disposes of a possible accumulation of pure-gauge matrix norms, but does not provide the missing all-depth transverse coefficient tube or the separate physical-origin velocity bounds.

The applications below are to the already constructed homogeneous families CA/NC/TC/TR/TS and the smooth marked family SW/PJ. Their stated fixed-depth constants remain fixed-depth constants.

## 1. Complete supports and the real gauge-orbit tube

Let the retained lattice have oriented positive links e with endpoints e_- and e_+. Write

\[
 U^g_e=g(e_-)U_eg(e_+)^{-1},\qquad
 (U^h)^g=U^{gh},\qquad
 \mathcal G=\prod_x SU(N).
 \tag{EC.1}
\]

When a retained gauge acts on an earlier layer, use its actual block-constant lift. Every intermediate target, force, reference, exceptional-coordinate input and independent fluctuation coordinate is transformed at the same time. A free Lie-algebra coordinate transforms by the adjoint map at its source endpoint. The independent-coordinate list contains complete Lie-algebra fibers.

A carrier X includes the storage cells of every determining raw link and every input/output index of a tensor coefficient. Its *gauge endpoint list* consists of the vertices acting on those data. This is a deterministic incidence list belonging to the same full footprint; it is not a field-dependent path or an enclosing box. If two nominal components share such an endpoint or a constraint/gauge stencil, merge them before asserting independence.

We use the following domain already supplied by the native construction. At a real regular center V, write each physical perturbation in a relative chart, for example

\[
 U_e=\exp(A_e)V_e,\qquad \|A\|_{\rm phys}<r.
 \tag{EC.2}
\]

Take the union of these charts over the admitted real centers and all their real gauge transforms, keeping the same physical radius and all prescribed analytic buffers. Denote this union, with its complete simultaneous input data, by \(\mathfrak D_r\). A real gauge maps (EC.2) to the chart at \(V^g\), with
\(A_e\mapsto\operatorname{Ad}_{g(e_-)}A_e\). Thus it preserves the physical radius. The assertion concerns small complex perturbations of arbitrary real centers; it does not assert that all real regular fields have one global small-link representative.

Here are the actual source inputs for using this domain.

* CMP116, Lemma 2, printed p.11, states the gauge invariance of each localized native fluctuation coefficient and of both its quadratic and higher parts under simultaneous complex transformations in a neighborhood of **all** real gauge transformations. Its bounds (1.36), (1.39), (1.40), (1.43) are the native bounds on that family.
* CMP116, printed pp.21–22, applies the same statement to the complete component integrals (2.14), including their operators, and extends them constantly along the gauge orbits meeting the native domain.
* The raw reference BR.27–BR.29 is equivariant with the specified block lift. Its local resolvent contours, dual frames, regular bundle identification, force and mismatch have uniform bounds at arbitrary real centers. The fixed geometrical reference rule is transported; it is not replaced by a fresh identity reference after a gauge change.
* The scalar decouplers in CMP116 (1.6)–(1.18), the full local matrix solves, and the fixed-target exceptional equations commute with a fixed gauge transformation. Their local analytic branches are unique. Their absolute estimates use unitary conjugations on real gauge orbits. The fundamental-theorem extraction in these scalar decouplers therefore defines the same complete raw tags on \(\mathfrak D_r\), with the same native bounds.
* At the fixed depths in CA/NC/TC, the remaining raw substitutions, conditional integrations and determinant branches retain all their inputs in one family. Real changes of free variables are orthogonal and preserve the fixed product balls. Saved Q domains require simultaneous transport of their full real references; that case is treated in Section 6.

These facts establish orbit-uniform admission of the **existing fixed-depth** raw families. In the small-link family PJ, the corresponding domain is the union of the real gauge images of its fixed physical chart, with the entire raw reference family transformed. It is not a product ball about the identity after an arbitrary gauge transformation.

## 2. Scalar projection with unchanged support

Let \(f_{n,X}(U_X)\) be a complete scalar coefficient, anchored at n, holomorphic on the projection of \(\mathfrak D_r\) onto its actual input list. All external source parameters and all declared independent coefficient parameters may be included. They are kept fixed in the following integral. Write

\[
 \|f\|_{\kappa,r}
 =\sup_n\sum_{X\ni n}e^{\kappa n(X)}
        \sup_{U\in\mathfrak D_r}|f_{n,X}(U_X)|.
 \tag{EC.3}
\]

The same argument applies to unanchored action coefficients and to the common nonnegative majorants of the tagged construction. Define normalized Haar projection by

\[
 (\mathcal P f_{n,X})(U)
   =\int_{\mathcal G}f_{n,X}(U^g)\,dg
   =\int_{\mathcal G_X}f_{n,X}(U^g)\,dg_X,
 \tag{EC.4}
\]

where \(\mathcal G_X\) contains only the finite gauge endpoint list. The second equality integrates out all irrelevant factors, each of total mass one.

### Theorem EC.1 — invariant scalar carriers

The coefficients \(\widehat f_{n,X}=\mathcal P f_{n,X}\) have the following properties.

1. Each coefficient depends only on the original raw determining inputs in X. Its anchor, connected carrier, incidence list and source labels are unchanged.
2. It is holomorphic on the same orbit-saturated tube and invariant under every real gauge transformation. Its invariance continues to complex gauges in the continuation of that identity from the real group. On a declared source gauge-orbit family it therefore has the same constant orbit continuation.
3. The analytic coefficient norm is contractive:

\[
 \|\widehat f\|_{\kappa,r}\le\|f\|_{\kappa,r}.
 \tag{EC.5}
\]

4. If the exact normally convergent sum \(F_n=\sum_X f_{n,X}\) is gauge invariant, then

\[
 F_n=\sum_X\widehat f_{n,X}
 \tag{EC.6}
\]

on the physical domain and on its given holomorphic continuation. Source derivatives may be taken before or after this operation on the same source discs.
5. Common component restriction identities are preserved. In particular the projection of a coefficient whose complete footprint lies in H is identical whether that coefficient is constructed in H or in a larger containing component with the same full input data. The operation introduces no gauge-volume factor, no rank factor, and no dependence on the number of preceding scales.

**Proof.** Only link values in the original input list enter \(f_{n,X}(U^g)\); the additional integration variables are fixed compact parameters and introduce no outside raw argument. This proves the support assertion. For a fixed real h, the convention (EC.1) gives

\[
 (\mathcal P f_{n,X})(U^h)
    =\int f_{n,X}(U^{gh})\,dg
    =(\mathcal P f_{n,X})(U)
 \tag{EC.7}
\]

by right invariance of Haar measure. The orbit-saturated tube is stable under this real action, so the integral of the coefficient supremum gives (EC.5). Uniform boundedness on compact subsets permits Morera's theorem, or differentiated Cauchy integrals, to pass through the compact Haar integral; hence the result is holomorphic. Analyticity of the action and the identity theorem extend (EC.7) to complex gauges in a neighborhood of the real compact group and then along that continued identity. A constant continuation to its orbit is well-defined wherever the original family supplies compatible orbit germs; in the source applications the complete functions have the continuation described in CMP102 (181) and CMP116 pp.21–22. The elementary Haar theorem by itself is not a gluing theorem for unrelated analytic branches on disconnected orbit intersections.

Normal convergence and normalized Haar measure permit interchange of the sum and integral. If F_n is invariant, \(\mathcal P F_n=F_n\), proving (EC.6). The same argument applies to a source derivative on a smaller fixed source disc. Finally, a component identity is an equality between the same local coefficient functions on their complete argument lists. Apply the same finite endpoint Haar integral to each side. Irrelevant endpoint factors again have mass one, so adding unused vertices or a larger containing component changes nothing. No estimate involves the number of gauge vertices. \(\square\)

There is a necessary distinction about products. For two complete factors with disjoint gauge endpoint lists, the product Haar measure factors, and

\[
 \mathcal P(f_X f_Y)=(\mathcal P f_X)(\mathcal P f_Y).
 \tag{EC.8}
\]

For overlapping lists this equality need not hold. Thus one may project the complete scalar action coefficients and retain their unchanged invariant total, or project an already complete connected scalar primitive. One must not independently project arbitrary overlapping factors in a product and call the resulting product the old integrand. An exact component partition function, its numerator and its denominator retain their common construction. This is also why Section 4 projects the Gram map before building the Gaussian family.

If every complete component sum \(F_H\) is invariant, its value is unchanged individually, since \(\mathcal P F_H=F_H\). If the original auxiliary coefficient restriction was not itself invariant, the projection defines a new, restriction-consistent auxiliary representation of the unchanged physical sum; it does not assert numerical equality of the two auxiliary restrictions.

For a hard-Q primitive with saved real core data R, holomorphy in this statement applies only to its already admitted analytic coefficient slots and outside parameters. Its compact Haar average also transforms R simultaneously. Support, real value bounds and existing real first-jet envelopes still obey the same projection argument, but that operation does not turn the raw R-dependence of intersecting sharp domains into a holomorphic function.

### Corollary EC.2 — estimating gauges do not enlarge a carrier

Let g(U) be any real gauge choice on a finite neighborhood containing the full input list of X, and extend it arbitrarily to the lattice. Then

\[
 \widehat f_{n,X}(U)=\widehat f_{n,X}(U^{g(U)}).
 \tag{EC.9}
\]

Consequently a radial/tree gauge on a bounding box may be used to estimate this coefficient. The coefficient on the left still has its original raw support X, even if the chosen estimating gauge reads more links. The estimate must include the actual size of the gauged links and the range of its admitted chart. In particular a long or winding carrier does not acquire a uniform small-link estimate merely from (EC.9).

**Proof.** Apply (EC.7) pointwise at each fixed U. No differentiation or analytic continuation of the gauge choice is required for this identity. The original left side gives the support statement. \(\square\)

## 3. Raw jets and physical current labels

Choose an orthonormal real basis \(T_a\) of \(\mathfrak{su}(N)\), with \(d_G=N^2-1\). A normalized raw derivative at retained scale k is

\[
 D_{e,a}f(U)
   =\left.\frac d{dt}
        f(\ldots,e^{t g_kT_a}U_e,\ldots)\right|_{t=0}.
 \tag{EC.10}
\]

For a fixed real g,

\[
 D_{e,a}[f(U^g)]
   =\sum_b O_{ba}(g(e_-))(D_{e,b}f)(U^g),
 \qquad O(g)=\operatorname{Ad}_g\in O(d_G).
 \tag{EC.11}
\]

No differentiated gauge appears in this formula: the integration parameter g in (EC.4) is fixed while U varies.

### Theorem EC.3 — coupling and summed-direction bounds survive

For any fixed q, let the q-jet norm use the sum of absolute values over ordered normalized raw coordinate directions and the same coefficient weight as (EC.3). Then

\[
 \sup_U\sum_{d_1,\ldots,d_q}
  |D_{d_1}\cdots D_{d_q}\widehat f_{n,X}(U)|
 \le d_G^{q/2}
 \sup_U\sum_{d_1,\ldots,d_q}
  |D_{d_1}\cdots D_{d_q}f_{n,X}(U)|.
 \tag{EC.12}
\]

The same statement holds after the carrier sum, and with a gauge-invariant regulator dividing the values or jets. In particular every explicit factor \(g_k^q\) in a physical Cauchy estimate is retained. The constant depends on the fixed colour dimension and q, not on the carrier's volume or its ancestry.

**Proof.** Every row or column of an orthogonal \(d_G\times d_G\) matrix has absolute sum at most \(\sqrt{d_G}\). Differentiate the Haar integral, apply (EC.11) q times, take absolute values and sum the coordinate indices. At a fixed U and g all the derivatives on the right are evaluated at the same \(U^g\); hence the supremum of their sum bounds that integral. This proves (EC.12). A gauge-invariant regulator has the same value at U and \(U^g\) and can be carried through the argument. \(\square\)

For an endpoint path current, one must retain its actual first-jet certificate. A sum of independent path suprema cannot in general be bounded by moving all the suprema outside a sum. Two sufficient bounds already used in the finite-depth construction are available here:

* If \(|D_{e,a}f_{n,X}(U)|\le b_{n,X;e,a}\) on the full buffered orbit tube, with a common summable nonnegative envelope, (EC.11) gives another such envelope with only the fixed colour factor. It bounds every admitted finite path by its length times that envelope.
* Starting from the holomorphic value norm (EC.3) with physical radius r, Cauchy on a smaller physical tube gives \(C g_k/r\) times the coefficient envelope per direction. The full input list has at most \(C n(X)\) directions. A strict carrier-rate loss pays this fixed incidence polynomial, and the bound is uniform on the entire short path.

These are the deterministic envelope or buffered Cauchy arguments of CA/TC/TR. They yield an actual common path representation after projection. No equality of arbitrary differently ordered path-supremum norms is asserted.

The projection can also retain the existing origin labels. Suppose \(j_{n,X}^{\ell}(U;H)\) is a labelled first-jet coefficient, linear in the raw direction H, and

\[
 df_{n,X}(U)[H]=\sum_\ell j_{n,X}^{\ell}(U;H).
 \tag{EC.13}
\]

Define

\[
 \widehat j_{n,X}^{\ell}(U;H)
   =\int j_{n,X}^{\ell}(U^g;g_*H)\,dg.
 \tag{EC.14}
\]

Then \(d\widehat f_{n,X}=\sum_\ell\widehat j_{n,X}^{\ell}\), and the absolute norm bound applies **for each label separately**. If the exact full labelled current is covariant under a fixed real gauge, the full current with that label is unchanged. The physical insertion-at-fixed-free-variable and kernel-at-fixed-test labels have this fixed-gauge covariance by the same constant, measure-preserving change of free coordinates; boundary labels also transform together with their real domains. Their distinct labels are retained.

This result concerns a fixed gauge in (EC.11). It does not justify deleting the derivative of a field-dependent ancestral transport. That distinction is made explicit in Section 7.

## 4. Equivariant Gram restrictions and one Gaussian family

For matrix coefficients use the same full footprints, including their input and output storage fibers. Let \(T_{\rm in}(g)\), \(T_{\rm out}(g)\) be their pointwise orthogonal real gauge representations. For a covariant matrix map

\[
 B(U^g)=T_{\rm out}(g)B(U)T_{\rm in}(g)^{-1},
 \tag{EC.15}
\]

define

\[
 \widehat B_X(U)
   =\int T_{\rm out}(g)^{-1}B_X(U^g)T_{\rm in}(g)\,dg.
 \tag{EC.16}
\]

The same Haar substitution proves (EC.15) for each \(\widehat B_X\). In the row/column carrier norm with the operator norm on each fixed colour block, the integral is contractive. If a scalar-entry norm is used, changing to and from that block norm costs only a fixed group-dependent factor. It does not cost the matrix rank. Holomorphy, complete support, raw jet bounds and component consistency follow exactly as for scalar coefficients.

Take the actual complete real precision K, including its constraint-force correction and full nonlinear averaged soft sampler. At a fixed depth its actual gap is m. Choose \(0<\sigma<m\), and use the supported PR functional calculus to obtain

\[
 B=(K-\sigma I)^{1/2}=\sum_X B_X.
 \tag{EC.17}
\]

Here the analytic transpose continuation agrees with the real adjoint. Gauge covariance of K and uniqueness of its analytic positive-root branch give (EC.15) for B. Thus \(\sum_X\widehat B_X=B\). For a component region H put

\[
 \widehat B^H=\sum_{X\subset H}\widehat B_X,\qquad
 \widehat K^H=\sigma I+(\widehat B^H)^{\mathsf T}\widehat B^H.
 \tag{EC.18}
\]

For every real input,

\[
 \sigma I\le\widehat K^H\le(\sigma+b_0^2)I
 \tag{EC.19}
\]

in the block norm convention, with b_0 the common Gram bound. At the full physical restriction, \(\widehat K=K\) exactly. The Gram product is assigned its true carrier \(X\cup Y\); a nonzero product has a common summed index and hence a connected union. Consequently

\[
 \widehat K^H=\sigma I+\sum_{Z\subset H}\widehat A_Z
 \tag{EC.20}
\]

is the same exact restriction identity as GM.5. There is no assertion that Haar averaging commutes with squaring B; the squaring in (EC.18) is the definition of the new auxiliary Gram family, and the unchanged full physical B proves the full physical equality.

Apply the same PR construction to all matrices (EC.18), with common truncation sizes, local inverse cubes and tag conventions. GM.1–GM.3 then construct a common covariance, local marginal inverse and determinant branch. Their hypotheses remain valid by (EC.19), the contractive Gram bound and (EC.20). These derived operations are themselves equivariant: their finite local matrices contain full colour fibers, scalar geometrical cutoffs commute with the gauge representation, and inverses and the analytic functional calculus commute with conjugation. On separated complete components the matrices split into the exact corresponding smaller constructions.

This is one consistent Gaussian family. Neither an inverse nor a determinant is independently Haar averaged. Its local rank cost remains exactly the one in GM.17–GM.18; projection has not removed that cost. A complex outside-parameter radius is whatever the common GM/CA/TC construction actually proves. The positivity of real Gram restrictions alone is not a proof of a depth-independent transverse complex radius.

## 5. Background angles and exact fixed-target core frames

Use the actual independent relative angles in CA.3–CA.4,

\[
 a_e(W)=\frac1i\Log\{H_{*,e}(W)U_{f,e}(W)^{-1}\}
       =\sum_X a_{eX}(W_X).
 \tag{EC.21}
\]

The actual minimum representative \(H_*\) and the face lift \(U_f\) transform by the same specified block lift. The angle therefore transforms by its endpoint adjoint. Its logarithm is the small relative branch; it is not the logarithm of an arbitrary large link. Project each angle coefficient with the covariant version (EC.16), denoting the result by \(\widehat a_{eX}\). Then

\[
 \sum_X\widehat a_{eX}=a_e,\qquad
 \widehat a^{D}_e=\sum_{X\subset D}\widehat a_{eX}
 \tag{EC.22}
\]

has the same tail bound as the original complete family and is exactly equivariant. Restore the exceptional coordinates with the actual target W:

\[
 \widehat H_D(W)=\Xi_W(\widehat a^D(W)).
 \tag{EC.23}
\]

The exceptional equations transform covariantly, and their local small solution is unique. Hence

\[
 \Xi_{W^g}(\operatorname{Ad}_{\widetilde g}a)
       =\Xi_W(a)^{\widetilde g}.
 \tag{EC.24}
\]

This proves exact covariance of the constrained frame, with its prescribed averages unchanged. The same argument applies to the omitted-carrier parameter family. Its core domain is defined from the same full determining stencils and references; its fixed-L collars do not increase under the projection.

If a previous auxiliary restricted frame was not equivariant termwise, (EC.23) is a new choice of restricted frame. The physical s=1 background is unchanged by (EC.22). The exact constrained coordinate change CA.11–CA.13 is replayed with this frame, including its Jacobian, so that the physical integral is unchanged. The finite-depth tail admission is unchanged because (EC.22) does not increase the coefficient tails. This does not assert that the new auxiliary frame is a critical field, nor that an arbitrary-depth common registry has thereby been constructed.

## 6. A complete real core integral on a complex gauge orbit

Let R denote the **full** real core data: targets, local Q comparison references, preceding saved inputs, free-coordinate lists and gauge/constraint collars. Let \(D_R\) be its real integration domain, including the literal Q tests and any fixed P balls. For a real retained gauge g, lifted block constantly at each required earlier layer, the actual source change of variables gives

\[
 D_{R^g}=T_gD_R.
 \tag{EC.25}
\]

This is the real simultaneous-domain covariance of BG.26 and the source characteristic functions. A Q test with its reference held fixed does not satisfy this identity by itself.

Let \(\psi(z;\lambda)\,dz\) be a complete analytic component density with its mark, Jacobians, relative Gaussian normalization and every other retained coefficient, written before insertion of \(1_{D_R}\). Here \(\lambda\) includes its complete analytic input list. The same real gauge change gives

\[
 \psi(T_gz;\lambda^g)\det T_g=\psi(z;\lambda).
 \tag{EC.26}
\]

For the adjoint action on complete independent colour fibers, \(\det T_g=1\). Its complexification also has determinant one and is orthogonal for the complex-bilinear trace form. In particular the precision and an invariant fiber marginal transform together:

\[
 K(\lambda^g)=T_gK(\lambda)T_g^{\mathsf T},\qquad
 C_I(\lambda^g)=T_{g,I}C_I(\lambda)T_{g,I}^{\mathsf T}.
 \tag{EC.27}
\]

The determinant is unchanged, and its branch is the same branch fixed by the positive real reference. All statements concern the complete common family, not unrelated continuations of its pieces.

### Theorem EC.4 — exact cancellation of the pure gauge part

For any finite product v of complexified retained gauges for which the source orbit continuation is defined, set

\[
 I_R^{\rm orb}(v,\lambda)
  :=\int_{D_R}\psi(T_vz;\lambda^v)\det T_v\,dz.
 \tag{EC.28}
\]

This is an analytic gauge-orbit continuation of the actual transformed real core integral, and

\[
 I_R^{\rm orb}(v,\lambda)
    =\int_{D_R}\psi(z;\lambda)\,dz.
 \tag{EC.29}
\]

Thus its bound has no factor involving \(\|T_v\|\), the number of gauges in v, or a fresh Gaussian rank store. The same statement holds for a normalized complete component ratio when its numerator and denominator use the identical family and its denominator is nonzero on the already established analytic domain.

**Proof.** For real v, change variables \(z'=T_vz\) and use (EC.25)–(EC.26). This gives exactly the actual core integral with data \(R^v\). For the analytic integrand, (EC.26) continues to a complex neighborhood of the real compact group by the identity theorem. Equivalently one may continue one real Lie-algebra direction at a time; its complexification generates the connected complex group. CMP102 (181) and CMP116 pp.21–22 provide the compatible orbit continuation of the underlying source functions. On that continuation (EC.26) remains an algebraic identity. Substitute it into (EC.28) **before** estimating absolute values. The integrand is then precisely the original one, proving (EC.29) and its analytic dependence wherever the original integral is analytic. Finite products introduce no additional factor. Numerator and denominator obey the same identity separately, proving the ratio statement on its existing nonzero domain. \(\square\)

For an unbounded real domain, (EC.28) is understood through this pulled-back, algebraically equal integrand, or first with the fixed real caps already present in the source coefficient construction. It is not a claim that a nonaccretive transformed quadratic form is absolutely integrable on the untransformed real contour. If external transverse parameters s already have a fixed-domain holomorphic family and a common integrable majorant, the same argument is joint in (s,v). It supplies the gauge-orbit part of that family; it does not create its transverse s-domain.

For complex v, (EC.28) is **not** obtained by evaluating a norm-based Q indicator at complex links. The real set \(D_R\) is kept fixed, and all of its transformed references occur through the analytic pullback. This distinction preserves both the literal real Q equality and the fixed-domain analytic meaning.

Applied to a complete invariant carrier from Theorem EC.1, the same identity can delete a field-dependent product of gauges pointwise before taking a coefficient bound. Its raw support then remains the original carrier support. An uncontracted tensor coefficient retains its gauge endpoints, and an incomplete product is not covered by this scalar cancellation.

### 6.1. Why the pure gauge product cannot first be bounded in a raw matrix norm

There is an actual source-background example, extending AF's one-step example. It concerns one first-birth precision and an arbitrary finite number m of later real steps. Use the fixed sufficiently large odd L of AF, a torus large enough for the following blocks to be embedded, and microscopic spacing one for the geometric description. Let the common face lie between the integers

\[
 x_*=(L^{m+1}-1)/2\quad\hbox{and}\quad x_*+1.
\]

For \(1\le j\le m\), choose the j-grid center

\[
 y_j=((L^{m+1}-L^j)/2,0,0,0),
 \qquad
 v_j(y_j)=e^{it_jH},\quad v_j(y)=I\ (y\ne y_j),
 \tag{EC.29a}
\]

where H is a fixed noncentral traceless Hermitian generator. These centers belong to the j-grid but not the (j+1)-grid. The centered j-blocks \(B_j(y_j)\) are nested along their common right face. Let \(u_j\) be the literal block-constant microscopic lift of v_j and define

\[
 F_i=I^{u_i\cdots u_m},\quad V_i=\mathcal M^iF_i
       \quad(1\le i\le m),\qquad
 F_{m+1}=V_{m+1}=I.
 \tag{EC.29b}
\]

Every plaquette is flat. Each \(u_j\) is identity at every (j+1)-center: its supporting j-block is not the one centered at such a vertex. Endpoint covariance of the literal average therefore gives \(\mathcal M V_i=V_{i+1}\). The product in \(F_i\) is constant on i-blocks, so CMP102 (181) gives the exact source representative \(U_i(V_i)=F_i\). These are actual nested critical backgrounds.

At step j remove the real outer product \(u_{j+1}\cdots u_m\), which is block constant on the next blocks. The remaining innovation is the single center-fixed small pure gauge \(I^{v_j}\). AF's literal Q/axial verification applies unchanged: for \(|t_j|\le c\delta_j\), with the same sufficiently small fixed c and the source \(\delta_j/\epsilon_j\) hierarchy, its link discrepancy is strictly inside the Q threshold and its axial cutoff is strictly satisfied. All curvature tests are flat. Thus every supplied finite weak-coupling trajectory gives an actual admitted real box of parameters in (EC.29b); the R partition is summed as in the current operation. No all-depth interacting density induction is needed for this finite background example.

At the first birth, every \(u_j\) is block constant on the first L-block partition. Hence the actual averaged sampler is already canonical, and the complete force-corrected precision satisfies

\[
 K_0(F_1)=T_0(u_1\cdots u_m)K_0(I)
                        T_0(u_1\cdots u_m)^{\mathsf T}.
 \tag{EC.29c}
\]

For real parameters the transpose is the ordinary adjoint; (EC.29c) continues holomorphically in all t_j by the source orbit identity. Take AF.9–AF.10's fixed two Q-null tangential cochains a,b in the adjacent first blocks on the two sides of the common face. Their full independent embeddings are exactly a,b. Their soft cross pairing is zero, while their flat Wilson cross pairing is \(-c_W\), with \(c_W>0\). The first cochain is inside every selected j-block and the second is outside all of them. Thus the matrix between their colour fibers is exactly

\[
 -c_W\operatorname{Ad}_{\exp(iH\sum_jt_j)}.
 \tag{EC.29d}
\]

Choose a root colour of H and put \(t_j=i r_j\), \(r_j\ge0\). The corresponding adjoint eigenvalue has modulus \(\exp(c_H\sum_jr_j)\), for one choice of root sign. Therefore

\[
 \|K_0(F_1)\|_{\rm op}
       \ge c_W\exp\!\left(c_H\sum_{j=1}^m r_j\right).
 \tag{EC.29e}
\]

Consequently independent ancestor-gauge discs whose radii have unbounded sum cannot give a depth-uniform bound on this raw birth matrix. On normalized innovation discs \(t_j=\delta_jz_j\), \(|z_j|\le r\), the exponent is \(c_Hr\sum_j\delta_j\). This last statement is a sum-radii condition; no divergence of that sum is assumed for every trajectory. Summable radii are not ruled out, and the example is not an obstruction to a quotient construction.

In fact the determinant is constant in this example, and the complete scalar core integral is constant by EC.4. The example proves precisely why a generally growing complex adjoint product must be canceled by the complete gauge identity before a raw coefficient norm is taken. It does not contradict the real isometric comparison AP/BG or imply that a gauge-invariant physical scalar has a growing norm.

## 7. The gauge-orbit identity does not merge current origins

Let T(t) be a differentiable real gauge representation, and let

\[
 V_t(z)=\dot T(t)T(t)^{-1}z.
 \tag{EC.30}
\]

In fixed raw coordinates, a simultaneous pure-gauge change gives an insertion \(f_t(z)=f_0(T(t)^{-1}z)\) and density \(p_t(z)=p_0(T(t)^{-1}z)\), with unit Jacobian. Therefore

\[
 \partial_t f_t=-V_t\cdot\nabla f_t,\qquad
 \partial_t p_t=-\operatorname{div}(p_tV_t),\qquad
 \partial_t(p_tf_t)=-\operatorname{div}(p_tf_tV_t).
 \tag{EC.31}
\]

On an invariant domain, the integrated insertion and kernel derivatives can be nonzero with opposite signs. On a moving Q domain the boundary current also participates. Only their complete sum is killed by the simultaneous gauge identity. The sums of their separate absolute norms need not vanish and are not bounded by the absolute norm of that sum.

Consequently EC.14 is a representation theorem for each existing labelled current, and EC.29 is an exact identity for a complete scalar integral. Neither proves the needed uniform bound on \(\dot T T^{-1}\) for every origin in a field-dependent ancestor transport. BG.20 still contains the moving-reference term

\[
 C\,|a|\,|\dot{\bar V}_+|_{\rm local},
 \tag{EC.32}
\]

in addition to \(C|\dot a|\). The summable fixed-base age estimate BG.18 does not alone estimate that term on one terminally varying chronological family.

## 8. Actual application and remaining all-depth work

The exact smooth local mark \(\Phi_n\) of SW.8/PJ.1 is invariant under the retained gauge group by the full three-layer change of variables. Its raw coefficient representation is available on the finite-depth native family and, in PJ, on the fixed physical chart. Section 1 supplies the corresponding real orbit tube with all reference and target slots transformed. Applying EC.1 gives

\[
 \Phi_n=\sum_{X\ni n}\widehat\Phi_{n,X},\qquad
 \widehat\Phi_{n,X}(W^g)=\widehat\Phi_{n,X}(W),
 \tag{EC.33}
\]

with the same analytic carrier bounds. Applying the same physical Cauchy argument to (EC.5) retains the coupling-weighted finite jets of PJ.8 and its spatial-moment bounds. For jet envelopes already uniform on the orbit tube, EC.12 gives the direct fixed-colour bound. An estimating gauge on a box containing X is legitimate by EC.9, while the coefficient itself keeps support X. This is the precise support-preserving input available to the local nonlinear Ward extraction.

The completed physical hard-Q scalar has the same real retained-gauge covariance when all its local Q references and previous cores transform. Its existing fixed-depth primitive coefficient integrals can therefore be treated by EC.4. This statement does not supply high real raw derivatives of intersecting sharp Q boundaries, nor a new all-depth analytic law. The latter issues cannot be inferred from smooth-orbit covariance.

For the common complex/core problem, the new conclusions are definite:

* Termwise scalar invariance can be imposed by an explicit normalized integral without changing the physical scalar, complete support, connectedness, analytic rate, source identity, or fixed-depth component law.
* Covariant background and Gram coefficient choices produce exact fixed-target frames and one compatible local inverse/determinant family. The actual full precision and physical law are unchanged.
* Any finite product of pure block-constant gauges has zero cost in a complete pulled-back scalar core integral. It need not be bounded as a product of complex matrix norms.

What is not supplied is equally specific: one all-depth transverse raw family simultaneously controlling every saved real core, the analytic radii and ranks of its full Gaussian restrictions, moving-base terms such as (EC.32), and every separately retained insertion, kernel and boundary current. CC's grouped carrier contraction and AP/BG's age summability can be used only after that simultaneous family is identified. The present theorem removes a pure-gauge representation cost from that problem; it does not declare M04 or Yang–Mills existence proved.

Primary sources used: Balaban, CMP102 (1985), Section G, (172)–(181), Proposition 9 and (190); CMP109 (1987), (0.11), (2.10), (2.16)–(2.18); CMP116 (1988), (1.6)–(1.18), Lemma 2 on p.11, and the final gauge-orbit discussion on pp.21–22; CMP119 (1988), the simultaneous characteristic-function transformation following (1.17) and the local Q reconstruction of (3.7)–(3.19). Mathematical prerequisites: BR, PR, GM, CA, NC, TC, TR, TS, SW, PJ and BG. All support, source and target conventions in those inputs are retained.
