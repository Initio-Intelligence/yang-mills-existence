# Exact nonlinear support, joined consistency and bounded gauge conversion

**Annex AL.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


This note proves a nonlinear shell-support identity for the source averaging operation, a consistency theorem under an exact constraint-inclusion premise, and an anchored transport-gauge estimate. It also gives an explicit completed splice for which the constraint-inclusion premise holds. Identifying that splice with the incomplete-tuple notation in CMP119 (2.35), and matching the bounded transport gauge to the actual reconstructed representative, remain necessary source checks. The physical family of true minima is not identified with arbitrary independently extended current/background coordinates or with separately prepared kernels. Because of these limitations, the actual-model estimate is not completed here.

### 1. The lattice convention does not remove the fine collar

Write \(a\) for the physical fine spacing, and \(h_r=L^ra\) for the physical spacing after \(r\) averages. When the \(j\)-th coarse spacing is the unit, the fine spacing is \(\xi=L^{-j}\). When the \(p\)-th coarse spacing is the unit, it is \(\eta_p=L^{-p}\). The coordinate change is

\[
 x^{[p]}=L^{j-p}x^{[j]},\qquad
 a=h_j\xi=h_p\eta_p.
 \tag{JR.1}
\]

These are the same physical fine links, expressed in different units. This convention is explicit in the geometric discussion of CMP109, printed p.257, and in its definition of reconstructed currents in (1.15). CMP119 (2.35) and (2.37) retain it. In particular,

\[
 L^{-2p}(L^nL^{-p})^{-2}=L^{-2n},
\]

while multiplying the current bound in (2.37) by \(h_p^{-3}\) gives the physical current weight

\[
 h_p^{-3}L^{n-\min(p,n)}(L^nL^{-p})^{-3}
 =h_n^{-2}h_{\min(p,n)}^{-1}.
 \tag{JR.2}
\]

Consequently a fine determining collar is not removed by the appearance of \(L^{-p}\) in the reconstructed-current formula. Its local determining blocks can still be smaller than \(h_{\min(p,n)}\). The deficit identified in RT.12–RT.13 is a real deficit of the generic estimate; the question is whether the actual data enjoy an exact cancellation.

### 2. What one averaging step uses

Let \(\mathsf M_r\) denote one source averaging step from the lattice of spacing \(h_r\) to that of spacing \(h_{r+1}\). Thus

\[
 M^{r+1}=\mathsf M_r\circ M^r.
 \tag{JR.3}
\]

The source average uses the two endpoint blocks of an output bond. In CMP109 (0.12), the relevant paths consist of a path from the first coarse endpoint to a point in its block, the translated straight coarse bond, and a path within the second endpoint block. Its reference path is contained in the same pair of blocks. The symmetric contour averages in (0.11) do not enlarge that support. Hence:

> If two input connections agree on the fine bonds in the two endpoint blocks of a coarse bond, including the connecting bonds, their one-step averages agree at that coarse bond.

This is a statement about the actual nonlinear group average. No linearization or Abelian replacement is used. The definition as iterated averaging gives (JR.3); the corresponding derivative composition is also displayed in CMP99 (3.15).

The footprint conclusion must be used carefully. A change inside one endpoint block can change an output bond whose other endpoint lies outside the changed region. Averaging therefore gives **star support**, not support on bonds with both endpoints in the region.

### 3. The exact bond-set convention gives a star-support induction

Write \(\operatorname{st}_r Y\) for the level-\(r\) bond set induced by a point set \(Y\): its bonds have at least one endpoint in \(Y\). The source set difference is taken on these bond sets. In particular, it is not generally the star of the difference of the point sets. Let an admitted determining history of depth \(p\) be

\[
 X_0\supset X_1\supset\cdots\supset X_p,
 \qquad X_{p+1}=\varnothing.
 \tag{JR.4}
\]

Each \(X_r\) is a union of the appropriate \(r\)-blocks. Define the determining bond sets by the actual source convention

\[
 \Lambda_r=\operatorname{st}_r X_r\setminus
                 \operatorname{st}_r X_{r+1},
 \quad 0\le r\le p,
 \tag{JR.5}
\]

with the exterior also fixed at level zero. The prescribed values are imposed on these bond sets. A bond joining the point shell to the inner region lies in \(\operatorname{st}_r X_{r+1}\), so it is not fixed merely because it touches the point shell. This distinction is visible in CMP96 (2.3), whose accompanying text applies the difference separately to the site and bond sets.

#### Lemma JR.1 — nonlinear shell support induction

Suppose \(U,W\) agree on the exterior fine bonds and share the complete determining data of (JR.4)–(JR.5). At every step where the averages are defined,

\[
 \operatorname{supp}(M^rW-M^rU)
 \subset\operatorname{st}_r X_{r+1},
 \qquad 0\le r\le p.
 \tag{JR.6}
\]

In particular, the \(p\)-th averages agree. This statement can be applied on the finite dependency cone of a specified higher average; it does not require defining averages in unrelated large-field regions.

**Proof.** At level zero, the prescribed \(\Lambda_0\) values and the fixed exterior imply that every changed fine bond lies in \(\operatorname{st}_0X_1\). Cross-boundary bonds incident to \(X_1\) may still vary; they are retained in this support statement.

Assume (JR.6) at level \(r<p\). If both endpoints of an \((r+1)\)-bond lie outside \(X_{r+1}\), their endpoint blocks also lie outside \(X_{r+1}\), because that set is a union of these blocks. Every fine bond in the actual two-block averaging footprint has both endpoints in this outside union. It therefore misses \(\operatorname{st}_rX_{r+1}\), including the cross-boundary bonds retained in the induction hypothesis. The input fields agree throughout the footprint. Before imposing the next determining data, the changed output bonds consequently belong to \(\operatorname{st}_{r+1}X_{r+1}\).

The actual prescribed level-\((r+1)\) datum fixes the set difference
\(\operatorname{st}_{r+1}X_{r+1}\setminus
\operatorname{st}_{r+1}X_{r+2}\). Removing that difference leaves precisely
\(\operatorname{st}_{r+1}X_{r+2}\), proving the induction step. At \(r=p\), the set \(X_{p+1}\) is empty and no changed bond remains. \(\square\)

At no stage is the support asserted to have both endpoints inside the next domain. Cross shell-to-inner bonds are allowed until their actual data are fixed at the appropriate subsequent level. The terminal empty star is sufficient for equality. The larger source separation is needed elsewhere for the admissible variational problem and for patching the action; the support induction itself uses block alignment and the exact set differences.

The conclusion uses the exact group-valued data, not their linearized approximations. It remains an equality under holomorphic continuation wherever the same averaging expressions are defined.

#### Dependency-cone convention

In the actual large-field history, \(\Gamma_0=\Omega_1^c\) can contain fixed data outside the domain on which higher averages are used. The proof does not manufacture a globally defined \(M^pU\) there. For an old constrained bond \(c\) at level \(r\), consider only the intermediate bonds and paths occurring in the actual iterated expression for \(M^rU(c)\). Those intermediate expressions are part of the source's definition of that constraint. On portions of this cone outside the varied collar, the input links coincide. On its remaining portions, Lemma JR.1 is applied using the shell data. Every equality needed for that old constraint is therefore obtained without any new averaging in unrelated bad regions.

### 4. The source joined tuple and the inclusion of old constraints

The full determining tuple of CMP119 (2.2) is

\[
 \Gamma_0=\Omega_1^c,\quad
 \Gamma_r=\Omega_r^{(r)}\setminus\Omega_{r+1}^{(r)}\ (0<r<k),
 \quad\Gamma_k=\Omega_k^{(k)}.
 \tag{JR.7}
\]

Its values are \(M^rU\), by (2.11). The reconstruction in (2.35) is written

\[
 U_{p,X}(M^\bullet U)
 =U\bigl(B_p(X)\cup\{\Gamma_i\}_{i<p},M^\bullet U\bigr).
 \tag{JR.8}
\]

The two operations involved here have to be kept separate:

1. Truncation at \(p\) retains the old determining shells below \(p\), and fills the remaining last region with level-\(p\) determining data.
2. Localization to \(X\) introduces the source fine collar and the proper-scale boundary splice. The exact splice is (2.14): the old determining set is retained in the interior and the local set supplies the collar. Its generalized version treats each admitted boundary-layer patch separately.

Under this operational reading of (JR.8), the completed localized history has depth at most \(p\). Its interior retains every old shell below \(p\); where a boundary splice replaces an old determining block, it uses that block's scale or finer scales. In particular it refines, rather than coarsens, the old data below \(p\). The source-tuple identification has not been independently established from the displayed notation. The construction below proves a result for the explicitly completed splice, and must not be read as having settled that identification.

#### 4.1 An explicit determining-set dictionary for that identification

Complete the old truncated sequence by

\[
 \Omega^{[p]}_i=\Omega_i\quad(1\le i\le p),\qquad
 \Omega^{[p]}_{p+1}=\varnothing,
 \qquad
 \Gamma^{[p]}_i=\operatorname{st}_i\Omega^{[p]}_i
                  \setminus\operatorname{st}_i\Omega^{[p]}_{i+1}.
 \tag{JR.11}
\]

The level-zero exterior is included as in (JR.7). In particular,
\(\Gamma^{[p]}_i=\Gamma_i\) for \(i<p\); the last set fills the old \(\Omega_p\) with level-\(p\) data.

For one admitted boundary patch lying in old layer \(n\), put \(r=\min(n,p)\). Let \(C_r\) denote its actual proper-scale collar in the source construction, and \(I\) the retained interior. Let \(\Lambda^{\mathrm{loc},r}_i\), \(0\le i\le r\), be the determining sets of the source local depth-\(r\) problem on that patch. Formula (2.14) gives, component by component,

\[
 \widehat\Gamma_i
  =\bigl(\Gamma^{[p]}_i\cap I\bigr)
    \cup\bigcup_{r\ge i}
       \bigl(\Lambda^{\mathrm{loc},r}_i\cap C_r\bigr).
 \tag{JR.12}
\]

The intersections are taken in the scale of the indicated determining variable. For multiple boundary layers, the source explicitly prescribes the sum of the corresponding right-hand sides. Equation (JR.12) records that prescription; it is not an intersection of two independently invented domain sequences. The fixed exterior supplies the remaining level-zero set.

The completed nested physical domains can be recovered from their determining **sites** by

\[
 \widehat\Omega_i
 =\bigcup_{s=i}^{p}\ \bigcup_{y\in\widehat\Gamma_s^{\mathrm{sites}}}
                  \operatorname{cell}_s(y),
 \qquad 1\le i\le p,
 \qquad \widehat\Omega_{p+1}=\varnothing.
 \tag{JR.13}
\]

Here \(\operatorname{cell}_s(y)\) is the physical block of side \(h_s\); faces are assigned by the common source convention. The determining bond sets are then the differences of the stars of these domains, not stars of site-shell differences. The validity and block compatibility of this admitted local geometry are the source's construction (2.13)–(2.15).

The mesh comparison can now be checked by cases. An interior determining cell is an old truncated cell, so its level is the old level, capped at \(p\). A collar cell in \(C_r\) has a level at most \(r\). If that patch lies in old layer \(n<p\), then \(r=n\), so no collar cell is coarser than the old cell there. If \(n\ge p\), then \(r=p\), so the same conclusion holds. Across an old layer boundary, the source uses the contributions restricted to each side; no cell from the coarser-side list is assigned to the fine side. Once the point sets have been formed, a bond crossing that boundary is assigned by the star-difference convention, so it is not silently counted as a datum on both sides. This proves the domain inclusion required for the constraint argument:

\[
 \widehat\Omega_i\subset\Omega_i\quad(1\le i\le p).
 \tag{JR.14}
\]

The associated datum at every retained or newly exposed determining bond of level \(i\) is the same \(M^iU\) evaluated on that bond. There is no averaging of the already assigned heterogeneous tuple, and no substitution of the minimizing field for that datum.

The remaining identification question is narrow: (JR.12) is the source localization of the explicitly completed truncated history, and gives the desired constraint inclusion. The notation (JR.8) must denote that history, with these data, for the result to apply to the displayed B-domain. Its incomplete old-family notation and reversed join order are why this point remains a premise. LFR II uses the same localization join in the reversed order \(B(Y)\cup B_k\), so argument order alone cannot distinguish two maps; that observation does not replace the componentwise dictionary above. Although the lower determining site shells uniquely determine the domains \(\Omega_1,\ldots,\Omega_p\) of a depth-\(p\) completion, this uniqueness alone does not specify how that completion is combined with the collar in the notation (JR.8).

The resulting constraint inclusion has a direct verification. Clamp a local competitor to \(U\) outside the localized fine collar, and call the patched field \(\widetilde W\). For old indices \(r<p\), Lemma JR.1 and (JR.14) give

\[
 \operatorname{supp}(M^r\widetilde W-M^rU)
 \subset\operatorname{st}_r\widehat\Omega_{r+1}
 \subset\operatorname{st}_r\Omega_{r+1},
 \tag{JR.15}
\]

which is disjoint from the old determining bond set
\(\Gamma_r=\operatorname{st}_r\Omega_r\setminus
\operatorname{st}_r\Omega_{r+1}\). For old indices \(r\ge p\), that lemma first fixes every required \(p\)-level intermediate value; iteration (JR.3) then fixes the old \(r\)-level datum. Therefore

\[
 M_{B}\widetilde W=M_BU.
 \tag{JR.9}
\]

There are two boundary checks in this assertion. The local fine collar fixes all links needed to patch the Wilson plaquettes crossing \(\partial X\). Also, an old constrained bond whose endpoint blocks lie wholly outside \(X\) cannot change. If its averaging footprint meets \(X\), its datum or its finer replacement is part of the joined tuple. For \(X\in D_j\) and \(p\le j\), the source carrier is a union of current \(j\)-scale cubes, hence is aligned with the finer block partitions used in this check; the layer-dependent splice retains the additional old-boundary buffers. No estimate of a remote influence is used to replace these exact boundary data.

For \(p=0\), the local tuple consists of fine data and the reconstructed connection equals the supplied connection directly. For \(p=k\), (JR.9) is the ordinary localization of the full old history. The same argument treats components and holes of an admitted carrier: all component boundary collars are clamped. A component with no active interior has no variable competitor.

### 5. Consistency of true constrained minima

#### Proposition JR.2 — consistency on the actual minimal family

Assume the source joined tuple has the constraint inclusion (JR.9), and let \(U=U_B(V)\) be a real, regular critical configuration of the original Wilson variational problem. Then its restriction, in the corresponding gauge orbit, is the regular critical configuration for the joined problem with its own determining data \(M^\bullet U\).

**Proof.** The point \(U\) belongs to the joined regular class: the new determining mesh is no larger than the old mesh, and the absolute small-field estimates required for the local variational theorem are therefore weaker than the old estimates, after the fixed unit conversion (JR.1). Consider any sufficiently small differentiable variation through the joined constraint fiber at \(U\). Patch it to \(U\) outside the fine collar. Equation (JR.9) makes this a variation through the original constraint fiber. At each finite cutoff, sufficiently small variations stay in the original open regular class. Their Wilson first variations vanish because \(U\) is critical there.

The localized and original first variations agree: every potentially affected boundary plaquette is fixed by the fine collar. Thus \(U\) is critical in the joined problem. The uniqueness of the regular critical orbit in CMP102 Theorem 1 identifies it with the joined minimum. \(\square\)

This proof uses local stationarity and uniqueness, rather than claiming that every globally admissible joined competitor satisfies the stronger old regularity bounds. That latter assertion is unnecessary and would not follow from mesh refinement alone.

For scalar gauge-invariant outputs the identity is exact. For covariant current outputs it is equality after the actual change between the two source gauge representatives. The change is not silently discarded: on real fields its adjoint action is isometric, and on a sufficiently small complex chart its parallel-transport factors must be bounded. A global equality between unrelated axial-gauge representatives is not asserted.

### 6. Complex current variations and the remaining scope distinction

Fix real physical determining data and let \(V(z)\) be the actual unprepared current-coordinate insertion into those data. For real \(z\), the field \(U_B(V(z))\) is a true Wilson minimizing field. Proposition JR.2 therefore applies throughout the real source chart. Both variational maps are holomorphic in the determining variables on the absolute small-field domain supplied by CMP102 Proposition 9. Once the joined determining data are shown to stay in that absolute domain for \(\|z\|_\infty<2P_k\), the finite-dimensional identity theorem extends the gauge-invariant consistency identity to that whole connected complex current tube.

This admission concerns an absolute map radius, before the smaller running B-domain is tested. The existing original-geometry estimate gives relative determining variations of size at most \(C g_kP_k\) when the joined mesh is no larger than the original mesh. Taking the common coupling ceiling small makes this fit the fixed variational-map radius. The finer source weights do not need to be proved by a generic joined current kernel first: on this family the output equals the original minimizing field.

In physical units, the original current estimate \(|\delta J|\le u_nh_n^{-3}\) is stronger than the reconstructed target (JR.2), because

\[
 h_n^{-3}\le h_{\min(p,n)}^{-1}h_n^{-2}.
 \tag{JR.10}
\]

Thus exact consistency removes the fine-collar amplification on the true-minimizer family. The normalized endpoint and age bounds already proved on the original geometry can be retained there, subject to the bounded gauge representative change. The same reasoning permits admissible variations of the original retained determining data, since they still parameterize true minima on the same fixed history.

It does **not** prove equality for arbitrary off-minimum backgrounds \((U,J)\), nor for independently altered preparation kernels. In the source's native extension, an independent \(J\) is a free analytic coordinate and need not equal the physical Wilson current of \(U\). Equality on \(J=J(U)\) is not an identity theorem in that larger space. An original C-05 completion must either prove the required native extension and prepared-domain estimates, or supply a complete actual-boundary derivative argument that does not require this larger intermediate map theorem. Either application requires verification of the stated estimate on its declared domain.

### 7. A bounded anchored transport gauge, with its matching condition exposed

There is an elementary local gauge construction that resolves the size of a gauge converter once the reconstructed representative is known to obey the corresponding transport condition. It does not require a bound on a generic second derivative of a covariance. The distinction between constructing this gauge and identifying the source's chosen gauge is essential.

Let a complete admitted determining history partition its active sites into aligned blocks \(B_s(y)\), whose roots \(y\) are determining sites. The block has physical side \(h_s\). Fix in each block a path \(\gamma_{yx}\) from its root to each fine site \(x\), with length at most \(c_dh_s\), contained in that block. The constant \(c_d\) depends only on dimension; coordinate-ordered shortest paths give such a choice. Put

\[
 T_U(y,x)=U(\gamma_{yx}),\qquad
 g_U(x)=T_{U_0}(y,x)^{-1}T_U(y,x),
 \tag{JR.16}
\]

where \(U_0\) is real and \(g_U(y)=1\). For the convention
\(U^g(x,x')=g(x)U(x,x')g(x')^{-1}\), products telescope and give

\[
 T_{U^{g_U}}(y,x)=T_{U_0}(y,x).
 \tag{JR.17}
\]

Thus (JR.16) is an explicitly defined, anchored relative transport gauge. All its operations are holomorphic wherever the input fields are holomorphic.

#### Proposition JR.3 — constraint preservation and a uniform local bound

Suppose \(U=\exp(iaA)U_0\), with \(U_0\) group valued and

\[
 \delta_{s,y}=c_dh_s\sup_{b\subset B_s(y)}\|A(b)\|<\delta_*.
 \tag{JR.18}
\]

Then

\[
 \|g_U(x)\|,\ \|g_U(x)^{-1}\|\le e^{\delta_{s,y}},\qquad
 \|g_U(x)-1\|\le e^{\delta_{s,y}}-1.
 \tag{JR.19}
\]

The gauge preserves every actual determining datum:

\[
 M_{\widehat B}(U^{g_U})=M_{\widehat B}(U).
 \tag{JR.20}
\]

**Proof.** Expand a path product by inserting \(\exp(iaA)\) on each edge and move the baseline unitary transports to the outside. The remaining factors are exponentials of unitary conjugates of the edge perturbations. Submultiplicativity bounds their product and its inverse by
\(\exp(a\sum_{b\in\gamma}\|A(b)\|)\). A telescoping expansion of the difference from the baseline bounds it by the same exponential minus one. The length bound gives (JR.19). Reversed edges obey the same estimate, because the corresponding baseline conjugation is unitary.

For (JR.20), first observe that the two endpoints of every determining bond are determining roots, possibly at different levels. Indeed, a level-\(r\) determining bond lies in
\(\operatorname{st}_r\widehat\Omega_r\setminus
\operatorname{st}_r\widehat\Omega_{r+1}\), so neither endpoint lies in the next inner domain. An endpoint in the level-\(r\) site shell is a level-\(r\) root. An endpoint in an earlier shell is a root of that finer shell, because the aligned odd-block lattices are nested. The gauge (JR.16) equals one at all these roots. The exact one-step group average is equivariant under endpoint gauge transformations, and composition preserves that property. Every prescribed iterated average therefore has unchanged endpoints and unchanged value. This proves (JR.20). \(\square\)

The same algebra works with any analytic, endpoint-equivariant averaged transport in place of the single path, provided its local perturbation estimate is supplied. CMP99 (3.55)–(3.59) supplies such local estimates for its hierarchical transport variables. It is not necessary to replace those variables by the single-path choice to use the algebra.

If \(A\) has an endpoint-sensitive first variation, direct differentiation of the path product gives

\[
 \|g_U(x)^{-1}D_i g_U(x)\|
 \le C e^{C\delta_{s,y}}h_s
       \sup_{b\subset B_s(y)}\|D_iA(b)\|.
 \tag{JR.21}
\]

Each differentiated edge contributes one factor \(aD_iA\); the sum of the edge lengths is at most \(c_dh_s\). No number of fine links remains after this length normalization. If the old geometry bounds the relative field by \(u_nh_n^{-1}\) and the joined block has \(h_s\le h_n\), (JR.18)–(JR.21) have no factor \(h_n/h_s\). An endpoint exponential remains available when the diameter of the block in the old inverse-mesh metric is bounded, because replacing the distance to an endpoint by the distance to this block changes that distance by a bounded amount. This last statement is a local consequence of the admitted mesh comparison; it does not itself prove the complete carrier and age summations required by C-05.

#### What would identify this converter with the actual reconstructed field

Suppose \(W\) is a reconstructed representative in the same anchored gauge orbit as \(U\), and suppose its exact gauge condition is
\(T_W(y,x)=T_{U_0}(y,x)\). If \(W=U^v\) with \(v(y)=1\), covariance of the transport implies

\[
 T_U(y,x)v(x)^{-1}=T_{U_0}(y,x),
 \qquad v(x)=g_U(x).
 \tag{JR.22}
\]

Consequently (JR.19)–(JR.21) would be the required bounds for that representative change. However, the actual relative axial condition in CMP102 p.280 is referred to CMP99 **pp.75–102**, equation (1.19), a different paper from the background-propagator paper CMP99, 389–434. Its complete formula is not used here. CMP109 (0.14)–(0.16) discusses averaged-contour exponential gauge fixing, but this is not a substitute for checking the exact relative axial condition used for its minimizing maps. Therefore the equality of the actual gauge condition with the hypothesis of (JR.22) remains unproved. Real gauge equivalence and analyticity alone do not provide a uniform complex norm bound.

### 8. Exact current conversion and the remaining nonlinear-chart issue

The physical Wilson current transforms by conjugation. This can be derived without differentiating the gauge in physical space: apply gauge invariance to the first variation of the Wilson action and use invariance of the trace pairing. At a bond whose initial endpoint is \(x\),

\[
 J(U^g)(b)=g(x)J(U)(b)g(x)^{-1}.
 \tag{JR.23}
\]

The same identity holds for the holomorphic extension of that current and for its fixed changes of lattice units. Differentiating with respect to a parameter \(i\), and setting \(K_i=g^{-1}D_i g\), gives the exact formula

\[
 D_iJ(U^g)
 =g\bigl(D_iJ(U)+[K_i,J(U)]\bigr)g^{-1}.
 \tag{JR.24}
\]

It follows from (JR.19) and (JR.21) that an admitted converter with
\(h_s\|D_iA\|\lesssim u_n\) and
\(\|J(U)\|\lesssim\alpha_nh_n^{-3}\) contributes at most
\(C\alpha_nu_nh_n^{-3}\) through the commutator. This has the original physical current weight, and hence the weaker reconstructed weight in (JR.2). There is no spatial derivative of \(g\) in (JR.23) and no extra fine-collar factor in this calculation.

Equations (JR.23)–(JR.24) concern the actual physical current. If a proof instead uses a different current coordinate or a quadratic-Hessian current, it must still identify that coordinate with the source's nonlinear current and bound the conversion. An independently extended source current \(J\) is not made equal to \(J(U)\) by this calculation. Thus the transport identity removes a potential nonlinear-current loss **after** the actual representative and physical graph have been identified; it does not complete that identification or the independent-current extension.

### 9. Application conditions for C-05

The advances and their exact scopes are:

| Result | Status | Limitation |
|---|---|---|
| Same physical fine graph under the \(j\)- and \(p\)-unit conventions, (JR.1)–(JR.2) | Checked against source scale factors | Fine collars remain present. |
| Nonlinear shell-support induction, Lemma JR.1 | Proved for the actual endpoint-block average and admitted complete histories | Uses the actual star-difference bond convention and defined dependency cones. |
| Constraint inclusion for the explicit completed splice, (JR.11)–(JR.15) | Proved under the source's admitted patch geometry | The notation (JR.8) has not been independently identified with that splice. |
| True-minimum consistency, Proposition JR.2 | Proved implication | Needs the exact source-tuple identification, regular admission and fixed boundary patching. |
| Anchored transport gauge and norm bound, Proposition JR.3 | Proved | Its equality with the actual relative axial representative is not checked. |
| Physical-current conjugation and variation, (JR.23)–(JR.24) | Proved | Does not identify an arbitrary independent current coordinate with the physical current. |
| Complete actual B pullback on its common complex current contour | Open | All actual tuple, representative, domain and localization premises must hold together. |

The remaining work for this route is concrete. First, identify the actual joined determining set in CMP119 (2.35) component by component, including its fine exterior data and every admitted mixed boundary patch. Second, obtain the exact relative gauge condition or an equivalent source theorem that supplies a uniformly bounded analytic converter into the actual representative on the full common contour. Third, prove the resulting native background/current extension and the endpoint-localized application to all B sectors. An alternative extension using an independent displacement from the physical current may be useful, but its agreement with the actual activity and its full source-domain admission require proof. These are additional hypotheses, not consequences of the shell-support identity.

Neither C-05 nor BM.24 is proved here.

### 10. Sources

- CMP119 (1988), 243–285, (2.2), (2.10)–(2.15), (2.34)–(2.39), and pp.276–277. Printed pp.255–257 and 261 give the determining sets, the tuple and the scale factors.
- CMP102 (1985), 277–309, (1)–(7), Theorem 1, and Proposition 9. The uniqueness assertion is for the regular critical orbit on the source's fixed determining geometry.
- CMP99 (1985), 389–434, (3.15), composition of the actual averaging derivatives; the nonlinear averaging operations referred to there are the iterated operations.
- CMP96 (1984), 223–250, printed p.224, (2.3): the determining sets use the set difference for sites and bonds separately. This is the source of the star-support convention used in the induction.
- CMP109 (1987), 249–301: (0.11)–(0.12), the geometric scaling discussion at p.257, and (1.15)–(1.16). DOI https://doi.org/10.1007/BF01215223.
- The gauge-condition source is Balaban, *Spaces of regular gauge field configurations on a lattice and gauge fixing conditions*, CMP99 (1985), 75–102, DOI `10.1007/BF01466594`. Its equation (1.19) is not used here, so the identification of the actual gauge condition remains a hypothesis.
