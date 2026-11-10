# M-04: exact scalar identification, bounded extraction, and the action-minimum test

This note does **not** claim the full M-04 bound. It fixes the scalar normalization, gives a useful finite-rank extraction theorem with its actual hypotheses exposed, and records the primary-source facts needed for testing the specified ambient norm at a hard selector. No final running normalization is assumed.

## 1. The F-01 scalar is exactly the Wilson action density

The Annex X, equations (F.4)–(F.7) and (F.17), fixes

\[
 e_S=I_6/\sqrt6,\qquad
 \sigma_h(x):=\langle e_S,\widetilde q_h(x)\rangle
 =\frac{2}{\sqrt6}w_h(x),
\]

\[
 w_h(x)=\frac1{4h^4}\sum_{\mu<\nu}\sum_{\epsilon,\epsilon'=\pm1}
 s(P_{\epsilon e_\mu,\epsilon'e_\nu}(x)),
 \qquad s(P)=N-\operatorname{ReTr}P.
\]

Consequently

\[
 h^4\sum_x\sigma_h(x)=\frac2{\sqrt6}S(U),\qquad
 S(U)=\sum_ps(U_p).                                            \tag{SE.1}
\]

There is no clover-to-plaquette approximation in this channel. The scalar repair in F-01 makes (SE.1) exact. For the energy-normalized coordinate use

\[
 \varphi_h(x)=\beta_h\sigma_h(x).
\]

This is a scalar multiple of the fixed F-01 representative, not a change of observable. If the fixed incoming F-01 scalar coefficient is \(z_S^{\rm in}>0\), the same basis element is \((z_S^{\rm in}/\beta_h)\varphi_h\). A coefficient relative to \(\varphi_h\) converts to that basis by multiplication by \(\beta_h/z_S^{\rm in}\). This conversion exposes the given input normalization; it does not assume any F-05 bound.

## 2. An explicit nonzero scalar probe

Take a periodic lattice large enough that the elementary plaquettes in a scalar stencil do not wrap onto themselves. Let every link equal the identity except the link \(e=(x,x+he_0)\), and put

\[
 U_e=\exp\bigl(tH/\sqrt{1+\beta_h}\bigr),\qquad
 H=\frac{i}{\sqrt2}\operatorname{diag}(1,-1,0,\ldots,0),
 \quad 0<t\le\tfrac14 .                                    \tag{SE.2}
\]

The generator is anti-Hermitian, traceless and has Hilbert–Schmidt norm one. Exactly six of the 24 oriented plaquettes in \(w_h(x)\) contain this link. The other 18 are trivial. Orientation changes replace the pulse by its inverse and leave \(s\) unchanged. Hence

\[
 h^4\varphi_h(x;U^{(1)})
 =\sqrt{\frac32}\,\beta_h\,
 2\left[1-\cos\left(\frac{t}{\sqrt{2(1+\beta_h)}}\right)\right]
 =:d(\beta_h,t).                                             \tag{SE.3}
\]

At the all-identity datum \(U^{(0)}\), \(\varphi_h=0\). Using
\(1-\cos u\ge u^2/4\) for \(|u|\le1\),

\[
 d(\beta_h,t)\ge
 \sqrt{\frac32}\frac{\beta_h t^2}{4(1+\beta_h)}
 \ge \sqrt{\frac32}\frac{t^2}{8}
 \quad(\beta_h\ge1).                                        \tag{SE.4}
\]

The upper bound \(1-\cos u\le u^2/2\) also gives a fixed upper bound. Thus this finite probe separates the scalar from the identity at uniform energy-normalized cost. Averaging the probe over the finitely many signed coordinate directions gives a hypercubic-symmetric extraction functional; the scalar denominator is unchanged. Global color conjugation may also be averaged without changing the denominator.

## 3. A bounded extraction theorem, conditional only on explicit norm data

This section is a theorem about the existing M-03 space. It does not prove that the actual conditional kernel maps its input into that space.

Let \(\mathbf A_X=(A_X,B_X,J_X)\) be a genuine compatible first-order output carrier at current spacing \(h\), and suppose the complete output has already been proved to have finite M-03 norm at spatial rate \(\kappa+\delta\), \(\delta\ge0\). All carriers contain the insertion anchor. Let \(S\) be the fixed carrier of \(\varphi_h\). Use the all-reference ambient datum \(v_0\) and the pulse datum \(v_1\) from (SE.2), with all other padded coordinates fixed to their reference values.

Define, separately for every tagged output carrier,

\[
 c_X=A_X(v_0),\qquad
 a_X=\frac{h^4[A_X(v_1)-A_X(v_0)]}{d(\beta_h,t)},               \tag{SE.5}
\]

\[
 \mathcal R_X=A_X-c_X-a_X\varphi_h,
 \quad B_X^{\mathcal R}=B_X-a_X\delta\varphi_h,
 \quad J_X^{\mathcal R}=J_X.                                 \tag{SE.6}
\]

Every scalar and constant in (SE.5) is field-independent. Therefore

\[
 \delta\mathcal R_X=B_X^{\mathcal R}+J_X^{\mathcal R}           \tag{SE.7}
\]

exactly. All existing kernel-current records are retained, even if they cancel against some part of the direct record. Assign the residual and subtractions to \(X\cup S\). Since \(X\) and \(S\) share the anchor,

\[
 w_{h,\kappa}(X\cup S)\le w_{h,\kappa}(X)w_{h,\kappa}(S).      \tag{SE.8}
\]

Suppose the following two numerical data have been established for the actual native coordinate list and actual outer law:

\[
 \widehat R_{h,X}(v_i)\le C_R(1+|X|)^r,\quad i=0,1,            \tag{SE.9}
\]

and the canonical scalar triple has its local budget

\[
 v_{h,1,S}(\varphi_h)+g_{h,1,S}(\delta\varphi_h)\le C_S.       \tag{SE.10}
\]

For \(r=0\) no spare spatial rate is needed. For \(r>0\) take \(\delta>0\). Then

\[
 \sum_Xw_{h,\kappa}(X\cup S)
 \left(|a_X|+h^4|c_X|
 +v_{h,1,X\cup S}(\mathcal R_X)
 +g_{h,1,X\cup S}(B_X^{\mathcal R})
 +j_{h,1,X\cup S}(J_X^{\mathcal R})\right)
 \le C\|\mathbf A\|_{h,\kappa+\delta},                       \tag{SE.11}
\]

where \(C\) depends on \(C_R,C_S,r,\delta,t,\kappa,S\), not on scale, volume or the number of tagged carriers.

### Proof

The pointwise term of (M.11) bounds

\[
 h^4|A_X(v_i)|\le
 \widehat R_{h,X}(v_i)\,v_{h,1,X}(A_X).
\]

Equations (SE.4)–(SE.5) yield

\[
 |a_X|+h^4|c_X|
 \le C C_R(1+|X|)^r v_{h,1,X}(A_X).                           \tag{SE.12}
\]

A constant placed on the anchor has normalized value cost at most \(2h^4|c_X|\), since \(\mathfrak m_1(1)=1\) and \(\widehat R\ge2\). The enlarged union regulator dominates the scalar stencil regulator. Thus (SE.10) bounds the subtracted scalar triple by \(C_S|a_X|\). Apply the triangle inequality to (SE.6), then (SE.8). Finally use

\[
 (1+n)^r\le C_{r,\delta}e^{\delta n},\qquad
 w_{h,\kappa}(X)e^{\delta|X|}\le w_{h,\kappa+\delta}(X).
\]

This proves (SE.11) and absolute convergence of the displayed decomposition. The exact sum represents the original \(A=\sum_XA_X\), never a freshly inserted coarse field. ∎

### The scope of this extraction theorem

The theorem is useful because, once the genuinely difficult actual output bound is known, scalar/identity extraction need not require a new nondegeneracy theorem or differentiation of that output. The finite probe and its denominator are explicit. It is also honest about the two norm facts required:

* For an independent native list of plaquettes formed from raw links, with uniformly bounded link-to-plaquette incidence and comparable inverse-coupling labels, (SE.9) holds with \(r=0\). At a reference or pulse datum an elementary shift excites only a bounded number of native energy terms, each at bounded normalized cost. The same holds for independent dimensionless Euclidean slots. The supremum in \(\widehat R\) permits only one further elementary shift, not a sum of simultaneous shifts.
* An extensive list of reconstructed old plaquettes can violate that uniform incidence premise. The theorem does not silently identify those with independent native links. Its actual incidence and coefficient ratios must be checked, or the growth in (SE.9) must be paid by the spare carrier rate.
* The microscopic version of (SE.10) is Proposition M.1. On a later actual outer law, its averaged part requires the actual coarse/native energy reserve. Compactness alone gives finite but coupling-dependent bounds.
* A finite-probe extraction is a concrete complementary projection onto the fixed F-01 scalar and identity directions. The M-04 statement fixes that incoming basis and requests an exact decomposition with a bounded remainder; it does not specify a unique Taylor or separated-measurement projector for an arbitrary output. Thus this construction supplies its algebraic extraction once the actual operator norm has been proved. F-01's physical measurements normalize the basis itself. A different coefficient prescription required by a later F-03/Gamma calculation would need its own scheme comparison there, not as an additional M-04 requirement. Average the pulse functional over the finite signed coordinate-permutation group at the anchor, and translate it with the anchor and blocking convention, to make the projector covariant. The denominator and bounds are unchanged.

No claim of M-04 closure follows from (SE.11) without the actual output bound and (SE.9)–(SE.10).

## 4. Primary-source resolution of the Wilson-versus-soft-gauge question

A proposed hard-selector test compares the mean of the exact Wilson scalar on a regular fluctuation fiber to the scalar at its reference input. One must not infer a Wilson-action minimum merely from a minimum of Wilson action plus a positive soft-gauge action.

The relevant stronger statement is present in the primary sources:

1. Bałaban, *The Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*, CMP **102** (1985), 277–309, printed p.278, equations (2)–(6), defines the regular field class and fixed-average fiber. The regular class is gauge invariant. The fixed-average fiber is invariant under gauge transformations equal to the identity at the retained coarse sites, equation (4).
2. Theorem 1, printed p.279, constructs a **minimal orbit of the Wilson action itself**, not a minimum of an augmented gauge action, in that regular fiber and states uniqueness of its critical orbit in the small domain.
3. Section A, printed pp.280–281, explicitly uses those center-fixed gauge transformations to put arbitrary configurations in the fiber into the axial slice, without changing the Wilson action. Equations (18)–(21) identify that reduction.
4. Section E, printed p.299, equations (141)–(142), identifies the constrained positive quadratic variation at the background. Non-gauge constrained fluctuations have positive action variation. The nonlinear small-chart remainder is retained in that source analysis.
5. CMP **119** (1988), printed p.248, equation (1.12), defines \(U_1\) as the stationary point of Wilson plus soft gauge action but immediately states that on the axial slice it is the stationary point of Wilson action alone and explicitly invokes the preceding variational theorem. Thus its physical background is the Wilson minimal orbit; the soft gauge factor fixes its representative and weights gauge coordinates.

For an actual first regular step, the remaining application check is that its entire regular conditional support lies in the variational small-field class to which this minimum statement applies. One cannot omit this domain check just because both formulas use the word “small.” In the wholly regular first-step chart, the source's independent fluctuation cutoffs and the small background bounds are the concrete inputs for that check. The coarse selector margin must remain inside the larger variational chart.

## 5. Strict action-mean and selector-jump lemmas

The following elementary implications isolate exactly what is needed in that application.

### Lemma SE.1 — strict mean above the physical minimum

Let \(q_v\) be the actual positive normalized conditional measure on a regular finite Wilson fiber. Suppose \(U_*(v)\) is the Wilson-action minimum on its entire support, and suppose a set of positive \(q_v\)-measure consists of non-gauge fluctuations with
\(S(U)>S(U_*(v))\). Then

\[
 q_vS-S(U_*(v))>0.                                         \tag{SE.13}
\]

The proof is integration of a nonnegative function which is strictly positive on a set of positive measure. In the source's finite positive coarea density, a nonempty open set of non-gauge fluctuations has positive measure. Soft gauge weights are strictly positive and do not remove that set. They do not alter the gauge invariance of \(S\).

For the microscopic centered scalar family \(F_x=\alpha\beta\sigma_h(x)-c\) with \(\alpha\ne0\), (SE.1) implies

\[
 h^4\sum_x\bigl(q_vF_x-F_x(U_*(v))\bigr)
 =\alpha\beta\frac2{\sqrt6}
   \bigl[q_vS-S(U_*(v))\bigr]\ne0.                           \tag{SE.14}
\]

Thus at least one actual local scalar has a nonzero conditional-reference mismatch. No sign claim for every individual plaquette is needed. If the inactive extension sends the whole old configuration to identity instead, the positivity argument is even simpler: \(S\ge0\), its reference value is zero, and positive-measure physical fluctuations give strictly positive mean.

### Lemma SE.2 — a nonzero jump cannot have finite M-03 current norm

Let an allowed continuous elementary retained coordinate cross a hard active-sector boundary at \(v_*\). Suppose the active conditional scalar value has a finite one-sided limit \(A_+\), the fixed inactive reference version has value \(A_-\), and \(A_+\ne A_-\). Assume the native regulator is finite at \(v_*\), as it is at each finite compact/raw-coordinate datum. Then the M-03 norm of every compatible representation of this output is infinite.

Indeed, along the crossing direction,

\[
 \left|\frac{A(\tau_t v_*)-A(v_*)}{t}\right|\longrightarrow\infty.
\]

For every compatible representation,
\(\delta A=\sum_X(B_{X,\tau}+J_{X,\tau})\).
At a fixed finite cutoff, the full native list is finite and the ambient block graph is finite. Thus every carrier regulator at this datum is bounded by the one full-torus shifted regulator \(\widehat R_{h,\mathrm{all}}(v_*)<\infty\). The pointwise terms of (M.11), \(w_h(X)\ge1\), and absolute summation then give the explicit bound

\[
 |\delta_\tau A(v_*)|\le h^{-4}(3/2)^{3/2}
 \widehat R_{h,\mathrm{all}}(v_*)^{3/2}
 \|\mathbf A\|_{h,\kappa}.
\]

This bound is independent of the crossing increment \(t\), so it contradicts the displayed divergence. Equivalently, for any finite representation the triangle inequality forces at least one summed direct/current envelope to diverge; the absolutely summable case follows from the same norm bound.

Subtracting a finite constant and a continuous fixed coarse scalar does not change the jump. Thus the extraction in Section 3 cannot repair this failure. A history-dependent discontinuous “identity coefficient” would merely move the same response into another marked record; it is not a finite scalar constant in the fixed basis, and its current must be retained.

This lemma is an exact consequence of the specified (M.1), (M.4), (M.7), (M.11) conventions, which take ambient suprema and include arbitrarily small divided coordinate shifts. It is not a claim that every possible continuation of an inactive kernel has such a jump. The chosen continuation matters.

## 6. Status

The full actual M-04 theorem is not proved here. The scalar identity and pulse denominator are exact. The extraction theorem is proved with explicit regulator and scalar-budget inputs. The primary-source minimum facts resolve the potential soft-gauge confusion, while the actual selector obstruction still requires its support/extension/crossing identifications. If those identifications are established, a finite-cutoff jump disproves bounded transport in the original strong norm; no improvement of an ordinary conditional moment estimate can repair that particular failure. A changed ambient continuation or a norm with boundary-current measures would be a new, explicitly stated interface, not closure of the unchanged specified one.

## 7. Analysis of the coarse-selector crossing

This section analysis the concrete crossing construction proposed in [support analysis](support_analysis.md). The construction works at its stated default-version scope, with the following quantitative and domain details included.

### 7.1 Where the local constraint really is imposed

The scan of CMP119 p.246 prints

\[
 U_{1,D'}(V)=U\bigl(\mathcal B_1(D'^{\sim4}),
                    M^\bullet(Q_1^{s*}V)\bigr)                 \tag{SE.15}
\]

in (1.2), not a bare formula \(U_{1,D'}(V)=U(V)\). Its (1.3) puts the lifted field \(Q_1^{s*}V\) equal to identity on intrablock bonds and equal to \(V(c)\) on interblock bonds over the coarse bond \(c\). Every averaging path crosses that interblock interface once, so its coarse average is exactly \(V\). The linearization has the same right-inverse property.

CMP119 p.256 (2.11) defines the determining-set readout by \(M_{\mathcal B}U=M^jU\) on \(\Gamma^j\). The minimal determining set based on a domain retains its last-scale interior beyond a collar of only \(2M_1\) in the indicated lattice units (p.256, text following (2.12)). Hence for \(\mathcal B_1(D'^{\sim4})\) a coarse plaquette deep inside \(D'\), including all its averaging paths, lies in the last-scale interior. On those bonds the actual local minimizer therefore satisfies the exact coarse constraint with datum \(V\).

One must choose the perturbed coarse bond and an adjacent coarse plaquette in this interior, rather than at a partition seam. The cube scale in the source is much larger than the fixed one-step averaging stencil, so this is available on a compatible sufficiently large torus.

### 7.2 A quantitative flat curl test

Let \(v\) be a Lie-algebra-valued coarse one-form supported on that single coarse bond, with nonzero oriented curl around an adjacent coarse plaquette. Let
\(V(t)=\exp(tv)\). The background maps are analytic in their native chart (CMP102, pp.305–307, (172)–(181)); write the linearized local minimizer as \(B_{D'}\). The preceding exact constraint gives

\[
 Q B_{D'}=v
\]

on the interior coarse bonds. Here \(Q\) is the fixed one-step flat linear averaging operation of CMP98, p.19 (14), obtained by differentiating its nonlinear average (15); the first sentence of p.20 confirms this linearization. Gauge covariance is (11).

It is preferable to use a quantitative local Stokes bound, rather than merely saying that a nonzero coarse curl forces a nonzero fine curl. On the finite simply connected fine-lattice box containing the coarse plaquette's averaging paths, the functional \(\ell(B)=d(QB)\) annihilates all gradient one-forms: this follows either directly from the endpoints of those paths or by differentiating gauge covariance. The annihilator of the kernel of the fine coboundary \(d\) is the range of its transpose. Thus, componentwise in the color algebra, there is a fixed finite plaquette cochain \(c\) such that

\[
 d(QB)=\sum_{p\in\mathcal P_L}c_p\,dB(p),\qquad
 |d(QB)|\le C_L\max_{p\in\mathcal P_L}|dB(p)|.                \tag{SE.16}
\]

The coefficients and \(C_L=\sum_p|c_p|\) depend only on the fixed averaging operation and blocking factor \(L\), not on \(R_1\), the large cube or torus. The set \(\mathcal P_L\) is contained in the tested \(D'^{\sim}\) when the coarse plaquette is chosen as above. Since \(d v\ne0\), (SE.16) yields a nonzero fine-curvature derivative with a lower bound uniform in the large localization cube.

The complete good-field test is the maximum of finitely many continuous plaquette norms of analytic local minimizing fields. Consequently, for \(t>0\) small,

\[
 f(t):=\max_{D',\,p\subset D'^{\sim}}
       |U_{1,D'}(V(t),\partial p)-1|
       =c t+O(t^2),\qquad c\ge c_L>0.                       \tag{SE.17}
\]

The analytic-domain estimates make the remainder uniform on the source's small neighborhood. For sufficiently small threshold \(r=\epsilon_1L^{-2}>0\), there is a crossing at
\(t_*=r/c+O(r^2)\), with good field below and bad field above. The chosen one-parameter group direction is an elementary retained direction after the constant normalization in (M.3). Arbitrarily small crossing increments have magnitude at most one in that normalized coordinate. The crossing stays within the larger analytic domain.

The inequality \(c\ge c_L\), rather than just \(c>0\) at each finite volume, matters: it prevents the crossing from escaping the analytic buffer as the source localization radius changes.

### 7.3 Other selectors and the actual reference value

The wholly first-step regular branch has no old E/B/R history factors. All its actual coarea, Haar and soft-gauge factors remain in its positive finite density. The regular free-coordinate domain has nonempty interior. CMP119 pp.248–251 removes redundant old fine selectors and replaces the approximate fluctuation tests by the final independent free-coordinate cutoffs. The choice \(A_0\gg A_1\), the small background threshold and the exponentially close local/global backgrounds leave strict room for those fine, gauge and approximate-fluctuation tests on a smaller nonempty free-coordinate ball. Thus crossing the *outer retained* selector does not collapse the regular fluctuation integral. At the crossing the same native positive integral is well-defined on the larger buffered chart.

There are two reference conventions to distinguish.

* Crossing the outer retained good-field selector while remaining inside the reconstruction chart invokes M.1's reference **kernel input**. In the independent fluctuation coordinates its value is \(A=0\), so the reconstructed configuration is the background \(U_1(V)\).
* If the reconstruction chart itself is left, M.1 also assigns the old-state reference configuration to the map. That is a different boundary and a different reference value, usually identity. The coarse-selector proof uses the first case and does not need the second case.

The existence of a physical fluctuation is also explicit. On a four-dimensional periodic first-step lattice with \(n_f\) fine sites and \(n_c=n_f/L^4\) coarse sites, the derivative of the coarse readout is surjective by its right inverse. Thus its constrained tangent space has dimension \(4(n_f-n_c)\dim G\). Center-fixed gauge directions have dimension \((n_f-n_c)\dim G\), since a gauge transformation fixed at all coarse centers has no nontrivial infinitesimal constant stabilizer. The quotient therefore has dimension \(3(n_f-n_c)\dim G>0\) for \(L>1\). Exceptional-bond elimination and small-chart continuity preserve these ranks. Hence the fluctuation integral is not confined to the minimal gauge orbit.

At fixed finite coupling the native conditional density is positive on its fixed product domain and varies continuously in \(V\) in the buffer. Its normalizer has a positive continuous limit. Dominated convergence therefore gives the native active-side scalar limit. The reference extension gives the background value on the inactive side.

The exact Wilson minimal-orbit statement is especially clear in CMP119 p.256, (2.12): the paper calls it the **set of minima** of the Wilson action on regular configurations with the given determining-set readout. This is independent of the soft-gauge weight in the chosen coordinate representative. On the small first-step support, with a non-gauge fluctuation direction present, Lemma SE.1 supplies a strictly positive action mismatch, and (SE.14) produces a nonzero jump in at least one actual local scalar. Lemma SE.2 then rules out a finite M-03 current norm for the default extension.

This analysis establishes a defect of that specified ambient version. It does not disprove a one-step bound for a different explicitly recorded buffered extension. The physical Wilson conditional expectation is unchanged by changing its values on inactive ambient data, but the strong ambient M-03 norm is changed, so that repair must be stated.

### 7.4 A shorter nonlinear crossing proof

A primary-source inequality removes the need for the Taylor expansion in Section 7.2. CMP98, printed pp.24–26, (44) and Proposition 1, (50)–(51), proves the local implication

\[
 \max_{p\subset\Delta(p')}|U(\partial p)-1|\le a
 \quad\Longrightarrow\quad
 |\overline U(\partial p')-1|
 \le L^2a+C_0(L^2a)^2.                                    \tag{SE.18}
\]

The proof expressly says that only the fine plaquettes in the fixed averaging neighborhood \(\Delta(p')\) are used. Choose the coarse plaquette in the determining-set interior as in Section 7.1. If all the source good tests hold, then for the corresponding local minimizing field one may put \(a=\epsilon_1L^{-2}\). Its exact coarse constraint and (SE.18) imply

\[
 |V(\partial p')-1|\le\epsilon_1+C_0\epsilon_1^2.              \tag{SE.19}
\]

Now choose the single coarse-link pulse to have
\(|V(\partial p')-1|=2\epsilon_1\), with \(C_0\epsilon_1<1\). The pulse and the path from identity to it stay in the larger variational chart for sufficiently small coupling. Equation (SE.19) proves that this endpoint cannot have every good test. Let \(f(t)\) be the continuous maximum of all the test curvatures along that path and let \(t_*\) be the first time \(f(t)\ge\epsilon_1L^{-2}\). Then \(f(t)<\epsilon_1L^{-2}\) before \(t_*\) and equality holds at \(t_*\).

That equality point suffices. The good selector in CMP119 (1.4) uses a strict inequality, so its value is zero at \(t_*\). The default reference kernel is therefore used there, while active points approach it along the same elementary retained-link direction. The nonzero conditional-reference mismatch at \(t_*\) makes the divided difference diverge. No open interval on the bad side, regularity of the boundary stratum, or uniform transversality estimate is needed.

This nonlinear argument is the preferred crossing proof. Section 7.2 remains a useful independent consistency check on the local geometry and the scale of the boundary.
