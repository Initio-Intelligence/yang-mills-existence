# Original-kernel averaged S2 and phase criteria

**Current status:** The sufficient dissipative mean metric S8-C is now supplied by N9 for bounded normalized scalar/pseudoscalar seeds. P9 gives every moment order. The general matrix counterexample and stronger tensor endpoint limitations remain valid. Full historical S2 is still open.

**Status.** The translation-averaged exit criterion below is an exact theorem for the original positive kernels and requires translation invariance only of the microscopic law. It removes a need for a worst-phase conditional bound. The independent-phase moment theorems are separate proved implications. N8 now supplies the exact phase representation for the admitted deterministic bulk and its bounded scalar mean normalization. The quantitative matrix hypotheses on the anisotropic channels and the remaining actual-history estimates must still be verified before these results supply the complete exit criterion.

### 1. Average complete covariances, with no change of kernel

Let \(\Lambda_0\) be the finite periodic microscopic translation group, and let \(\mu_0\) be translation invariant. Fix the microscopic normalization matrix and deterministic subtraction once. For the real scalar field write \(F_{0,z}(x)=F_0(x+z)\). For each translate use the same original, frozen positive kernels:

\[
F_{k+1,z}(x)=Q_kF_{k,z}(x),\qquad
D_{k,z}(x,y)=Q_k(F_{k,z}(x)F_{k,z}(y))
-F_{k+1,z}(x)F_{k+1,z}(y).
\tag{S8.1}
\]

No output measure is assumed translation invariant. The fields indexed by \(z\) are simply different initial insertions transported by the same actual chain. In particular the kernel is not averaged over block origins.

#### Theorem S8-A: an averaged sufficient exit criterion

Let \(\operatorname{Av}_z=|\Lambda_0|^{-1}\sum_{z\in\Lambda_0}\). The original physical covariance obeys

\[
\begin{aligned}
|\operatorname{Cov}_{\mu_0}(F_0(x),F_0(y))|
\le{}&
\sum_{k<K}\operatorname{Av}_z
\mathbb E_{\mu_{k+1}}|D_{k,z}(x,y)|\\
&+
\left[
\operatorname{Av}_z\operatorname{Var}_{\mu_K}F_{K,z}(x)\,
\operatorname{Av}_z\operatorname{Var}_{\mu_K}F_{K,z}(y)
\right]^{1/2}.
\end{aligned}
\tag{S8.2}
\]

For a translated single field family, the two averaged variances in the last line are equal. Thus the following two estimates suffice for the original physical S2 bound:

\[
\sum_{k<K}\operatorname{Av}_z
\mathbb E|D_{k,z}(x,y)|
\le C r^{-8}\left(1+\log\frac{\ell_0}{r}\right)^b,
\qquad
\operatorname{Av}_z\operatorname{Var}_{\mu_K}F_{K,z}(x)
\le C\ell_0^{-8}.
\tag{S8.3}
\]

**Proof.** Apply the exact covariance telescope separately to every pair of initial translates. Its left side is independent of \(z\) by invariance of \(\mu_0\). Average those complete identities. Use the triangle inequality for the defect terms and Cauchy–Schwarz first in \(\mu_K\), then in the finite translation average, for the terminal covariance. Finally \(z\mapsto z+y-x\) permutes the microscopic translation group, so the averaged variances agree. \(\square\)

There is no covariance of a new random block-origin variable in this proof. Such a term appeared in N7.56 because that construction took the covariance of a mixed-kernel conditional expectation. Here the covariance identities are completed before the scalar average is taken.

#### Corollary S8-A1: averaged source norms suffice for a localized defect bound

Suppose a valid actual-history estimate has the form

\[
\mathbb E|D_{k,z}(x,y)|
\le C h_k^{-8}\mathcal D_k(r)\,
\mathbb E[A_{k,x+z}A_{k,y+z}],
\tag{S8.4}
\]

with nonnegative amplitudes under one specified common normalized law. If
\(\operatorname{Av}_z\mathbb E A_{k,x+z}^2\le B_k^2\), then the averaged defect is at most \(C h_k^{-8}\mathcal D_k(r)B_k^2\). Apply Cauchy–Schwarz in the product of that law and the uniform translation measure. The two second moments coincide by reindexing the translation sum, without any translation invariance of the intermediate law.

Thus one may aim for translation-averaged incoming second moments instead of a supremum over every microscopic blocking phase. The actual-history premise in (S8.4), the common normalization, and the terminal bound are still required.

### 2. An exact backward critical coordinate for independent phase maps

This section is an abstract operator theorem. Let
\(\mathcal X=\mathbb C^d\oplus\mathcal R\), where the finite critical space carries its Euclidean norm and \(\mathcal R\) is a Banach space of stable fields. Fixed equivalent critical norms can be introduced after the Hilbert-space estimates, with one fixed equivalence constant. Let independent phase variables \(\omega_k\) select bounded operators

\[
L_{k,\omega}
=
\begin{pmatrix}A_{k,\omega}&B_{k,\omega}\\
C_{k,\omega}&D_{k,\omega}\end{pmatrix},
\quad
\|A_{k,\omega}-I\|+\|B_{k,\omega}\|\le C t_k,\quad
\|C_{k,\omega}\|\le C,\quad
\|D_{k,\omega}\|\le q<1,
\tag{S8.5}
\]

where \(t_k=x_k^{-1}\), \(x_k\ge x_{k+1}+c_-\), and
\(x_k-x_{k+1}\le c_+\). All constants are independent of the horizon \(K\). A fixed blocking of several steps is allowed only when these bounds have been proved uniformly for the corresponding complete phase words.

Put \(\overline L_k=\mathbb E_\omega L_{k,\omega}\). Starting from \(V_K=0\), define backward

\[
E_k=\overline A_k+V_{k+1}\overline C_k,\qquad
V_k=E_k^{-1}(\overline B_k+V_{k+1}\overline D_k),\qquad
\ell_k=(I,V_k).
\tag{S8.6}
\]

For a sufficiently weak fixed coupling endpoint this recursion is defined and

\[
\|V_k\|\le C_Vt_k,\qquad
\|E_k-I\|\le C_Et_k,\qquad
\ell_{k+1}\overline L_k=E_k\ell_k.
\tag{S8.7}
\]

**Proof.** Since \(t_{k+1}/t_k\le1+C t_k\), take \(C_V\) larger than the fixed \(\overline B\)-bound divided by \(1-q\). In the ball \(\|V_{k+1}\|\le C_Vt_{k+1}\), the inverse of \(E_k\) has norm \(1+O(t_k)\). The second formula in (S8.6) then stays inside \(\|V_k\|\le C_Vt_k\) after reducing the coupling endpoint. Backward induction starts from \(V_K=0\). Multiplying out the two block rows gives the last identity exactly. \(\square\)

The use of a backward graph is useful: the mean critical coordinate evolves without a predictable stable feedback term.

### 3. A matrix moment theorem with its exact summability condition

Let \(P_{b,a}=E_{b-1}\cdots E_a\) for \(b>a\), and \(P_{a,a}=I\). Start the random recursion \(f_{k+1}=L_{k,\omega_k}f_k\) from

\[
f_0=(P_{K,0}^{-1}v,0),\qquad v\in\mathbb C^d.
\tag{S8.8}
\]

Write \(f_k=(m_k,r_k)\), \(\xi_k=\ell_kf_k\), and
\(Y_k=P_{K,k}\xi_k\). Conditional independence and (S8.7) give

\[
Y_{k+1}=Y_k+\Delta_k,\qquad
\Delta_k=P_{K,k+1}\ell_{k+1}
(L_{k,\omega_k}-\overline L_k)f_k,\qquad
\mathbb E[\Delta_k\mid\omega_0,\ldots,\omega_{k-1}]=0.
\tag{S8.9}
\]

In particular \(Y_0=v\). This is an exact finite-dimensional martingale, even though \(\mathcal R\) need not be a Hilbert space.

Set
\[
a_k=\|P_{K,k}^{-1}\|,\qquad
\Gamma_k=\|P_{K,k+1}\|\,a_k,\qquad
\mathcal Q=\sum_{k<K}t_k^2\Gamma_k^2.
\tag{S8.10}
\]

#### Theorem S8-B: phase-averaged normalized second moments

Under (S8.5)–(S8.7),

\[
\boxed{
\mathbb E\|f_k\|_{\mathcal X}^2
\le C a_k^2e^{C\mathcal Q}\|v\|^2.
}
\tag{S8.11}
\]

Here the product norm can be any fixed equivalent sum norm. Constants depend on the block estimates and the finite critical dimension, not on the phase count, ultraviolet depth, or dimension of the stable space.

**Proof.** Since \(\xi_k=m_k+V_kr_k\), the stable recursion is

\[
r_{k+1}=C_{k,\omega_k}\xi_k+
(D_{k,\omega_k}-C_{k,\omega_k}V_k)r_k.
\tag{S8.12}
\]

Its stable coefficient has norm at most \(q+Ct_k<q_1<1\). Also \(a_k/a_{k+1}\le1+Ct_k\), by the adjacent bound on \(E_k\). Let
\(R_k=(\mathbb E\|r_k\|^2)^{1/2}/a_k\).
Minkowski's inequality gives
\[
R_{k+1}\le C(\mathbb E\|Y_k\|^2)^{1/2}+q_2R_k,
\qquad q_2<1.
\]
Because \(\mathbb E\|Y_k\|^2\) is nondecreasing for the martingale and \(R_0=0\), geometric summation gives
\(R_k\le C(\mathbb E\|Y_k\|^2)^{1/2}\).
Thus \(\mathbb E\|f_k\|^2\le Ca_k^2\mathbb E\|Y_k\|^2\).

The row \(\ell_{k+1}(L_{k,\omega}-\overline L_k)\) has norm at most \(Ct_k\): its upper blocks are \(O(t_k)\), and its lower blocks are multiplied by \(V_{k+1}=O(t_k)\). Hence
\(\mathbb E\|\Delta_k\|^2\le Ct_k^2\Gamma_k^2\mathbb E\|Y_k\|^2\).
Martingale orthogonality proves

\[
\mathbb E\|Y_{k+1}\|^2
\le(1+Ct_k^2\Gamma_k^2)\mathbb E\|Y_k\|^2.
\tag{S8.13}
\]

Multiply these inequalities and use \(1+u\le e^u\). This proves (S8.11). No Banach-space martingale type assumption is needed, because orthogonality is used only in the finite-dimensional critical coordinate. \(\square\)

For a single invariant scalar marginal channel, \(\Gamma_k=|E_k|^{-1}\), which is uniformly bounded. The AF comparison gives \(\mathcal Q\le C/x_K\). Thus the phase variance costs only a summable \(g_k^4\)-series and preserves the scalar logarithmic benchmark.

For a matrix critical space, a sufficient additional estimate is

\[
\Gamma_k\le C(x_k/x_K)^\omega,\qquad 0\le\omega<\tfrac12.
\tag{S8.14}
\]

Indeed, the lower AF increment and the integral test give
\(\mathcal Q\le C_\omega/x_K\). If also \(a_k\le C(x_k/x_K)^s\), then (S8.11) yields the desired averaged incoming bound with the same fixed exponent \(s\).

### 4. Why the full matrix condition cannot be omitted

The \(O(g^2)\) block estimates alone do not imply bounded phase variance after a common matrix normalization.

Take \(x_k=X+K-k\), \(t_k=1/x_k\), two critical coordinates and no stable coordinates. For independent symmetric signs \(\varepsilon_k\), set

\[
E_k=\begin{pmatrix}(x_k/x_{k+1})^\omega&0\\0&1\end{pmatrix},
\qquad
L_{k,\varepsilon}=E_k+\varepsilon_k t_k
\begin{pmatrix}0&1\\0&0\end{pmatrix}.
\tag{S8.15}
\]

The mean is \(E_k\), and all deviations are \(O(t_k)\). Start in the second coordinate, which the mean normalization leaves unchanged. The variance of the terminal first coordinate is exactly

\[
\sum_{k<K}x_k^{-2}
(x_{k+1}/X)^{2\omega}.
\tag{S8.16}
\]

For fixed \(X\), it diverges logarithmically in the ultraviolet horizon when \(\omega=\tfrac12\), and as a power when \(\omega>\tfrac12\). This is an operator counterexample to the inference from the displayed block estimates. It is not asserted to be a Yang–Mills kernel.

In the actual 21-channel problem, a microscopic scalar insertion cannot automatically be treated as a one-dimensional phasewise invariant system: an individual blocking phase can break the rotation symmetry fixing its root. Anisotropic dimension-four curvature bilinears remain marginal fields. They may not be relabeled stable merely because their phase average is zero.

### 5. Exact remaining application to the original Yang–Mills construction

The original-kernel averaged exit criterion (S8.2) is unconditional once the original positive chain and microscopic translation invariance are given. Applying the moment theorem requires three additional verifications:

1. An exact reanchored independent-digit representation for the benchmark transport. N8.8–N8.12 supplies it for the admitted deterministic covariant bulk. Born forcing and mixed histories must use the separate uniform estimates appropriate to them, rather than an unsupported independence assumption.
2. Uniform marginal/stable bounds for every complete phase map, with the actual field and projection compatibility.
3. Either a phasewise invariant scalar sector, a summable matrix condition such as (S8.14), or a stronger telescoping/source-Ward correction for the anisotropic phase terms.

The original source phase counterexample does not rule out the averaged route, but the matrix example (S8.15) rules out declaring it solved from \(O(g^2)\) bounds alone. The new criterion provides a precise quantitative alternative to worst-phase point normalization; it does not complete the all-history or terminal estimates by itself.

### 6. A stronger scalar strategy: dissipativity of the mean marginal system

The worst-matrix factor \(\Gamma_k\) can be unnecessary for a particular initial field. The following second-moment theorem does not conjugate the noise by the inverse of every critical channel.

Retain (S8.5)–(S8.7). Suppose positive Hermitian matrices \(H_k\) obey

\[
c_H I\le H_k\le C_H I,\qquad
E_k^*H_{k+1}E_k\le(1+C_Ht_k^2)H_k.
\tag{S8.17}
\]

The matrices and backward graphs are deterministic. Their constants are independent of the horizon. This assumption allows first-order dissipation and only a summable positive second-order error. In particular it is satisfied when, in a fixed equivalent Euclidean norm, \(E_k=I+t_k B_k+O(t_k^2)\) uniformly and \(B_k+B_k^*\le0\).

#### Theorem S8-C: a dissipative mean gives bounded phase moments

For every deterministic initial vector \(f_0\), not necessarily (S8.8),

\[
\sup_{0\le k\le K}\mathbb E\|f_k\|_{\mathcal X}^2
\le C\exp\!\left(C\sum_{j<K}t_j^2\right)
\|f_0\|_{\mathcal X}^2.
\tag{S8.18}
\]

**Proof.** Write \(\xi_k=\ell_kf_k\). The exact recursion is
\(\xi_{k+1}=E_k\xi_k+\zeta_k\), where
\(\zeta_k=\ell_{k+1}(L_{k,\omega_k}-\overline L_k)f_k\)
has conditional mean zero and norm at most \(Ct_k\|f_k\|\). Define
\(s_k=\mathbb E\langle\xi_k,H_k\xi_k\rangle\).
The cross term vanishes after conditioning. By (S8.17),

\[
s_{k+1}\le (1+Ct_k^2)s_k+Ct_k^2\mathbb E\|f_k\|^2.
\tag{S8.19}
\]

The stable recursion (S8.12), Minkowski's inequality, and a geometric sum imply
\[
(\mathbb E\|r_k\|^2)^{1/2}
\le q_1^k\|r_0\|+C\max_{j<k}s_j^{1/2}.
\]
Consequently \(\mathbb E\|f_k\|^2\le C M_k\), where
\(M_k=\max\{\|f_0\|^2,s_0,\ldots,s_k\}\).
Equation (S8.19) gives \(M_{k+1}\le(1+Ct_k^2)M_k\).
Multiplication proves (S8.18). As before, only the finite critical coordinate uses a Hilbert norm. \(\square\)

If the one common normalized scalar seed has \(\|f_0\|\le C\), this theorem and \(\sum t_k^2\le C/x_K\) give a uniform phase-averaged bound for that seed. A neutral mean scalar channel with one-step factor \(1+O(t_k^2)\), and no mean mixing out of it, supplies such a bounded scalar normalization. No assertion is made that all 21 separately normalized seeds have bounded initial norm: the inverse normalization in a damped tensor channel may grow with the ultraviolet depth, and (S8.18) by itself does not repair that issue.

N8.28–N8.38 now provides the actual bounded scalar mean normalization in the identified regular reference, with its slightly more general summable error. That result supplies the initial scalar bound; it does not supply (S8.17) on the anisotropic components reached by individual phase operators.

The same proof allows the more general estimate
\(E_k^*H_{k+1}E_k\le(1+e_k)H_k\), where \(e_k\ge0\) and \(\sum_k e_k\) is uniformly bounded. The right side of (S8.18) is then multiplied by \(\exp(C\sum_k e_k)\). This includes a rigorously controlled mean-coordinate remainder of order \(g_k^4+g_k^3r_{\chi,k}\): its scale sum is finite under the AF comparison and a fixed polylogarithmic cutoff. An actual proof must still supply that remainder; calling a formal series summable does not bound it.

#### 6.1 What the continuum one-loop calculation suggests, and what it does not prove

There is concrete primary-source motivation for (S8.17). Ferretti, Heise and Zarembo, *New Integrable Structures in Large-N QCD*, hep-th/0404187v3, pp.4–5, equations (6)–(7), use canonical curvature \(F_{\mathrm{can}}=dA+ig[A,A]\) and \(\Gamma=Z^{-1}dZ/d\log\Lambda\). They give the dimension-four one-loop eigenvalues

\[
\gamma_{\mathrm{scalar}}=\gamma_{\mathrm{pseudoscalar}}
=-\frac{11Ng^2}{24\pi^2},\qquad
\gamma_{\mathrm{stress}}=0,\qquad
\gamma_{(2,0)\oplus(0,2)}=\frac{7Ng^2}{24\pi^2}.
\tag{S8.20}
\]

Their stated setting is the large-\(N\) theory. This note does not extend that calculation to every compact simple group without proof. The following sign conversion is an algebraic inference in their conventions, assuming the usual one-loop \(x=g^{-2}\) increment in the same normalization. Geometric curvature is \(F_{\mathrm{geom}}=gF_{\mathrm{can}}\); hence its bilinear adds the factor \(g_{\mathrm{fine}}^2/g_{\mathrm{coarse}}^2=x_{\mathrm{coarse}}/x_{\mathrm{fine}}\) in forward bare-to-coarse transport. Since the bare canonical insertion transports with \(Z^{-1}\), the three corresponding powers of \(x_{\mathrm{coarse}}/x_{\mathrm{fine}}\) are

\[
0\quad\text{(scalar and pseudoscalar)},\qquad
1\quad\text{(stress)},\qquad
\frac{18}{11}\quad\text{(the ten remaining components)}.
\tag{S8.21}
\]

These are neutral or damping directions. They motivate a scalar strategy that checks the Hermitian part of the **full mean critical map**, including stable feedback, instead of trying to bound a worst-channel condition number. The referenced calculation is available at [arXiv:hep-th/0404187](https://arxiv.org/abs/hep-th/0404187).

It is not a proof of (S8.17) for the actual Balaban operation. N8 proves the scalar mean neutrality directly from the actual gauge/cutoff identity. The matrix application still needs: the exact conversion of curvature and coupling conventions; a one-loop calculation or matching theorem for the anisotropic channels of the frozen block kernel with stable feedback; the permitted finite change of local source basis; and a uniform summable bound on the relevant higher-order and finite-volume terms. A continuum anomalous dimension does not by itself control a finite blocking phase or a history-dependent boundary. This strategy therefore remains an explicit calculation to complete, while Theorem S8-C is proved under its displayed hypotheses.

---
