# Shell bounds, mixing and phase transfer

Throughout, *the route* (also *the Route* or *the observable route*) is [Yang–Mills existence through observable derivatives](../observable_route.md); section, proposition and equation numbers attributed to it refer to that note.

## Part I. Source-free base, normalization, and group scope

### 1. Exact normalization

For the same set of unoriented plaquettes, let
\[
s_p=N-\operatorname{Re}\operatorname{Tr}U_p,
\quad S=\sum_p s_p,\quad A_B=S/N.
\]
The route uses the density \(\exp(-2NxS)\), so Balaban's coefficient multiplying his normalized-trace action is
\[
X_B=2N^2x,\qquad g_B^{-2}=X_B.
\]
This dictionary identifies the coefficient multiplying the action; differently named couplings are not equated without this conversion. CMP109 (0.2), printed p.252, explicitly uses normalized trace; its geometry, p.251, starts with odd \(L>11\). Fix one sufficiently large admitted odd \(L\), respecting all subsequent size requirements.

At fixed cutoff, compactness justifies differentiation of the finite integral. For \(x\)-independent lattice observables,
\[
\partial_x\log Z=-2N\langle S\rangle_x,
\quad \partial_x^m\log Z=(-2N)^m\kappa_x(S,\ldots,S),
\]
and
\[
\partial_x\langle F\rangle_x=-2N\operatorname{Cov}_x(F,S).
\]
For coupling-dependent \(F_x\), add \(\langle\partial_xF_x\rangle_x\). Also \(\partial_x=2N^2\partial_{X_B}\). These factors must be applied to imported beta coefficients and ultraviolet amplitudes.

The exact scalar plaquette density \(q_a(z)=a^{-4}\sum_{\mu<\nu}s_{p_{\mu\nu}(z)}\) satisfies \(a^4\sum_zq_a(z)=S\). A source \(j(z)\) changes the local exponent from \(-2Nx s_p\) to \(-[2Nx-j(z_p)]s_p\). Thus the scalar source shifts \(x(z)\) by \(-j(z)/(2N)\). A general tensor source is not this scalar shift. Neither identity proves uniform derivatives of the renormalized hierarchy.

### 2. Precisely scoped source-free input

LFR II, printed pp.355--356, Theorem 1 assumes that all effective couplings lie in a sufficiently small interval. Equation (0.1) is
\[
\chi_k\exp[-g_k^{-2}A(U_k)-E_-|T_\eta|]
\le\rho_k\le\exp[E_+|T_\eta|].
\]
The following page states that \(E_\pm\) are independent of \(k,T_\eta,U_k\). The lower bound retains both \(\chi_k\) and the Wilson action. The same introduction identifies physical-observable estimates as future applications. The sentence about an unpublished proof concerns the state of publication in 1989; it is not a claim about all later work.

CMP109, pp.258--259, (0.29)--(0.30), counts the remaining extensive factor at the current physical/coarse scale. CMP119, pp.262--264, separates regular, R, boundary, and scalar terms before its stability conclusion. These are compatible with the route's current-scale volume dictionary. They do not supply derivatives with respect to external observable marks.

CMP109 Theorem 1, p.259, states the small-field result for compact semisimple matrix groups. Theorem 2 on that page is stated for SU(2); the author calls this restriction superficial on p.260, while deferring its perturbative proof. An all-group trajectory and all-group marked induction still need their actual proofs. The separately named N2-F proof is not among the supplied files.

### 3. A sharp scalar shooting lemma

**Proposition B.1 (proved for the specified scalar recurrence).** Let \(\beta>0\), \(C\ge0\), \(x_*>0\) with \(x_*\ge 2C/\beta\), and suppose the maps
\[
F_k(x)=x-\beta+r_k(x),\quad k=0,\ldots,K-1,
\]
are continuous for \(x\ge x_*\), with \(|r_k(x)|\le C/x\). Then there is a trajectory \(x_{k+1}=F_k(x_k)\), \(x_K=x_*\), for which
\[
x_*+\tfrac\beta2(K-k)\le x_k\le x_*+\tfrac{3\beta}2(K-k),
\]
and
\[
|x_0-x_*-\beta K|
\le \frac{2C}{\beta}\log\left(1+\frac{\beta K}{2x_*}\right).
\]

**Proof.** Given a target \(u\ge x_*\), evaluate \(F_k\) at \(u+\beta/2\) and \(u+3\beta/2\). The first value is at most \(u\) and the second at least \(u\). The intermediate value theorem gives a preimage in that interval. Repeat backwards. The interval bounds follow by summing. Summing the recurrence gives \(x_0=x_*+\beta K-\sum_{k=0}^{K-1}r_k(x_k)\). Bound the last sum by
\[
C\sum_{j=1}^K\frac1{x_*+\beta j/2}
\le\frac{2C}{\beta}\log\left(1+\frac{\beta K}{2x_*}\right).
\]
This proves the claim.

If in addition \(|r'_k(x)|\le C_1/x^2\) and \(C_1/x_*^2\le1/2\), the preimages are unique and the derivative of the terminal coupling along this scalar flow obeys
\[
\exp\left[-\frac{4C_1}{\beta x_*}\right]
\le\frac{\partial x_K}{\partial x_0}
\le\exp\left[\frac{4C_1}{\beta x_*}\right].
\]
Indeed this derivative is \(\prod_k[1+r'_k(x_k)]\), \(|\log(1+u)|\le2|u|\) for \(|u|\le1/2\), and \(\sum_kx_k^{-2}\le2/(\beta x_*)\).

With \(\beta=b\log L\) and \(a=L^{-K}\ell_0\), the first conclusion is \(x_0=b\log(\ell_0/a)+O(\log\log(\ell_0/a))\). This closes the elementary shooting part *if* the actual recurrence and its uniform remainder are proved. Real Balaban flows may have history-dependent irrelevant coordinates; the displayed memory-free scalar maps cannot be substituted for those dynamics without a reduction theorem. The derivative hypothesis is an additional estimate; \(|r_k|\le C/x\) alone does not imply it.

### 4. Group-independent low-dimensional field algebra

For a compact simple Lie algebra, every invariant linear functional is zero and invariant symmetric bilinear forms form a one-dimensional space. A covariant derivative has engineering dimension 1 and curvature has dimension 2. Consequently an invariant polynomial of positive dimension at most 4 contains either one covariantly differentiated curvature, which has zero invariant linear contraction, or exactly two undifferentiated curvatures. The positive-dimensional field space is therefore
\[
Q_{AB}=B(F_A,F_B),\qquad A,B\in\{12,13,14,23,24,34\},\quad Q_{AB}=Q_{BA},
\]
with 21 spacetime components. Add the identity as a mixing direction. No linear relation is lost when the color dimension is less than 6: configurations \(F_A=v_A X\) produce the rank-one matrices \(B(X,X)vv^T\), and rank-one symmetric matrices span all of \(\operatorname{Sym}^2\mathbb R^6\). Differential Bianchi identities impose no further pointwise linear relation of this kind.

Under SO(4), the decomposition \(\Lambda^2=\Lambda^2_+\oplus\Lambda^2_-\) gives
\[
\operatorname{Sym}^2\Lambda^2=(1\oplus5)\oplus(1\oplus5)\oplus9.
\]
An orientation-reversing transformation exchanges the two Hodge summands. The scalar, pseudoscalar, and stress-type channels contain 11 components; the remaining ten must be retained. A stress-type representation alone does not prove stress-tensor conservation or generation of translations.

### 5. Finite-cutoff positivity for any fixed compact matrix group

Let \(R\) be a finite-dimensional unitary representation of a compact group, with character \(\chi_R\), and let \(\lambda\ge0\). The class function
\[
w(g)=\exp[\lambda\operatorname{Re}\chi_R(g)]
\]
has a character expansion with nonnegative coefficients. Indeed,
\[
w(g)=\sum_{p,q\ge0}\frac{(\lambda/2)^{p+q}}{p!q!}
\chi_{R^{\otimes p}\otimes\bar R^{\otimes q}}(g),
\]
and every tensor-product character decomposes with nonnegative integral multiplicities. This series converges uniformly because \(|\chi_R|\le\dim R\).

For a reflection-compatible cut through a Wilson lattice, each crossing plaquette can be split into a path product \(u\) in one half and the reflected path product \(v\) in the other. Since
\[
\chi_\pi(uv^{-1})=\sum_{i,j}\pi(u)_{ij}\overline{\pi(v)_{ij}},
\]
the crossing weight is a convergent sum of positive reflected squares. Combining it with the two reflected half-weights and product Haar measure gives \(\langle\Theta F\,F\rangle\ge0\) for the half-lattice observable algebra. This is the algebraic content of the usual Wilson reflection-positivity proof, subject to the chosen compatible cut/torus geometry.

For any compact connected simple \(G\), choose a faithful unitary \(R\) and normalize its invariant trace form. This supplies the finite-lattice positivity input and the same 21-dimensional quadratic observable algebra. It does not transfer the marked induction, beta remainder, large-field geometry, or ultraviolet coefficients to every group. A nonfaithful representation changes the global group information and is not an innocuous replacement when the target specifies \(G\).

### B.6 Continuum perturbative convention check

With Hermitian generators satisfying \(\operatorname{Tr}(T^aT^b)=\delta^{ab}/2\), one plaquette for each \(\mu<\nu\), and the curvature evaluated at a plaquette center (or a symmetric clover prescription),
\[
N-\operatorname{ReTr}U_p=\frac{a^4}{4}\sum_a F_{\mu\nu}^a{}^2+O(a^6).
\]
Thus \(g_{\rm YM}^{-2}=Nx\) and \(x=g_t^{-2}\), where \(g_t^2=N g_{\rm YM}^2\). The conventional pure-theory one-loop beta coefficient [BB19, (3.7)] predicts, for fixed \(L\),
\[
x'=x-\frac{11}{24\pi^2}\log L+O(x^{-1}),\qquad
X'_B=X_B-\frac{11N^2}{12\pi^2}\log L+O(X_B^{-1}).
\]
This is a perturbative coefficient conversion, not a proof of the actual Balaban recurrence or its uniform remainder. At a lower plaquette corner the generic pointwise Taylor error is \(O(a^5)\); the leading dictionary is unchanged.

## Part II. S2 and M: local shells, nonlinear remainders, and all-order control

### 2. Exact centering and the full positive history law

#### Proposition 2.1: identity shifts disappear from connected orders at least two

Let the finite-cutoff field family be \(Q_{\alpha,n}\), and let \(c_{\alpha,n}\) be any deterministic numbers. For \(m\geq2\),

\[
\kappa_m(Q_{\alpha_1,n}-c_{\alpha_1,n},\ldots,Q_{\alpha_m,n}-c_{\alpha_m,n})
=\kappa_m(Q_{\alpha_1,n},\ldots,Q_{\alpha_m,n}).
\]

**Proof.** The formal logarithm of the joint moment series changes by the linear polynomial \(-\sum_i t_i c_{\alpha_i,n}\). Its degree at least two coefficients are unchanged. The argument applies directly at each finite cutoff, with no infinite-source analyticity hypothesis. QED.

This removes deterministic identity mixing from the separated connected estimate. It does **not** remove collision-subcluster counterterms, tensor-to-tensor mixing, or the need to fix the one-point normalization before forming the complete moment hierarchy.

#### Proposition 2.2: averaging conditional connected functions misses history terms

Let \(Y\) be a positive history variable, and put \(m_i(Y)=E[X_i\mid Y]\), \(c_{ij}(Y)=\operatorname{Cov}(X_i,X_j\mid Y)\). Then

\[
\operatorname{Cov}(X_1,X_2)=E[c_{12}]+\operatorname{Cov}(m_1,m_2),
\]

and

\[
\begin{aligned}
\kappa_3(X_1,X_2,X_3)
={}&E[\kappa_3(X_1,X_2,X_3\mid Y)]
+\kappa_3(m_1,m_2,m_3)\\
&+\operatorname{Cov}(m_1,c_{23})
+\operatorname{Cov}(m_2,c_{13})
+\operatorname{Cov}(m_3,c_{12}).
\end{aligned}
\]

More generally the cumulant of order \(m\) is the sum over partitions \(\pi\) of the cumulant, over the history law, of the conditional cumulants indexed by the blocks of \(\pi\).

**Proof.** Expand \(\log E_Y\exp[\log E(e^{\sum t_iX_i}\mid Y)]\) as a formal polynomial to the desired degree. The degree-two and degree-three terms give the displayed formulas. QED.

For example, let \(X_i=Z+\eta_i\), where the \(\eta_i\) are independent centered Gaussians and \(Z\) is a nondegenerate centered common variable. Conditioned on \(Z\), distinct \(X_i\) have zero covariance; unconditionally their covariance is \(\operatorname{Var}Z\). Thus excellent conditional off-diagonal estimates alone do not control the complete positive history law. The route's terminal covariance and generated response vertices cannot be omitted.

#### Proposition 2.3: the two-point shell is positive as a quadratic form

For each exact positive transport step \(Q_k\), the kernel

\[
K_k(x,y)=E\{Q_k(F_k(x)F_k(y))-Q_kF_k(x)Q_kF_k(y)\}
\]

is positive semidefinite. For every finite linear combination \(F_k(f)\), its quadratic form is \(E\operatorname{Var}(F_k(f)\mid\text{output})\geq0\). Consequently the exact telescoping decomposition is an additive positive variance budget on the diagonal:

\[
\operatorname{Var}(F_0(f))=\sum_{k<K}E\operatorname{Var}(F_k(f)\mid\text{output})+\operatorname{Var}(F_K(f)).
\]

This is useful for auditing a proposed estimate: a large positive variance contribution cannot be canceled by another shell. Positivity does not by itself yield spatial decay or a cutoff-uniform upper bound.

### 3. A new Gaussian-shell estimate retaining all tensor background chains

Work in physical units with reference length \(\ell_0=1\); units can be restored by dimensional scaling. Let the finite number of curvature components be \(d\), fixed once the compact gauge group is fixed. On a central no-wrap region (or using torus distance throughout), at shell size \(h\), let \(Y\) denote the retained data. Conditional on \(Y\), write the curvature variable as

\[
B_h^Y(x)+\xi_h^Y(x),\qquad E(\xi_h^Y\mid Y)=0,
\]

where \(\xi_h^Y\) is jointly Gaussian. Write \(K_h^Y(x,y)=E[\xi_h^Y(x)\xi_h^Y(y)^T\mid Y]\). Let \(M_i\) be real symmetric \(d\times d\) matrices with norm at most one, so the argument covers every scalar and tensor quadratic mark. Set

\[
O_i=\tfrac12(B_h^Y(x_i)+\xi_h^Y(x_i))^T M_i(B_h^Y(x_i)+\xi_h^Y(x_i)).
\]

The matrices selecting the 21 curvature bilinears have uniformly bounded norm after fixing a basis and the invariant quadratic form. A finite change of tensor basis only changes the exponential base in the following bounds.

#### Proposition 3.1: conditional cumulants with an averaged retained background

Assume

\[
\|K_h^Y(x,y)\|\leq k\gamma_h h^{-4}e^{-c|x-y|/h}
\tag{G1}
\]

on the relevant conditional Gaussian kernels, including the diagonal, and assume the positive history law satisfies

\[
E|B_h^Y(x)|^2\leq b\gamma_hh^{-4}
\tag{G2}
\]

uniformly in the points, cutoff, shell and chosen torus. Here \(\gamma_h>0\) is the covariance prefactor; in a quadratic action normalized as in the route it is proportional to the reciprocal inverse coupling, with the proportionality fixed by the action dictionary.

Let \(\mathcal T(X)\) be the length of a Euclidean minimum spanning tree joining \(x_1,\ldots,x_m\). Then for \(m\geq2\),

\[
E\big|\kappa_m(O_1,\ldots,O_m\mid Y)\big|
\leq C^m m!\,\gamma_h^m h^{-4m}e^{-c\mathcal T(X)/h},
\tag{G3}
\]

where \(C\) depends only on \(d,k,b\). In particular,

\[
E|\operatorname{Cov}(O_1,O_2\mid Y)|
\leq \big(\tfrac d2k^2+bk\big)\gamma_h^2h^{-8}e^{-c|x_1-x_2|/h}.
\tag{G4}
\]

**Proof.** The conditional cumulant is the sum of a cycle term and a path term. For distinct formal labels the cycle term is

\[
\frac1{2m}\sum_{\sigma\in S_m}
\operatorname{Tr}\!\left(M_{\sigma(1)}K_{\sigma(1),\sigma(2)}\cdots M_{\sigma(m)}K_{\sigma(m),\sigma(1)}\right),
\]

and the path term is

\[
\frac12\sum_{\sigma\in S_m}
B_{\sigma(1)}^TM_{\sigma(1)}K_{\sigma(1),\sigma(2)}M_{\sigma(2)}\cdots
K_{\sigma(m-1),\sigma(m)}M_{\sigma(m)}B_{\sigma(m)}.
\]

These follow either by completing the Gaussian square or by the exact finite-dimensional formulas in the route, §4. Every cycle or path visits every marked point and therefore has total edge length at least \(\mathcal T(X)\). A cycle has \(m\) covariance factors and is bounded by

\[
d\,k^m\gamma_h^mh^{-4m}e^{-c\mathcal T(X)/h}.
\]

A path has \(m-1\) covariance factors. Cauchy–Schwarz and (G2) give

\[
E|B_{\sigma(1)}||B_{\sigma(m)}|\leq b\gamma_hh^{-4},
\]

so its history average is bounded by

\[
b k^{m-1}\gamma_h^mh^{-4m}e^{-c\mathcal T(X)/h}.
\]

Multiplication by the permutation counts proves (G3). For \(m=2\) the exact terms are \(\tfrac12\operatorname{Tr}(M_1K_{12}M_2K_{21})\) and \(B_1^TM_1K_{12}M_2B_2\); the cycle decay is stronger, and (G4) follows. QED.

**What this adds to the observable route.** The estimate is local in the retained background and explicitly controls the tensor chains, even for a constant tensor mark. It does not depend on the scalar endpoint cancellation. A *local second moment* of the retained curvature is sufficient for all orders of the history-averaged **conditional Gaussian cumulant**, because each connected Gaussian graph contains at most two retained-background endpoints. There is no global background energy or total fluctuation dimension in the bound.

**What it does not add.** Neither (G1) on all positive histories nor (G2) for the retained interacting background is supplied by the source-free stability theorem. The transported Wilson observables are not known to remain purely quadratic. Higher generated vertices and the cumulants of history-dependent conditional means must still be estimated. Actual renormalized shell marks have their prescribed running normalization; one cannot freely divide each shell by \(\gamma_h\) without checking that normalization. If the mark carries a scalar or matrix factor \(Z_h\), the right side contains \(\|Z_h\|^m\gamma_h^m\).

#### Random-envelope variant

Suppose (G1) holds with a nonnegative history envelope \(A_h(Y)\) in place of \(k\). Set \(\beta_i=|B_h^Y(x_i)|/(\gamma_h^{1/2}h^{-2})\). It suffices, for every order \(m\geq2\), to prove

\[
EA_h^m+\max_{i\ne j}E[A_h^{m-1}\beta_i\beta_j]
\leq C_0^m(m!)^r.
\tag{G5}
\]

The same proof gives

\[
E|\kappa_m(O_1,\ldots,O_m\mid Y)|
\leq C_1^m(m!)^{1+r}\gamma_h^mh^{-4m}e^{-c\mathcal T(X)/h}.
\]

A sufficient condition for \(r=1\) is a uniform exponential moment of
\(A_h+(\beta_i^2+\beta_j^2)/2\) for each marked endpoint pair. Indeed \(A_h^{m-1}\beta_i\beta_j\) and \(A_h^m\) are bounded by that nonnegative variable to power \(m\), and the exponential moment bounds the latter by \(Cm!c^{-m}\). Such an envelope must be localized to marked carriers; taking a maximum over an entire expanding torus would generally introduce volume growth. Again, (G5) is a concrete sufficient missing estimate, not an established property of the Wilson history law.

### 4. An all-order scale-summation budget with one fixed factorial exponent

#### Proposition 4.1: geometric scale sum

Let \(h_j=L^{-j}\), \(L>1\), \(s,c>0\), \(r>0\) and \(m\geq1\). Then

\[
\sum_{j\geq0}h_j^{-sm}e^{-cr/h_j}
\leq \frac{\Gamma(sm)}{\log L}\left(\frac Lc\right)^{sm}r^{-sm}
\leq C_{s,L,c}^{m}(m!)^s r^{-sm}.
\tag{S1}
\]

**Proof.** Put \(u_j=r/h_j=rL^j\). For \(u\in[u_j,Lu_j]\),

\[
u^{sm}e^{-cu/L}\geq u_j^{sm}e^{-cu_j}.
\]

Integrating with measure \(du/u\), then summing disjoint intervals, bounds \(\sum_j u_j^{sm}e^{-cu_j}\) by

\[
(\log L)^{-1}\int_r^\infty u^{sm-1}e^{-cu/L}\,du
\leq (\log L)^{-1}(L/c)^{sm}\Gamma(sm).
\]

The final bound follows from Stirling's inequalities; their ratio is bounded by a constant to power \(m\). For the integer case \(s=4\), one may use \((4m)!\leq4^{4m}(m!)^4\), up to harmless constants. QED.

Thus, **if** an actual renormalized connected-shell decomposition has

\[
|C_{m,h}(X)|\leq A^m(m!)^p h^{-sm}e^{-c\mathcal T(X)/h},
\]

then its absolute shell sum has the route's joint off-diagonal bound with singularity exponent \(\sigma=s\) and factorial exponent \(p+s\), since \(\mathcal T(X)\geq\delta_m(X)\) for \(m\ge2\), with \(\delta_m=\min(1,\min_{i<j}|x_i-x_j|)\). A terminal term bounded by \(A^m(m!)^p\) is harmless in this estimate. In the Gaussian uniform-envelope estimate above, this would give \(\sigma=4,p_{\mathrm{final}}=5\). In the exponential-envelope variant \(r=1\), the safe final exponent is \(6\).

The existence of that shell decomposition, and the control of all its generated response terms, remain separate inputs. At orders at least three, the law of total cumulance prevents simply adding history-averaged conditional cumulants and calling the result the full cumulant.

#### Logarithms do not force an order-dependent exponent

For fixed \(b\geq0\) and \(\varepsilon>0\),

\[
(1+\log(1/h))^{bm}\leq C_{b,\varepsilon}^m h^{-\varepsilon m},\qquad0<h\leq1.
\]

This follows by maximizing \(e^{-\varepsilon t}(1+t)^b\), \(t\geq0\). Therefore the scale sum including such logarithms has fixed singularity exponent \(s+\varepsilon\) and fixed factorial exponent \(p+s+\varepsilon\). This gives an explicit budget for running normalization factors whose degree is linear in the number of marks. If the actual localization length contains logarithms, the actual decay profile must first be put into an equally summable form; the argument does not authorize deleting those logarithms from the exponent.

### 5. The exact first nonlinear remainder equation

Let \(\nu_t(dz)=Z_t^{-1}e^{-tV(z)}\nu_0(dz)\), \(0\leq t\leq1\), on a fixed integration domain. Assume all differentiations are justified, for example by integrable dominating exponential moments. For \(t\)-independent marks,

\[
\frac d{dt}\kappa_{\nu_t}(O_1,\ldots,O_m)
=-\kappa_{\nu_t}(O_1,\ldots,O_m,V).
\tag{N1}
\]

**Proof.** Differentiate the formal generating polynomial
\(\log E_{\nu_t}e^{\sum s_iO_i}\). Its derivative is minus the expectation of \(V\) in the tilted law plus the un-tilted expectation of \(V\). The mixed coefficient of positive source degree is the displayed cumulant. QED.

In particular,

\[
\operatorname{Cov}_{\nu_1}(O_x,O_y)
=\operatorname{Cov}_{\nu_0}(O_x,O_y)
-\int_0^1\kappa_{\nu_t}(O_x,O_y,V)\,dt.
\tag{N2}
\]

If \(V=\sum_ZV_Z\) is a justified local interaction decomposition, a sufficient nonlinear bound for a shell is

\[
\sum_Z\int_0^1 E_Y\left|\kappa_{\nu_{t,Y}}(O_x,O_y,V_Z)\right|dt
\leq B h^{-8}(1+\log(1/h))^b e^{-c|x-y|/h}.
\tag{N3}
\]

This isolates a concrete missing estimate for S2. A source-free smallness bound on \(V_Z\) is not identical to (N3); it needs an anchored **connected** estimate with the two physical insertions, normalized under the actual conditional laws and averaged over the full positive history lift. Higher-order versions of (N1) require the full marked hierarchy and do not close by differentiating a source-free bound without more work.

Hard small-field characteristic functions require their own comparison or boundary terms. If the reference measure is already a truncated Gaussian, the untruncated formulas of §3 cannot simply be reused. Changing cutoffs, source-dependent observables, gauge coordinates, or retained-field parametrizations contributes the corresponding explicit response terms. The route's frozen source-free transport avoids certain differentiations of a moving minimizer, but does not make its transported insertion purely quadratic.

### 6. A finite-jet majorant theorem that closes factorial growth if the renormalized step is summably small

This provides a precise sufficient induction statement for the coefficient-majorant step (M). It concerns coefficient norms; it does not impose convergence of a physical finite-source functional.

#### Proposition 6.1: summable nonlinear jet growth preserves a single factorial exponent

Let \(p\geq1\) and \(C\ge1\), and let \(u_{k,m}\geq0\) be bounds on renormalized marked coefficient norms, after canonical scaling and marginal linear mixing have been removed. Suppose

\[
u_{0,m}\leq A^m(m!)^p
\]

and, for every \(m\geq1\),

\[
u_{k+1,m}\leq u_{k,m}+
\varepsilon_k\sum_{\substack{\pi\in\Pi_m\\|\pi|\geq2}}
C^{|\pi|}|\pi|!\prod_{B\in\pi}u_{k,|B|},
\qquad\sum_k\varepsilon_k\leq E<\infty.
\tag{J1}
\]

Then there is \(A'\), depending only on \(A,C,E,p\), such that

\[
u_{k,m}\leq (A')^{m+1}(m!)^p
\tag{J2}
\]

for every scale and source degree. No dependence on the total number of RG steps appears.

**Proof.** Divide by \((m!)^{p-1}\) and use \(\prod_{B\in\pi}|B|!\leq m!\). The normalized coefficients are dominated by the derivatives of a nonnegative formal power series \(V_k(z)\) satisfying

\[
V_0(z)=\frac{Az}{1-Az},\qquad
V_{k+1}(z)=V_k(z)+\varepsilon_k\frac{C^2V_k(z)^2}{1-CV_k(z)}.
\tag{J3}
\]

The standard exponential generating-function partition identity gives exactly (J3): \(|\pi|!\) cancels the \(1/|\pi|!\) in the exponential generating function of set partitions.

Choose \(z_0>0\) small enough that \(y_0=V_0(z_0)\leq\min\{1/(4C),1/(8C^2E)\}\), omitting the second restriction when \(E=0\). If previous values are at most \(2y_0\), then \(CV_k(z_0)\leq1/2\) and

\[
V_{k+1}(z_0)\leq y_0+\sum_{j\leq k}2C^2\varepsilon_j(2y_0)^2\leq2y_0.
\]

Induction proves the bound at every scale. Positivity of coefficients gives \([z^m]V_k\leq2y_0z_0^{-m}\). Restoring the factorials proves (J2). The argument is valid for every finite source truncation, with constants independent of the truncation degree, and hence for the formal infinite hierarchy. QED.

Summable inhomogeneous additions \(f_{k,m}\) can be included when \(\sum_kf_{k,m}\leq D^m(m!)^p\): preload this upper bound into the initial positive majorant, which is valid because all the majorant maps are coefficientwise monotone.

**Required Wilson certificate.** To apply this theorem one must prove (J1) in a norm controlling joint off-diagonal kernels, the contact prescription, and the positive history average; retain all generated response vertices; identify the actual linear matrix that is removed; and prove \(\sum\varepsilon_k\leq E\) uniformly in cutoff and expanding volume. An unsummed \(O(g_k^2)\) loss does not satisfy this input. A demonstrated \(O(g_k^4)\) loss may, using the verified trajectory. Neither the source-free density theorem nor the formal jet partition identity proves (J1).

## Part III. Locality, positivity, mixing, and rotation restoration

### L.1 A shrinking collision strip can be controlled directly

**Proposition L.1 (P).** Let a finite family of actual lattice fields satisfy
\[
\sup_{\alpha,x,U}|\Phi_{n,\alpha}(x;U)|\le K a_n^{-D},\qquad 0<a_n\le1,
\]
with fixed \(K,D\) independent of volume. Let \(0<\eta<1\), \(w_n=a_n^\eta\), and use the *uncapped* separation
\[
r_m(X)=\min_{i<j}|x_i-x_j|.
\]
On a central coordinate lift where torus and Euclidean distances agree, let \(|\chi_n(X)|\le1\). For \(m\ge2\), define the actual full-moment contribution
\[
E_{m,n}(F)=a_n^{4m}\sum_X\chi_n(X)\mathbf1_{\{r_m(X)\le w_n\}}
S^{\rm raw}_{m,n}(X)F(X).
\]
For every fixed integer \(q>\max\{4,D/\eta+2\}\),
\[
|E_{m,n}(F)|\le C^{m+1}a_n^\eta\nu_{qm}(F),
\qquad F\in\mathcal S_0(\mathbb R^{4m}),                     \tag{L1}
\]
with no factorial loss. The analogous integral statement also holds.

**Proof.** Probability normalization and the deterministic field bound give \(|S^{\rm raw}_{m,n}|\le K^m a_n^{-Dm}\). For a noncollision point in the strip, project a nearest pair to its midpoint. The resulting \(Y\) lies on \(\Delta_m\), and \(V=X-Y\) satisfies
\[
\|V\|_1\le2r_m(X),\quad |V|^2=r_m(X)^2/2,\quad Y\perp V.
\]
The midpoint need not be a lattice site: it is used only to evaluate the continuum test function. Put \(j_m=\lceil Dm/\eta\rceil+1\le qm\). Taylor expansion from \(Y\), where every derivative vanishes, gives
\[
|F(X)|\le\frac{(2r_m(X))^{j_m}}{j_m!}
(3/2)^{qm/2}\nu_{qm}(F)(1+|X|^2)^{-qm/2}.
\]
Here the ratio of the weight at \(X\) to the weight along \(Y+tV\) is at most \(3/2\), because \(r_m\le1\). On the strip,
\[
a_n^{-Dm}r_m(X)^{j_m}\le a_n^{\eta j_m-Dm}\le a_n^\eta.
\]
The remaining Taylor factors are at most an exponential in \(m\). Finally,
\[
a_n^{4m}\sum_X(1+|X|^2)^{-qm/2}
\le\left[a_n^4\sum_{x\in a_n\mathbb Z^4}(1+|x|^2)^{-q/2}\right]^m
\le C_q^m.
\]
Exact collisions contribute zero. No union bound over pairs or derivatives of the strip indicator are needed. QED.

**Consequence (P as an implication).** It is enough to prove the route's joint kernel bound on \(\delta_m(X)>a_n^\eta\), together with the deterministic polynomial bound on each actual renormalized field. The omitted strip gives (L1); the route's proof handles the complement. Thus the external coincidence-flat reconstruction need not wait for a distributional extension of every product onto all collision diagonals.

Compactness of SU(N) gives \(\|F_a^{\rm clover}\|_\infty\le Ca^{-2}\), hence \(\|Q_a^{\rm clover}\|_\infty\le Ca^{-4}\). If the finite field-mixing matrix has norm at most \(Ca^{-z}\) and the identity subtraction at most \(Ca^{-(4+z)}\), L.1 applies with \(D=4+z\). Fixed logarithmic growth can be absorbed into an arbitrarily small extra power. **The existence and polynomial growth of the correctly normalized mixing are still O.** Internal collision subtractions may remain necessary to prove the marked kernel estimate; L.1 only simplifies the external reconstruction interface.

**Ultraviolet rescaling qualification.** This lemma immediately controls the limit \(a\to0\) at *fixed* physical smearing scale \(\rho\). It is not an automatic joint-limit bound. For \(F_\rho(X)=\rho^{-4m}F((X-x_*)/\rho)\) and \(a^\eta\le\rho\le1\), the same proof in scaled variables gives
\[
|E_{m,a}(F_\rho)|\le C^{m+1}a^\eta\rho^{-j_m}\nu_{qm}(F).
\]
Any ultraviolet normalization multiplies this error too. The route's continuum-first order of limits avoids an unjustified uniformity claim.

### L.2 A general quantitative contact-stencil criterion

Suppose
\[
E_{m,n}(F)=\sum_{|\alpha|\le dm}\int\partial^\alpha F(X)\,d\mu_{\alpha,m,n}(X),
\]
where all measures are supported within Euclidean distance \(w_n\le1\) of \(\Delta_m\), and
\[
\sum_\alpha\int(1+|X|^2)^{-tm/2}
\,d|\mu_{\alpha,m,n}|(X)
\le C^{m+1}(m!)^p w_n^{-\lambda m}.
\]
For a fixed \(q>\max\{t,d+\lambda+2\}\), Taylor expansion of \(\partial^\alpha F\) to order \(\lceil\lambda m\rceil+1\) gives
\[
|E_{m,n}(F)|\le C_1^{m+1}(m!)^p w_n\nu_{qm}(F).       \tag{L2}
\]
The distance in this version is the distance in \(\mathbb R^{4m}\): it equals the nearest-pair distance divided by \(\sqrt2\). Thus \(\|V\|_1\le\sqrt8 w_n\) and the weight ratio is at most 2. These change only the exponential constant. The assumed total-variation sum already includes all derivative indices.

Shrinking support without a coefficient bound is insufficient. A compactly supported smooth test equal near the origin to \(\exp[-1/|x-y|^2]\), extended by zero at \(x=y\), is flat. Nevertheless
\[
e^{2/a^2}F(0,ae_1)=e^{1/a^2}
\]
diverges for small \(a\). The quantitative coefficient hypothesis in (L2) cannot be omitted.

### L.3 Reflection positivity on the correct test domain

Use full moments of actual local lattice fields with real mixing that commutes with the geometric tensor reflection. If the stencil radius tends to zero, a polynomial whose support has a fixed positive distance from the reflection plane belongs to the lattice positive-time algebra eventually. Its reflected quadratic form is nonnegative by Wilson reflection positivity.

For reconstruction, start with compact smooth kernels supported in
\[
0<t_1<t_2<\cdots<t_m,
\]
with fixed positive time gaps. Reflect and reverse one ordered kernel and concatenate it with another. The result belongs to the coincidence-flat space. Such compact, separated kernels are dense in the ordered Schwartz domain: smooth cutoffs remove small time gaps and large distances; flatness on the boundary and rapid decay give convergence in every fixed seminorm. The common OS bound therefore extends positivity to the full ordered algebra.

For the expanding-torus embedding used in this argument, choose a real reflection-compatible *product* cutoff tending to one on compact sets, supported in a central cube of coordinate diameter at most \(T_n/2\). L.1 itself permits any bounded cutoff, but an arbitrary joint cutoff need not preserve the finite-cutoff moment interpretation or positivity. Discarding the collision strip affects each limiting reflection form by a vanishing error; this does not assert positivity of the separately truncated finite-cutoff hierarchy.

### R.1 The 21 fields have seven hypercubic mixing channels

Let \(V=\mathbb R^4\), \(W=\operatorname{Sym}^2(\Lambda^2V)\), and let \(H_4\) be the full group of signed coordinate permutations, including reflections. Write \(Q_{ij,kl}=Q_{kl,ij}\), antisymmetric in each pair.

**Proposition R.1 (P).** The restriction of \(W\) to \(H_4\) is multiplicity-free, with irreducible real dimensions
\[
1+3+2+6+6+1+2=21.                                    \tag{R1}
\]
An equivariant mixing matrix therefore has seven scalar coefficients. Only the trivial scalar channel can mix with the identity.

**Explicit projectors and proof.** Divide the coordinates into three invariant groups.

**Diagonal pairs, dimension 6.** Put \(d_{ij}=Q_{ij,ij}\),
\[
s=\frac16\sum_{i<j}d_{ij},\qquad
r_i=\sum_{j\ne i}d_{ij}-3s,\qquad\sum_i r_i=0.
\]
The scalar projector gives \(d^s_{ij}=s\). The three-dimensional projector gives \(d^R_{ij}=(r_i+r_j)/2\). The remaining two-dimensional part \(d^W=d-d^s-d^R\) has all row sums zero, equivalently
\[
d^W_{12}=d^W_{34},\quad d^W_{13}=d^W_{24},\quad d^W_{14}=d^W_{23},
\qquad d^W_{12}+d^W_{13}+d^W_{14}=0.
\]

**Pairs sharing one index, dimension 12.** For \(i\ne j\) and complementary indices \(\{k,l\}\), write
\[
u_{ij}^{(k)}=Q_{ik,jk},\qquad u_{ij}^{(l)}=Q_{il,jl}.
\]
Their sums give a six-dimensional off-diagonal Ricci-type channel. Their differences give another six-dimensional channel.

**Disjoint pairs, dimension 3.** Define
\[
v=(Q_{12,34},-Q_{13,24},Q_{14,23}).
\]
The common mean is the pseudoscalar channel; the sum-zero remainder has dimension two.

Independent sign flips act on these three groups respectively by the trivial character, by the six distinct characters \(s_i s_j\), and by \(s_1s_2s_3s_4\). The groups therefore cannot mix. The permutation representations in the first group are the trivial, standard three-dimensional, and matching two-dimensional representations of \(S_4\). The third group's matching representation is twisted by determinant. For each middle-group pair character, the complementary-index transposition exchanges the two basis vectors. Its sum and difference are inequivalent stabilizer characters; permutations transport each through all six pair characters. These give two irreducible inequivalent induced six-dimensional spaces. This proves multiplicity-freeness and (R1). QED.

Independent exact enumeration of the 384 signed permutations confirms
\[
\langle\chi_W,1\rangle=1,\quad
\langle\chi_W,\det\rangle=1,\quad
\langle\chi_W,\chi_W\rangle=7.
\]
This finite arithmetic check supports the algebraic proof; it is not evidence for an interacting estimate.

Under \(O(4)\), the channels assemble into scalar 1, pseudoscalar 1, stress-type \(3+6=9\), and Weyl-type \(2+6+2=10\). An \(O(4)\)-equivariant endomorphism has four coefficients: its two stress-type coefficients agree and its three Weyl-type coefficients agree in these projector conventions. The actual lattice mixing coefficients are not asserted to satisfy these relations without renormalization and rotation restoration.

In particular, the only reflection-even hypercubic invariant quadratic-curvature scalar action is proportional to \(\sum_{i<j}Q_{ij,ij}\). Sign flips kill off-diagonal entries and permutations equalize the diagonals. There is no second dimension-four anisotropic scalar action counterterm in this class. This does not collapse the seven tensor-observable channels to one.

### R.2 A useful selection rule for a correctly defined angular defect

**Proposition R.2 (P).**
\[
\operatorname{Hom}_{H_4}(\Lambda^2V,\operatorname{Sym}^2\Lambda^2V)=0. \tag{R2}
\]

**Proof.** For an equivariant map \(T\), sign flips force \(T(e_i\wedge e_j)\) into
\(\operatorname{span}\{Q_{ik,jk},Q_{il,jl}\}\), where \(\{k,l\}\) is complementary. The transposition \(i\leftrightarrow j\) negates \(e_i\wedge e_j\) but fixes both target vectors, by symmetry under exchange of the two curvature pairs. Thus both coefficients vanish. The two-form representation also has no invariant vector. QED.

Consequently, **if** an exact angular Ward identity yields a translation-covariant, gauge-invariant, local dimension-six field \(D_{\mu\nu,a}\) transforming as \(\Lambda^2V\) under the full \(H_4\), and the renormalization prescription respects that transformation law, it has no identity or dimension-four \(Q\) mixing channel away from external-insertion contacts. Dimension-five \(FDF\) terms are excluded by central inversion: they are odd, while a two-form is even. Lower positive-dimensional invariant polynomials vanish for a simple Lie algebra.

The hypothesis is essential. A schematic scalar dimension-six artifact is not automatically such an angular field. One must derive the exact defect identity, separate orbital total derivatives, boundaries and contacts, and prove the actual-history bound on its insertion. The selection rule does not bound that insertion.

For example, if
\[
A_{6,a}=A_{6,a}^{\rm ren}+a^{-2}c_a S_a+a^{-6}d_a1,
\]
then multiplying by \(a^2\) and taking an angular variation leaves \(c_a\mathcal L S_a\), unless \(S_a\) is exactly invariant under that continuous generator. Hypercubic symmetry alone does not prove this finite-cutoff cancellation. The identity power before multiplying by \(a^2\) is \(a^{-6}\), not \(a^{-4}\).

### R.3 Tensor reconstruction and its reflection action

OS II [OSII], p.283, Remark 5, explicitly extends the corrected results to indexed fields of arbitrary spin, with the formulation in OS I, section 6. Use the corrected growth theorem in OS II, section IV.1, pp.287-288. No scalar-only reinterpretation of the 21 indices is needed.

For \(Q_{\mu\nu,\rho\sigma}\), reflection in time contributes \((-1)^r\), with \(r\) the number of time indices among the four displayed indices. The OS involution includes this tensor action, complex conjugation and reversal of product order. A componentwise bound uniform in the labels costs at most \(21^m\) on tensor-valued tests, which changes only its exponential constant. Wick factors \(i^r\) (or consistently \((-i)^r\)) fix the corresponding Hermitian Minkowski convention; they must be retained when discussing pseudoscalars and reflection positivity.

### R.4 A limited free-symbol diagnostic

For a centered spectral interpolation of free lattice curvature, put
\(\widetilde p_\mu=(2/a)\sin(ap_\mu/2)\). Let \(\Gamma^a\) be the free curvature covariance multiplier obtained by replacing each momentum in the continuum degree-zero curvature projector by \(\widetilde p\), and extend it by zero outside the Brillouin zone. The inequalities
\[
\widetilde p^2\ge(4/\pi^2)|p|^2,\qquad
|\widetilde p-p|\le Ca^2|p|^3
\]
inside the zone give \(\|\Gamma^a(p)-\Gamma(p)\|\le Ca^2|p|^2\). Outside it, boundedness of \(\Gamma\) gives the same bound. Plancherel therefore yields
\[
|C_a(f,g)-C(f,g)|\le Ca^2\|\nabla f\|_2\|\nabla g\|_2.
\]
Continuum rotational covariance gives an analogous finite-rotation defect bound. The kinetic symbol displays the anisotropy:
\[
\widetilde p^2=p^2-\frac{a^2}{12}\sum_\mu p_\mu^4+O(a^4|p|^6),
\quad
(p_\mu\partial_{p_\nu}-p_\nu\partial_{p_\mu})\sum_\lambda p_\lambda^4
=4(p_\mu p_\nu^3-p_\nu p_\mu^3).
\]
This calculation concerns a free spectral diagnostic. It neither proves an interacting angular estimate nor identifies a local reflection-positive Wilson interpolation.

## Part IV. Ultraviolet coefficients, energy estimates, and phase transfer

### 1. A decisive ultraviolet normalization check: the free scalar three-point coefficient is zero

#### 1.1 Explicit conventions

Let \(d_A=\dim\mathfrak g\). Use a canonical free Euclidean gauge potential with covariance
\[
 \langle a_\mu^c(x)a_\nu^d(y)\rangle
 =\delta^{cd}\delta_{\mu\nu}\Delta(x-y),\qquad
 \Delta(z)=\frac1{4\pi^2|z|^2}.
\]
Only the gauge-invariant linearized curvature \(f_{\mu\nu}=\partial_\mu a_\nu-\partial_\nu a_\mu\) is used below. Write \(A=(\mu,\nu)\), \(\mu<\nu\), for the six independent two-form indices. For \(z\ne0\), direct differentiation gives
\[
 K_{\mu\nu,\rho\sigma}(z)
 =-\delta_{\nu\sigma}\partial_\mu\partial_\rho\Delta
   +\delta_{\nu\rho}\partial_\mu\partial_\sigma\Delta
   +\delta_{\mu\sigma}\partial_\nu\partial_\rho\Delta
   -\delta_{\mu\rho}\partial_\nu\partial_\sigma\Delta.
 \tag{U1}
\]
Since
\[
 \partial_\mu\partial_\rho\Delta(z)
 =\frac1{2\pi^2|z|^4}\left(-\delta_{\mu\rho}+4\frac{z_\mu z_\rho}{|z|^2}\right),
\]
this becomes
\[
 K(z)=\frac1{\pi^2|z|^4}\Lambda^2 I(z),\qquad
 I(z)=1-2\frac{zz^T}{|z|^2}.
 \tag{U2}
\]
Here \(I(z)\) is an orthogonal reflection of \(\mathbb R^4\), and \(\Lambda^2 I\) acts on the six independent two-form components. Formula (U2) is a separated-point formula; contact terms are not asserted to vanish.

Define the centered scalar
\[
 O_0(x)=\frac12\sum_{c=1}^{d_A}\sum_{\mu<\nu}:f^c_{\mu\nu}(x)^2:
       =\frac14\sum_{c,\mu,\nu}:f^c_{\mu\nu}(x)^2:.
 \tag{U3}
\]
This normalization is stated explicitly so that no coefficient is confused with a different `Tr F²` convention.

#### 1.2 Two-point coefficient

For distinct \(x,y\), Wick's rule gives
\[
 \kappa_2(O_0(x),O_0(y))
 =\frac{d_A}{2}\operatorname{tr}_{\Lambda^2}\bigl(K(x-y)K(y-x)\bigr)
 =\frac{3d_A}{\pi^4|x-y|^8}.
 \tag{U4}
\]
Indeed \(I(z)^2=1\) and \(\dim\Lambda^2\mathbb R^4=6\). For disjointly supported test functions the coefficient is the corresponding double integral; there is no extension across a collision in this assertion.

#### 1.3 Three-point coefficient and all odd scalar cumulants

For three distinct points, Wick's rule gives
\[
 \kappa_3(O_0(x_1),O_0(x_2),O_0(x_3))
 =d_A\operatorname{tr}\bigl(K_{12}K_{23}K_{31}\bigr).
 \tag{U5}
\]
This expression is identically zero in dimension four.

**Proof.** Let \(*\) be the Euclidean Hodge star on two-forms. If \(R\in O(4)\) reverses orientation, then
\[
 *\Lambda^2R=-\Lambda^2R*.
\]
Each \(I(x_i-x_j)\) reverses orientation. Thus every \(K_{ij}\) anticommutes with \(*\), and an odd product of these matrices also anticommutes with \(*\). In the decomposition into self-dual and anti-self-dual two-forms, an anticommuting matrix has zero diagonal blocks, hence zero trace. Apply this to (U5). Equivalently, \(I_{12}I_{23}I_{31}\) is orientation reversing, so \(\operatorname{tr}\Lambda^2(I_{12}I_{23}I_{31})=0\). This proof does not require the three displacement vectors to be independent. \(\square\)

The same argument proves a stronger statement: **every separated odd connected cumulant of the free scalar \(O_0\) vanishes.** The connected Wick diagrams of quadratic fields are cycles, and every odd cycle contains an odd number of curvature covariance matrices. Centering removes the one-point term. Every odd full centered moment at separated points also vanishes: any Wick graph on an odd number of quadratic vertices has an odd cycle. The even connected cumulants need not vanish, so this statement does not make \(O_0\) a Gaussian random field.

This is more specific than the observable route's general warning that a quadratic composite of a free field can have a nonzero third cumulant. That warning applies to generic quadratic composites, but the four-dimensional free scalar action density has the cancellation above.

#### 1.4 Tensor marks can have a nonzero Gaussian three-point coefficient

For symmetric real \(6\times6\) matrices \(B_i\), set
\[
 O_{B_i}(x)=\frac12\sum_c:f^c(x)^TB_if^c(x):.
\]
At separated points,
\[
 \kappa_2(O_{B_1}(x_1),O_{B_2}(x_2))
 =\frac{d_A}{2}\operatorname{tr}(B_1K_{12}B_2K_{21}),
\]
\[
 \kappa_3(O_{B_1}(x_1),O_{B_2}(x_2),O_{B_3}(x_3))
 =d_A\operatorname{tr}(B_1K_{12}B_2K_{23}B_3K_{31}).
 \tag{U6}
\]
The two orientations of the triangle give equal traces, by transposition, because the \(B_i\) and \(K_{ij}\) are symmetric.

Choose every \(B_i\) to project onto the \((1,2)\) curvature component and put the three points on the fourth coordinate axis. Then
\[
 \kappa_3(O_B(x_1),O_B(x_2),O_B(x_3))
 =\frac{d_A}{\pi^6|x_{12}|^4|x_{23}|^4|x_{31}|^4}>0.
 \tag{U7}
\]
The kernel remains positive in sufficiently small disjoint neighborhoods, so positive test functions in those neighborhoods give a nonzero smeared coefficient. This establishes a valid tensor benchmark, but it does not replace the Route's scalar target or demonstrate a nonabelian interaction.

#### 1.5 Consequence for the requested nonzero scalar ultraviolet law

For the conventional connection normalization
\[
 S(A)=\frac1{4g^2}\int\sum_{c,\mu,\nu}F^c_{\mu\nu}(A)^2,
 \qquad A=g a,
\]
write the bare scalar as
\[
 O_{\mathrm{bare}}=\frac14\sum F(A)^2
 =g^2O_0+g^3O_1+g^4O_2.
\]
Its separated two-point function starts formally at \(g^4\rho^{-8}\) with the nonzero coefficient (U4). Its candidate \(g^6\rho^{-12}\) scalar three-point term is zero by (U5). Gaussian parity eliminates the candidate order \(g^7\): one cubic insertion or one cubic interaction vertex leaves an odd total number of canonical Gaussian fields. The first perturbatively allowed scalar three-point order is therefore \(g^8\rho^{-12}\). This is only power counting: it does **not** prove that the order-\(g^8\) coefficient is nonzero, nor that the asymptotic expansion holds for the full Wilson measure.

For the canonical scalar \(g^{-2}O_{\mathrm{bare}}\), the first candidate three-point coefficient is instead order \(g^2\rho^{-12}\). A running multiplicative renormalization changes both normalizations again. Thus:

1. Determine the first actually nonzero scalar perturbative coefficient in the chosen scheme.
2. Specify the running field normalization and convert the coupling convention.
3. Prove the full-law remainder is smaller than that first nonzero order. A mere `O(g²)` error around the zero canonical Gaussian three-point coefficient cannot identify its order-\(g²\) coefficient.
4. Prove the cutoff remainder after the same normalization tends to zero, taking the continuum limit at fixed physical separation before sending the separation to zero.
5. Transfer the resulting coefficient to the selected phase.

A sufficient form, if the canonical scalar has nonzero first coefficient \(c_3^{(1)}\), is
\[
 \left|\frac{\rho^{12}}{g(\rho)^2}
 S^c_{3,n}(\widetilde O_\rho(f_{1,\rho}),\widetilde O_\rho(f_{2,\rho}),\widetilde O_\rho(f_{3,\rho}))
 -c_3^{(1)}(f_1,f_2,f_3)\right|
 \le\epsilon_{\mathrm{UV}}(\rho)+\epsilon_{\mathrm{cut}}(a_n/\rho,\rho/T_n),
 \tag{U8}
\]
with both errors vanishing in the stated order of limits. Here \(\widetilde O_\rho\) explicitly denotes the scalar whose leading canonical free coefficient is (U3), after its known running multiplicative factor is removed. Formula (U8) is a **target**, not a proved Yang–Mills estimate.

#### 1.6 Primary perturbative cross-check and contact warning

The perturbative OPE in [BB19, section 3.2, (3.4)-(3.7)] has a separated coefficient \(4\beta_0g_t^2/(\pi^2|x|^4)\) multiplying its canonically normalized \(F^2\), and a tree-level contact term. Appendix A records the vanishing lowest-order separated three-point function. An integrated coupling derivative can therefore receive contact contributions; it cannot establish a nonzero separated Gaussian coefficient. These are perturbative checks, without a constructive Wilson remainder.

#### 1.7 Optional small-plaquette dictionary for the Route's action

Under the explicit conventions \(\operatorname{Tr}(T^cT^d)=\delta^{cd}/2\), Hermitian generators, and one plaquette for each \(\mu<\nu\),
\[
 N-\operatorname{ReTr}U_{\mu\nu}(x)
 =\frac{a^4}{4}\sum_cF^c_{\mu\nu}(x)^2+O(a^6)
\]
for smooth classical fields with curvature evaluated at the plaquette center, or with a symmetric centered prescription. A lower-corner evaluation generally gives an \(O(a^5)\) remainder instead. Hence the Route's \(2Nx\sum_p(N-\operatorname{ReTr}U_p)\) has classical leading action
\[
 Nx\int O_{\mathrm{bare}},\qquad g^{-2}=Nx.
 \tag{U9}
\]
The coupling-derivative density is then \(N O_{\mathrm{bare}}\) at leading classical order, and its canonical Gaussian two-point coefficient is
\(3d_A/(\pi^4x^2|x-y|^8)\).
If oriented plaquettes are double-counted, the dictionary must be changed accordingly. This smooth-field expansion does not establish the quantum renormalized field, its running mixing, or its full-law continuum asymptotics.

#### 1.8 A published fixed-shape perturbative benchmark

The conformal perturbative framework of [BP24, (6.11), p.26; section 6.2, p.28] specifies
\[
 [g_t^2]\,\kappa_3^{\mathrm{pert}}(q(x_1),q(x_2),q(x_3))
 =\frac{3\beta_0(N^2-1)}{\pi^6|x_{12}|^4|x_{23}|^4|x_{31}|^4},
 \quad q=F^2/4,\quad\beta_0=\frac{11}{3(4\pi)^2}.           \tag{U10}
\]
The source uses a conformal ansatz and OPE matching at this order; \([g_t^2]\) means a formal coefficient. This nonzero pure-SU(N) benchmark supplies no controlled Wilson remainder. The required error is \(o(g_t^2)\) after canonical normalization, with running field matching and phase transfer still to prove. A formal next order is not a rigorous error estimate.

### 2. An exact energy-cutoff version of the missing operator estimate

The Route proves that a heat-semigroup estimate implies a polynomial energy bound (Proposition 8.1 of [Yang–Mills existence through observable derivatives](../observable_route.md)). The following equivalence gives a second concrete exit criterion.

#### Proposition E1: spectral cutoff and heat estimates are equivalent

Let \(H\ge0\) be self-adjoint and \(\phi(f)\) closed. Set \(P_E=1_{[0,E]}(H)\). Assume \(r\ge0\), and assume the stated domains and bounds hold uniformly in the finite field label.

The spectral-cutoff hypothesis
\[
 P_E\mathcal H\subset D(\phi(f)),\qquad
 \|\phi(f)P_E\|\le C\nu_s(f)(1+E)^r
 \quad(E\ge0)
 \tag{E1}
\]
implies
\[
 e^{-tH}\mathcal H\subset D(\phi(f)),\qquad
 \|\phi(f)e^{-tH}\|\le C_r\nu_s(f)t^{-r}
 \quad(0<t\le1).
 \tag{E2}
\]
Conversely (E2) implies (E1), with constant \(eC_r\).

**Proof, forward.** The spectral theorem gives the strongly convergent identity
\[
 e^{-tH}=t\int_0^\infty e^{-tE}P_E\,dE.
\]
On finite upper intervals this identity and its image under \(\phi(f)\) define graph-valued integrals. By (E1), the image integral converges in norm, with
\[
 t\int_0^\infty e^{-tE}\|\phi(f)P_E\|\,dE
 \le C\nu_s(f)t^{-r}\int_0^\infty e^{-u}(t+u)^rdu
 \le C\nu_s(f)t^{-r}\int_0^\infty e^{-u}(1+u)^rdu.
\]
Closedness proves domain inclusion and (E2). Measurability can be seen by restricting to finite spectral intervals, where \(\phi(f)P_M\) is bounded. **Reverse.** Take \(t=(1+E)^{-1}\). Since \(e^{tH}P_E\) is bounded by \(e\),
\[
 \phi(f)P_E=\phi(f)e^{-tH}e^{tH}P_E,
\]
which proves (E1). \(\square\)

Applying Proposition 8.1 of [Yang–Mills existence through observable derivatives](../observable_route.md) yields \(\|\phi(f)(1+H)^{-R}\|\le C_R\nu_s(f)\) for every \(R>r\). This result turns E into a spectral-subspace estimate with a precise degree-independent constant. It does not make that estimate follow from vacuum cumulants.

#### Proposition E2: a sufficient OS quadratic-form criterion

Let \(\mathcal P_+\) be the positive-time algebra used in reconstruction, with OS seminorm
\[
 \|P\|_{\mathrm{OS}}^2=S(\Theta P\,P),
\]
and quotient map \(q:\mathcal P_+\to\mathcal H\) with dense image. Suppose a rigorously defined linear insertion/translation map \(B_{f,t}\) on a dense linear domain satisfies
\[
 q(B_{f,t}P)=\phi(f)e^{-tH}q(P)
 \tag{E3}
\]
on a common dense domain, and suppose
\[
 S(\Theta B_{f,t}P\,B_{f,t}P)
 \le C^2\nu_s(f)^2t^{-2r}S(\Theta P\,P)
 \quad\text{for every }P\in\mathcal P_+.
 \tag{E4}
\]
Then \(B_{f,t}\) descends through the null space, extends to a bounded operator of norm at most \(C\nu_s(f)t^{-r}\), and (when \(\phi(f)\) is closed and (E3) is verified on the stated core) gives the desired heat estimate by closure.

**Proof.** A null vector on the right is null on the left, so the quotient is well-defined. The inequality gives a bounded map on a dense subspace; extend it continuously. Closedness of \(\phi(f)\) applies to sequences \(q(P_j)\to v\): \(e^{-tH}q(P_j)\to e^{-tH}v\), while the bounded insertion images converge. \(\square\)

The same inequality for arbitrary linear combinations of finitely many polynomials is equivalent to the matrix inequality
\[
 [S(\Theta B_{f,t}P_i\,B_{f,t}P_j)]_{i,j}
 \preccurlyeq C^2\nu_s(f)^2t^{-2r}
 [S(\Theta P_i\,P_j)]_{i,j}.
 \tag{E5}
\]
This is a checkable all-state target. Its constant must not grow with the polynomial degree or number of vectors. The value at \(P=1\) is only a vacuum estimate. Formula (E3), including its analytic continuation and domains for spacetime-smeared fields, remains part of the construction; an unproved time-zero identification cannot be inserted here.

For an actual finite-cutoff transfer Hamiltonian \(H_n\), the corresponding requirement is the quadratic-form inequality
\[
 \|\phi_n(f)e^{-tH_n}v\|^2
 \le C^2\nu_s(f)^2t^{-2r}\|v\|^2\quad(v\in\mathcal H_n),
 \qquad e^{-tH_n}\mathcal H_n\subset D(\phi_n(f)).          \tag{E6}
\]
Equivalently, after the bounded extension is established, \((\phi_ne^{-tH_n})^*(\phi_ne^{-tH_n})\le C^2\nu_s(f)^2t^{-2r}I\). No unverified operator-product domain for \(\phi_n^*\phi_n e^{-tH_n}\) is assumed. Constants must be independent of cutoff and volume; a single vacuum matrix element does not suffice.

### 3. A weaker sufficient phase-transfer criterion than uniform central control

Proposition 8.2 of [Yang–Mills existence through observable derivatives](../observable_route.md) proves a pointwise almost-everywhere phase conclusion from a bound against every central projection. A useful alternative is a projected second-moment estimate plus summability.

#### Proposition P-UV: projected vacuum variance and Borel–Cantelli

Assume a measurable direct-integral decomposition
\[
 \mathcal H=\int^\oplus\mathcal H_\xi\,d\nu(\xi),\quad
 \Omega=\int^\oplus\Omega_\xi\,d\nu(\xi),
\]
where \(\|\Omega_\xi\|=1\), and the translation-invariant subspace in each component is exactly \(\mathbb C\Omega_\xi\). Thus
\[
 P_0=\int^\oplus |\Omega_\xi\rangle\langle\Omega_\xi|\,d\nu(\xi).
\]
Here \(P_0\) is the projection onto translation-invariant vectors. If it is instead defined as \(1_{\{0\}}(H)\), identify these projections using the joint spectral condition.
Let \(A_j\) be decomposable and \(\Omega\in D(A_j)\). Put \(a_j(\xi)=\langle\Omega_\xi,A_{j,\xi}\Omega_\xi\rangle\). Then
\[
 \|P_0(A_j-c_jI)\Omega\|^2
 =\int |a_j(\xi)-c_j|^2d\nu(\xi).
 \tag{P1}
\]
If the left side is at most \(\epsilon_j^2\), and positive \(\delta_j\to0\) satisfy
\[
 \sum_j\frac{\epsilon_j^2}{\delta_j^2}<\infty,
 \tag{P2}
\]
then for almost every phase, \(|a_j(\xi)-c_j|\le\delta_j\) for all sufficiently large \(j\).

**Proof.** Identity (P1) is the direct-integral formula for \(P_0\). Chebyshev bounds the measure of \(\{|a_j-c_j|>\delta_j\}\) by \(\epsilon_j^2/\delta_j^2\). The first Borel–Cantelli lemma proves the conclusion; no independence is required. \(\square\)

Countably many test configurations and raw moments may be combined by a summable weighted exceptional-set budget, or handled one at a time and intersected after each conclusion is proved. To conclude a quantitative law for all continuously varying scales, one still needs a phasewise modulus of continuity between the chosen scale nodes. A statement on a discrete subsequence cannot silently be upgraded to all scales.

For example, at \(\rho_j=e^{-j}\), if \(\epsilon_j\le Cj^{-\beta}\), one may take \(\delta_j=j^{-\alpha}\) whenever \(0<\alpha<\beta-1/2\). If \(\beta\le1/2\), this particular grid/rate argument does not supply a decaying polynomial tolerance. A sparser scale sequence may restore summability, but requires additional interpolation control if the target quantifies all scales.

This criterion is weaker than the Route's uniform bound \(\|P_0(A_\rho-c_\rho)P_0\|\le\epsilon(\rho)\): it uses only the specified vacuum vector and an \(L^2\) phase error. It is still an unproved interacting estimate, and the full norm \(\|(A_\rho-c_\rho)\Omega\|\) generally need not shrink because local ultraviolet fluctuations persist. The projection \(P_0\) is essential.

#### 3.1 Quantitative stability of connected coefficients

Let \(\mu_I\) and \(\mu_I^*\) be raw moments of normalized fields for nonempty subsets \(I\subset\{1,\ldots,m\}\). Suppose
\[
 |\mu_I|,|\mu_I^*|\le M,\qquad |\mu_I-\mu_I^*|\le\epsilon.
\]
Using the finite partition formula for cumulants and telescoping each product,
\[
 |\kappa_m(\mu)-\kappa_m(\mu^*)|
 \le\epsilon\sum_{k=1}^m S(m,k)k!M^{k-1}.
 \tag{P3}
\]
Here \(S(m,k)\) are Stirling numbers of the second kind. In particular,
\[
 |\Delta\kappa_2|\le(1+2M)\epsilon,\qquad
 |\Delta\kappa_3|\le(1+6M+6M^2)\epsilon.
 \tag{P4}
\]
Thus phase-transfer bounds must be supplied for all lower raw moments needed by the subtractions, unless each component has already been centered by a compatible local prescription.

For scalar translation-invariant components and test functions with integral zero, every phase mean vanishes. The conditional cumulant formulas then imply that the mixed second and third connected functions equal the averages of their phase values. At order four an extra term remains:
\[
 \kappa_4^{\mathrm{mix}}
 =\int\kappa_4^\xi d\nu
  +\sum_{\{ij\}\{kl\}}\operatorname{Cov}_\nu(\kappa_2^\xi(i,j),\kappa_2^\xi(k,l)).
\]
Even at order three, knowing only the average coefficient does not identify its phase value or select a common phase at all scales; Proposition P-UV or the Route's central-projection condition addresses that missing step.

### 4. A concrete sufficient mechanism to transfer factorial growth to almost every phase

This statement makes clear what a quantitative phase-growth proof would have to supply. It does not assert that the Route's mixed flat-Schwartz bound alone verifies its Hilbert-space hypothesis.

#### Proposition P-Growth: Hilbert-dual summability transfers the whole order sequence

For each \(m\), let \(\mathcal D_m\) be the actual Fréchet test space, continuously embedded in a separable Hilbert space \(\mathcal T_m\). Choose an orthonormal basis \(e_{m,k}\subset\mathcal D_m\) whose finite span is dense in \(\mathcal D_m\) in its original Fréchet topology. Assume the phase distributions are continuous on \(\mathcal D_m\) on a common full-measure set. Pack all field-label tuples into this test space (or sum the following hypothesis over those tuples). Suppose
\[
 \int\sum_k|\ell_{m,\xi}(e_{m,k})|^2d\nu(\xi)
 \le C^{2m+2}(m!)^{2p}.
 \tag{P5}
\]
Then almost every phase admits a finite constant \(C_\xi\) such that, simultaneously for every \(m\),
\[
 |\ell_{m,\xi}(F)|
 \le C_\xi^{m+1}(m!)^p\|F\|_{\mathcal T_m}.
 \tag{P6}
\]

**Proof.** By Fubini, \(N_m(\xi)^2=\sum_k|\ell_{m,\xi}(e_{m,k})|^2\) is finite for each \(m\) on a common full-measure set and is the squared dual norm. Markov gives
\[
 \nu\{N_m>2^mC^{m+1}(m!)^p\}\le4^{-m}.
\]
Borel–Cantelli makes this bound hold for every sufficiently large \(m\) for almost every phase. Absorb the finitely many exceptional \(N_m\)'s into one finite \(C_\xi\). Cauchy–Schwarz gives (P6) on the finite span. Its density in the original test topology, continuity of the original phase functional, and continuity of the Hilbert embedding identify the extension on every original test. \(\square\)

If, uniformly in \(m\),
\[
 \|F\|_{\mathcal T_m}\le D^{m+1}(m!)^q\nu_{cm+d}(F),
\]
then (P6) gives the desired fixed linear Schwartz order and fixed factorial exponent \(p+q\), with a phase-dependent base constant. This is sufficient for a selected phase. Hilbert density alone is insufficient: an \(L^2\)-basis of smooth functions vanishing at the origin has zero coefficients for \(\delta_0\), although that distribution is not zero. The stronger density/continuity hypothesis above is therefore necessary for the identification.

One route to (P5) would be a verified decomposable Euclidean product \(A_m(F)\) for which
\[
 |\ell_{m,\xi}(F)|^2\le\|A_{m,\xi}(F)\Omega_\xi\|^2,
 \qquad
 \sum_k\|A_m(e_{m,k})\Omega\|^2
 \le C^{2m+2}(m!)^{2p}.
 \tag{P7}
\]
The second inequality is a quantitative nuclearity/summability requirement on the mixed hierarchy and the chosen test Hilbert norms. One must verify Euclidean product decomposability, ordered-time domains and contact control, and the order-dependent constants. Those checks are not consequences of merely writing a direct integral for Minkowski Wightman fields. This theorem provides an alternative to requiring a uniform central bound against every projection at every order.

### 5. Disconnected symmetries require an additional phase-selection argument

The need for the Route's discrete-symmetry check can be seen in an elementary exact model. Let a central pseudoscalar have constant value \(+v\) in one one-dimensional phase and \(-v\) in another, with equal weights. At the Wightman level, each phase is translation invariant, satisfies Hilbert-space positivity and trivial polynomial energy bounds, and has a factorially bounded hierarchy. The mixture is invariant under parity when parity exchanges the phases and changes the sign of the pseudoscalar. Neither individual phase is parity invariant if \(v\ne0\).

This is a Wightman-level symmetry counterexample. A real constant Euclidean pseudoscalar with reflection sign minus is not an OS-positive example without the appropriate Wick/reality convention. At the Wightman level the construction can be tensored with a fixed ultraviolet theory, or implemented by shifts \(P(x)\mapsto P(x)\pm vI\) of a dimension-four pseudoscalar in two copies. Its leading separated ultraviolet coefficients are unchanged by a constant identity shift after the appropriate dimension-four scaling, while parity can still exchange the two phases. Therefore common ultraviolet coefficients and inherited energy bounds do not, on their own, select a parity-invariant phase.

A completion must prove that a phase carrying the required ultraviolet laws, growth bounds and operator bounds is fixed by the disconnected symmetry, or supply another phase-selection construction achieving the required covariance. Averaging two symmetry-related pure phases restores the symmetry but usually loses purity; it does not close this requirement.

### E.3 Verified scope of the phase-decomposition theorem

In Driessler–Summers [DS], Definition 2.1 (p.334) allows a positive decreasing energy regulator \(F_f(H)\) with a domain inclusion and bounded \(\phi(f)F_f(H)\). A polynomial energy bound supplies such a regulator. Theorem 2.3 (pp.335-336) yields pure-phase Wightman components with unique vacua; clause (vi) transfers existing energy estimates almost everywhere, and the paper states the finite-component extension. These conclusions do not themselves assert the same fixed factorial Euclidean growth estimate or invariance of a selected phase under every disconnected symmetry. Those remain the quantitative checks described above.
