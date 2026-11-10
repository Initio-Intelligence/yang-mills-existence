# Heterogeneous constrained coercivity, conditional on the boundary estimate

**Annex AI.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Conditional statement and inputs

The unchanged C-06 statement is:

> Extend the admitted regular derivative/coercivity estimates to the heterogeneous retained backgrounds and layer geometry actually encountered, with explicit weighted norms and domain margins.

The goal is a uniform estimate on the stated heterogeneous class, with its explicit boundary and regular-action budgets.

This note proves the C-06 implication with those predecessor conclusions as inputs. C-04 has been proved. **C-05 has not been proved.** Accordingly the conclusion for the complete interacting conditional law is conditional on C-05; neither that conclusion nor C-05's boundary budget is asserted unconditionally. The new actual-model checks in this note are the identification and admission of the heterogeneous principal form, its uniform gap and weighted locality in the exact free coordinates, the bulk classical and measure budget on that class, and the common-domain assembly. The elementary matrix perturbation argument by itself would not discharge C-06.

We retain the source-free construction and coupling assumptions of J0/C-01. An independent proof of that input, current-scale means and all-order interacting cumulants, arbitrary retained-coordinate changes, and selector/interface currents are separate obligations.

### 2. Which coordinates are integrated

Fix an admitted cutoff, scale, positive history sector and retained datum \(v\). Use the regular inner expression in CMP119 (3.23)–(3.25), identified directly in C-01. This pointwise Hessian argument does not use C-07 or its support/Neumann theorem; C-07 is a downstream application, so there is no circular dependency. Its variables are the Lie-algebra values of **current-unit free bonds** in \(\Lambda=\Lambda_{k+1}\). Old-layer fields and the exterior current field \(y\) belong to \(v\). They are parameters, not additional coordinates in this integral.

Let \(I\) denote these free bonds and \(D=\dim\mathfrak g\). On the real vector space \((\mathfrak g)^I\) use

\[
 \|z\|_2^2=\sum_{i\in I}|z_i|^2,
 \qquad \|z\|_\infty=\max_{i\in I}|z_i|.
 \tag{HC.1}
\]

The block dimension is fixed. Distances \(\rho_k(i,j)\) are measured on the current-unit lattice, using the shortest periodic lattice distance when appropriate. The free-bond set has at most \(d\) positively oriented bonds per site. Thus there is an explicitly finite lattice-counting majorant

\[
 \mathcal N_d(t)=d\left(1+\frac{2}{e^t-1}\right)^d,
 \qquad
 \sup_i\sum_j e^{-t\rho_k(i,j)}\le C_d\mathcal N_d(t),
 \quad t>0.
 \tag{HC.2}
\]

The harmless fixed \(C_d\) allows the chosen bond-origin convention. Counting shortest representatives of periodic displacement classes proves the same inequality on every torus, including small ones. Restrictions to \(I\) can only reduce the sum.

For block matrices set

\[
 \|A\|_\gamma
 =\max\left\{
 \sup_i\sum_j e^{\gamma\rho_k(i,j)}\|A_{ij}\|_{\rm op},
 \sup_j\sum_i e^{\gamma\rho_k(i,j)}\|A_{ij}\|_{\rm op}
 \right\}.
 \tag{HC.3}
\]

This norm is submultiplicative by the triangle inequality for \(\rho_k\). The two sums agree for a real symmetric matrix. The norm does not insert a fine-lattice coordinate weight into a current-unit coordinate. Heterogeneity remains in the background, determining geometry, and precision matrix.

There is also a genuine layer-weighted norm, used for background admission rather than for the coordinates in (HC.1). With \(h_n=L^n\eta\), use the actual local gauges of CMP99 (3.35)–(3.38) and the quantities

\[
 \|A\|_{\rm lay,2}
 =\sup_n\max\left\{
 h_n\|A\|_n,
 h_n^2\|\nabla A\|_n,
 h_n^3\|d^*dA\|_n
 \right\},
 \qquad
 \|J\|_{\rm lay,J}=\sup_n h_n^3\|J\|_n.
 \tag{HC.4}
\]

If a source chart requires a Hölder norm, append its specified term \(h_n^{2+\beta}\|\nabla A\|_{\beta,n}\). Current extensions are evaluated in their actual independent \(J\) slot. Equation (HC.4) does not assert that a first-derivative bound controls a second derivative; the latter is checked from the variational theorem below. For the reconstructed-output restrictions of B, use C-05's full domain, including its additional \(p,n\) weights. This note does not replace those restrictions by (HC.4).

### 3. Admission of the actual heterogeneous source class

#### Lemma HC.1 — geometry and real background admission

The regular inner domain and real minimizing backgrounds of the retained construction satisfy the hypotheses of the unit-lattice propagator result, uniformly in the remaining admitted history, after one fixed reduction of the coupling ceiling.

**Proof.** Section E of CMP99, pp.427–428, requires \(\Lambda\subset A_k=\Omega_k^{(k)}\), a union of the admitted blocks, separated from \(A_k^c\) by more than the fixed propagator distance \(RM\). CMP119 (3.2)–(3.5), pp.264–265, constructs the next regular region by removing the old bad region and several layers of current-size cubes. The interior used in the Gaussian integral is smaller still. The rectangularization of the bad complement in CMP119 p.251, repeated on p.269, enlarges that complement; it does not enlarge \(\Lambda\) towards \(A_k^c\). Consequently its distance is at least a fixed positive multiple of the running collar width, up to a fixed endpoint offset. Choose the fixed lower admissible running radius so that

\[
 c_{\rm col}L M R_{k+1}-C_{\rm edge}M>RM.
 \tag{HC.5}
\]

The source running radii tend to infinity as the common coupling ceiling is reduced, so this is a uniform fixed-parameter condition. The determining geometries retain the inter-layer separation conditions required by CMP99; they are the admitted geometries in J0, not arbitrary nested sets.

For the background, CMP102 Theorem 1, pp.278–279, gives both its gauge-invariant field/current bounds and, on the proper-scale local gauge cubes, its first- and second-order bounds (9)–(10). In particular it supplies the \(d^*dA\) condition (3.36) of CMP99. A plaquette bound alone would not supply that condition.

Write \(\varepsilon_*\) for a uniform upper bound on the admitted determining-data regularity, after the fixed selection constants are included. For the running thresholds used in the construction a sufficient choice is

\[
 \varepsilon_*=C_{\rm sel}A_0g_*\ell_*^{p_0},
 \qquad \ell_*=\log g_*^{-2}>2p_0.
 \tag{HC.6}
\]

Indeed \(g(\log g^{-2})^{p_0}\) is increasing in \(g\) on that range. Hence every admitted \(g_n\le g_*\) obeys the same bound. Choose \(g_*\) so small that, with the constants in CMP102 Theorem 1 and CMP99,

\[
 \varepsilon_*<a_1/2,
 \quad B_3\varepsilon_*<a_0/2,
 \quad M\varepsilon_*<R_1M_1a_1/2,
 \quad M C_{\rm reg}B_3\varepsilon_*<a_{99}/8.
 \tag{HC.7}
\]

The third condition puts the required local cubes within the range \(M<M(\varepsilon_*)\) of CMP102. The fourth is the smallness required for the background propagators. The fixed constant \(C_{\rm reg}\) accounts for the specified overlap of proper-scale cubes and gauge conventions. All choices are independent of the number of layers, volume, and derivative order. The source places no regularity restriction on the gauge field outside its active background domain; none has been added here. This proves admission of the actual, possibly nonconstant and heterogeneous, real background class. \(\square\)

This lemma retains the source bounds on determining data as part of the admitted source-free construction. It does not independently establish J0, its trajectory, or its history decomposition.

### 4. The principal form is the actual constrained form

The source's free-coordinate precision is

\[
 K_{k,v}=C_{k,v}^*\Delta^{(k)}_{v}C_{k,v},
 \qquad K_\Lambda=(K_{k,v})_{II}.
 \tag{HC.8}
\]

Here \(C\) solves the linearized averaging constraint on its exceptional bonds. The quadratic form \(\Delta^{(k)}\) includes the term involving \(H_1D^{(2)}\) and the background current in CMP99 (3.156). Removing that term would change the constrained Hessian.

The precise primary inputs are CMP99 (3.155)–(3.158), the paragraph after (3.158), and Theorem 3.15. The paragraph after (3.158) states the uniform positive lower bound for the free-coordinate form on arbitrary backgrounds satisfying (3.35)–(3.36), and its uniform exponential locality. The covariance in Theorem 3.15 has exponential decay, and (3.158) identifies its restriction with the inverse free-coordinate precision. Those inputs concern the actual heterogeneous geometry admitted in Lemma HC.1.

Consequently there are fixed \(\lambda_0,K_0,\delta_K>0\), independent of scale, volume, retained datum and admitted history, such that

\[
 K_\Lambda\ge\lambda_0I,
 \qquad
 \|(K_\Lambda)_{ij}\|_{\rm op}
 \le K_0e^{-\delta_K\rho_k(i,j)}.
 \tag{HC.9}
\]

Principal restriction preserves the lower bound and the entrywise estimate. The source estimate is first applied on the full admitted current fluctuation region with its already fixed map \(C\); only then is the free-coordinate matrix restricted to \(I\). The constraints are not re-solved inside \(\Lambda\) after conditioning. This order also covers a free bond whose \(C\)-image contains a neighboring exceptional bond. No translation invariance of \(K\) is assumed.

The map \(C\) introduces no depth-dependent loss. It is local to finitely many current blocks and equals the identity on free bonds. In local axial gauge its exceptional block \(Q_E(U)\) is a finite-dimensional perturbation of \(Q_E(1)\). If \(\sigma_E>0\) is the latter's least singular value and \(c_E\) bounds the derivative of that fixed block, the explicit condition

\[
 c_E\|U-1\|_{\rm block}\le\sigma_E/4
 \tag{HC.10}
\]

gives \(\|Q_E(U)^{-1}\|\le2/\sigma_E\) and a common complex neighborhood of invertibility. Compact gauge changes act unitarily and do not change this singular-value bound. Finite block size and (HC.7) give (HC.10) uniformly. This is a local inverse estimate, not a bound on an extensive determinant. The coarea factor depending only on \(v\) stays in the outer law.

#### Lemma HC.2 — explicit weighted principal bounds

Let \(0<\gamma\le\delta_K/2\), and define

\[
 A_K=K_0\sup_i\sum_j
 \rho_k(i,j)e^{-\delta_K\rho_k(i,j)/2}<\infty.
 \tag{HC.11}
\]

The right side can be replaced by a fixed lattice sum using (HC.2). For every real 1-Lipschitz function \(f\) on the current lattice and \(D_f=\operatorname{diag}(e^{\gamma f_i})\),

\[
 \|D_fK_\Lambda D_f^{-1}-K_\Lambda\|_{2\to2}
 \le\gamma A_K.
 \tag{HC.12}
\]

Choose

\[
 0<\gamma\le
 \min\{\delta_K/2,\gamma_{ER},\gamma_B,
             \lambda_0/(4A_K)\},
 \tag{HC.13}
\]

omitting the last bound if \(A_K=0\). Then \(K_\Lambda^{-1}\) obeys

\[
 \|(K_\Lambda^{-1})_{ij}\|_{\rm op}
 \le\frac{4}{3\lambda_0}e^{-\gamma\rho_k(i,j)},
 \quad
 \|K_\Lambda^{-1}\|_{\gamma/2}
 \le\frac{4C_d\mathcal N_d(\gamma/2)}{3\lambda_0}.
 \tag{HC.14}
\]

**Proof.** The inequality \(|e^t-1|\le |t|e^{|t|}\) and (HC.9) bound both Schur sums of the difference by \(\gamma A_K\). The block Schur test proves (HC.12). For the inverse bound choose \(f_i=\rho_k(i,j)\), truncated if desired; it is 1-Lipschitz. The real part of the conjugated quadratic form is at least \(3\lambda_0/4\). Its inverse has operator norm at most \(4/(3\lambda_0)\), and the \(ij\) matrix element gives the first estimate. Summation using (HC.2) gives the second. All arguments apply to periodic distance and arbitrary admitted restrictions. \(\square\)

### 5. Complete perturbation accounting

For fixed \(v\), the actual regular inner potential, up to a constant independent of \(z\), is

\[
 V_{k,v}(z)
 =\tfrac12\langle z,K_\Lambda z\rangle
  +\langle z,K_{I,I^c}y\rangle
  -W_{ER}(z;v)-W_B(z;v)-W_{\rm loc}(z;v).
 \tag{HC.15}
\]

This is the C-01 identity, not an approximation. \(W_{\rm loc}\) consists of the bulk nonlinear classical/gauge remainder and the current Haar/constraint density. \(W_B\) includes the inherited B activities, E/R activities assigned to B, the heterogeneous coefficient difference and the complete boundary relocation with its Jacobian. Components are assigned once, according to the source classification. If a C-05 bookkeeping convention already includes a local classical term, omit that term from \(W_{\rm loc}\); the estimates below then only improve.

In particular, the nonconstant coefficient is retained by the identity

\[
 -\Delta A(g_k(\cdot)^{-2},U)
 =-g_k^{-2}\Delta A(1,U)
  -\Delta A(g_k(\cdot)^{-2}-g_k^{-2},U).
 \tag{HC.16}
\]

The last term is bounded by C-05. It is not used to replace the principal form with a fictitious homogeneous full action. The exterior force in (HC.15) is exact and has zero current Hessian; its possibly large effect on the mean remains a C-08 task. Its accompanying Schur complement stays in the outer marginal.

#### 5.1 What is taken from the declared predecessors

C-04 supplies the actual regular E/R bound

\[
 \sup_z\|D_z^2W_{ER}(z;v)\|_\gamma
 \le\varepsilon_{ER}(g_k),
 \qquad \sup_{0<g\le g_*}\varepsilon_{ER}(g)\longrightarrow0
 \quad(g_*\downarrow0).
 \tag{HC.17}
\]

C-05, when completed, must supply the corresponding bound on its actual admitted multiscale domain,

\[
 \sup_z\|D_z^2W_B(z;v)\|_\gamma
 \le\varepsilon_B(g_k),
 \qquad \sup_{0<g\le g_*}\varepsilon_B(g)\longrightarrow0,
 \tag{HC.18}
\]

as well as its local native derivative bounds and quantitative domain reserve. The current boundary proof records precisely such an output in (BV.14)–(BV.18), conditionally on the remaining joined reconstruction and localization checks. **Equation (HC.18) is an input here, not a new proof of those checks.** No coercivity assumption is included in (HC.18); the argument below establishes coercivity from it.

#### 5.2 Bulk classical and measure terms on the actual background class

Take a fixed \(\epsilon>0\), below the absolute preparation radius in CMP116 (1.15)–(1.21), and work first on the larger current disc

\[
 \|z\|_\infty<\epsilon/g_k.
 \tag{HC.19}
\]

This denotes the absolute small-map domain for the full current input (the exterior part will be held fixed as specified below). It is used only for the bulk classical and measure terms. It does not assert that old B activities are admitted on (HC.19). Their domain remains C-05's domain.

The prepared nonlinear constraint obeys \(B'=g_kCz-hD(g_kCz)\); the source bounds its map and all required output norms by a fixed multiple of \(g_k\|z\|_\infty\). The cubic classical remainder is after removal of the *complete* constrained quadratic term in (HC.8). CMP116 (1.37)–(1.40) localizes this remainder; its proof, before Lemma 2, treats the other classical \(P^{(k)}\) terms by the same expansion. Lemma 1 treats the separate old-E contribution. Therefore using the classical part here does not count the E contribution twice.

CMP119 pp.275–277 transfers the classical calculation to the proper-scale cube cover and the full multiscale random walks. Lemma HC.1 admits the background hypotheses for those maps. The bulk terms on the current layer have fixed-parameter carrier bounds of the form

\[
 \sup_{\|z\|_\infty<\epsilon/g_k}|W_{{\rm cl},Y}|
 \le C_{\rm cl}\,g_k^{-2}\epsilon^3
             e^{-\kappa_{\rm cl}d_k(Y)}.
 \tag{HC.20}
\]

The supremum is on the disc in (HC.19). A fixed carrier-volume factor from the plaquette partition has been paid with part of the available decay. Remote proper-scale and boundary-classified terms are in \(W_B\), not in an unproved homogeneous extension of (HC.20). The nonlinearity is cubic or higher after the exact quadratic subtraction, including the quadratic constraint-current contribution; this is essential for the factor \(\epsilon^3\).

For the measure terms, the local Haar logarithm is analytic on the same small-map domain. The nonlinear constraint determinant has the form \(\det(I-T)\), where the local analytic \(T\) has weighted norm \(O(\epsilon)\). Reducing \(\epsilon\) until that norm is at most \(1/2\), the convergent expansion

\[
 \log\det(I-T)=-\sum_{r\ge1}\frac1r\operatorname{Tr}(T^r)
 \tag{HC.21}
\]

is a sum over local loops, not one volume-dependent determinant bound. The local factors and the source localization yield

\[
 \sup_{\|z\|_\infty<\epsilon/g_k}|W_{{\rm meas},Y}|
 \le C_{\rm meas}\epsilon
                  e^{-\kappa_{\rm meas}d_k(Y)}.
 \tag{HC.22}
\]

The exceptional linear-constraint coefficient is controlled by (HC.10); its determinant independent of current coordinates is not inserted into (HC.22). Boundary-change Jacobians remain in C-05. All fixed preparation, block, group and localization constants are retained in \(C_{\rm cl},C_{\rm meas}\).

The actual real support is \(\|z_i\|\le P_k=A_1\ell_k^{p_0}\). There is a separate amplitude check for the retained exterior current \(y\). The classical action is evaluated at the full current field \(t=z+y\), before the inner/exterior split. CMP119 (3.14) bounds the physical current fluctuation on its whole new active domain before that split; after the fixed local coordinate constants this gives

\[
 g_k\|y\|_\infty\le C_{\rm ret}\varepsilon_k.
 \tag{HC.23a}
\]

Old layers outside that current domain remain source retained variables; their boundary-classified contributions are in C-05. Reduce \(g_*\) so that \(C_{\rm ret}\varepsilon_k\le\epsilon/4\), and also so that

\[
 g_kP_k\le\epsilon/4
 \quad\hbox{for every admitted scale.}
 \tag{HC.23}
\]

Let \(c_{\mathfrak g}\ge1\) be the fixed conversion constant from scalar-coordinate sup norm to the chosen Lie-algebra norm. A simultaneous scalar-coordinate polydisc of radius \(\epsilon/(2c_{\mathfrak g}g_k)\) about each such real point, with \(y\) held fixed, keeps the full current field \(t=z+y\) in the absolute map domain (HC.19). The supports of \(z\) and \(y\) are disjoint. Thus this is uniform on the actual admitted exterior-current support, not for arbitrary unbounded exterior amplitudes. Apply the simultaneous Hessian-row estimate BD.2 to (HC.20) and (HC.22), then sum the actual carriers as in DS.3–DS.7. Choose \(\gamma\) smaller if necessary to retain that carrier entropy reserve. This gives

\[
 \sup_z\|D_z^2W_{\rm loc}(z;v)\|_\gamma
 \le C_{\rm cl}'\epsilon
      +C_{\rm meas}'g_k^2/\epsilon.
 \tag{HC.24}
\]

No total number of current coordinates occurs. This proof uses the larger disc only for terms whose actual absolute domains were admitted, and never differentiates a characteristic function. The same Cauchy argument gives each finite local current derivative and joint native derivative with the actual radii retained. For example the order-\(m\) current derivative of one classical carrier is bounded by

\[
 m!\,C_{\rm cl}g_k^{-2}\epsilon^3
       (2c_{\mathfrak g}g_k/\epsilon)^m e^{-\kappa' d_k(Y)}
 \tag{HC.25}
\]

for coordinate derivatives, and by an additional fixed \(e^m\) factor for multilinear unit directions in a norm ball. The resulting factorial exponent is fixed. No source-order-dependent change of \(\epsilon\) is made.

### 6. Common domains and a single parameter choice

The real admission inequalities are supplemented by an actual complex propagator reserve. CMP99 Theorem 3.4 and (3.37)–(3.38) give a positive absolute analytic ceiling \(a_{\rm ana}\) for relative fields in the full layer norm (HC.4). Let \(a_J>0\) be a fixed ceiling for the independent current in the already specified source extension; it can be reduced so that the perturbation estimate for the constraint-current term in CMP99 (3.134)–(3.138) has Neumann norm at most \(1/4\). The original real center has the strict slack in (HC.7). One sufficient quantitative choice is

\[
 r_{\rm prop}=\min\{a_{\rm ana}/4,
                  a_{99}/(16M C_{\rm reg})\},
 \quad r_{\rm prop,J}=a_J/4,
 \quad r_C=\sigma_E/(4c_EC_{\rm block}),
 \tag{HC.26a}
\]

where \(C_{\rm block}\) converts the strong native norm to the actual fixed unit-block chart. These radii are fixed before the final coupling ceiling. The strong complex field norm includes the second-order term; this assertion is not made for a first-derivative-only or arbitrary raw-coordinate direction. The explicit independent-current slot retains its own radius. Later changes to weaker coordinates must carry their actual norm conversion, which belongs to their matching estimate.

Keep the common current contour and native external domains supplied by C-04 and by the declared C-05 conclusion. Intersect them with the absolute local-map domain in (HC.19), the propagator domain from (HC.7), and the exceptional-coordinate neighborhood (HC.10), taking one half of each verified reserve. This is a quantitative construction: in each native direction use

\[
 r_{\rm joint}=\tfrac12\min\{r_{ER},r_B,r_{\rm prop},r_{\rm prop,J},r_C,r_{\rm loc}\},
 \tag{HC.26}
\]

in that direction's own normalization. For the current coordinate the first two radii are fixed multiples of \(P_k\), while (HC.23) supplies a fixed larger absolute-map reserve. In this current direction the propagator and exceptional-coordinate reserves are first pulled back through the actual \(g_k\)-scaled current map: their radii are fixed absolute constants divided by \(g_k\), not the unconverted field-slot constants in (HC.26a). For the layer-weighted background/current slots, \(r_B\) includes all C-05 reconstructed-output restrictions; it is not replaced by an unrestricted raw-coordinate ball. Thus the intersection adds only fixed losses to Cauchy estimates, and no new factor depending on the number of layers. If C-05 does not supply those uniform reserves, its hypothesis here has not been met.

Fix parameters in the following order:

1. The group, an admitted \(L\), source geometry and localization parameters, with the required carrier and collar reserves.
2. The constants \(\lambda_0,K_0,\delta_K\) of (HC.9) and a positive \(\gamma\) satisfying (HC.13) and the local-carrier reserve.
3. One absolute \(\epsilon\) satisfying the local map conditions and \(C_{\rm cl}'\epsilon\le\lambda_0/16\).
4. One coupling ceiling \(g_*\) satisfying (HC.5)–(HC.7), (HC.10), (HC.23)–(HC.23a), the predecessor domain conditions, and

\[
 \sup_{0<g\le g_*}
 [\varepsilon_{ER}(g)+\varepsilon_B(g)
                +C_{\rm meas}'g^2/\epsilon]
 \le3\lambda_0/16.
 \tag{HC.27}
\]

This last choice is available from the predecessor conclusions and the explicit local remainder. It is not asserted to have been verified while C-05 is open. Once it is available, the complete perturbation satisfies

\[
 \eta_\gamma:=
 \sup_{z,v}\|D_z^2(W_{ER}+W_B+W_{\rm loc})\|_\gamma
 \le\lambda_0/4.
 \tag{HC.28}
\]

The source field radii \(\alpha_{i,n}=C_i g_n\ell_n^q\), with the fixed \(q>p_0\) of the contour theorems, can simultaneously be made smaller than all absolute background ceilings by imposing \(\ell_*>2q\) and reducing \(g_*\). The polynomial logarithmic factors do not obstruct any fixed absolute smallness condition. No parameter is adjusted with derivative order, volume or cutoff depth.

### 7. The heterogeneous extension theorem

#### Theorem HC.3 — uniform complete regular coercivity on the admitted heterogeneous class

Retain the J0/C-01 construction hypotheses. Assume the original C-04 and C-05 conclusions, with their actual complete native domains and uniform bounds as specified in Section 5.1. Then the actual inner potential (HC.15), on its actual regular support and for every admitted heterogeneous retained background/history, satisfies

\[
 D_z^2V_{k,v}(z)\ge\tfrac34\lambda_0I.
 \tag{HC.29}
\]

For every real 1-Lipschitz \(f\), its weighted conjugate has

\[
 \operatorname{Re}\langle u,
 D_fD_z^2V_{k,v}(z)D_f^{-1}u\rangle
 \ge\tfrac12\lambda_0\|u\|_2^2.
 \tag{HC.30}
\]

Consequently its pointwise matrix inverse obeys

\[
 \|[(D_z^2V_{k,v}(z))^{-1}]_{ij}\|_{\rm op}
 \le \frac{2}{\lambda_0}e^{-\gamma\rho_k(i,j)},
 \qquad
 \|(D_z^2V_{k,v}(z))^{-1}\|_{\gamma/2}
 \le\frac{2C_d\mathcal N_d(\gamma/2)}{\lambda_0}.
 \tag{HC.31}
\]

The current and native local derivative estimates hold on the explicit common domain (HC.26), with their original running radii and one fixed factorial exponent. All constants are uniform in cutoff depth, expanding volume, and the admitted remaining history. Real linear tilts of this conditional law have the same Hessian estimates.

**Proof.** Equations (HC.8)–(HC.10) identify and admit the actual principal form without setting its background to the identity. The source-normal-form identity (HC.15) includes every current-dependent contribution once. The exterior force and current-independent constants have zero Hessian; they have not been removed from the corresponding probability or outer law.

The symmetric block Schur estimate bounds the perturbation operator norm by \(\eta_0\le\eta_\gamma\). Combining (HC.9) and (HC.28) gives (HC.29). For (HC.30), (HC.12) loses at most \(\lambda_0/4\), and conjugation of the perturbation has both Schur sums at most \(\eta_\gamma\le\lambda_0/4\). The remaining lower bound is \(\lambda_0/2\). The same distance-weight argument as in Lemma HC.2 gives (HC.31). The domain and derivative statements follow from the predecessor bounds, (HC.25), and the half-reserve intersection (HC.26). The proof differentiates analytic coefficient functions within a fixed history/chart, not moving selectors. Adding a real linear function changes neither the Hessian nor the real support. \(\square\)

This is a precision/inverse/coercivity theorem. It is not an identity between the inverse Hessian and the interacting covariance. The latter requires the support and Neumann argument already proved in C-07, and its complete moment/decay application belongs to C-08. The theorem does not bound the conditional mean merely from coercivity. It does not assume the missing C-05 estimate and then claim that estimate has been established.

### 8. Application and remaining application

The new contribution is the actual heterogeneous application: the correct constrained precision and nonlinear constraint-current term; the source eligibility of the regular region; the second-order local background bounds; the current-unit coordinate identification; the bulk local remainder; and the fixed domain/parameter choices. It uses no identity-background extrapolation, no unverified balancing weights, no discarded heterogeneous coefficient, and no extensive determinant estimate.

The heterogeneous coercivity theorem is conditional on the complete regular and boundary derivative estimates for the same conditional representation.

The original C-05 reconstruction and spatial-localization problem remains open, as do H-03 and all later applications not separately established. No four-dimensional Yang–Mills existence theorem is claimed.

### Primary references

- Balaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP 99 (1985), 389–434: (3.35)–(3.38), Section E, (3.155)–(3.158), the lower-bound/locality paragraph on p.428, and Theorem 3.15.
- Balaban, *The Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*, CMP 102 (1985), 277–309: Theorem 1, (2), (9)–(10), and the analytic relative-map construction.
- Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories II*, CMP 116 (1988), 1–22: (1.15)–(1.21), (1.37)–(1.40), and the separate treatment of the classical and old-E terms before Lemma 2.
- Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243–285: p.251; (3.2)–(3.5); (3.15)–(3.25); and pp.275–277.
- Existing estimate proofs: C-01/Annex W; C-07/Annex AA; C-04/Annex AH; C-05's conditional boundary output (BV.14)–(BV.18) in Annex AF, whose actual reconstruction premise is expressly still open.

### Supplement AI.1. Admission of the heterogeneous principal form


#### 1. Scope and decision

The source inputs support a uniform principal-operator theorem on the actual admitted heterogeneous determining geometries and nonconstant backgrounds. This is stronger than extrapolating an identity-background estimate.

A full C-06 theorem may use the **declared predecessor conclusions C-04 and C-05** as hypotheses for the regular E/R and complete boundary perturbation sums. It must keep C-05 visibly open and must prove its own principal-operator and remaining classical/measure estimates. The following checks show that this is a noncircular mathematical step: C-05's required derivative estimates do not assume coercivity of the full conditional action, whereas C-06 obtains that coercivity from the source principal operator and the predecessor bounds.


#### 2. The exact Gaussian operator and free coordinates

See CMP99, p.428. Formula (3.156) is

\[
 \langle B,(QG_1Q^*)^{-1}B\rangle
 -a\langle B,B\rangle
 -2\langle H_1\widetilde D^{(2)}(B),J\rangle
 =\langle B,\Delta_k B\rangle.
 \tag{HA15.1}
\]

The background-current contribution from the quadratic nonlinear constraint is part of \(\Delta_k\). It must not be dropped or reinserted as an unrelated perturbation.

The constraints are the axial conditions and the one-step linear averaging condition \(Q_1B=0\), together with the Dirichlet condition outside the current region \(\Lambda\). The source chooses the actual nonexceptional bond coordinates \(z\) and writes

\[
 B=Cz,\qquad K=C^*\Delta_k C.
 \tag{HA15.2}
\]

The map \(C\) is the identity on nonexceptional bonds. Its other entries solve the local linear averaging equations and depend only on a fixed number of surrounding current unit blocks. In particular, this is not a change to unrelated curl variables.

The exact identity (3.158) identifies the inverse of \(K\) with the restriction of the source covariance to the free bonds. The paragraph immediately after (3.158) states a positive lower bound for \(K\), independent of \(k\) and of the admitted background \(U\), under the full conditions (3.35)–(3.36) and sufficiently small \(M\alpha_0\). It also explicitly retains uniform exponential decay of \(K\). This passage first mentions the identity-field proof and then states the nonconstant-background extension using the local analysis of its Section B. Reading only the identity-field sentence would omit the source's actual scope.

Theorem 3.15, (3.187), p.432, gives exponential decay of the unit-lattice covariance with constants depending on the fixed dimension and block size. Its underlying operators depend on the **entire** determining sequence. They are not operators defined only for a homogeneous history.

#### 3. The current domain has the required collar

CMP99 Section E, starting on p.427, assumes a current unit-lattice domain \(\Lambda\subset A_k=\Omega_k^{(k)}\), consisting of admitted big blocks, with

\[
 \operatorname{dist}(\Lambda,A_k^c)>R_{\rm prop}M_{\rm prop}.
 \tag{HA15.3}
\]

The actual CMP119 construction has this property after a fixed choice of its separation parameters. Equations (3.2)–(3.5), pp.264–265, first surround the old bad region \(Z_k\) by several layers of current-size cubes. The new region \(\Omega_{k+1}\) excludes those layers. The final regular integration region in (3.20), p.269, is a further interior subset of \(\Omega_{k+1}\). Since \(\Omega_k^c\subset Z_k\), this supplies a collar to the old determining-region complement as well.

The smallest constant needed in (HA15.3) is fixed. The construction's running cube radius is bounded below by a freely chosen fixed minimum, so one chooses that minimum to make the construction's collar larger than the right side of (HA15.3), with a fixed reserve for local stencils and block conventions. This is one parameter choice; it does not depend on cutoff depth or on the individual history.

The source's rectangularization does **not** enlarge the regular region across a bad set. On p.251 it explicitly takes small connected components of \(\Lambda_1^c\) and replaces them by enclosing rectangles. Page 269 repeats the same operation on components of \(\Lambda_{k+1}^c\). Thus it enlarges the bad complement and shrinks the regular region. The collar in (HA15.3) cannot deteriorate under this operation. Both pages were in these hypotheses.

The source's periodic block and locality conventions are retained. On an admissible torus the distances are periodic; if the active determining region is the whole torus, the complement condition is void. No rectangular extension of a theorem for arbitrary nonadmitted geometry is assumed.

#### 4. Actual minimizing backgrounds satisfy the full source class

CMP99 (3.35) requires a local gauge with physically normalized potential and first-difference bounds. Its additional (3.36) is a second-order bound. A curvature bound alone is not a justification for the latter.

The correct source input is CMP102 Theorem 1, pp.278–279. Its regular space (2) includes the plaquette and physical-current bounds. Its local gauges satisfy (9), and (10) gives both the \(\partial^{\eta *}\partial^\eta A\) and the component Laplacian bounds. These are exactly the kinds of norms used to admit CMP99's operator construction.

The background in the exact C-01/C-07 current law is the source's constrained Wilson minimum with the actual determining data. The localized coefficient \(g_k(x)^{-2}\) is not silently substituted into the defining variational problem: the exact action split separates its difference from the homogeneous current coefficient as a boundary perturbation. Thus the source minimizing-background theorem applies to the principal operator under discussion.

For clarity, the common smallness choice can be made using one uniform ceiling, rather than trying to prove a new running-weight estimate for every operator entry. Let

\[
 \epsilon_j=A_0g_j(\log g_j^{-2})^{p_0},\qquad g_j\le\bar g,
 \qquad\bar\ell=\log\bar g^{-2}>2p_0.
 \tag{HA15.4}
\]

The function \(g\mapsto g(\log g^{-2})^{p_0}\) is increasing on that interval. Hence

\[
 \epsilon_j\le\epsilon_*:=A_0\bar g\bar\ell^{p_0}.
 \tag{HA15.5}
\]

Include the fixed source comparison and local averaging constants in \(C_{\rm sel}\). The actual selected determining data obey the regular input bound with \(\epsilon_1=C_{\rm sel}\epsilon_*\). The local source gauge constants then give an admissible uniform parameter \(\alpha_*=C_{\rm reg}\epsilon_*\). Choose \(\bar g\) so that

\[
 C_{\rm sel}\epsilon_*\le a_1,
 \qquad
 M_{\rm prop}\alpha_*\le a_{99},
 \qquad
 M_{\rm gauge}\le R_1M_1\frac{a_1}{C_{\rm sel}\epsilon_*}.
 \tag{HA15.6}
\]

The last inequality is the explicit local-gauge cube-size condition \(M\le M(\epsilon_1)\) in CMP102. The fixed \(M_{\rm gauge}\) accommodates the cubes used by CMP99. All these inequalities can be met after fixing the geometry and localization constants, because \(\epsilon_*\to0\). They are uniform in the number of layers.

This verification includes the nonconstant physical current and the second-order local gauge information. It is not an extrapolation from \(U=1\). As elsewhere, it is a source-scoped assertion on actual admitted source histories; an independent verification of J0 and the coupling-trajectory construction remain open.

#### 5. The correct norm is a current-scale norm

The inner conditional integration is over free bonds of one current lattice. Old determining layers, old fluctuation fields and the retained exterior current are parameters. Consequently the natural quadratic Hilbert norm for this theorem is

\[
 \|z\|_{\rm cur}^2=\sum_{b\in I_\Lambda}\|z_b\|_{\mathfrak g}^2.
 \tag{HA15.7}
\]

The coordinate weights on the integrated variables are \(\omega_b=1\). The source's full layer dependence resides in \(K(U,\{\Omega_j\})\), the admitted native external norms, and the nonlinear perturbation. Assigning different physical-layer weights to these current bonds would describe a different coordinate space.

For the raw dimensionless fluctuation \(q_b=g_kz_b\), the same statement has weights \(g_k^{-1}\). For a physical potential with \(q_b=h_kA_b\), the weights are \(h_k/g_k\). These are exact scalar changes of coordinates at the current scale. They do not prove a coercivity theorem on a simultaneous integration over every archived scale.

Native retained directions still use their true layerwise radii. In particular the background Laplace/current restrictions and the boundary reconstructed-data restrictions must not be replaced by a raw unweighted link supremum. Arbitrary selector or history-interface currents remain separate obligations.

#### 6. Remaining classical and measure contributions can be bounded separately

CMP116 Section 1 separates the inherited E fluctuation, treated by Lemma 1, from the first, classical part of the fluctuation action. The exact classical algebra after eliminating the constraints is recorded in Annex AI, Section 1. Its quadratic constraint contribution belongs to (HA15.1); every residual classical term begins at degree at least three.

The localized cubic bound in CMP116 (1.37)–(1.39), together with its stated extension to the other classical terms before Lemma 2, gives an analytic activity norm on a fixed absolute free-current disc of radius \(\epsilon_{\rm abs}/g_k\). Its value budget is proportional to \(g_k^{-2}\epsilon_{\rm abs}^3\), with the source's fixed carrier-polynomial factors and exponential decay. If

\[
 g_kP_k\le\epsilon_{\rm abs}/4,
 \tag{HA15.8}
\]

there is a translated simultaneous disc of radius at least \(\epsilon_{\rm abs}/(2g_k)\) around every point of the actual support. The BD.2 row estimate, followed by the actual carrier count, therefore yields a classical Hessian budget of order \(C_{\rm src}\epsilon_{\rm abs}\).

This argument does not need to reconstruct the unread detailed coefficient display (1.43). It uses the source's complete classical decomposition, the proved representative analytic bound and its explicitly stated extension to the remaining classical terms. It also does not double-count the inherited E fluctuation from Lemma 1.

The Haar and exceptional-constraint density can be treated directly in the actual finite unit-block chart. After dividing out the background-only linear coarea factor, the variable determinant is \(\det(I+A(q))^{-1}\), with \(A(0)=0\), fixed interaction range and absolute row/column norm at most \(C\epsilon_{\rm abs}\). Uniform invertibility of the exceptional linear coefficient follows from its nonzero finite-block coefficient at the identity and a fixed small-neighborhood estimate, using the admitted local gauge. The logarithmic determinant is its convergent trace-loop series. The anchored loop norm is \(O(\epsilon_{\rm abs})\), hence Cauchy gives a current Hessian budget \(O(g_k^2/\epsilon_{\rm abs})\). The Haar logarithms obey the same conservative bound.

The principal gap is fixed before choosing \(\epsilon_{\rm abs}\); take that absolute radius sufficiently small and then take \(\bar g\) sufficiently small for (HA15.8) and the measure budget. This is compatible with the source's absolute minimizing-map domain and a wider fixed native regularity class. The classical sector has no old-activity dyadic-domain requirement of its own. Boundary-classified outputs, heterogeneous coefficient differences and relocation are assigned to C-05 once, as required by the exact density ledger.

#### 7. Scope of the predecessor-conditional conclusion

With the actual principal estimates above, a proof of C-06 can combine:

- C-04's already established regular E/R weighted derivative budget;
- C-05's full boundary derivative conclusion, **retained as an unproved predecessor**;
- the classical and measure estimates in Section 6;
- the actual precision/covariance bounds in Sections 2–4.

The retained cross term has the form \(\langle z,K_{IO}y\rangle\). It changes the conditional mean but has zero current Hessian, so it does not alter coercivity. It must not be declared small or removed from subsequent moment bounds. The shifted Gaussian normalization stays in the outer marginal.

This is a genuine actual-model uniform step conditional on its stated predecessor: its new content is the checked applicability of the source principal operator and complete remaining perturbation estimates on the actual heterogeneous class. It is not an unconditional full-potential theorem before C-05 is supplied, a statement about convexity of the complete positive history space, or a mean/decay theorem for marked observables.

#### Sources

- CMP99, pp.396–399 and 427–432: source class, uniformity in the determining sequence, exact constrained quadratic form, free-coordinate covariance, nonconstant-background gap and exponential bounds.
- CMP102, pp.278–279, (2), Theorem 1 and (9)–(10): actual minimizing-field regularity including second-order local gauges.
- CMP119, pp.251, 264–270: current geometry, actual support, complement rectangularization, relocation and Gaussian split.
- CMP116, Section 1, (1.19)–(1.21), (1.33)–(1.43): primary equations. Annex B gives the classical and measure bounds within their stated scope.

### Supplement AI.2. Covariance, perturbations and domain margins


#### Decision and exact scope

The C-06 implication assumes the regular and boundary derivative estimates of C-04 and C-05. Uniformity on all required Wilson histories remains conditional.


The complete perturbation budget includes the boundary action B.

#### Checks performed

##### 1. Actual variables and principal form

The integrated variables are the current-unit free bonds in the regular inner expression of CMP119 (3.23)–(3.25). Archived layers and the exterior current are fixed parameters. Consequently the Hilbert norm in (HC.1) and the current-lattice weighted matrix norm in (HC.3) are the correct norms for this conditional Hessian. Arbitrary weighted products over all historical layers would describe a different integration space.

The exact precision includes the background-current quadratic constraint contribution in CMP99 (3.156). The source on p.428 explicitly identifies the free precision, its covariance inverse, its nonconstant-background lower bound under (3.35)–(3.36), and its exponential locality. This is an actual heterogeneous source result, not an extrapolation of its preceding identity-background example.

The argument fixes the full current map \(C\) before conditioning and then takes the principal matrix restriction. This matters for free bonds whose images include neighboring exceptional bonds; re-solving a different constraint problem inside the inner region would not give the same conditional precision. The stated order preserves both the lower bound and the entrywise decay.

##### 2. Source geometry and background admission

CMP99 Section E requires an admitted current domain with a fixed collar to the previous active-region complement. CMP119 (3.2)–(3.5) removes layers around the old bad set, and its final inner region is smaller. The source rectangularization enlarges small components of the bad complement. Thus it cannot destroy that collar. The inequality (HC.5) is a fixed parameter choice, with source-admitted geometries retained.

CMP119 p.256 defines the determining field by its layer values and requires regularity on the determining set before invoking the constrained minimum. CMP102 Theorem 1 supplies the first- and second-order local-gauge bounds needed by CMP99; a plaquette bound is not substituted for the second-order condition. The common ceiling in (HC.6)–(HC.7) is legitimate because \(g(\log g^{-2})^{p_0}\) is increasing for \(\log g^{-2}>2p_0\) and tends to zero at the origin. These checks retain the admitted source-free construction and trajectory as inputs.

##### 3. Weighted matrix proof

For a 1-Lipschitz distance weight, the entrywise conjugation error has both Schur sums bounded by \(\gamma A_K\). The block Schur test therefore proves (HC.12), with no translation-invariance assumption. For \(\gamma A_K\le\lambda_0/4\), the conjugated principal matrix has real part at least \(3\lambda_0/4\). Applying its inverse to a vector supported at one bond gives the entrywise exponential bound; the current lattice count gives the row and column sum at half the exponent.

The same argument for the full Hessian uses the weighted perturbation norm and loses another \(\lambda_0/4\), leaving \(\lambda_0/2\). The resulting inverse matrix estimate in (HC.31) is correct. It is not identified with the interacting covariance. The theorem neither assumes nor proves a bound for the conditional mean.

The counting estimate is uniform on an admitted torus by choosing shortest periodic representatives. A principal restriction only decreases the relevant sums.

##### 4. Exhaustive action accounting

The conditional potential retains the exact exterior cross force. This term has zero current Hessian but can affect the mean, so its omission from a coercivity budget does not justify its omission from future moment estimates.

The homogeneous current coefficient supplies the principal quadratic form. The heterogeneous coefficient difference is an exact residual term assigned to C-05. It has not been set to zero. The old E/R activities, inherited B activities, boundary relocation and its Jacobians, bulk classical remainder, and current Haar/constraint density are assigned once.

C-05 is assumed only through its original required complete derivative and domain conclusions. No coercivity assumption is included in this premise. In particular the new theorem does not assume its own principal-plus-perturbation conclusion.

##### 5. Classical and measure bounds on the real support

The exact constrained quadratic term must be removed before using cubic vanishing. The algebra retained from CMP109/CMP116 does this, including the quadratic nonlinear-constraint current. The proof of the localized classical bound in CMP116 explicitly extends its treatment to the remaining classical terms. CMP119 pp.275–277 uses the actual proper-scale cube cover and full determining-sequence propagators: interior terms retain the stated regular bounds, and remote or boundary-classified terms are assigned to B.

The absolute current disc is used for the local classical and measure sector only. It is not silently imposed on the narrower old-B domain. The retained exterior current satisfies the smallness bound from CMP119 (3.14), on the whole new active domain before the split, so the full current field remains inside the local map disc when the inner coordinates move in the displayed simultaneous polydisc.

The local Haar logarithms and finite-range nonlinear constraint determinant have convergent analytic logarithms on that disc. The determinant is expanded as anchored loops with a uniform row/column norm; no extensive determinant ratio is used. With the local value estimates, simultaneous Cauchy and the admitted carrier count yield

\[
 \|D^2W_{\rm loc}\|_\gamma
 \le C_{\rm cl}'\epsilon+C_{\rm meas}'g_k^2/\epsilon.
\]

The order of choices, first \(\epsilon\) and then the coupling ceiling, makes both terms small and does not depend on volume or derivative order.

##### 6. Native domains and absence of a circular premise

The complex propagator domain includes the actual second-order background norm and independent-current radius. Neither a first-derivative norm nor an arbitrary retained-coordinate direction is substituted. The actual current-coordinate reserve is pulled back through its \(g_k\)-scaled map; one does not incorrectly intersect an \(O(P_k)\) current disc with an unconverted \(O(1)\) physical-field radius.

The half-reserve intersection in (HC.26) uses C-05's complete reconstructed-output restrictions. If those uniform reserves are not proved, the hypothesis is not available. This retains the precise open reconstruction issue.

The derivation uses the C-01 source normal form directly. C-07 is a downstream support/IBP result and is not a premise. Thus its catalogue dependency on C-06 causes no cycle.

#### Remaining limits

The stated theorem does not establish:

- C-05's actual joined reconstruction, current response, carrier localization or complete boundary budget;
- selector and retained-history currents outside a fixed admitted native chart;
- current-scale conditional means or interacting cumulant decay;
- a full-law history estimate, the local renormalized Schwinger hierarchy, rotation restoration, operator bounds, or phase transfer.


#### Sources

- CMP99: source class (3.35)–(3.38) and Section E, especially p.428 and (3.155)–(3.158).
- CMP102, Theorem 1, pp. 278–279, (2), (9)–(10).
- CMP119, pp. 251, 256–257, 261, 269 and 275–277, (3.10)–(3.14).
- CMP116 and CMP109 supply the sector decomposition, local map bounds and classical and measure estimates on their stated domains.

No new theorem of the source-free construction, coupling flow or four-dimensional existence is imported through these references.
