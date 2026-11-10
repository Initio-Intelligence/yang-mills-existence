# Compact SU(2) operators and the periodic-state criterion

**Annex M.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

The interacting physical operator obligation **E0 remains open**. The new results are:

1. **P — an actual compact-Wilson estimate.** For SU(2), a representation-uniform kinetic multiplier inequality improves the bare temporal plaquette bound from the previous square-root weak-coupling estimate to \(O((1+\log\beta)/\beta)\), with an actual closed-field domain. Spatial interactions and every compact field configuration are retained.
2. **C — a proved bridge on the existing cubic sequence.** Uniform renormalized ground-Hamiltonian slabs imply the required periodic OS insertion inequality if a specified thermal trace increment is sublinear in the physical time side and each fixed polynomial has a controlled cutoff norm. The proof does not assume a rectangular extension of Balaban's construction, does not require a uniform mass gap, and does not replace a periodic state by a ground state without an estimate.
3. **P — a sharp obstruction to omitting state control.** Strictly positive finite transfer matrices can satisfy uniform ground-Hamiltonian slabs, Gaussian full-hierarchy and complex-source bounds, and an extensive pressure bound, while their periodic limits have an unbounded constant field and zero Hamiltonian. Thus those hypotheses alone do not prove the periodic-limit operator estimate.

Here P means the displayed assertion is proved, C a proved implication with unverified Yang–Mills premises, L a scoped primary-source input, and O an unproved Yang–Mills assertion. No novelty claim is made. The separate vacuum-block criterion in Annex L can transfer a prescribed ultraviolet coefficient without first deriving this operator estimate. The operator work remains necessary for the requested energy bounds and for any phase-decomposition route that uses them.

### 1. Normalization and the retained compact transfer comparison

Use normalized Haar measure and

\[
s(g)=N-\operatorname{Re}\operatorname{Tr}g,\qquad
\beta=2Nx_0,\qquad X_B=N\beta=2N^2x_0.
\tag{1.1}
\]

At a finite spatial cutoff, on the full link Hilbert space, put

\[
\begin{aligned}
Z_1(\beta)&=\int_G e^{-\beta s(g)}\,dg,\\
(C_\beta f)(u)&=Z_1(\beta)^{-1}
 \int_G e^{-\beta s(uv^{-1})}f(v)\,dv,\\
K&=\bigotimes_{l}C_\beta,\qquad
V_s=\beta\sum_{p\ {\rm spatial}}s(U_p),\\
A&=e^{-V_s/2},\qquad T_0=AKA.
\end{aligned}
\tag{1.2}
\]

Gauge projection commutes with these operators. The physical restriction \(T\) has the same simple positive largest eigenvalue \(\lambda_0\) as \(T_0\). Set \(H=-a^{-1}\log(T/\lambda_0)\ge0\). The compact positive kernel and positive Fourier coefficients are used here, rather than a small-field approximation. The source normalization dictionary in (1.1) is unchanged.

The following already-proved local comparison is the starting point. For a finite link set \(\Gamma\), delete exactly the spatial plaquettes incident on \(\Gamma\), denote the top eigenvalue of the remaining transfer factor by \(\lambda_r\), and set

\[
\Delta_\Gamma=\log(\lambda_r/\lambda_0)\ge0.
\tag{1.3}
\]

If \(K^{1/2}A=WT_0^{1/2}\) is the polar decomposition, then \(W\) is unitary, commutes with gauge projection, and

\[
\boxed{W^*L_\Gamma W\le aH+\Delta_\Gamma I,\qquad
L_\Gamma=-\log K_\Gamma}
\tag{1.4}
\]

as closed quadratic forms. The direct bound is
\(\Delta_\Gamma\le2N\beta|\mathcal P_\Gamma|\).
On the compatible spatial geometry used there, with all incident plaquettes fitting in a fixed \(B\)-site cube,

\[
0\le\Delta_\Gamma
\le B^3\{c_N+2(N^2-1)\log(1+\beta)\}.
\tag{1.5}
\]

Equation (1.5) was proved by a compact-Wilson cylinder reserve and a trace limit at each fixed spatial cutoff. That elementary auxiliary Wilson integral does not import a rectangular source-free RG theorem. The unitary \(W\) is not asserted to be spatially local.

One also retains the proved closed-domain consequence. If a central multiplier on \(\Gamma\) satisfies

\[
|F_{\boldsymbol\lambda}|
\le A_F(b+\ell_\Gamma(\boldsymbol\lambda))^r,\qquad
\ell_\Gamma=\sum_{l\in\Gamma}-\log c_{\lambda_l},\quad r\ge1,
\tag{1.6}
\]

then its exact midpoint realization \(O_F=W^*FW\) is closed, its Hermitian version is selfadjoint, and

\[
\begin{aligned}
D((1+H)^{r+1})&\subset D(O_F),\\
\|O_F(1+H)^{-(r+1)}\|
&\le 2^{r+1}A_F(eb+2r+\Delta_\Gamma+a)^r .
\end{aligned}
\tag{1.7}
\]

This statement comes from range factorization of fractional transfer powers, followed by a dyadic spectral sum; no form inequality is squared.

### 2. A representation-uniform SU(2) kinetic inequality

This section specializes to \(G=SU(2)\). Write \(n=1,2,\ldots\) for the dimension of an irreducible representation, and let \(I_\nu\) denote the modified Bessel function.

#### 2.1 Exact one-link Fourier coefficients

For class angle \(\theta\), normalized Haar class measure is
\(2\pi^{-1}\sin^2\theta\,d\theta\),
\(s=2-2\cos\theta\), and
\(\chi_n(\theta)=\sin(n\theta)/\sin\theta\).
Consequently

\[
\begin{aligned}
a_n(\beta)
&=\frac1n\int_{SU(2)}e^{-\beta s(g)}\chi_n(g)\,dg\\
&=\frac{e^{-2\beta}}n
 \{I_{n-1}(2\beta)-I_{n+1}(2\beta)\}
 =e^{-2\beta}\frac{I_n(2\beta)}{\beta}.
\end{aligned}
\tag{2.1}
\]

The last equality follows either by termwise differentiation of the power series or by integration by parts. Therefore

\[
c_n(\beta)=\frac{a_n(\beta)}{a_1(\beta)}
 =\frac{I_n(2\beta)}{I_1(2\beta)},\qquad
\ell_n(\beta)=-\log c_n(\beta).
\tag{2.2}
\]

Only standard defining Bessel formulas are used below. They are recorded in the official DLMF at [10.25.2](https://dlmf.nist.gov/10.25.E2), [10.32.2](https://dlmf.nist.gov/10.32.E2), and [10.32.3](https://dlmf.nist.gov/10.32.E3). The inequality that follows is proved here rather than imported from that reference.

#### 2.2 Ratio lemma

**Lemma 2.1 (P).** For \(\nu\ge1\), \(x>0\), and
\(r_\nu(x)=I_{\nu+1}(x)/I_\nu(x)\),

\[
0<r_\nu(x)<1,\qquad
0\le x\frac{r_\nu'(x)}{r_\nu(x)}
\le \frac{-\log r_\nu(x)}{\log2}.
\tag{2.3}
\]

**Proof.** The integral representation

\[
I_\nu(x)=\frac{(x/2)^\nu}
 {\sqrt\pi\,\Gamma(\nu+1/2)}
 \int_{-1}^{1}e^{xt}(1-t^2)^{\nu-1/2}\,dt
\tag{2.4}
\]

and \(I_\nu'=I_{\nu+1}+\nu I_\nu/x\) identify \(r_\nu\) with the mean of \(t\) under the probability density proportional to the integrand. Thus
\(0<r_\nu<1\) and \(r_\nu'=\operatorname{Var}(t)>0\).

There are two elementary upper bounds. First, write

\[
I_\nu(x)=\frac{(x/2)^\nu}{\Gamma(\nu+1)}
A_\nu(x^2/4),\qquad
A_\nu(z)=\sum_{k\ge0}\frac{z^k}{k!(\nu+1)_k}.
\tag{2.5}
\]

Here \((b)_k=b(b+1)\cdots(b+k-1)\), with \((b)_0=1\).
Then \(A_{\nu+1}(z)/A_\nu(z)\) is the mean of
\((\nu+1)/(\nu+1+k)\) under the probability weights proportional to the summands of \(A_\nu\).
Its derivative with respect to \(\log z\) is the covariance of this decreasing function with \(k\), and is nonpositive. Since

\[
\frac{r_\nu(x)}x
=\frac1{2(\nu+1)}
 \frac{A_{\nu+1}(x^2/4)}{A_\nu(x^2/4)},
\]

we obtain
\[
x r_\nu'(x)\le r_\nu(x).
\tag{2.6}
\]

For the second bound set \(u=1-t\) and \(A_\nu^0=\nu-\tfrac12>0\).
The density of \(u\) is proportional to
\(e^{-xu}[u(2-u)]^{A_\nu^0}\), \(0<u<2\).
Integration of the derivative of \(u\) times that density gives

\[
x\,\mathbb E u
= A_\nu^0+1-A_\nu^0\mathbb E\frac{u}{2-u}.
\tag{2.7}
\]

The endpoint terms vanish; the displayed expectations and their \(x\)-derivatives are integrable for \(\nu\ge1\).
Differentiation yields

\[
x\operatorname{Var}(u)
=\mathbb E u-A_\nu^0
 \operatorname{Cov}\!\left(u,\frac{u}{2-u}\right)
\le\mathbb E u.
\tag{2.8}
\]

The covariance is nonnegative because both functions increase. Therefore

\[
x r_\nu'(x)\le1-r_\nu(x).
\tag{2.9}
\]

Combining (2.6) and (2.9),
\[
x(\log r_\nu)' \le
\min\{1,(1-r_\nu)/r_\nu\}
\le(-\log r_\nu)/\log2.
\]
For \(r_\nu\le1/2\), the last assertion follows from
\(-\log r_\nu\ge\log2\). For \(1/2\le r_\nu<1\), concavity of \(-r\log r\) above the chord joining its values at \(1/2\) and \(1\) gives
\(-r\log r\ge(1-r)\log2\). This proves (2.3). ∎

**Theorem 2.2 (P: all representations and all couplings).** For every \(n\ge1\) and \(\beta>0\),

\[
\boxed{
0\le\beta\,\partial_\beta\log c_n(\beta)
\le\frac{\ell_n(\beta)}{\log2}.}
\tag{2.10}
\]

**Proof.** For \(n\ge2\),
\(c_n(\beta)=\prod_{\nu=1}^{n-1}r_\nu(2\beta)\).
Sum (2.3), using
\(\beta\partial_\beta=x\partial_x\) at \(x=2\beta\).
For \(n=1\), both sides vanish. ∎

Let

\[
\mu_\beta=\frac{\int s(g)e^{-\beta s(g)}\,dg}{Z_1(\beta)}
 =-\partial_\beta\log Z_1(\beta).
\tag{2.11}
\]

Equations (2.1) and (2.4) give
\[
\mu_\beta=2(1-r_1(2\beta)),\qquad
0<\mu_\beta\le\min\{2,3/(2\beta)\}.
\tag{2.12}
\]
The \(3/(2\beta)\) bound follows directly from (2.7), dropping its last nonnegative term at \(\nu=1\).

The exact multiplier of the unnormalized temporal mark \(s\) is
\(F_n=-a_n'/a_n\). Therefore

\[
\boxed{
0\le\mu_\beta-F_n
=\partial_\beta\log c_n
\le\frac{\ell_n}{\beta\log2}.}
\tag{2.13}
\]

This inequality includes high representations. It is stronger than a fixed-representation weak-coupling expansion.

### 3. Consequences for the full interacting compact-Wilson operator

Take one temporal plaquette based on a spatial link \(l\), and let \(\Gamma\) contain that link. Its exact selfadjoint midpoint field is
\(O_s=W^*F_lW\).
All spatial action factors remain in \(W\) and \(H\).

**Theorem 3.1 (P).** Define \(D_l=\mu_\beta I-O_s\). Then

\[
\boxed{
0\le D_l\le\frac{aH+\Delta_\Gamma I}{\beta\log2}}
\tag{3.1}
\]

as closed forms, and

\[
\begin{aligned}
D((1+H)^2)&\subset D(D_l),\\
\|D_l(1+H)^{-2}\|
&\le\frac{4(2+\Delta_\Gamma+a)}{\beta\log2}.
\end{aligned}
\tag{3.2}
\]

Let \(\Omega\) be the normalized physical ground vector and set
\[
m_l=\langle\Omega,O_s\Omega\rangle,\qquad
Q_l=O_s-m_lI.
\tag{3.3}
\]
Then, for every \(t>0\),

\[
\boxed{
\|e^{-tH}Q_l e^{-tH}\|
\le\frac{\Delta_\Gamma+a/(2et)}{\beta\log2}}
\tag{3.4}
\]

and

\[
\boxed{
\|Q_l(1+H)^{-2}\|
\le\frac{8+5\Delta_\Gamma+4a}{\beta\log2},
\qquad D((1+H)^2)\subset D(Q_l).}
\tag{3.5}
\]

**Proof.** Combine (2.13) and (1.4) for (3.1). Apply (1.7) to the nonnegative multiplier \(\mu_\beta-F_l\), with
\(r=1\), \(b=0\), and \(A_F=(\beta\log2)^{-1}\), to obtain (3.2). This also places \(\Omega\) in the actual operator domain.

Let \(c_l=\mu_\beta-m_l=\langle\Omega,D_l\Omega\rangle\).
Then
\[
0\le c_l\le\Delta_\Gamma/(\beta\log2).
\tag{3.6}
\]
The heat-domain result underlying (1.7) makes
\(B_D=e^{-tH}D_le^{-tH}\) an actual bounded positive operator.
The form bound gives
\[
0\le B_D,\qquad
\|B_D\|\le
\frac{\Delta_\Gamma+a\sup_{h\ge0}he^{-2th}}{\beta\log2}
=\frac{\Delta_\Gamma+a/(2et)}{\beta\log2}.
\tag{3.7}
\]
Now
\(e^{-tH}Q_le^{-tH}=c_le^{-2tH}-B_D\).
For positive bounded operators \(B,C\), the selfadjoint difference satisfies
\(\|B-C\|\le\max(\|B\|,\|C\|)\); this follows from
\(-\|C\|I\le B-C\le\|B\|I\).
Use this with (3.6)–(3.7), giving (3.4) without a factor of two.
Finally \(Q_l=c_lI-D_l\), so (3.2) and (3.6) give (3.5). ∎

On the compatible geometry of (1.5), both constants are
\(O((1+\log\beta)/\beta)\) at fixed \(t>0\) and \(0<a\le1\), uniformly in total spatial volume. This improves the earlier square-root logarithmic estimate for this SU(2) channel.

The physical ultraviolet loss has not disappeared. If the prescribed dimension-four field is
\[
Q^R_{l,a}=z_a a^{-4}Q_l+d_{a,V,\mu}I,
\tag{3.8}
\]
then the theorem proves only
\[
\|e^{-tH}Q^R_{l,a}e^{-tH}\|
\le |z_a|a^{-4}
 \frac{\Delta_\Gamma+a/(2et)}{\beta\log2}
 +|d_{a,V,\mu}|.
\tag{3.9}
\]
Spatial smearing costs the lattice \(L^1\) norm of the test and a finite orientation factor, rather than the full spatial volume. The factor \(a^{-4}\), the correct subtraction \(d_{a,V,\mu}\), mixing, and the remaining tensor channels still require renormalized estimates. This theorem does not extend (2.10) to arbitrary \(SU(N)\).

For a temporal-only coupling variation, ground normalization makes \(Q_l\) the exact centered transfer response. The completely positive response transform therefore gives the corresponding logarithmic-Hamiltonian response bound with its explicit factor \(a^{-1}\). That identity supplies no additional ultraviolet cancellation.

### 4. A same-cubic-geometry bridge from Hamiltonian slabs to periodic OS forms

#### 4.1 Setup and precise state hypothesis

Let \(a_n\downarrow0\) and \(T_n\uparrow\infty\) be the existing cofinal cubic sequence, with \(T_n/a_n\) even. At the finite spatial cutoff of side \(T_n\), let
\[
P_n=e^{-a_nH_n},\qquad H_n\ge0,\qquad
\mathcal Z_n(u)=\operatorname{Tr}e^{-uH_n}.
\tag{4.1}
\]
The normalization is by the largest eigenvalue of the same Wilson transfer operator as above.

Define the **spectral** trace increment
\[
\Gamma_n=\log\frac{\mathcal Z_n(T_n/2)}
 {\mathcal Z_n(T_n)}\ge0.
\tag{4.2}
\]
This is a trace of an already defined finite-spatial-volume operator. No source-free RG theorem on a rectangular torus of temporal side \(T_n/2\) is assumed. Trace class at these long times follows at fixed cutoff from the trace-class transfer operator.

For each fixed positive-time polynomial test \(F\), with all its actual lattice stencils contained in a fixed compact time interval, let \(A_{F,n}\) be its positive-half-circle transfer kernel. Write
\[
A_{F,n}=e^{-(T_n/2-r_{F,n})H_n}X_{F,n},\qquad
0\le r_{F,n}\le R_F<\infty,
\tag{4.3}
\]
where \(X_{F,n}\) is a bounded marked slab. The last support time and stencil margin can be included in \(r_{F,n}\). Exact reflection gives
\[
p_n(F)^2=\frac{\|A_{F,n}\|_2^2}{\mathcal Z_n(T_n)}.
\tag{4.4}
\]
Assume the selected full hierarchy converges, so \(p_n(F)^2\to p(F)^2<\infty\).

The sufficient state-and-mark condition is
\[
\boxed{
\frac{\Gamma_n+2\log^+\|X_{F,n}\|}{T_n}\longrightarrow0
\quad\hbox{for every fixed }F.}
\tag{4.5}
\]
Here \(\log^+x=\max(0,\log x)\), with \(\log^+0=0\).
A convenient stronger formulation is
\[
\boxed{
\Gamma_n/T_n\to0,\qquad
\log(1/a_n)/T_n\to0,\qquad
\|X_{F,n}\|\le C_Fa_n^{-d_F}.}
\tag{4.6}
\]
The exponent \(d_F\) and constant \(C_F\) may depend on the fixed polynomial, its degree, and its component tests. They are not required to be uniform over all polynomials. The final slab constant will be uniform over them.

The geometric middle condition is compatible with the proposed sequence
\(a_n=L^{-K_n}\ell_0,\ T_n=2L^{M_n}\ell_0\); for example \(K_n=M_n=n\) satisfies it. This geometric choice does not prove the first condition.

#### 4.2 Hilbert–Schmidt interpolation, including OS-null limits

**Lemma 4.1 (P).** Under (4.3)–(4.5), for every bounded sequence \(t_n\ge0\) converging to a fixed \(t\),
\[
\boxed{
\frac{\|e^{t_nH_n}A_{F,n}\|_2^2}{\mathcal Z_n(T_n)}
-p_n(F)^2\longrightarrow0.}
\tag{4.7}
\]
All terms are defined once \(n\) is large enough. In particular this includes limits with \(p(F)=0\).

**Proof.** Put
\[
S_{F,n}=T_n/4-r_{F,n}>0,\qquad
q_{F,n}(u)=\frac{\|e^{uH_n}A_{F,n}\|_2^2}
 {\mathcal Z_n(T_n)},\quad0\le u\le S_{F,n}.
\tag{4.8}
\]
At the upper endpoint,
\[
\begin{aligned}
q_{F,n}(S_{F,n})
&=\frac{\operatorname{Tr}
 [X_{F,n}^*e^{-(T_n/2)H_n}X_{F,n}]}
 {\mathcal Z_n(T_n)}\\
&\le\|X_{F,n}\|^2 e^{\Gamma_n}.
\end{aligned}
\tag{4.9}
\]
Thus \(\log^+q_{F,n}(S_{F,n})=o(S_{F,n})\).

Using the spectral resolution of \(H_n\), \(q_{F,n}(u)\) is the Laplace transform of a positive measure with variable \(2u\). It is nondecreasing, since \(H_n\ge0\), and is log-convex by Hölder. Therefore, for \(0\le t_n\le S_{F,n}\),
\[
q_{F,n}(0)\le q_{F,n}(t_n)
\le q_{F,n}(0)^{1-t_n/S_{F,n}}
     q_{F,n}(S_{F,n})^{t_n/S_{F,n}}.
\tag{4.10}
\]
If \(q_{F,n}(0)=0\), then \(A_{F,n}=0\) and every term is zero.
Otherwise use \(q_{F,n}(0)=p_n(F)^2\).
When \(p(F)^2>0\), (4.10) and (4.9) squeeze the limit to \(p(F)^2\).
When \(p(F)=0\), eventually \(q_{F,n}(0)\le1\) and \(t_n/S_{F,n}\le1/2\), so
\[
q_{F,n}(t_n)
\le q_{F,n}(0)^{1/2}
 \exp\!\left[\frac{t_n}{S_{F,n}}
                  \log^+q_{F,n}(S_{F,n})\right]\longrightarrow0.
\tag{4.11}
\]
This proves (4.7), including null limits. ∎

#### 4.3 The field norm that this interpolation can transfer

Assume, in addition, an actual Hermitian renormalized one-field insertion \(q_{\alpha,n}(g)\) whose midpoint placements agree with the chosen hierarchy. Its compatible form sandwiches are assumed to satisfy
\[
\boxed{
\|e^{-uH_n}q_{\alpha,n}(g)e^{-uH_n}\|
\le C u^{-\kappa}\rho_s(g),\qquad0<u\le1,}
\tag{4.12}
\]
uniformly in \(n\), with fixed \(C,\kappa,s\), where
\(\rho_s(g)=\sum_{|\beta|\le s}\|\partial^\beta g\|_{L^1(\mathbb R^3)}\).
Reality and adjoint labels include the stipulated Wick phases. This is the renormalized Hamiltonian slab premise; the bare estimate in Section 3 does not prove it.

For lattice shifts \(t_n\to t>0\) and a central time \(\delta\), the exact thermal insertion identity is
\[
\begin{aligned}
N_{n,t_n,\delta}(F,G)
&=\frac1{\mathcal Z_n(T_n)}
\operatorname{Tr}\!\left[
A_{F,n}^*e^{2t_nH_n}A_{G,n}
B_{n,t_n,\delta}\right],\\
B_{n,t_n,\delta}
&=e^{-(t_n-\delta)H_n}
 q_{\alpha,n}(g)e^{-(t_n+\delta)H_n}.
\end{aligned}
\tag{4.13}
\]
The formula follows from
\(A_{\tau_tF}=e^{tH_n}A_Fe^{-tH_n}\), then cyclicity of the trace. Exact half-step midpoint locations are retained; a finite shrinking stencil is accommodated by its actual support buffer.

For \(|\delta|<t/8\), and eventually \(t_n\) sufficiently close to \(t\), both heat times, after allowing this stencil buffer, exceed \(t/2\). Factor out the symmetric sandwich at \(t/2\). Equation (4.12) gives
\[
\|B_{n,t_n,\delta}\|
\le 2^\kappa Ct^{-\kappa}\rho_s(g).
\tag{4.14}
\]
Apply the Hilbert–Schmidt Cauchy–Schwarz inequality in (4.13):
\[
|N_{n,t_n,\delta}(F,G)|
\le 2^\kappa Ct^{-\kappa}\rho_s(g)
\sqrt{q_{F,n}(t_n)q_{G,n}(t_n)}.
\tag{4.15}
\]
This bound is uniform in the allowed central location. It is not obtained by declaring periodic translations to be contractions.

**Theorem 4.2 (C: same-cubic transfer to the reduced periodic OS hypothesis).** Assume exact cutoff transfer realizations (4.3)–(4.4), convergence of the chosen hierarchy, the condition (4.5), and the renormalized bound (4.12). For every fixed positive-time complex polynomial \(F\), every fixed real spatial test \(g\), \(0<t\le1\), and every fixed nonnegative even mollifier
\(\chi_\epsilon(u)=\epsilon^{-1}\chi(u/\epsilon)\) with \(\epsilon<t/8\), the actual periodic hierarchy satisfies
\[
\begin{aligned}
&\left|S_n\bigl((\Theta\tau_tF)
 Q_{\alpha,n}(\chi_\epsilon\otimes g)(\tau_tF)\bigr)\right|\\
&\qquad\le C' t^{-\kappa}\rho_s(g)\,p_n(F)^2
 +\varepsilon_n(F,t,\epsilon,g,\alpha),\qquad
\varepsilon_n\longrightarrow0,
\end{aligned}
\tag{4.16}
\]
where \(C'\) is independent of \(F\), its polynomial degree, and \(\epsilon\).
Consequently the periodic OS slab-to-domain theorem applies, subject to its J1–J3 premises.

**Proof.** Integrate (4.15), with \(G=F\), against the nonnegative lattice sampling of \(\chi_\epsilon\). At each fixed \(\epsilon\), its lattice \(L^1\) sum tends to one and is eventually at most two, including a fixed half-step sampling shift. Thus \(C'=2^{\kappa+1}C\) is sufficient. Lemma 4.1 replaces \(q_{F,n}(t_n)\) by \(p_n(F)^2\), with an error tending to zero for this fixed \(F,t\).

Fine-lattice shifts \(t_n\to t\) and the actual stencil placements converge in the chosen hierarchy by its uniform distribution continuity. That convergence adds another test-dependent vanishing error. Products are evaluated on the coincidence-flat positive-time test algebra, so separated support groups do not introduce an uncontrolled contact distribution. The finite-cutoff scheme must actually have these transfer realizations; they are not inferred merely from symmetry of a counterterm.

The exponents \(d_F\) in (4.6), if used, occur only in the error through \(\log\|X_{F,n}\|/T_n\). They do not enter \(C'\), so the estimate retains the degree-independent constant required in the previous operator theorem. ∎

The order of limits is essential and unchanged: first \(n\to\infty\) at every fixed \(\epsilon>0\); then \(\epsilon\downarrow0\) in the already constructed continuum bounded forms. The previous semigroup regularity and convolution argument gives operator-norm unsmearing and the common spacetime-field domain. No estimate for \(\epsilon=\epsilon(a_n)\) is asserted.

#### 4.4 Where the polynomial mark budget comes from

There is a simple sufficient cutoff bound for \(X_{F,n}\). Suppose the explicitly chosen compact one-field representatives, including their mixing and identity coefficients, have pointwise bound
\[
|\Phi_{\alpha,n}^R|\le C_\alpha a_n^{-b_\alpha}.
\tag{4.17}
\]
This is a finite polynomial normalization budget, not a uniform renormalized estimate. Logarithmically running coefficients satisfy such a budget after increasing the exponents. Required finite product-subtraction coefficients must obey corresponding finite budgets, or annihilate the tests by their shrinking coincidence support.

For a fixed polynomial \(F\), compact smearing and bounded lattice \(L^1\) sums yield a Euclidean path-mark bound
\[
\|F_n\|_\infty\le C_Fa_n^{-d_F}.
\tag{4.18}
\]
The exponent can increase with the degree of \(F\). No assertion of a single exponent for all degrees is needed.

Let \(K_{F,n}(u,v)\) be the unnormalized marked path kernel through its finite time interval and \(K_{r,n}\) the unmarked kernel. Positivity of every compact Wilson path density gives
\[
|K_{F,n}(u,v)|\le\|F_n\|_\infty K_{r,n}(u,v).
\tag{4.19}
\]
For \(f\in L^2\), this implies pointwise
\(|K_{F,n}f|\le\|F_n\|_\infty K_{r,n}|f|\).
Consequently, after division by the appropriate power of \(\lambda_0\),
\[
\|X_{F,n}\|\le\|F_n\|_\infty\|e^{-rH_n}\|
\le C_Fa_n^{-d_F}.
\tag{4.20}
\]
Gauge projection is contractive and preserves the same estimate. This argument treats all time-overlapping compact stencils together as a path mark, so it does not incorrectly replace an unbounded midpoint operator by its Euclidean sup norm. It incurs no total-volume factor.

#### 4.5 What the thermal condition means and what has not been proved

Whenever the derivative is taken at these trace-class times,
\[
\Gamma_n
=\int_{T_n/2}^{T_n}
\frac{\operatorname{Tr}(H_ne^{-uH_n})}
 {\operatorname{Tr}e^{-uH_n}}\,du.
\tag{4.21}
\]
Thus \(\Gamma_n=o(T_n)\) asks for a vanishing average *total* thermal excitation energy in this low-temperature interval. It does not require the thermal ground-state probability to tend to one, and it does not assume a positive mass gap. A cubic sequence still changes the spatial transfer operator when time grows.

The source-free pressure estimate of order physical four-volume, by itself, does not give (4.5) or (4.6). Nor does finite-cutoff uniqueness of the ground state. No available Balaban theorem is claimed here to establish this trace increment. The next section shows why an additional assertion of this type, or a direct periodic inequality, is needed for the proposed Hamiltonian bridge.

### 5. A positive-transfer counterexample to an automatic periodic energy bound

This example is finite dimensional at every cutoff and has a strictly positive transfer kernel. It is not a Wilson gauge model and is not claimed to satisfy Yang–Mills field identification. Its purpose is to refute a general inference from ground-Hamiltonian slab estimates and source/pressure bounds to an operator bound in an expanding periodic limit.

#### 5.1 Cofinal parameters and a strictly positive transfer matrix

Fix an odd \(L\ge3\), set the physical reference length to one, and use
\[
a_n=L^{-n},\qquad T_n=2L^n,\qquad
N_n=T_n/a_n=2L^{2n},\qquad E_n=T_n^2.
\tag{5.1}
\]
Thus the time step count is even and these are the same cubic cofinal scales.
Let
\[
D_n=2\left\lceil e^{2T_nE_n}/2\right\rceil,\qquad
\mathcal H_n=\mathbb C^{D_n},\qquad
\Omega_n=D_n^{-1/2}(1,\ldots,1).
\tag{5.2}
\]
Write \(\Pi_n=|\Omega_n\rangle\langle\Omega_n|\), \(R_n=I-\Pi_n\), and define
\[
H_n=E_nR_n,\qquad
P_n=e^{-a_nH_n}
=\eta_nI+(1-\eta_n)\Pi_n,\quad
\eta_n=e^{-a_nE_n}.
\tag{5.3}
\]
Every matrix entry of \(P_n\) is strictly positive. It is symmetric, positive definite, stochastic, and has unique normalized ground vector \(\Omega_n\). Its nonzero excitation energy is \(E_n\), which tends to infinity.

#### 5.2 A bounded cutoff field with uniform Gaussian marginals

Let \(\Phi\) be the standard Gaussian distribution function and define
\[
q_{j,n}
=D_n\int_{(j-1)/D_n}^{j/D_n}\Phi^{-1}(u)\,du,
\qquad
Q_n=\operatorname{diag}(q_{1,n},\ldots,q_{D_n,n}).
\tag{5.4}
\]
The even number of bins and Gaussian symmetry give
\[
\langle\Omega_n,Q_n\Omega_n\rangle=0.
\tag{5.5}
\]
Conditional Jensen gives, for every \(p\ge1\),
\[
\frac1{D_n}\sum_j|q_{j,n}|^p\le\mathbb E|G|^p,
\qquad G\sim N(0,1).
\tag{5.6}
\]
In particular \(\|Q_n\Omega_n\|\le1\).
For any bin of probability \(D_n^{-1}\) and real \(z\),
\[
e^{zq_{j,n}}\le
D_n\,\mathbb E e^{zG}=D_ne^{z^2/2}.
\]
Optimizing \(z\) with either sign gives
\[
\|Q_n\|\le\sqrt{2\log D_n}\le3E_n.
\tag{5.7}
\]
The last inequality holds for the present \(T_n\ge1\), since
\(\log D_n\le2T_n^3+\log3\).

The quantile step functions in (5.4) converge pointwise on \(0<u<1\) to \(\Phi^{-1}(u)\). Their \(L^{2p}\) norms are uniformly bounded by Jensen. Hence they converge in \(L^p\) for each finite \(p\), and
\[
\mu_{m,n}:=D_n^{-1}\operatorname{Tr}Q_n^m
\longrightarrow\mathbb E G^m.
\tag{5.8}
\]

#### 5.3 Uniform ground-Hamiltonian slab estimates

Since \(\Pi_nQ_n\Pi_n=0\),
\[
e^{-tH_n}Q_ne^{-tH_n}
=e^{-tE_n}(\Pi_nQ_nR_n+R_nQ_n\Pi_n)
 +e^{-2tE_n}R_nQ_nR_n.
\tag{5.9}
\]
Equations (5.6)–(5.7) imply, for all \(t>0\),
\[
\begin{aligned}
\|e^{-tH_n}Q_ne^{-tH_n}\|
&\le2e^{-tE_n}+3E_ne^{-2tE_n}\\
&\le \frac{7}{2e}\,t^{-1}.
\end{aligned}
\tag{5.10}
\]
The constant is independent of \(n\). Declaring the field spatially constant makes its spatially smeared bound cost only the lattice \(L^1\) norm of the spatial test. Thus this is precisely a uniform ground-Hamiltonian slab bound of the relevant kind, with \(\kappa=1\).

#### 5.4 The actual periodic hierarchy has a constant Gaussian limit

Use the positive periodic Markov-chain law of length \(N_n\) with weight
\(\prod_{k=0}^{N_n-1}(P_n)_{x_kx_{k+1}}\), \(x_{N_n}=x_0\). Its normalization is
\[
\mathcal Z_n(T_n)
=\operatorname{Tr}P_n^{N_n}
=1+(D_n-1)e^{-T_nE_n}.
\tag{5.11}
\]
Every one-time marginal is exactly uniform, since every diagonal entry of \(P_n^{N_n}\) is equal. Hölder and (5.6) therefore give, at arbitrary lattice time arguments,
\[
\left|\mathbb E_{{\rm per},n}\prod_{j=1}^mQ_n(t_j)\right|
\le M_m,\qquad M_m=\mathbb E|G|^m.
\tag{5.12}
\]

For a sharper convergence statement, arrange the \(m\) insertions cyclically, with integer gaps \(r_i\ge0\) summing to \(N_n\). In the marked trace, expand each
\[
P_n^{r_i}=\eta_n^{r_i}I+(1-\eta_n^{r_i})\Pi_n.
\]
The term with no \(\Pi_n\) is
\(D_ne^{-T_nE_n}\mu_{m,n}\).
Every other term is a product of moments
\(\mu_{k_1,n}\cdots\mu_{k_j,n}\), with \(\sum k_i=m\), multiplied by a coefficient of magnitude at most one. Hölder bounds each product by \(M_m\). Since
\[
1-\frac{D_ne^{-T_nE_n}}{\mathcal Z_n(T_n)}
=\frac{1-e^{-T_nE_n}}{\mathcal Z_n(T_n)},
\]
we obtain the uniform-in-position estimate
\[
\boxed{
\left|S_{m,n}(t_1,\ldots,t_m)-\mu_{m,n}\right|
\le\frac{2^mM_m}{\mathcal Z_n(T_n)}
\longrightarrow0.}
\tag{5.13}
\]
Thus the full hierarchy converges to a single standard Gaussian variable \(G\), constant at every spacetime point.

Reflection positivity at each cutoff follows directly by reflecting the positive half-chain: its quadratic form is the Hilbert–Schmidt norm of the half-chain marked matrix, divided by (5.11). The limiting hierarchy is symmetric, translation invariant, fully Euclidean invariant, and reflection positive.

It also has the required type of factorial Schwartz bound. For \(q>4\), the lattice \(L^1\) sum of a Schwartz test in \(4m\) variables is bounded by
\(C_q^m\nu_{qm}(F)\), uniformly for \(a_n\le1\). One may use
\[
(1+\textstyle\sum_{i=1}^m|x_i|^2)^{-qm/2}
\le\prod_{i=1}^m(1+|x_i|^2)^{-q/2}
\]
and factor the lattice sums. Since
\(M_m\le C^m(m!)^{1/2}\), (5.12) gives an OS-type linear-order factorial bound for the entire cutoff hierarchy, not only separated two-point functions.

There are even uniform complex exponential-source bounds. For complex coefficients \(z_i\), put \(S=\sum_i|z_i|\). Generalized Hölder, the exactly uniform marginals, and conditional Gaussian Jensen give
\[
\left|\mathbb E_{{\rm per},n}
 e^{\sum_i z_iQ_n(t_i)}\right|
\le \exp(S^2/2).
\tag{5.14}
\]
The statement for \(S=0\) is immediate; otherwise use Hölder weights \(|z_i|/S\), taking real parts in the modulus. The same bound applies to smeared lattice sources with their lattice \(L^1\) norm.

#### 5.5 Failure of the limiting energy bound and of the thermal criterion

OS reconstruction of the limiting constant field gives
\[
\mathcal H=L^2(\mathbb R,d\gamma),\qquad
\Omega=1,\qquad H=0,\qquad
\phi(f)=M_G\int_{\mathbb R^4}f(x)\,dx,
\tag{5.15}
\]
where \(M_G\) is multiplication by the Gaussian coordinate. Polynomials are dense, so this is the reconstructed cyclic Hilbert space. For \(\int f\ne0\), multiplication by \(G\) is unbounded. Hence
\[
\boxed{
\|\phi(f)(1+H)^{-r}\|=\infty
\quad\hbox{for every }r\ge0.}
\tag{5.16}
\]
Thus the uniform finite-cutoff ground slabs in (5.10) do not imply the desired operator estimate in this periodic limit.

Even a strong extensive pressure statement does not repair the inference. Here
\[
\log\mathcal Z_n(T_n)
=T_nE_n+o(1)=T_n^3+o(1),
\qquad
T_n^{-4}\log\mathcal Z_n(T_n)\longrightarrow0.
\tag{5.17}
\]
In contrast,
\[
\Gamma_n
=\log\frac{1+(D_n-1)e^{-T_nE_n/2}}
 {1+(D_n-1)e^{-T_nE_n}}
=\tfrac12T_nE_n+o(1),
\quad
\Gamma_n/T_n\longrightarrow\infty.
\tag{5.18}
\]
The state criterion in Section 4 correctly fails.

This is a global finite-state model, not a local compact gauge action. It proves a logical obstruction to an abstract bridge, not a counterexample to Yang–Mills existence or to a Wilson-specific theorem. A phase decomposition of the constant Gaussian example yields point masses, so it also does not disprove a separately proved phase-first strategy. It shows why that strategy must be stated and verified, rather than inferred from mixed-state vacuum bounds.

### 6. Remaining operator and phase premises

| Obligation | What this argument proves | What is still required |
|---|---|---|
| Bare temporal operator, SU(2) | All-representation inequality (2.10), sign-controlled centering (2.13), interacting compact bounds and domains (3.1)–(3.5) | Physical \(a^{-4}\) cancellation, all tensor components, prescribed finite normalization |
| Ground-Hamiltonian scalar response | Exact earlier completely positive transform combines with the improved bare bound | Uniform renormalized response in the same field convention; control of the identity shift |
| Periodic state versus ground Hamiltonian | Theorem 4.2 on the existing cubic geometry | A proof of (4.5), or its stronger version (4.6), together with actual renormalized slabs (4.12); alternatively the direct periodic OS inequality |
| Fixed-polynomial kernel norm | Positive path-kernel domination (4.19)–(4.20) | A verified finite cutoff-power budget for the chosen operator normalization and any surviving product redefinitions |
| Limiting operator domains | The prior periodic slab-to-domain theorem applies after (4.16) | Its interacting periodic premise remains unproved; excellent vacuum moments do not supply it |
| Phase decomposition | No new decomposition theorem is imported | Check the actual hypotheses of the chosen decomposition theorem, or supply a different proved phase construction |
| Ultraviolet coefficient in a phase | The separate vacuum-block criterion of Annex L is available | Prove its actual interacting block estimates; an operator-bound assumption is not automatically necessary for this transfer |

The main unresolved operator estimate is still (4.12), or directly (4.16), for the full renormalized finite tensor family in the prescribed Wilson hierarchy. Neither the representation estimate nor the thermal interpolation supplies the nonlinear marked ultraviolet analysis.

### 7. Source formulas

| Source | Exact location | Scope used here |
|---|---|---|
| M. Lüscher, *Construction of a selfadjoint, strictly positive transfer matrix for Euclidean lattice gauge theories*, DESY 76/54; published CMP 54 (1977), 283–292 | [DESY preprint](https://bib-pubdb1.desy.de/record/396349/files/7611148.pdf), printed preprint pp.7–9: (17), (20)–(23), Proposition 1; pp.10–11: (25)–(29), Proposition 2. | Compact Wilson transfer factors, strict positivity and gauge invariance, periodic trace interpretation. No continuum bound, uniform thermal estimate, or pure-phase theorem is imported. |
| NIST Digital Library of Mathematical Functions | [10.25.2](https://dlmf.nist.gov/10.25.E2), [10.32.2](https://dlmf.nist.gov/10.32.E2), [10.32.3](https://dlmf.nist.gov/10.32.E3) | Official reference for defining series and integral identities only. The representation-uniform derivative inequality and its consequences are derived in this annex. |
| Local transfer-energy comparison and volume-uniform midpoint bounds | Local deletion form and logarithmic increment | Range factorization and the closed-domain multiplier theorem on their stated geometry. |
| Periodic OS slabs and the reconstructed operator domain | Periodic trace identity and reduced even-mollifier hypothesis | Conditional passage to the common field domain. |
| Scalar transfer response | Annex C, Sections 1–2 | Exact scalar transfer/logarithmic-response relation and the distinction between ground centering and the prescribed finite normalization. |

The same-side geometry of the source-free Balaban construction is cubic. In particular, \(\mathcal Z_n(T_n/2)\) in this annex is not presented as the output of an independently admitted rectangular RG construction. No unpublished announcement or proof is used.


---
