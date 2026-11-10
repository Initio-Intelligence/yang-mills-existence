# Protected-core hierarchy and selected terminal control

**Current status:** The carrier and selected-terminal qualifications remain. The companion notes add all-order clean/prefix histories and regular phase moments; it does not promote a selected terminal estimate to the full terminal old field.

**Status:** The estimates below sharpen the actual protected-core contribution. They do not identify that conditional contribution with the complete S2 defect. The remaining full-law interfaces are stated explicitly.

### 1. A sharper use of the existing rare-core reserve

The [protected-core transport notes](local_sources/protected_core_transport.md) prove a normalized conditional core-gas estimate of the form

\[
|\kappa^{\rm core}_{m,k}(\mathbf x\mid e)|
\le C^{m+1}(m!)^\Delta
\max\{h_k^{-\Delta},\delta^{-\Delta}\}^{m}
\eta_k\exp\left[-c\frac{\delta}{h_kR_k}\right],
\qquad \eta_k=e^{-c_0p_0(g_k)}.
\tag{S7.1}
\]

Here \(e\) is the still-fixed exterior, \(\delta=\min\{1,\min_{i\ne j}|x_i-x_j|\}\), and lengths are temporarily in terminal-scale units. The carrier has no remaining unprocessed exterior large-field components. The marks use the fixed protected-root selectors of CG0 and remain actual old marks in the source operations. All the restrictions of PC-C and CG14 are retained.

The previous estimate replaced the radius by a small inverse power of \(h_k\), losing part of the spatial singular exponent. That replacement is unnecessary when the rare-core factor is retained. The localization radius is only a fixed power of \(\log g_k^{-2}\), while the source penalty is a larger power inside an exponential.

Write

\[
x_k=g_k^{-2},\qquad t_k=\log(e+x_k),
\]

and assume the admitted quantitative trajectory and source parameter bounds

\[
x_k\ge x_K+c_-(K-k),\qquad
p_0(g_k)\ge c_p t_k^P,\qquad
1\le R_k\le C_Rt_k^\rho,
\qquad P>1.
\tag{S7.2}
\]

The first condition is the route's trajectory premise. The radius is the source's least-power-of-\(L\) choice; replacing \(\log x\) by \(\log(e+x)\) only changes fixed constants in its small-coupling range. The protected-core induction still needs its previously stated reserve \(p_0/R^{d+2}\to\infty\). In the pure-power parametrization and \(d=4\), the sufficient choice is \(P>6\rho\). No new trajectory theorem is claimed here.

#### Lemma S7-A: factorial moments of the localization radius

For each fixed \(b\ge0\), there are fixed constants \(C_b,c_*>0\) such that, for every integer \(m\ge1\),

\[
\boxed{
\sum_{k=0}^{K}\eta_kR_k^{bm}
\le C_b^{m+1}(m!)^{\rho b/P}
\exp[-c_*t_K^P].
}
\tag{S7.3}
\]

The threshold and constants do not depend on \(m,K\), the microscopic cutoff, or the torus volume. A fixed terminal matching range can alternatively be used, with the final exponential absorbed in the constant.

**Proof.** Let \(a=c_0c_p>0\), decreasing it once if a source reserve has already been spent. Split the penalty into two equal parts:

\[
\eta_kR_k^{bm}
\le C_R^{bm}
\left[t_k^{\rho bm}e^{-at_k^P/2}\right]
e^{-at_k^P/2}.
\tag{S7.4}
\]

For \(q=\rho b\), maximizing the bracket over \(t>0\) gives

\[
\sup_{t>0}t^{qm}e^{-at^P/2}
=\left(\frac{2qm}{aPe}\right)^{qm/P}
\le C^{m}(m!)^{q/P},
\tag{S7.5}
\]

with the evident interpretation when \(q=0\). This is an optimization of a power of \(\log x\), not of \(x^{cm}\). The latter would have a different and potentially superfactorial behavior.

Choose the fixed lower threshold for \(x_K\) so that \((a/4)t^P\ge2t\) for every allowed \(t\). Then

\[
\begin{aligned}
\sum_k e^{-at_k^P/2}
&\le e^{-at_K^P/4}\sum_k(e+x_k)^{-2}\\
&\le e^{-at_K^P/4}
\sum_{n\ge0}(e+x_K+c_-n)^{-2}
\le C e^{-at_K^P/4}.
\end{aligned}
\tag{S7.6}
\]

Combining these estimates proves the lemma. \(\square\)

#### Theorem S7-B: the bare protected-core hierarchy has spatial order \(4m\)

With \(\Delta>0\) fixed in (S7.1),

\[
\boxed{
\sum_k\sup_e
|\kappa^{\rm core}_{m,k}(\mathbf x\mid e)|
\le
C^{m+1}(m!)^{\,2\Delta+\rho\Delta/P}
\delta^{-\Delta m}e^{-c_*t_K^P}.
}
\tag{S7.7}
\]

**Proof.** If \(h_k\ge\delta\), the maximum in (S7.1) is \(\delta^{-\Delta}\), and the desired bound follows after discarding the spatial exponential. If \(h_k<\delta\), put \(u=\delta/(h_kR_k)\). Then

\[
h_k^{-\Delta m}e^{-c\delta/(h_kR_k)}
=\delta^{-\Delta m}R_k^{\Delta m}u^{\Delta m}e^{-cu}
\le C^m(m!)^\Delta\delta^{-\Delta m}R_k^{\Delta m}.
\tag{S7.8}
\]

Because \(R_k\ge1\), the last expression also bounds the coarse-scale case. Insert it into (S7.1), and apply Lemma S7-A with \(b=\Delta\). \(\square\)

For bare dimension-four fields, the factorial exponent is \(8+4\rho/P\) and the singular order is exactly \(4m\). Under the sufficient source choice \(P>6\rho\), one may use the convenient integer factorial exponent nine:

\[
\sum_k\sup_e|\kappa^{\rm core}_{m,k}(\mathbf x\mid e)|
\le C^{m+1}(m!)^9\delta^{-4m}e^{-c_*t_K^P}.
\tag{S7.9}
\]

At \(m=2\), this proves the sharp protected-core power \(\delta^{-8}\). It improves the \(\delta^{-10}\) sufficient all-order estimate recorded in the [protected-core transport notes](local_sources/protected_core_transport.md). It does not prove the full physical covariance because the conditioning and protected-root selection have not been removed.

### 2. Preserve logarithmic incoming normalization without changing dimension four

Let

\[
T(h)=1+\log(1/h),\qquad 0<h\le1.
\tag{S7.10}
\]

Suppose the same deterministic microscopic field normalization gives the seed bound

\[
|F_i|\le A_i a^{-4}T(a)^s,
\qquad s\ge0\text{ fixed}.
\tag{S7.11}
\]

This bound must be established for the actual common field family. The theorem below preserves it; it does not construct the normalization. A scalar identity subtraction must be included in (S7.11) unless it is a single deterministic constant removed from the complete observable outside all history selectors. For a selected mark \(\chi_iF_i\), replacing \(F_i\) by \(F_i-c_i\) produces the random term \(\chi_i c_i\); that term must remain in the seed bound or be matched explicitly with complementary sectors. Carrier-dependent conditional means are not removed.

#### Lemma S7-C: logarithmic first-meeting charge

Fix any \(\epsilon>0\) and write \(q=4+\epsilon\). On the protected-core class of PC-C, one common threshold gives

\[
\boxed{
\left|\mathcal T'_k(X)\prod_{i=1}^mF_i\right|
\le C^{m+1}(m!)^q
\left(\prod_iA_i\right)
\delta^{-4m}T(\delta)^{sm}
\eta_k e^{-\kappa_*d_k(X)},\qquad m\ge2.
}
\tag{S7.12}
\]

The one-root version is

\[
|\mathcal T'_k(X)F_1|
\le CA_1h_k^{-4}T(h_k)^s
\eta_ke^{-\kappa_*d_k(X)}.
\tag{S7.13}
\]

**Proof.** Keep the first-meeting stopping rule of PC-C. If a root stops at step \(r\), the exact factorization of its incoming scale is

\[
a^{-4}T(a)^s
=h_r^{-4}T(h_r)^s
\prod_{j=1}^{r}
\left[L^4\left(\frac{T(h_{j-1})}{T(h_j)}\right)^s\right].
\tag{S7.14}
\]

Since \(h_j=Lh_{j-1}\),

\[
\frac{T(h_{j-1})}{T(h_j)}
=1+\frac{\log L}{T(h_j)}
\le1+\log L.
\tag{S7.15}
\]

Before a first meeting, every charged component-step contains at most one root. The logarithm of the extra charge is therefore at most

\[
4\log L+s\log(1+\log L),
\tag{S7.16}
\]

independently of \(m\). The source budget enlargement in PC8–PC10 applies with this fixed charge. Its final ordinary spatial reserve and a fixed geometric exponential reserve remain available.

At a meeting event \((j,Z)\), all roots that stop there have \(h_r=h_j/L\). Put \(u=\delta/h_j\). The physical diameter reserve gives \(q_j(Z)\ge c\delta/h_j=cu\). Also

\[
T(h_r)=T(\delta)+\log u+\log L
\le C_L T(\delta)(1+\log_+u).
\tag{S7.17}
\]

For every fixed \(s,\epsilon\),

\[
(1+\log_+u)^s\le C_{s,\epsilon}(1+u)^\epsilon.
\tag{S7.18}
\]

If \(n\) roots stop at this event, their remaining scale factors, multiplied by its geometric reserve, are at most

\[
C^n\delta^{-4n}T(\delta)^{sn}
u^{4n}(1+u)^{\epsilon n}e^{-cu}
\le C^n(n!)^{4+\epsilon}
\delta^{-4n}T(\delta)^{sn}.
\tag{S7.19}
\]

For \(u\le1\), use a fixed constant; for \(u\ge1\), use \((1+u)^{\epsilon n}\le2^{\epsilon n}u^{\epsilon n}\) and the same factorial maximization as PC16. The meeting groups partition the root labels, so \(\prod_en_e!\le m!\). Apply the positive history majorant with the fixed charge (S7.16). This proves (S7.12). For one root, charge through scale \(k\), leaving exactly the factor in (S7.13). \(\square\)

The constant may depend on the fixed logarithmic order \(s\) and the chosen \(\epsilon\). Neither varies with the number of insertions. In particular, this does not replace a logarithm by an extra physical singular power.

### 3. Exact connected normalization with the logarithmic seed class

Define

\[
B_k(\delta)
=\max\{h_k^{-4}T(h_k)^s,\,
\delta^{-4}T(\delta)^s\}.
\tag{S7.20}
\]

All subset moments in the matched core operations now obey

\[
|\mathcal T_{k,I}(X)|
\le C^{|I|+1}(|I|!)^q B_k(\delta)^{|I|}
\eta_ke^{-\kappa_*d_k(X)},\qquad q=4+\epsilon.
\tag{S7.21}
\]

For one label, use (S7.13); for at least two, use (S7.12). The empty coefficient has the original unmarked bound. The pointwise proof still allows an additional bounded integrand, as required for the operation-valued Mayer expansion.

Repeat the finite-algebra construction of CG3–CG14 with

\[
r_k=\frac{\varepsilon_0}{C B_k(\delta)m^q}.
\tag{S7.22}
\]

The calculation

\[
\sum_{l=1}^m\binom ml(l!)^q
\frac{\varepsilon_0^l}{m^{ql}}
\le\sum_{l=1}^m\varepsilon_0^l
\tag{S7.23}
\]

is unchanged because \(q\ge1\). The same marked activity, anchored KP, and logarithmic-normalization estimates therefore give the actual conditional connected coefficient

\[
\boxed{
|\kappa^{\rm core}_{m,k}(\mathbf x\mid e)|
\le C^{m+1}(m!)^q B_k(\delta)^m
\eta_k e^{-c\delta/(h_kR_k)}.
}
\tag{S7.24}
\]

This uses the same carrier, fixed per-root selectors, and conditioning as CG14. No division by a small individual core mass is introduced.

#### Theorem S7-D: sharp spatial power with logarithmic field normalization

Under (S7.2) and (S7.11),

\[
\boxed{
\sum_k\sup_e|\kappa^{\rm core}_{m,k}(\mathbf x\mid e)|
\le C^{m+1}(m!)^{q(2+\rho/P)}
\delta^{-4m}T(\delta)^{sm}e^{-c_*t_K^P},
\qquad q=4+\epsilon.
}
\tag{S7.25}
\]

**Proof.** The function \(h^{-4}T(h)^s\) decreases as \(h\) increases. Thus, if \(h_k\ge\delta\), the maximum in (S7.20) is its second argument. If \(h_k<\delta\), put \(u=\delta/(h_kR_k)\), and write

\[
T(h_k)=T(\delta)+\log R_k+\log u
\le T(\delta)(1+\log R_k)(1+\log_+u).
\tag{S7.26}
\]

Apply (S7.18) once with \(u\), and once with \(R_k\ge1\). The same factorial maximization gives

\[
B_k(\delta)^m e^{-c\delta/(h_kR_k)}
\le C^m(m!)^q
\delta^{-4m}T(\delta)^{sm}R_k^{qm}.
\tag{S7.27}
\]

This also bounds the coarse-scale case. Insert it into (S7.24), then use (S7.3) with \(b=q\). \(\square\)

Under the sufficient source choice \(P>6\rho\), take \(\epsilon=1/8\). Then

\[
q(2+\rho/P)<\frac{33}{8}\frac{13}{6}
=\frac{143}{16}<9.
\tag{S7.28}
\]

Consequently the convenient fixed exponent nine still suffices even with any fixed logarithmic incoming order \(s\):

\[
\sum_k\sup_e|\kappa^{\rm core}_{m,k}(\mathbf x\mid e)|
\le C^{m+1}(m!)^9
\delta^{-4m}T(\delta)^{sm}e^{-c_*t_K^P}.
\tag{S7.29}
\]

The numerical exponent is not optimized. The advance is retaining engineering dimension four and one hierarchy-wide threshold while keeping the logarithmic normalization explicit.

### 4. The resulting S2 contribution in physical units

Restore terminal length \(\ell_0\). For \(0<r=|x-y|\le\ell_0\), multiply the dimensionless two-root estimate by \(\ell_0^{-8}\), and set \(\delta=r/\ell_0\). Then

\[
\boxed{
\sum_k\sup_e
|\kappa^{\rm core}_{2,k}(x,y\mid e)|
\le C r^{-8}
\left(1+\log\frac{\ell_0}{r}\right)^{2s}
e^{-c_*[\log(e+g_K^{-2})]^P}.
}
\tag{S7.30}
\]

Every supremum is over the source-admitted exterior for the restricted carrier. An arbitrary probability average of these absolute bounds is legitimate. Thus this controls the corresponding term in any exact full-law decomposition that identifies it with those conditional core coefficients.

The estimate is already summed over the reset scales. It is useful for the S2 exit criterion even if its individual terms are not reorganized into precisely the pointwise shell majorant (12) of the route. The covariance telescope requires an absolute bound on the sum of the actual contributions; it does not require that one predetermined proof of each contribution be used.

There is no claim that the sum in (S7.30) equals the complete covariance or the complete defect. The exterior conditional means, regular/core cross terms, nonprotected marks, and unprocessed exterior components remain to be included. The selected conditional covariance can also contain both signs; the proof bounds its absolute value rather than asserting positivity of each cluster term.

### 5. Exact S2 bookkeeping for the combined gates

For the frozen positive transport, retain

\[
F_{k+1,n}=Q_kF_{k,n},\qquad
D_{k,n}(x,y)=Q_k(F_{k,n}(x)F_{k,n}(y))
-F_{k+1,n}(x)F_{k+1,n}(y).
\tag{S7.31}
\]

The exact covariance identity is

\[
\operatorname{Cov}_{\mu_{0,n}}(F_{0,n}(x),F_{0,n}(y))
=\sum_{k<K}\mathbb E_{\mu_{k+1,n}}D_{k,n}(x,y)
+\operatorname{Cov}_{\mu_{K,n}}(F_{K,n}(x),F_{K,n}(y)).
\tag{S7.32}
\]

The work in this part closes the sharp protected-core summation needed by a possible decomposition of its first term. Gate 1 must supply the actual regular input/output class, Gate 2 the common normalization and its logarithmic bound, and Gate 3 the exact normalized integration of the other history sectors and their conditional means. Once those identify all terms in (S7.32), the regular hard-cutoff covariance estimate and shell sum can be applied on their proved carriers.

The remaining terminal target is

\[
\|F_{K,n}(x)-\mathbb E F_{K,n}(x)\|_{L^2(\mu_{K,n})}
\le C\ell_0^{-4}.
\tag{S7.33}
\]

This is a bound on the actual old numerator ratio in the chosen terminal sigma-algebra. A fresh-field bound or a subtraction chosen separately on each carrier does not establish it. A proof can use a bounded terminal operator representation plus an \(L^2\) remainder, but that representation must include all residual history functions.

**Gate 4 status from this module:** a sharp, logarithmically normalized protected-core S2 contribution is proved, and its all-order extension improves the prior singular exponent. The complete S2 defect and terminal theorem are not proved by these estimates alone.

#### 5.1 A completed terminal second-moment estimate on the protected carrier

There is also a useful partial terminal theorem. Its proof uses a single composite root; it does not take a coincident-point limit of the separated-root estimate.

Let \(0\le\chi\le1\) be a fixed genuine local history selector in the conditional core gas, with no remaining unprocessed exterior component. Require \(\chi=0\) unless the complete seed lies in a processed protected core component; in particular, the selected marked numerator vanishes for the empty core family. Let \(\widetilde F=F-c\), where \(c\) is the common deterministic physical subtraction, and assume the bound for the complete incoming centered seed

\[
|\widetilde F|\le A a^{-4}T(a)^s.
\tag{S7.34}
\]

The selected mark is \(H=\chi\widetilde F\). It remains the old seed throughout its protected ancestry. In particular, the scalar and cross terms in \(\chi(F-c)^2\) are retained.

#### Theorem S7-E: the selected posterior mean has a terminal \(L^2\) bound

For the actual normalized conditional core law at scale \(k\),

\[
\boxed{
\mathbb E_{\mathrm{core}}[\chi\widetilde F^2\mid e]
\le C A^2 h_k^{-8}T(h_k)^{2s}\eta_k.
}
\tag{S7.35}
\]

The constant is uniform over admitted exteriors. Consequently, for any conditional expectation \(M=\mathbb E[H\mid\mathscr G]\) within this same normalized conditional law, followed by any probability average of the admitted exterior,

\[
\|M-\mathbb E M\|_{L^2}
\le \|M\|_{L^2}
\le C A h_k^{-4}T(h_k)^s\eta_k^{1/2}.
\tag{S7.36}
\]

**Proof.** Regard \(\chi\widetilde F^2\) as one composite insertion of engineering dimension eight and fixed logarithmic degree \(2s\). Charge its entire unresolved age at the fixed rate

\[
8\log L+2s\log(1+\log L).
\tag{S7.37}
\]

There is only one charged root per component-step. The positive history budget therefore absorbs this fixed enlargement, leaving the output factor \(A^2h_k^{-8}T(h_k)^{2s}\), the rare factor, and the ordinary spatial reserve. The resulting one-root marked activity has the same unused weighted KP reserve as the one-root construction in CG. Its coefficient in the normalized logarithmic generating function is the actual expectation of this composite insertion. The rooted sum gives (S7.35). The expectation is nonnegative, even though its connected expansion may have signed terms.

Since \(\chi^2\le\chi\), conditional Jensen and integral preservation give

\[
\mathbb E|M|^2\le\mathbb E|H|^2
\le\mathbb E[\chi\widetilde F^2].
\tag{S7.38}
\]

Use the uniform bound (S7.35), and then subtract the unconditional mean, which can only decrease the second moment. This proves (S7.36). \(\square\)

At the terminal scale, restoring physical units gives \(C A\ell_0^{-4}\eta_K^{1/2}\). This is a proved terminal bound for the selected protected contribution on this carrier. The posterior weight of \(\chi\) is retained in \(M\); dividing by its probability would be a different statement. The result does not supply the full terminal field's regular, mixed-boundary, unprocessed-exterior, or between-carrier mean contributions.

### 6. Sources and dependencies

- The source-admitted core geometry, positive history budget, first-meeting construction, and ordinary final spatial reserve are PC1–PC20 in the [protected-core transport notes](local_sources/protected_core_transport.md).
- The actual marked component gas, fixed history selectors, full weighted KP estimate, and conditional coefficient identity are CG0–CG14 in the same notes.
- The source radius is CMP119 (1988), (2.5), printed p.255: the least power of \(L\) above a fixed power of \(\log g_k^{-2}\).
- The rare penalty and cost reserve are LFR II (1989), (1.79)–(1.89), printed pp.383–387; the marked use of the component gas is anchored in (1.90)–(1.100).
- The source definition \(p_0(g)=A_0(\log g^{-2})^{p_0}\) appears at the start of LFR I (1989), printed p.175. Its exponent and the trajectory bounds are kept as explicit fixed inputs.
- The exact S2 telescope and its complete-law and terminal requirements are taken as stated in the observable-hierarchy formulation. No N2-F argument is used as a substitute for that trajectory premise.

The new proofs above are the logarithmic stopping charge and the simultaneous rarity/radius optimization. They do not change the underlying probability law, reset kernels, source normalization, or source parameter quantifiers.

---

## Primary-source index

The marked theorems in these notes are deductions developed here. The papers below supply the cited unmarked constructions, domains, operator bounds, geometry, positivity, and normalization identities.

| Source | Main use in these notes |
|---|---|
| [Yang–Mills existence through observable derivatives](observable_route.md) | Observable route, exact positive telescope, S2 exit criterion, and subsequent existence obligations |
| Bałaban, CMP96 (1984), 223–250 (propagators and renormalization transformations II) | Flat propagator estimates and explicit dependence of available coercivity and decay constants on the fixed block factor |
| Bałaban, CMP99 (1985), 389–434 (propagators in a background field) | Background propagator estimates, normalized adjoints, localized inverses, and the small constraint-Hessian correction |
| Bałaban, CMP102 (1985), 277–309 (variational problem) | Constrained minimizing fields, nonflat equations, nonlinear force, and analytic/Hölder response |
| [Balaban, CMP109 (1987), 249–301](https://doi.org/10.1007/BF01215223) | Intrinsic independent-current source domains, fixed-domain pure activities, fixed-M-block metric, averaging geometry, and action covariance |
| [Balaban, CMP116 (1988), 1–22](https://doi.org/10.1007/BF01239022) | Switched nonlinear response, cluster expansion, support-decay regeneration, and intrinsic gauge invariance |
| Bałaban, CMP119 (1988), 243–285 (convergent renormalization expansions) | Actual birth selectors, shrinking historical domains, regular-R interpolation, density bounds, rooted insertion expansion, and source-position hats |
| Bałaban, Large field renormalization I, CMP122 (1989), 175–202 | Eligible reset components, positive normalized reset operation, and retained boundary dependence |
| Bałaban, Large field renormalization II, CMP122 (1989), 355–392 | Positive history budget, clean lifespan, component and spatial reserves, and fixed-family boundary normalization |
| [Brydges–Fröhlich–Seiler, IHES/P/78/237 (1978)](https://repo-archives.ihes.fr/FONDS_IHES/I_Prepublications/FROHLICH/1978-1980/P_78_237/P_78_237_web.pdf) | Original-Wilson reflection positivity and chessboard, Theorems 2.8 and 2.10 |
| [Lüscher, CMP85 (1982), 39–48](https://doi.org/10.1007/BF02029132) | Admissible-cell topological charge; T9 supplies the group/trace extension, uniform source-domain bounds, and actual mean comparison used here |
| [Ferretti–Heise–Zarembo, hep-th/0404187v3](https://arxiv.org/pdf/hep-th/0404187) | Continuum dimension-four one-loop comparison; U9 derives the needed finite-group principal source trace directly |
| Jaffe–Witten, *Quantum Yang–Mills Theory* (Clay problem statement) | Distinction between the reduced observable-existence target and the complete existence-and-mass-gap problem |

