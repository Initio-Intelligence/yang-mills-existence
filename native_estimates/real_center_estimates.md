# The complex extension centered at real data

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

**Local convention.** Work about a fixed real center. Complex representatives of the same orbit need not agree as axial-gauge representatives; use the center-relative bounds in [Complex reconstruction](complex_reconstruction.md).

## 1. What "reconstruction from complex data" means in the source

**CMP109 p.262, clause (iv)** source: "We consider \(X\) as \(\Omega_0\), and we construct the sequence \(\{\Omega_n\}\) … of maximal possible domains … we construct the functions \(U_n(V)\) in the axial gauges, for regular \(G^c\)-valued configurations \(V\). We consider the pair \((U_n(M'(\mathbf U)),J_n(M'(\mathbf U)))\) … where \(M'(\mathbf U,b)=M^p(\mathbf U,b)=\bar{\mathbf U}^p(b)\) for \(b\in\Lambda_p\)". The complex reconstruction is therefore [V]'s \(U_k\) (with \(k=n\), \(\Omega_0=X\)) evaluated at complex data.

**[V] Proposition 9** source: "The minimal configuration \(U_k(V)=U_k(V'V_0)\) in the axial gauge has an extension to an analytic function of \(G^c\)-valued small configurations \(V'\) on \(\mathfrak B_k\). It can be extended further to all orbits of such configurations \(V'V_0\) by the equality (181). The function \(U_k(V'V_0)U_k(V_0)^{-1}\) transformed to the Landau gauge is, by the definition, equal to \(\exp i\eta\mathscr H(B)\), where \(B=1/i\log V'\). … It satisfies the conditions (19)–(21) with \(\varepsilon_2=B_5\varepsilon_1\)". "Small" is (172), p.305 (source): "\(V=V'V_0\), \(V_0\) satisfies the condition (7), \(V'\) satisfies \(\lvert V'-1\rvert<C_1\varepsilon_1\), hence \(V'=e^{iB'}\), \(\lvert B'\rvert<2C_1\varepsilon_1\) on \(\mathfrak B_k\), for \(\varepsilon_1\) sufficiently small." P.307 (source, matches p.309's summary): "It is an analytic function of \(V'\) … and for \(V'\) with values in \(G\) it coincides with the minimal configuration constructed in the previous sections."

**[V] Theorem 1** (source input; p.279): "There exist positive constants \(a_0,a_1,B_3,\dots\) such that for an arbitrary configuration \(V\) satisfying (7) with \(\varepsilon_1<a_1\) there exists a minimal orbit in the space \(\mathfrak U_k(\{\Omega_j\},B_3\varepsilon_1)\cap\mathfrak B_k(\mathfrak B_k,V)\)", where (2): \(\lvert\partial U(p)-1\rvert<\varepsilon_0L^{-2j}\), \(\lvert(D^{\eta*}\partial U)(b)\rvert<\varepsilon_0\eta^2(L^j\eta)^{-3}\) on \(\Omega_j\), \(\eta=L^{-k}\).

**Two remarks.** (i) Theorem 1 and Proposition 9 hold for every \(\varepsilon_1\) below an absolute ceiling; if \(V_0\) satisfies (7) with a small \(\varepsilon_1\) it satisfies it with any larger one. The tube \(\lvert V'-1\rvert<C_1\varepsilon_1\) is therefore available with \(\varepsilon_1\) **absolute**, at the price of a crude output bound \(B_5\varepsilon_1\). CMP109 p.263 instead took \(\varepsilon_1=2\alpha_0'(L^p\xi)^2\), and with that choice the complex data are outside the tube (analysis §2.6). (ii) The extension "to all orbits by (181)" and single-valuedness are asserted, not argued; Lemma 2.1 below proves single-valuedness on the union of absolute tubes, which is all that is needed.

**Units.** CMP109: fine spacing \(\xi\), level-\(p\) block size \(\ell_p:=L^p\xi\le\ell_n\) (\(p\le n\)). [V] with \(k=n\): \(\eta=L^{-n}=\xi/\ell_n\). Plaquette deviations are dimensionless: a [V]-bound \(\varepsilon L^{-2n}\) on \(\Omega_n\) equals \(\varepsilon\,\ell_n^{-2}\xi^2\). Level-\(p\) data of a fine configuration with curvature \(\kappa\) (i.e. \(\lvert\partial-1\rvert\le\kappa\xi^2\)) have plaquettes \(\le2\kappa\ell_p^2\) ([A] Proposition 2, as quoted in [R] p.87: "the bounds \(\lvert\partial U-1\rvert<\alpha_0\eta^2\) imply \(\lvert\partial\bar U^j-1\rvert<\dots<2\alpha_0L^{2j}\eta^2\)"; and CMP109 p.263: "\(\lvert\partial\bar{\mathbf U}^p-1\rvert<2\alpha_0'(L^p\xi)^2\)"). For data from one fine configuration the mixed plaquettes of (7) are plaquettes of \(\bar U^p\) (the averages are iterated, [A] (43)), so (7) holds with \(\varepsilon_1=2\kappa\ell_n^2\).

**Notation for this derivation.** \(\mathbf U=e^{i\xi A'}U\), \(U\) unitary, \(A'=A'_R+iA'_I\) with \(A'_R,A'_I\) hermitian (\(\lvert A'_R\rvert,\lvert A'_I\rvert\le\lvert A'\rvert\), operator norm). \(a_1:=\sup_Z\lvert A'\rvert\); \(a_c:=\sup_{p\subset Z}\lvert\partial\mathbf U(p)-1\rvert/\xi^2\) (clause (iii) of CMP109 gives \(a_c<\alpha_0\)). The **real slice** is \(\mathbf U_t:=e^{i\xi(A'_R+tA'_I)}U\), \(t\in\mathbb C\): unitary for real \(t\), \(\mathbf U_i=\mathbf U\).

## 2. Lemmas

Absolute constants of the sources: \(B_3,B_5,C_1\) ([V]), \(\varepsilon_9\le a_1^{[V]}\) the ceiling on \(\varepsilon_1\) in Proposition 9, \(c_3\) ([A] (131)), \(d\). Fix
\[
\varepsilon^\sharp:=\varepsilon_9/8,\qquad\text{and assume }C_1\varepsilon^\sharp\le\tfrac1{10},\ 16dB_5\varepsilon^\sharp\le\tfrac14,\ B_5\varepsilon^\sharp\le\tfrac1{16}.
\]
(These only shrink \(\varepsilon^\sharp\).)

### 2.1 Single-valued complex reconstruction on the union of absolute tubes

For real data \(V_0\) satisfying (7) with \(\varepsilon^\sharp\) put \(T(V_0):=\{e^{iB'}V_0:\lvert B'\rvert_\infty<\tfrac12C_1\varepsilon^\sharp\}\) (convex in \(B'\), contained in Proposition 9's domain since \(e^{\lvert B'\rvert}-1<C_1\varepsilon^\sharp\)), and let \(E_{V_0}\) be Proposition 9's extension on it. \(\mathcal D:=\bigcup_{V_0}T(V_0)\).

> **Lemma 2.1.** The \(E_{V_0}\) agree on overlaps; they define one holomorphic map \(U^c\) on \(\mathcal D\), equal to the axial minimiser at real data. conditional on Proposition 9 at \(\varepsilon_1=8\varepsilon^\sharp=\varepsilon_9\).

*Proof.* Let \(V\in T(V_0)\cap T(V_1)\), \(V=e^{iB'}V_0=e^{iB''}V_1\). Then \(\lvert V_1V_0^{-1}-1\rvert\le e^{C_1\varepsilon^\sharp}-1\le2C_1\varepsilon^\sharp\), and every \(W=e^{iB'''}V_1\in T(V_1)\) has \(\lvert WV_0^{-1}-1\rvert\le e^{\frac52C_1\varepsilon^\sharp}-1<3C_1\varepsilon^\sharp<8C_1\varepsilon^\sharp\). So \(T(V_1)\) lies in the domain of the extension \(E^\flat_{V_0}\) of Proposition 9 at \(\varepsilon_1=8\varepsilon^\sharp\) (\(V_0\) satisfies (7) with \(\varepsilon^\sharp\le8\varepsilon^\sharp\)). On the real points of \(T(V_1)\) (unitary \(e^{iB'''}\)) both \(E^\flat_{V_0}\) and \(E_{V_1}\) equal the minimiser (p.307 quote; uniqueness of the critical orbit, Theorem 1, and of its axial representative). The real points form a totally real submanifold of maximal dimension of the connected open set \(T(V_1)\); by the identity theorem \(E^\flat_{V_0}=E_{V_1}\) on \(T(V_1)\). Likewise \(E^\flat_{V_0}=E_{V_0}\) on \(T(V_0)\). Evaluate at \(V\). \(\square\)

So on \(\mathcal D\) the source's object is unambiguous; outside \(\mathcal D\) nothing is used.

### 2.2 Two constants with a slit

> **Lemma 2.2.** Let \(f\) be holomorphic on a neighbourhood of \(\bar D(0,T)\), \(T\ge2\), with values in a normed space, \(\lVert f\rVert\le M\) on \(D(0,T)\) and \(\lVert f\rVert\le m\le M\) on \([-1,1]\). Then \(\lVert f(i)\rVert\le m\,(M/m)^{\theta}\), \(\theta\le\log(1+\sqrt2)/\log T\).

*Proof.* \(J(w)=\frac12(w+w^{-1})\) maps \(\{\lvert w\rvert>1\}\) onto \(\mathbb C\setminus[-1,1]\) and \(\{1<\lvert w\rvert<R\}\) into \(D(0,T)\setminus[-1,1]\) for \(R+R^{-1}=2T\) (\(R\ge T\)). \(u=\log\lVert f\circ J\rVert\) is subharmonic, \(\le\log m\) on \(\lvert w\rvert=1\) (continuity across the slit), \(\le\log M\) on \(\lvert w\rvert=R\). Compare with the harmonic \(h=\omega\log m+(1-\omega)\log M\), \(\omega(w)=\log(R/\lvert w\rvert)/\log R\). \(J^{-1}(i)=i(1+\sqrt2)\), so \(1-\omega=\log(1+\sqrt2)/\log R\). \(\square\)

### 2.3 The real slice is controlled by the complex curvature

> **Lemma 2.4.** Assume \(\lvert\partial U-1\rvert\le0.05\), \(\xi a_1\le\frac1{128}\), \(a_c\xi^2\le\frac12\). For real \(t\) with \(32\xi a_1(1+\lvert t\rvert)\le1\), the unitary configuration \(\mathbf U_t\) satisfies on \(Z\)
> \[
> \lvert\partial\mathbf U_t-1\rvert\le\hat\kappa(t)\,\xi^2,\qquad\hat\kappa(t):=2(1+\lvert t\rvert)a_c+344(1+\lvert t\rvert)^2a_1^2.
> \]

*Proof.* Fix \(p\). \(X(t):=\partial\mathbf U_t(p)\) is entire. For \(\lvert t\rvert\le\rho:=1/(16\xi a_1)\) each link factor has \(\lvert e^{i\xi(A'_R+tA'_I)}-1\rvert\le e^{0.07}-1\le0.073\), so \(\lvert X(t)-\partial U(p)\rvert\le1.073^4-1\le0.33\) and \(\lvert X(t)-1\rvert\le0.4\). Hence \(\Psi(t):=(i\xi^2)^{-1}\log X(t)\) is holomorphic on \(D(0,\rho)\) with \(\xi^2\lvert\Psi\rvert\le0.67\); Cauchy gives \(\lvert\psi_k\rvert\le0.67\,\xi^{-2}(16\xi a_1)^k\) for the Taylor coefficients, in particular \(\lvert\psi_2\rvert\le172a_1^2\). For real \(t\), \(X(t)\) is unitary near \(1\), so \(\Psi(t)\) is hermitian and so are all \(\psi_k\). Write \(\Psi(i)=H+iO\) with \(H=\sum_{k\,\rm even}(-1)^{k/2}\psi_k\), \(O=\sum_{k\,\rm odd}(-1)^{(k-1)/2}\psi_k\) hermitian; then \(\lvert H\rvert,\lvert O\rvert\le\lvert\Psi(i)\rvert\le2a_c\) (real and imaginary parts of a matrix have norm \(\le\) its norm; \(\lvert\log(1+Y)\rvert\le2\lvert Y\rvert\) for \(\lvert Y\rvert\le\frac12\)). For real \(t\),
\(\Psi(t)=H+tO+\sum_{k\ge2}\psi_k(t^k+c_k(t))\) with \(\lvert t^k+c_k(t)\rvert\le(1+\lvert t\rvert)^k\). With \(q=16\xi a_1(1+\lvert t\rvert)\le\frac12\): \(\sum_{k\ge2}\lvert\psi_k\rvert(1+\lvert t\rvert)^k\le172a_1^2(1+\lvert t\rvert)^2(1+2q)\le344a_1^2(1+\lvert t\rvert)^2\). Finally \(\lvert e^{i\xi^2\Psi}-1\rvert\le\xi^2\lvert\Psi\rvert\) for hermitian \(\Psi\). \(\square\)

The \(a_1^2\) term is genuine: the stress test of §10 builds plaquettes with \(a_c=0\) exactly and finds real-slice curvature \(\approx1.5(1+\lvert t\rvert)^2a_1^2\) (the constant 344 is crude). Physically: \(F_{\rm real}-[A_I,A_I]\) small does not make \(F_{\rm real}\) small.

### 2.4 The family stays in \(\mathcal D\)

> **Lemma 2.5.** Assume Lemma 2.4's hypotheses, and let \(r\in\mathbb R\) satisfy \(32\xi a_1(1+\lvert r\rvert)\le1\), \(2\hat\kappa(r)\ell_n^2\le\varepsilon^\sharp\). Then \(V_0(r):=M'(\mathbf U_r)\) satisfies (7) with \(\varepsilon^\sharp\), and \(M'(\mathbf U_t)\in T(V_0(r))\) for \(\lvert t-r\rvert<T_s:=C_1\varepsilon^\sharp/(64a_1\ell_n)\). conditional on [A] Propositions 2, 4, 6, 7.

*Proof.* (7): Lemma 2.4 and [A] Proposition 2 (§1). Tube: \(\mathbf U_t=e^{i\xi X}\mathbf U_r\) with \(X=(i\xi)^{-1}\log(e^{i\xi(A'_R+tA'_I)}e^{-i\xi(A'_R+rA'_I)})\). For fixed \(P\), \(\lvert P\rvert\le\frac14\), \(g(\Delta):=e^Pe^{-P+\Delta}-1\) vanishes at \(\Delta=0\) and is bounded by \(4\) on \(\lvert\Delta\rvert\le\frac12\), so \(\lvert g(\Delta)\rvert\le8\lvert\Delta\rvert\) and \(\lvert\log(1+g)\rvert\le16\lvert\Delta\rvert\) when \(8\lvert\Delta\rvert\le\frac12\); with \(\Delta=i\xi(t-r)A'_I\): \(\lvert X\rvert\le16\lvert t-r\rvert a_1\). [A] Proposition 4, (131) (c)\rvert<\dots<2\alpha_1\)", with \(Q_j(U_0,\eta A)=\frac1i\log\bar U_1^j\) the relative average), valid for complex \(A\) by Propositions 6–7 (c) is an analytic function of \(A'\) for \(A'\) with values in the complexified algebra … Proposition 4 holds uniformly in \(A'\)"), after rescaling the top level to unit size, gives \(\lvert\log(\bar{\mathbf U}_t^p(\bar{\mathbf U}_r^p)^{-1})\rvert\le2\ell_p\lvert X\rvert\le32\ell_n\lvert t-r\rvert a_1<\frac12C_1\varepsilon^\sharp\). The hypothesis of (131) (\(\ell_n\lvert X\rvert\le c_3/2\)) holds since \(C_1\varepsilon^\sharp\le c_3\) may be assumed. \(\square\)

### 2.5 Crude bound on the tube

> **Lemma 2.6.** Under Lemma 2.5, for \(\lvert t-r\rvert<T_s\) and every plaquette \(p\subset\Omega_n\) and bond \(b\subset\Omega_n\):
> \[
> \lvert\partial U^c(M'(\mathbf U_t))(p)-1\rvert\le M_{\rm p}:=2(2B_3+3B_5)\,\varepsilon^\sharp L^{-2n},\qquad
> \mathcal J(U^c(M'(\mathbf U_t)))(b)\le M_{\rm J}:=2(B_3+2B_5)\,\varepsilon^\sharp ,
> \]
> where \(\mathcal J(W)conditional:=(L^n\eta)^3\eta^{-2}\lvert(D^{\eta*}_W\partial W)(b)\rvert\) (the normalisation of [V] (2)). conditional on Theorem 1, Proposition 9, [R] (1.47)–(1.50), (1.54), (1.70)–(1.72).

*Proof.* By Lemma 2.1, \(U^c(M'(\mathbf U_t))=E_{V_0(r)}(\cdot)=(e^{i\eta\mathscr H}W_r)^u\), \(W_r=U_n(V_0(r))\in\mathfrak U_n(\{\Omega_j\},B_3\varepsilon^\sharp)\) (Theorem 1), \(\mathscr H\) satisfying (19) with \(\varepsilon_2=B_5\varepsilon^\sharp\): \(\lvert\mathscr H\rvert<\varepsilon_2(L^j\eta)^{-1}\), \(\lvert\nabla\mathscr H\rvert<\varepsilon_2(L^j\eta)^{-2}\), \(\lvert D^*D\mathscr H\rvert,\lvert\Delta\mathscr H\rvert<\varepsilon_2(L^j\eta)^{-3}\) on \(\Omega_j\) ([V] p.281, source).
*Plaquette.* [R] (1.21), (1.47), (1.49)–(1.50) (source input; pp.84–85; "this equality holds for arbitrary \(A\) in the complexified Lie algebra"): \((\partial_{W}e^{i\eta\mathscr H})(p)-1=i\eta^2(D\mathscr H)(p)-\frac12\eta^2V_2+O_1(\frac1{3!}\eta^3(\partial\lvert\mathscr H\rvert(p))^3)\), \(\lvert V_2\rvert\le\eta^2\lvert D\mathscr H\rvert^2+12\lvert\mathscr H\rvert^2\). On \(\Omega_n\) this is \(\le(2\varepsilon_2+8\varepsilon_2^2+22\varepsilon_2^3)L^{-2n}\le3\varepsilon_2L^{-2n}\); the full plaquette adds \(\lvert\partial W_r-1\rvert\) times a transport factor \(\le1.21\). 
*Axial gauge.* \(u\) is the transformation of [R] Theorem 4 / (106) of [A]; [R] (1.70)–(1.72) source: "\(\lvert u_1(x)-1\rvert\le2\sum_{n=0}^{j-1}\max\lvert\frac1i\log(\bar R^n_{0,x_{n+1}}\bar U^n_1)(\Gamma_{x_{n+1},x})\rvert\) … \(\le4dB_1(\alpha_0+\alpha_1)L^{n+1-j}\) … \(\lvert u_1(x)-1\rvert<8dB_1(\alpha_0+\alpha_1)\frac1{1-L^{-1}}\le16dB_1(\alpha_0+\alpha_1)\), \(x\in\Omega_0\)", with \(B_1(\alpha_0+\alpha_1)\) the bound on \(\lvert A\rvert\) in (1.69); [V] p.297 (source): "satisfies the bounds (1.70)–(1.74) of that paper, with \(B_1(\alpha_0+\alpha_1)\) replaced by \(\varepsilon_2\)". The sum is geometric because on \(\Omega_j\) the field bound is set by level \(j\) and lower-level averages run over shorter contours; so \(\lvert u-1\rvert\le16d\varepsilon_2\le\frac14\) **uniformly in the number of levels**, and conjugation by \(u(x)\) costs \(\frac{5/4}{3/4}\le2\).
*Current.* [R] (1.54) source: "\(D^{\eta*}_{U_1U_0}\partial U_1U_0=D^{\eta*}_{U_0}\partial U_0+i\eta^2D^{\eta*}_{U_0}D^\eta_{U_0}A+O_1(36d\alpha_2(L^j\eta)^{-1}\lvert\nabla A\rvert\eta^2)+O_1(50d\alpha_2^3(L^j\eta)^{-3}\eta^2)+O_1(10d\alpha_0\alpha_2(L^j\eta)^{-3}\eta^2)\)" with \(\alpha_2=\varepsilon_2\), \(\alpha_0=B_3\varepsilon^\sharp\); the current transforms by \(R(u_-)\) (CMP109 (1.10)), factor \(\le2\). \(\square\)

## 3. The theorem

Set \(K:=4(2B_3+3B_5)/(B_3C_1^2\varepsilon^\sharp)\) (assume \(C_1^2\varepsilon^\sharp\le1\)) and \(T_0:=\max\{e^2,K\}\). **Ceilings** (all absolute):

- (Ce1) \(a_1\ell_n\le C_1\varepsilon^\sharp/(64T_0)\);
- (Ce2) \(2\hat\kappa(T_0)\ell_n^2\le\varepsilon^\sharp\), i.e. \(4(1+T_0)a_c\ell_n^2+688(1+T_0)^2a_1^2\ell_n^2\le\varepsilon^\sharp\);
- (Ce3) \(\lvert\partial U-1\rvert\le0.05\), \(\xi a_1\le\frac1{128}\), \(a_c\xi^2\le\frac12\).

> **Theorem 3.1 (CR).** Let \(Z\) be a domain with its maximal sequence \(\Omega_1(Z)\supset\dots\supset\Omega_n(Z)\) (CMP109 (iv)), \(\mathbf U=e^{i\xi A'}U\) on \(Z\) with \((a_c,a_1)\) as in §1 satisfying (Ce1)–(Ce3). Then \(M'(\mathbf U)\in\mathcal D\), and the source's complex reconstruction \(U_n(Z;M'(\mathbf U))=U^c(M'(\mathbf U))\) satisfies, on \(\Omega_n(Z)\),
> \[
> \lvert\partial U_n(Z;M'(\mathbf U))-1\rvert\le K_c\,(a_c+344a_1^2)\,\xi^2,\qquad
> \mathcal J(U_n(Z;M'(\mathbf U)))\le K_c\,(a_c+344a_1^2)\,\ell_n^2,
> \]
> with \(K_c:=8(1+\sqrt2)^3B_3\le113B_3\) (for the current, \(K_c\) with \(B_3+2B_5\) replacing \(2B_3+3B_5\) inside \(K\); the same value \(113B_3\) suffices). The constants depend on \(d,L\) only, through \(B_3,B_5,C_1,\varepsilon_9,c_3\); not on \(n\), the number of levels, the scale \(s\), \(Z\), \(M\), the torus. On the real part \(U\) the same bounds hold with \(2B_3a\) (Theorem 1, as in CMP109 (1.17)). Since \(\Omega_n(Z)\supseteq Z^{(n)}\) for \(M\ge(1+L)R_1M_1\) (analysis §4.3) and \(\Omega_n(Z)\supseteq\tilde X^{-2}\), this is clause (iv) in either convention. **conditional** on the inputs listed in §2.

*Proof.* Let \(T_r:=\sup\{r\ge0:32\xi a_1(1+r)\le1,\ 2\hat\kappa(r)\ell_n^2\le\varepsilon^\sharp\}\), \(T:=\min\{T_r,T_s\}\). By (Ce1)–(Ce3), \(T\ge T_0\) (for the first condition in \(T_r\): \(32\xi a_1(1+T_s)\le32\xi a_1+\frac12C_1\varepsilon^\sharp\le1\), using \(\xi\le\ell_n\)). For \(\lvert t\rvert<T\) take \(r=\operatorname{Re}t\): Lemma 2.5 gives \(M'(\mathbf U_t)\in T(V_0(r))\subset\mathcal D\). So \(t\mapsto f(t):=\partial U^c(M'(\mathbf U_t))(p)-1\) is holomorphic on \(D(0,T)\) (composition of \(U^c\) with the analytic data map), \(\lVert f\rVert\le M_{\rm p}\) there (Lemma 2.6). For \(t\in[-1,1]\) the data are real and satisfy (7) with \(\varepsilon_1=2\hat\kappa(1)\ell_n^2\); \(U^c\) is the minimiser (Lemma 2.1), so by Theorem 1, \(\lVert f(t)\rVert\le m:=2B_3\hat\kappa(1)\ell_n^2L^{-2n}=2B_3\hat\kappa(1)\xi^2\).
*Ratio.* If \(T=T_s\): \(a_1\ell_n=C_1\varepsilon^\sharp/(64T)\) and \(\hat\kappa(1)\ell_n^2\ge1376a_1^2\ell_n^2\ge C_1^2\varepsilon^{\sharp2}/(3T^2)\), so \(M_{\rm p}/m\le3(2B_3+3B_5)T^2/(B_3C_1^2\varepsilon^\sharp)\le KT^2\). If \(T=T_r\) through its second condition: \(2\hat\kappa(T)\ell_n^2=\varepsilon^\sharp\) and \(\hat\kappa(T)\le\frac12(1+T)^2\hat\kappa(1)\), so \(M_{\rm p}/m\le(2B_3+3B_5)(1+T)^2/B_3\le KT^2\). (The first condition of \(T_r\) is never binding, shown above.)
*Interpolation.* Lemma 2.2: \(\lVert f(i)\rVert\le m(KT^2)^{\log(1+\sqrt2)/\log T}=m\,(1+\sqrt2)^2K^{\log(1+\sqrt2)/\log T}\le(1+\sqrt2)^3m\) since \(T\ge T_0\ge K\) (if \(K<e^2\) the last factor is \(\le(1+\sqrt2)^{\log K/2}\le1+\sqrt2\)). With \(\hat\kappa(1)=4a_c+1376a_1^2\): \(\lVert f(i)\rVert\le8(1+\sqrt2)^3B_3(a_c+344a_1^2)\xi^2\). The current clause is identical with \(\mathcal J\) in place of \(\lVert f\rVert\) (Theorem 1's second line of (2) for the real slit; Lemma 2.6 for the disc). \(\square\)

**Remarks.** (1) The proof never compares the complex reconstruction with a real one; it only uses the real theory on a segment and the crude complex theory on a polynomially large disc. That is why no decay estimate, no linear-response bound and no second-order propagator bound is needed. (2) Only \(\lvert A'\rvert\) enters, not \(\lvert\nabla A'\rvert\): the complex curvature \(a_c\) (CMP109 clause (iii)) carries the derivative information. (3) The same argument, with Theorem 1's bound on \(\Omega_j\), gives bounds on every \(\Omega_j\), \(j\le n\), in [V]'s normalisation \(\varepsilon L^{-2j}\) with \(\varepsilon=2\hat\kappa\ell_n^2\); clause (iv) needs only \(\Omega_n\).

## 5. The second-order premise

(CR) does not use any second-order linear bound: the current clause enters only through Theorem 1 (real) and Proposition 9's (19) (crude).

Two places still lean on second-order statements:

1. **Proposition 9's second-order bounds for complex \(B\)** (used in Lemma 2.6, current). [V] derives them from (179)–(180), where p.306 says (source): "From the estimate (3.137) it follows that \(\Delta^{(2)}\) is a small perturbation of \(\Delta_a\), and the new operator \(G\) has exactly the same properties as \(\Delta_a^{-1}\)." This is a Neumann series: \(G=\sum_nG_0(\Delta^{(2)}G_0)^n\) with \(G_0=\Delta_a^{-1}\), for which [P] Theorem 3.3 asserts all of (3.42)–(3.47) *including* the covariant-Laplacian inequality ([P] p.421: "the operator we have investigated in previous sections … \(G_0=(\Delta+DRD^*+Q^*aQ)^{-1}\)"; the exception on p.422 concerns \(G=\Delta_{\mathcal R}^{-1}\), whose perturbation \(\Delta'_{\mathcal R}\) contains derivatives). \(\Delta^{(2)}\) is zeroth order and small ((3.137): "\(\lvert(\Delta^{(2)}A)(b)\rvert\le O(1)M\alpha_0(L^j\eta)^{-2}\lvert A\rvert\) … the supremum \(\lvert A\rvert\) is taken over several \(j\)-blocks", source). Hence \(\Delta_UG=\Delta_UG_0\,(I-\Delta^{(2)}G_0)^{-1}\) with the decay of \(\Delta_UG_0\). **conditional** on [P] Theorem 3.3 for \(G_0\) and (3.137).
2. **The locality theorem's current clause** (analysis Lemma 2.1, (V3′)). What Lemma 2.1 uses is the first Taylor coefficient of \(\mathscr H\). In the representation (179)–(180) it is \(H_0B+G\Delta^{(2)}H_0B\) (\(D\) is quadratic by [V] (55)). [V] (130) (source input; p.298): "\(\lvert(\Delta_{U_0}H_{0,\mu\nu})(x,y')\rvert\le B_0(L^j\eta)^{-3}(L^{j'}\eta)^{-d}e^{-\delta_0d(y,y')}\)". Combined with item 1, (3.133) for \(H_0\) and locality of \(\Delta^{(2)}\), the linear term has the Laplacian bound with decay \(\frac12\delta_0\); \(D^*D\) follows by [V] (134)–(135), (140) (\(DPD^*\) bounded with decay, (3.49)). **conditional**. This replaces the one-sentence status of the analysis by displayed source bounds at the same level as the first-order ones ((3.132) is itself "same way" in [P]).

The proof assumes (3.132) or Theorem 3.3; the reduction is to them.
