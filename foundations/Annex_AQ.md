# A genuine strong native ball for the primitive domain

**Annex AQ.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


This note completes the fixed-point and real physical-identification steps for the zero-relative-data construction in Annex AP. It states the strong external-background hypotheses explicitly. Its conclusion is a bound in the source's relative Landau representation. The passage to a specified raw-data representative, and the admission of the complete primitive boundary activity with its retained older fluctuation arguments, are separate application steps. C-05 is not completed by this annex alone.

### 1. Geometry, norms and the primary inputs actually used

Let an admitted determining history have fine mesh \(\eta\), terminal meshes \(h_a\), terminal blocks \(\Delta(a)\), and source distance \(d(a,b)\). Let \(h_n\) denote an older physical mesh on the same location. The application considered here has

\[
 h_a\le h_n,\qquad
 w_a=\alpha_nh_n^{-3},\qquad
 e_a=h_a^3w_a,\qquad e_*:=\sup_a e_a\le\alpha_*.
 \tag{NP.1}
\]

Every profile used in a row sum, including \(w,e,e^2\), must satisfy the comparison inequalities for the actual multiscale metric with a fixed positive rate reserve. This is the geometric condition in CC.1–CC.4 of Annex AM; it is not a comparison with unweighted Euclidean distance. The geometry is fixed before the coupling ceiling. Its constants do not depend on the total volume or on the number of layers.

For the running profiles used below this condition is obtained as follows. The admitted AF comparison bounds \(\alpha_n/\alpha_m\) in either direction by \(C(1+|n-m|)^b\), with fixed \(b\). Crossing the old layers costs at least \(RM(|n-m|-1)_+\) in the old source metric. A refinement makes its path weights no smaller, so the joined metric has the same lower bound. Consequently \(w_a/w_b\) is at most a fixed constant times \(\exp(\beta d(a,b))\), where \(\beta\) can be chosen proportional to \((3\log L+1)/(RM)\); the polynomial is absorbed with a fixed coefficient. The joined mesh ratios similarly have exponent \(c_h=\log L/(RM)\). Thus \(e_a/e_b\) and \(e_a^2/e_b^2\) have comparison exponents at most \(3c_h+\beta\) and \(6c_h+2\beta\), respectively. Choose the admitted geometric separation once so that these exponents and the finitely many physical-volume powers leave all the kernel row-sum reserves used in RM and CC positive. This choice does not depend on the derivative order.

Use the norms

\[
 \|f\|_{F_w}=\sup_a w_a^{-1}\|f\|_{\infty,\Delta(a)},
\]
\[
 \|A\|_{X_w}=\sup_a\max\left\{
  (h_a^2w_a)^{-1}\|A\|_{\infty,\Delta(a)},
  (h_aw_a)^{-1}\|\nabla_{U_0}A\|_{\infty,\Delta(a)}
 \right\},
 \tag{NP.2}
\]

and let \(E_w\) also include the component covariant Laplacian divided by \(w_a\). The component Laplacian is not being identified with every second partial derivative. The ordinary absolute norm is

\[
 \|A\|_{X_{\rm abs}}
   =\sup_a\max\{h_a|A|,h_a^2|\nabla_{U_0}A|\}.
 \tag{NP.3}
\]

It satisfies \(\|A\|_{X_{\rm abs}}\le e_*\|A\|_{X_w}\).

Fix an external background \(U_0\) on this geometry, and prescribe its **own** actual raw determining data \(V=M_{\mathcal B}U_0\). This point must be admitted by the source variational construction. For real \(U_0\), its real regularity and the regularity of \(V\) are required. For complex \(U_0\), the actual source complex-background conditions are required. In particular the latter include the second-order relative-field restriction in CMP99 (3.38), in addition to the value and first-gradient restrictions in (3.37). It would be incorrect to invoke Proposition 9 of CMP102 on a value-only background ball.

The source normalization of the relative averages gives zero corrected datum for this choice of \(V\): the relative field at the input point is the identity, so every relative transport, mean and correction is the identity. This is RM.3; it does not assert equality of raw and reference-corrected averaging derivatives on arbitrary tangent vectors.

The following inputs are retained with their stated source scopes:

1. The source critical-orbit existence and uniqueness theorem and the axial/Landau reduction, CMP102 Theorem 1 and Proposition 2. The enlarged-gauge variation argument on pp.296–297 supplies unrestricted variations within the corrected determining fiber at the physical Landau critical point.
2. The regular constrained covariance \(C_0\), with the weighted map \(F_w\to E_w\), proved as CC.3 using CMP99 Theorem 3.3 and CMP102 (129)–(130).
3. The chosen dimensionless-data right inverse \(\mathsf H\), with \(hQ\mathsf H=I\), \(RD^*\mathsf H=0\), and value, gradient and current kernel bounds, as specified in RM.4–RM.6. Here the chosen formal external-background family is the extension of CMP102 (174)–(175). Its first coefficient is \(H_1\), including at an admitted off-minimum external background. The primary extension in Proposition 9 is used for this family; no equality with the alternative off-minimum family (179)–(180) is inferred.
4. The exact changed linearizing map, its local inverse, and the complete unrestricted Wilson-action remainder from RM.9–RM.23. These are the deductions in Annex AP, including every cross term.

All adjoints in analytic formulas are the bilinear transposes for the source physical measures, rather than conjugate-dependent maps. This convention is necessary for holomorphy.

### 2. The weighted analytic fixed point

Assume

\[
 \|J_0\|_{F_w}\le\mu,
 \qquad J_0=\mathscr J(U_0).
 \tag{NP.4}
\]

Write the exact physical relative field as

\[
 A=A'-\mathsf H D(A'),\qquad
 D(A')_b=C_j\!\left(h_b[A'-\mathsf H D(A')]\right)_b.
 \tag{NP.5}
\]

The corrected determining datum is \(hQA'\). The map is an analytic bijection on a fixed smaller ordinary source ball and preserves the Landau condition in both directions. The action in this coordinate is

\[
 S(e^{i\eta A}U_0)=S(U_0)+\langle A',J_0\rangle
  +\tfrac12\langle A',(\Delta-D_{2,\mathsf H})A'\rangle
  +V_{\mathsf H}(A').
 \tag{NP.6}
\]

The exact formulas for \(V_{\mathsf H}\) and its derivative are RM.17 and RM.21. In particular the physical Wilson Hessian \(\Delta\) is used before restricting to Landau; no extension of its quadratic form is silently substituted on unrestricted vectors.

Let \(K\) bound \(C_0:F_w\to E_w\). With one fixed \(c\), the estimates of Annex AP give, on \(\|A'\|_{X_w}\le\rho\),

\[
 \|D_{2,\mathsf H}A'\|_{F_w}\le c\mu e_*\rho,
\]
\[
 \|V_{\mathsf H}'(A')\|_{F_w}
       \le c\rho^2e_*(1+\mu e_*),
 \qquad
 \|V_{\mathsf H}''(A')\|_{X_w\to F_w}
       \le c\rho e_*(1+\mu e_*).
 \tag{NP.7}
\]

The derivative bound is taken on a fixed smaller ball within the ball used for the value estimate. Replace \(c\) by a larger fixed constant once so that these simultaneous radii are understood throughout.

#### Proposition NP.1 — a projection estimate driven by physical current

Put \(R=2K\mu\). If \(\mu=0\), the fixed point is zero. Otherwise choose the absolute smallness ceiling so that

\[
 cK e_*\{\mu+2R(1+\mu e_*)\}\le\tfrac14,
 \qquad 2Re_*<\varepsilon_{\rm lin},
 \tag{NP.8}
\]

where \(\varepsilon_{\rm lin}\) is the fixed radius needed for the changed linearizing map. Then

\[
 A'=-C_0J_0+C_0D_{2,\mathsf H}A'-C_0V_{\mathsf H}'(A')
 \tag{NP.9}
\]

has a unique solution in \(\|A'\|_{X_w}\le R\). It satisfies

\[
 \|A'\|_{X_w}\le 2K\mu,
 \qquad \|A'\|_{E_w}\le C\mu,
 \tag{NP.10}
\]

and depends holomorphically on all admitted finite-dimensional external parameters on any common domain with these reserves.

**Proof.** Denote the right side of (NP.9) by \(\mathcal T(A')\). Its constant term has norm at most \(K\mu=R/2\). On the radius-\(R\) ball, the other two terms have norm at most

\[
 Kc\mu e_*R+KcR^2e_*(1+\mu e_*),
\]

which is at most \(R/4\) after (NP.8). The segment integral of the derivative in (NP.7) makes the Lipschitz constant at most \(1/4\). Thus \(\mathcal T\) maps the closed ball strictly into itself and is a contraction. Start the Picard iteration at zero. Every iterate satisfies \(QA'=0\), since \(QC_0=0\). Convergence is uniform in the Banach norm and uniform on smaller external parameter domains. Every iterate is holomorphic there, so the limit is holomorphic. This is a finite-dimensional statement at each cutoff with constants uniform in the cutoff and volume.

Apply the stronger \(F_w\to E_w\) covariance bound to the fixed-point equation. The forcing on its right side is bounded by \(C\mu w\), which proves the second estimate in (NP.10). No claim that (NP.9) alone imposes the Landau gauge is made in this argument. \(\square\)

### 3. Identification with the actual physical solution

The preceding qualification is essential: CMP102 p.300 explicitly distinguishes its equation (143), used for regularity, from the equation that proves existence in the gauge slice. A weighted solution of a projected equation is not automatically a physical critical point.

#### Proposition NP.2 — uniqueness in an enclosing ordinary ball

There is one fixed \(\delta>0\) such that, for admitted external backgrounds with sufficiently small absolute regularity and

\[
 j_*:=\sup_a h_a^3|J_0|\le\mu e_*
 \tag{NP.11}
\]

sufficiently small, (NP.9) has at most one solution in \(\|A'\|_{X_{\rm abs}}\le\delta\).

**Proof.** Repeat the actual estimates with the admissible ordinary profile \(\bar w_a=h_a^{-3}\). Its associated \(\bar e_a\) is one. The current parameter in those estimates is now \(j_*\), and the field radius is \(\delta\). The derivative of the right side of (NP.9) on that ball is at most

\[
 K_{\rm abs}c\{j_*+\delta(1+j_*)\}.
 \tag{NP.12}
\]

Choose \(\delta\) within the ordinary linearization radius and so that the term independent of \(j_*\) is at most \(1/8\). Then lower the common background and current ceiling until the entire expression is at most \(1/4\). For any two solutions the segment integral of the derivative gives a contraction estimate for their difference. They must coincide. This argument establishes uniqueness for the **changed** coordinate equation; it does not assume that the source's uniqueness proposition for a differently written nonlinear equation transfers without proof. \(\square\)

#### Theorem NP.3 — physical identification in the relative Landau chart

For a real admitted \(U_0\), let the regular critical orbit for \(V=M_{\mathcal B}U_0\) be the orbit supplied by the source theorem. Assume the ordinary regularity ceiling is chosen so that the source relative Landau representative and its transformed \(A'\) lie in the ball of Proposition NP.2. Choose \(e_*\) so that also \(Re_*<\delta\). Then the weighted fixed point in Proposition NP.1 is precisely that physical representative in the changed linearizing coordinate. Consequently the associated \(A\) satisfies

\[
 Q\text{-corrected datum}(A)=0,
 \qquad RD^*A=0,
\]
\[
 |A|\le C\mu h_a^2w_a,
 \quad |\nabla A|\le C\mu h_aw_a,
 \quad |\Delta_{\rm cov} A|\le C\mu w_a.
 \tag{NP.13}
\]

On a common holomorphic external chart these identities and bounds continue to complex inputs, in the same relative Landau representation.

**Proof.** The source reduction of the real critical orbit has zero corrected datum by the exact choice \(V=M_{\mathcal B}U_0\). Transform it using the local analytic inverse in (NP.5). Since \(RD^*\mathsf H=0\), the transformed field remains Landau, and it satisfies \(QA'=0\).

At this physical critical point, the source gauge-orbit argument allows all small variations in the corrected determining fiber, without requiring their variations to be Landau. The changed coordinate map is a local bijection of these fibers. Differentiating the exact action (NP.6) therefore yields

\[
 \langle v,J_0+(\Delta-D_{2,\mathsf H})A'
                   +V_{\mathsf H}'(A')\rangle=0
 \quad(Qv=0).
 \tag{NP.14}
\]

Since the point itself is Landau, one may insert the regular gauge-fixing quadratic term in this stationarity equation at that point. Apply the regular constrained covariance, as in CMP102 (128)–(143); this gives exactly (NP.9). The actual physical solution and the weighted fixed point both lie in the ordinary radius-\(\delta\) ball. Proposition NP.2 identifies them. Landau is obtained from this identification, not from an unsupported property of the range of \(C_0\).

The quadratic estimates RM.11–RM.12 applied with \(\rho=2K\mu\) show that the linearizing correction has value, gradient and component-Laplacian bounds at most \(C\mu^2e_*\) times the respective \(X_w,E_w\) weights. Combine them with (NP.10) to obtain (NP.13).

For holomorphic external parameters, the operators and fixed point are holomorphic on the common admitted chart. The real identities are identities on a real open parameter set, so they continue by the finite-dimensional holomorphic identity theorem. This continuation requires actual common admission; it does not supply a missing domain radius by itself. \(\square\)

#### Physical current in the same representation

The Landau condition also gives the physical second-order estimate needed here. The covariant lattice identity used in CMP102 (134)–(140) writes \(D^*DA\) as the component covariant Laplacian plus a curvature multiplier, minus \(DD^*A\). Write \(I=R+P\) on the scalar gauge space. Since \(RD^*A=0\),

\[
 DD^*A=DPD^*A.
 \tag{NP.15}
\]

The source smoothing row for \(DPD^*\), CMP99 (3.49), applied with the same profile reserve, maps \(h_a^2w_a\) into \(w_a\). The curvature multiplier is bounded by the admitted absolute regularity times \(h_a^{-2}\); it has the same mapping property. It follows that

\[
 |D^*DA|+|\Delta A|\le C\mu w_a.
 \tag{NP.16}
\]

Here \(\Delta\) is the physical Wilson Hessian at \(U_0\). This step uses Landau after physical identification. It is not an \(L^\infty\) estimate for arbitrary second derivatives of an arbitrary field.

To compare with the actual current, let \(W=e^{i\eta A}U_0\). The derivative of the local exponential chart is an invertible finite-dimensional matrix at every link; its norm and inverse norm are bounded when \(\eta|A|\) is within the fixed source radius. The derivative of the physical action in this chart is

\[
 J_0+\Delta A+V_0'(A).
\]

The local analytic chart factor converts this derivative to \(\mathscr J(W)\). The Wilson remainder bound RM.23 is \(C\mu^2e_*w_a\). Therefore

\[
 |\mathscr J(W)|\le C\mu w_a.
 \tag{NP.17}
\]

Define the physical curvature norm here by \(F(U)(p)=\eta^{-2}(U(\partial p)-1)\), on the indicated small plaquette chart. This differs by the displayed factor from a convention that calls the unscaled plaquette difference itself \(F\). The corresponding curvature expansion, using the value and first-gradient bounds in (NP.13), gives

\[
 |F(W)-F(U_0)|\le C\mu h_aw_a
 \le C\mu\alpha_nh_n^{-2}.
 \tag{NP.18}
\]

In particular (NP.17) has the older current weight \(\alpha_nh_n^{-3}\), not the weaker generic joined weight \(\alpha_nh_a^{-3}\). This is the point of the zero-data argument.

### 4. A genuine strong native input ball

Fix a real source background \(U_*\) with the local old-layer strong bounds

\[
 h_n^2|F(U_*)|+h_n^3|\mathscr J(U_*)|\le C_{\rm hist}\varepsilon_n,
 \qquad \varepsilon_n=A_0g_n\ell_n^{p_0}.
 \tag{NP.19}
\]

Its local real charts must include the value, first-gradient and second-order bounds in CMP99 (3.35)–(3.36). Let

\[
 \alpha_n=C_\alpha g_n\ell_n^q,\qquad q>p_0.
 \tag{NP.20}
\]

Use a complex perturbation \(U_0(E)=e^{i\eta E}U_*\) with the **strong** norm

\[
 \|E\|_{\mathfrak N}=\sup_n\max\left\{
 \frac{h_n|E|}{\alpha_n},\frac{h_n^2|\nabla_{U_*}E|}{\alpha_n},
 \frac{h_n^3|D_{U_*}^*D_{U_*}E|}{\alpha_n}
 \right\}.
 \tag{NP.21}
\]

The second-order row required by the primary external-background theorem cannot be omitted. A component-Laplacian row is not imposed on the external perturbation: it is an output supplied by the regular covariance for the correction in NP.10. This distinction matters for a subsequent smooth gauge interpolation, whose curl-current row is controlled by exact current covariance. A ball in (NP.21) is a sufficient external-background domain; no equivalence with a value/gradient-only ball is claimed.

For \(\|E\|_{\mathfrak N}<r\), the local Wilson expansion and bounded chart factors give

\[
 |\mathscr J(U_0(E))|\le C\left(C_{\rm hist}\frac{\varepsilon_n}{\alpha_n}+r+r^2\alpha_*\right)w_a.
 \tag{NP.22}
\]

The real-center ratio \(\varepsilon_n/\alpha_n\) is at most \(C\ell_*^{p_0-q}\). The absolute joined-scale norm is smaller than the corresponding old-scale norm because \(h_a\le h_n\). Thus a fixed choice of \(r\), followed by a sufficiently small common coupling ceiling, admits the source external-background operators and makes the \(\mu\) in Proposition NP.1 a fixed small number. The bound is independent of total volume.

#### Lemma NP.4 — absolute raw-data admission on the whole ball

Use the actual joined determining history of JI.1–JI.4 in Annex AO, with its proper-scale collars and star conventions. The determining datum \(M_{\widehat B}U_0(E)\) lies in a common absolute analytic chart throughout a sufficiently small fixed radius \(r\) of (NP.21), once the common coupling ceiling is chosen. The constants are uniform over the admitted old histories and carrier sizes.

**Proof.** At a determining bond of mesh \(h_s\), the relative transport and relative-average estimates in CMP99 (3.55)–(3.59), with the corresponding symmetric operators, bound the raw relative increment by

\[
 C h_s\sup_{\operatorname{foot}(b)}|E|.
 \tag{NP.25}
\]

The raw/reference-corrected endpoint factor is retained in this estimate; it is the bounded factor explicitly present after (3.57). No identification of their derivatives is needed. The footprint comprises the actual two endpoint blocks and connecting averaging paths. The source separation permits that footprint to reach at most a fixed neighboring earlier layer. At all other points it is in the same or a coarser old layer. Adjacent meshes and running radii differ by fixed factors. Since the joined mesh is no larger than the old mesh, (NP.25) is at most \(Cr\alpha_*\).

The real reference \(U_*\) itself witnesses a nonempty regular fiber for its own joined data: the joined meshes are smaller, so its old current and curvature bounds imply the required absolute joined bounds. CMP102 p.278, immediately after (7), explicitly states that a nonempty regular fiber implies the determining-data condition (7), with a fixed multiple of its regularity constant. That statement includes the special crossing plaquettes defined in the preceding paragraph. Thus the real reference data have the absolute bound \(C C_{\rm hist}\varepsilon_*\). No desired running reconstructed-current estimate is used to obtain it. Reduce the common coupling ceiling until that bound and \(Cr\alpha_*\) fit fixed fractions of the source real and complex data radii. The resulting chart contains the entire strong ball, not just its real diameter or its first tangent. \(\square\)

The field space in this lemma is on the actual carrier dependency set, including the fixed collar links that supply its determining data and the stencils used by the strong norm. Those links are external input data and may vary with \(E\). They are not extended by zero across a newly imposed boundary. The unknown correction in NP.5 has the source fixed-boundary conditions relative to each such input. This distinction prevents a spurious fine-mesh derivative from a sharp extension of an input tangent.

#### Theorem NP.5 — the U-dependent primitive boundary domain has a fixed strong radius

Use the normalized converter RM.3 of Annex AP, in the corresponding source symmetric family, followed by its root-fixed conversion to the adopted absolute auxiliary representative. Fix the real source bounds (NP.19), the current/field normalization ratios, and the admitted geometry. There exist fixed \(r_0>0\) and a common coupling ceiling such that, for every \(\|E\|_{\mathfrak N}<r_0\), all the U-dependent inequalities CMP119 (2.34), (2.35), (2.37), (2.38), (2.39) hold with a fixed reserve, for every reconstructed level \(p\) in that primitive domain. The radius is independent of the fine mesh, layer count and total volume. The independent current slot in (2.36) may be included on the common radius of BC16.21–BC16.23.

**Proof.** Lemma NP.4 admits the internal source maps first, on their fixed absolute domains. The strong external assumptions in (3.35)–(3.38) hold by (NP.19), (NP.21), the smaller joined meshes, and the same choice of ceiling. Propositions NP.1–NP.3 therefore apply to every reconstruction. The old-layer current and curvature bounds are (NP.17)–(NP.18), with

\[
 \mu\le C\{C_{\rm hist}\ell_*^{p_0-q}+r_0+r_0^2\alpha_*\}.
 \tag{NP.26}
\]

RM.3 gives a holomorphic converter and inverse with a uniform bound on this whole ball. The additional root-fixed gauge used to reach the actual auxiliary axial convention is bounded by comparison to its fixed real reference using the same local transport estimate. Current and plaquette differences transform exactly by conjugation. Thus those bounds acquire only a fixed multiplier. In physical units the required reconstructed-current weight is \(\alpha_n h_n^{-2}h_{\min(p,n)}^{-1}\), which is no smaller than \(\alpha_nh_n^{-3}\). The reconstructed curvature restriction similarly follows from the old-layer physical curvature bound. The reference field and its real local gauges supply (2.38). The input relative-potential and gradient restrictions are directly (NP.21); an auxiliary axial potential is never used to prove (2.39).

Let \(s_*=1-\beta\). Every numerical coefficient in the listed source restrictions is at least \(s_*\). Let \(C_{\rm dom}\) be a common constant in the preceding estimates, including the finitely many normalization ratios and the uniform embedding of actual layers into an older primitive's innermost-region convention. Choose \(r_0\) so that \(C_{\rm dom}(r_0+r_0^2)\le s_*/8\). Then choose the common coupling ceiling so that \(C_{\rm dom}C_{\rm hist}\ell_*^{p_0-q}\le s_*/8\), and all absolute smallness requirements in NP.8–NP.12 and RM.3 also hold. Every running output then uses at most a fixed fraction of its allowed radius. The real-reference restrictions and input-field restrictions have the same reserve after one further fixed reduction of \(r_0\), if needed.

For the common older-primitive embedding, the actual layer \(n\ge j\) has ratios bounded by a fixed polynomial in \(n-j\) times \(L^{-r(n-j)}\), with \(r=1,2,3\) for value, gradient/curvature and current respectively. The suprema are finite. Include them once in \(C_{\rm dom}\); no factor grows with the number of older activities. The independent current slot does not enter the reconstructed field predicates and is treated as in BC16.4. This proves a genuine ball contained in the complete field/current part of the primitive domain. \(\square\)

This theorem does not by itself identify a current-dependent smooth representative of the **input** primitive with the source's original axial pullback when older fluctuation variables are present. That is the distinct fixed-old-variable gauge interpolation in AD17.3. It also does not supply a joint contour for an unmatched, newly introduced decoupling operator family.

### 5. Endpoint use and the exact uncompleted application

Suppose the actual primitive input family, in a smooth chart with all older arguments accounted for, has a current-coordinate tangent \(v_i\) satisfying

\[
 \|v_i\|_{\mathfrak N,X}
 \le \frac{\vartheta_X}{P_k}e^{-c d_X(i)}.
 \tag{NP.23}
\]

If a fixed radius \(r_0\) of the strong ball above is contained in the **complete** primitive domain at each such center, then Cauchy on the genuine affine curve in that chart gives

\[
 |\partial_i b_X(\Phi(z))|
 \le \frac{K_X}{r_0}\frac{\vartheta_X}{P_k}e^{-c d_X(i)}.
 \tag{NP.24}
\]

The fixed-factorial all-order carrier summation BC16 then applies. The missing assertion cannot be replaced by a bound for first derivatives of the reconstructed outputs. That invalid inference was excluded by the exact counterexample BC16.19a.

At the present scope, the following are still separate checks:

- The chosen native directions and their extensions use the actual local source geometry and remain in its complete strong external-background class.
- The source raw-data gauge converter is uniformly bounded, with the needed endpoint response, on that common ball.
- The actual primitive pullback can be evaluated in a smooth input chart while preserving every old fluctuation, independent current, constraint and relocation argument. Real simultaneous gauge covariance alone does not supply a complex radius for an older variable.
- The complete source sector ledger has the endpoint/carrier prefactors required by BC16 and the earlier boundary value budget.

These are application conditions for C-05, not new estimates. The projection theorem above removes a specific fine-collar loss; it does not remove those conditions.

### Primary references

- T. Bałaban, *Propagators for lattice gauge theories in a background field*, Commun. Math. Phys. **99** (1985), 389–434: (3.35)–(3.38), Theorem 3.3, (3.49), (3.127)–(3.133). DOI: https://doi.org/10.1007/BF01240355.
- T. Bałaban, *The variational problem and background fields in renormalization group method for lattice gauge theories*, Commun. Math. Phys. **102** (1985), 277–309: Theorem 1, Proposition 2, (123)–(143), (174)–(190), Proposition 9. DOI: https://doi.org/10.1007/BF01229381.
- T. Bałaban, *Convergent renormalization expansions for lattice gauge theories*, Commun. Math. Phys. **119** (1988), 243–285: (2.34)–(2.42), (3.15), (3.43). DOI: https://doi.org/10.1007/BF01217741. These identify the eventual application, rather than supplying its new estimates.
