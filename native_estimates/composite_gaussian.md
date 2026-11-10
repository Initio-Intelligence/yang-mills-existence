# Composite constrained Gaussians and the scalar projection

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 1. Objects and conventions (fixed once)

1. **Coupling and action.** \(A(U)=\sum_p[1-\operatorname{Re}\operatorname{tr}U(\partial p)]\), normalised trace \(\operatorname{tr}1=1\) (CMP109 (0.2), page source), weight \(\exp(-YA)\), \(Y=g_B^{-2}\). Standard Wilson: \(Y=\beta_{\rm std}=2N/g_{\rm std}^2\). Program units (the constant-flux calculation, N2): \(x=Y/(2N^2)\).
2. **Projection.** For a gauge-invariant, Euclidean-covariant, localised function \(F\) of scale-\(m\) block fields \(V=\exp iB\), let \(\Pi_F\) be the infinite-volume Hessian kernel at \(B=0\), and \(\mathcal P_mF:=\sum_x\Pi_{F,\mu\nu}(x)x_\mu x_\nu\) (\(\mu\ne\nu\)) in scale-\(m\) lattice units, as in CMP109 (1.20)–(1.22) (p.264, source). Write
\[
\tilde{\mathcal P}_mF:=\mathcal P_mF\big/\mathcal P_m[A\circ U_m].
\]
By Corollary 4.3 below, \(\mathcal P_m[A\circ U_m]=\mathcal P_0[A]\) for every \(m\). In a basis of \(\mathfrak g\) orthonormal for \(\langle X,Y\rangle=\operatorname{tr}(XY)\) one has \(\mathcal P_0[A]=1\), so \(\tilde{\mathcal P}=\mathcal P\) is literally (1.22). This is the normalisation under which (1.22) is the coefficient of \(A\), as (0.20) requires.
3. **Gaussian decrement** (C2 §1.4; CMP109 (1.4), (1.20)). \(Z^{(k)}(U)=\int dB\,\delta(\tilde QB)\exp[-\tfrac12\langle B,\Delta^{(k)}(U)B\rangle]\) with the quadratic form (1.5) (p.261, source), and
\[
d^G_k:=\tilde{\mathcal P}_{k+1}\big[\log Z^{(k)}\circ U_{k+1}\big].
\]
4. **Composite one-loop density.** Fix a finite torus and a depth \(n\). Let \(A_n(V)\) be Bałaban's \(n\)-step small-field action (iterated (0.17)–(0.20)), a function of the scale-\(n\) field \(V\) near \(1\). Define, when the limit exists,
\[
\log\mathfrak D_n(V)-\log\mathfrak D_n(1):=\lim_{g_0\to0}\big[A_n(V)+Y_0A(U_n(V))\big],
\tag{1.1}
\]
the \(g^0\) term of the exact blocked density relative to coarse-link Haar measure. Set \(C_n:=\tilde{\mathcal P}_n\log\mathfrak D_n\) (infinite-volume limit of the torus readouts).
5. **the constant-flux calculation object.** the constant-flux calculation (1)–(3), §3: \(D_{\rm hard}\) is "the native one-loop density relative to coarse link Haar" of the composite readout CMP109 (0.12)/(0.10), with the hard \(\delta\) and free internal gauge integration; its cumulative decrement \(D^G_n\) is read by the same second moment in program units. §3.5 checks that the constant-flux calculation (1) is the Laplace prefactor of the composite integral, i.e. \(\mathfrak D_n\) up to \(V\)-independent constants. Hence \(D^G_n=C_n/(2N^2)\).

## 2. Theorem S (the seam)

> **Theorem S.** Fix \(N\), odd \(L\), and the CMP109 constants. For every \(n\ge1\):
> 1. (Bałaban's \(\beta\) at zero coupling.) \(d^G_k=\beta_{k+1}(0)\), where \(\beta_{k+1}(g_k)\) is defined by CMP109 (1.20)–(1.22), and \(\beta_{k+1}(g)\to d^G_k\) as \(g\to0\).
> 2. (Exact composite identity at order \(g^0\).) On every torus, for \(V\) in the small-field region, the limit (1.1) exists and
> \[
> \log\mathfrak D_n(V)-\log\mathfrak D_n(1)=\sum_{k<n}\big[\log Z^{(k)}(U_n(V))-\log Z^{(k)}(1)\big].
> \]
> 3. (Transport.) For every \(k<n\): \(\tilde{\mathcal P}_n[\log Z^{(k)}\circ U_n]=\tilde{\mathcal P}_{k+1}[\log Z^{(k)}\circ U_{k+1}]=d^G_k\).
> 4. Consequently \(\sum_{k<n}d^G_k=C_n=2N^2D^G_n\) exactly.
> 5. (Convention independence.) \(d^G_k\) does not depend on the gauge-fixing coefficient \(\alpha\) in (0.14)–(0.15), nor on any small-field cutoff, nor on constant normalisations.
> **Hypotheses.** CMP109 (0.13)–(0.20), (1.3)–(1.6), (1.20)–(1.22), (2.1)–(2.14) and the bound on \(\mathbf P^{(k)}\) on p.269 (all page-checked, §3); the localised representation of \(\log Z^{(k)}\) (CMP109 p.261, citing [16]); the flat-background structural inputs (F-a)–(F-c) of §4. Parts 3 and 4 are deduction given these inputs.

## 3. Proof of Theorem S, parts 1, 2, 5 (exactness)

### 3.1 Source statements used (printed pages; decisive text quoted)

- **(0.15), p.254.** For \(y\in T^{(1)}\), \(x\in B(y)\), \(x\ne y\):
  \(\frac1z\int du(x)\exp\big[-\frac1\alpha[1-\operatorname{Re}\operatorname{tr}U(y,x)u^{-1}(x)]\big]\chi(\{|U(y,x)u^{-1}(x)-1|<\varepsilon_0\})=\frac1z\int du(x)\exp\big[-\frac1\alpha[1-\operatorname{Re}\operatorname{tr}u(x)]\big]\chi(\{|u(x)-1|<\varepsilon_0\})=1\).
  The middle step is Haar invariance, so **\(z\) does not depend on the field**. P.255: "we change the order of integrations and apply the gauge transformation \(U\to U^{u^{-1}}\) … By the gauge invariance with respect to such transformations the integrand does not depend on \(u\) and the integral over \(u\) is equal to 1."
- **(0.17)–(0.20), pp.255–256.** \(\mathbf N_k\) "is given by the integral above with \(V=1\)". (0.20): \(1/g_{k+1}^2=1/g_k^2-\beta_{k+1}(g_k)\).
- **(1.3)–(1.4), p.260.** \(A_k(U_k)=-\frac1{g_k^2}A(U_k)+\sum_{j=0}^{k-1}\{-\beta_{j+1}(g_j)A(U_k)+[\log Z^{(j)}(U_k)-\log Z^{(j)}(1)]+[E^{(j+1)}(g_j,U_k)-E^{(j+1)}(g_j,1)]\}\). "We have written explicitly terms of the order 0 in the coupling constants." (1.4): \(Z^{(j)}(U_k)=\int dB\,\delta(\tilde QB)\exp[-\frac12\langle B,\Delta^{(j)}(U_k)B\rangle]\).
- **(1.5)–(1.6), p.261.** \(\langle B,\Delta^{(j)}(U_k)B\rangle=\langle H_{1,j}B,\Delta_1H_{1,j}B\rangle-2\langle H_{1,j}h\tilde C^{(2)}(\bar U^j_k,B),J\rangle+G^{(2)}(B)\). (1.6) folds \(\log Z^{(j)}\) into \(\mathbf E^{(j+1)}\).
- **(1.20)–(1.22), p.264.** \(\Pi^{ab}_{j+1,\mu\nu}=\big(\frac{\delta^2}{\delta B^a_\mu\delta B^b_\nu}\mathbf E^{(j+1)}\big)(g_j,0)\) with \(\mathbf E^{(j+1)}(g_j,B)=\mathbf E^{(j+1)}(g_j,U_{j+1}(\exp iB))\); "we take a limit of these functions as \(T^{(j+1)}\nearrow\mathbb Z^d\)"; \(\beta_{j+1}(g_j)=\sum_x\Pi_{j+1,\mu\nu}(g_j,x)x_\mu x_\nu\); "It is a smooth function defined on the interval \([0,\gamma]\)".
- **(2.1), p.265.** \((\mathbf T_kA_k)(W)=\log\mathbf N_k^{-1}\int dV\delta(\bar VW^{-1})\chi_k\exp[-\frac1{g_k^2}\mathbf G(V)-\frac1{g_k^2}A(U_k(V))+\mathbf E_k(U_k(V))]\).
- **(2.10), p.267.** "\(\int dB'\sigma(B')\delta(\tilde Q(B'))\) … where the factors \(\sigma_0\) are included into the normalization factor \(\mathbf N'_k\)." The change \(B'=B-h\tilde D(B)\) "linearizes the function \(\tilde Q(B')\)", \(\tilde D\) "has an expansion beginning with quadratic terms". "The quadratic form in \(B'\) above … defines the \(k\)-th normalization factor \(Z^{(k)}(U_{k+1})\) given by the formula (1.4) with \(j=k\)."
- **(2.12)–(2.14), p.268.** \(A_{k+1}(U_{k+1})=-\frac1{g_k^2}A(U_{k+1})+\mathbf E_k(U_{k+1})+[\log Z^{(k)}(U_{k+1})-\log Z^{(k)}(1)]+\log\mathbf N''^{-1}_k\int d\mu_{C^{(k)}}\chi_k\exp[\mathbf P^{(k)}+\{\cdots\}]\). "Let us remark that the expression under the exponential above vanishes at \(g_k=0\), and \(\log\mathbf N''_k=E^{(k+1)}(g_k,1)\)." "The equalities (2.12), (2.14) together with the definitions (2.13), (2.15) imply that the action \(A_{k+1}\) is given by (1.3) with \(k+1\) instead of \(k\)."
- **p.269.** \(\mathbf P^{(k)}\) "is bounded by a second order polynomial in \(B\), with coefficients of the order \(O(\varepsilon_1)\), hence it can be treated as a small perturbation of the basic quadratic form".

### 3.2 Part 2

Fix the torus and \(n\). Iterating (2.12) with \(\mathbf E_k=(1/g_k^2)A+A_k\) (p.265) gives the exact identity (Bałaban's (1.3) at \(k=n\))
\[
A_n(V)=-Y_0A(U_n)+\sum_{k<n}\big[\log Z^{(k)}(U_n)-\log Z^{(k)}(1)\big]+\sum_{k<n}\big[E^{(k+1)}(g_k,U_n)-E^{(k+1)}(g_k,1)\big],
\tag{3.1}
\]
with \(U_n=U_n(V)\). The coupling renormalisation (2.15) only reallocates multiples of \(A(U_n)\), and \(\sum\) of all coefficients of \(A(U_n)\) is \(-1/g_0^2\) by (0.20).

Let \(g_0\to0\) at fixed \(n\). Bałaban's \(\beta_j\) are bounded on \([0,\gamma]\), so \(Y_k\ge Y_0-Cn\to\infty\) and every \(g_k\to0\). For each \(k\), \(E^{(k+1)}(g_k,U)=\log\int d\mu_{C^{(k)}}\chi_k e^{\mathbf P^{(k)}+\{\cdots\}}\) (2.13). The exponent tends to \(0\) pointwise in \(B\) (2.14). The cutoff (2.9) is \(|B'(b)|<\varepsilon_1\) in the physical variable \(B'=g_kB\), so \(\chi_k\to1\) pointwise. On the support of \(\chi_k\): \(|\mathbf P^{(k)}|\le O(\varepsilon_1)(1+|B|^2)\) (p.269), and \(|\{\cdots\}|\le C\) by the inductive bound (1.18). Since \(C^{(k)}\le\gamma_0^{-1}\) (CMP99 p.428; at \(U=1\), CMP96 Lemma 2.4, stated by the comparison argument), \(e^{O(\varepsilon_1)|B|^2}\) is \(d\mu_{C^{(k)}}\)-integrable for \(\varepsilon_1\) small. This is a finite-dimensional integral on a fixed torus, so dominated convergence gives \(E^{(k+1)}(g_k,U)\to0\). The convergence is uniform for \(U\) in a compact neighbourhood of the small-field configurations, and analytic in \(V\), so derivatives in \(V\) converge too (Weierstrass). Hence the limit (1.1) exists and equals the \(Z\)-sum. conditional

**Remark (why only \(Z^{(k)}\) can carry \(g^0\) background dependence).** Every factor of the step integral is accounted for in §3.1. Haar density \(\sigma\) and the Jacobian of \(B'\mapsto B-h\tilde D(B)\) appear in (2.12) as functions of \(g_kCB\) that vanish at \(g_k=0\) (\(\sigma(0)=1\), \(\tilde D\) quadratic). The \(\delta\)-function \(\delta(\tilde QB)\) and its elimination Jacobian are inside \(Z^{(k)}\) by (1.4). \(\sigma_0\), \(\mathbf N_k,\mathbf N'_k,\mathbf N''_k\), \(z\) are field-independent. So nothing background-dependent at order \(g^0\) is left outside \(Z^{(k)}\). If a background-dependent factor had been placed in \(\mathbf N'_k\), (1.3) would be false as an identity, not merely a convention; The interpretation of (2.10)'s \(\sigma_0\) is the constant Haar-to-Lie-algebra conversion of the coarse \(\delta\) at the identity additional assumption, and the argument above does not depend on that reading because it uses (1.3)/(2.12) as stated.

### 3.3 Part 1

By (1.6) and (1.20), \(\beta_{k+1}(g_k)=\tilde{\mathcal P}_{k+1}\big[\log Z^{(k)}\circ U_{k+1}\big]+\tilde{\mathcal P}_{k+1}\big[E^{(k+1)}(g_k,\cdot)\circ U_{k+1}\big]\). The second term tends to \(0\): \(E^{(k+1)}(g_k,X,\cdot)\) is analytic on the absolute domain with \(|E^{(k+1)}|\le E_0e^{-\kappa d(X)}\), it is \(C^\infty\) in \(g\) on \([0,\gamma]\) (p.263), and it vanishes at \(g=0\) (§3.2). So its local terms are \(O(g)\) uniformly, and the readout of C2 Lemma 4.7 step 3 bounds the projection by \(Cg\). C2 Theorem 2.1 gives the quantitative \(O(g^2)\) for the driven comparator. conditional

So \(d^G_k\) is **Bałaban's own \(\beta_{k+1}\) at zero coupling**, and (G) is the statement \(\sum_{k<n}\beta_{k+1}(0)=d_Bn+O(1)\), the content of Bałaban's announced perturbative paper.

### 3.4 Part 5

For any \(\alpha>0\), (0.15) is an exact identity with field-independent \(z(\alpha)\). So the exact step integral (2.1), normalised by its value at \(V=1\), does not depend on the gauge-fixing coefficient (nor on the gauge-fixing function, as long as (0.15) holds). By induction every \(A_k\) is independent of it, hence so is the \(g^0\) part of \(A_{k+1}-A_k(U_{k+1})\), which is \(\log Z^{(k)}(U_{k+1})-\log Z^{(k)}(1)\) by §3.2 applied to one step. Individual \(Z^{(k)}\) computed with \(\alpha^{-1}G^{(2)}\) in place of \(G^{(2)}\) therefore differ from Bałaban's by a field-independent constant. The same argument with \(\chi_k\to1\) shows cutoff independence. conditional

### 3.5 the constant-flux calculation (1) is the Laplace prefactor (check of the identification in §1 item 5)

the constant-flux calculation (1): \(D_{\rm hard}=\det(V^*V)/[\det(QQ^*)\det(T^*(H+VV^*)T)]^{1/2}\), with \(V=dK\) the internal gauge directions (\(QV=0\), \(HV=0\) at a stationary field), \(T\) an isometric inclusion of \(\ker Q\). Split \(\ker Q=\operatorname{Ran}V\oplus T'\), \(T'=\ker Q\cap(\operatorname{Ran}V)^\perp\). Since \(HV=0\), \(H\) maps \(T'\) into \((\operatorname{Ran}V)^\perp\), and \(VV^*\) vanishes on \(T'\) and preserves \(\operatorname{Ran}V\). So \(\det(T^*(H+VV^*)T)=\det(H|_{T'})\det(V^*V)\), and
\[
D_{\rm hard}=\frac{\det(V^*V)^{1/2}}{\det(QQ^*)^{1/2}\det(H|_{T'})^{1/2}}
=(\text{orbit volume})\times(\text{coarea of the hard }\delta)\times(\text{transverse Gaussian}).
\]
This is the Morse–Bott Laplace prefactor of \(\int dU\,\delta(\bar U^nV^{-1})e^{-YA(U)}\) at a stationary field deduction. By §3.4 the composite with Bałaban's gauge-fixing factors has the same \(g^0\) density up to field-independent factors. So the constant-flux calculation \(D_{\rm hard}\) is \(\mathfrak D_n\) at the stationary backgrounds it uses (zero and constant Cartan flux, where the multiplier term of (1.5) vanishes), relative to the same coarse Haar measure. The readout the constant-flux calculation §3 uses is "the transverse \(p^2\) coefficient" of the zero-field Hessian, identified "with the off-diagonal spatial moment of CMP109 (1.22)" with "native \(\beta=4Nc\)", i.e. \(\tilde{\mathcal P}\). deduction for the algebra; the evaluation at nonzero quantized flux and its reduction to the zero-field second moment are part of the constant-flux calculation computation, i.e. of (G-val), not of the seam.

## 4. The Transport Lemma (proof of Theorem S, part 3)

### 4.1 Setting

Fine lattice \(\mathbb Z^d\) (scale \(m\)), coarse lattice \(L\mathbb Z^d\) (scale \(m+1\)), \(L\) odd. Bond fields \(a_\nu(x)\) at flat background, colour-diagonal (at \(U=1\) all Hessians are \(\delta^{ab}\otimes\) a real kernel, by colour invariance, CMP109 p.264 argument after (1.20)). \(Q\) is the linearisation at \(1\) of the average (0.12) with the contour families \(G(y,x)\) of p.252:
\[
(Qa)(c)=L^{-d}\sum_{x\in B(c_-)}\Big[\overline{\ell}(c_-\!\to x)+\ell(x\to x')-\overline{\ell}(c_+\!\to x')\Big],\qquad x'=x+Le_\mu,
\]
with \(\ell\) the line sum and \(\overline\ell\) its average over \(G\). \(\Psi_m:=M^m\circ U_{m+1}\) is the map from scale-\(m+1\) data to the scale-\(m\) field \(V^{(m)}\) of (2.3) ("\(V^{(k)}=\bar U^k_{k+1}=M^k(U_{k+1})\)", p.265, source); \(U_{m+1}=U_m\circ\Psi_m\) (p.265, "\(U_k(V'V^{(k)})=U'_k(V')U_{k+1}\)" at \(V'=1\)). Its linearisation \(D:=D\Psi_m(1)\) is the constrained minimiser of \(K:=\operatorname{Hess}(A\circ U_m)(1)\) on \(\{Qa=\alpha\}\), in the axial representative (2.2)–(2.3).

**Inputs (flat background only).**
- **(F-a)** \(K\) and \(H_G:=\operatorname{Hess}G(1)\), for \(G\) gauge-invariant, Euclidean-covariant and localised, are translation invariant, annihilate lattice gradients \(\nabla\chi\) (gauge invariance), are invariant under lattice reflections, and have exponentially decaying kernels. source: (1.19) and p.263 (gauge and Euclidean invariance), the localised representations (1.7), and for \(K\) CMP96 Prop. 2.5 (decay of the flat minimiser and propagator, constants \(d,L\) only; stated by the native estimate §1.8.6).
- **(F-b)** \(\hat K(p)\) is positive definite on vectors orthogonal to the gradient symbol \(\hat e(p)\), for \(p\notin2\pi\mathbb Z^d\). Proof deduction: Jensen. For any fine \(a\) with \(Qa=b\), the coarse curl is \((db)(p')=L^{-d}\sum_{x}\Phi_x\), where \(\Phi_x\) is the flux of \(a\) through the \(L\times L\) square based at \(x\) (the contour pieces \(c_-\!\to x\) of adjacent coarse bonds cancel, since both are averages over the same block with the same families). (For the four bonds of \(p'\) the averaged contour pieces cancel pairwise after the substitution \(x\to x+Le_\mu\), by translation covariance of the families.) Jensen and Cauchy–Schwarz give \(|db(p')|^2\le L^{-d}\sum_x|\Phi_x|^2\le L^{2-d}\sum_x\sum_{q\in{\rm sq}(x)}|da(q)|^2\). Each fine plaquette lies in exactly \(L^2\) of the pairs \((p',x)\) (in-plane offsets; the transverse coordinates of \(x\), hence its block and \(p'\), are then determined). Summing, \(\|db\|^2\le L^{4-d}\|da\|^2\), i.e. \(\|db\|^2\le\|da\|^2\) in \(d=4\). So \(K\ge L^{d-4}K_0\), the scale-\(m\) Wilson form, whose transverse symbol \(\sum_\mu4\sin^2(p_\mu/2)\) is positive off \(2\pi\mathbb Z^d\).
- **(F-c)** \(G'(1)=0\): a colour-invariant linear functional on adjoint-valued fields vanishes (the adjoint representation has no invariant vector). Hence \(\operatorname{Hess}(G\circ\Psi_m)(1)=D^{\!\top}H_GD\).

### 4.2 Statement and proof

> **Lemma T.** Under (F-a)–(F-c), write \(\hat H_G(p)=c_G(|p|^2\delta-pp^\top)+O(|p|^4)\) and \(\hat K(p)=c_K(\cdots)+O(|p|^4)\). Then the coarse kernel \(D^{\!\top}H_GD\) has transverse \(q^2\) coefficient \(L^{d-4}c_G\) (coarse units \(q=Lk\)), for **every** gauge-invariant \(G\). In particular
> \[
> \tilde{\mathcal P}_{m+1}[G\circ\Psi_m]=\tilde{\mathcal P}_m[G],
> \]
> and in \(d=4\) also \(\mathcal P_{m+1}[G\circ\Psi_m]=\mathcal P_m[G]\) without normalisation.

*Step 0 (form of the symbols).* Gauge invariance gives \(\hat H(p)\hat e(p)=0\), \(\hat e_\mu(p)=e^{ip_\mu}-1=ip_\mu+O(p^2)\). Point reflection is a lattice symmetry, so \(\hat H\) is even. Hence \(\hat H(p)=H_2(p)+O(p^4)\) with \(H_2\) quadratic, \(H_2(p)p=0\). The general hypercubic-covariant symmetric quadratic tensor is \(a|p|^2\delta_{\mu\nu}+b\,p_\mu p_\nu+e\,\delta_{\mu\nu}p_\mu^2\). The Ward condition gives \((a+b)|p|^2p_\nu+e\,p_\nu^3=0\) for all \(p\), so \(e=0\), \(b=-a\). So \(\hat H(p)=c(|p|^2\delta-pp^\top)+O(p^4)\), and the second moment (1.22) is \(-\partial_\mu\partial_\nu\hat H_{\mu\nu}(0)=c\) for \(\mu\ne\nu\). Base-point versus mid-point phase conventions change \(\hat H\) by factors \(1+O(p)\), which do not affect the \(p^2\) coefficient because \(\hat H=O(p^2)\).

*Step 1 (Bloch form).* For a coarse plane wave \(a(c)=\alpha e^{ik\cdot y}\) (\(k\in(-\pi/L,\pi/L]^d\) in fine units), \(Da=\sum_{n\in\mathbb Z_L^d}\varphi_ne^{ik_n\cdot x}\), \(k_n=k+2\pi n/L\). The minimiser satisfies the KKT system \(\hat K(k_n)\varphi_n=\hat q_n(k)^\dagger\lambda\) for each alias \(n\), and \(\sum_n\hat q_n(k)\varphi_n=\alpha\), where \(\hat q_n(k)\) is the Bloch symbol of \(Q\). The coarse kernel is \(\widehat{D^\top H_GD}(k)[\alpha,\alpha]=L^d\sum_n\varphi_n^\dagger\hat H_G(k_n)\varphi_n\). Changing the internal-gauge representative adds \(\hat e(k_n)\chi_n\) with \(\sum_n\chi_n=0\) and changes nothing, since \(\hat H_G\hat e=0\).

*Step 2 (the multiplier is \(O(k^2)\)).* The coarse kernel is gauge invariant, so it suffices to take \(\alpha\perp\hat e'(k)\) (transverse). Work in the representative orthogonal to internal gauge directions (any other representative gives the same values). Then \(\varphi\) is bounded uniformly as \(k\to0\). The only direction in which the KKT system degenerates is the coarse-gauge direction \(g_c=(\hat e(k_n)\chi_n)\), \(\sum\chi_n=1\), whose \(Q\)-image is \(\hat e'(k)\). Its coefficient is fixed by the \(\hat e'(k)\)-component of \(\alpha-Q\varphi_\perp\), which is \(O(k)\cdot O(1)\), divided by \(|\hat e'(k)|\asymp k\). For \(n=0\): \(|\hat q_0(k)^\dagger\lambda|=|\hat K(k)\varphi_0|\le C|k|^2\). \(\hat q_0(0)\) acts on constant fine fields as \(L\cdot\mathrm{Id}\) (line sum over \(L\) bonds), so it is invertible near \(k=0\) and \(\lambda=O(k^2)\).

*Step 3 (aliases are gauge up to \(O(k^2)\)).* For \(n\ne0\), \(k_n\) stays away from \(2\pi\mathbb Z^d\), so by (F-b) \(\hat K(k_n)\) is invertible on \(\hat e(k_n)^\perp\) with a uniform bound. From \(\hat K(k_n)\varphi_n=\hat q_n^\dagger\lambda=O(k^2)\): \(\varphi_n=\hat e(k_n)s_n+O(k^2)\). Therefore \(\varphi_n^\dagger\hat H_G(k_n)\varphi_n=O(k^4)\) for every gauge-invariant \(H_G\).

*Step 4 (the principal alias).* From the constraint and Step 3, \(\hat q_0(k)\varphi_0=\alpha-\sum_{n\ne0}\hat q_n\hat e(k_n)s_n+O(k^2)\). \(Q\) maps fine gradients to coarse gradients, so the sum is along the coarse gradient symbol and contributes to \(\varphi_0\) only a multiple of \(\hat e(k)\), which \(\hat H_G\) kills. So \(\varphi_0=\alpha/L+\hat e(k)t+O(k)\), and \(\varphi_0^\dagger\hat H_G(k)\varphi_0=L^{-2}\alpha^\dagger\hat H_G(k)\alpha+O(k^3)\). With \(L^d\) from Parseval and \(q=Lk\): the coarse transverse coefficient is \(L^{d}\cdot L^{-2}\cdot c_G\cdot L^{-2}=L^{d-4}c_G\).

*Step 5.* Apply Steps 1–4 to \(G\) and to \(G=A\circ U_m\) (for which \(H_G=K\), and \(A\circ U_{m+1}=(A\circ U_m)\circ\Psi_m\) by the composite-minimiser property). The ratio gives the normalised statement. \(\square\)

> **Corollary 4.3.** \(\mathcal P_m[A\circ U_m]=\mathcal P_0[A]\) for all \(m\) (\(d=4\)). So the normalisation \(\mathcal PA=1\) of C2 §1.1 is a single convention, exactly scale independent, not a consequence to be extracted from CMP109 (4.38)–(4.42), (5.42).

> **Corollary 4.4 (Theorem S, part 3).** For \(k<n\), iterate Lemma T with \(G=\log Z^{(k)}\circ U_m\), \(m=k+1,\dots,n-1\), using \(U_{m+1}=U_m\circ\Psi_m\). The hypotheses hold for each \(m\): \(\log Z^{(k)}\) is gauge invariant and Euclidean covariant (p.263) and has a localised expansion (p.261), so its Hessian at flat has an exponentially decaying kernel. Constants may depend on \(m\); only exactness is used. conditional

**Numerical check (§12, item 1).** In \(d=2,3,4\) with \(L=3\) (and \(d=2\), \(L=5\)), with the actual linearised (0.12) including the permutation contour families, a non-Wilson classical form \(K\), and a gauge-invariant \(H_G\) containing a \(p^4\) term: \(c_{\rm coarse}[K]/L^{d-4}=1.000000\), \(c_{\rm coarse}[H_G]/(L^{d-4}c_G)=1.000000\), identical in the minimal-norm and in an axial-like representative. The non-gauge part of the alias components is \(O(k^3)\). A non-gauge-invariant control form is representative-dependent and is not transported (its "coefficient" is \(6\times10^4\) in the axial-like representative in \(d=4\)). This shows that gauge invariance of \(G\) is what removes the aliases.

**What this replaces.** N2 H.1 item 2 and the constant-flux calculation Lemma 1.6.1 asserted transport via "stationary affine reproduction" (constant-curvature data; per-volume \(F^2\) coefficients). That route needs quantized flux on a periodic torus and an interchange of limits that was not written. Lemma T needs only the flat Hessians and the KKT structure.

## 6. The transient, and the coordinate

Write \(D^G_i:=\sum_{k<i}d^G_k\) and \(b_i:=D^G_i-d_Bi\). (G-val) says \(|b_i|\le B_G\). The actual recursion gives \(Y_{i+1}=Y_i-p_{i+1}\). Theorems B′, C′ (with (C2\(^*\)) and the R-mismatch) give \(p_{i+1}=d^G_i+\epsilon_i\), \(|\epsilon_i|\le C/Y_i\). Then, for \(y_i:=Y_i+b_i\),
\[
y_{i+1}=y_i-d_B-\epsilon_i\qquad\text{exactly},
\]
because \(b_{i+1}-b_i=d^G_i-d_B\). For \(y_i\ge2B_G\), \(Y_i\ge y_i/2\), so \(|\epsilon_i|\le2C/y_i\). In the ultraviolet indexing \(v_m=1/y_{K-m}\):
\[
v_{m+1}=v_m-d_Bv_m^2+r_m,\qquad r_m=-\epsilon v_m^2+\frac{s^2v_m^3}{1+sv_m},\quad s=d_B+\epsilon,\quad |r_m|\le Av_m^3.
\]
deduction given the inputs; one may take \(A=2C+2(d_B+2C)^2\) for \(v_m(d_B+2C)\le\frac12\). Consequences:

- \(b=d_B\) is the asymptotic value. The transient is absorbed **exactly** into a deterministic, coupling-independent, history-independent shift of the coordinate. It is not in \(r_m\).
- Only **boundedness** of \(b_i\) is needed, not convergence and not a per-step sign. The numerical check (§12 item 4) uses a bounded non-convergent transient: \(\sup|r|/v^3=6.6\) in the shifted coordinate, while the unshifted \(1/Y\) gives \(\sup|r|/u^3\approx1.5\times10^3\), growing with \(Y\).
- If one wants a \(k\)-independent coordinate \(u=1/(Y+b_\infty)\), one needs \(|d^G_i-d_B|\le C/Y_i\), e.g. geometric convergence of \(d^G_i\) (route R2 (i)). That is stronger than (G-val) and not available.

## 7. (S4)(ii)–(iii): only the flat background is needed

C2 uses (S4) in Lemma 4.5 (insertions \(\partial^\beta M\) and tangents), Proposition 4.6 and Lemma 4.7. Every derivative there is taken **at \(u=0\)**:
- the cumulant expansion of \(\partial_s^2\partial_{u_x}\partial_{u_0}\log Z\) is evaluated at \(u=0\), with the law \(\mu_s\) at \(u=0\);
- the Gaussian insertions are \(\partial^\beta M(0)\), \(\beta\subset\{\mathsf x,\mathsf 0\}\);
- the inherited and explicit insertions need Cauchy on the absolute domains (S2), (S3) and the tangents \(\partial_{u_x}U_{k+1}\), \(\partial_{u_x}\partial_{u_y}U_{k+1}\) at \(u=0\);
- Lemma 4.7 step 3 needs the same tangents at flat.

So (S4) reduces to:
- **(S4)(i)₀**: \(M(0)\ge\gamma_0\), \(\gamma_0=\gamma_0(d,L)\). CMP96 Lemma 2.4 and its consequence p.246 (proved in the source, stated by the native estimate §1.8.6) give it for the \(\delta\)-axial gauge. CMP109 p.267 identifies \(\Delta^{(k)}\) with CMP99 (3.156) "with the \(\delta\)-function gauge fixing term replaced by the exponential one", and CMP99 p.428 asserts \(\gamma_0\) for \(C^*\Delta_kC\). The transfer: write \(B=B_{\rm ax}+\nabla_{\rm int}\omega\); the physical form sees only \(B_{\rm ax}\), and \(G^{(2)}\) controls \(\omega\) through the bounded triangular axial map. It is sketched here, not written in detail. conditional; additional assumption
- **(S4)(ii)₀**: exponential decay of \(M(0)\), \(\partial_uM(0)\), \(\partial_u^2M(0)\) from the derivative sites. At flat, \(\partial_u\) of a propagator is \(-G\,(\partial_u\Delta)\,G\), with \(G\) the flat propagator (CMP96 Prop. 2.5: "satisfies all the inequalities (1.110)–(1.114) of the Proposition 1.2 with a positive constant \(\delta_2\) … depends on \(d\) and \(L\) only", stated by the comparison argument) and \(\partial_u\Delta\) a local vertex. Second derivatives come from the resolvent identity once more. Decay from the derivative site follows from the decay of each factor. conditional on flat source statements.
- **(S4)(iii)₀**: the first tangent at flat is the flat linearised minimiser (CMP96, flat; CMP99 p.399: "the theorems are reduced to the corresponding theorems for propagators without external gauge field. They were proved in [4]"). The second tangent at flat is \(-\mathfrak G_0\,V_3(D\Psi e_x,D\Psi e_y)\) by implicit differentiation, with \(\mathfrak G_0\) the flat constrained propagator (CMP99 Thm 3.13 at \(U=1\), Thm 3.15) and \(V_3\) the local cubic vertex. conditional

**Not written here:** the depth-uniform bookkeeping of the fine-lattice vertex factors (\(\eta\)-scalings of \(\Delta_1\), \(H_{1,k}\) and their derivatives, which CMP99 (3.42)–(3.47) and CMP102 (190) record in scaled norms) at \(U=1\). Every constant involved is a flat-background constant depending on \(d,L\) only. **Consequence:** CMP102 (190) at general backgrounds, and its replacement T′♯ of C05 Source operators for the deformed reconstruction, are **not** inputs of (C2). They remain inputs of (S3) and of the locality theorem.

## 11. The B-part restriction on the tilde spaces

**What the source says.**
- CMP119 p.276 (source): "The expression determined by the boundary terms \(\mathbf B_k\) is much simpler to deal with. To its terms we apply the formulas (3.6), (3.7) [I], and next we localize the obtained expressions. … Terms of this expansion can be extended [as in (I.3.13)] to analytic functions defined on the corresponding spaces (3.43)."
- (3.43) is \(\tilde{\mathbf U}^c_{k+1}(Y,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\times\{A:\operatorname{supp}A\subset Y\cap\Lambda^{(k)*}_{k+1},|A|<C_1p_1(g_k)\}\).
- p.277 (source, consistent with the image of p.276): "on the domain \(\Omega^c_{k+1}\) there is no regularity improvement of the configuration \(U_{k+1}\), on the other hand we have to use a part of the analyticity domains of terms in \(\mathbf B_k\) for the function \(\mathbf H_k\). This is the reason for putting the powers of 1/2 in the conditions (2.36)–(2.39). The analyticity domains become smaller after each step, but the difference is very small and exponentially decreasing in the number of steps. The localization of the fluctuation field, and the exponential decay of the minimizing function \(\mathbf H_k\) imply that this difference is still much greater than bounds on this function."
- The tilde spaces (CMP119 p.261, source) impose (2.34)–(2.37), including the reconstructed configurations \(U_{p,x}(M^\cdot(\mathbf U))\), "on \(X\cap(\Omega_n\setminus\Omega_{n+1})\) for \(n=1,\dots,j-1\), or on \(X\cap\Omega_j\) for \(n=j\)", with margins \((1-\beta(1-2^{-(j-n)}))\alpha_{0,n}\).

**Assessment.**

1. The regions are the layers of the **common** sequence \(\{\Omega_j\}\), not "\(X\) minus two layers of \(X\)'s own cubes". So the non-nesting of literal regions that forced the level-adapted restriction (CMP109 clause (iv)) does not occur in the same form: all B-terms of a step see the same layers. additional assumption
2. What is needed instead is a per-layer smallness statement:

   > **(BL)** For \((\mathbf U,\mathbf J,A)\) in (3.43), the configuration \(\exp i\xi\mathbf H_j(B(t))U_{k+1}\) of CMP109 (3.6), and its level-\(p\) reconstructions, differ from those of the background on \(X\cap(\Omega_n\setminus\Omega_{n+1})\) by at most \(\beta2^{-(k+1-n)}\alpha_{0,n}\) in the norms of (2.34)–(2.37), for every \(n\le k\).

   Then the margin consumed at step \(k\) at level \(n\) fits the budget \(\beta2^{-(k+1-n)}\), and the margins telescope to at most \(\beta\).
3. **Is (BL) plausible?** A fluctuation localised in \(\Omega_{k+1}\) reaches the layer \(\Omega_n\setminus\Omega_{n+1}\) only through the layers \(n+1,\dots,k\). If each layer \(m\), of width \(\gtrsim MR_m\) cubes of its own scale, contributes a factor \(e^{-cMR_m}\le e^{-cM}\le\frac14\), the displacement is \(\le\varepsilon_k\prod_me^{-cMR_m}\ll2^{-(k-n)}\alpha_{0,n}\). That is a **multiscale** decay estimate. It is what CMP99 Theorems 3.7–3.10 "in their full generality" (CMP119 p.276) provide for propagators; the minimiser version is CMP102 Proposition 9 on sequences \(\{\Omega_j\}\).
4. **Not covered by the locality theorem.** The locality theorem ([Locality](locality.md), Theorem 4.1) compares reconstructions on nested single domains \(Z\subset Z'\). It does not give the per-layer factor. The CR theorem gives absolute bounds (\(K_c(\cdot)\xi^2\)), not the \(2^{-(k-n)}\) budget.

**Hypotheses:** (BL) is additional assumption, with Bałaban's assertion source input. It is the precise residual for the B-part of (F1). B-terms are attached to large-field regions (CMP119 (2.41), p.261 image: "the sum is over domains \(X\in\mathbf D_j\) such, that \(X\cap\Omega_j\ne\emptyset\), and \(X\cap Z_j^\sim\ne\emptyset\)"), so they do not enter the projection \(p_{k+1}\) of the whole-lattice regular sector (F2) (reading, additional assumption). They enter B-03 only through admission and (F1)'s uniform bounds. So (BL) affects the remainder bound's validity, not the coefficient.
