# Original point phases and complete first coefficient

**Current status:** Parts I–III and VII now close the mean-metric and bounded-initial-seed phase-moment question left below. Scalar and pseudoscalar mean-normalized seeds are covered. The fully renormalized stress/Weyl point-family issue remains separate.

**Scope:** The original frozen regular observable kernels, the actual Wilson/clover microscopic family, and their admitted intrinsic source norms. The preceding N7 derivation is retained in Appendix G. This module does not substitute a global random-phase kernel for the original chain.

**Status:** The common original-kernel point normalization is not yet proved. This module establishes an exact phase-digit representation for the deterministic bulk, a sharper actual finite-jet expansion, a local endpoint comparison, and a finite-volume projection estimate. It also proves mean scalar one-loop neutrality for the actual Wilson density, using the constrained physical Hessian and an explicit residual-gauge projection, with the normalized cutoff flux retained. The resulting scalar mean normalization is uniformly bounded. This does not control anisotropic marginal components created by individual blocking phases. The original-kernel translation-averaged S2 theorems are in [Appendix D](observable_appendix_d.md). The remaining actual matrix hypothesis is substantive.

### 1. The actual microscopic family and its symmetry

Keep the previously constructed positive Wilson/clover family. With \(s_p=N-\operatorname{Re}\operatorname{Tr}U_p\), its scalar trace is

\[
q_W(x)=\frac1{2a^4}\sum_{p\ni x}s_p,
\qquad
Q^W_{AB}=Q^C_{AB}+\frac{\delta_{AB}}6(q_W-q_C),
\qquad
a^4\sum_xq_W(x)=2S(U).
\tag{N8.1}
\]

The incident sum contains 24 leaves. These formulas, positivity, and the exact hypercubic transformation law were proved in the microscopic observable construction. The matrix has 21 independent entries. Its smooth curvature jet is the symmetric bilinear form on the six two-form components.

For a local scalar source \(j(x)\), the exact geometric identity is

\[
a^4\sum_xj(x)q_W(x)
=2\sum_p\bar j_p s_p,
\qquad
\bar j_p=\frac14\sum_{x\in\partial p}j(x).
\tag{N8.2}
\]

Thus a local Wilson source is a specified perturbation of the four incident plaquette couplings. It is not a derivative of the running coupling trajectory. A constant source reproduces the action derivative, with the factor two in (N8.1).

Although \(q_W\) is a scalar under simultaneous rotations of the lattice, an individual blocking phase need not preserve the rotation group fixing its root. Consequently the phasewise transport of this scalar may have anisotropic dimension-four curvature coefficients. Those coefficients belong to the other marginal channels. They cannot be put into the stable space merely because their phase average vanishes. The mean covariant action and a single phase operator have different symmetry statements.

### 2. Finite-volume projections can be compared without a fine-mesh loss

Use the smooth physical cutoff-affine tests of A7.31a–A7.32, with independent current \(J=0\). Suppose the torus of physical diameter \(D\) contains the required protective patches, and let two test centers differ by at most \(C h_k\). Choose the cutoff plateaux so that both include a common ball of radius \(cD\) about the rooted support.

On a coefficient supported in that common plateau, changing the affine origin changes its test connection by a constant one-form. This is a local linearized gauge direction. The Hessian of an invariant coefficient annihilates it because its first differential at the flat pair vanishes. The two curvature functionals therefore agree exactly on that coefficient.

For a remaining coefficient the connected support must reach a distance at least \(cD/h_k\) in current units. Its directional Cauchy bound has only a fixed polynomial support factor, uniformly in the original fine mesh. The rooted exponential norm absorbs it. Thus, within the same finite volume,

\[
\left\|\Pi_{k,x}f-\Pi_{k,y}f\right\|
\le C e^{-cD/h_k}\|f\|_{k,\kappa},
\qquad |x-y|\le Ch_k.
\tag{N8.3}
\]

The same estimate applies to the difference between translating a test and translating the rooted field, when the compared plateaux overlap as above. A smooth cutoff has no discontinuous seam and introduces no power of the microscopic mesh \(a^{-1}\).

For any fixed polynomial exponent \(p\), the AF upper increment and \(h_j=h_KL^{-(K-j)}\) give

\[
\sum_{j<K}\left(\frac{x_j}{x_K}\right)^p e^{-cD/h_j}
\le C_p e^{-c'D/h_K},
\qquad x_j=g_j^{-2}.
\tag{N8.4}
\]

This proves a summable projection/reanchoring error on the admitted periodic family. It does **not** prove that two independently constructed finite- and infinite-volume quantum coefficients agree locally. That identification uses the actual compatible local coefficient construction; a norm bound alone cannot establish it. No arbitrary physical-current test in the cutoff annulus is identified with the independent-current test.

### 3. What a common-patch adjoint graph does, and what it does not do

Consider the full marginal/stable recurrence on one protected rooted patch. Use the backward critical row from S8.6–S8.7,

\[
\ell_k=(I,V_k),\qquad
\ell_{k+1}L_k=E_k\ell_k,
\qquad V_K=0,
\qquad \|V_k\|\le Cg_k^2.
\tag{N8.5}
\]

The bound follows from the small reverse block and the stable contraction. The operator \(L_k\) here is the same original operator for both insertions being compared; the coefficients and projection are not changed for the second insertion.

If two microscopic seeds \(q_x,q_y\) have bounded separation in microscopic current units, their union fits one fixed protected patch and their curvature jets are equal. Hence \(q_y-q_x\in\ker\Pi_0\), with bounded rooted norm. Let \(P_{K,0}=E_{K-1}\cdots E_0\) for the reference seed in this common patch. The terminal marginal difference is exactly

\[
\Pi_K L_{K-1}\cdots L_0(q_y-q_x)
=P_{K,0}V_0(q_y-q_x),
\qquad
\|V_0(q_y-q_x)\|\le Cg_0^2.
\tag{N8.6}
\]

This is a useful endpoint comparison for nearby roots. It retains the stable feedback instead of charging a new unrelated \(O(g_k^2)\) error at every later step.

It is not yet a global common normalization. The cocycle in (N8.6) belongs to the chosen reference patch. For two roots at fixed distinct physical positions, their initial support separation is of order \(L^K\). A rooted exponential norm for their difference can then cost

\[
\|q_y-q_x\|_{0,\kappa,x}
\le C\exp(C\kappa |y-x|/a),
\tag{N8.7}
\]

which is not a usable uniform endpoint bound. Chaining adjacent-root comparisons likewise introduces a number of links depending on the microscopic depth. The positive phase example SP22–SP29 is consistent with uniformly controlled neighboring-root comparisons while its macroscopically separated roots acquire different powers of the ultraviolet scale interval. Thus a local adjoint graph does not, by itself, prove a uniformly bounded spatial corrector.

For a 21-channel common normalization, even a proved \(W_0(x)-I=O(g_0^2)\) still requires the matrix endpoint condition SP37, or an appropriate weaker bound for the intended conclusion. Matrix conjugation by the complete marginal product cannot be omitted.

### 4. Exact independent-digit representation of the deterministic bulk

This section applies to a deterministic bulk sequence with the compatible covariance of its **complete** original operators. It is an identity about translated insertions, not a modification of the forward kernel.

Let \(T_n\) translate an observable by \(n\) current lattice units, and suppose

\[
\widehat Q_k T_{Ln}=T'_n\widehat Q_k,
\qquad \widehat Q_k=L^4Q_k.
\tag{N8.8}
\]

For \(r\in\{0,\ldots,L-1\}^4\), define the reanchored phase operator

\[
L_{k,r}=\widehat Q_k T_r.
\tag{N8.9}
\]

All its outputs are rooted in one fixed enlarged coarse patch. Write a microscopic root as

\[
x=L^k n_k+\sum_{j=0}^{k-1}L^j r_j.
\tag{N8.10}
\]

Repeatedly using (N8.8) gives the exact field identity

\[
\widehat Q_{k-1}\cdots\widehat Q_0(T_xq_0)
=T_{n_k}\,L_{k-1,r_{k-1}}\cdots L_{0,r_0}q_0.
\tag{N8.11}
\]

The induction is elementary: write \(n_k=Ln_{k+1}+r_k\), move \(T_{Ln_{k+1}}\) through the next complete operator, and retain \(T_{r_k}\) in the phase map.

On a periodic torus whose microscopic side lengths are divisible by \(L^K\), a uniform microscopic translation has independent uniform lower base-\(L\) digits:

\[
\Pr(r_0=s_0,\ldots,r_{K-1}=s_{K-1})=L^{-4K}.
\tag{N8.12}
\]

The remaining coarse anchor is independent of these digits. Reanchoring removes it from the bulk rooted norm. Equations (N8.11)–(N8.12) therefore give the exact independent-phase representation needed by S8-B for a covariant bulk sequence. A fixed multi-step block uses complete phase words; its contraction must be proved uniformly over those words. A7's direct polynomial-jet proof applies with one common root collar because the total physical displacement in such a word is bounded by a constant times the output scale.

The mean operator is \(\overline L_k=L^{-4}\sum_rL_{k,r}\). As an algebraic mean of insertion maps it is the same finite average that occurred in N7.53. Here it is used only to define a deterministic comparison coordinate and its normalization. All covariance telescopes continue to use the original kernels.

#### 4.1 Born forcing is not automatically independent of future phases

An arbitrary historical forcing profile can depend on the current geometry and on higher root digits. It must not be inserted into the independent-phase martingale theorem as though it were independent of those digits. The appropriate estimate is instead N7.49, applied uniformly over complete phase words, followed by the weighted age convolution N7.50–N7.51. A uniform narrow-chart forcing bound controls its translation-averaged norm without an independence assumption.

Thus only the pure benchmark needs the independent-digit moment theorem. Regular \(R\) corrections can use the deterministic polynomial propagator and the actual identified action difference from Gate 1. Mixed-boundary and terminal terms retain their separate actual-law obligations.

### 5. The frozen amplitude map is even, and its actual first coefficient is explicit

Use the amplitude interpolation of J6–J8 and N7.40. The cutoff domain \(D_k\) is the actual symmetric domain, held fixed. Old couplings and potentials are also fixed. For a joint insertion \(f(U,J)\), write its integrand \(F_{\tau,u}(A)\) and its action \(H_{\tau,u}(A)\), with \(u\) a finite collection of smooth background test parameters.

The analytic pair map depends on the amplitude through \(\tau A\), and the classical remainder has the form \(\tau^{-2}W(U,J,\tau A)\), with cubic vanishing. Therefore

\[
F_{-\tau,u}(A)=F_{\tau,u}(-A),
\qquad
H_{-\tau,u}(A)=H_{\tau,u}(-A).
\tag{N8.13}
\]

Changing variables \(A\mapsto-A\) in numerator and denominator proves that the normalized expectation \(\Psi(\tau,u)\) is exactly even in \(\tau\). This is stronger than the first-derivative cancellation alone.

At zero amplitude, \(F_{0,u}\) is independent of \(A\). In the exact second-derivative identity J11, the covariance with \(H''_0\) and the third cumulant with \(F_0\) therefore vanish. For an admitted local source define the actual curvature-jet operator

\[
\mathfrak B_k f
=\frac{L^4}{2}\Pi\left[
 \mu_{0,u}\bigl(F''_{0,u}\bigr)
 -2\mu_{0,u}\bigl(F'_{0,u}H'_{0,u}\bigr)
 \right]_{u=0}.
\tag{N8.14}
\]

Here \(\Pi\) means the prescribed background Hessian, not evaluation before differentiation. The product expectation in the second term is a covariance because \(\mu_{0,u}F'_0=0\). The score \(H'_0\) contains the classical cubic remainder, the old-action linear score, and the Jacobian score. They must all be retained.

The same fixed-order cumulant argument as N7.40–N7.44 can be carried to four amplitude derivatives and two background derivatives. Cumulants of order at most seven suffice. The source Taylor remainder gives finite local polynomial bounds; the flat HC-W and moment estimates sum their locations. Thus

\[
\boxed{
\Pi L^4Q_kf
=\Pi L^4Q_{0,k}f+g_k^2\mathfrak B_kf
+O(g_k^4\|f\|_{\rm input}).
}
\tag{N8.15}
\]

The constants are uniform on the admitted fixed domain. This is an auxiliary-amplitude expansion at frozen physical data. The coefficient \(\mathfrak B_k\) can depend on the old action, the actual cutoff, and the microscopic depth. It has not been identified with a universal continuum coefficient merely by calling it the first coefficient.

For the microscopic current-unit seed \(q_{k,x}\), the required actual phase function is therefore

\[
b_k(x)=\mathfrak B_kq_{k,x},
\qquad
\bar b_k=L^{-4}\sum_{r\bmod L}b_k(r).
\tag{N8.16}
\]

The original point-source problem requires control of this function together with the stable-field terms below. Formula (N8.14) makes the remaining computation concrete: it is a localized Gaussian expectation with specified response and score derivatives, followed by a curvature Hessian.

### 6. The complete mean coefficient includes stable feedback

For the reanchored mean phase map, denote the classical blocks by
\(A_k^0=I,B_k^0=0,C_k^0,D_k^0\). Let \(A_k^1,B_k^1\) be the critical blocks supplied by (N8.14). Let \(S_k^0\) be the classical forward graph for the actual seed family:

\[
S_0^0=0,\qquad
S_{k+1}^0=C_k^0+D_k^0S_k^0.
\tag{N8.17}
\]

It is uniformly bounded because \(D_k^0\) contracts after the fixed blocking. The actual graph differs from it by a stable convolution of the full-norm quantum error. With \(\varepsilon_k=Cg_kr_{\chi,k}\), the slow variation of the coupling gives \(\|S_k-S_k^0\|\le C\varepsilon_k\). Consequently the forward critical matrix has the expansion

\[
E_k^{\rm f}
=I+g_k^2G_k^{\rm f}
+O(g_k^4+g_k^2\varepsilon_k),
\qquad
G_k^{\rm f}=A_k^1+B_k^1S_k^0.
\tag{N8.18}
\]

Both displayed errors are summable on the AF ultraviolet segment. It is not valid to test only \(A_k^1\) and omit \(B_k^1S_k^0\). Reanchoring a point family can produce a bounded classical lattice remainder even though a representative at one fixed physical fine root reproduces classically exactly.

There is an exact first-order relation with the backward coordinate used in S8.6. Define

\[
V_k^1=B_k^1+V_{k+1}^1D_k^0,
\qquad V_K^1=0,
\qquad
G_k^{\rm b}=A_k^1+V_{k+1}^1C_k^0.
\tag{N8.19}
\]

Then \(V_k^1\) is uniformly bounded. The backward stable convolution, the full-norm error \(O(\varepsilon_k)\), and \(g_{k+1}^2-g_k^2=O(g_k^4)\) give
\(V_k=g_k^2V_k^1+O(g_k^4+g_k^2\varepsilon_k)\) and
\(E_k^{\rm b}=I+g_k^2G_k^{\rm b}+O(g_k^4+g_k^2\varepsilon_k)\).
Put \(R_k=V_k^1S_k^0\). Multiplication of (N8.17) and (N8.19) gives

\[
\boxed{
G_k^{\rm f}-G_k^{\rm b}=R_k-R_{k+1}.
}
\tag{N8.20}
\]

This is a bounded **mean-coordinate** coboundary. It explains why a continuum matching theorem may use either critical coordinate after an explicitly controlled change. It is not the missing pointwise phase identity: the latter involves the complete phase-dependent functional on every root.

There is no uncontrolled endpoint in this particular coordinate change. The chosen initial and terminal graphs give \(R_0=R_K=0\). Put \(t_k=g_k^2\) and \(U_k=I-t_kR_k\). At a sufficiently weak endpoint these matrices and their inverses are bounded, and

\[
U_{k+1}E_k^{\rm b}U_k^{-1}
=E_k^{\rm f}+O(t_k^2+t_k\varepsilon_k).
\tag{N8.20a}
\]

This follows by multiplication, (N8.20), and \(t_{k+1}-t_k=O(t_k^2)\). Thus a verified dissipative mean generator in one of these coordinates can be transferred to the other with a uniformly equivalent metric and a summable error. This statement concerns the mean matrices; it is not a replacement for SP37 in the original pointwise problem.

### 7. Gaussian source derivatives and the determinant strategy

#### 7.1 Exact finite-dimensional identities

The local source identity itself is exact. For a frozen regular integral with local action source \(\lambda h\),

\[
\left.\partial_\lambda\log
\int_D e^{-H(A)+\lambda h(A)}\,dA\right|_{\lambda=0}
=\frac{\int_D h(A)e^{-H(A)}\,dA}{\int_D e^{-H(A)}\,dA}.
\tag{N8.21}
\]

A source-dependent minimizer is a change of variables in this identity, not permission to omit its response or its Jacobian. The counterterm numbers and running couplings remain fixed.

For an untruncated Gaussian on a fixed Euclidean space, with positive precision \(M(\lambda)\),

\[
\partial_\lambda\log Z_{\rm G}(\lambda)
=-\frac12\operatorname{Tr}
\bigl(M(\lambda)^{-1}\partial_\lambda M(\lambda)\bigr).
\tag{N8.22}
\]

If a chosen coordinate chart has a source-dependent volume factor \(J(\lambda)\), its additional term is \(\partial_\lambda\log J\). It must be included before identifying the derivative with an observable.

Split the fluctuation coordinates into fine and retained coordinates and write the precision as

\[
M(\lambda)=
\begin{pmatrix}A(\lambda)&B(\lambda)\\
B(\lambda)^*&D(\lambda)\end{pmatrix},
\qquad
S(\lambda)=D(\lambda)-B(\lambda)^*A(\lambda)^{-1}B(\lambda).
\tag{N8.23}
\]

Gaussian elimination proves, exactly,

\[
\det M=\det A\det S,
\qquad
\operatorname{Tr}(M^{-1}M')
=\operatorname{Tr}(A^{-1}A')+
  \operatorname{Tr}(S^{-1}S').
\tag{N8.24}
\]

Iterating this identity telescopes local-source derivatives of Gaussian logarithms through nested linear constraints. The equality includes the derivative of the Schur complement, rather than only the direct derivative of its \(D\) block.

For the actual fixed cutoff one instead has

\[
\log Z_D(\lambda)
=\log Z_{\rm G}(\lambda)
 +\log\Pr_{M(\lambda)^{-1}}(A\in D).
\tag{N8.25}
\]

The last derivative is the cutoff score. Truncation is not removed by a determinant identity. It is a separate localized rare term only when the corresponding source cutoff estimate has been verified.

#### 7.2 What is still needed to turn the identities into a point corrector

The identities above suggest a specific actual-kernel construction. Represent the local Wilson source (N8.2) as a perturbation of the constrained quadratic precision and the minimizing chart. Prove that its first-amplitude coefficient (N8.14), including the old-action and chart scores, agrees with the derivative of the complete constrained Gaussian logarithm. Then use the nested Schur identities to isolate the difference between two blocking origins as a retained-mode endpoint.

That program has two further mathematical steps. The nonlinear source-dependent constraint chart must satisfy the corresponding determinant/volume factorization, and the endpoint must have a uniform local curvature-jet bound as the fine mesh tends to zero. The elementary identity (N8.24) alone proves neither. In particular, a trace with a local plaquette source can contain coincident propagator derivatives; smoothness of a formal retained-mode difference must be established in the source norm before claiming a mesh-independent bound.

If the resulting complete phase coefficient satisfies

\[
b_k^{\rm eff}(x)-\bar B_k
=H_k(x)-(P_L^*H_{k+1})(x),
\qquad
\sup_{k,x}\bigl(\|H_k(x)\|+\operatorname{Lip}H_k\bigr)<\infty,
\tag{N8.26}
\]

then the weighted running-coupling version follows by Abel summation. Since \(g_{k+1}^2-g_k^2=O(g_k^4)\), the first-order corrected identity has an \(O(g_k^4)\) residual, plus the explicitly retained cutoff and finite-volume terms. Higher-order corrections or channel estimates may still be required to pay matrix conjugation and satisfy SP37. The statement (N8.26) for the actual coefficient is the remaining source theorem, not a consequence of its phase average being zero.

### 8. How the averaged route changes the required theorem

The companion S8-A proves an exact exit criterion for the **original** positive chain by averaging complete covariances over microscopic translations. It introduces no new conditional random phase, and requires translation invariance only of the initial law. The phase-digit lemma above supplies the independent representation for the deterministic bulk benchmark.

The backward-adjoint phase moment theorem S8-B is correct with Euclidean norm on its finite critical coordinates and any equivalent final norm. It needs the summability condition

\[
\sum_{k<K}g_k^4
\|P_{K,k+1}\|^2\|P_{K,k}^{-1}\|^2<\infty
\quad\hbox{uniformly in }K.
\tag{N8.27}
\]

A single **phasewise invariant** scalar channel satisfies this condition. A full matrix system need not: S8.15–S8.16 give an exact two-channel example with divergence at spectral spread \(\tfrac12\). The scalar nature of the microscopic Wilson trace does not itself establish phasewise invariance, as explained in §1.

Theorem S8-C gives a more useful alternative for one scalar seed. If the full mean critical matrices admit uniformly equivalent Hermitian metrics such that

\[
E_k^*H_{k+1}E_k\le (1+e_k)H_k,
\qquad cI\le H_k\le CI,
\qquad \sum_k e_k<\infty,
\tag{N8.27a}
\]

then the independent-digit field has a uniformly bounded second moment whenever its initial norm is bounded. The noise costs only \(\sum_k g_k^4\). The stable space can remain Banach; orthogonality is used only in the finite critical coordinate. Its proof includes recovery of the stable norm by a geometric convolution. Section 9 below supplies the bounded **mean scalar normalization** needed for the actual scalar seed. It does not supply (N8.27a) on the anisotropic directions reached by phase noise.

A useful further route is a verified dissipative one-loop generator in a fixed invariant metric, with a summably small remainder and a compatible scalar normalization. The continuum calculation of Ferretti, Heise, and Zarembo, hep-th/0404187, uses canonical \(F=dA+ig[A,A]\), \(O_{\rm ren}=ZO_{\rm bare}\), and gives the dimension-four scalar/pseudoscalar, stress, and Weyl anomalous coefficients in its equations (6)–(7) and preceding paragraph. These are a concrete guide for the sign computation. Their identification with \(G_k^{\rm f}\) or \(G_k^{\rm b}\) in this frozen lattice scheme still requires matching the field convention, the actual stable feedback, the finite blocking prescription, and the cutoff terms. A continuum anomalous dimension is not by itself that matching theorem.

The exact current targets are therefore alternatives:

1. Prove the actual pointwise identity (N8.26), its residual estimate, and its original microscopic endpoint condition.
2. Verify the complete bulk mean critical matrix well enough to meet S8-B or S8-C, then use the original-kernel averaged exit. Control regular forcing by the deterministic polynomial propagator, not by an unsupported independence assertion for new births.

Both routes also need the actual mixed-history and terminal estimates. The second avoids a worst-phase incoming norm, but does not make those other obligations disappear.

### 9. Mean scalar neutrality for the actual Wilson source

This section concerns the admitted deterministic regular reference identified in A8.27–A8.41, on physical minimizing backgrounds. It uses the same Gaussian precision and the same fluctuation cutoff as the actual regular construction. The conclusion is a mean scalar statement, not a claim of phasewise scalar invariance.

#### 9.1 An exact classical scalar density embedding

Partition the microscopic roots into the nested current cells \(B_k(z)\). Define the dimensionless intrinsic density

\[
\rho_k(z;U)=\sum_{x\in B_k(z)}a^4q_W(x;U).
\qquad
\sum_z\rho_k(z;U)=2S(U).
\tag{N8.28}
\]

The incident plaquette stencils add only one microscopic layer to each cell. On the normalized current \(C^{1,\beta}\) domain, each summand is \(O(\xi_k^4)\), where \(\xi_k=a/h_k\), and each cell has \(\xi_k^{-4}\) roots. Thus the density has a uniformly bounded intrinsic norm and bounded current support. Its curvature coefficient \(e_W=\Pi\rho_k\) is independent of \(k\). Normalize this vector once if a unit scalar coefficient is preferred.

Use centered representatives of the \(L^4\) phases, consistent with the source's odd block size. The mean classical density operation merely regroups the same original fine links:

\[
\overline L_k^0\rho_k=\rho_{k+1}.
\tag{N8.29}
\]

Indeed \(\overline L_k^0=L^{-4}\sum_r L^4T_{0,k}T_r=\sum_rT_{0,k}T_r\), and the cells indexed by \(Lz+r\) partition \(B_{k+1}(z)\). This is an exact identity of this particular density embedding. It does not assert exact reproduction of every localized tensor representative.

Choose the scalar column of the critical embedding to be \(\rho_k\). In these mean coordinates \(C_k^0e_W=0\), and consequently \(S_k^0e_W=0\). Replacing another admitted scalar representative by this one changes it by a uniformly bounded stable field. At \(k=0\), \(\rho_0\) is the actual dimensionless microscopic Wilson seed. No change of microscopic observable is made.

#### 9.2 The Wilson Hessian is not the full gauge-fixed precision

Let \(\mathcal A\) be the precise Wilson functional multiplying the inverse coupling in the frozen source integral. Keep the fixed convention factor \(c_W\) defined by \(2S=c_W\mathcal A\). This handles the normalized trace used in the source without silently changing the coupling convention.

At a physical minimizing background, write the current constrained fluctuation in independent coordinates \(a\). The curve \(\mathcal U(\tau a)\) stays on the same next-scale constraint manifold. Constrained stationarity and the full constraint Hessian give

\[
\left.\partial_\tau\mathcal A(\mathcal U(\tau a))\right|_0=0,
\qquad
\left.\partial_\tau^2\mathcal A(\mathcal U(\tau a))\right|_0
=a^{\mathsf T}M_W a.
\tag{N8.30}
\]

The nonlinear constraint correction is essential. It is included in CMP102 (78)–(81), (141)–(142), and in the current-step expansion CMP109 (2.6)–(2.11). The Gaussian precision in that last source also contains the quadratic exponential gauge-fixing term from (2.5). Consequently the correct identity is

\[
M=M_W+T^{\mathsf T}\mathcal K T,
\tag{N8.31}
\]

not \(M=M_W\). Here \(T\) is the derivative of the averaged contour-gauge variables, and \(\mathcal K\) is their fixed positive quadratic form.

For completeness the gauge factor can be removed from equipartition without changing the integral. There is one residual gauge variable at each nonroot current site. Let \(K\) be its infinitesimal action in the independent constrained coordinates, with sign chosen so that

\[
TK=I,\qquad M_WK=0.
\tag{N8.32}
\]

The first equality follows directly from endpoint covariance of the averaged contour variable \(U(y,x)\): with the coarse-root gauge fixed and \(U(y,x)=1\), its derivative along a residual gauge transformation is the site gauge parameter, up to this sign. There is one averaged contour variable per site, not one independent variable for every path in its average. The blocked constraint is preserved because the gauge transformation equals the identity at its endpoints. The second equality follows by differentiating gauge invariance on the constraint manifold at its critical point. It would generally be false for an unconstrained Hessian with its constraint correction omitted.

Both maps are uniformly local in current units. The contours stay in a current block, and the source elimination of dependent bonds uses a fixed current-block pivot. Pulling \(T\) and \(K\) through that elimination costs only fixed powers of \(L\), with no power of the original fine mesh. The pair has been independently checked against CMP109 (0.11), (0.15)–(0.16), (2.3)–(2.5), and the elimination preceding (2.12).

Define \(P=I-KT\). On the real physical section, (N8.31)–(N8.32) give

\[
P^2=P,\qquad
\operatorname{Tr}P=n-n_{\rm gauge},\qquad
P^{\mathsf T}M=M_W.
\tag{N8.33}
\]

The transpose is the real adjoint, continued bilinearly when taking analytic derivatives. No assertion of physical stationarity for arbitrary independent \(J\) is needed.

#### 9.3 The remaining term is a normalized local cutoff flux

For the actual fixed Gaussian domain \(D\), the divergence theorem with the vector field \(Pa\) gives

\[
\begin{aligned}
\mu_{0,U}[a^{\mathsf T}M_Wa]
&=n-n_{\rm gauge}-\mathcal B_P(U),\\
\mathcal B_P(U)
&=\frac{1}{Z_D(U)}
\int_{\partial D}(Pa\cdot n_D)
\exp[-a^{\mathsf T}M(U)a/2]\,d\sigma(a).
\end{aligned}
\tag{N8.34}
\]

For smooth cutoffs use the corresponding expression with one differentiated cutoff. This identity retains the normalization and all gauge directions. An uncut equipartition identity is not being applied to a truncated measure.

The generalized flux estimate A8.47–A8.49 applies: \(P\) is a bounded local, background-analytic linear map, so the flux has one local boundary factor and a bounded local linear insertion. Its connected density expansion has the same Gaussian tail as A8.45. After density reassignment to current output roots and physical curvature extraction, for any fixed \(Q\),

\[
\|\Pi_\infty\mathbf B_{P,k}\|
\le C_Qx_k^{-Q}.
\tag{N8.35}
\]

The bold symbol denotes the local density representation of the global flux; its sum is \(\mathcal B_P\). The multiplicity of the output density cells is included in this representation. Background derivatives of \(P\) and \(M\) add only fixed local polynomial factors. No lower bound on an extensive global partition function is used.

Now sum the insertion densities before differentiating the amplitude. By (N8.28)–(N8.30), their total first amplitude derivative is zero, and their second derivative is \(c_Wa^{\mathsf T}M_Wa\). Therefore the complete score term in (N8.14) vanishes for this total insertion. This includes the old-action score and the measure/Jacobian scores, rather than discarding either. The remaining Gaussian term is (N8.34). Its dimension term has zero curvature coefficient.

Apply the source's full covariant action-density projection \(\Pi_\infty\), as in A8 §3, to this identity of extensive physical functions. Its coefficient is the coefficient per current cell; no statement that every separate polymer coefficient vanishes is used. Reflection covariance excludes the pseudoscalar total-derivative channel. The local invariant scalar coefficient is therefore identified by this full action projection. In the exact scalar embedding of §9.1, this proves

\[
G_k^{\rm f}e_W
=-\frac{c_W}{2}\Pi_\infty\mathbf B_{P,k},
\qquad
\|G_k^{\rm f}e_W\|\le C_Qx_k^{-Q}.
\tag{N8.36}
\]

The factor \(1/2\) is the amplitude Taylor factor in (N8.14). The physical curvature projection agrees with the independent-current projection on the affine plateau by A8 §3.1. Compatible finite-volume coefficients carry the additional wrapping/annulus family from A8 §3.2 and (N8.3)–(N8.4). This proof does not identify the physical current with zero throughout a cutoff annulus.

#### 9.4 What this proves for the scalar normalization

Full lattice reflection and axis-permutation covariance leave a unique scalar curvature bilinear, the trace on the six two-form coordinates. Hence the covariant whole-lattice **mean** critical system preserves this scalar line. Combining (N8.18) with (N8.36) gives its actual one-step factor

\[
E_k^{\rm f}e_W=e_k^W e_W,\qquad
e_k^W=1+O\!\left(
g_k^4+g_k^3r_{\chi,k}+x_k^{-Q}
\right).
\tag{N8.37}
\]

The mean stable graph was not set to zero in this conclusion: its quantum deviation is exactly the \(O(g_kr_{\chi,k})\) term already retained in (N8.18). Only this chosen scalar embedding has zero **classical** mean descendant. Finite-volume wrapping corrections remain separate and obey their weighted tail estimate.

The AF comparison and fixed polylogarithmic cutoff make every term on the right of (N8.37) summable, uniformly in the ultraviolet horizon. At a sufficiently weak fixed endpoint the factors are nonzero, and

\[
Z^W_{j,k}:=\prod_{\ell=j}^{k-1}(e_\ell^W)^{-1},
\qquad
0<c\le |Z^W_{j,k}|\le C<\infty.
\tag{N8.38}
\]

This is one deterministic, bounded scalar **mean** normalization for the actual Wilson seed in the identified regular reference. It supplies the bounded initial scalar normalization required in the proposed application of S8-C. The original point field still creates anisotropic marginal components under individual phase maps; (N8.38) does not estimate those components.

#### 9.5 Why positivity alone does not finish the matrix step

The remaining matrix estimate cannot be inferred solely from positivity of conditional expectation. Curvature extraction follows vacuum subtraction, and is not a positivity-preserving operation. For example, on a small real interval let \(Y\mid u\) be Gaussian with variance \(1-\epsilon u^2>0\). The positive observable \(Y^2\) has conditional mean \(1-\epsilon u^2\); after subtracting its vacuum value, its quadratic coefficient is negative. This finite-dimensional example is not a Yang–Mills kernel. It shows why a positive kernel alone supplies no positive-cone statement for its projected curvature map.

A Kraus-type or dissipative representation for the actual score-complete operator (N8.14) would require an additional identity. None is asserted here. The precise remaining scalar S2 calculation is to prove (N8.27a) on the phase-accessible marginal channels, with the actual coefficient (N8.18), or instead complete the original pointwise corrector and endpoint theorem (N8.26), SP37.

### 10. Summary and source anchors

#### Established in this module

- The exact local Wilson-source geometry, with the existing normalization (N8.1–N8.2).
- The same-volume smooth cutoff projection comparison and its weighted scale sum (N8.3–N8.4).
- The precise nearby-root endpoint lemma and its limitation (N8.5–N8.7).
- The exact independent-digit realization of a covariant original bulk sequence (N8.8–N8.12).
- Exact amplitude parity, the explicit score-complete first coefficient, and a uniform \(O(g^4)\) finite-jet remainder on the admitted class (N8.13–N8.16).
- The complete mean stable-feedback coefficient and its forward/backward coordinate coboundary (N8.17–N8.20).
- The normalized local-source identity and Gaussian Schur-complement derivative identities, with the cutoff score retained (N8.21–N8.25).
- Exact classical block-sum embedding of the actual Wilson scalar; the physical constrained Hessian and residual-gauge factorization; the normalized local cutoff-flux Ward identity; and bounded mean scalar normalization (N8.28–N8.38).
- Verification of S8-A, S8-B, and S8-C, including the product order, stable norm recovery, the matrix counterexample, and summable mean errors.
- Verification of the nonlinear first-exit estimates A8.31–A8.39, after the full critical-profile and stable-descendant corrections.

#### Not established by these results

- A uniformly bounded corrector (N8.26) for the original microscopic point family.
- A phasewise scalar invariant sector for the actual Wilson trace.
- A matched actual mean generator on the anisotropic channels with the required dissipative or spectral property. The scalar mean neutrality alone is now proved.
- The full 21-channel endpoint SP37.
- Mixed-history admission or a terminal full-law covariance theorem.

#### References used

- The source observable construction and the microscopic observable construction, for (N8.1–N8.2) and the 21-component microscopic family.
- **CMP109 (1987), 249–301**, the source integral and compatible Euclidean covariance; (0.11), (0.15)–(0.16), (1.5), and (2.3)–(2.12) for the contour gauge, constrained Wilson Hessian, and actual Gaussian precision. [DOI](https://doi.org/10.1007/BF01215223).
- **CMP102 (1985), 277–309**: (78)–(81) and (141)–(142) for the full constrained action Hessian and stationarity at a minimizing background.
- **CMP116 (1988), 1–22**, the analytic local source construction. [DOI](https://doi.org/10.1007/BF01239022).
- **CMP119 (1988), 243–285**: the fixed fluctuation cutoff, (3.25)–(3.32); action-density hats and covariance, (3.39)–(3.42); and the local curvature projection and source Ward identities, (3.48)–(3.67).
- J6–J18 and N7.40–N7.49 for normalized finite jets and the common admitted norm; SP22–SP37 for the point-phase obstruction and endpoint requirement.
- A8.27–A8.41 for the identified regular reference and its fixed-domain admission; A8.43–A8.49 for normalized Gaussian cutoff fluxes with a bounded local linear insertion.
- G. Ferretti, R. Heise, and K. Zarembo, **New Integrable Structures in Large-N QCD**, [hep-th/0404187v3](https://arxiv.org/pdf/hep-th/0404187), pp.2–5, for the explicitly stated continuum convention and dimension-four perturbative spectrum. It is used as a matching target, not as a proof of the lattice comparison.

No earlier file is silently promoted from a conditional operator theorem to a completed Yang–Mills point-normalization theorem. The new explicit coefficient (N8.14), together with its stable correction (N8.18), is the remaining calculation that distinguishes the actual model from the abstract phase counterexamples.

---
