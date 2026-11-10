# Every phase-moment order at one weak threshold

**Status.** This is the all-orders theorem for the independent-phase regular benchmark. N9.19–N9.28 now establish its mean-growth hypothesis for the actual admitted regular reference. The result therefore applies to bounded deterministic initial seeds, including the mean-normalized scalar and pseudoscalar families, at one weak-coupling threshold independent of the moment order. Fully renormalized stress/Weyl point seeds need a further initial-normalization estimate. Mixed histories and full Yang–Mills existence are outside this theorem.

### 1. Hypotheses already isolated by the regular analysis

Retain the exact phase recursion and backward critical coordinate of S8:

\[
f_{k+1}=L_{k,\omega_k}f_k,\qquad
\xi_k=\ell_kf_k,\qquad
\xi_{k+1}=E_k\xi_k+\zeta_k,
\qquad
\mathbb E[\zeta_k\mid\mathscr F_k]=0.
\tag{P9.1}
\]

The digits \(\omega_k\) are the actual independent reanchored digits of a uniform microscopic translate, as proved in N8.11–N8.12. The initial mark is deterministic. The finite critical space has dimension 21, and the stable space may be Banach. On the admitted weak segment put \(t_k=x_k^{-1}\), with \(x_k=g_k^{-2}\). The regular estimates give

\[
\|\zeta_k\|\le Ct_k\|f_k\|,\qquad
\|r_{k+1}\|\le q_1\|r_k\|+C\|\xi_k\|,
\quad q_1<1,
\tag{P9.2}
\]

after the fixed block grouping used for classical contraction. They also give the deterministic arbitrary-profile propagator bound N7.49,

\[
\|L_{b-1,\omega_{b-1}}\cdots L_{a,\omega_a}\|
\le C\left(\frac{x_a}{x_b}\right)^{p_{\mathrm b}}
\quad(0\le a<b\le K),
\tag{P9.3}
\]

uniformly over complete phase words. The fixed exponent \(p_{\mathrm b}\) is independent of the moment order and of the horizon.

Assume, in addition, uniformly equivalent deterministic Hermitian metrics satisfy

\[
cI\le H_k\le CI,
\qquad E_k^*H_{k+1}E_k\le H_k.
\tag{P9.4}
\]

The summably approximate version in S8 is equivalent for the present purpose: if the right side is \((1+e_k)H_k\), with \(e_k\ge0\) and \(\sum e_k\le C\), replace \(H_k\) by
\(H_k/\prod_{i<k}(1+e_i)\). Its equivalence constants stay uniform and (P9.4) follows. T9 supplies an explicit metric construction from interval bounds on the seven commuting mean channels; N9 now proves the five substantive tensor bounds through its bounded finite-part identity and the direct U9 sign calculation.

The standing AF inequalities imply, on the fixed grouped scales,
\(0<b_-\le x_k-x_{k+1}\le b_+<\infty\). In particular,

\[
\sum_{k:x_k\ge X}x_k^{-2}\le C/X
\tag{P9.5}
\]

for \(X\) above a fixed threshold.

### 2. A high-moment estimate in the ultraviolet portion

Fix an integer \(p\ge2\). Use \(|\xi|_k^2=\langle\xi,H_k\xi\rangle\), and set

\[
a_k=(\mathbb E|\xi_k|_k^p)^{1/p},\qquad
M_k=\max\{\|f_0\|,a_0,\ldots,a_k\}.
\tag{P9.6}
\]

Minkowski's inequality applied to the stable recursion gives

\[
(\mathbb E\|r_k\|^p)^{1/p}
\le q_1^k\|r_0\|+
C\sum_{i<k}q_1^{k-1-i}a_i
\le CM_k,
\qquad
(\mathbb E\|f_k\|^p)^{1/p}\le CM_k.
\tag{P9.7}
\]

The constant here is independent of \(p\). No Hilbert norm on the stable space is asserted.

For a Euclidean vector norm and \(p\ge2\), Taylor's formula with its second-derivative bound gives

\[
|u+v|^p
\le |u|^p+p|u|^{p-2}\operatorname{Re}\langle u,v\rangle
+C p^2|v|^2(|u|+|v|)^{p-2}.
\tag{P9.8}
\]

Apply this in the next metric with \(u=E_k\xi_k\), \(v=\zeta_k\). The linear term has zero conditional expectation. By Hölder and Minkowski, the expectation of the last factor is at most

\[
C p^2\|\zeta_k\|_{L^p}^2
\bigl(\|E_k\xi_k\|_{L^p,H_{k+1}}
+\|\zeta_k\|_{L^p,H_{k+1}}\bigr)^{p-2}
\le C p^2t_k^2(1+Ct_k)^{p-2}M_k^p.
\tag{P9.9}
\]

Here (P9.4) bounds the deterministic mean by \(a_k\), and (P9.2), (P9.7) bound the noise. If \(p t_k\le c_0\), the factor \((1+Ct_k)^{p-2}\) is uniformly bounded. Therefore

\[
M_{k+1}^p\le(1+Cp^2t_k^2)M_k^p
\quad\text{while }x_k\ge C_0p.
\tag{P9.10}
\]

Choose \(C_0\) once, sufficiently large. The sum of \(p^2t_k^2\) over this ultraviolet portion is at most \(Cp\) by (P9.5). Thus throughout it,

\[
M_k\le C\|f_0\|.
\tag{P9.11}
\]

The split point depends on \(p\); the admissible coupling threshold does not.

### 3. Treat the remaining scales by the deterministic propagator

Let \(k_p\) be the first index at which \(x_{k_p}<C_0p\), if such an index exists. Before it, (P9.11) applies. After it, use the existing bound (P9.3) pointwise in the remaining digits, and then take the \(L^p\) norm. Since the terminal weak endpoint is fixed below by \(x_K\ge X_*>0\),

\[
\sup_{k\le K}(\mathbb E\|f_k\|^p)^{1/p}
\le C(1+p)^{p_{\mathrm b}}\|f_0\|.
\tag{P9.12}
\]

If \(x_0<C_0p\), use (P9.3) from the initial step instead. If no \(k_p\) exists, (P9.11) covers the whole interval. These cases include every moment order at the same fixed weak endpoint.

#### Theorem P9-A: fixed factorial phase moments

Let \(\nu=\lceil p_{\mathrm b}\rceil\). Under (P9.1)–(P9.5),

\[
\boxed{
\sup_{k\le K}\mathbb E\|f_k\|^m
\le C^{m+1}(m!)^{\nu}\|f_0\|^m
\qquad(m\ge1).
}
\tag{P9.13}
\]

For \(m\ge2\), this follows from (P9.12) and
\(m^m\le e^m m!\). The case \(m=1\) follows from the second moment. If \(p_{\mathrm b}=0\), the interpretation \(\nu=0\) is valid. All constants and the weak-coupling threshold are independent of \(m\).

This split is stronger than using the crude estimate
\(\exp(Cm^2\sum t_k^2)\) over the whole trajectory. That crude estimate would not supply a fixed factorial exponent. The potentially expensive scales with \(x_k\lesssim m\) instead cost only a fixed power of \(m\) in the norm, because their deterministic growth is controlled by an inverse-coupling ratio.

### 4. A common translation for several roots

For arbitrary specified roots \(x_1,\ldots,x_m\), let \(f_{k,i,z}\) be the corresponding benchmark insertion translated by the **same** microscopic \(z\), with uniformly bounded deterministic initial norm. Each root separately has the independent-digit representation, although the phase words of the different roots are correlated.

Hölder's inequality in the one common translation average gives

\[
\operatorname{Av}_z\prod_{i=1}^m\|f_{k,i,z}\|
\le\prod_{i=1}^m
\left(\operatorname{Av}_z\|f_{k,i,z}\|^m\right)^{1/m}
\le C^{m+1}(m!)^\nu\prod_i\|f_{0,i}\|.
\tag{P9.14}
\]

No independence between different roots is used. Therefore a complete original-kernel marked expansion with a fixed factorial local coefficient budget would retain a fixed factorial budget after this phase average. The theorem supplies this order bookkeeping; it does not construct that complete mixed-history expansion.

The bounded initial normalization is currently available for the scalar and the pseudoscalar mean families. A full 21-channel renormalized microscopic seed can have additional channel-dependent ultraviolet factors, so P9.13 must not be applied to that seed without its own initial-norm estimate. Likewise a history-born forcing term need not have independent future digits: its existing deterministic age-weighted propagation estimate remains the appropriate input.

---
