# Periodic transfer states and a finite-volume criterion

The positive-trace comparison holds on intermediate rectangular Wilson tori. A thermal-to-vacuum comparison for polynomial insertions also requires the [marked-insertion condition](transfer_normalization.md). The Laplace estimate concerns $\beta\ge\beta_*m^{C_0}$ and gives no bound on a physically matched sequence with fixed terminal coupling.

## 1. The thermal criterion depends on the hierarchy only through coefficient growth

### 1.1 Setting

Use Annex M §4 and Annex V §1 verbatim:
- \(a_n\downarrow0\), \(T_n\uparrow\infty\), and \(N_n:=T_n/a_n\in2\mathbb Z\).
- \(P_n\) is the positive, trace-class, gauge-projected Wilson transfer operator of Lüscher (CMP 54 (1977) 283) on the spatial torus with \(N_n^3\) sites, at bare coupling \(\beta_n\). Its top eigenvalue \(\lambda_{0,n}\) is simple.
- \(H_n:=-a_n^{-1}\log(P_n/\lambda_{0,n})\ge0\), \(Z_n(u):=\operatorname{Tr}e^{-uH_n}\) and \(f_n(u):=\log Z_n(u)\) for \(u>0\).
- Annex M (4.2) defines \(\Gamma_n=f_n(T_n/2)-f_n(T_n)\). For \(0<\theta<1\) put \(\Gamma_{n,\theta}:=f_n(\theta T_n)-f_n(T_n)\).

Every \(f_n\) is finite, nonincreasing and convex on \((0,\infty)\), with \(f_n(u)\downarrow0\). It is the logarithm of the Laplace transform of the spectral counting measure of \(H_n\), whose ground state is simple. (deduction; elementary)

Annex M (4.3)–(4.4) gives each fixed positive-time polynomial \(F\) a transfer realization \(A_{F,n}=e^{-(T_n/2-r_{F,n})H_n}X_{F,n}\), with \(0\le r_{F,n}\le R_F\), and \(p_n(F)^2=\lVert A_{F,n}\rVert_2^2/Z_n(T_n)\). Set
\[
q_{F,n}(u)=\frac{\operatorname{Tr}\big[X_{F,n}^*e^{-(T_n-2r_{F,n}-2u)H_n}X_{F,n}\big]}{Z_n(T_n)},\qquad 0\le u<T_n/2-r_{F,n}.
\]
Annex M shows that \(q_{F,n}\) is nondecreasing and log-convex, with \(q_{F,n}(0)=p_n(F)^2\).

### 1.2 Interpolation with boundedness only

**Lemma 1.1.** Let \(q_n:[0,S_n]\to[0,\infty)\) be nondecreasing and log-convex, with \(S_n\to\infty\), \(\sup_nq_n(0)\le Q<\infty\) and \(S_n^{-1}\log^+q_n(S_n)\to0\). Then \(q_n(t_n)-q_n(0)\to0\) for every sequence \(0\le t_n\le\bar t\).

*Proof.* Put \(\vartheta_n=t_n/S_n\to0\). Log-convexity gives \(q_n(t_n)\le q_n(0)^{1-\vartheta_n}q_n(S_n)^{\vartheta_n}\). Fix \(\eta\in(0,1)\) and split into two cases.
- If \(q_n(0)\ge\eta\), then \(q_n(t_n)/q_n(0)\le\exp\{\vartheta_n(\log^+q_n(S_n)+\log\eta^{-1})\}\to1\), uniformly in such \(n\). Hence \(q_n(t_n)-q_n(0)\le Q(\exp\{\cdots\}-1)\to0\).
- If \(q_n(0)<\eta\), then for \(\vartheta_n\le1/2\) we get \(q_n(t_n)\le\eta^{1/2}\exp\{\vartheta_n\log^+q_n(S_n)\}\le2\eta^{1/2}\) eventually.

Monotonicity gives \(q_n(t_n)\ge q_n(0)\). Hence \(\limsup_n\lvert q_n(t_n)-q_n(0)\rvert\le2\eta^{1/2}\) for every \(\eta\), which proves the lemma. \(\square\)

Apply the lemma with \(S_n=T_n/4-r_{F,n}\). Then \(q_{F,n}(S_n)\le\lVert X_{F,n}\rVert^2e^{\Gamma_n}\), because \(\operatorname{Tr}[X^*\rho X]\le\lVert X\rVert^2\operatorname{Tr}\rho\) for \(\rho\ge0\). The rest of Annex M Theorem 4.2 then goes through unchanged, with "the hierarchy converges" weakened to \(\sup_np_n(F)^2<\infty\).

The only exception is the convergence of fine-lattice shifts \(t_n\to t\). It is not needed if, as in (E.17), time translations are defined by their lattice realizations.

### 1.3 The mark budget for actual renormalized marks

**Proposition 1.2.** Make the following assumptions.
- The renormalized one-field representatives are \(\Phi^R_{\alpha,n}(x)=\sum_\beta Z^{(n)}_{\alpha\beta}a_n^{-4}O_\beta(x)+c^{(n)}_\alpha\). Here the \(O_\beta\) are fixed gauge-invariant compact Wilson stencils, with \(\lvert O_\beta\rvert\le C_O\). These include clover, trace-repair, temporal and mixed realizations.
- Any finite list of local product redefinitions carries coefficients \(b^{(n)}\).
- \(F\) is a fixed positive-time polynomial of degree \(m\). Its kernel \(f\) is sampled on the lattice, with time support in \([0,R_F]\) and \(\lVert f\rVert_{1,n}:=\sum a_n^{4m}\lvert f\rvert\le C_f\).

Then
\[
\log^+\lVert X_{F,n}\rVert\le\log^+C_f+m\log^+\!\Big(C_O\big(\lVert Z^{(n)}\rVert a_n^{-4}+\lvert c^{(n)}\rvert+\lvert b^{(n)}\rvert+1\big)\Big).
\]
Consequently, \(\log^+\lVert X_{F,n}\rVert=o(T_n)\) for every fixed \(F\) of every degree as soon as

\[
\textbf{(G)}\qquad \log\big(1+\lVert Z^{(n)}\rVert+\lvert c^{(n)}\rvert+\lvert b^{(n)}\rvert\big)=o(T_n)\quad\text{and}\quad \log(1/a_n)=o(T_n).
\]

*Proof.* The sup norm of the path mark is at most \(\lVert f\rVert_{1,n}\) times the \(m\)-th power of the sup of the renormalized local fields. Positive path-kernel domination, Annex M (4.19)–(4.20), gives \(\lVert X_{F,n}\rVert\le\lVert F_n\rVert_\infty\), with no volume factor. \(\square\)

**Corollary 1.3.** Take the B-02 sequence of Port_11_7_1_Base §§1–3:
- \(a_n=L^{-K_n}\ell_0\) and \(T_n=2L^{H_n}\ell_0\), with \(H_n\ge3n\) and \(K_n\le n\);
- \((\log Y_0)^r=L^{2n+s+1/2}\) with \(r\ge2\) and \(\beta_{W,n}=Y_0/N\).

In units \(\ell_0=1\):
- \(\log(1/a_n)/T_n=K_n\log L/(2L^{H_n})\to0\);
- \(\log\beta_{W,n}/T_n\le L^{n+(s+1/2)/2}/(2L^{3n})\to0\).

Hence (G) holds for every coefficient prescription bounded by a fixed power of \(\beta_{W,n}/a_n\). This includes the multipliers \(z_h\sim\beta_W/2\) of the weak comparison family in the quadratic comparison.

A direct estimate of the slab by the sup norm gives a sufficient coefficient-growth condition; a lower bound for that sup norm is not a lower bound for the slab norm.

**Conclusion of §1.** On any cubic sequence obeying the structural marked-insertion condition (S) and (G), the E-05 thermal criterion for **all** fixed marks of **all** degrees is equivalent to the single observable-free statement \(\Gamma_n=o(T_n)\). Matching enters only through (G). This makes precise the finite-cutoff construction remark that a mark-independent result could advance the route.

Remark deduction. Lemma 1.1 can be run with any fixed fraction. Taking \(q_{F,n}(u_\theta)\), where \(T_n-2r-2u_\theta=\theta T_n\), shows that \(\Gamma_{n,\theta}=o(T_n)\) for some \(\theta\in(0,1)\) suffices. Convexity gives \(\Gamma_n=\Gamma_{n,1/2}\le\Gamma_{n,\theta}\) for \(\theta\le1/2\), so fractions \(\theta<1/2\) are formally stronger requirements. Section 2 uses \(\theta=1/L\) and the inequality \(\Gamma_n\le\Gamma_{n,1/L}\).

## 2. A purely Euclidean, cubic bound on the thermal increment

### 2.1 Statement

Write \(Z^W(M_0,M_1,M_2,M_3)\) for the bare Wilson partition function \(\int\prod dU\,e^{-\beta\sum_ps(U_p)}\), with \(s(g)=N-\operatorname{Re}\operatorname{tr}g\ge0\) and normalized Haar measure. It lives on the torus with \(M_\mu\) sites in direction \(\mu\), at the fixed \(a_n,\beta_n\). Put \(Z^W_{\rm cube}(M):=Z^W(M,M,M,M)\).

**Theorem 2.** Let \(L\ge2\) be an integer with \(L\mid N_n\), and set
\[
\Phi_n:=L^4\log Z^W_{\rm cube}(N_n/L)-\log Z^W_{\rm cube}(N_n).
\]
Then
\[
0\le\Gamma_n\le\Gamma_{n,1/L}\le\frac{\Phi_n}{L},\qquad \Phi_n\ge0.
\]

### 2.2 Proof

*Step 1.* Since \(f_n\) is nonincreasing and \(T_n/L\le T_n/2\),
\[
\Gamma_n=f_n(T_n/2)-f_n(T_n)\le f_n(T_n/L)-f_n(T_n)=\Gamma_{n,1/L}.
\]

*Step 2.* \(Z_n(u)=\lambda_{0,n}^{-u/a_n}\operatorname{Tr}P_n^{u/a_n}\) for \(u\in a_n\mathbb N\). Hence
\[
\Gamma_{n,1/L}=\log\operatorname{Tr}P_n^{N_n/L}-\log\operatorname{Tr}P_n^{N_n}+(1-1/L)N_n\log\lambda_{0,n}.
\]
Since \(\lambda_{0,n}^{N_n}\le\operatorname{Tr}P_n^{N_n}\), this gives
\[
\Gamma_{n,1/L}\le\log\operatorname{Tr}P_n^{N_n/L}-\tfrac1L\log\operatorname{Tr}P_n^{N_n}.
\]
This step removes \(\lambda_{0,n}\), using only an upper bound on it.

*Step 3.* By Lüscher's construction source input, \(\operatorname{Tr}P_n^{M}=Z^W(M,N_n,N_n,N_n)\) for every integer \(M\ge1\); the trace is the physical trace. The Wilson action is invariant under the hypercubic group. Hence the same construction in direction \(\mu\), on the transverse torus of any side lengths, gives a positive trace-class transfer operator \(P^{(\mu)}\) with \(Z^W=\operatorname{Tr}(P^{(\mu)})^{M_\mu}\).

For a positive trace-class \(Q\) and integers \(k,M\ge1\), \(\operatorname{Tr}Q^{kM}=\sum\mu_i^{kM}\le(\sum\mu_i^M)^k\). Apply this in directions 1, 2, 3 with \(k=L\) and \(M=N_n/L\):
\[
Z^W(N_n/L,N_n,N_n,N_n)\le Z^W_{\rm cube}(N_n/L)^{L^3}.
\]

*Step 4.* Combining Steps 2 and 3,
\[
\Gamma_{n,1/L}\le L^3\log Z^W_{\rm cube}(N_n/L)-L^{-1}\log Z^W_{\rm cube}(N_n)=\Phi_n/L.
\]
Applying Step 3 in all four directions gives \(Z^W_{\rm cube}(N_n)\le Z^W_{\rm cube}(N_n/L)^{L^4}\), i.e. \(\Phi_n\ge0\). \(\square\)

### 2.3 Consequences

**Corollary 2.1.** On a cubic sequence with \(L\mid N_n\) and (G), the following implication holds:
\[
\boxed{\ \Phi_n=L^4\log Z^W_{{\rm cube},a_n,\beta_n}(T_n/L)-\log Z^W_{{\rm cube},a_n,\beta_n}(T_n)=o(T_n)\ }
\ \Longrightarrow\ \text{Annex M (4.5) holds for every fixed }F\text{ of every degree.}
\]
If the renormalized slab premise (4.12) also holds, Annex M Theorem 4.2 (with Lemma 1.1) gives the periodic OS insertion bound (E.17).

The slab premise (4.12) is the content of E-02 to E-04, not of E-05.

Remarks.
- Equivalently, write \(p_\infty(\beta)=\lim_k\log Z^W_{\rm cube}(L^kM)/(L^kM)^4\), which exists by Step 3. Let \(\varphi_n(M):=\log Z^W_{\rm cube}(M)-M^4p_\infty(\beta_n)\ge0\) be the **finite-size free energy** of the cube. Then \(\Phi_n=L^4\varphi_n(N_n/L)-\varphi_n(N_n)\le L^4\varphi_n(N_n/L)\). So "the cube's finite-size free energy is \(o(\text{side})\)" suffices.
- Both tori are cubes. If \(T_n=2L^{H_n}\ell_0\) is a B-02 period, then so is \(T_n/L=2L^{H_n-1}\ell_0\) after raising the lower bound on \(H_n\) by one; B-02 permits such enlargements. Thus, unlike TS20's three-length defect, **no rectangular torus and no rectangular extension of a source-free theorem is needed.** This removes the geometric objection in TS20 Part IV §5.
- The quantity \(\Phi_n\) is the sharp form of the T6 "S94" difference. S94 asks for \(p_{a,T^*}-p_{a,qT^*}\le C_0\) per unit volume. E-05 needs \(\operatorname{Vol}(T)(p_{a,T/L}-p_{a,T})=o(T)\).

**Corollary 2.2 (a; thermodynamic integration).** At \(\beta=0\) both cube partition functions equal 1. By translation and hypercubic invariance every plaquette has the same expectation, and the side-\(M\) cube has \(6M^4\) plaquettes. Hence
\[
\Phi_n=6N_n^4\int_0^{\beta_n}\big(\langle s_p\rangle_{N_n,\beta}-\langle s_p\rangle_{N_n/L,\beta}\big)\,d\beta.
\]
Thus E-05 is implied by a single-plaquette finite-size estimate, integrated along the whole coupling path:
\[
\int_0^{\beta_n}\lvert\langle s_p\rangle_{N_n}-\langle s_p\rangle_{N_n/L}\rvert\,d\beta=o(T_nN_n^{-4}).
\]
This form makes visible that intermediate couplings enter. The direct estimate at \(\beta_n\) in §5 avoids the path.

### 2.4 Why a Hamiltonian-slab route cannot avoid state information

Assume \(A=X^*e^{-sH}X\ge0\) and \(B=e^{-(t-\delta)H}qe^{-(t+\delta)H}\), with \(\lvert\delta\rvert<t\). Any use of the slab bound \(\lVert e^{-uH}qe^{-uH}\rVert\le Cu^{-\kappa}\) inside the periodic trace \(\operatorname{Tr}[AB]/Z(T)\) works as follows:
- by \(\lvert\operatorname{Tr}[A'B']\rvert\le\lVert B'\rVert\operatorname{Tr}A'\), with the heat factors \(e^{-uH}\) moved into \(B'\);
- this leaves a trace of circumference \(T-2u\).

Hence the bound is
\[
Cu^{-\kappa}\,\frac{Z(T-2u)}{Z(T)}\times\Big(\text{periodic norm of }\tau_{t-u}F\text{ on a circle of length }T-2u\Big).
\]
The factor \(Z(T-2u)/Z(T)=\exp\int_{T-2u}^TE(v)\,dv\) is a thermal quantity, and so is the marked analogue. This is an identity for the factorization, not a no-go theorem for every conceivable argument. It shows that any proof passing through \(H_n\) must control the ratio of periodic traces at two circumferences. Only a genuinely Euclidean periodic estimate could bypass this.

## 3. Localization of \(\Phi_n\) to the terminal scale (conditional)

### 3.1 Hypotheses imported from T6

Use T6 (Infinite-volume scalar comparison, §2.5 and §3.4) for every admissible cubic torus \(R\):
- the representation \(Z_{a,R}=e^{A_a(R)}\Xi_{a,R}\), with the scalar recipe \(A_a(R)=\sum_{k\le K}\sum_{X}e^{(R)}_k(X)\) of T6 (3.2);
- the copying property (N\(_k\)), with \(\rho_k\le\rho_0(1+r)^v\) for \(r=K-k\);
- the decay property (D\(_k\)): \(\sum_{X\ni x,\,d(X)\ge D}\lvert e^{(R)}_k(X)\rvert\le C(1+r)^ue^{-\kappa D/(1+r)^v}\).

T6 states (N\(_k\)) and (D\(_k\)) as proved for the Gaussian-normalizer and coordinate-measure parts. They are **unverified** for the nonlinear E- and R''-terms (T6 §3.4(v), item R-2).

### 3.2 Statement

**Theorem 3 conditional.** Assume (N\(_k\)) and (D\(_k\)) for all \(k\le K_n\), and assume both \(T_n\) and \(T_n/L\) are admissible cubic periods. Then
\[
\Phi_n=\Psi_n+\epsilon_n,\qquad \Psi_n:=L^4\log\Xi_{a_n,T_n/L}-\log\Xi_{a_n,T_n},
\]
\[
\lvert\epsilon_n\rvert\le C(1+L^4)\sum_{r\ge0}\Big(\frac{L^rT_n}{\ell_0}\Big)^4(1+r)^u\exp\Big\{-\kappa\,\frac{L^rT_n/(2L\ell_0)-2\rho_0(1+r)^v}{(1+r)^v}\Big\}\xrightarrow[T_n/\ell_0\to\infty]{}0,
\]
uniformly in \(a_n\).

### 3.3 Proof

\(\Phi_n=[L^4A(T_n/L)-A(T_n)]+\Psi_n\). Let \(\pi\) be the \(L^4\)-fold covering of the \(T_n/L\)-torus by the \(T_n\)-torus; it induces coverings of every step-\(k\) lattice. Call a step-\(k\) carrier \(X\) of the small torus *short* if \(\operatorname{diam}X+2\rho_k<T_n/(2L\ell_k)\).

*Short carriers cancel.* A short \(X\) has exactly \(L^4\) connected lifts \(X'\), each mapped injectively. By (N\(_k\)), \(e^{(T_n)}_k(X')=e^{(T_n/L)}_k(X)\). Conversely, a connected \(X'\) with \(\pi(X')\) short and \(\pi\vert_{X'}\) injective is one of these lifts. So these terms cancel exactly in \(L^4A(T_n/L)-A(T_n)\).

*All other carriers are long.* Every remaining carrier on either torus has tree-length at least \(D_k=T_n/(2L\ell_k)-2\rho_k\). This holds trivially for non-short \(X\). It holds for an \(X'\) with \(\pi\vert_{X'}\) not injective because two of its points differ by a nonzero period of the small torus, so their distance is at least \(T_n/(L\ell_k)\).

*Sum the long carriers.* Sum (D\(_k\)) over the \((T_n/\ell_k)^4\) step-\(k\) sites of the large torus and the \(L^{-4}\) times as many of the small one, with multiplicities \(1\) and \(L^4\). Put \(\ell_k=L^{-r}\ell_0\). This gives the displayed bound. Each term decays faster than any power of \(T_n/\ell_0\), and the series in \(r\) converges because \(L^r/(1+r)^v\to\infty\). \(\square\)

**Corollary 3.1 conditional.** Under (N\(_k\)), (D\(_k\)) and (G), E-05's thermal criterion holds for all degrees on any admissible cubic sequence with \(L\mid N_n\) on which

\[
\textbf{(IR\(_{\rm term}\))}\qquad \Psi_n=L^4\log\Xi_{a_n,T_n/L}-\log\Xi_{a_n,T_n}=o(T_n).
\]

Here \(\Xi_{a,R}\) is the terminal integral of T6, over step-\(K\) links on a lattice of side \(R/\ell_0\), at the terminal coupling. The bounds of T6 (H1) control \(\log\Xi\) only to \(O((R/\ell_0)^4)\). As TS20 Part IV §5 already observed for its rectangular defect, subtracting such numbers gives no subextensive estimate. Theorem 3 shows that this terminal defect is the **only** part of E-05 not cancelled by ultraviolet structure, and that only cubes are involved.

## 4. The transverse Gaussian reference: thermal criterion holds, local criterion fails

### 4.1 The Gaussian theory and its thermal increment

**The Gaussian theory.** This is the quadratic, temporal-gauge, Gauss-law-projected, nonzero-momentum part of the Wilson transfer at weak coupling. It is the finite-cutoff construction "transverse quadratic reference".
- On the spatial torus \((\mathbb Z/N)^3\), lattice units, take \(d_G=N^2-1\) colours of real fields \(A_i(x)\). Let \(\mathcal T\) be the subspace with \(d^*A=0\) and \(\sum_xA=0\).
- The Gaussian Markov chain on \(\mathcal T\) has transfer kernel \(\exp\{-\frac\beta2[\lVert A-A'\rVert^2+\frac12(\lVert dA\rVert^2+\lVert dA'\rVert^2)]\}\), which is a positive operator.
- In Fourier variables \(\kappa_i=e^{ik_i}-1\), the space \(\mathcal T\) at \(k\ne0\) is \(\kappa^\perp\) (Hermitian). On it \(d^*d\) acts as \(\lambda(k)=\sum_i4\sin^2(k_i/2)\).
- So the Gaussian theory is a product of independent one-dimensional chains, two per colour per \(k\ne0\), with \(\lambda=\lambda(k)\).

**One-mode facts.** For the chain weight \(\exp\{-\frac\beta2[(q-q')^2+\frac\lambda2(q^2+q'^2)]\}\), define \(\omega>0\) by \(\cosh\omega=1+\lambda/2\).
- The kernel is \(\mathrm{const}\times\) Mehler's kernel in the variable \(x=q\sqrt{\beta\sinh\omega}\), since its exponent is \(-\frac\beta2[\cosh\omega(q^2+q'^2)-2qq']\).
- Hence the normalized transfer is \(e^{-\omega b^\dagger b}\) and \(Z_{\rm mode}(u)=(1-e^{-u\omega})^{-1}\).
- The vacuum law of \(q(0)\) is \(N(0,(2\beta\sinh\omega)^{-1})\).
- The periodic law over \(M\) steps is \(N(0,\coth(M\omega/2)(2\beta\sinh\omega)^{-1})\).

**Proposition 4.1.** On the cube (\(M=N\)),
\[
\Gamma^G=\sum_{\rm modes}\log\big(1+e^{-N\omega_k/2}\big)\le 2d_G\sum_{j\in\mathbb Z^3\setminus0}e^{-\lvert j\rvert}\approx 48.8\,d_G,
\]
uniformly in \(N,\beta\), and hence in \(a\) and \(T\).

*Proof.*
1. The increment per mode is \(\log[(1-e^{-N\omega})/(1-e^{-N\omega/2})]=\log(1+e^{-N\omega/2})\le e^{-N\omega/2}\).
2. With \(k=2\pi j/N\) and \(\lvert j_i\rvert\le N/2\), the bound \(\sin y\ge2y/\pi\) on \([0,\pi/2]\) gives \(\lambda\ge(4/\pi^2)\lvert k\rvert^2=16\lvert j\rvert^2/N^2\).
3. \(\sinh(\omega/2)=\sqrt\lambda/2\), and \(\operatorname{arcsinh}y\ge y/\sqrt{1+y^2}\). Since \(\lambda\le12\), this gives \(\omega\ge\sqrt\lambda/2\ge2\lvert j\rvert/N\).
4. Hence \(N\omega/2\ge\lvert j\rvert\). Each \(k\) carries \(2d_G\) modes, and the lattice sum is \(24.39\). \(\square\)

The exact values are \(\Gamma^G/(2d_G)\approx0.48\)–\(1.37\) for \(N=4\)–\(64\) (check 3).

### 4.2 The local criterion fails for the same model

**Proposition 4.2.** Fix \(h_*\in C_c^\infty(\mathbb R^3)\) with \(h_*\ge0\), \(\int h_*>0\) and support in the ball of radius \(R\). Put \(h(x)=h_*(ax)\) and \(X=\sum_xh(x)(dA^{1})_{12}(x,0)\), a time-zero smeared magnetic flux. Let \(\mu_n,\nu_n\) be the periodic-cube and vacuum laws of Annex V §2 for the same spatial transfer. Then, for \(T\ge T_0(h_*)\) and \(a\le a_0(h_*)\), with every cylinder containing the support,
\[
\delta_n\ \ge\ \mathrm{TV}\big(\mathcal L_{\mu_n}(X),\mathcal L_{\nu_n}(X)\big)\ \ge\ \frac{\phi(1)}{2\sqrt2}\min\Big(1,\frac{c_\pi\sqrt2}{16}\,\frac{(\int h_*)^2}{\lVert h_*\rVert_2\lVert\nabla h_*\rVert_2}\,T^{-4}\Big),
\]
where \(c_\pi=\coth\pi-1\) and \(\phi\) is the standard normal density.

*Proof.* Write \(\hat h(k)=\sum_xh(x)e^{-ik\cdot x}\) and \(w_k=(-\bar\kappa_2,\bar\kappa_1,0)\). Since \(\langle\kappa,w_k\rangle=0\), the vector \(w_k\) is transverse, and \(\lVert w_k\rVert^2=\lvert\kappa_1\rvert^2+\lvert\kappa_2\rvert^2\).

*Exact variances.* \(X\) is centered Gaussian under both laws, with
\[
\sigma^2:=\mathrm{Var}_\nu X=N^{-3}\sum_{k\ne0}\lvert\hat h(k)\rvert^2\frac{\lvert\kappa_1\rvert^2+\lvert\kappa_2\rvert^2}{2\beta\sinh\omega_k},\qquad
\mathrm{Var}_\mu X=\sigma^2+D,
\]
where \(D\) is the same sum weighted by \(\coth(N\omega_k/2)-1\ge0\).

*Upper bound on \(\sigma^2\).* Use \(\lvert\kappa_1\rvert^2+\lvert\kappa_2\rvert^2\le\lambda\), \(\sinh\omega\ge\sqrt\lambda/2\), Cauchy–Schwarz, Parseval and Riemann sums:
\[
\sigma^2\le\beta^{-1}\big(\textstyle\sum_xh^2\big)^{1/2}\big(\sum_x\lvert\nabla h\rvert^2\big)^{1/2}\le2\beta^{-1}a^{-2}\lVert h_*\rVert_2\lVert\nabla h_*\rVert_2.
\]

*Lower bound on \(D\).* Keep only \(k=\pm(2\pi/N)e_1\). There \(\lambda=\lvert\kappa_1\rvert^2=4\sin^2(\pi/N)\), \(\omega_1=2\operatorname{arcsinh}\sin(\pi/N)\le2\pi/N\) and \(\sinh\omega_1\le2\sqrt2\sin(\pi/N)\). Hence
\[
D\ge 2\sqrt2c_\pi\lvert\hat h(k_1)\rvert^2/(\beta N^4).
\]
Center the support at the origin and take \(T\ge6R\). Then \(\lvert\hat h(k_1)\rvert\ge\cos(\pi/3)\sum_xh\ge\frac14a^{-3}\int h_*\). Since \(N^4=T^4/a^4\),
\[
D/\sigma^2\ge c_\pi\sqrt2(\int h_*)^2/(16\lVert h_*\rVert\lVert\nabla h_*\rVert T^4).
\]

*Total variation.* For \(\varepsilon=D/\sigma^2\le1\), the event \(\{\lvert X\rvert\le\sigma\}\) gives \(2[\Phi(1)-\Phi((1+\varepsilon)^{-1/2})]\ge\phi(1)\varepsilon/(2\sqrt2)\). Restriction to a smaller sigma-algebra cannot increase total variation. \(\square\)

The ratio \(D/\sigma^2\) is independent of \(\beta\) and \(a\): it scales as \((R/T)^4\). Exact lattice sums give \(D\sigma^{-2}T^4\approx3.5\)–\(5.9\) for a Gaussian bump with \(R=1\) (check 4).

**Consequence.**
- If \(T_n\le Ca_n^{-k_0}\), then \(a_n^{-4k_0-1}\delta_n\to\infty\), so (E.13) fails.
- On B-02, \(H_n\le3K_n+C\), so \(T_n\le C(\ell_0/a_n)^3\ell_0\). The failure occurs at \(k=13\).
- The weaker finite-degree condition (E.15), with polynomial marks of degree \(m\) and \(d_W=4m\), fails for \(m\ge4\).

**Implications additional assumption.**
- The Gaussian reference is the Wick limit of the weak Wilson family of the finite-cutoff construction, and it is gapless at the scale \(T\). On the B-02 family, which is weakly coupled up to scale \(T_n\), the same \(T^{-4}\) local thermal correction is expected.
- The E-01 local route therefore needs either a mass gap or periods superpolynomial in \(1/a\). B-02's optional period enlargement permits the latter, but there (E.12) also fails because the multipliers are of order \(\beta\); see the finite-cutoff construction §4.
- The thermal route, by contrast, has \(\Gamma=O(1)\) here on **every** cubic geometry.
- This is the physically relevant instance of Annex V's statement that the two criteria are incomparable: on the free reference, the thermal criterion holds and the local one fails.

### 4.3 Exact extensive cancellation for torus determinants

**Lemma 4.3.** Let \(\Delta_m\) be the scalar lattice Laplacian on \((\mathbb Z/m)^d\), and let
\[
e_d=\int_{[-\pi,\pi]^d}\log\Big(\sum_\mu4\sin^2\frac{k_\mu}2\Big)\frac{d^dk}{(2\pi)^d}.
\]
Then for all \(m\ge2\), with \(C_d\) depending only on \(d\),
\[
\big\lvert\log\det{}'\Delta_m-m^de_d-2\log m\big\rvert\le C_d.
\]

*Proof.* Frullani's integral gives \(\log\lambda=\int_0^\infty(e^{-t}-e^{-t\lambda})\,dt/t\). The images formula gives \(\operatorname{Tr}e^{-t\Delta_m}=m^d\sum_{w\in\mathbb Z^d}p_t(mw)\), where \(p_t(x)=\prod_\mu e^{-2t}I_{x_\mu}(2t)\). Hence
\[
R(m):=\log\det{}'\Delta_m-m^de_d=\int_0^\infty\big(1-e^{-t}-\psi_m(t)\big)\frac{dt}t,\qquad \psi_m=m^d\sum_{w\ne0}p_t(mw).
\]
We bound the integral on three ranges.

*Range \(t\le1\).* The bound \(e^{-2t}I_k(2t)\le t^ke^{t^2}/k!\) gives \(\psi_m\le C_dm^dt^m/m!\). This range contributes \(O(1)\).

*Range \(1\le t\le m^2\).* Shift the contour in \(e^{-2t}I_k(2t)=\frac1{2\pi}\int e^{-ik\theta-2t(1-\cos\theta)}d\theta\) to \(\theta+is\), with \(s=\min(1,k/2.2t)\). This gives
\[
e^{-2t}I_k(2t)\le Ct^{-1/2}\exp[-\min(k^2/4.4t,k/2)].
\]
Hence \(\psi_m(t)\le C_d(m^2/t)^{d/2}e^{-\min(m^2/4.4t,\,m/2)}\), whose integral against \(dt/t\) is bounded. Also \(\int_1^{m^2}(1-e^{-t})\,dt/t=2\log m+O(1)\).

*Range \(t\ge m^2\).* Write the integrand as \(-e^{-t}-(\operatorname{Tr}e^{-t\Delta_m}-1)+m^dp_t(0)\). We have \(\operatorname{Tr}e^{-t\Delta_m}-1\le\sum_{j\ne0}e^{-16t\lvert j\rvert^2/m^2}\le C_de^{-16t/m^2}\), and \(m^dp_t(0)\le C_dm^dt^{-d/2}\). Both integrate to \(O(1)\) against \(dt/t\).

Collecting the three ranges proves the lemma. \(\square\)

Numerically, for \(d=4\), \(R(m)-2\log m\) decreases from \(-2.65\) at \(m=2\) to \(-1.70\) at \(m=32\) (check 5).

**Corollary 4.4.** \(\lvert L^4\log\det{}'\Delta_{N/L}-\log\det{}'\Delta_N\rvert\le(L^4+1)(2\log N+C_4)\).

On the torus, \(\Delta_1=d^*d+dd^*\) acts componentwise as \(\Delta_0\). So \(\det{}'(d^*d\vert_{\rm coexact\,1\text{-forms}})=(\det{}'\Delta_0)^{3}\) and \(\det{}'(dd^*\vert_{\rm exact})=\det{}'\Delta_0\). Every Gaussian determinant of the gauge-fixed 4D quadratic Wilson action is therefore a power of \(\det{}'\Delta_0\). Its contribution to \(\Phi\) has an exactly cancelling extensive part, and the remainder is \(O(\log N)\).

The remaining Gaussian constants are counts of modes and links multiplied by \(\log(2\pi/\beta)\) or by Haar volumes. Their extensive parts cancel identically, because \(L^4(N/L)^4=N^4\). They leave \(O(L^4\log\beta)\) from the finitely many zero modes.

*Caution.* The one-dimensional chain model of §4.1 omits the spatial zero-momentum sector, so it is not hypercubically symmetric. Theorem 2 does not apply to it, and its naive \(\Phi\) is \(O(N\log\beta)\). The exact 4D bookkeeping is essential; see §5.

## 5. The B-02 Wilson family: reduction to a finite-volume weak-coupling lemma

**Lemma (W) — not proved here.** There exist a function \(p(\beta)\) and constants \(C,c,C_0,C_1\), depending only on \(N\), with the following property. For every cubic torus of side \(m\ge2\) and every \(\beta\ge m^{C_0}\),
\[
\big\lvert\log Z^W_{\rm cube}(m;\beta)-m^4p(\beta)\big\rvert\le C(\log\beta+\log m)+Cm^{C_1}\beta^{-c}.
\]
The error \(o(m^{3/4})\) in place of \(C(\log\beta+\log m)\) would suffice on B-02.

**Theorem 5 conditional.** Assume (W). On the B-02 family, with \(L\mid N_n\),
\[
\Phi_n\le C(L^4+1)(\log\beta_{W,n}+\log N_n)+o(1)=o(T_n).
\]
If (S) and (G) also hold for the chosen prescription, the E-05 thermal criterion (4.5) holds for every fixed \(F\) of every degree on this family.

*Proof.* Apply (W) to \(m=N_n/L\) and \(m=N_n\); the terms \(m^4p\) cancel exactly. On B-02:
- \(\log N_n\le(H_n+K_n+1)\log L=O(n)\);
- \(\log\beta_{W,n}\le L^{n+O(1)}\) because \(r\ge2\);
- \(\beta_{W,n}\ge N_n^{C}\) eventually for every \(C\);
- \(T_n\ge2L^{3n}\ell_0\).

Then apply Corollary 2.1. \(\square\)

**Why (W) is expected, and what a proof needs additional assumption.** On B-02, \(\beta_{W,n}=\exp(L^{(2n+s+1/2)/r})\) exceeds every power of the lattice volume \(N_n^4\sim L^{16n}\). This is the regime of direct finite-volume weak coupling; no RG is needed. A proof would proceed in five steps.
1. **Large fields.** Remove them by the chessboard or Annex A reserve, as in TS20.2, at plaquette threshold \(\beta^{-1/2+\epsilon}\). The union bound costs \(m^4e^{-c\beta^{2\epsilon}}\to0\).
2. **Gauge fixing.** Use exact maximal-tree gauge, with no Jacobian. On the small-field set, every configuration lies within \(O(m\beta^{-1/2+\epsilon})\) per link of a flat configuration with commuting holonomies. For \(SU(N)\), commuting tuples are simultaneously diagonalizable.
3. **Gaussian integration.** At abelian flat backgrounds \(\theta\), the quadratic form is the twisted Laplacian, diagonal in roots and momenta. Its determinants are those of Lemma 4.3 twisted by \(\theta\). The \(\theta\)-dependence is subextensive by the winding (\(w\ne0\)) part of the images formula.
4. **Remainder terms.** Cubic and quartic remainders and Haar Jacobians cost \(m^{C}\beta^{-c}\) in total.
5. **Zero modes.** The moduli integral, including neighbourhoods of reducible holonomies where charged modes soften and quartic terms take over, costs \(e^{O(\log\beta+\log m)}\). Here only a crude bound is needed.

The genuinely delicate step is the **upper** bound for the small cube near reducible flat connections, which needs a uniform tubular-neighbourhood estimate for the commuting variety. The lower bound for the large cube follows from Jensen's inequality with a Gaussian trial measure on a neighbourhood of the trivial flat connection.

Note that (W) does **not** apply to the finite-cutoff construction comparison family. There the period is chosen with \(T\ge\beta_W^2\ell_0\), so the volume exceeds \(\beta\).

The B-02 family has vanishing terminal coupling. Its free limit does not establish the fixed-terminal-coupling thermal comparison.

## 6. Physically matched sequences: what remains is an infrared estimate

**Exact reductions (deduction; b).** For any admissible cubic sequence:
\[
\text{E-05 (thermal)}\ \Longleftarrow\ (G)+\big[\Phi_n=o(T_n)\big]\ \overset{\rm Thm\,3}{\Longleftarrow}\ (G)+(\mathrm N_k)+(\mathrm D_k)+\big[\Psi_n=o(T_n)\big].
\]
The minimal list of inputs for the sharpest conditional theorem is:
- (G), the coefficient growth bound;
- (N\(_k\)) and (D\(_k\)) of T6 for the nonlinear E- and R''-terms. These are ultraviolet properties of the source-free construction;
- (IR\(_{\rm term}\)): \(\Psi_n=o(T_n)\).

The renormalized slab premise (4.12) is needed only to *use* the criterion (E-02 to E-04), not for E-05.

**Assessment additional assumption.**
- At fixed terminal coupling \(g_*>0\), \(\Psi_n\) compares terminal compact gauge integrals on lattices of sides \(T_n/(L\ell_0)\) and \(T_n/\ell_0\), at one fixed weak coupling. It is the finite-size free energy of a fixed-coupling lattice gauge theory on growing cubes, which must be sublinear in the side.
- For a gapped theory \(\Psi\) is exponentially small. For a gapless one at weak coupling it is of order \(1+\log\) (§4–5).
- At intermediate scales, where the coupling runs to strong values, no method in the sources controls it better than \(O((T/\ell_0)^4)\). This is the same infrared content as TS20 Part IV §5's "stopping scale obstruction", now reduced to cubes alone.
- F-05 and M-07 construct normalized observables and matching at fixed physical scales. \(\Phi_n\) and \(\Psi_n\) are bare and observable-free, and they are governed by scales of order \(T_n\). So the finite-cutoff construction deferral to F-05/M-07 does not address the obstacle; only (G) links E-05 to the matching proposition.
- The known alternative is the time-first rectangular geometry (Annex C §4). There the state passage is trivial, since a fixed-volume large-time limit is legitimate. Its cost is the local restoration of the time–space permutation symmetry used by the rotation proposition. Heuristically this is the same comparison of two geometries, and equally sensitive to the infrared.
