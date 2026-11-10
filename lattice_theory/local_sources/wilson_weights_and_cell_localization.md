# Wilson source weights and localization of the vacuum term

## Bare normalization and the plaquette anchor

For a four-dimensional periodic \(SU(N)\) Wilson lattice, \(N\ge2\), put \(s_p=N-\operatorname{Re}\operatorname{Tr}U_p\) and \(S=\sum_p s_p\). With inverse coupling \(x=\beta/(2N)\), a scalar source \(j_p\) gives the plaquette coefficient \(2Nx-j_p\). The coefficient multiplying \(1-N^{-1}\operatorname{Re}\operatorname{Tr}U_p\) is \(2N^2x-Nj_p\).

The factor can be recovered from a density ratio even when the vacuum normalization is arbitrary. Take at least three sites in each direction. Replace one link of the identity configuration by \(\operatorname{diag}(e^{i\theta},e^{-i\theta},1,\ldots,1)\). Each of the six incident plaquettes contributes \(\sigma=2-2\cos\theta>0\). If at zero source the densities \(c\exp(-2Nx S)\) and \(d\exp[-\sum_p(x+e_p)s_p]\) agree, their log ratios to the identity give

\[
 (2N-1)x=\tfrac16\sum_{p\ni b}e_p.
\]

Thus uniformly bounded \(e_p\) cannot absorb this change along \(x\to\infty\). The identity holds for arbitrarily small nonzero \(\theta\), including a regular neighborhood that shrinks with the cutoff. Continuity and full support of Haar measure suffice if the two densities agree almost everywhere on that neighborhood.

Let \(p_{\mu\nu}(x)\) denote the positive plaquette with initial vertex \(x\), and let \(\Theta\) reverse coordinate \(\mu\). Reversing the plaquette and changing its base point preserve its real trace. Consequently

\[
 s_{p_{\mu\nu}(x)}(\Theta U)=s_{p_{\mu\nu}(\Theta x-a e_\mu)}(U).
\]

For a plaquette in two directions transverse to \(\mu\), the reflected initial vertex is \(\Theta x\). An exactly covariant *different* sampling rule is \(\bar j_p=\tfrac14\sum_{v\in p}j(v)\). Its conjugate observable is \(O^{\mathrm{sym}}_a(v)=(4a^4)^{-1}\sum_{p\ni v}s_p\), giving \(\sum_v a^4 j(v)O^{\mathrm{sym}}_a(v)=\sum_p\bar j_p s_p\). For lower-vertex sampling, transferring a reflection estimate requires control of the difference with the actual subtractions. The two finite-lattice observables are distinct.

## A cell decomposition from a counted carrier bound

Fix a cell side \(\ell\), a torus of side \(T\ge2\ell\) tiled by \(N_T=(T/\ell)^4\) cells, and meshes \(a=\ell L^{-K}\le h_k=\ell L^{-(K-k)}\), \(L\ge2\). All grids are aligned. Take a scalar periodic \(C^5\) source \(j\), restricting its values to the bare grid. Write \(\|j\|_{5,\ell}=\max_{0\le m\le 5}\ell^m\|D^m j\|_\infty\).

**Proposition.** Suppose the *complete* vacuum difference \(V_{a,T}(j)\), including the integration and coordinate normalizations, has an absolutely convergent expansion \(\sum_{k,y,X} A_{k,T}(y,X;j)\) over roots \(y\in\Lambda_{h_k,T}\) and rooted carriers \(X\), with \(A(0)=0\). Assume the following bounds for \(r=K-k\).

1. A carrier of size \(d(X)\) uses only source samples within radius \(h_k(d(X)+\rho_r)\) of its root, where \(\rho_r\le C(1+r)^v\). Its activity is holomorphic on the complex ball of radius \(R>0\) in the sup norm of those samples, bounded by \(M_{k,T}(y,X)\) and real for real samples.
2. Inside a neighborhood of diameter smaller than a fixed fraction of \(\ell\), embedded activities and their enumeration agree with common local formulas. These formulas, their geometric cutoffs, and their source sampling transform under the translations and face reflections required for the cell functional. Contributions that fail to copy belong to the long-carrier tail.
3. In the torus expansion and in the common local formulas, uniformly in the root,

\[
 \sum_{d(X)\ge D}M_{k,T}(y,X)\le A(1+r)^q\exp[-\kappa D/(1+r)^v],\qquad D\ge0,
\]

with \(A,\kappa>0\), \(q,v\ge0\) independent of \(T,K\).

There is a functional \(L_a\) of the samples in one closed cell, real on real sources and holomorphic on sufficiently small finite-dimensional complex source families, with \(L_a(0)=0\). It respects the indicated cell symmetries, is independent of \(T\), and for \(\|j\|_{5,\ell}\) sufficiently small satisfies

\[
 \big|V_{a,T}(j)-\sum_c L_a(j|_c)\big|\le C N_T\|j\|_{5,\ell}.
\]

**Proof.** A function on the complex sup-norm ball bounded by \(M\) satisfies \( |A(z)-A(z')|\le(2M/R)\|z-z'\|_\infty\) on the half-radius ball. Apply Cauchy's one-variable formula along the unit direction of the difference, then integrate along the segment. This step is independent of the number of source coordinates.

At a root \(y\in c\), choose signs \(\sigma_i\in\{-1,1\}\) so that the stencil \(y+a\sigma\alpha\), \(\alpha\in\mathbb N_0^4\), \( |\alpha|\le4\), lies in \(c\), with componentwise multiplication. Such signs exist for \(\ell\ge8a\). Average over all admissible choices the polynomial

\[
 P^\sigma_{y,c}j(z)=\sum_{|\alpha|\le4}(\Delta_{a\sigma}^{\alpha}j)(y)
 \prod_{i=1}^4\binom{(z_i-y_i)/(a\sigma_i)}{\alpha_i}.
\]

Here \(\Delta\) is an undivided forward difference. The resulting \(P_{y,c}\) reproduces all polynomials of total degree at most four, uses only closed-cell samples and commutes with cell reflections. Compare with the fourth-degree Taylor polynomial at \(y\). On the stencil the Taylor error is at most \(C\|j\|_{5,\ell}(a/\ell)^5\). At distance at most \(D\ge a\) the sum of the absolute interpolation coefficients is at most \(C(1+D/a)^4\). Polynomial reproduction and the Taylor estimate on that ball give

\[
 \|j-P_{y,c}j\|_{B(y,D)}\le C\|j\|_{5,\ell}((D+a)/\ell)^5.
\]

Use the lifted source on each embedded ball for this estimate. Choose \(0<\delta<1/16\) small enough for the common local formulas, and call a carrier short if \(h_k(d(X)+\rho_r+8)\le\delta\ell\). Keep \(r\ge r_*\) with a fixed \(r_*\) large enough for the stencils. In \(L_a(j|_c)\) sum the common short activities evaluated on \(P_{y,c}j\). A root on \(b\) coordinate faces of the cell receives weight \(2^{-b}\) in each incident cell. These weights sum to one. Choosing the source ball small compared with \(R\) keeps each evaluated polynomial inside the half-radius ball.

The short substitution error is bounded per carrier by \(C\|j\|_{5,\ell} M L^{-5r}(d(X)+\rho_r+8)^5/R\). Integration of the counted tail gives \(\sum_X M(d(X)+\rho_r+8)^5\le C A(1+r)^{q+5v}\). There are \(N_T L^{4r}\) roots. The short errors therefore sum to at most \(C N_T\|j\|_{5,\ell}\sum_{r\ge r_*}L^{-r}(1+r)^{q+5v}\). For long carriers use \(d(X)>\delta L^r-\rho_r-8\). Their cost is bounded by the same prefactor times a convergent sum \(\sum_r L^{4r}(1+r)^q e^{-c L^r/(1+r)^v}\), after absorbing finitely many scales. The discarded coarse scales also cost at most \(C N_T\|j\|_{5,\ell}\). Normal convergence on finite-dimensional source families gives the asserted holomorphy. The stencil average, root weights and common formulas give the symmetries. ∎

**Counterexample.** Fix \(T\), set \(n_a=(T/a)^4\), and attach the field-independent activity \(\bar j^2\) to every fine site, with \(\bar j=T^{-4}\int j\). These bounded analytic activities depend on no gauge links. For sources \(f,g\) of nonzero average supported strictly inside different cells, the mixed difference of \(n_a\bar j^2\) equals \(2n_a\bar f\bar g\). Any sum of single-cell functionals has zero mixed difference there, while a uniformly bounded \(C N_T\) remainder contributes at most \(4C N_T\). The divergence at fixed \(T\) proves that localization in the gauge variables alone cannot give the source-local decomposition.

This proposition requires counted source-local activities for the full interacting vacuum difference. The explicit first-step Gaussian and compact Wilson kernels have their own localization estimates. [Spatially varying Wilson couplings](../varying_coupling.md)

## The scalar Hessian on a fixed regular constraint chart

Consider a link curve \(U_b(t)=e^{tv_b}U_b\) with anti-Hermitian \(v_b\). On a reversed edge take \(v_{b^{-1}}=-\operatorname{Ad}_{U_b^{-1}}v_b\). Transport the four oriented tangents around a plaquette to its initial vertex to obtain \(\xi_1,\ldots,\xi_4\), and put \(K_p=\sum_i\xi_i\), \(C_p=\sum_{i<j}[\xi_i,\xi_j]\). Differentiating \(U_p(t)=(\prod_i e^{t\xi_i})U_p\) twice gives

\[
 s_p''(0)=\|K_p\|_{\rm HS}^2-\operatorname{Re}\operatorname{Tr}[(K_p^2+C_p)(U_p-I)].
\]

Indeed \(\operatorname{Tr} C_p=0\) and \( -\operatorname{Tr} K_p^2=\|K_p\|_{\rm HS}^2\). With \(\delta_p=\|U_p-I\|_{\rm op}\), the absolute correction is at most \(\delta_p(\|K_p\|_{\rm HS}^2+3\sum_i\|\xi_i\|_{\rm HS}^2)\). This follows from \(\|[A,B]\|_1\le2\|A\|_{\rm HS}\|B\|_{\rm HS}\) and \(2ab\le a^2+b^2\). In a nonlinear constraint chart, let \(w_b(v,v)\) be the quadratic acceleration in the link exponential and \(\Omega_p\) its transported plaquette sum. The same formula then has the additional term \( -\operatorname{Re}\operatorname{Tr}[\Omega_p(U_p-I)]\).

For the scaled estimate let \(\eta\) be the fine mesh and \(h\) the single averaging scale. Fix an admitted regular background and constraint chart in the geometry of Bałaban, *Communications in Mathematical Physics* **99** (1985), 389–434, (3.35)–(3.36), (3.127)–(3.128). Write \(\mathcal T=\{A:QA=0,\ RD^*A=0\}\) for the constrained tangent space, \(D\) for the covariant differential in this chart, and \(\Psi\) for its configuration map. Here and below the scalar products use the corresponding fine and coarse lattice measures. Define

\[
 \mathcal H_f(A)=D^2\!\left[\sum_p f_p(1-N^{-1}\operatorname{Re}\operatorname{Tr}U_p)\circ\Psi\right](0)[A,A],
 \quad q(A)=\|DA\|_2^2,\quad P(A)=h^{-2}\|A\|_2^2 .
\]

**Proposition.** Under the one-scale regular propagator and lifting estimates specified below, with regularity parameter \(\varepsilon\) sufficiently small, there exist constants independent of the core size and of \(\eta,h\) such that for \(A\in\mathcal T\) and bounded real plaquette weights \(f\),

\[
 \mathcal H_1(A)\ge c P(A),\qquad |\mathcal H_f(A)|\le C\|f\|_\infty\mathcal H_1(A).
\]

**Proof.** Let \(G_1\) be the positive one-scale propagator in the chart, and suppose its block restrictions satisfy \(\|P_yG_1P_z\|_{2\to2}\le B h^2 e^{-\delta d(y,z)}\) as in Theorem 3.12 and (3.46) of the cited work. The block Schur estimate yields \(\|G_1\|\le C_G h^2\). Both penalties in (3.128) vanish on \(\mathcal T\), giving \(P(A)\le C_G\mathcal H_1(A)\).

Let \(F\) denote the normalized Lie-algebra projection of the plaquette curvature and \(J_f=D^*(fF)\). With the fine variables and normalization of (3.10), regularity gives \(\|U_p-I\|\le C\varepsilon\eta^2h^{-2}\) and \(\|F\|_\infty\le C\varepsilon h^{-2}\). Expanding the ambient Hessian \(\Delta_f\) leaves the principal form \(\langle DA,f DA\rangle\). The quadratic curvature error is bounded by \(C\|f\|_\infty\varepsilon q(A)\), and the commutator error by \(C\|f\|_\infty\varepsilon P(A)\), using the bounded plaquette incidence at a bond. The chart Hessian contains in addition \( -2\langle H C^{(2)}(A),J_f\rangle\), where \(H\) lifts the coarse datum \(QA=B\) and \(C^{(2)}\) is the quadratic constraint term in (3.127).

For this term the differentiated lifting kernel in (3.133) gives \(\sup_y\sum_p\eta^4\|D_xH(p,y)\|\le C h^{-1}\): the block kernel size is \(O(h^{-5})\) times exponential block-distance decay, and a block has \(O(h^4)\) fine measure. Hence \(\|H^*J_f\|_\infty=\|(DH)^*(fF)\|_\infty\le C\|f\|_\infty\varepsilon h^{-3}\). Use the quadratic averaging bound of (3.136)–(3.137), \( |\langle C^{(2)}(A),b\rangle|\le C h\|b\|_\infty\|A\|_2^2\), in this normalization. Its constant is uniform for the one-scale blocks, with the prescribed boundary conditions. Together the three terms give

\[
 |\mathcal H_f(A)-\langle DA,fDA\rangle|\le C\varepsilon\|f\|_\infty(q(A)+P(A)).
\]

First use \(f=1\) and \(P\le C_G\mathcal H_1\), and absorb \(C\varepsilon q\) to obtain \(q\le C'\mathcal H_1\). Apply this bound to general \(f\). ∎

In particular, \(\mathcal H_{X-f}\ge(X-C\|f\|_\infty)\mathcal H_1\) for constant \(X>0\). For bare Wilson sources \(X=2N^2x\) and \(f_p=Nj_p\). The comparison applies at the fixed regular background. A uniform existence radius for a source-dependent minimizing field, and the corresponding estimates in nested multiscale geometries, require additional bounds. The mixed clover form has separate curvature and chart terms. [Tensor quadratic admission](tensor_quadratic_admission.md)
