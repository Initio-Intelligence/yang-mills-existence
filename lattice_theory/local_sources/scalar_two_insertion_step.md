# Two scalar insertions at a single integration step

## 1. Scope and hypotheses

**Status:** proved one-step scalar estimates and a summable Gaussian vacuum contact subtraction; the complete interacting two-insertion induction remains open. This paper records the calculation and its exact remaining hypotheses.

This paper starts the following calculation: carry two scalar plaquette insertions through the existing source-free small-field integration and localized large-field R-operation, with the maps and selectors frozen at zero source. The target is an actual marked induction estimate, not another assertion that real source stability implies correlation bounds.

The underlying action is the Wilson action. Balaban's normalized-trace convention is kept distinct: if \(s_p=N-\operatorname{Re}\operatorname{Tr}U_p\), his plaquette action is \(a_p=s_p/N\). Thus the coefficient multiplying his action at the initial step is \(X_{B,0}=N\beta_a=2N^2x_0\). Scalar marks in the Wilson normalization are \(\sum_p f_p s_p=N\sum_p f_p a_p\). Source-independent constants cancel in normalized expectations; mark coefficients and covariance factors do not disappear under that cancellation.

The primary inputs are the CMP 109 effective-action paper (Bałaban, CMP 109 (1987), 249–301), CMP 116 cluster-expansion paper (Bałaban, CMP 116 (1988), 1–22), CMP 119 inductive-representation paper, CMP 99 background-propagator paper, CMP 102 constrained-variational paper, and LFR I and II. Formulas cited as literature inputs are checked against the printed papers. No N0 dictionary or sourced extension is silently assumed. N2-F remains the numerical flow interface allowed by the original program, subject to the normalization dictionary; the single-step algebra below does not require a stronger flow theorem.

The labels are: **(P)** a result proved here; **(L)** a checked primary-source statement in its stated scope; **(C)** a conditional application with displayed premises; and **(O)** an estimate still requiring proof. A conditional marked estimate is not called a completed Yang–Mills step.

Three distinctions govern the calculation.

- A frozen positive integration transports a marked numerator exactly, but does not by itself bound its ultraviolet behavior.
- A conditional expectation on a rare history can be large. The quantity entering the complete density is its product with that history's weight. Bounds below retain this product and do not invent a lower bound on the rare history mass.
- The first bare marks are explicit functions of plaquettes. Once small-field integrations generate local, multilocal, and contact vertices, their bounds must be proved separately. A bound on the bare plaquette function is not automatically a bound on all its transported derivatives.

The calculation is organized around three concrete mechanisms: density-weighted cumulant estimates without rare denominators; a local source-difference identity at the original constrained Wilson minimum; and marked small-field/cluster estimates in the actual covariance and interaction norms. The later sections record which of these mechanisms has been established and which applications remain conditional.

## 2. Fixed maps, positive histories, and the quantities to estimate

### 2.1 The localized reference denominator is held fixed

At one real, positive history and fixed retained data \(v\), write the incoming local integral and the source-free reference normalizer as

\[
I(v)=\int f_0(u,v)\,d\nu_v(u),\qquad
H(v)=\int h_0(u',v)\,d\nu'_v(u')>0.
\tag{2.1; P: notation}
\]

The frozen R replacement is \(h_0(u',v)I(v)/H(v)\). All old history factors, cutoffs, Haar Jacobians, constraints, E/R/B factors, and previous integrations belong in \(f_0\,d\nu_v\). They are not silently removed from the conditional measure. Introduce the finite positive measure

\[
d\sigma_v(u)=H(v)^{-1}f_0(u,v)\,d\nu_v(u),\qquad
t(v)=\sigma_v(1),\qquad
\mu_v=t(v)^{-1}\sigma_v
\quad\text{when }t(v)>0.
\tag{2.2; P: definitions}
\]

The measure \(\sigma_v\) retains the reference denominator but does not divide by the potentially rare numerator \(I(v)\). Null histories contribute zero and require no conditional probability measure.

For an affine source with local marks \(A_f,A_g\), the first two raw numerator coefficients and the logarithmic mixed coefficient are

\[
D_f t=\sigma(A_f),\qquad
D_fD_g t=\sigma(A_fA_g),\qquad
D_fD_g\log t=\operatorname{Cov}_{\mu}(A_f,A_g).
\tag{2.3; P}
\]

The last expression is used only where \(t>0\). In the full density, the corresponding covariance is weighted by \(t\), so the useful object is \(t\,\operatorname{Cov}_{\mu}(A_f,A_g)\). Bounding the bare conditional covariance while losing \(t\) can discard the large-field suppression.

### 2.2 Nonlinear incoming jets are retained

If the incoming log source has a second-order vertex \(A_{fg}\), its transformed coefficient is

\[
A_f'=Q A_f,\qquad
A_{fg}'=Q A_{fg}+\operatorname{Cov}_Q(A_f,A_g).
\tag{2.4; P}
\]

This follows by differentiating the finite-dimensional integral, or by formal Taylor algebra through degree two. The term \(QA_{fg}\) is present after earlier integrations even when the original source was affine. The raw second derivative instead transports \(A_{fg}+A_fA_g\). Both conventions will be tracked explicitly.

A mark supported outside the integrated variables is a function of \(v\) alone and factors out of the integral. Such deterministic terms pass through; they are not vacuum counterterms unless they are also independent of retained fields. Conditional cumulants of order at least two are unchanged by subtracting a deterministic term from any argument.

### 2.3 Energy and history budgets

For the estimates below, \(T(u)\ge0\) denotes a specified coercive local energy and \(\mathcal Q\ge0\) a specified history-size budget. They are different objects. The positive number \(\kappa\) is an energy exponent. A useful pair of bounds is

\[
\sigma(1)\le C_0e^{-a\mathcal Q},
\qquad
\sigma(e^{\kappa T})\le C_1e^{b\mathcal Q},
\qquad a>0,\ b\ge0.
\tag{2.5; C: two estimates to be checked on the actual history}
\]

The first is the unmarked large-field estimate. The second estimates an integral after restoring a fraction of the damping energy. Neither is a lower bound on \(\sigma(1)\).

A second route uses a deterministic mark budget rather than energy. Suppose the actual marks satisfy

\[
|A_i(u)|\le c_i\mathcal Q
\quad\text{on the history support},
\qquad
\sigma(1)\le C_0e^{-a\mathcal Q}.
\tag{2.6; C: direct history-budget hypothesis}
\]

This is particularly relevant for still-unintegrated compact plaquette functions. It must be checked with the correct history carrier and scale counting. It does not apply automatically to generated source vertices.

### 2.4 Constrained Gaussian notation

Let \(z=0\) represent the original constrained Wilson minimum in a fixed local coordinate chart. Let \(a_p(z)\) be the plaquette contributions whose sum is the constrained Wilson action \(\mathcal A(z)\). Every plaquette depending on the integrated variables is included; boundary-crossing plaquettes are not omitted. Set

\[
v_p=D a_p(0),\qquad H_p=D^2a_p(0),\qquad
H_{\mathcal A}=\sum_pH_p,\qquad
\sum_pv_p=0.
\tag{2.7; P: definitions and stationarity hypothesis}
\]

The tangent space has its gauge null directions removed. If the Gaussian quadratic form is \(XH_{\mathcal A}>0\), its covariance is \(C=(XH_{\mathcal A})^{-1}\). A general actual covariance will be denoted \(C_{\mathrm{act}}\), and any mismatch from this identity is recorded rather than suppressed.

For a scalar weight \(f_p\), the degree-two Taylor mark is

\[
A_f^{[2]}(z)=c_f+b_f^Tz+\tfrac12z^TV_fz,\qquad
c_f=\sum_pf_pa_p(0),\quad
b_f=\sum_pf_pv_p,\quad
V_f=\sum_pf_pH_p.
\tag{2.8; P}
\]

The nonlinear Wilson action need not be replaced by a globally quadratic curvature model for these identities. Only its Taylor coefficients at the original constrained minimum are used. In physical source-kernel estimates, \(d_T(p,q)\) means the torus distance between the assigned source positions \(x_p,x_q\). The usual plaquette-support or block distances in the propagator imports differ by bounded fine or shell distances, which alter only the fixed constants in the exponential estimates. Source Lipschitz and Taylor estimates always use the distance of their evaluation points.

## 3. Main results and the remaining full-step target

### 3.1 Moments and cumulants with the rare history weight retained

**Theorem 3.1 (P).** Under the two numerical hypotheses (2.5), set
\(\theta=a\kappa/[2(a+b)]\) and
\(C_*=C_0^{1-\theta/\kappa}C_1^{\theta/\kappa}\). Then

\[
\sigma(T^m)\le C_*\,m!\theta^{-m}e^{-a\mathcal Q/2},
\qquad m\ge0.
\tag{3.1; P}
\]

If \(|A_i-c_i(v)|\le a_iT\), the conditional cumulants of order \(m\ge2\) satisfy

\[
t\,|\kappa_\mu(A_1,\ldots,A_m)|
\le C_*\,2^{m-1}(m!)^2\theta^{-m}
 e^{-a\mathcal Q/2}\prod_i a_i.
\tag{3.2; P}
\]

No lower bound on \(t\) is assumed. For two arbitrary square-integrable marks,

\[
t\,|\operatorname{Cov}_\mu(F,G)|
\le2\sqrt{\sigma(|F-c|^2)\sigma(|G-d|^2)}.
\tag{3.3; P}
\]

The proof is in §4.1. This gives factorial-compatible estimates even when the old history mass is arbitrarily small. For a full incoming second jet, \(\sigma(A_{fg})\) must be added to the bound for the covariance term.

### 3.2 A weighted version of the actual large-field history estimate

Let \(\mathcal V(\omega)\) be the positive geometric cost appearing in the proof of LFR II (1.79), written without its adjustable fixed coefficient:

\[
\mathcal V(\omega)
=\sum_j M^dR_j^{d+1}
 \sum_{Z\in\mathcal Z_j(\omega)}d'_j(Z).
\tag{3.4; L/P: history cost from LFR II pp.380–383}
\]

All sets, scale volumes, and linear-size functions have the meanings used in that proof; arbitrary microscopic regions are not substituted for them.

**Theorem 3.2 (P: extension of the checked numerical estimate).** Fix \(s>0\). For the real positive operation \(T'_k(X)\) of LFR II (1.71), on its admitted geometry and regular retained configurations, the proof of (1.79)–(1.89) also bounds the operation with the history multiplier \(e^{s\mathcal V}\). After a sufficiently small fixed choice of the admitted coupling ceiling, depending on \(s\) and the original construction constants,

\[
\sigma_{X,v}(e^{s\mathcal V})
\le \varepsilon_k,\qquad
\varepsilon_k
=\exp\!\left[-2(1+\beta_0)^{-1}p_0(g_{B,k})\right].
\tag{3.5; P}
\]

Here \(\sigma_{X,v}\) is the post-cancellation positive kernel whose mass is \(T'_k(X)1\). Identifying it with a pre-localization quotient such as (2.2) requires assigning all retained-field and new-action factors first. No automatic identification of those two kernels is used. The symbol \(\beta_0\) is Balaban's history parameter, not the one-loop flow coefficient. Consequently,

\[
\sigma_{X,v}(\mathcal V^m)
\le m!s^{-m}\varepsilon_k.
\tag{3.6; P}
\]

The fixed geometric cost in (1.79) is replaced by that cost plus \(s\mathcal V\). The same shrinking, birth, and merger inequalities then apply with larger fixed constants. The proof and its small-coupling requirements are detailed in §4.2. This is a theorem about the actual positive history measure, not a hypothetical old-component lower bound.

For marks satisfying \(|A_i-c_i(v)|\le a_i\mathcal V\), it follows that

\[
t\,|\kappa_\mu(A_1,\ldots,A_m)|
\le 2^{m-1}(m!)^2s^{-m}\varepsilon_k\prod_i a_i,\qquad m\ge2.
\tag{3.7; P}
\]

Still-unintegrated bare plaquette sums on the history domains counted by (3.4) satisfy a bound of this kind, with the fixed plaquette multiplicities included. Complete transported vertices require an additional estimate; Theorem 3.2 does not assert it.

### 3.3 The constant scalar Gaussian sector on the actual gauge-fixed tangent space

**Theorem 3.3 (P).** At the constrained Wilson critical orbit, let \(K\) be the Wilson Hessian on the tangent space of the coarse constraint, let \(\mathcal N\) be its infinitesimal gauge directions fixing the coarse block basepoints, and let \(D\) be the linearized axial gauge map of CMP 109 (2.5). Then the actual untruncated quadratic precision is \(K+D^*D\). Its Wilson part satisfies

\[
P=(K+D^*D)^{-1}K,\qquad
P^2=P,\qquad
\operatorname{Tr}P^m=r:=\dim E-\dim\mathcal N
\quad(m\ge1).
\tag{3.8; P}
\]

The rank is fixed on the family of admitted constrained minimizing backgrounds for a fixed integration geometry; it can depend on that geometry and on the scale. Couple a constant scalar source to the quadratic Taylor part of the physical plaquette sum \(S=N\mathcal A\). Its untruncated Gaussian logarithm has the form

\[
tN\mathcal A(U_0)
-\frac r2\log\!\left(1-Ng_B^2t\right).
\tag{3.9; P}
\]

Its source derivatives of order at least two are therefore background-independent vacuum terms. This assertion is about the quadratic Taylor mark, not the full nonlinear Wilson function integrated under a Gaussian measure. The factor \(r\) counts the physical tangent directions, not all soft-gauge Gaussian variables. The proof uses the gauge covariance displayed on CMP 109 p.265 and the explicit axial coordinates on p.266; see §4.3.

Equation (3.9) does not include the small-field cutoff or the interacting potential. Their contributions are treated separately. Replacing \(P\) by the identity on the entire soft-gauge space would give an incorrect vacuum coefficient.

### 3.4 An exact local source-difference identity

**Theorem 3.4 (P).** With the first variations \(v_p\) in (2.7) and any symmetric positive covariance \(C\), define \(K_{\mathrm{lin}}(p,q)=v_p^TCv_q\). Then

\[
\sum_qK_{\mathrm{lin}}(p,q)=0,\qquad
b_f^TCb_g
=-\frac12\sum_{p,q}K_{\mathrm{lin}}(p,q)
 (f_p-f_q)(g_p-g_q).
\tag{3.10; P}
\]

This uses exact constrained Wilson stationarity and does not require the action to be globally quadratic. If some plaquettes are omitted, write
\(r_p=\sum_qK_{\mathrm{lin}}(p,q)\); the exact formula then has the extra term \(\sum_pr_pf_pg_p\). Boundary forces are not silently discarded.

Using the checked current-shell covariance and lift estimates, the principal curvature part has physical kernel bound

\[
|\mathcal R_h(p,q)|
\le C X^{-1}h^{-4}e^{-c d_T(p,q)/h},
\qquad
\sup_p\sum_q a^4
 \left(1+\frac{d_T(p,q)}h\right)^5
 \frac12\left|\operatorname{Tr}
 [\mathcal R_h(p,q)\mathcal R_h(q,p)]\right|
\le C X^{-2}h^{-4}.
\tag{3.11; P in the admitted current regular core}
\]

Here \(X\) is the literal normalized-trace quadratic coefficient, and the fine measure is \(a^4\). This estimate uses the hard constrained covariance of CMP 99 §E, as defined precisely in §4.4. It is not an identification of every weighted quadratic vertex in that chart with the soft-gauge chart in Theorem 3.3. The lift is the current-shell lift, not a substitute for all previously integrated fine fields. Proof and boundary qualifications are in §4.4.

### 3.5 The interacting regular-bulk response and its application boundary

A marked extension of the actual CMP 116 cluster estimate is proved in §4.5. Its precise input is an analytic, anchored, quadratically dominated local vertex norm, uniform also under the paper's complex decoupling deformations. For two admitted vertices with norm bounds \(a_f,a_g\), its mixed activity satisfies

\[
|K_{fg}(X)|\le C a_fa_g e^{-\kappa_*d(X)},
\tag{3.12; C: under the marked-vertex norm of §4.5}
\]

and vanishes for carriers missing either source anchor. Its mixed Taylor remainder is bounded by
\(C|st|a_fa_g(|s|a_f+|t|a_g)e^{-\kappa_*d(X)}\).

For newly inserted bare scalar plaquette marks in the admitted regular bulk, the holomorphic plaquette identity and the checked lifted-field estimates give

\[
a_f\le C\|f\|_\infty
 \bigl(g_B\epsilon_{\mathrm{bg}}+g_B^2\bigr).
\tag{3.13; P: regular-bulk admission}
\]

The constant background value is extracted before this estimate. The source-free cutoff, Jacobian, Haar terms, nonlinear constraints, and previous source-free effective interaction remain in the integral. On a shrinking regular background domain with
\(\epsilon_{\mathrm{bg}}\lesssim g_Bp(g_B)\), this yields a two-mark bound of order \(g_B^4p(g_B)^2\). On the larger fixed complex background domain, (3.13), rather than that sharper power, is the justified estimate.

**Full-step status (O).** These results do not yet prove the complete marked induction. The complete incoming first and second jets must simultaneously satisfy the analytic carrier norm in the regular regions and an admissible energy/history bound on every old large-field integration region. Their contact and marginal projections must then close one scale-dependent norm. Section 7 states this remaining problem as explicit estimates, rather than identifying it with the already proved bare-mark results.

## 4. Proofs and the actual one-step estimates

### 4.1 Density-weighted moments and cumulants

Hölder's inequality for the finite positive measure gives

\[
\sigma(e^{\theta T})
\le \sigma(1)^{1-\theta/\kappa}
 \sigma(e^{\kappa T})^{\theta/\kappa}
\le C_*e^{-a\mathcal Q/2}.
\tag{4.1; P}
\]

The exponential series gives \(T^m\le m!\theta^{-m}e^{\theta T}\), proving (3.1). No probability normalization or lower mass estimate is used.

For (3.3), subtract \(c,d\), expand
\(t\operatorname{Cov}_\mu(F,G)=\sigma(FG)-\sigma(F)\sigma(G)/t\), and apply Cauchy–Schwarz to both terms. For any partition \(\pi\) of \(m\) arguments, Lyapunov's inequality gives

\[
t\prod_{B\in\pi}\mu(T^{|B|})
\le t\prod_{B\in\pi}\mu(T^m)^{|B|/m}
=\sigma(T^m).
\tag{4.2; P}
\]

The sum of absolute cumulant coefficients is at most
\(\sum_\pi(|\pi|-1)!\le m!2^{m-1}\). Order the blocks, encode an ordered partition by a permutation and cuts, and discard the factor dividing by its number of blocks. This proves (3.2). Constants may first be subtracted from the cumulant arguments.

### 4.2 A reserve in history volume, with all reference cancellations intact

LFR II p.380 bounds the non-Wilson and nonquadratic terms by fixed multiples of \(M^dR_j^{d+1}d'_j(Z_j)\). The sums leading to (1.79), p.383, have positive cost \(C\mathcal V\), alongside negative seed and preparatory costs. On each fixed history, \(e^{s\mathcal V}\) is constant in all integration variables. It replaces this cost by \((C+s)\mathcal V\) without changing any reference denominator or Wilson cancellation.

Equation (1.81), p.385, bounds the entire future cost of one component by a fixed multiple of \(M^dL^{d+1}R_j^{d+2}(d'_j(Z)+1)\). Equation (1.82) supplies a seed cost proportional to \(A_1^2p_0(g_j)^2(d'_j(Z)+1)\). Equations (1.83)–(1.88) treat propagation, preparatory births, and mergers, retaining the final term \(2(1+\beta_0)^{-1}p_0(g_{j+1})\). Choose the logarithmic exponents with the strict margins used there: the \(p_0\) power dominates \(R_j^{d+2}\), and p.383 requires \(2p_1-(d+5)r_0>p_0\). Every fixed increase of \(C\) is then paid by one smaller coupling ceiling. Repeating those numerical inequalities with \(C+s\) proves (3.5). The exponential series proves (3.6).

For still-explicit old-history plaquettes of bounded multiplicity, supported in a fixed one-step enlargement of the actually counted history domains, compactness and the same scale-volume count give

\[
\#\mathcal P(\omega)\le C\sum_j|Z_j(\omega)|_j
\le C'\mathcal V(\omega),\qquad
|F_f|\le 2NC'\|f\|_\infty\mathcal V.
\tag{4.3; P}
\]

A one-bond enlargement or one-step scale change costs a fixed factor. Counting all microscopic plaquettes in an arbitrary current coarse box would not be this estimate. Hence

\[
|\sigma(F_f)|\le a_fs^{-1}\varepsilon_k,\quad
|\sigma(F_fF_g)|\le2a_fa_gs^{-2}\varepsilon_k,\quad
t|\operatorname{Cov}_\mu(F_f,F_g)|
\le4a_fa_gs^{-2}\varepsilon_k.
\tag{4.4; P}
\]

These are actual marked estimates on the old positive operation.

A stronger energy-stripping argument is **not claimed as proved**. The operation contains older T-operations and reference denominators. LFR II (1.10), p.358, puts \(\exp[xA(\zeta_0,U_0)]\) in a reciprocal reference normalizer; (1.30)–(1.32), p.364, cancel the corresponding potentially large background action. If \(xA(u)=C(v)+E(u,v)\), weakening a nested numerator with its denominator fixed gives

\[
\frac{\int e^{-(1-\kappa)xA(u)}\,d\nu}
 {\int e^{-xA(u)}\,d\nu}
=e^{\kappa C(v)}
 \frac{\int e^{-(1-\kappa)E(u,v)}\,d\nu}
 {\int e^{-E(u,v)}\,d\nu}.
\tag{4.5; P}
\]

A determinant-entropy estimate controls only the second factor. The first has not been bounded by the history cost. Top-level positivity after cancellation does not resolve this recursive mismatch. The history-volume multiplier avoids it exactly.

The alternative representation in LFR II (1.103)–(1.104), pp.391–392, keeps old unresolved R components as positive multiplication factors rather than reopened integrations. It may support a stronger reserve after a separate recursive verification; it is not needed for (4.4).

**Smaller ceiling from N2-F (P).** Put \(b=b_0\log L\), \(B=C_r\gamma^2\), and \(X_c=\max(\gamma^{-2},2C_r/b)\). Choose
\(X_1>\max(\gamma_1^{-2},X_c+B,4\gamma^{-2})\).
For \(x\ge X_c\), the flow decreases \(x\) by at least \(b/2\); for \(x<X_c\), its next value is below \(X_c+B<X_1\). Thus \(\{x<X_1\}\) is forward invariant. Choosing \(g_*^{-2}\ge X_1\) forces every earlier \(x_j\ge X_1\), hence all couplings below the smaller ceiling \(\gamma_1\). This uses a consistently normalized N2-F and a choice of one sufficiently small terminal coupling, not a new monotonicity assumption.

### 4.3 Gauge directions and the constant-source Gaussian determinant

CMP 109 (2.1)–(2.5), pp.265–266, fixes coarse averages and introduces axial coordinates for every non-basepoint vertex in a block. Gauge transformations equal to the identity at block basepoints preserve the coarse constraint. Path covariance gives, up to the sign convention,

\[
D(\lambda)(y,x)
=-\operatorname{Ad}_{V^{(k)}(y,x)}\lambda(x),
\qquad \lambda(y)=0.
\tag{4.6; P}
\]

Here \(V^{(k)}(y,x)\) denotes the **averaged contour variable** in CMP 109 (0.11), p.253. The endpoint transformation in (4.6) is exact even with symmetric path averaging: property (0.6) makes the average bi-equivariant, and (0.9) keeps a real average in the compact group. It is not an average of unequal adjoint operators. Thus \(D|_{\mathcal N}\) is an isomorphism, orthogonal in endpoint gauge-parameter coordinates on real backgrounds. Its analytic extension is boundedly invertible on a smaller complex neighborhood. Differentiating gauge invariance at the constrained critical orbit gives \(K\mathcal N=0\). The actual precision \(H=K+D^*D\) includes the nonlinear constraint correction in CMP 109 (1.5), (2.11).

The splitting \(E=\mathcal N\oplus\ker D\) diagonalizes the two bilinear forms into their gauge and physical blocks. Consequently

\[
H^{-1}K(n+s)=s,\qquad n\in\mathcal N,\ s\in\ker D.
\tag{4.7; P}
\]

This proves (3.8). The free-coordinate inclusion solving the average constraint is a coordinate change on \(E\), so rank and traces are unchanged. A constant physical scalar mark has no linear term and has quadratic vertex \(Ng_B^2K\). Therefore
\(\det(I-tNg_B^2H^{-1}K)=(1-tNg_B^2)^r\), proving (3.9).

This identity concerns the actual minimizing-background family and its analytic continuation. Arbitrary independent auxiliary \((U,J)\) pairs need not be stationary. On the larger auxiliary domain use the stationarity-reduced extension from (2.11), and return to the physical family before asserting the determinant identity.

The identity cancels the **sum** of field-dependent Gaussian terms for a constant source. It does not make each canonical localized Gaussian activity vanish. One may instead localize the interacting-minus-Gaussian difference and assign the remaining global Gaussian scalar to the vacuum term. Variable sources still require the complete marked kernel.

### 4.4 Complete Gaussian vertices and source differences

In this subsection, \(C^{(k)}\) is the **hard constrained** unit covariance of CMP 99 §E, (3.156)–(3.158), p.428. If \(E_{\mathrm h}\) is its free-coordinate inclusion, define \(C_X=X^{-1}(E_{\mathrm h}^*\Delta_kE_{\mathrm h})^{-1}\) in those coordinates, so the embedded covariance is \(X^{-1}C^{(k)}\). This fixes the meaning of \(C_X\), independently of the special notation in §2.4. The unit quadratic form has a uniform gap; Theorem 3.15, (3.187), p.432, gives exponential decay. The lift and its first fine derivative satisfy (3.133), Theorem 3.12, pp.422–423. In the current terminal regular core \(L^k\eta=1\), and hence

\[
|D_\eta H_1(p,y)|\le Ce^{-cd(p,y)},\qquad
|X^{-1}D_\eta H_1C^{(k)}H_1^*D_\eta^*(p,q)|
\le CX^{-1}e^{-cd(p,q)}.
\tag{4.8; P}
\]

The intermediate sums are over unit bonds. Fine root sums carry \(\eta^4\), canceling the \(\eta^{-4}\) anchors per unit cube. Physical curvature has dimension two, giving the \(h^{-4}\) factor in (3.11).

The full Hessian has an additional minimizing-map term. If \(m(B)\) is the nonlinear minimizing map, then

\[
D^2(a_p\circ m)[u,v]
=D^2a_p(m)[Dm\,u,Dm\,v]
+Da_p(m)[D^2m(u,v)].
\tag{4.9; P}
\]

Here \(m\) is expressed through the Landau-gauge logarithmic field \(\mathcal H(B)\) of CMP 102 Proposition 9, pp.305–309. Its domain (172) and derivative estimate (190) give analyticity and first-derivative decay on a fixed complex neighborhood. On a strict inner ball of radius \(\rho\), coordinate Cauchy and symmetry give

\[
|D^2m(p;y,z)|
\le C\rho^{-1}e^{-c[d(p,y)+d(p,z)]/2}.
\tag{4.10; P in the current regular core}
\]

Cauchy first gives \(C\rho^{-1}e^{-cd(p,y)}\), and symmetry gives the same bound with \(z\). Taking their minimum proves (4.10). The same argument applies to the fine first derivative in (190). Endpoint scale powers equal one in this core; mixed-scale layers must keep their stated scale factors.

For density normalization set \(e_p=\eta^{-4}a_p\) in unit physical-block coordinates; thus \(V_f=\sum_p\eta^4f_pD^2e_p\). Using (4.10) in (4.9) gives an anchored two-leg bound for this complete plaquette Hessian density. Convolution with the constrained covariance bounds its quadratic two-mark kernel by
\(CX^{-2}h^{-8}e^{-cd_T(p,q)/h}\). The fifth rooted moment with measure \(a^4\) is \(CX^{-2}h^{-4}\), as in (3.11). The same bounds imply
\(\|C_X^{1/2}V_fC_X^{1/2}\|\le C\|f\|_\infty/X\).
Carrier locality uses the decoupled nonlinear maps below; it does not follow from pointwise decay alone.

**Hard-to-soft covariance bound (P with a common coarse constraint).** The two axial slices need not coincide. Let \(R\lambda\) generate the vertical gauge directions on \(E=\ker Q\), let \(S_{\mathrm h}\) be the hard tree-gauge slice, and let \(D\) be the averaged soft gauge map. Put \(A=DR\), which is invertible, and

\[
J_D=I-R A^{-1}D.
\tag{4.10a; P}
\]

Then \(J_D:S_{\mathrm h}\to\ker D\) is an isomorphism along gauge orbits, and \(KJ_D=K\). If \(\mathsf C_{\mathrm{hard},X}\) is the embedded covariance on \(S_{\mathrm h}\), independent Gaussian coordinates on \(S_{\mathrm h}\) and on the gauge parameters give

\[
\mathsf C_{\mathrm{soft},X}
=J_D\mathsf C_{\mathrm{hard},X}J_D^*
 +X^{-1}R(A^*A)^{-1}R^*.
\tag{4.10b; P}
\]

Indeed write the vector as \(J_Ds+R\lambda\); its quadratic form is \(X\langle s,Ks\rangle+X\langle\lambda,A^*A\lambda\rangle\), with no cross term. The constant coordinate Jacobian cancels on normalizing the Gaussian. On real backgrounds \(A\) is orthogonal by the endpoint identity above. Both \(R\) and \(D\) act within fixed-size coarse blocks with bounded coefficients, so (4.10b) transfers exponential covariance bounds and their rooted moments to the soft chart.

For this application the hard and soft forms must use the **same** averaging constraint. CMP 109 p.253 explicitly states that the preceding results apply to the admitted averaging operations; p.254 discusses the modified average, and p.267 after (2.11) identifies the quadratic form with CMP 99 (3.156), with delta gauge fixing replaced by exponential gauge fixing. This is the specific literature extension used to apply the hard bound with that common \(Q\). We do not identify a covariance for the old averaging definition with one for a different constraint. Nor does (4.10b) equate individual weighted quadratic Taylor marks in different nonlinear coordinate charts. Their complete Hessians, including (4.9), must be used in their own chart. Theorem 3.3 already uses CMP 109's own physical Hessian.

For the linear response, \(\sum_pv_p=0\) makes the row and column sums vanish. Expanding the two differences in (3.10) proves that identity. Omitting plaquettes gives the exact additional row-defect term. For the exact Wilson first variation, use the lattice curvature \(F_{\mathrm{bg}}(p)=a^{-2}\operatorname{Im}U_p\), with the harmless fixed trace normalization included in \(C\). The first variation is its pairing with the linearized plaquette curvature; this is an exact first-variation formula, not a replacement of the action by a principal quadratic model. On the stated critical background, exponential decay and the two source differences yield

\[
|b_f^TC_Xb_g|
\le CX^{-1}h^2\|\nabla f\|_\infty\|\nabla g\|_\infty
 \|F_{\mathrm{bg}}\|_{L^2}^2.
\tag{4.11; P on the stated core}
\]

Use the Lipschitz bounds and \(2|F_pF_q|\le|F_p|^2+|F_q|^2\); the exponential covariance has second moment \(O(h^2)\). This avoids a component-diameter loss.

For the complete quadratic Taylor marks in the same chart, Wick's rule gives the exact formula

\[
\operatorname{Cov}_{\gamma_{C_X}}(A_f^{[2]},A_g^{[2]})
=b_f^TC_Xb_g+\tfrac12\operatorname{Tr}(C_XV_fC_XV_g).
\tag{4.11a; P}
\]

The linear–quadratic terms vanish by oddness, and the two cross-pairings give the factor \(1/2\). This uses the full Hessian in (4.9). For physical marks multiply by \(N^2\).

To state the complete density-kernel estimate, write this covariance as \(\sum_{p,q}a^8f_pg_q\sum_YK^G_{h,Y}(p,q)\), with \(Y\) a connected carrier containing the two marked blocks. Let \(d_h(Y)\) be its block-tree size in shell units and \(\epsilon_{\mathrm{bg}}=\sup_p h^2|F_{\mathrm{bg}}(p)|\). With some reserved exponent \(\kappa_*>0\), the estimates above and the componentwise construction of §4.5 give

\[
\sup_p\sum_q a^4
\left(1+\frac{d_T(p,q)}h\right)^5
\sum_Y e^{\kappa_*d_h(Y)}|K^G_{h,Y}(p,q)|
\le
C h^{-4}\left(X^{-2}+\epsilon_{\mathrm{bg}}^2X^{-1}\right).
\tag{4.11b; P on the admitted current regular core}
\]

For the quadratic term combine the two exponentially localized Hessian legs with the two covariance contractions. For the linear term use the exact background curvature factors at the two roots and the exponentially localized first variations. In each case relative root summation contributes \(O(h^4)\) against a density kernel \(O(h^{-8})\). The fifth moment costs a fixed part of the decay. Componentwise decoupling retains the original marked blocks; a sufficiently large fixed Cauchy radius for each exterior block pays their counting and leaves the positive carrier exponent. At zero fluctuation the decoupled nonlinear map is zero, so changing its decoupling parameters leaves the actual background plaquette unchanged. Thus these carrier estimates retain the actual real \(\epsilon_{\mathrm{bg}}\). They do not replace a larger external-background Cauchy norm by that smaller real number.

These background-dependent terms are operator-valued source vertices, not yet vacuum scalars. A gradient gain alone is not claimed to remove every contact divergence. A fifth-moment source-kernel bound permits degree-four Taylor subtraction with remainder \(h^5h^{-4}=h\). Iteration still needs compatible partial-collision subtractions.

### 4.5 The interacting cluster estimate and fresh scalar admission

The integral is the actual CMP 109 (2.12)–(2.14), pp.268–269. Write \(\mathsf C_{\mathrm{sf}}=(\iota_{\mathrm{sf}}^*\Delta^{(k)}\iota_{\mathrm{sf}})^{-1}\) for its soft-gauge covariance in free averaging-constraint coordinates, with \(\iota_{\mathrm{sf}}\) the linear inclusion denoted \(C\) in that paper:

\[
I(s,t)=\int d\mu_{\mathsf C_{\mathrm{sf}}}(B)\,\chi_k(B)
 \exp\{V_k(U,B)+sW_f(U,B)+tW_g(U,B)\}.
\tag{4.12; L/P: frozen sourced integral}
\]

The potential retains the Haar and constraint Jacobians, higher gauge and Wilson terms, and the difference of the previous source-free effective action. The covariance, minimizing maps, and cutoff are independent of \(s,t\).

The precise marked input, on the same complex background/fluctuation/decoupling domains as CMP 116, is

\[
|W_i(Y,B)|\le w_i(Y)(1+\sum_{b\subset Y}|B(b)|^2),\qquad
\sup_b\sum_{Y\ni b}e^{\omega d(Y)}w_i(Y)\le a_i.
\tag{4.13; C: marked analytic carrier norm}
\]

The carrier exponent retains counting room, and each marked carrier contains its original source anchor, also after decoupling. Keep explicit slack in the unmarked estimates: \(\alpha_5\sup_Z\|\mathsf C_{\mathrm{sf}}(Z,0)\|\le1/4\), a fixed smaller complex background domain, and a rooted hard-core activity norm
\(\sup_\Delta\sum_{Z\ni\Delta}|H_0(Z)|e^{|Z|+\kappa'd(Z)}\le(4D)^{-1}\).
Here \(D\) is the fixed local incompatibility multiplicity. The parameter choices and exponential counting in CMP 116 Lemma 3 permit these stricter bounds in the regular bulk. They are premises when applying the lemma to any other integral.

**Marked cluster lemma (P as an implication of (4.13)).** For a sufficiently small fixed \(\delta\), the connected activities of (4.12) are analytic on \(|s|a_f+|t|a_g<\delta\), with a uniform exponential carrier bound. To prove this, insert the additional vertices into CMP 116 Lemma 2, (1.41)–(1.43). They increase the coefficients in its Gaussian domination estimates (2.20), (2.23) by at most \(C(|s|a_f+|t|a_g)\). Choose \(\delta\) below the unused margin in
\(\alpha_5\|\mathsf C_{\mathrm{sf}}(Z_0)\|<1/2\), (2.24). The determinant, tail, and carrier estimates through (2.38) then remain summable. Choose \(\delta\) also so that the additional rooted activity norm is at most \((4D)^{-1}\). The extra potential contributes at most a fixed construction-constant multiple of \(\delta\) after the same tree sums and carrier counts. The resulting norm is at most \((2D)^{-1}\); summing incompatibilities over the blocks of a polymer gives a strict connected-tree convergence margin. Polynomial carrier volumes use a reserved part of \(\omega\). The connected logarithm (2.39)–(2.41) supplies its analytic branch uniformly on smaller polydiscs. No positivity of individual activities is assumed.

Cauchy on radii \(\delta/(4a_f),\delta/(4a_g)\) gives (3.12). After subtracting the two one-source restrictions and the constant term, all remaining terms beyond \(st\) have total degree at least three; their geometric majorant gives the stated mixed remainder. An activity missing a source anchor has no dependence on that source. A connected carrier meeting both supports spends part of its decay on their separation.

For a fresh scalar mark, the holomorphic plaquette action is

\[
a(P)=1-\tfrac12\operatorname{tr}(P+P^{-1})
=-\tfrac12\operatorname{tr}[(P-1)^2P^{-1}].
\tag{4.14; P}
\]

Thus \(|a(P)-a(P_0)|\le C(|P_0-1||P-P_0|+|P-P_0|^2)\). The lifted-field bounds give a fine plaquette fluctuation \(Cg_B\eta^2\) times a local fluctuation envelope, while \(|P_0-1|\le\epsilon_{\mathrm{bg}}\eta^2\). Each marked difference therefore contributes
\(\eta^4(g_B\epsilon_{\mathrm{bg}}|B|+g_B^2|B|^2)\). Summing a unit block cancels its \(\eta^{-4}\) density.

For source and background locality, use CMP 116 (1.2)–(1.10), pp.2–4. The text between (1.9) and (1.10) proves that the deformed kernels vanish across disconnected components and that the nonlinear fixed-point equations separate componentwise. The lifted \(H_k(s,B')\) in an original block depends only on the component containing that block and its collar. Equations (1.11)–(1.21) control its complex derivatives, and (1.23)–(1.25) give the Cauchy carrier factor.

Apply that construction to the weighted plaquette difference in each original block. The bounded coefficients \(f_p\) remain in that block; neither propagators nor fixed-point equations change. All resulting carriers contain its source anchor. Differentiating the already localized expression retains the same carrier and includes the second term in (4.9). These estimates give (4.13) with (3.13). This proves admission for new scalar vertices in the admitted regular bulk, not for all older source derivatives or all boundary integrals.

### 4.6 Quantitative interaction and cutoff remainder

Suppose the interaction norm is \(v\), and \(W_i=Q_i+R_i\) has quadratic and remainder norms \(a_i,r_i\). Assume the Gaussian, analytic-domain, and polymer slack just specified, \(v\le c\delta\) so that a fixed \(u\)-disc contains the interval \([0,1]\), and the product cutoff in the independent free coordinates of (4.12). Interpolate by \(uV_k\) with fixed cutoff. The three-parameter Cauchy bound for \(\partial_u\partial_s\partial_t\), integrated from zero to one, bounds the interaction correction by \(Cva_fa_g\). Replacing either mark by its remainder contributes \(r_fa_g+a_fr_g+r_fr_g\).

Next compare the quadratic cutoff Gaussian with the untruncated quadratic Gaussian using factors
\(\prod_b(1-z\mathbf1_{\mathrm{bad},b})\). A changed connected activity contains a bad-field factor. The Gaussian tail estimate used in CMP 116 (2.22) supplies \(e^{-cR_{\mathrm{fl}}^2}\), uniformly on the smaller quadratic-source polydisc. Here \(R_{\mathrm{fl}}=\epsilon_{\mathrm{fl}}/g_B\). Only quadratic marks remain when the cutoff is removed; no nonlinear coordinate chart is extended beyond its domain. Thus the localized difference satisfies

\[
|D_{fg}(X)|\le C[
va_fa_g+r_fa_g+a_fr_g+r_fr_g
+e^{-cR_{\mathrm{fl}}^2}a_fa_g]e^{-\kappa_*d(X)}.
\tag{4.15; P under the stated regular-bulk norms}
\]

For precision, the **matched regular bulk** here means exactly the integral CMP 109 (2.13), with the previous source-free \(E\) satisfying its (1.18), the specified free-coordinate product cutoff, and the source-free minimizing maps. CMP 116 Lemma 1, (1.33)–(1.36), bounds the whole old-\(E\) increment; Lemma 2, (1.41)–(1.43), bounds the remaining potential, including both Jacobians and the gauge and Wilson remainders. These give \(v=O(\epsilon_{\mathrm{fl}})\). This statement does not yet identify every term of CMP 119 (3.15) with that integral.

For constant scalar marks the stationarity-reduced quadratic norm is \(O(g_B^2)\). The fixed raw-fluctuation analytic radius \(\rho\) in CMP 116 (1.14)–(1.21) is independent of the smaller cutoff \(\epsilon_{\mathrm{fl}}\). After the stationary linear term and quadratic Taylor term are removed, the mark remainder starts at degree three. On \(g_B|B|\le\epsilon_{\mathrm{fl}}\), its bound \(Cg_B^3|B|^3\le C\epsilon_{\mathrm{fl}}g_B^2|B|^2\) gives \(r_i=O(\epsilon_{\mathrm{fl}}g_B^2)\), with the same carrier localization. Hence

\[
|D_{11}(X)|\le Cg_B^4[
\epsilon_{\mathrm{fl}}+e^{-c\epsilon_{\mathrm{fl}}^2/g_B^2}]
e^{-\kappa_*d(X)}.
\tag{4.16; P for the defined CMP 109 regular-bulk integral}
\]

The summed physical Gaussian response is the vacuum scalar in (3.9). Therefore the vacuum-subtracted total constant-source response is represented by
\(\sum_X[D_{11}(X,U)-D_{11}(X,1)]\), with the displayed bound on each difference. This is a chosen representation of the difference, not a termwise cancellation in a prior Gaussian recipe.

With a matched logarithmic cutoff \(\epsilon_{\mathrm{fl}}=g_Bq(g_B)\), the coefficient is
\(Cg_B^5q(g_B)+Cg_B^4e^{-cq(g_B)^2}\). LFR I (1.9), p.178, explicitly has \(|A_j|<g_j^{-1}\delta_j\); CMP 119 p.265 defines \(\delta_j=g_j(A_1/A_0)p_0(g_j)\). This is the regular \(p_0\) threshold, distinct from the R-core \(p_1\) threshold. Applying the sharper bound to any particular CMP 119 boundary integral still requires matching its coordinates and selectors.

### 4.7 A local contact subtraction for the Gaussian vacuum two-mark kernel

**Proposition 4.1 (P: Gaussian vacuum contact estimate).** Restrict the complete quadratic Gaussian kernel to the identity background. Its linear part vanishes; write the remaining density kernel as \(K_h^{\mathrm{vac}}(p,q)\). Equation (4.11b) gives its absolute fifth rooted moment with coefficient \(CX^{-2}h^{-4}\). For smooth scalar tests define

\[
B_h^{\mathrm{vac}}[f,g]
=\sum_{p,q}a^8f(x_p)g(x_q)K_h^{\mathrm{vac}}(p,q).
\tag{4.17; P: definition}
\]

Choose once a smooth displacement cutoff \(\chi\), equal to one near zero and supported in the ball of radius \(\ell_0/8\). All compatible tori have a unique local displacement coordinate on this ball. Let \(r_{pq}\) be the lift of \(x_q-x_p\) in this local ball wherever the cutoff is nonzero; thus the distance used here is \(d_T(p,q)=\operatorname{dist}_T(x_p,x_q)\). Set

\[
c_{\alpha,h}(p)
=\frac1{\alpha!}\sum_q a^4
  \chi(r_{pq})r_{pq}^{\alpha}K_h^{\mathrm{vac}}(p,q),
\qquad |\alpha|\le4,
\quad
C_h^{\mathrm{vac}}[f,g]
=\sum_p a^4f(x_p)
  \sum_{|\alpha|\le4}c_{\alpha,h}(p)\,\partial^\alpha g(x_p).
\tag{4.18; P: local contact prescription on smooth tests}
\]

Terms with zero cutoff need no choice of displacement. This counterterm is supported on the source diagonal as a bilinear distribution: it depends on both tests at the same point, with derivatives through order four. For the symmetrized prescription replace \(C_h^{\mathrm{vac}}[f,g]\) by one half of its sum with \(C_h^{\mathrm{vac}}[g,f]\).

Taylor's theorem near zero, and the fixed positive distance from zero on the complement where \(1-\chi\ne0\), give the global bound
\[
\left|g(x_q)-
\chi(r_{pq})\sum_{|\alpha|\le4}
  \frac{r_{pq}^{\alpha}}{\alpha!}\partial^\alpha g(x_p)\right|
\le C_{\ell_0}\|g\|_{C^5}\,d_T(p,q)^5.
\tag{4.19; P}
\]

Here the \(C^5\) norm uses the physical \(\ell_0\) convention, and orientation multiplicities are fixed. Combining this bound with the fifth rooted moment proves

\[
|B_h^{\mathrm{vac}}[f,g]-C_h^{\mathrm{vac}}[f,g]|
\le C_{\ell_0}X^{-2}h\,\|f\|_{L^1_a}\|g\|_{C^5}.
\tag{4.20; P}
\]

The complete quadratic Gaussian covariance gives \(K_h^{\mathrm{vac}}(p,q)=K_h^{\mathrm{vac}}(q,p)\), hence \(B_h^{\mathrm{vac}}[f,g]=B_h^{\mathrm{vac}}[g,f]\). For the symmetrized prescription use the average of the two bounds with \(f,g\) interchanged. The identity is an equality of bilinear forms on smooth tests; no finite-source analyticity claim is needed.

The physical shell lengths form a geometric sequence ending at the fixed physical scale. Thus \(\sum_hh\le L\ell_0/(L-1)\), uniformly in the number of ultraviolet steps. If \(X^{-1}\) stays in the admitted bounded interval, the sum of the remainders (4.20) is uniformly bounded for compactly supported tests, independently of the fine spacing and admitted torus size. The coefficients \(c_{\alpha,h}\) themselves can diverge on summing shells; they are precisely the local contact subtractions.

This proves the Gaussian **vacuum** part of the proposed degree-four contact mechanism. It does not subtract an operator-valued retained-field term, identify the counterterm for the full interacting measure, establish its compatibility with all higher products, or prove convergence of the underlying non-Gaussian distributions. Those distinctions matter even though the Gaussian remainder is already summable.

## 6. Interface supplied by this calculation

### 6.1 Assumed flow and normalization

For completeness, the only numerical flow interface allowed by the original program is reproduced unchanged below. Its status is **(C: assumed interface)**.

> **(N2-F) Coupling flow.** There are constants γ ∈ ]0, 1], b_0 > 0, C_r < ∞, depending only on N, L and Balaban's fixed construction constants, such that for every K ∈ N and every g\_\* ∈ ]0, γ/2] there is a bare coupling g_0 = g_0(K; g\_\*) with the following properties. Let x_k = g_k^{-2}, k = 0, …, K, be Balaban's effective couplings for the theory on Λ\_{a,T}, a = L^{-K} ℓ_0 (x_k is the coefficient of the Wilson term in the inductive representation of ρ_k, in the normalization in which x_0 = g_0^{-2} = β_a/(2N); by N0's dictionary D2 it does not depend on the torus T). Then: (i) x\_{k+1} = x_k − b_0 log L + r_k(x_k) with |r_k(x)| ≤ C_r/x for all 0 ≤ k < K and all x ≥ γ^{-2}; (ii) g_k ≤ γ for all 0 ≤ k ≤ K; (iii) g_K = g\_\*; (iv) x_0 = b_0 K log L + O(log(K+1)) with the O depending only on (N, L, g\_\*); (v) g\_\* ↦ g_0(K; g\_\*) is continuous on ]0, γ/2]; (vi) each r_k extends to a function of x that is C^1 on [γ^{-2}, ∞) with |r_k′(x)| ≤ C_r/x². Here b_0 is the one-loop coefficient in the normalization x = g^{-2} (expected value 11N/(24π²) for SU(N); the value in the preamble's conventions, with its derivation, is part of the coupling-flow input N2-F).

The coefficient sentence in that quote still needs the explicit normalization repair stated as **ICR-N1-1** in [Lattice conventions and hypotheses](../lattice_conventions.md), §4. Here we keep the prescribed Wilson measure and use \(X_{B,0}=2N^2x_0\) at initialization. Identifying the entire normalized running sequence with Balaban's literal coefficients remains part of the source-free base ledger. The one-step results in §§3–4 are stated directly in the literal Balaban coefficient \(X=g_B^{-2}\), so they do not depend on silently repairing the quote.

Only the numerical recurrence, admitted interval, and terminal value are used in the smaller-ceiling argument of §4.2 and the summability calculation below. They are algebraic consequences for that sequence; applying them to a complete Wilson construction requires the coefficient identification. No position-dependent flow, second derivative of \(r_k\), or uniform source-dependent tensor transport is assumed. No new ICR is required by the present one-step results.

### 6.2 The large-field operation can receive complete jets with an explicit bound

**Theorem 6.1 (P: receiving implication).** Let \(\sigma\) be the actual post-cancellation positive measure of Theorem 3.2, with \(t=\sigma(1)\), \(Q=\sigma/t\), and \(\sigma(e^{s\mathcal V})\le\varepsilon_k\). Suppose the complete incoming first and second logarithmic jets obey, on every sampled field and history,

\[
|A_f-c_f(v)|\le b_f\mathcal V,\qquad
|A_g-c_g(v)|\le b_g\mathcal V,\qquad
|A_{fg}-c_{fg}(v)|\le b_{fg}(\mathcal V+\mathcal V^2).
\tag{6.1; C: the receiving hypotheses}
\]

All three \(c\)'s depend only on the retained variables of this operation, not on its integrated variables or summed histories. Then

\[
|\sigma(A_f)-tc_f|
\le b_fs^{-1}\varepsilon_k,
\tag{6.2; P}
\]

and

\[
\left|t\left[
QA_{fg}+\operatorname{Cov}_{Q}(A_f,A_g)-c_{fg}
\right]\right|
\le
\left[b_{fg}(s^{-1}+2s^{-2})
+4b_fb_gs^{-2}\right]\varepsilon_k.
\tag{6.3; P}
\]

**Proof.** Use (3.6) for the first and second powers of \(\mathcal V\). The incoming second-jet contribution is at most \(b_{fg}\sigma(\mathcal V+\mathcal V^2)\). The covariance is at most \(2b_fb_g\sigma(\mathcal V^2)\) by (3.3). The exact transport identity (2.4) then gives (6.3). On a zero-mass component all density-weighted outputs are defined to be zero. No rare-mass denominator remains. The retained contribution is still \(tc_{fg}(v)\); it has not been declared a vacuum scalar. \(\square\)

### 6.3 The regular carrier norm implies the receiving volume norm

At scale \(j\), let the actual sampled coordinates satisfy \(|B_j(b)|\le P_j\). Suppose

\[
|W_{f,j}(Y,B_j)|
\le w_{f,j}(Y)\left(1+\sum_{b\in Y}|B_j(b)|^2\right),\qquad
\sup_b\sum_{Y\ni b}e^{\lambda d_j(Y)}w_{f,j}(Y)\le a_{f,j}.
\tag{6.4; C: input carrier and cutoff norm}
\]

Here \(Z_j^+\) is the fixed enlargement of the history domain counted in \(\mathcal V\). Sum a carrier meeting \(Z_j^+\) over all its intersection bonds, an overcount. Connected carriers satisfy \(|Y|\le C_\lambda e^{\lambda d_j(Y)/2}\), so a reserved part of the exponential norm pays the fluctuation volume. This proves

\[
\sum_{Y:Y\cap Z_j^+\ne\varnothing}|W_{f,j}(Y,B_j)|
\le C_\lambda a_{f,j}(1+P_j^2)|Z_j^+|_j.
\tag{6.5; P}
\]

Consequently, if \(\sup_j a_{f,j}(1+P_j^2)\le C_f\|f\|_{C^5}\), the sum over all assigned history pieces is bounded by \(CC_f\|f\|_{C^5}\mathcal V\). Part of the source-to-component carrier decay can be retained; it need not all be spent on \(|Y|\). A polynomial envelope of degree \(r\) instead requires the corresponding bound with \(1+P_j^r\).

For a fresh scalar fluctuation vertex, (3.13) gives the concrete coefficient test

\[
a_{f,j}(1+P_j^2)
\le C\|f\|_\infty
(g_{B,j}\epsilon_{\mathrm{bg},j}+g_{B,j}^2)(1+P_j^2).
\tag{6.6; P in the matched regular sector}
\]

This is uniformly bounded for an actual logarithmic cutoff \(P_j\) and a fixed bounded \(\epsilon_{\mathrm{bg},j}\). On a shrinking real background it has the sharper \(g_{B,j}^2\) times logarithms. Thus the fresh fluctuation parts do meet the receiving volume test when the sampled coordinates and cutoff are matched to the regular sector used in §4.5.

The extracted background value requires separate care. A quantity independent of one small-field fluctuation can depend on variables integrated by a later R-operation. It can be put in \(c_f(v)\) only if it is independent of **all** the variables and histories summed by that later operation. Otherwise it remains in \(A_f\). An explicit regular plaquette sum over a counted region can be bounded by \(C\|f\|_\infty\epsilon_{\mathrm{bg},j}^2\) times its scale-volume: each plaquette contributes \(C\epsilon_{\mathrm{bg},j}^2\eta^4\), canceling the fine plaquette density. Applying that estimate requires the actual sampled background to satisfy the stated regularity there. There is no such conclusion for an arbitrary old background merely because its value was once extracted.

Equations (6.5)–(6.6) are a proved partial transfer of estimates from the small-field calculation to the large-field calculation. They do not assert (6.1) for all propagated marked E/R/B terms.

### 6.4 Complex backgrounds require relative mass control

Complex covariance below means the bilinear cumulant used by holomorphic differentiation, with no complex conjugation.

For an analytic continuation of a component, sufficient hypotheses are

\[
d\sigma_z=G_z\,d\sigma_0,\qquad
|G_z|\le M,\qquad
|t_z|=|\sigma_z(1)|\ge c\,t_0,\qquad c>0,
\tag{6.7; C: relative-integrand and relative-mass bounds}
\]

together with the incoming bounds (6.1) throughout that domain. Cauchy–Schwarz in the real positive measure gives

\[
\left|t_z\left[
Q_zA_{fg}+\operatorname{Cov}_{Q_z}(A_f,A_g)-c_{fg}
\right]\right|
\le
\left[
M b_{fg}(s^{-1}+2s^{-2})
+2\left(M+\frac{M^2}{c}\right)b_fb_gs^{-2}
\right]\varepsilon_k.
\tag{6.8; P from the displayed hypotheses}
\]

For the product of first moments, use \((\sigma_0\mathcal V)^2/t_0\le\sigma_0(\mathcal V^2)\). This cancels the small real mass. LFR II (1.73)–(1.75), p.380, supplies (6.7) for its admitted complex **background** continuation, with \(M=e^\epsilon\), \(c=e^{-2\epsilon}\), for sufficiently small \(\epsilon\), after bounding the complete relative exponent by \(\epsilon\). The marked vertices must extend to that domain with their own bounds.

This does not give a uniform complex-source neighborhood for the logarithm of every sourced rare component. For example, on two histories of total mass \(t_n\), take \(\mathcal V=n\) and a mark \(F=\pm n\). Then \(\sigma_0(e^{s\mathcal V})=t_ne^{sn}\) can be arbitrarily small while \(\sigma_0(e^{zF})=t_n\cosh(nz)\) has a zero at \(z=i\pi/(2n)\). The finite density-weighted jets at zero source remain controlled. Their calculation needs no uniform nonvanishing disc for these component logarithms.

### 6.5 The regular constant-source error has a summable coupling power

**Proposition 6.2 (P: numerical consequence of the narrowed N2 recurrence).** On the sufficiently small terminal trajectory chosen in §4.2, let \(b=b_0\log L>0\). The drift gives

\[
x_j\ge x_K+\tfrac b2(K-j).
\tag{6.9; P}
\]

For every fixed \(p>2\) and \(q\ge0\), comparison with the integral of \(x^{-p/2}(1+\log x)^q\) yields

\[
\sup_K\sum_{j=0}^{K}g_j^p(1+|\log g_j|)^q
\le C_{p,q,b}\,
g_*^{\,p-2}(1+|\log g_*|)^q<\infty
\tag{6.10; P}
\]

after enlarging the fixed constant on the chosen terminal interval. A fixed normalization conversion gives the same conclusion for the literal Balaban couplings once that conversion is identified at every scale.

Therefore the coefficient \(g_B^4\epsilon_1\) in the checked fixed-cutoff version of (4.16) has a summable scale power. A correctly matched logarithmic cutoff gives the stronger \(g_B^5q(g_B)\) plus Gaussian-tail coefficient. This is a useful check on the constant-source regular-bulk calculation.

Summability of an activity coefficient does not remove a physical root density \(h^{-4}\), prove a contact subtraction, or control accumulated operator mixing. Nor does it match the boundary terms automatically. Those separate operations are precisely the ones required for the induction in §7.

### 6.6 Delivered versus still required

| Item | Status at the end of this calculation |
|---|---|
| Exact frozen first/second-jet transport | **P**, including the incoming second jet |
| Bare scalar marks in the actual positive old-history operation | **P**, with the explicit history-domain counting and smaller ceiling |
| Complete fixed-map Gaussian calculation for linear and quadratic Taylor marks on the stated regular core | **P/L**, with nonlinear Hessian terms, the hard/soft distinction, and the stated covariance imports |
| Local contact subtraction for the Gaussian vacuum two-mark kernel | **P**, with the summable remainder (4.20) |
| Fresh scalar vertices in the actual B109/B116 interacting regular integral | **P**, with an anchored analytic norm and quantitative source remainder |
| Constant-source quadratic Gaussian vacuum cancellation and interacting comparison | **P** for that defined bulk integral; logarithmic-cutoff application requires its matching conditions |
| Conversion of an admitted carrier norm into the receiving history norm | **P** as the explicit implication (6.4)–(6.6) |
| Bounds for all propagated first and second E/R/B/contact vertices | **O** |
| One closed two-insertion induction, uniformly in ultraviolet depth | **O** |
| A renormalized continuum two-point distribution, or the complete YM-E target | **O**; neither is claimed here |

## 7. Residual propositions for a complete scalar two-insertion induction

The first induction step of this approach is still open. It is now narrower than the original finite-source stability theorem: the regular-bulk fresh vertices, complete Gaussian Taylor calculation, Gaussian vacuum contact subtraction, and large-field receiving estimate have been supplied. The following propositions are needed to connect them for the complete observable.

### R1. Match the complete localized step, including backgrounds that become variables (O)

Start with the original physical scalar mark \(A_f=N\sum_p f_pa_p\) and \(A_{fg}=0\). In the full CMP 119 transformation (3.15), identify each first and second derivative with the corresponding term of the exact frozen-map formula (2.4). The ledger must include previous marked E-terms, all R- and B-terms, geometry-dependent Wilson increments, old normalizers, dependent-coordinate constraints, and every selector appearing in the actual sampled integral.

For each such term specify its actual coordinates, its source anchor or pair of anchors, and whether it is integrated or retained by the current operation. Match the interior part to (4.12) and place the remaining terms in the history norm. In particular, a previously extracted minimizing-background value must not be treated as a retained constant if this step integrates variables on which it depends.

**Required conclusion:** the complete first and second jets have the analytic regular-sector bounds and the pointwise bounds (6.1) on every admitted history, with constants independent of the number of past steps after the specified normalizations. Source-free bounds on E/R/B do not imply bounds on their external-source derivatives.

### R2. Preserve the two source anchors through localization and histories (O)

The marked bulk construction retains anchors, and (6.5) retains part of the decay from an anchor to a history domain. The complete localized R-operation must preserve these properties when all histories and previously generated carriers are combined.

For two marked carriers \(Y_f,Y_g\) attached to an erasable component \(X\), the natural union is \(X\cup Y_f\cup Y_g\). Show that the outgoing connected second coefficient can be decomposed into connected carriers of this type, or their controlled enlargements, with a positive remaining decay exponent and a summable rooted norm. For carriers wholly inside an erasable \(X\), the remaining \(p_0(g_k)\) suppression pays its logarithmic geometry. Long carriers extending outside \(X\) require their own source-to-boundary decay and cannot be counted only by \(|X|\).

The proof must also specify how finite tori, wrapping carriers, and the mixed-scale layers use the original geometric hypotheses. The terminal-core estimates in §4.4 cannot be reused with all endpoint scale factors set to one in those layers.

### R3. Give one local extraction for the interacting and operator-valued two-jet (O)

The vacuum Gaussian contact subtraction in §4.7 is proved. The full second jet also contains the retained-field term (4.11), nonlinear interactions, the incoming \(A_{fg}\), and boundary/history contributions. It needs one compatible projection onto:

- identity terms and source-contact distributions;
- the dimension-four scalar field channel, with its running normalization;
- the remaining irrelevant vertices, retained in a norm that contracts after rescaling.

The exact source-difference formula handles the leading linear Gaussian part without a component-diameter loss. The summed constant-source Gaussian identity removes its field-dependent zero-mode response in the physical family. Neither identity defines the general interacting projection for nonconstant \(f,g\).

**Required conclusion:** define the contact and marginal coefficients from the actual localized second jet, prove their source-diagonal support and symmetry properties, and bound the remaining vertex in the same carrier/history norms used in R1–R2. Show that a term subtracted at this step is neither lost nor counted twice when it reappears as an incoming second vertex. The Gaussian prescription alone is not a renormalization prescription for the full theory.

### R4. Close the scale inequality in those norms (O)

After R1–R3, write the actual inequality for the normalized first-jet carrier norm, the connected second-jet norm, and the associated history bounds at consecutive scales. The factors must come from the rescaling and the computed marginal projection. An unspecified contraction constant is not an estimate.

The results proved here supply three parts of this inequality: the receiving bound (6.3), the regular mixed activity and comparison bounds (3.12), (4.15), and the Gaussian vacuum contact remainder (4.20). The constant-source regular comparison has a summable coupling coefficient by (6.10). These facts still do not bound the complete propagated marginal coefficient or the mixed-scale boundary remainder.

A successful inequality must yield cutoff- and volume-uniform renormalized two-point distributions on compactly supported tests, with a quantitative short-distance singularity bound. The hierarchy must also retain the one-point terms needed when passing from logarithmic derivatives to full moments. A uniform bound on a single conditional covariance is not that conclusion.

### R5. Scope beyond the first induction gate (O)

Even a completed R1–R4 would be a scalar two-insertion theorem. The full P1 target still needs the controlled three-point ultraviolet coefficient, all finite mark orders with the prescribed growth, the full tensor family and its actual mixing, restoration of continuous rotations, corrected OS reconstruction for the compatible hierarchy, and the energy/phase argument of §§4.10–4.11 ([Gaussian admission, gauge projection and reconstruction](gauge_projection.md)). Those are not inferred from the present scalar estimates.

The stronger energy-tilt reserve discussed in §4.2 is optional for the volume-norm approach developed here. It remains open unless its nested reference cancellations are verified, but it need not be made a prerequisite for R1–R4. The numerical two-point example in §6.4 also shows why the new approach works with finite density-weighted jets instead of demanding a uniform logarithm for each sourced rare component.

**Current mathematical conclusion:** the approach has passed several concrete one-step tests. The remaining gap is an interacting marked induction with local extraction and controlled histories. This paper neither proves that gap impossible nor assumes it solved.

