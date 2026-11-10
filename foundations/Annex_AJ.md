# Joined reconstruction, fine-collar currents and the remaining boundary application

**Annex AJ.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


The full reconstructed-current estimate (BM.24) requires a source-domain pullback. The following metric comparison concerns the localized operator on its actual geometry.

### 1. Source facts used

See CMP119, pp.255–257 and 261. In particular, (2.14) splices the original determining set in the interior to a newly constructed local determining set in the boundary collar. The reconstruction in (2.35) is written using the determining tuple

\[
 \mathfrak B_p(X)\cup\{\Gamma_i\}_{i<p}
 \tag{RT.1}
\]

and the data are the actual averages \(M^\bullet(U)\). The output restrictions (2.35)–(2.37) are imposed on the displayed intersections with \(X\); no interior restriction is printed there. By contrast, the simpler regular reconstruction condition CMP109 (1.16) explicitly uses \(X^{-2}\). The source-localization statement in LFR II, printed p.373, concerns a fixed underlying variational problem and its boundary data.

These facts have different roles. The fixed-geometry localization statement does not identify the data of a separately reconstructed minimizer, and the interior restriction from the regular case is not inserted into the multiscale definition without a proof.

### 2. A metric lemma for the actual boundary splice

Let an admitted determining geometry have local mesh function \(h(x)\), constant on the interiors of its determining blocks. Let \(X\) be an admitted source localization domain. On a patch of \(\partial X\) lying in original layer \(r\), apply the source construction (2.14): keep the original determining set in the interior and use the local determining set of depth \(r\) in its proper-scale collar. Let \(\widehat h(x)\) be the resulting local mesh.

#### Lemma RT.1 — localization refines the boundary mesh

On such a patch, away from the conventions that assign points lying on block boundaries,

\[
 \widehat h(x)\le h(x).
 \tag{RT.2}
\]

Consequently the path distance defined by integrating inverse local mesh satisfies

\[
 \widehat d(x,y)\ge d_\Omega(x,y)
 \tag{RT.3}
\]

when both sides use the same physical endpoint convention and the left-hand paths are restricted to the localization domain. Passing to the source's determining-block centers changes only fixed endpoint constants. The analogous statement holds for the finitely many boundary-layer patches in the generalized source construction.

**Proof.** In the interior the determining sets coincide, so the mesh functions are equal. In the collar, the source hypothesis puts the original boundary in layer \(r\), at the stated distance from every original layer boundary lying inside \(X\). The original local mesh there is \(h_r\). The new minimal local determining set has levels only through \(r\), so all of its local meshes are at most \(h_r\). This proves (RT.2). Every common physical path therefore has at least as large an integral of inverse mesh for the new geometry. The infimum over paths restricted to \(X\) is no smaller than the unrestricted old infimum, proving (RT.3). In the multiple-patch version the same pointwise argument is applied on each source proper-scale patch. Endpoint assignment changes distances over only fixed proper-scale collars. \(\square\)

This argument uses the actual boundary splice. It does **not** replace (2.14) by an intersection of arbitrary nested sets. Such an intersection generally changes the interior, whereas the source operation leaves the original determining set there.

#### The extra identification for (RT.1)

For comparison, truncating the original determining sequence at \(p\) produces

\[
 \mathfrak B^{\langle p\rangle}
 =\bigcup_{i<p}\Gamma_i\ \cup\ \Omega_p^{(p)}.
 \tag{RT.4}
\]

Its mesh is \(\min\{h(x),h_p\}\), with the usual block-center conventions. If the tuple (RT.1), with its prescribed data and collars, is identified with the source localization of (RT.4), Lemma RT.1 gives

\[
 h_{p,X}(x)\le\min\{h(x),h_p\}.
 \tag{RT.5}
\]

The conditional statement is useful, but (RT.5) is not asserted for (RT.1) solely from its notation. The joining symbol is used in different argument orders in the sources, and a union with the incomplete family \(\{\Gamma_i\}_{i<p}\) must specify how the remaining coarse determining data and boundary blocks are supplied. The data remain \(M^\bullet(U)\), regardless of how the geometry is described.

### 3. Fixed-lattice dilation and genuine reconstruction

For a fixed bond graph with the same link matrices, a change of units \(x'=\lambda x\), \(\eta'=\lambda\eta\) gives

\[
 F_{\eta'}=\lambda^{-2}F_\eta,
 \qquad J_{\eta'}=\lambda^{-3}J_\eta.
 \tag{RT.6}
\]

The raw plaquette variable \(dU\) is unchanged. These are direct substitutions in \(F_\eta=\eta^{-2}\pi\operatorname{Im}dU\) and \(J_\eta=D_{\eta,U}^*F_\eta\). They do not compare two different constrained projectors or variational problems.

In a reconstruction indexed by \(p\), the exact weights from CMP119 are

\[
 w_F(n,p)=L^{-2p}(L^nL^{-p})^{-2}=L^{-2n},
 \tag{RT.7}
\]

\[
 w_J(n,p)=L^{n-\min(p,n)}(L^nL^{-p})^{-3}
 =\begin{cases}
 L^{3(p-n)},&n\le p,\\
 L^{-2(n-p)},&n>p.
 \end{cases}
 \tag{RT.8}
\]

Thus the smoother case \(n>p\) asks for a two-power gain in the reconstructed current. It is not obtained by treating all output currents as having the same unweighted supremum norm. Nor is the change in units (RT.6) an identity between the original and reconstructed minimizers.

### 4. What the local two-power gain proves, and where it loses a power

Take a local determining block of mesh \(h_s\le h_n\) inside an original smooth layer \(n\). Suppose the prepared input variation satisfies the already proved original-geometry bounds

\[
 |\delta A|\le u_nh_n^{-1},\qquad
 |\nabla\delta A|\le u_nh_n^{-2}.
 \tag{RT.9}
\]

Lemma BM.2 gives the response of its actual gauged determining average:

\[
 |\delta B_s|\le C u_n(h_s/h_n)^2.
 \tag{RT.10}
\]

For a generic application of the minimizing-map derivative kernel, the normalized curvature and current output rows have scales \(h_s^{-2}\) and \(h_s^{-3}\), respectively. Thus (RT.10) gives the curvature estimate

\[
 h_s^{-2}|\delta B_s|\le C u_nh_n^{-2},
 \tag{RT.11}
\]

with no loss when the determining collar is finer than the original layer. For the current it gives only

\[
 h_s^{-3}|\delta B_s|\le C u_nh_s^{-1}h_n^{-2}.
 \tag{RT.12}
\]

The desired current scale in unrescaled units is

\[
 u_n h_{\min(n,p)}^{-1}h_n^{-2}.
 \tag{RT.13}
\]

Their ratio is \(h_{\min(n,p)}/h_s\). It can be arbitrarily large at a fine collar. Since the input and output can lie in the same determining block, there need not be any positive endpoint distance that could absorb this ratio. A scalar exponential in \(k-n\) does not repair it either: the ratio depends on the collar refinement even with \(k-n\) fixed.

This is a failure of this particular norm estimate, not a counterexample to the actual reconstruction theorem. It identifies the cancellation or regularity statement that a successful proof must preserve. The refined metric and the local two-power averaging gain are insufficient by themselves.

### 5. A kernel-composition statement with explicit scope

The following elementary statement makes precise what can be done after the geometric and output-norm issues are settled. It is not one of the catalogue estimates.

Let \(K_1(x,y)\), \(K_2(y,z)\) be nonnegative normalized kernel majorants on a common measured discrete space. Assume

\[
 \sup_x\sum_y\mu(y)e^{a d(x,y)}K_1(x,y)\le C_1,
 \qquad
 \sup_y\sum_z\mu(z)e^{a d(y,z)}K_2(y,z)\le C_2.
 \tag{RT.14}
\]

Then, for their composition with the same normalized measure,

\[
 \sup_x\sum_z\mu(z)e^{a d(x,z)}
       (K_1K_2)(x,z)\le C_1C_2.
 \tag{RT.15}
\]

**Proof.** Use \(d(x,z)\le d(x,y)+d(y,z)\), exchange the nonnegative sums, apply the second row bound, and then the first. \(\square\)

If changing from one output normalization to the other inserts a factor bounded by \(C e^{b|r-s|}\), and every complete layer crossing costs at least \(RM\) in \(d\), reserve a rate \(b/(RM)\) plus a fixed margin from the original exponential before applying (RT.15). The fixed missing endpoint crossing is included in \(C\). A positive endpoint rate and an age rate can then be retained simultaneously.

This composition principle pays genuine mesh ratios between separated layers. It does not pay the zero-distance current loss (RT.12). It also does not create a localized walk expansion: the prepared source kernel expansions must supply that expansion, with the same normalized measures and with sufficient exponential reserve for the carrier count.

### 6. Exact cancellation for a structured residual

This section uses the actual operators of CMP99, Section D, printed pp.417–426. The argument remains on one admitted determining geometry throughout. It does not identify two minimizers on different geometries or change the source's averaging map.

#### 6.1 Definitions and conventions

Use the source's physical inner products: fine-lattice counting measure is multiplied by \(\eta^d\), and the measure of a determining variable in a block of side \(h_b\) is multiplied by \(h_b^d\). Let \(Q\) be the dimensionful linearized averaging operator, so that the dimensionless determining variation in (3.110) is \(h_b(QA)(b)\). Let \(D\) be the covariant derivative, \(R\) the source scalar projection, and \(G'\) the scalar propagator. Define

\[
 K=DG'RD^*,\qquad \Pi=I-K.
 \tag{RT.16}
\]

The source gauge projection identities give

\[
 K^2=K,\qquad QK=0,\qquad RD^*\Pi=0.
 \tag{RT.17}
\]

In particular, \(\Pi\) takes a field into the chosen gauge slice without changing its determining average. These are the identities used in CMP99 (3.115), (3.119), and the derivations following them.

Write \(\Delta\) for the Wilson quadratic Hessian and \(D_2\) for the symmetric operator defined by the quadratic form in (3.134):

\[
 \langle A,D_2A\rangle=2\langle HC^{(2)}(A),J\rangle.
 \tag{RT.18}
\]

Here \(H\) is the earlier minimizing operator in (3.126); it is distinguished from \(H_1\) below. The normalization of \(C^{(2)}\) is matched to this dimensionful \(H\), as specified in the paragraph following source (3.127); the alternative convention that moves a factor of \(h\) between \(H\) and \(C^{(2)}\) is not mixed with it. To fix the sign directly from the defining quadratic form (3.128), set

\[
 T=\Delta-D_2,\qquad
 L=\Pi^*T\Pi,\qquad
 G_1^{-1}=L+DRD^*+Q^*aQ.
 \tag{RT.19}
\]

Thus \(L\) denotes the complete gauge-invariant Hessian appearing in (3.128); the argument does not depend on the signs used in later shorthand names for its two summands. All inverses below are taken on the source's specified finite spaces, with the common null modes removed as in the construction.

The exact minimizing operator, projection, and constrained covariance are

\[
 H_1=G_1Q^*(QG_1Q^*)^{-1},\qquad
 \psi=I-H_1Q-G_1DRD^*,\qquad
 \mathcal G=\psi G_1=G_1\psi^*.
 \tag{RT.20}
\]

These are CMP99 (3.129), (3.147), and (3.153). In particular, the last expression is \(G_1\psi^*\), with the adjoint; it is not generally \(G_1\psi\). The source also proves

\[
 G_1DR=DG'R,\qquad RD^*G_1=RG'D^*.
 \tag{RT.21}
\]

The stars in this subsection refer to the real physical inner products. Their holomorphic continuations mean the corresponding bilinear transposes, as required when continuing the algebraic identities to complex coordinates. No conjugate-dependent operation is inserted into a holomorphic source map.

#### Proposition RT.2 — exact structured-residual identity

For these operators on one fixed admitted geometry,

\[
 \mathcal GL=\psi,\qquad L\mathcal G=\psi^*,
 \qquad
 H_1QA=A-KA-\mathcal GLA.
 \tag{RT.22}
\]

If a forcing has the structured form \(f=LA\), then

\[
 RD^*G_1f=0,\qquad
 L\mathcal Gf=f-Q^*H_1^*f.
 \tag{RT.23}
\]

**Proof.** The range of \(\psi\), and hence of \(\mathcal G\), is the simultaneous kernel of \(Q\) and \(RD^*\). Self-adjointness of the real covariance therefore gives

\[
 Q\mathcal G=0,\quad RD^*\mathcal G=0,\quad
 \mathcal GQ^*=0,\quad \mathcal GDR=0.
\]

Multiplying the identity for \(G_1^{-1}\) in (RT.19) on the left by \(\mathcal G\), and using (RT.20), gives \(\mathcal GL=\psi\); taking the adjoint gives \(L\mathcal G=\psi^*\). Equations (RT.20)–(RT.21) then imply the last identity in (RT.22).

Because \(\Pi DG'R=0\), the definition of \(L\) gives \(LDG'R=0\). Transposing and using (RT.21) yields \(RD^*G_1L=0\). For \(f=LA\), the last term in

\[
 \psi^*f=f-Q^*H_1^*f-DRD^*G_1f
\]

therefore vanishes. This proves (RT.23). \(\square\)

The printed derivation (3.145) first writes its cancellation with the covariance constrained only by \(Q\), denoted \(\overline G_1\). Its difference from \(G_1\) is

\[
 G_1Q^*(QG_1Q^*)^{-1}QG_1.
\]

The source identity \(RD^*G_1Q^*=0\) kills this difference. Thus the full-
\(G_1\) cancellation in (RT.23) agrees with the source calculation; no distinction between the two covariances has been suppressed.

The proof is algebraic in \(T\). In particular, it remains valid if the coefficient \(J\) of the quadratic form (RT.18) is an independently specified small current, provided all displayed operators are constructed together from that same quadratic form and the same gauge projection, on a domain where their inverses exist. It is not an inference from the lower-dimensional relation \(J=J(U)\). Conversely, it does not prove that an arbitrary prepared family obtained by separately altering kernels continues to satisfy those identities. That matching must be checked for the actual preparation parameters.

#### Proposition RT.3 — weighted adjoint-minimizer bound

Here a genuine part of the current normalization can be verified from the source estimates. Work in dimension \(d=4\), with one admitted determining geometry satisfying CMP96 Lemma 2.1. Let \(\delta>0\) be an exponential rate in the value estimate (3.133) for \(H\) or \(H_1\). Reserve a positive rate \(\kappa\) such that

\[
 \delta-\kappa-\frac{\log L}{RM}>0,
 \tag{RT.24}
\]

and retain a further positive margin for the summation condition of that lemma. This is an explicit condition on the chosen geometric constants; it is not asserted for an arbitrary smaller choice of \(R,M\).

For any source set \(A_0\) of determining blocks, define

\[
 \|f\|_{-3,\kappa;A_0}
 =\sup_a h_a^3 e^{\kappa d(a,A_0)}
       \sup_{x\in\Delta(a)}|f(x)|.
 \tag{RT.25}
\]

Then

\[
 \sup_b h_b^3 e^{\kappa d(b,A_0)}|(H_1^*f)(b)|
 \le C\|f\|_{-3,\kappa;A_0},
 \tag{RT.26}
\]

with a uniform constant on the source geometries and regular backgrounds covered by the cited estimate. The same assertion holds with \(H\) in place of \(H_1\).

**Proof.** The dimensionful convention in (3.126), (3.129), and (3.133) gives

\[
 |H_1(x,b)|\le C h_b^{-d}e^{-\delta d(a,b)},
 \qquad x\in\Delta(a).
 \tag{RT.27}
\]

Taking the adjoint with the physical fine and coarse measures and grouping the fine variables into their determining blocks gives

\[
 |(H_1^*f)(b)|
 \le C\sum_a h_a^d h_b^{-d}
                  e^{-\delta d(a,b)}\sup_{\Delta(a)}|f|.
 \tag{RT.28}
\]

Fixed bond-direction multiplicities and endpoint conventions are included in \(C\). By the triangle inequality for the source distance,

\[
 h_b^3 e^{\kappa d(b,A_0)}|(H_1^*f)(b)|
 \le C\|f\|_{-3,\kappa;A_0}
       \sum_a\left(\frac{h_a}{h_b}\right)^{d-3}
                       e^{-(\delta-\kappa)d(a,b)}.
 \tag{RT.29}
\]

In dimension four the displayed mesh ratio has exponent one. If \(a,b\) have layer indices \(r,s\), CMP96 (2.60) at printed p.234, gives

\[
 d(a,b)\ge RM\max\{|r-s|-1,0\},\qquad
 \frac{h_a}{h_b}\le L\exp\left(\frac{\log L}{RM}d(a,b)\right).
 \tag{RT.30}
\]

The reserved rate in (RT.24) and the exponential row sum (2.61) now bound (RT.29). This proves (RT.26). \(\square\)

This is a source-weighted normalized kernel estimate, not merely a qualitative boundedness assertion. It retains an endpoint exponential from an arbitrary fixed source set. Its unweighted specialization agrees with the bound on \(H^*J\) stated immediately after CMP99 (3.136).

Using the dimensionless determining operator \(Q_B=hQ\) would replace \(H_1\) by \(H_{1,B}=H_1h^{-1}\). The combination occurring in (RT.23) is unchanged:

\[
 Q_B^*H_{1,B}^*=Q^*H_1^*.
 \tag{RT.31}
\]

Therefore a change between those conventions must not create or erase a power of mesh in the multiplier term.

#### 6.2 What remains to convert the cancellation into a physical current bound

Equation (RT.23) controls the **complete constrained Hessian**. The current required in BM.24 is obtained from the actual Wilson field. It is not legitimate to identify these operators without retaining the remaining terms.

Set \(a=\mathcal Gf\). Since \(\Pi a=a\), the definitions give the exact identity

\[
 \Delta a
 =La+D_2a+K^*(\Delta-D_2)a.
 \tag{RT.32}
\]

For a structured residual this becomes

\[
 \Delta\mathcal Gf
 =f-Q^*H_1^*f+D_2\mathcal Gf
       +K^*(\Delta-D_2)\mathcal Gf.
 \tag{RT.33}
\]

Two pieces of this identity now have the correct source weights. Proposition RT.3 proves the weighted \(H_1^*\) estimate. Also, the value bound for \(\mathcal G\) in CMP99 Theorem 3.13, combined with (3.137), gives

\[
 \|D_2\mathcal Gf\|_{-3,\kappa';A_0}
 \le C M\alpha_0\|f\|_{-3,\kappa;A_0}
 \tag{RT.34}
\]

for a suitably reserved \(0<\kappa'<\kappa\). Indeed, the covariance value estimate takes a current of size \(h^{-3}\) to a field of size \(h^{-1}\), while (3.137) multiplies the local field bound by \(CM\alpha_0h^{-2}\). The finite neighboring-block support in (3.137) costs only a fixed endpoint factor. This use of Theorem 3.13 needs no Laplacian estimate.

The complete estimate nevertheless still needs the actual local \(Q^*\) bound in the source measures and control of the last term of (RT.33). Neither follows merely by naming \(K\) a gauge projection. For example, \(K^*D_2a=DRG'D^*D_2a\) contains a differentiated scalar propagator on both sides of a potentially rough input. The corresponding scalar estimate in CMP99 (3.44) requires additional input regularity; a uniform supremum bound does not follow from (3.137) alone.

The source gauge identity (3.117) does identify a useful cancellation in part of that last term. At a real background with its actual Wilson current \(J_U\), differentiating the quadratic gauge identity once in a gauge parameter yields

\[
 D^*\Delta a=\mathcal B_{J_U}a,
 \tag{RT.35}
\]

where \(\mathcal B_{J_U}\) is a local zeroth-order operator. Explicitly, with the source parallel transport \(R_b\), its bilinear form is

\[
 2\langle\lambda,\mathcal B_{J_U}a\rangle
 =\left\langle
 i[\lambda(b_-),a(b)]-i[a(b),R_b\lambda(b_+)],J_U(b)
 \right\rangle.
 \tag{RT.36}
\]

Hence \(|\mathcal B_{J_U}a|\le C|J_U||a|\), with only the finite endpoint shifts, and

\[
 K^*\Delta a=DRG'\mathcal B_{J_U}a.
 \tag{RT.37}
\]

This replaces a third derivative by a scalar propagator and a local current vertex. It does not replace \(J_U\) by an independent source coordinate. Nor does it control the separate \(K^*D_2a\) term or identify the forcing produced by the joined reconstruction. The formula is recorded to make the remaining cancellation problem precise.

The scope restriction is necessary: CMP99 Theorems 3.12 and 3.13 explicitly exclude the covariant-Laplacian bound for \(G_1\) and \(\mathcal G\). Their value, first-derivative, and Hölder estimates therefore cannot be cited as an unconditional bound for \(\Delta\mathcal G\). Equations (RT.22)–(RT.37) show what additional structure can replace that missing generic bound and which terms still require an estimate.

Equation (RT.33) is a Wilson quadratic-Hessian identity. Its transfer to the nonlinear current in the actual local Lie-algebra chart, including the current and chart conversion terms, remains part of BM.24.

Finally, to use this cancellation at a fine collar one needs a smooth tangent lift on the reconstructed geometry whose actual determining variation equals that of the original prepared field. A comparison of tangent fields in two separately chosen gauges does not establish this equality. The paired gauge identification, any correction of the averaging mismatch, its physical current norm, and its compatibility with independent \(J\) and complex preparation remain part of the actual-model application.

### 7. Remaining actual theorem

To finish (BM.24), the proof still needs all of the following in one compatible construction:

1. A checked identification of the actual joined determining geometry (RT.1), its data, and the relevant scale conversion, or a direct estimate that does not need this identification.
2. A reconstructed-current estimate preserving the smooth input response through its fine collars. A generic first derivative kernel applied to (RT.10) has the explicit deficit (RT.12).
3. Joint validity for the independently extended source current and the actual complex preparation parameters, with a strictly admitted domain before Cauchy differentiation. Equality on the physical relation \(J=J(U)\) cannot justify that joint extension.
4. The marked-path or equivalent local expansion retaining a positive endpoint rate, so the boundary carrier and collar sums can be charged as in the complete sector analysis.

The source's claimed multiscale analytic extension is relevant evidence, but this note does not replace the missing quantitative current-coordinate application by that claim. The present result is therefore a source-checked structural improvement and an explicit obstruction to a shortcut, not a completed C-05 proof.

### Primary references and verification scope

- T. Balaban, CMP119 (1988), 243–285: (2.14), (2.34)–(2.39), and the discussion of (3.43) in this and the argument.
- T. Balaban, CMP102 (1985), 277–309: Proposition 9 and (190), with the five different physical output powers retained.
- T. Balaban, CMP99 (1985), 389–434: (3.115)–(3.153), especially the defining quadratic form (3.128), projection (3.147), covariance identity (3.153), kernel estimate (3.133), and the explicit Laplacian exceptions in Theorems 3.12–3.13. Printed pp.420–426 were for the operator signs, adjoints, and constraints.
- T. Balaban, CMP96 (1984), 223–250: Lemma 2.1, (2.60)–(2.61), printed p.234 for the layer-distance and normalized summation bounds.
- T. Balaban, CMP109 (1987), 249–301: article, (1.15)–(1.16) and the explanation immediately following (1.16).
- T. Balaban, CMP122 (1989), 355–392, LFR II: (1.61) and the associated fixed-geometry localization statement, pp.373–375.

### Supplement AJ.1: Complete boundary-sector application and a local Wilson difference bound


This part checks the downstream boundary application and proves a useful local Wilson-action estimate. The joined reconstruction estimate (BM.24), including its spatially localized version, is not obtained here. The C-05 statement and its application conditions are unchanged.

#### 1. What the primary source actually localizes

See CMP119, pp.251, 254–255, 261–262, 269 and 276–277. The complete boundary ledger of Annex AF, Section 2, is retained. In particular:

- the current Gaussian quadratic form and its retained cross force stay in the exact Gaussian split;
- the classical and nonlinear-constraint terms, Haar and coarea factors, inherited E/R terms assigned to B, inherited B terms, heterogeneous Wilson coefficient and relocation/Jacobian are all present;
- the older cross-component Gaussian terms already assigned to B are covered by the inherited B sector;
- retained-only boundary constants cancel only from the conditional normalized law, and remain in the outer marginal;
- the relocation cutoff is smooth in the old real variable, which remains a parameter. Its analyticity in the small relocation field does not assert analyticity of arbitrary old-selector derivatives.

CMP119 p.276 applies the complete generalized random-walk expansions of CMP99 Theorems 3.7–3.10 to the full determining sequence. It describes the localized terms by current-scale domains and retains only the genuinely regular domains in E/R. Its boundary terms use the separate multiscale domain (3.43). On p.277 the B-origin fluctuation expansion retains the primitive full-tree decay, together with the small response factor. The heterogeneous coefficient and relocation terms are treated immediately afterward.

These are useful primary statements, but their analyticity domain is not a substitute for showing that the actual proposed current-coordinate tube is mapped into it. The proof must retain the full tuple of conditions (2.34)–(2.39), including the reconstructed field and current.

#### 2. A fine-spacing-independent Wilson difference estimate

Use any fixed matrix norm on the complexification of the defining representation of SU(N). On a neighborhood of the identity in the invertible matrices define the holomorphic Wilson plaquette function

\[
 s(P)=N-\frac12\operatorname{Tr}(P+P^{-1}).
 \tag{BC15.1}
\]

For a unitary plaquette this is exactly the scalar plaquette observable \(N-\operatorname{Re}\operatorname{Tr}P\). No change to the source coefficient dictionary is made.

##### Lemma BC15.1 — local curvature differences pay the fine-cell count

Work in dimension \(d=4\), and let \(0<\eta\le h\). Suppose two plaquette matrices, expressed in one common local trivialization, obey

\[
 \|P_0-I\|\le a(\eta/h)^2,
 \qquad
 \|P_1-P_0\|\le u(\eta/h)^2,
 \qquad a+u\le\tfrac14.
 \tag{BC15.2}
\]

Then

\[
 |s(P_1)-s(P_0)|
 \le C_N(au+u^2)(\eta/h)^4.
 \tag{BC15.3}
\]

If a proper-scale localization cube has side at most \(C_b h\), and its fixed partition function has modulus at most \(C_\zeta\), summing the corresponding plaquette differences in that cube gives

\[
 \left|\sum_{p}\zeta(p)[s(P_1(p))-s(P_0(p))]\right|
 \le C_{N,d,C_b,C_\zeta}(au+u^2).
 \tag{BC15.4}
\]

The constant does not depend on \(\eta/h\).

**Proof.** The segment \(P_t=P_0+t(P_1-P_0)\), \(0\le t\le1\), lies in the ball of radius \(1/4\) about the identity. It need not lie in SU(N): the holomorphic extension (BC15.1) is defined there. Differentiating and using cyclicity of trace gives

\[
 Ds(P)[H]=\frac12\operatorname{Tr}[(P^{-2}-I)H].
 \tag{BC15.5}
\]

On that ball, the inverse identity or its convergent geometric series gives
\(\|P^{-2}-I\|\le C\|P-I\|\). Thus

\[
 |Ds(P_t)[P_1-P_0]|
 \le C_N(a+u)u(\eta/h)^4.
\]

Integrating proves (BC15.3). The number of plaquettes in the cube is at most \(C_{d,C_b}(h/\eta)^d\). For \(d=4\), this cancels the fourth power in (BC15.3). The bounded partition function contributes only its stated constant. This proves (BC15.4). \(\square\)

The proof works on a complex admitted contour and is consequently suitable for subsequent Cauchy differentiation. It must use a common chart, or an explicitly bounded gauge comparison. It does not compare unrelated plaquette matrices in different moving gauges.

The primitive output estimate needed in (BC15.2) is a curvature estimate, not merely an undifferentiated link estimate. In the original determining geometry it is supplied by the prepared-field/current estimates (BM.10)–(BM.11) and the exact local current/plaquette calculation in Annex AD. For a reconstructed output on the joined geometry, it remains part of the actual transfer theorem.

#### 3. The heterogeneous coefficient does not need a beta-function sign assumption

The source coefficient is the localized recursion CMP119 (2.24). Write \(w_l=g_l^{-2}\), \(\beta_l=w_{l-1}-w_l\). Then

\[
 w_k(x)-w_k=\sum_{l=1}^k\beta_l(1-\phi_l(x)).
 \tag{BC15.6}
\]

At a point whose earliest nontrivial cutoff index is \(n\), the uniform cutoff bound and the admitted coupling comparison yield

\[
 |w_k(x)-w_k|
 \le C(1+k-n)^2g_k^{-2}.
 \tag{BC15.7}
\]

Indeed, bound \(|\beta_l|\) by \(w_{l-1}+w_l\), use \(w_l\le C(1+k-l)w_k\), and sum. No monotonicity or sign of \(\beta_l\) is used.

The earliest active cutoff layer must still be identified with the appropriate geometrical layer, up to the source's fixed collar convention, when applying a layerwise kernel bound. Interlacing alone is not that check. The construction of \(\Omega_{l+1}\) in CMP119 (3.2)–(3.5) surrounds the prior bad set before admitting the next region; the fixed cutoff \(\phi_l=1\) on the prescribed interior of \(\Lambda_l\) is used together with that collar. The enlarged bad-complement rectangles do not weaken a regular-to-bad separation: pp.251 and 269 enlarge components of \(\Lambda_l^c\), so the regular region only shrinks.

Combining (BC15.4), (BC15.7) and a verified original-geometry response

\[
 u_n\le C g_kP_k\,e^{-cR_k}e^{-\Gamma(k-n-c_0)_+}
 \tag{BC15.8}
\]

gives a local heterogeneous-action value bound proportional to

\[
 g_k^{-2}(g_kP_k)(1+k-n)^2
      e^{-cR_k}e^{-\Gamma(k-n-c_0)_+}.
 \tag{BC15.9}
\]

Here (BC15.8) has the actual current-to-old-boundary connector: the factor \(e^{-cR_k}\) cannot be asserted at an arbitrary point without that boundary anchor. The original-geometry connector in (BM.14) supplies the needed distinction.

This calculation closes the fine-spacing normalization in the heterogeneous sector. A naive Lipschitz estimate on individual link matrices would lose powers of \(\eta\); the curvature-square structure in (BC15.5) avoids that error. The localized carrier sum still uses the actual prepared-kernel expansion described next.

#### 4. The exact extra interface required of the joined reconstruction

An age-only version of (BM.24) proves common-domain admission but does not, by itself, prove an anchored spatial boundary bound. The actual transfer needed by the full C-05 application must retain all of the following:

1. **Joint admission.** The full reconstructed field/current tuple is holomorphic on one simultaneous tube containing \(\|z\|_\infty<2P_k\), with all required native external and preparation variables. Its normalization is exactly that in (2.34)–(2.39), including the two \((p,n)\) weights recorded in (BM.23).
2. **A marked endpoint.** A current-to-output response attached at an old output point \(y\) retains a positive exponential in the actual joined-geometry path distance from the current input. A scalar age norm with the attachment point forgotten is insufficient.
3. **Normalized rows.** Its input measure and output normalization yield a uniform kernel row bound, rather than a sum over unnormalized fine bonds.
4. **Prepared localization.** The same statement holds under the source's complex decoupling parameters, with sufficient unspent walk/tree decay to produce exact current-scale carriers.
5. **External directions.** The admitted native background/current directions have quantitative radii. A raw field direction is not assigned such a radius merely because the composite activity is analytic on a nonempty set.

The primitive decay (2.42) is a full-tree bound. It therefore combines with a marked minimizing-map path. The path and primitive tree together connect the current anchor to the old boundary. As in (BV.6)–(BV.9), divide the available exponentials into separate shares for the current collar, layer age, row/carrier summation and final spatial localization. One must not spend the same exponential twice.

CMP99 Theorem 3.10 explicitly supplies generalized walk localization and endpoint estimates for admitted determining geometries. The discussion on p.427 also treats the tree-shaped expansions generated by the background-current term. CMP116 (1.7)–(1.11) uses separate walk-localization and endpoint factors: a sufficiently large fixed localization block allows complex decouplings while leaving a positive endpoint rate. Its (1.10) and (1.23) then localize the composite analytic functions; disconnected decoupling derivatives vanish. CMP119 p.276 transfers this procedure to the full multiscale cover.

Those primary facts apply to the joined reconstruction only after its determining geometry, all inputs and output norms have been verified. No same-lattice minimizer-localization identity is used to identify two different reconstructed minima.

#### 5. Quantitative completion once that actual transfer holds

This section is an implication with the precise actual-map premise of Section 4. It is not a declaration that the premise has been proved.

Fix the localization parameters first. Reserve enough primitive and prepared decay for the anchored cube count of Annex AH. Choose the effective age rate, after all exponent shares, so that

\[
 \Gamma>4\log L+\log 2+\delta,\qquad\delta>0.
 \tag{BC15.10}
\]

Increase the fixed admissible separation constant to meet the normalized row entropy condition. Choose one fixed \(q>p_0\), one \(\kappa_0\ge12\), and one geometric cutoff exponent \(r>1\). Only after these choices reduce the common coupling ceiling.

For \(\ell_k=\log g_k^{-2}\), put

\[
 P_k=A_1\ell_k^{p_0},\qquad
 \delta_k=g_kP_k,\qquad
 \theta_k=\ell_k^{p_0-q}.
 \tag{BC15.11}
\]

The old B derivative consumes a factor \(2^{j-n}/\alpha_{*,n}\). The common-contour map contributes \(g_kP_k e^{-\Gamma(k-n)}\), and the running-radius comparison contributes at most \(C\sqrt{1+k-n}\theta_k\). At fixed \(a=k-n\), there are at most \(1+a\) choices of \(j\). Even retaining a conservative \(L^{4a}\) old-cell count, the resulting sum is bounded by

\[
 C B_0\theta_k
 \sum_{a\ge0}(1+a)^b e^{-\delta a},
 \tag{BC15.12}
\]

where one fixed \(b\) includes all finite polynomial age costs. The current collar is helpful but is not needed for this row after the common contour has been admitted. It remains indispensable in the heterogeneous row (BC15.9).

The resulting complete conditional boundary fluctuation can be localized as

\[
 \widetilde B_k=\sum_Y b_{k,Y},\qquad
 \sup_{\mathcal C_k}|b_{k,Y}|
 \le K_{B,k}e^{-\kappa_Bd_k(Y)},
 \tag{BC15.13}
\]

with the conservative prefactor

\[
\begin{split}
 K_{B,k}\le C_{\rm src}(1+S_{b,\delta})\bigl[
 &\mathfrak K_E+C_Rg_k^{\kappa_0-11}+B_0\theta_k\\
 &+g_k^{-2}\delta_k^3+\delta_k
   +g_k^{-2}\delta_ke^{-cR_k}+g_k^\nu\bigr],\qquad
 S_{b,\delta}=\sum_{a\ge0}(1+a)^b e^{-\delta a}.
\end{split}
 \tag{BC15.14}
\]

The first two terms include E/R-origin carriers meeting the newest boundary, for which no old-boundary collar gain is asserted. The third comes from the inherited B terms. The next two are the cubic classical and measure remainders. The sixth is the heterogeneous term whose fine-spacing normalization is proved in Lemma BC15.1. The final term is the relocation/Jacobian contribution, for any one fixed positive power \(\nu\), using the actual exponentially small relocation field and the same complete-action localization. Older cutoff variables stay fixed in this native complex estimate.

The exact current Gaussian cross force is not included in (BC15.14). It remains in the conditional Gaussian mean.

Let \(r_z=c_GP_k\) be the scalar-coordinate radius retained by the common contour. The simultaneous-row estimate BD.2 and the actual anchored carrier count give

\[
 \sup_i\sum_l e^{\gamma\rho_k(i,l)}
     \|D_iD_l\widetilde B_k\|_{\rm op}
 \le C_{G,\gamma}K_{B,k}P_k^{-2}.
 \tag{BC15.15}
\]

The value and gradient bounds have respectively no factor \(P_k^{-1}\) and one factor \(P_k^{-1}\). For fixed local directions in the admitted slots, define \(q_s\) as their norm divided by the actual slot radius. The same carrier sum gives

\[
 \sum_Y e^{\gamma\operatorname{diam}(I_Y)}
 |D_{h_1}\cdots D_{h_m}b_{k,Y}|
 \le C N(S_1)K_{B,k}e^m m!\prod_{s=1}^m q_s.
 \tag{BC15.16}
\]

Here \(S_1\) is the support of any chosen first direction, and \(N(S_1)\) counts its incident localization cubes. Higher coefficients of an additional nonlinear parameter-to-slot map remain separate chain-rule terms. This estimate is not a dimension-free sum of all absolute order-\(m\) tensor coefficients.

All terms on the right side of (BC15.15) tend to zero with the common coupling ceiling. The classical term gives \(g_kP_k\); the bounded E term gives \(O(P_k^{-2})\); the heterogeneous term gives \(g_k^{-1}P_k^{-1}e^{-cR_k}\), which tends to zero because \(R_k\ge\ell_k^r\) and \(r>1\). Thus the completed map interface would yield an arbitrarily small uniform boundary Hessian budget, with no hidden volume or distance factor.

#### 6. Application conditions

The sector list and downstream numerical/carrier deductions are now explicit. Lemma BC15.1 proves the actual local Wilson normalization needed by the heterogeneous sector. The primitive source localizations have the appropriate form for the final sum.

The joined-reconstruction transfer, in the stronger spatial/prepared form in Section 4, is still required before applying this conclusion to the full boundary action. In particular, the existence of a holomorphic activity on (3.43), the original-geometry bound, or the local two-power averaging result does not establish that transfer.

**C-05 remains open in this note.**

#### Primary sources

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243–285, especially (2.24), (2.34)–(2.42), and pp.269, 276–277.
- T. Balaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP 99 (1985), 389–434, Theorems 3.7–3.10 and the tree-expansion discussion on p.427.
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. II. Cluster Expansions*, CMP 116 (1988), 1–22, (1.7)–(1.11), (1.23)–(1.36). DOI: https://doi.org/10.1007/BF01239022.
