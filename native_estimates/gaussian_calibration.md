# Transverse variation of the blocked covariance

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 1. The constrained Gaussian density and its projection

**1.1 Composite identification.** Assume parts 1–2 of [Theorem S for the constrained Gaussian](composite_gaussian.md), which identify the actual blocked map and its scalar projection. Then \(\sum_{k<n}d^G_k=C_n:=\tilde{\mathcal P}_n\log\mathfrak D_n\), where \(\mathfrak D_n(V)\) is the \(g^0\) density (Laplace prefactor) of
\(\rho_n(V)=\int dU\,\delta(\bar U^n(U)V^{-1})e^{-YA(U)}\) relative to coarse Haar measure, and \(\tilde{\mathcal P}\) is the second moment CMP109 (1.22) normalised by \(\tilde{\mathcal P}A=1\). The finite-dimensional steps use the Jensen bound $\|d^{\prime}Qa\|^2\le L^{4-d}\|da\|^2$, the transport identity of Lemma T, and the Laplace expansion at the constrained critical orbit. These calculations do not establish parts 1–2 of Theorem S.

**1.2 Notation.** Fine lattice \(\mathbb Z^4\); block centres \(L^n\mathbb Z^4\) (\(L\) odd). \(Q_U:=D\bar U^n(U)\) in right-invariant coordinates \(U'=e^{iw}U\); \(d_U\) the infinitesimal gauge action, \((d_U\lambda)_b=\lambda(b_-)-\mathrm{Ad}_{U_b}\lambda(b_+)\); \(E\) the restriction of site functions to block centres; \(K\) the inclusion of \(\ker E\); \(V_U:=d_UK\) (internal gauge directions). Gauge covariance of the average gives, exactly and for every \(U\),
\[
Q_UV_U=0,\qquad Q_Ud_U=d'_{\bar U^n(U)}E. \tag{1.1}
\]
\(H_U\) is the Hessian of \(A\) at \(U\) in the chart \(w\mapsto e^{iw}U\). \(T'_U:=\ker Q_U\cap(\operatorname{Ran}V_U)^\perp\). At a constrained minimiser \(U=U_n(V)\) with multiplier \(\lambda_V\), \(H^\lambda:=\operatorname{Hess}(A-\lambda_V\cdot\bar U^n)(U)\) annihilates \(\operatorname{Ran}V\) and
\[
\log\mathfrak D_n(V)=\tfrac12\log\det(V^*V)-\tfrac12\log\det(QQ^*)-\tfrac12\log\det\bigl(H^\lambda|_{T'}\bigr)\quad(\text{up to a constant}). \tag{1.2}
\]
(This is the Morse–Bott Laplace prefactor; Gaussian transport §3.5, deduction.)

**1.3 Reading on fine plane waves.**

> **Lemma 1.1 conditional.** Let \(F\) be a gauge-invariant analytic function of fine configurations near \(1\), invariant under the lattice symmetries that preserve the block structure, such that the Hessian at \(V=1\) of \(F\circ U_n-\log\mathfrak D_n\) has a symbol \(o(\lvert K\rvert^2)\) at small coarse momentum \(K\), and with a second-derivative kernel at \(U=1\) whose Bloch symbol \(\hat F''(k,k')\) (\(k-k'\in 2\pi L^{-n}\mathbb Z^4\)) is continuous. Then
> \[
> C_n=\lim_{p\to0}\frac{F''[a_p,a_p]}{A''[a_p,a_p]},
> \]
> where \(a_p\) is a transverse plane wave of fine momentum \(p\) in a fixed colour direction, and \(F''[a_p,a_p]\) is the second variation per unit volume (the diagonal Bloch block \(\hat F''(p,p)\)).

*Proof.* \(F'(1)=0\) (a colour-invariant linear functional on adjoint fields vanishes), so \(\operatorname{Hess}_V(F\circ U_n)(1)=D^{\!\top}F''D\) with \(D=DU_n(1)\). For a coarse transverse wave \(b=\beta e^{iK\cdot y}\), \(Db=\sum_m\varphi_me^{ik_m\cdot x}\), \(k_m=(K+2\pi m)/L^n\), and by Steps 2–4 of Lemma T (Gaussian transport §4.2): \(\varphi_m=\hat e(k_m)s_m+O(K^2)\) for \(m\ne0\) and \(\varphi_0=\beta L^{-n}+\hat e(k_0)t+O(K)\). Gauge invariance gives \(\hat F''(k,k')\hat e(k')=0\), and \(\hat F''(k_0,\cdot)=O(K)\) because a constant field is a pure gauge. Hence \(\langle Db,F''Db\rangle=L^{-2n}\beta^\dagger\hat F''(k_0,k_0)\beta+O(K^3)\). The same holds for \(A\) (with \(\hat A''\) diagonal). The ratio of the two coarse second moments is therefore the limit of the ratio of the diagonal blocks. \(\square\)

So \(C_n\) is the coefficient of \(A\) in \(F\) on slowly varying fine backgrounds, for **any** admissible extension \(F\). The choice of \(F\) matters for what can be proved (§8).

**1.4 Three extensions.**
\[
\begin{aligned}
F^{(\lambda)}&:\ \text{(1.2) itself, on constrained minimisers};\\
F^{(1)}(U)&:=\log\det(V^*V)-\tfrac12\log\det(QQ^*)-\tfrac12\log\det{}_{\ker Q}\bigl(H_U+V_UV_U^*\bigr)\qquad(\text{the constant-flux calculation (1), no multiplier});\\
\tilde F(U)&:=\tfrac12\log\det(V^*V)-\tfrac12\log\det(QQ^*)-\tfrac12\log\det\bigl(\tilde H_U|_{T'}\bigr),\qquad \tilde H_U:=P_UH_UP_U,
\end{aligned}
\]
with \(P_U\) the orthogonal projection on \((\operatorname{Ran}d_U)^\perp\). All three are gauge invariant and coincide when \(U\) is a critical point of \(A\) (then \(H_Ud_U=0\)).

> **Lemma 1.2.** (i) Under the constrained-gap hypothesis, \(F^{(1)}\) satisfies the hypotheses of Lemma 1.1. (ii) Under the additional absolute-convergence hypothesis, \(\tilde F\) gives the same limit.

*Proof of (i).* At \(U=1\) the operator \(H+VV^*\) on \(\ker Q=\operatorname{Ran}V\oplus T'\) is block diagonal and strictly positive: on \(T'\) by the hard gap (CMP96 Lemma 2.4, used here as a spectral input), on \(\operatorname{Ran}V\) because \(K^*\Delta K\) (lattice Laplacian with Dirichlet condition at the block centres) is positive. (On the Bloch orbits used in , \(n=1\), \(L=3\), the lowest eigenvalue of \(H+VV^*\) on \(\ker Q\) is \(0.30\), and that of \(\tilde H\) on \(T'\) is \(1.26\).) So the second-variation kernel of \(F^{(1)}\) decays exponentially (at a rate that depends on \(n\)) and its symbol is analytic. On constrained minimisers \(F^{(1)}-F^{(\lambda)}\) is a sum of terms each containing the multiplier \(\lambda_V\) or the current \(J=A'(U)=Q^*\lambda_V\). At second order in \(V\): the terms linear in the second-order part of \(\lambda\) vanish by colour invariance; the rest is a bilinear form \(B(\lambda_1,b)\) with \(\lambda_1=H_cb=O(K^2)b\). \(B\) has an analytic symbol, and \(B(\lambda,d'c)=0\) for all \(c\) by gauge covariance (a constant abelian background is a gauge transform of \(1\), which does not rotate a Cartan-valued \(\lambda\)). An analytic symbol annihilating \(\hat e'(K)\) for all \(K\) vanishes at \(K=0\). So \(B(\lambda_1,b)=O(K^3)\). \(\square\)

*On (ii).* \(\tilde F-F^{(1)}\) is again proportional to the current, but its kernels contain one massless factor \(\Delta^{-1}\), so the symbol of the bilinear form is continuous at \(0\) (each loop integral converges absolutely at \(p=0\), using \(Ed^*G_{T'}dE^*=O(\theta^2)\) at small coarse momentum) but not analytic. Continuity and the same gauge argument give the same limit. This extension requires absolute convergence of the massless kernel integrals uniformly enough to pass to the continuous symbol. That estimate is an additional input for $\tilde F$; the fixed-depth argument above applies directly to $F^{(1)}$.

## 2. Sector decomposition (abelian background)

Take the background \(U_b=e^{ia_bT}\), \(T\) in a Cartan subalgebra, \(\operatorname{Tr}T^2=\frac12\), \(T=\operatorname{diag}(t_1,\dots,t_N)\). Then \(A=\sum_pF_p^2/(4N)+O(a^4)\), \(F_p=(da)_p\). Fluctuations split into root components \(w^{ij}E_{ij}+\overline{w^{ij}}E_{ji}\) (charge \(q_{ij}=t_i-t_j\)) and Cartan components.

> **Lemma 2.1.** For the plaquette with bonds \(1,2,3,4\) (signs \(\sigma=(+,+,-,-)\)), the quadratic part of \(1-\frac1N\operatorname{Re}\operatorname{Tr}U'_p\) on the \((i,j)\) component is
> \[
> \frac1N\Bigl\{\tfrac12\lvert Y\rvert^2\bigl(\cos F_pt_i+\cos F_pt_j\bigr)-\bigl(\sin F_pt_i-\sin F_pt_j\bigr)\sum_{a<b}\sigma_a\sigma_b\operatorname{Im}(x_a\bar x_b)\Bigr\},
> \]
> \(x_1=w_1,\ x_2=e^{iqa_1}w_2,\ x_3=e^{iq(a_1+a_2-a_3)}w_3,\ x_4=e^{iqF_p}w_4,\ Y=\sum_a\sigma_ax_a\).

*Proof.* \(U'_p=e^{iX_1}e^{iX_2}e^{-iX_3}e^{-iX_4}U_p\) with \(X_a\) the transported fluctuations; the second-order term is \(-\frac12(\sum\sigma_aX_a)^2-\frac12\sum_{a<b}\sigma_a\sigma_b[X_a,X_b]\); take the trace against \(e^{iF_pT}\). \(\square\)

To second order in \(a\): \(\cos F t_i+\cos Ft_j=2-\frac12F^2(t_i^2+t_j^2)\), \(\sin Ft_i-\sin Ft_j=qF\). So, after normalising the form to \(\lVert\operatorname{curl}w\rVert^2\) at \(a=0\), every component sees (α) a charge-\(q\) covariant structure depending on \(qa\) only (also through \(Q_U\) and \(d_U\)), and (β) a relative weight \(1-\varpi F_p^2\) on its plaquette term, \(\varpi=\frac14(t_i^2+t_j^2)\) per real root direction and \(\frac12\langle X,T^2X\rangle\) per Cartan direction. Summing: \(\sum_{i<j}q_{ij}^2=N/2\) and \(\sum\varpi=(N^2-1)/(4N)\).

> **Proposition 2.2 deduction, given Lemma 1.1.**
> \[
> C_n=2N^2\kappa_n+\frac{N^2-1}{2}\,E_n,\qquad E_n=\tfrac12\bigl(1-L^{-4n}\bigr),
> \]
> where \(\kappa_n\) is defined by: the one-loop log-density of one **complex** vector field of unit charge, with the weights (β) dropped, is \(\kappa_n\sum_pF_p^2\) on slowly varying \(a\).

*Proof.* The contribution (α) of a pair \(\{i,j\}\) is \(q_{ij}^2\kappa_n\sum F_p^2\); the Cartan components are not charged and their average is linear, so they contribute to (β) only. A weight change \(-\varpi F_p^2\lvert Y_p\rvert^2\) on a real direction shifts the log-density by \(+\frac12\varpi F_p^2\langle\lvert Y_p\rvert^2\rangle\), the expectation being in the constrained flat Gaussian. Since that Gaussian is \((H_0|_{T'})^{-1}\) and \(H_0=\sum_p\operatorname{curl}_p^*\operatorname{curl}_p\), \(\sum_p\langle\lvert Y_p\rvert^2\rangle=\dim T'\): per fine site \(4-4L^{-4n}\) (kernel of \(Q\)) minus \(1-L^{-4n}\) (internal gauge), over 6 plaquettes. So \(E_n=\langle\lvert Y_p\rvert^2\rangle=\frac12(1-L^{-4n})\) exactly. Total coefficient of \(\sum F_p^2\): \(\frac N2\kappa_n+\frac{N^2-1}{8N}E_n\); multiply by \(4N\). \(\square\) (, `tadpoleE`: \(E_1=40/81\), \(E_2=0.4999238=\frac12(1-3^{-8})\) to 15 digits.)

The tadpole term converges geometrically and is harmless for (G-val). From here on only \(\kappa_n\) matters, and the problem is that of a single complex charged vector field: operators \(d_a,\ H_a,\ Q_a\) depending on a real abelian bond field \(a\), with (complex normalisation)
\[
\tilde F_C=\log\det(V^*V)-\log\det(QQ^*)-\log\det(\tilde H|_{T'}),\qquad F^{(1)}_C=2\log\det(V^*V)-\log\det(QQ^*)-\log\det{}_{\ker Q}(H+VV^*).
\]

**The charged average.** For CMP109 (0.12) with the mean (0.10) (pp. 253–254), at the background \(e^{iaT}\), with \(\theta_\Gamma\) the background phase of a contour, \(\bar\theta\) the mean over \(\mathbf G(y,x)\), \(\delta_\Gamma=\theta_\Gamma-\bar\theta\), \(\omega_\Gamma\) the transported sum of \(w\) along \(\Gamma\), \(h_-(z)=z/(e^z-1)\), \(r(z)=(e^z-1)/z\):
\[
\beta_{y,x}=\frac{\sum_\Gamma h_-(i\delta_\Gamma)\,\omega_\Gamma}{\sum_\Gamma h_-(-i\delta_\Gamma)},\qquad
\Omega_x=\beta_{y,x}+e^{i\bar\theta_{y,x}}\omega_{[x,x']}-e^{i(\bar\theta_{y,x}+a_{[x,x']}-\bar\theta_{y',x'})}\beta_{y',x'}-e^{i\varphi_x}\omega_c ,
\]
\[
(Q_aw)(c)=r(i\bar\varphi)\,L^{-4}\!\!\sum_{x\in B(y)}h_-(i\varphi_x)\,\Omega_x+e^{i\bar\varphi}\omega_c,\qquad a'_c=\bar\varphi+a(c), \tag{2.1}
\]

## 3. Exact blocked formulas

Write \(\Delta=d^*d\), \(M=H+dd^*\), \(\tilde M=\tilde H+dd^*\), and for coarse objects
\[
\mathcal C=QM^{-1}Q^*,\quad \tilde{\mathcal C}=Q\tilde M^{-1}Q^*,\quad G_E=E\Delta^{-1}E^*,\quad W=Ed^*M^{-1}dE^*,\quad Y=QM^{-1}dE^*.
\]

> **Proposition 3.1.** For every fine background (no critical-point assumption), as identities between determinants of finite matrices satisfying (1.1):
> \[
> F^{(1)}_C=2\log\det\Delta-\log\det M+2\log\det G_E-\log\det\mathcal C-\log\det\bigl(1-W+Y^*\mathcal C^{-1}Y\bigr), \tag{3.1}
> \]
> \[
> \tilde F_C=2\log\det\Delta-\log\det\tilde M-\log\det\tilde{\mathcal C}-\log\det\bigl(d'^*\tilde{\mathcal C}^{-1}d'\bigr). \tag{3.2}
> \]

*Proof.* (3.1): \(\det(V^*V)=\det(K^*\Delta K)=\det\Delta\det G_E\) (Schur, \(EE^*=1\)). \(H+VV^*=M-(Ed^*)^*(Ed^*)\) because \(KK^*=1-E^*E\). On \(\ker Q\): \(\det_{\ker Q}(M-B^*B)=\det_{\ker Q}M\cdot\det(1-BG_{\ker Q}B^*)\) with \(B=Ed^*\), \(G_{\ker Q}=M^{-1}-M^{-1}Q^*\mathcal C^{-1}QM^{-1}\), and \(\det_{\ker Q}M=\det M\det\mathcal C/\det(QQ^*)\). The factor \(\det(QQ^*)\) cancels. (3.2): \(\tilde Hd=0\) exactly, so \(\tilde Md=d\Delta\) and \(\tilde M\) is block diagonal on \(\operatorname{Ran}d\oplus(\operatorname{Ran}d)^\perp\). Then \(W=1\), \(Y=d'G_E\) by (1.1), and the chain of (3.1) with \(H\to\tilde H\) gives \(1-W+Y^*\tilde{\mathcal C}^{-1}Y=G_Ed'^*\tilde{\mathcal C}^{-1}d'G_E\); it remains to check \(\det_{\ker Q}(\tilde H+VV^*)=\det(V^*V)\det(\tilde H|_{T'})\), which holds because \(\tilde HV=0\). \(\square\)

**Interpretation.** (3.2) says: one-loop density \(=\) (fine one-loop functional) \(/\) (coarse one-loop functional), the coarse theory having covariance \(\tilde{\mathcal C}\) and "ghost" operator \(d'^*\tilde{\mathcal C}^{-1}d'\). The fine factor \(2\log\det\Delta-\log\det\tilde M\) is the Wilson theory alone.

**Second variations.** With \(a=\epsilon(A e^{ip\cdot x}+\bar Ae^{-ip\cdot x})\), an operator \(O\) is carried through order \(\epsilon^2\) on the three Bloch fibres \(\kappa,\kappa\pm p\) ("jets": zeroth-order blocks \(O_0\) on the three fibres, the four first-order blocks between neighbours, the second-order block \(O_S\) on the centre). Products, inverses and adjoints are closed at this order. The \(\epsilon^2\) coefficient of \(\log\det O\) per fibre is
\[
\ell_2(O)(\kappa)=\operatorname{tr}\bigl[O_0^{-1}O_S\bigr]-\tfrac12\sum_\pm\operatorname{tr}\bigl[O_0(\kappa)^{-1}O_{\mp}(\kappa\pm p)\,O_0(\kappa\pm p)^{-1}O_\pm(\kappa)\bigr], \tag{3.3}
\]
and (3.1), (3.2) hold for the sums of \(\ell_2\) over closed orbits \(\{\kappa+jp\}\), hence for the integrals over the Brillouin zone. Fine operators are diagonal in the alias index \(m\) (\(k_m=(\theta+2\pi m)/L^n\)); a coarse operator is an alias average, e.g. \(\tilde{\mathcal C}(\theta)=L^{-4n}\sum_mQ(k_m)\tilde M(k_m)^{-1}Q(k_m)^*\), computed level by level.

## 4. The decomposition \(\kappa_n=\sum_{k<n}s_2(k)+\mathcal B_n\)

There are two versions, one for each blocked formula. Let
\[
f^{\rm F}(k;p):=2\ell_2(\Delta)-\ell_2(M),\qquad \tilde f(k;p):=2\ell_2(\Delta)-\ell_2(\tilde M)
\]
at fine momentum \(k\) and fine background momentum \(p\) (transverse polarisation): the Wilson one-loop density in the local Feynman form and in the projected form. By (3.1), (3.2), per unit fine volume and with \(p_0=pL^{-n}\),
\[
F^{(1)\prime\prime}_C=\int_{[-\pi,\pi]^4}\!\frac{d^4k}{(2\pi)^4}f^{\rm F}(k;p_0)+L^{-4n}\!\!\int\!\frac{d^4\theta}{(2\pi)^4}\bigl[2\ell_2(G_E)-\ell_2(\mathcal C)-\ell_2(1-W+Y^*\mathcal C^{-1}Y)\bigr],
\]
\[
\tilde F_C''=\int_{[-\pi,\pi]^4}\!\frac{d^4k}{(2\pi)^4}\tilde f(k;p_0)-L^{-4n}\!\!\int\!\frac{d^4\theta}{(2\pi)^4}\bigl[\ell_2(\tilde{\mathcal C})+\ell_2(d'^*\tilde{\mathcal C}^{-1}d')\bigr].
\]
Split the fine integral at the cell \(c_n=\{\lvert k_i\rvert\le\pi L^{-n}\}\) (the zero alias), and \(c_0\setminus c_n\) into shells \(c_k\setminus c_{k+1}\). With \(\mathsf N(p_0)=2\sum_{\mu<\nu}\lvert\hat p_\mu A_\nu-\hat p_\nu A_\mu\rvert^2\) the second variation of \(\sum F_p^2\) per unit volume (\(\hat p_\mu=e^{ip_{0,\mu}}-1\)), define for \(f=f^{\rm F}\) or \(\tilde f\)
\[
\sigma_k(p_0):=\frac1{\mathsf N(p_0)}\int_{c_k\setminus c_{k+1}}\frac{d^4k}{(2\pi)^4}f(k;p_0),\qquad
\beta_n(p):=\frac{1}{\mathsf N(p_0)}\Bigl\{\int_{c_n}\!\frac{d^4k}{(2\pi)^4}f(k;p_0)+[\text{coarse integral}]\Bigr\}.
\]
For \(k\) in a shell and \(\lvert p_0\rvert\) small compared with \(L^{-k-1}\), \(f(k;\cdot)\) is real-analytic and even, so \(\sigma_k(p_0)=s_0(k)\lvert p_0\rvert^{-2}+s_2(k)+O(p_0^2)\). The \(\lvert p_0\rvert^{-2}\) terms are the pieces that a sharp momentum cut does not keep gauge invariant; they cancel in the sum because the total is gauge invariant (numerically \(a_0+b_0=O(10^{-6})\), §7). Set
\[
s_2(k):=\bigl[\sigma_k\bigr]_{p^0},\qquad \mathcal B_n:=\lim_{p\to0}\Bigl(\beta_n(p)+\lvert p_0\rvert^{-2}\sum_{k<n}s_0(k)\Bigr)=\kappa_n-\sum_{k<n}s_2(k), \tag{4.1}
\]
with superscripts \({}^{\rm F}\) or \(\tilde{\ }\) according to the version. For the Feynman version (4.1) rests on Lemma 1.1 and Lemma 1.2(i) only; for the projected version also on Lemma 1.2(ii). (4.1) is a definition plus the reduction; its content is that \(s_2(k)\) involves the Wilson action only, and that \(\mathcal B_n\) lives at the top scale: in units of the top lattice it is an integral over \(\theta\in[-\pi,\pi]^4\) of the zero-alias Wilson density plus the coarse density.

## 5. The logarithm: \(s_2(k)\to\frac{11}{24\pi^2}\log L\)

> **Theorem 5.1 (a; step (1) of the proof is argued without explicit constants on compact momentum shells).** For both versions, \(s_2(k)=\dfrac{11}{24\pi^2}\log L+O(L^{-k})\). In particular \(\sum_{k<n}s_2(k)=\dfrac{11}{24\pi^2}\,n\log L+O(1)\).

*Proof.* (1) *Scaling.* Each of \(f^{\rm F},\tilde f\) (written \(f\)) is a fixed rational function of the jets of \(d_a\) and \(H_a\), which are trigonometric polynomials in \(k,p\) with denominators \(\Delta_0(\kappa)=\sum_\mu4\sin^2(\kappa_\mu/2)\) at the three fibres. Under \(k\to tk,\ p\to tp\) the jets converge, after division by their homogeneity factors, to the jets of the continuum operators
\[
d^{\rm c}\lambda=-D\lambda,\qquad (H^{\rm c}w)_\nu=-D_\mu(D_\mu w_\nu-D_\nu w_\mu)-iF_{\nu\mu}w_\mu,\qquad D=\partial+ia,\quad [D_\mu,D_\nu]=iF_{\mu\nu},
\]
uniformly with error \(O(t)\) for \((k,p)\) in compact sets on which the three fibres stay away from \(0\), together with their \(p\)-derivatives (analyticity in a complex neighbourhood and Cauchy). [The sign of the last term of \(H^{\rm c}\) is fixed by the Ward identity \(H_ad_a=O(\partial F)\):  T3 shows \(\lVert H_ad_a\rVert=O(p^2)\) for the lattice form of Lemma 2.1 and \(O(p)\) if the magnetic term is dropped or reversed.] Since \(f\) is of second order in \(a\), \(f(tk;tp)=t^{-2}[f^{\rm c}(k;p)+O(t)]\) and for its \(p^2\)-coefficient \(f_2(tk)=t^{-4}[f_2^{\rm c}(k)+O(t)]\) with \(f^{\rm c}_2\) homogeneous of degree \(-4\). Hence, with \(k=L^{-k}\kappa\),
\[
s_2(k)=\frac{1}{\mathsf N^{(2)}}\int_{c_0\setminus c_1}\frac{d^4\kappa}{(2\pi)^4}f^{\rm c}_2(\kappa)+O(L^{-k})=\frac{\log L}{(2\pi)^4\,\mathsf N^{(2)}}\int_{S^3}f_2^{\rm c}\,d\Omega+O(L^{-k}),
\]
the last step because the shell between two homothetic star-shaped surfaces of ratio \(L\) contributes \(\int_{r(\Omega)/L}^{r(\Omega)}dr/r=\log L\) in every direction. \(\mathsf N^{(2)}=2p^2\lvert A\rvert^2\) for transverse \(A\).

(2) *Feynman form.* Take \(f=f^{\rm F}\). In the continuum \(M^{\rm c}=-D^2+\mathsf E\), \(\mathsf E_{\nu\mu}=-2iF_{\nu\mu}\) (Hermitian), so \(2\ell_2(\Delta)-\ell_2(M)=-2\ell_2(-D^2)+\operatorname{tr}[G\mathsf E_+G\mathsf E_-]\), \(G=1/k^2\).
- *Scalar.* \(\ell_2(-D^2)=2\lvert A\rvert^2/k^2-4\lvert k\cdot A\rvert^2/(k^2(k+p)^2)\) (transverse \(A\), symmetrised in \(\pm p\)). Its \(p^2\)-coefficient is \(-4\lvert k\cdot A\rvert^2k^{-4}[-p^2k^{-2}+4(k\cdot p)^2k^{-4}]\). With \(\langle k_\mu k_\nu\rangle=\frac{k^2}{4}\delta_{\mu\nu}\) and \(\langle k_\mu k_\nu k_\rho k_\sigma\rangle=\frac{k^4}{24}(\delta\delta+\delta\delta+\delta\delta)\) on \(S^3\): angular mean \(=\frac13p^2\lvert A\rvert^2k^{-4}=\frac16\mathsf N^{(2)}k^{-4}\).
- *Magnetic.* \(\mathsf E_\pm=-2iF_\pm\), \(F_{+\mu\nu}=i(p_\mu A_\nu-p_\nu A_\mu)\), \(\mathsf E_-=\mathsf E_+^\dagger\); \(\operatorname{tr}[\mathsf E_+\mathsf E_-]=8\sum_{\mu<\nu}\lvert p_\mu A_\nu-p_\nu A_\mu\rvert^2=4\mathsf N^{(2)}\); the \(p^0\) coefficient of \(1/(k^2(k+p)^2)\) is \(k^{-4}\).

So \(\langle f^{\rm c,Feyn}_2\rangle=(4-\frac26)\mathsf N^{(2)}k^{-4}\), and with \(\lvert S^3\rvert=2\pi^2\): \(\frac{2\pi^2}{(2\pi)^4}\cdot\frac{11}{3}=\frac{11}{24\pi^2}\).

(3) *Projected form.* \(-\log\det M+\log\det\tilde M=-\operatorname{Tr}\log(1+\tilde M^{-1}(H-\tilde H))=-\operatorname{Tr}[\Delta^{-2}\mathfrak m]+O(J^2)\), \(\mathfrak m:=d^*Hd\). In the continuum \(H^{\rm c}D\lambda=-iJ\lambda\) with \(J_\nu=\partial_\mu F_{\mu\nu}\), so \(\mathfrak m=iJ\cdot D\), and \(J_+=-p^2A\) (transverse \(A\)) is already of order \(p^2\). The \(p^2\)-coefficient of \(-\operatorname{Tr}[\Delta^{-2}\mathfrak m]\) has integrand \(-\{-2\operatorname{Re}(J_+\!\cdot\!\bar A)k^{-4}+8\operatorname{Re}[(k\cdot\bar A)(k\cdot J_+)]k^{-6}\}\), whose angular mean is \(0\). The \(O(J^2)\) terms are \(O(p^4)\). So \(\tilde M\) and \(M\) give the same \(\langle f_2^{\rm c}\rangle\). \(\square\)

The scaling step uses the expansion of the lattice jets on compact momentum shells. It requires convergence of the second momentum derivatives there; it gives no uniform bound on the transverse remainder.

## 6. The remainder \(\mathcal B_n\) and hypothesis (U)

> **(U).** \(\sup_n\lvert\mathcal B^{\rm F}_n\rvert<\infty\). (Equivalently, given Lemma 1.2(ii): \(\sup_n\lvert\tilde{\mathcal B}_n\rvert<\infty\), since \(\mathcal B^{\rm F}_n-\tilde{\mathcal B}_n=\sum_{k<n}(\tilde s_2(k)-s^{\rm F}_2(k))\) converges by Theorem 5.1.)

> **Theorem 6.1 conditional on Theorem S for the composite constrained Gaussian.** For every \(n\)
> \[
> C_n-d_Bn=2N^2\Bigl[\sum_{k<n}\Bigl(s^{\rm F}_2(k)-\frac{11\log L}{24\pi^2}\Bigr)+\mathcal B^{\rm F}_n\Bigr]+\frac{N^2-1}{4}\bigl(1-L^{-4n}\bigr),
> \]
> the sum converges absolutely, and (G-val) holds if and only if (U) holds, with \(B_G\le 2N^2\bigl(\sum_k\lvert s^{\rm F}_2(k)-\frac{11\log L}{24\pi^2}\rvert+\sup_n\lvert\mathcal B^{\rm F}_n\rvert\bigr)+\frac{N^2-1}{4}\). The same formula holds with \(\tilde s_2,\tilde{\mathcal B}_n\) if Lemma 1.2(ii) is granted.

*Proof.* Lemma 1.1 with Lemma 1.2(i), Proposition 2.2, (3.1), (4.1), Theorem 5.1. \(\square\)

So the coefficient of \(n\) in \(C_n\) is \(d_B\), with its sign, if and only if \(\mathcal B^{\rm F}_n=o(n)\); and (G-val) is exactly the boundedness of \(\mathcal B^{\rm F}_n\). The projected version is described below.

**A gauge-invariant form of the coarse factor.**

> **Lemma 6.2.** For any \(\xi\) (coarse sites \(\to\) coarse bonds) and any \(\tau\) (coarse sites \(\to\) coarse sites), the coarse factor \(\log\det\tilde{\mathcal C}+\log\det(d'^*\tilde{\mathcal C}^{-1}d')\) of (3.2) is unchanged under \(\tilde{\mathcal C}\to\tilde{\mathcal C}+d'\xi^*+\xi d'^*+d'\tau d'^*\). Consequently, with \(P'\) the orthogonal projection on \((\operatorname{Ran}d')^\perp\),
> \[
> \tilde F_C=\bigl[\log\det\Delta-\log\det{}'(\tilde H|_{(\operatorname{Ran}d)^\perp})\bigr]-\bigl[\log\det(d'^*d')+\log\det{}'(P'\tilde{\mathcal C}P')\bigr].
> \]

*Proof.* \(\tilde{\mathcal C}+d'\xi^*+\xi d'^*+d'\tau d'^*=S\tilde{\mathcal C}S^*+d'\tau'd'^*\) with \(S=1+d'\eta^*\), \(\eta=\tilde{\mathcal C}^{-1}\xi\). For \(S\tilde{\mathcal C}S^*\): \(\det\) picks up \(\lvert\det(1+\eta^*d')\rvert^2\) and \(d'^*(S\tilde{\mathcal C}S^*)^{-1}d'=(1+\eta^*d')^{-*}(d'^*\tilde{\mathcal C}^{-1}d')(1+\eta^*d')^{-1}\) loses the same factor. For \(\mathcal C+d'\tau d'^*\): \(\det\) picks up \(\det(1+\tau\mathcal G)\), \(\mathcal G=d'^*\mathcal C^{-1}d'\), and by Woodbury \(d'^*(\mathcal C+d'\tau d'^*)^{-1}d'=\mathcal G(1+\tau\mathcal G)^{-1}\). Choosing \(\xi,\tau\) to remove the mixed blocks and normalise the longitudinal block gives the second statement; the fine bracket is \(2\log\det\Delta-\log\det\tilde M\) because \(\tilde M=\tilde H\oplus dd^*\). \(\square\)

So the one-loop density is exactly (fine orbit volume \(\times\) fine transverse Gaussian) \(/\) (coarse orbit volume \(\times\) coarse transverse Gaussian), and **only the transverse block of the blocked covariance enters**. This matters: the full regular part of \(\tilde{\mathcal C}\) is *not* uniformly bounded. Numerically, at the flat background, \(\lVert R_n\rVert\) grows linearly in \(n\) (e.g. \(0.39,\,0.66,\,0.89\) at the zone corner for \(n=1,2,3\)), while \(\lVert P'R_nP'\rVert\) stays bounded and converges (\(0.0091,\,0.0053,\,0.0049\) at the same point); see. The growth is the contour part of the average: \(Q=S+d'\gamma\) with \(\lvert\gamma(k)\rvert^2\sim k^{-2}\) between the block scale and the lattice scale, which gives \(\int d^4k/k^4\) in \(d'\gamma\tilde M^{-1}\gamma^*d'^*\). By Lemma 6.2 it is a pure coarse gauge term and drops out exactly.

**Why (U) should hold additional assumption.** Write \(\tilde{\mathcal C}=\mathcal C_0+R\), \(\mathcal C_0=L^{-4n}Q_0\tilde M_0^{-1}Q_0^*\) the zero-alias term and \(R\) the sum over aliases \(m\ne0\). By (1.1), \(Q(k_m)d(k_m)=d'(\theta)\) for every alias. If \(R\) is dropped, then \(d'^*\mathcal C_0^{-1}d'=L^{4n}d_0^*\tilde M_0d_0=L^{4n}\Delta_0^2\) and
\[
\bigl[2\ell_2(\Delta_0)-\ell_2(\tilde M_0)\bigr]-\ell_2(\mathcal C_0)-\ell_2(d'^*\mathcal C_0^{-1}d')=-\ell_2(Q_0)-\ell_2(Q_0^*)
\]
up to terms that are second differences \(g(\theta+p)+g(\theta-p)-2g(\theta)\), which integrate to boundary terms on the cell. The infrared-singular Wilson density of the zero alias cancels identically against the coarse density; what remains is the \(\epsilon^2\) variation of the zero-alias symbol of the average, a regular object. With \(R\) restored, the correction is a function of \(L^{4n}Q_0^{-1}RQ_0^{-*}\) which tends to \(0\) at \(\theta\to0\). So \(\mathcal B_n\) is bounded as soon as, in units of the top lattice, uniformly in \(n\), and **modulo the coarse gauge terms of Lemma 6.2**,

- **(U1)** the zero-alias symbol \(Q_{n,0}(\theta)\) of the composite average, its inverse, and its first two background jets are bounded on the cell;
- **(U2)** the regular part \(R_n(\theta)=L^{-4n}\sum_{m\ne0}Q(k_m)\tilde M(k_m)^{-1}Q(k_m)^*\) and its first two background jets are bounded.

**What (U) is not.** It is not a statement about large fields, histories, cutoffs or volumes: it concerns the Gaussian at the flat background, in infinite volume, for one complex scalar-charged vector field. It is the precise form of the bound "uniform \(O(1)\)", stripped of the logarithm.
