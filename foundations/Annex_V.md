# Local periodic-state comparison and phase-symmetry defects

**Annex V.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

This annex proves two precisely scoped intermediate statements:

- **E-01:** an exact local periodic-to-vacuum comparison identity and a quantitative theorem transferring renormalized vacuum slab estimates to the same periodic hierarchy.
- **V-01:** a criterion for almost-everywhere preservation of a time-preserving disconnected symmetry in a valid phase decomposition, expressed as a large-distance positive-time two-block estimate.

Neither statement proves its actual Yang–Mills analytic premise. In particular, **E-05**, the required local state-comparison rate on the changing cubic Wilson family, and **V-04**, the vanishing of the actual phase-reflection defects, remain open.

Annex R reduces the covariant tensor energy estimate to three seed inequalities.

The periodic bridge uses the sufficient global trace condition
\[
\frac1T\log
\frac{\operatorname{Tr}e^{-(T/2)H_{a,T}}}
     {\operatorname{Tr}e^{-T H_{a,T}}}\longrightarrow0.
\tag{E.1}
\]
The new comparison route does not assume (E.1). It concerns the restriction of the actual path laws to the support of each fixed observable. It is an alternative sufficient state input, not a proof that local vacuum equivalence holds in Yang–Mills.

### 1. An exact endpoint density for the compact Wilson transfer law

Fix one finite cutoff. Let \(X\) be the compact space of spatial-link configurations with its Haar reference measure \(dx\). Gauge projection can be included in the transfer kernel. Let \(P\) be the nonnegative, selfadjoint, ground-normalized transfer operator, represented by a nonnegative kernel \(p(x,y)\), and suppose
\[
P\Omega=\Omega,\qquad \Omega(x)>0,\qquad
\int_X\Omega(x)^2dx=1.
\tag{E.2}
\]
These are the finite-cutoff transfer objects retained in Annex Q. The trace below is the physical trace; representing the gauge-projected operator on the full link space gives the same trace, since its orthogonal complement is annihilated. Put
\[
\mathcal Z_N=\operatorname{Tr}P^N,\qquad
P=e^{-aH}\ \hbox{on the physical space}.
\tag{E.3}
\]
Take integers \(N>m\ge1\). The temporal circumference is \(T=Na\). The \(m\)-step segment is chosen to contain every link and auxiliary transition variable used by the marks under discussion.

The stationary vacuum path law on \(x_0,\ldots,x_m\) has density
\[
d\nu_m
=\Omega(x_0)
\left[\prod_{j=1}^m p(x_{j-1},x_j)\right]
\Omega(x_m)\prod_{j=0}^m dx_j.
\tag{E.4}
\]
It is a probability measure because
\(\langle\Omega,P^m\Omega\rangle=1\). Equivalently it is the stationary law of the Doob transition
\[
Q(x,dy)=p(x,y)\frac{\Omega(y)}{\Omega(x)}dy,
\qquad \pi(dx)=\Omega(x)^2dx.
\tag{E.5}
\]

The marginal of the periodic \(N\)-step path law on the same segment is
\[
d\mu_{N,m}
=\frac1{\mathcal Z_N}
\left[\prod_{j=1}^m p(x_{j-1},x_j)\right]
p^{(N-m)}(x_m,x_0)
\prod_{j=0}^m dx_j,
\tag{E.6}
\]
where \(p^{(k)}\) is the kernel of \(P^k\).

#### Theorem E.1 — exact local comparison identity

The Radon–Nikodym density of (E.6) relative to (E.4) is
\[
\boxed{
R_{N,m}(x_0,x_m)
=
\frac{p^{(N-m)}(x_m,x_0)}
{\mathcal Z_N\Omega(x_0)\Omega(x_m)}.
}
\tag{E.7}
\]
In particular \(\nu_m(R_{N,m})=1\).

Let \(\mathcal C\) be any sub-sigma-algebra describing a smaller spacetime cylinder inside this segment. If \(\mu_{\mathcal C},\nu_{\mathcal C}\) are the restricted laws, then
\[
\boxed{
\frac{d\mu_{\mathcal C}}{d\nu_{\mathcal C}}
=r_{\mathcal C}
:=\mathbb E_{\nu_m}[R_{N,m}\mid\mathcal C].
}
\tag{E.8}
\]
With total variation normalized as
\(\delta(\mu,\nu)=\sup_A|\mu(A)-\nu(A)|\),
\[
\boxed{
\delta_{\mathcal C}
=\frac12\mathbb E_{\nu_m}|r_{\mathcal C}-1|,
\qquad
|\mu(W)-\nu(W)|
\le2\delta_{\mathcal C}\|W\|_\infty
}
\tag{E.9}
\]
for every bounded complex \(\mathcal C\)-measurable mark \(W\).

**Proof.** Integrating out the complement of the segment in the periodic path gives the closing kernel \(p^{(N-m)}\), proving (E.6). Dividing the two displayed nonnegative densities gives (E.7), up to irrelevant null sets. The conditional-expectation identity
\[
\mathbb E_{\nu_m}[R_{N,m}W]
=\mathbb E_{\nu_m}[r_{\mathcal C}W]
\]
for \(\mathcal C\)-measurable \(W\) proves (E.8). The signed measure \((r_{\mathcal C}-1)d\nu_{\mathcal C}\) has total mass zero, so the integral of its positive part and of the absolute value of its negative part both equal \(\delta_{\mathcal C}\). This proves (E.9), also for complex marks by the total-variation norm inequality. \(\square\)

The same proof retains auxiliary transition variables. If a Wilson transfer kernel is obtained by integrating a nonnegative density \(p(x,z,y)\) over temporal links or other transition variables \(z\), use that density in every segment factor in both laws. Their ratio is still (E.7). Consequently temporal plaquettes and finite temporal clovers are covered. The statement is not restricted to time-zero multiplication observables.

The relevant target for E-05 is the **conditional** density (E.8), on the support of the observable. A bound on the full endpoint ratio is sufficient but can be unnecessarily strong. Conditioning can discard a large spectral contribution carried by degrees of freedom outside that cylinder.

#### Entropy version, with its proof

An alternative local input is
\[
D_{\mathcal C}
=\int r_{\mathcal C}\log r_{\mathcal C}\,d\nu_{\mathcal C}.
\tag{E.10}
\]
Then
\[
\delta_{\mathcal C}\le\sqrt{D_{\mathcal C}/2},
\qquad
|\mu(W)-\nu(W)|
\le\sqrt{2D_{\mathcal C}}\,\|W\|_\infty.
\tag{E.11}
\]

To verify the constant, put \(A=\{r_{\mathcal C}\ge1\}\), \(p=\nu_{\mathcal C}(A)\), and \(q=\mu_{\mathcal C}(A)\), so \(q-p=\delta_{\mathcal C}\). Jensen on \(A\) and its complement gives
\[
D_{\mathcal C}\ge
q\log(q/p)+(1-q)\log((1-q)/(1-p)).
\]
As a function of \(q\), the right side and its first derivative vanish at \(q=p\), while its second derivative is
\(q^{-1}+(1-q)^{-1}\ge4\). It is therefore at least \(2(q-p)^2\). The limiting cases \(p=0,1\) follow by continuity or give infinite relative entropy. This proves (E.11). No entropy estimate for the actual Wilson family is asserted here.

### 2. Quantitative transfer with the physical cutoff factors retained

Let \(a_n\downarrow0\), \(T_n\uparrow\infty\) be an admitted cubic sequence. At each \(n\), \(\mu_n\) is its actual periodic Wilson law and \(\nu_n\) is the vacuum path law constructed from the **same** finite-spatial-volume transfer operator. Thus the spatial side of both laws is \(T_n\). This definition does not change the temporal side while silently keeping a different spatial Hamiltonian fixed.

Choose nested physical cylinders \(\mathcal C_R\) exhausting compact spacetime sets. Give each test enough margin for every lattice stencil in its representative. Denote the total variation of the two restrictions by \(\delta_n(R)\). The exact formula (E.8) defines it even when its decay is unknown.

The **coefficient-budget hypothesis** is the following. For every fixed compact polynomial or joint-test path mark \(W_n\) used in the hierarchy, including its running field coefficients, identity subtractions and finite product redefinitions, there are \(R_W,d_W,C_W<\infty\) such that
\[
W_n\ \hbox{is }\mathcal C_{R_W}\hbox{-measurable},
\qquad \|W_n\|_\infty\le C_Wa_n^{-d_W}.
\tag{E.12}
\]
The constants and exponent may depend on the fixed degree and tests. They are uniform in \(n\) and in the selected volume. They must be verified for the actual field prescription.

For a degree-\(m\) product of dimension-four representatives, the bound can contain \(a_n^{-4m}\), multiplied by running normalization factors. It is not legitimate to treat its supremum as cutoff independent. A fixed logarithmic factor can be absorbed into an additional fixed power of \(a_n^{-1}\); an unrestricted subtraction coefficient cannot.

#### Theorem E.2 — local state comparison transfers the hierarchy

Suppose (E.12) holds and
\[
\boxed{
a_n^{-k}\delta_n(R)\longrightarrow0
\quad\hbox{for every fixed }R<\infty
\hbox{ and integer }k\ge0.
}
\tag{E.13}
\]
Then, for every such fixed marked hierarchy evaluation,
\[
\mu_n(W_n)-\nu_n(W_n)\longrightarrow0.
\tag{E.14}
\]
Thus whenever either of these two normalized hierarchies converges on these tests, the other has the same limit. If the common uniform Schwartz bounds needed for reconstruction have already been established, the equality extends by continuity from compact coincidence-flat tests to the full test spaces.

**Proof.** Equation (E.9) gives
\[
|\mu_n(W_n)-\nu_n(W_n)|
\le2C_Wa_n^{-d_W}\delta_n(R_W).
\]
Choose an integer \(k\ge d_W\), eventually \(a_n\le1\), and apply (E.13). The same common limit and the claimed continuity extension then follow directly. \(\square\)

For a particular finite set of evaluations, (E.13) can be weakened to precisely the finitely many rates
\[
a_n^{-d_W}\delta_n(R_W)\longrightarrow0.
\tag{E.15}
\]
The superpolynomial formulation is a convenient single sufficient condition for the whole hierarchy. It is not declared necessary.

Plain local total-variation convergence \(\delta_n(R)\to0\) is insufficient with no rate. For example, a bound \(\delta_n=a_n\) leaves the estimate for an \(a_n^{-8}\)-bounded two-field mark divergent. This is a defect of that proposed inference, not a claim that the actual moment difference must diverge.

#### Theorem E.3 — local comparison transfers the periodic OS insertion inequality

Assume the exact cutoff transfer realization of the chosen Hermitian renormalized insertion \(q_{\alpha,n}(g)\), with the correct identity coefficient and midpoint placement. Assume
\[
\|e^{-uH_n}q_{\alpha,n}(g)e^{-uH_n}\|
\le C u^{-\kappa}\rho_s(g),
\qquad 0<u\le1,
\tag{E.16}
\]
uniformly in \(n\). Here
\(\rho_s(g)=\sum_{|\beta|\le s}\|\partial^\beta g\|_{L^1(\mathbb R^3)}\).

Assume (E.12)–(E.13) for the actual cutoff polynomial products below. Fix a positive-time complex polynomial \(F\), \(0<t\le1\), real spatial \(g\), and a nonnegative even mollifier \(\chi_\epsilon\) of integral one with \(0<\epsilon<t/8\). Then
\[
\begin{split}
&\left|
\mu_n\!\left[
(\Theta\tau_tF)\,
Q_{\alpha,n}(\chi_\epsilon\otimes g)\,
(\tau_tF)\right]\right|\\
&\qquad\le
C' t^{-\kappa}\rho_s(g)\,
\mu_n[(\Theta F)F]
+\varepsilon_n(F,t,\epsilon,g,\alpha),
\qquad \varepsilon_n\longrightarrow0,
\end{split}
\tag{E.17}
\]
with \(C'\) independent of \(F\), its degree, and the fixed \(\epsilon\). In this cutoff formula, time translations mean the fixed lattice realizations \(\tau_{t_n}\), with \(t_n\to t\), and all marks use one specified lattice sampling. The order of limits remains: first \(n\to\infty\) at every fixed \(\epsilon>0\), then unsmear in the reconstructed continuum theory.

**Proof.** In the vacuum transfer representation, write \(\Psi_n(F)\) for the corresponding positive-time vector. Translation by \(t\) gives the heat factor \(e^{-tH_n}\). At a central insertion time \(\delta\) in the mollifier support, the relevant matrix element is
\[
\left\langle\Psi_n(F),
e^{-(t_n-\delta)H_n}
q_{\alpha,n}(g)
e^{-(t_n+\delta)H_n}
\Psi_n(F)\right\rangle,
\tag{E.18}
\]
with the actual lattice shifts \(t_n\to t\) and the fixed stencil buffer included. Eventually both heat intervals exceed \(t/2\). Factoring out the sandwich in (E.16) at \(t/2\) bounds the absolute value by
\[
2^\kappa C t^{-\kappa}\rho_s(g)
\|\Psi_n(F)\|^2.
\]
At each fixed \(\epsilon\), the lattice \(L^1\) sum of the sampled mollifier is eventually at most two. Hence the vacuum version of (E.17) holds with \(C'=2^{\kappa+1}C\).

Set
\[
W_n=(\Theta\tau_tF)
Q_{\alpha,n}(\chi_\epsilon\otimes g)(\tau_tF),
\qquad V_n=(\Theta F)F.
\]
Apply (E.9) separately to \(W_n\) and \(V_n\). The error can be taken to be
\[
\begin{split}
\varepsilon_n={}&
2\delta_n(R_W)\|W_n\|_\infty\\
&+2C't^{-\kappa}\rho_s(g)
\delta_n(R_V)\|V_n\|_\infty,
\end{split}
\tag{E.19}
\]
for these fixed sampled marks; no additional sampling error occurs in this identity. The two terms tend to zero by (E.12)–(E.13). Reflection positivity makes the quadratic norm terms nonnegative in their respective laws. The constants in (E.12) affect the error, not \(C'\). This proves (E.17). Replacing the specified sampling or rounded shifts by another approximation of the continuum tests requires the common S0 seminorm bounds and continuity; only under that additional premise does the resulting sampling difference tend to zero. \(\square\)

If \(F\) has degree \(d\), the central mark \(W_n\) can have degree \(2d+1\), and its physical coefficient budget can contain \(a_n^{-4(2d+1)}\). This dependence is included in (E.19). The theorem does not infer (E.16) from the dimensionless magnetic estimate in Annex Q.

The equality of the insertion prescriptions matters. A ground-centered observable and the prescribed F0-centered observable differ by an identity term, and that term must be bounded in (E.16) or explicitly included in the normalization. Local comparison does not erase it.

### 3. The exact diagonal-selection premise

The following is a useful way to formulate the open E-05 estimate without requiring a rate uniform in both \(a\) and \(T\) from the start.

For each fixed admitted \(a\), let \(\delta(a,T;R)\) be the local comparison defect between the periodic cube of side \(T\) and the vacuum path law of its finite-spatial-volume transfer operator \(H_{a,T}\). Assume
\[
\boxed{
\liminf_{\substack{T\to\infty\\T\ {\rm admitted\ at}\ a}}
\delta(a,T;R)=0
\quad\hbox{for every fixed }a,R.
}
\tag{E.20}
\]
The term \(H_{a,T}\) changes with \(T\). This is an additional cubic-family assertion, not the fixed-spatial-operator zero-temperature limit.

#### Proposition E.4 — one cofinal sequence suffices

Assume (E.20) on an admitted family of arbitrarily large cubes, and assume the source-free and marked hypotheses being used remain valid on the selected family. Let \(a_n\downarrow0\) be any admitted cutoff sequence. One can choose admitted \(T_n\to\infty\) such that (E.13) holds, while also imposing any prescribed finite lower bound on \(T_n\), for example
\[
T_n\ge n(1+\log(1/a_n)).
\tag{E.21}
\]

**Proof.** Choose nested cylinders \(\mathcal C_n\) containing every fixed compact cylinder eventually. At the fixed value \(a=a_n\), (E.20) with \(R=n\) permits an arbitrarily large admitted \(T_n\) with
\[
\delta(a_n,T_n;n)\le a_n^n/n.
\tag{E.22}
\]
Choose it also large enough for (E.21), the cylinder margin, the source-free minimum size, and \(T_n>T_{n-1}\). Restricting measures to a smaller sigma-algebra cannot increase total variation. Thus, for fixed \(R,k\) and all sufficiently large \(n\),
\[
a_n^{-k}\delta_n(R)
\le a_n^{\,n-k}/n\longrightarrow0.
\]
This is (E.13). \(\square\)

This diagonal argument is valid only **after** (E.20) is proved. Finite-cutoff spectral convergence at fixed spatial volume does not prove (E.20).

### 4. What the elementary spectral estimate does and does not give

At one fixed cutoff, suppose the physical normalized transfer operator has a unique ground state and gap \(\gamma>0\). Define
\[
\mathcal K
=\sup_{x\in X}
\left(\frac{p^{(2)}(x,x)}{\Omega(x)^2}-1\right).
\tag{E.23}
\]
For the continuous strictly positive compact kernel at a fixed finite cutoff, \(\mathcal K<\infty\). This fact is not a bound uniform in cutoff or spatial volume.

For every integer \(k\ge2\),
\[
\left|
\frac{p^{(k)}(x,y)}{\Omega(x)\Omega(y)}-1
\right|
\le \mathcal K e^{-(k-2)a\gamma}.
\tag{E.24}
\]
Indeed, set
\(u_x(z)=p(x,z)-\Omega(x)\Omega(z)\).
It is orthogonal to \(\Omega\), and
\[
\|u_x\|^2=p^{(2)}(x,x)-\Omega(x)^2.
\]
The kernel difference in (E.24) is
\(\langle u_x,P^{k-2}u_y\rangle\), up to the harmless real-kernel ordering. On \(\Omega^\perp\), the operator norm is at most \(e^{-(k-2)a\gamma}\). Cauchy–Schwarz proves (E.24).

Integrating the diagonal gives
\[
0\le\mathcal Z_N-1\le
\mathcal K e^{-(N-2)a\gamma}.
\]
If \(N-m\ge2\), (E.7) consequently yields
\[
\|R_{N,m}-1\|_\infty
\le2\mathcal K e^{-(T-ma-2a)\gamma},
\qquad
\delta_{\mathcal C}
\le\mathcal K e^{-(T-ma-2a)\gamma}.
\tag{E.25}
\]

This is a valid finite-cutoff bound for the actual kernel. In the cubic family it contains
\[
\mathcal K_{a,T}
\quad\hbox{and}\quad
\gamma_{a,T}.
\]
Neither is controlled by the local deletion cost in Annex Q. Therefore (E.25) cannot be used to select \(T_n\) by pretending that these quantities stay fixed as the spatial side grows. A useful actual-model estimate may instead exploit the conditional expectation in (E.8), which can be much smaller than the full endpoint supremum.

#### The two sufficient criteria are not comparable in general

The next finite-dimensional positive-transfer example shows that the local comparison criterion can hold when the old trace criterion fails. It is not a Yang–Mills or translation-invariant lattice model, and it does not by itself prove an implication between the two criteria.

Let the observable subsystem be two-dimensional, with unique strictly positive ground vector and Hamiltonian \(H_{\rm vis}\) having spectrum \(0,1\). Choose it so its heat kernel is strictly positive in the two-state basis. Tensor it with a spectator Hamiltonian \(H_{{\rm sp},n}\) having one ground level and \(d_n\) levels at energy one, with
\[
d_n=\lceil e^{cT_n}\rceil,\qquad \tfrac12<c<1.
\]
A strictly positive kernel is obtained by taking the ground projection onto the uniform vector and
\(H_{{\rm sp},n}=I-\Pi_{\rm ground}\).
All specified local marks act only on the observable subsystem.

The periodic and vacuum path restrictions of those marks differ by
\[
O_R(e^{-(T_n-R)}).
\]
For example, this follows directly from (E.7) for the fixed two-dimensional observable subsystem. Taking \(a_n=L^{-n}\) and \(T_n=2L^n\) makes the local error smaller than every power of \(a_n\).

In contrast, the spectator partition function is
\[
\mathcal Z_{{\rm sp},n}(u)=1+d_ne^{-u},
\]
so
\[
\frac1{T_n}\log
\frac{\mathcal Z_{{\rm sp},n}(T_n/2)}
     {\mathcal Z_{{\rm sp},n}(T_n)}
\longrightarrow c-\tfrac12>0.
\tag{E.26}
\]
Thus the local comparison route can succeed when (E.1) fails. The spectator may be viewed as a degree of freedom outside all specified local cylinders. This example proves no estimate for actual Wilson local marginals; it only prevents treating the global trace condition as a necessary state criterion.

The converse implication also fails. In a two-state space choose
\(\Omega=(\sqrt p,\sqrt{1-p})\), with \(0<p<1\) and \(p\ne1/2\), and put
\[
H_n=\epsilon_n(I-\Pi_\Omega),\qquad
\epsilon_n=T_n^{-2}.
\tag{E.27}
\]
Every positive-time kernel is strictly positive, and the ground state is unique. Its partition function is
\(\mathcal Z_n(u)=1+e^{-u\epsilon_n}\). Hence
\[
\frac1{T_n}\log
\frac{\mathcal Z_n(T_n/2)}{\mathcal Z_n(T_n)}
\longrightarrow0.
\]
Nevertheless, the periodic time-zero probability of the first state is
\[
\mu_n(\{1\})=
\frac{e^{-T_n\epsilon_n}+
(1-e^{-T_n\epsilon_n})p}
{1+e^{-T_n\epsilon_n}}
\longrightarrow\frac12,
\]
whereas its vacuum probability is \(p\). The local total variation therefore stays bounded away from zero. The old trace criterion can transfer a slab inequality without asserting equality of these two local laws.

Thus E-01 supplies an **alternative** sufficient route. It is not a uniformly weaker replacement. Its local norm comparison can be stronger than necessary for the energy conclusion, and the original trace route and the direct periodic OS route remain available.

### 5. A phase-reflection criterion in the actual positive-time test algebra

This section uses the corrected OS test spaces and their actual tensor reflection conventions. No statement about ordinary probability positivity after contact renormalization is assumed.

Assume that a continuum hierarchy and a valid phase-field disintegration have already been constructed:
\[
\mathcal H=\int^\oplus\mathcal H_\omega\,d\nu(\omega),
\quad
H=\int^\oplus H_\omega\,d\nu(\omega),
\quad
\Omega=\int^\oplus\Omega_\omega\,d\nu(\omega),
\quad
\|\Omega_\omega\|=1.
\tag{V.1}
\]
Assume the positive-time polynomial vectors disintegrate consistently,
\[
\Psi(F)=\int^\oplus\Psi_\omega(F)\,d\nu(\omega),
\qquad
S_\omega(F)=
\langle\Omega_\omega,\Psi_\omega(F)\rangle.
\tag{V.2}
\]
Assume the fibers are translation-ergodic phases in the following precise sense:
\[
\ker H_\omega=\mathbb C\Omega_\omega
\quad\hbox{for almost every }\omega.
\tag{V.3}
\]
The forward-cone spectrum makes \(\ker H\) equal the space invariant under all translations: on the joint spectrum, \(p^0=0\) implies \(\mathbf p=0\). The same applies in each fiber. Thus (V.3) is the unique translation-invariant-vacuum condition, rather than an unsupported assertion about arbitrary factor states.

Let \(G\) be a finite group of time-preserving spatial orthogonal transformations, including any desired spatial reflection. Use its stipulated action on field labels. Such a transformation preserves the positive-time test algebra and commutes with the time translations used below. Write
\[
D_gF=gF-F,\qquad
P_0=\mathbf1_{\{0\}}(H).
\tag{V.4}
\]

Require that the phase distributions are continuous on the relevant coincidence-flat test spaces and translation invariant. These properties must come from the valid phase construction, for example the previously proved energy-to-phase-regularity implication once its energy input is available.

Choose a countable complex rational-linear test core \(\mathcal D_+\), dense at each degree and field-label tuple on every compact positive-time support with positive margin. Such cores are obtained by a countable compact exhaustion and separability of the supported smooth test spaces; the coincidence-flat subspaces inherit a countable dense set. Enlarge the core by its finitely many \(G\)-images. No norm separability of a local von Neumann algebra is assumed.

#### Theorem V.1 — exact equivalence for phase reflection covariance

Under (V.1)–(V.4), the following are equivalent:

1. On one full-measure set of phases,
   \[
   S_\omega(gF)=S_\omega(F)
   \tag{V.5}
   \]
   for all \(g\in G\) and all tests in the full continuum hierarchy.

2. For every \(g\in G\) and every \(F\in\mathcal D_+\),
   \[
   \boxed{\|P_0\Psi(D_gF)\|=0.}
   \tag{V.6}
   \]

3. For every \(g\in G\) and every \(F\in\mathcal D_+\),
   \[
   \boxed{
   \lim_{R\to\infty}
   S\bigl((\Theta\tau_RF_g)(\tau_RF_g)\bigr)=0,
   \qquad F_g=D_gF.
   }
   \tag{V.7}
   \]
   Here products mean the full OS quadratic-form evaluation, including joint polynomial kernels; the expression is nonnegative.

The precise identity behind these equivalences is
\[
\boxed{
\lim_{R\to\infty}
S\bigl((\Theta\tau_RD_gF)(\tau_RD_gF)\bigr)
=
\|P_0\Psi(D_gF)\|^2
=
\int|S_\omega(D_gF)|^2d\nu(\omega).
}
\tag{V.8}
\]

**Proof.** Spectral calculus and (V.3) give
\[
P_0=
\int^\oplus
|\Omega_\omega\rangle\langle\Omega_\omega|
\,d\nu(\omega).
\]
Using (V.2), the fiber of \(P_0\Psi(D_gF)\) is
\[
S_\omega(D_gF)\Omega_\omega.
\]
Taking the direct-integral norm gives the second equality in (V.8).

OS time translation gives
\[
\Psi(\tau_RF_g)=e^{-RH}\Psi(F_g).
\]
The spectral theorem implies \(e^{-RH}\to P_0\) strongly as \(R\to\infty\). Consequently
\[
S((\Theta\tau_RF_g)(\tau_RF_g))
=\|e^{-RH}\Psi(F_g)\|^2
\longrightarrow\|P_0\Psi(F_g)\|^2.
\]
This proves the first equality. No gap or quantitative clustering rate is used.

Condition (V.5) immediately implies (V.6) by (V.8), and (V.6) and (V.7) are equivalent by the same identity. If (V.6) holds, then \(S_\omega(D_gF)=0\) for almost every \(\omega\) for each pair \(g,F\) in the countable core. Intersect these countably many full-measure sets. Continuity of each phase distribution extends the equality to all compact positive-time tests, at every degree and label tuple.

Every compact joint test can be shifted by one common time translation far enough to lie strictly in positive time. Since \(g\) preserves time and the phase distributions are translation invariant, the equality for the translated test implies the equality for the original test. Finally, compact cutoffs preserve coincidence flatness and converge in the Schwartz topology. Phase distribution continuity extends the identity to all the full hierarchy tests. Thus (V.5) holds on one full-measure set. \(\square\)

#### Bounded-algebra and macroscopic-average form

For the stated theorem, the same result has a bounded-algebra formulation. Let \(\mathfrak A_{\rm sep}\) be a **specified norm-separable unital \(C^*\)-algebra** of bounded decomposable observables, invariant under the finite symmetry automorphisms \(\alpha_g\). Suppose its represented phase states are
\[
\omega(A)=\langle\Omega_\omega,A_\omega\Omega_\omega\rangle.
\]
Do not identify \(\mathfrak A_{\rm sep}\) with an arbitrary local von Neumann algebra, which need not be norm separable. If invariance of this algebra is to determine all field distributions, that determining property is a separate application hypothesis.

Choose a countable norm-dense set \(A_j\), including its finitely many symmetry images and rational linear combinations. Then the phase states are \(G\)-invariant on \(\mathfrak A_{\rm sep}\) on one full-measure set if and only if
\[
\|P_0(\alpha_g(A_j)-A_j)\Omega\|=0
\quad\hbox{for all }g,j.
\tag{V.12}
\]
Indeed, direct integration gives the exact identity
\[
\|P_0(\alpha_g(A)-A)\Omega\|^2
=\int|\omega(\alpha_g(A)-A)|^2d\nu(\omega).
\tag{V.13}
\]
After the countable intersection, norm continuity of every state extends the equality from \(A_j\) to all \(A\). Conversely invariant phase states make the right side zero.

For a macroscopic translation-average version, choose nonnegative
\(\chi\in C_c^\infty(\mathbb R^4)\) of integral one and put
\(\chi_R(x)=R^{-4}\chi(x/R)\). Let \(U(x)\) be the strongly continuous translation representation and set
\[
v_R=\int_{\mathbb R^4}\chi_R(x)
U(x)(\alpha_g(A)-A)\Omega\,dx.
\tag{V.14}
\]
This is a norm-convergent vector integral; no operator-norm continuity of translations on a local von Neumann algebra is required. With the usual Fourier convention,
\[
v_R=\widehat\chi(RP)(\alpha_g(A)-A)\Omega.
\]
Here \(\widehat\chi(0)=1\), \(|\widehat\chi|\le1\), and
\(\widehat\chi(Rp)\to0\) for \(p\ne0\), by integration by parts for the smooth compactly supported function. Dominated convergence in the joint spectral measure and the forward-cone identification of \(P_0\) give
\[
v_R\longrightarrow
P_0(\alpha_g(A)-A)\Omega
\quad\hbox{in norm}.
\tag{V.15}
\]
Therefore the limit of the squared macroscopic-average norm is exactly (V.13). Equivalently it is the double integral of the corresponding translated two-block vacuum correlation. This proves the bounded-algebra statement of V-01 and its simultaneous-null-set requirement. The positive-time formulation (V.8) is preferable for the present observable route because its test algebra and full Schwinger functions are already specified.

#### What this criterion buys

The open V-04 target can now be stated as a concrete estimate on the mixed hierarchy:
\[
S((\Theta\tau_RD_gF)(\tau_RD_gF))
\longrightarrow0
\quad(R\to\infty)
\tag{V.9}
\]
for a countable determining family of positive-time tests and the required spatial reflection.

This is a two-block estimate at large Euclidean time separation. It is weaker than imposing clustering for every pair of observables: only the symmetry-defect vectors are required to have zero projection onto the vacuum subspace. It also differs from the ultraviolet block estimates of Annex L, which shrink the internal geometry of blocks while keeping their centers a fixed distance apart.

If the phase construction separately guarantees connected Euclidean covariance, one spatial reflection together with \(SO(4)\) generates \(O(4)\). Then (V.5) for that reflection gives full \(O(4)\) covariance of almost every phase hierarchy. This inference does not supply connected covariance or prove that a symmetry which permutes phases acts within each phase.

The conclusion is an almost-everywhere theorem. Existence of just one symmetric phase is weaker and could in principle be proved by another argument even if (V.9) fails. The criterion is offered as a clean sufficient route with an exact necessity statement for its stronger almost-everywhere conclusion.

#### Mixed symmetry only fixes the mean

If the mixed hierarchy is \(G\)-invariant, one knows
\[
S(D_gF)
=\int S_\omega(D_gF)\,d\nu(\omega)=0.
\tag{V.10}
\]
Equation (V.8) requires the squared modulus of this phase defect to have mean zero. Equation (V.10) does not imply that assertion.

A minimal Hilbert-space example makes the distinction exact. Take
\[
\mathcal H=\mathbb C^2,\quad
H=0,\quad
\Omega=2^{-1/2}(1,1),\quad
A=\operatorname{diag}(v,-v),
\]
and let a \(\mathbb Z_2\) unitary swap the two coordinates. The mixed state is invariant, each one-dimensional component has a unique vacuum, and the symmetry sends \(A\) to \(-A\). Hence
\[
\langle\Omega,(\alpha_g(A)-A)\Omega\rangle=0,
\qquad
\|P_0(\alpha_g(A)-A)\Omega\|^2=4v^2.
\tag{V.11}
\]
The two pure components are exchanged. This is an internal-symmetry finite-dimensional example, not a spacetime field construction or a Yang–Mills model. It illustrates precisely the mean-versus-variance obstruction; for spacetime reflection, (V.8) must be evaluated with the actual tensor and Wick conventions.

The same distinction explains why common ultraviolet coefficients alone cannot establish reflection invariance of phases. A fixed central order parameter can be invisible in a rescaled short-distance leading coefficient and still produce a nonzero defect in (V.8). The ultraviolet and large-distance tests have different limits and neither is substituted for the other.

### 6. Simultaneous phase selection once the separate premises are proved

The following is an application specification, not a third new theorem.

Suppose the chosen valid phase decomposition supplies energy/domain control and connected covariance on a full-measure set \(\mathcal G_{\rm field}\). Suppose the actual interacting four/six-block estimates satisfy the hypotheses of Annex L, giving the specified ultraviolet coefficients on a full-measure set \(\mathcal G_{\rm UV}\). Suppose (V.9) is proved, giving \(\mathcal G_{\rm refl}\).

Then
\[
\mathcal G_{\rm field}\cap
\mathcal G_{\rm UV}\cap
\mathcal G_{\rm refl}
\]
has full measure. Every phase in that set has all three properties. The countable-profile and continuous-scale arguments needed for \(\mathcal G_{\rm UV}\) remain those of Annex L; they are not proved a second time here. The target field family and normalization must be the same in each input.


---


---
