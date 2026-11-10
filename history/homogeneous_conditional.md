# Primitive homogeneous conditional Gaussian comparison

The conditional law, the R test and the common analytic chart are fixed throughout; the transfer to another law requires CL.

## 1. The exact fiber and the estimates used

Fix an admitted source-free step, an active component of the replacement, its retained exterior and an allowed axial graph. Write \(g=g_k\), \(\ell=\log g^{-2}\), \(p=p_0(g)=\varepsilon_k/g\), \(P=M_0p\), and \(R=R_k\). The source has \(p=A_0\ell^{p_0}\) and \(R\ge\ell^r\). The fresh variable is \(V'=\exp(igB)\). Its graph links equal the identity and the cutoff on each remaining bond is \(|B(b)|<P\). Call this product set \(D_P\). The integration is in graph coordinates, with the Euclidean norm and counting measure of the unit coarse lattice. All fixed norm equivalences on one Lie algebra are absorbed in constants. The core is contained in a cube of side \(100M\), so the real dimension \(m\) satisfies \(m\le m_*=4\dim(G)(100M+1)^4\). The construction fixes \(M\). The core volume obeys \( |\Lambda|\le (100M+1)^4\). The component outside the core may be larger. This estimate counts fresh integration variables only. LFR I, pp. 192–194, 201, (1.73), (1.100)–(1.101) CMP119, p. 255, (2.4)–(2.5)

Let \(U_0=U_{k,Z}(V_\Lambda)\) be the actual reference minimizing filling and let \(Q_v\) be the real symmetric form of LFR II (1.2), restricted to the graph complement:
\[
 Q_v[B,B]=\langle H_{1,k}B,\Delta_1(\zeta_0) H_{1,k}B\rangle .
\]
The variable \(v\) records the exterior and the fixed branch choices. The localization function \(\zeta_0\) remains in the form. Including its normalization, the exact probability on the fresh fluctuation is
\[
 K_v(dB)=\frac{\mathbf1_{D_P}(B)\exp[-Q_v[B,B]/2+u_v(B)]\,dB}
 {\int_{D_P}\exp[-Q_v[b,b]/2+u_v(b)]\,db}. \tag{1}
\]
Here \(u_v\) contains the full normalized logarithmic Haar density, the linear term of (1.2) and the nonlinear remainder. The constant terms \(-g^{-2}A(\zeta_0,U_0)+E_k(\Lambda)\) cancel. No part of the old numerator action \(\mathcal A_k''\) enters this reference fiber. The exterior extension selector is fixed on this branch. The restriction on the new field is \(D_P\), independent of \(v\) in these coordinates. LFR I, p. 201 LFR II, pp. 356–358, (1.1)–(1.11)

For sufficiently small \(g\), the cited estimates give a lower bound, uniform in \(v,k\), of
\[
 Q_v\succeq\lambda I,\qquad \lambda=\frac{\gamma_0}{2d(100M)^5},\quad d=4. \tag{2}
\]
Writing \(C_*\) for a constant depending on construction parameters and group conventions, choose the exponent \(0<\beta<1\) in the source's cubic-remainder estimate. On the actual support,
\[
 \sup_{D_P}|u_v|\le d_k :=
 C_*\bigl[(100M)^4 p^2e^{-R}
       + |\Lambda|g^{1-\beta}
       + m_* g^2P^2\bigr]. \tag{3}
\]
For the linear term use (1.5)–(1.6), where stationarity moves it to the tail of \(1-\zeta_0\); the second printed line of (1.6) bounds the result by a constant times \(p^2 e^{-R_k}(100M)^4\). The estimate for the cubic term follows in the text after (1.2). The logarithm of the one-link Haar density divided by its value at the origin is even and analytic there. This follows from inversion invariance of Haar measure and analyticity of the exponential Jacobian. Its absolute value is at most \(C|gB(b)|^2\) if \(gP\) is sufficiently small. Summing over the free bonds gives the final term in (3). These estimates show \(d_k\to0\) as \(g\to0\) uniformly in the admissible data. No infinite-volume measure or coupling beta-function calculation is needed for this single-step estimate. LFR II, pp. 356–358

## 2. Weighted variation and normalized marked response

Let \(N_v\) be the centered Gaussian on the free graph coordinates with covariance \(Q_v^{-1}\), on the full Euclidean space. For a signed measure use the variation measure convention \(\|\mu\|_W=\int W\,d|\mu|\), so the unweighted distance can reach 2. There are constants \(C,c>0\) depending only on group and construction parameters such that, with \(a=\lambda/16\),
\[
 \|K_v-N_v\|_{\exp(a|B|^2)}
 \le C\bigl[d_k+ e^{-c\lambda P^2}\bigr] =: C e_k . \tag{4}
\]
All these statements also hold with the point mass in dimension zero.

**Proof.** Work first with the Euclidean Lie norm on a bond. If the cutoff uses an equivalent norm, its complement implies \(|B|\ge c_G P\) with \(c_G>0\) fixed. A Gaussian with precision bounded below by \(\lambda I\) satisfies \(N_v(e^{s|B|^2})\le(1-2s/\lambda)^{-m_*/2}\) for \(0<s<\lambda/2\). Markov's inequality with \(s=\lambda/8\) bounds \(N_v(e^{a|B|^2}\mathbf1_{D_P^c})\le C\exp[-(\lambda/8)c_G^2P^2]\) by using the exponential moment at \(a+s\). In (1) the density relative to \(N_v\) is \(\mathbf1_{D_P}e^{u_v}/z\), where \(z=N_v(\mathbf1_{D_P}e^{u_v})\). Thus \(|z-1|\le e^{d_k}-1+N_v(D_P^c)\) and \(z\ge1/2\) for sufficiently small \(g\). On \(D_P\), \(|e^{u_v}/z-1|\le C(d_k+N_v(D_P^c))\). The weighted integral on the complement is the preceding tail bound. This proves (4).

For \(|f(B)|\le e^{a|B|^2}\) it follows that \(|K_v(f)-N_v(f)|\le C e_k\). In particular, a tensor product of \(s\) unit linear coordinates has absolute expectation error bounded by \(C e_k(s/(2ea))^{s/2}\) for \(s\ge1\), by maximizing \(x^se^{-ax^2}\). For the exponential linear source define \(Z_K(t)=K_v(e^{\langle t,B\rangle})\), using the complex bilinear extension. On the complex Euclidean ball \(|t|\le t_0\), for any fixed \(t_0\), (4) gives
\[
 |Z_K(t)-\exp(t^TQ_v^{-1}t/2)|\le C e_k e^{t_0^2/(4a)}.
\]
The modulus of the Gaussian expression is at least \(e^{-t_0^2/(2\lambda)}\). For sufficiently small \(g\) their ratio is within \(1/2\) of one. The logarithm anchored at zero therefore satisfies \(\sup_{|t|\le t_0}|\log Z_K(t)-t^TQ_v^{-1}t/2|\le C_{t_0}e_k\). For \(s\) unit linear marks, the polydisc of individual source radii \(t_0/s\) lies in the ball after the sources are added. Cauchy's formula bounds the mixed cumulant error by \(C_{t_0}e_k(s/t_0)^s\le C_{t_0}e_k(e/t_0)^s s!\). This comparison uses the same normalized reference at each retained datum. When observables are functions of the physical product \(V'V_\Lambda(v)\), one evaluates both laws on the corresponding map \(B\mapsto \exp(igB)V_\Lambda(v)\).

## 3. Complex normalization on the primitive source domain

Keep the fresh integration variable real and the graph and cutoff fixed. For the primitive continuation in LFR II p. 358 the retained variable is \(U\in\mathcal U_k^c(Z,\alpha_{0,k},\alpha_{1,k})\), with exterior inputs replaced by \(M^k(U)\) in the minimizing filling. Define
\[
 h_U(B)=\mathbf1_{D_P}(B)\sigma(gB)
 \exp[-Q_U[B,B]/2+L_U(B)+T_U(B)],\qquad
 I_0(U)=\int h_U(B)\,dB .
\]
Here \(L_U,T_U\) denote exactly the linear and nonlinear terms of (1.2) with their exponent signs. The one-link normalization of \(\sigma\) is absorbed into the fixed constant of (1.2). Comparing (1.2) to the inverse-normalizer formula (1.10) gives the complex identity
\[
 I_0(U)=e^{-I(U_0)},\qquad |I(U_0)|\le C\log M\,|\Lambda|\le C M^5. \tag{5}
\]
In particular the integral cannot vanish anywhere on this source domain, and its reciprocal has modulus at most \(e^{CM^5}\). The large potentially complex factor \(\exp[-g^{-2} A(\zeta_0,U_0)]\) was canceled before taking moduli. Positivity of the real normalizer would not prove (5). LFR II, p. 358, (1.10)–(1.11)

The marked kernel requires additional care. Complex gauge transformations can change the real graph integration cycle. The scalar identity (5) continues gauge-invariant normalizers. By itself it gives no estimate for an arbitrary graph-coordinate mark at a complex representative. Here is a quantitative local transfer that specifies the missing input.

Fix a gauge representative and a polydisc \(U(w)\), \(|w_i|<r_i\), with \(U(0)\) a physical real base. Use the same real graph cycle and the same cutoff throughout. Suppose (1.2) and (5) hold in those coordinates and
\[
 \sup_{w,\,|b|=1,\,b\ {\rm real}}|Q_{U(w)}[b,b]|\le B_Q,\qquad
 \sup_{w,\,B\in D_P}|L_{U(w)}(B)+T_{U(w)}(B)|\le B_T .
 \tag{6a}
\]
Set \(\theta=\min(1/4,\lambda/(4B_Q))\), with \(\theta=1/4\) for \(B_Q=0\). For \(w\) in the polydisc with radii \(\theta r_i\), restrict \(Q\) to the complex line through \(0,w\). Cauchy's geometric-series estimate gives
\[
 |Q_{U(w)}[b,b]-Q_{U(0)}[b,b]|
 \le B_Q\frac{\theta}{1-\theta}|b|^2\le\frac{\lambda}{2}|b|^2 .
\]
Together with (2), (5), and bounded Haar density on \(D_P\), this proves on that reduced polydisc
\[
 \int e^{a|B|^2}\,d|K_{U(w)}|(B)\le C_{M,G,B_T}.
 \tag{6}
\]
One may take a constant proportional to \(e^{CM^5+B_T}(1+\sqrt{\pi/(\lambda/4-a)})^{m_*}\), allowing for the fixed Haar normalization. For multi-indices \(\nu\), scalar Cauchy against all measurable tests bounded in modulus by \(e^{a|B|^2}\) gives
\[
 \left\|\left.\partial_w^\nu K_{U(w)}\right|_{w=0}\right\|_{\exp(a|B|^2)}
 \le C_{M,G,B_T}\,\nu!\prod_i(\theta r_i)^{-\nu_i}. \tag{7}
\]
Analyticity under the integral follows by the same Gaussian majorant. All positive-order jets integrate to zero. Direct derivatives of a mark that moves with the retained data must also be included. These implications do not differentiate the exterior selector. Uniform \(B_Q,B_T\) on the gauge-fixed chart, with (5) on that same cycle, are hypotheses if (6)–(7) are used for general marks. Arbitrarily large complex gauge transformations need not preserve \(|b|\). The real comparison (4) and scalar normalization (5) do not depend on the common-cycle premise (6a).

## 4. A quantitative preparatory contour and the unproved transfer

There is an explicit contour for the minimizing-orbit factor of LFR I Proposition 1. On the active exterior from its p. 193, let \(v\) be the real exterior coarse links. The discussion following (1.75) supplies \(\sup_{p'\subset Z\cap\Lambda^c}|v(\partial p')-1|\le C_{\mathrm{ext}} L^2R_k\varepsilon_k=:b_k\), after enlarging the fixed constant. Use a faithful unitary realization and its operator norm. For arbitrary complex coarse link increments of sup norm at most \(s\), write \(v'(b)v(b)=e^{iX_b}v(b)\). A telescoping product, using \(\|e^{\pm iX_b}\|\le e^s\) and \(\|e^{\pm iX_b}-I\|\le e^s-1\), bounds the change in every plaquette by \(e^{4s}-1\); orientations only conjugate these factors by unitary matrices. Take \(s\le b_k/16\) and \(b_k\) sufficiently small. Then every new plaquette is within \(2b_k\) of identity, and each relative link logarithm has norm less than \(2b_k\). Proposition 1, with its adjustable small parameter \(\varepsilon=2b_k\), applies to this entire contour. Consequently the *orbit-valued filling* for the actual selected exterior admits a physical coarse-link tube of radius \(b_k/16\), uniform over those exteriors. A choice of representative must follow its source gauge. This argument uses the larger regularity parameter only in Proposition 1. It does not impose a different real selector or enlarge any primitive activity domain. LFR I, pp. 193–194, Proposition 1

To apply (7) to current-coordinate localized activities one must still prove a joint radius for the complete input. More precisely, let \(F_{j,k,Y,\sigma}(z)\) denote the actual pair consisting of the localized field and independently extended current, including each stage (1.61)–(1.65) of LFR II, with the allowed complex decoupling data \(\sigma\). For every real \(z\) in the source-normal-form regular product support (C7.2) at fixed retained data and each differentiated coordinate pair \(i,l\), one needs a simultaneous inclusion
\[
 F_{j,k,Y,\sigma}(z+w_i e_i+w_l e_l)\in
 \mathcal D_{j,k,Y,\sigma}^{\rm source},
 \quad |w_i|,|w_l|<r_{j,k,Y}(z),\quad\text{uniformly in }\sigma, \tag{8}
\]
where each source-domain constraint is imposed at its corresponding stage, including the reconstructed plaquettes and currents, local gauges, relative complex field and discrete derivatives. LFR II p. 375 (1.65) transfers a primitive source-domain input to the prepared one. To use it in (8) requires admission of the current input on a quantitative tube about the actual cutoff points. Admission of the exterior minimizing orbit alone does not provide the other inputs of (1.65). LFR II, pp. 374–375 CMP119, pp. 259–261, 276–277

Writing \(D(z,r)\) for the pair disc in (8), a sufficient missing marginal and localization inequality for R is
\[
 \sup_z\sup_i\sum_{Y\ni i}\sum_{l\in Y}e^{\gamma d(i,l)}
 \frac{\sup_{D(z,r_{j,k,Y}(z))}|V^R_{j,k,Y}|}{r_{j,k,Y}(z)^2}
 \le C\ell_j^A g_j^{\kappa_0}\frac{g_k^2}{a_j^2}\Theta_k^2. \tag{9}
\]
Here \(a_j\) is the admitted old-field radius of Annex G, and \(\Theta_k\) the current-field budget factor in its (4.4). In (9) decoupling integrals, preparation and carrier multiplicities belong to \(V^R_{j,k,Y}\); an absolute expansion requires corresponding absolute majorants. The four powers \(L^{-4(k-j)}\) compensating old-cell multiplicity must already be realized before the sum in (9). They do not follow from (5), (6), or the smallness of a single fiber in (4). Until (8) and (9) are verified at the required scales, neither C-03 nor C-04 is closed. E additionally requires its own subtracted activity estimate on the same jointly admitted charts. The old numerator, the selected marginal and re-use of fresh labels in future marked maps retain their full normalized response.

## 5. Recovering the four old-scale powers on a narrower complex contour

There is another route to the marginal part of (9). A crude holomorphic bound and a real marginal estimate on *the same coefficient and same coordinates* suffice. The loss in the contour radius is polynomial in the age. This section proves the transfer and identifies the remaining mismatch in the published estimates.

**Lemma.** Let \(E_\rho\) denote the filled ellipse with foci \(\pm1\) and major semiaxis \((\rho+\rho^{-1})/2\). Let \(f\) be holomorphic near the interior of \(E_2\times E_2\), with supremum at most \(M\) there and supremum at most \(m\) on the real square \([-1,1]^2\), where \(0<m\le M\). There are absolute constants \(C,C_0\) such that, setting
\[
 N=\max\{4,\lceil\log_2(C_0M/m)\rceil\},\qquad
 \delta_N=(4N^2)^{-1},
\]
the supremum of \(|f|\) on the coordinatewise complex \(\delta_N\)-neighborhood of the full square is at most \(Cm\). In physical coordinates with real half-widths \(r_1,r_2\), this gives
\[
 |\partial_1\partial_2 f(x)|\le C\,m N^4/(r_1r_2)
 \tag{10}
\]
at all points of the closed real rectangle. The same-coordinate second derivative obeys \(CmN^4/r_1^2\). One-sided source intervals with \(x\) at an endpoint are included.

**Proof.** Compose \(f\) with \(z_i=(w_i+w_i^{-1})/2\) in both variables. The Laurent coefficients on the two annuli obey the corresponding Cauchy bounds by taking circles interior to radius 2 and passing to the limit. Invariance under \(w_i\leftrightarrow w_i^{-1}\) yields the Chebyshev series \(f=\sum_{n,l\ge0}c_{nl}T_n(z_1)T_l(z_2)\), with \(|c_{nl}|\le4M2^{-(n+l)}\). Let \(P_N\) be its truncation to \(n,l\le N\). On \(E_\rho^2\) for \(\rho=e^{1/N}\), \(|T_n|\le\rho^n\). The discarded rectangular tail is at most \(C_1M(\rho/2)^{N+1}\le C_2M2^{-N}\), by two geometric sums and the fixed lower bound \(N\ge4\). Choose \(C_0\ge C_2\). Then \(P_N\) has real-square norm at most \(2m\).

A univariate polynomial \(p_N\) of degree at most \(N\) obeys \(\sup_{E_\rho}|p_N|\le \rho^N\sup_{[-1,1]}|p_N|\). Indeed \(w^{-N}p_N((w+w^{-1})/2)\) is holomorphic on the exterior disc including infinity and bounded on the unit circle by the real-interval norm. Apply the maximum principle and then use the interior maximum principle on the ellipse. Applying this bound once per coordinate gives \(\sup_{E_\rho^2}|P_N|\le2m\rho^{2N}=2e^2m\). Add the preceding tail estimate. If \(\operatorname{dist}(z,[-1,1])<\delta_N\), its sum of distances to the two foci is at most \(2+2\delta_N<2\cosh(1/N)\), hence \(z\in E_\rho\). This proves the uniform complex bound. Cauchy on the resulting bidisc proves (10), including the factor 2 for a repeated derivative. If the real bound is zero, the identity theorem applied separately to the two variables gives \(f=0\).

For an old carrier at age \(a=k-j\), suppose the crude bound is \(M\) and a marginal *majorant* on the same real square is \(m=M L^{-4a}\). Then \(N\le C_L(1+a)\). The same holds if the ratio \(M/m\) is bounded by \(C L^{4a}(1+a)^b\) with fixed \(C,b\). Thus the full factor \(L^{-4a}\) survives on the smaller contour. One can use a deliberate upper majorant \(m\) even when the actual real values are much smaller. The inverse square of the radius in (10) gives an age penalty of at most \(C(1+a)^4\).

**Age summation.** Assume the numerical trajectory satisfies the old-scale estimate used in Annex G (4.5), \(\sum_{j\le n}g_j^t\le C_t g_n^{t-6}\) for \(t>6\), for all stage endpoints \(n\) under consideration. For every nonnegative integer \(q\) and \(s>6(q+1)\),
\[
 \sum_{j\le k}(1+k-j)^qg_j^s
 \le q!\left(\prod_{u=0}^q C_{s-6u}\right)g_k^{s-6(q+1)} . \tag{11}
\]
Indeed the number of nondecreasing chains \(j\le i_1\le\cdots\le i_q\le k\) is \(\binom{k-j+q}{q}\ge(1+k-j)^q/q!\). Sum over all chains from the earliest index outward, applying the assumed old-scale inequality at each endpoint. No additional monotonicity assumption enters (11). For \(q=4\) this loses at most 30 powers in total. This is a cost of the new narrower-contour route. The real value estimate in CMP119 (2.46) still loses six. With the old radius \(a_j\ge c g_j\) of Annex G, a factor \(Q_k^2/r_k^2\le \Theta_k^2g_k^2\), and a fixed \(\ell_j^A\), the corresponding Hessian sum is bounded by \(C_\epsilon\Theta_k^2 g_k^{\kappa_0-30-\epsilon}\) for \(\kappa_0>32+\epsilon\). This follows by applying (11) with \(s=\kappa_0-2-\epsilon\). The calculation assumes that the real and crude complex *carrier* bounds share any required spatial entropy reserve. It does not promote an unlocalized real estimate into an absolute bound on a chosen localized expansion.

**The remaining domain mismatch.** CMP119 p. 283 gives the four-power marginal gain for the vacuum-subtracted physical \(R^{(j)}(X,U_k)\) on regular real backgrounds, before the additional current localization used in (9). CMP119 (2.31) bounds the primitive analytic activity in a domain including an independently supplied current. The real square in the lemma has to be a real slice of the very analytic family to which it is applied. Holding the independent current at complex decoupling data need not preserve the physical slice. Even exact vanishing on the physical slice cannot control every independent-current extension: in logarithmic local coordinates a gauge-covariant current \(J_{\rm phys}(U)\) gives the gauge-invariant local analytic function \(\operatorname{tr}[(J-J_{\rm phys}(U))^2]\), which vanishes on the physical locus yet has nonzero second jet in an independent semisimple Lie-algebra current direction with nonzero trace square. This example concerns what the two bounds alone imply. The actual source supplies a specific extension, whose decoupled real estimates or regrouped real estimates must be checked. A bound for a regrouped coefficient would suffice if its two-coordinate complex domain and its current carrier are retained. Fixing \(\sigma=1\) in the real estimate while taking the supremum over complex \(\sigma\) in the analytic estimate fails this test. CMP119, pp. 259–261, 276–277, 283

An independent-current family with an admitted crude pair ellipse of half-width \(r_k\) and a real absolute marginal majorant on the corresponding two-coordinate rectangle would therefore suffice for this part of C-03. It gives an explicit usable radius \(r_k/(4N^2)\) and an old-scale sum with the losses above. The two verified source estimates currently apply on different slices for the general localized pullback. This is the unproved step left by the narrower-contour argument.

## 6. Flat homogeneous output at the first mature-R projection

A different physical regrouping is available for the bulk coupling projection. CMP119 already supplies analytic *output* birth activities after summing the internal localizations. Their one-scale space is the one specified by (2.27)–(2.28), incorporating CMP109 (1.11)–(1.16). The multiscale space (2.34)–(2.39) is introduced for boundary activities on pp. 260–261. At identity, one can exhibit an ordinary unweighted ball in the one-scale space with explicit scale cost. This estimate is specific to an output birth and its flat physical Hessian. CMP119, pp. 259–261 CMP109, pp. 262–264

Write \(n\) for the output index and \(\xi=L^{-n}\) for the fine spacing in its terminal-scale units. Put
\[
 h_n=\min(1,\alpha_{0,n},\alpha_{1,n}),\qquad
 \alpha_{u,n}=C_u g_n(\log g_n^{-2})^{q_u},\quad u=0,1.
\]
In identity link-log and independent-current coordinates consider
\[
 \|\log U\|_{\infty,X},\ \|J\|_{\infty,X}
 <\delta_n=c_0 h_n\xi^2 . \tag{12}
\]
Use a bounded faithful matrix representation and adjust \(c_0\) for fixed norm equivalences. Take the real reference configuration to be identically one. Its plaquette and local gauge-potential bounds (i) are immediate. The relative potential \(A'=(i\xi)^{-1}\log U\) satisfies \(\|A'\|\le\delta_n/\xi\), \(\|\nabla^\xi A'\|\le 2\delta_n/\xi^2\) up to the fixed number of directions. The plaquette variation is at most \(e^{4\delta_n}-1\le 5\delta_n\) for small \(\delta_n\), and the independent current already has bound \(\delta_n\). This verifies (i)–(iii) with smaller constants \(\alpha'_0,\alpha'_1\le Cc_0h_n\).

For the reconstructed fields the needed implication is given immediately after (1.16), CMP109 p. 263. For inputs satisfying (i)–(iii) with the smaller parameters, the source estimates the curvatures of the averages, applies CMP102 Proposition 9 to the reconstructed minimizing fields, and bounds their curvature and current by \(2B_3\alpha'_0\) times their respective scale factors in (1.16). It applies to the reference also. Taking \(c_0\) smaller than the reciprocal of the resulting fixed constant supplies (iv). This uses the source's quantitative smaller-space argument on the one-scale primitive domain. No comparison to the fluctuation cutoff is made in (12). CMP109, pp. 262–263

On the unrestricted homogeneous determining set, let \(\mathcal U_n(b)=(U_n(\exp ib),J_n(\exp ib))\) be the physical minimizing field and current in the flat-base chart. In the Landau representative relative to the identity, the field \(\xi^{-1}\log U_n\) is bounded on a fixed terminal \(b\) ball by CMP102 (172)–(175), Proposition 9. This is the homogeneous case of O0 §12.4. In particular \(\|\log U_n\|_\infty\le C\|b\|_\infty\) there after reducing the ball, by radial Schwarz. The current (CMP109 (1.8)) consists of the covariant difference of a projected plaquette variable divided by \(\xi^2\). Its finite stencil costs at most a further \(\xi^{-1}\) on a sufficiently small link-log ball. Its value at zero is zero. Consequently
\[
 \|J_n(\exp ib)\|_\infty\le C\xi^{-3}\|b\|_\infty .
\]
The independent-input action is invariant under the simultaneous gauge transformation of links and current, so this representative may be used for its evaluation. Equations (12) and the last two estimates give the physical output chart
\[
 \|b\|_\infty<r_n=c_1 h_n\xi^5 . \tag{13}
\]
This allows an arbitrary bounded superposition of physical plane waves with total complex amplitude below \(r_n\). If \(n\le C_*\log\log Y\) and \(g_n^{-2}\asymp Y\), then \(h_n\ge cY^{-1/2}\) for sufficiently large \(Y\), since \(q_u>1\), and \(\xi^5\ge(\log Y)^{-5C_*\log L}\). Thus \(r_n\ge Y^{-1}\) for sufficiently large \(Y\) depending on fixed construction parameters. This conclusion is conditional only on the displayed numerical depth/coupling window and on the source's ordinary admissibility assumptions for the birth being evaluated. CMP119, (2.28) CMP102, Prop. 9 and (190)

For the spatial tail let \(F_{X,z}\) be one such analytic zero-source birth coefficient at its insertion point \(z\in X\) with source norm \(E_0e^{-\kappa d_n(X)}\). Global color invariance and semisimplicity give \(DF_{X,z}(0,0)=0\). In (12), Cauchy for two independent unit sup-norm directions therefore bounds the Hessian by \(C E_0\delta_n^{-2}e^{-\kappa d_n(X)}\), and only first derivatives of \(\mathcal U_n\) enter its physical pullback at zero. At the flat base, (190) bounds each terminal-source tangent in the local fine potential by \(C e^{-c\,{\rm dist}(X,y)}\) in terminal units. The finite current stencil costs at most \(C\xi^{-3}\) and enlarges the distance footprint by a fixed fine-neighbor collar, which changes the constant only. Hence
\[
 |\partial_{b_y}\partial_{b_{y'}} F_{X,z}(\mathcal U_n(b))|_{b=0}
 \le C E_0r_n^{-2}e^{-\kappa d_n(X)}
 e^{-c\,{\rm dist}(X,y)-c\,{\rm dist}(X,y')}. \tag{14}
\]
The notation on the left denotes the absolute value after evaluation at zero. The homogeneous input-cell scale in (190) is one. All estimates use current physical units for \(y,y'\). Non-invariant arbitrary marks in a complex gauge are outside this statement. CMP102, pp. 305–309 CMP109, (1.18)–(1.22)

For clarity allow the larger length \(D_n=C(1+MR_n)\) in the passage from the size functional to the terminal-coordinate diameter. A connected polymer made from the specified localization cubes satisfies \({\rm diam}(X)\le D_n(1+d_n(X))\) by the spanning-tree definition. A bounded number of face-sharing cubes can meet even at a point, accounting for the additive constant. Use a fixed fraction of the diameter and tangent exponents to pay first \(|y-y'|/D_n\) and then \(|z-y|/D_n\), by the triangle inequality. The remaining rooted polymer sum over \(X\ni z\) is finite by the source's entropy reserve. Summing \(z\) costs at most \(C D_n^4\). At a local tagged birth and after its full homogeneous sum this proves, respectively, (14) and
\[
 |\Pi_n(y,y')|\le C E_0 r_n^{-2}D_n^4 e^{-c'|y-y'|/D_n}. \tag{15}
\]
The per-site value on the physical chart is also bounded by the rooted activity norm on summing (2.27), without differentiating the cutoff. In this depth window \(R_n\le L(\log g_n^{-2})^r\), so the prefactor in (15) is at most polynomial in \(Y\) and the decay length at most polylogarithmic. The cubic lattice count and the second-moment weight then cost a further polynomial in \(D_n\) and the truncation radius. The bound holds with periodic distances and passes to the admitted thermodynamic projector. CMP109, (0.24)–(0.26) CMP119, (2.5), (2.26)–(2.28)

The full output uses the actual CMP119 (2.27) primitive analytic norm. Equations (12)–(15) also hold for an independently established pure regular comparator with the same one-scale norm, including one with fixed larger primitive radii by restriction. Comparing a newly defined same-\(g\), no-\(R'\) operation against the full birth requires its own output norm: e.g. check that all its earlier \(E\) inputs are the same fixed-chart germs as those already constructed, and that the actual real cutoff and chart hypotheses of CMP116 hold in its new step. The full output norm by itself says nothing about that modified operation. An all-orders comparison across different post-replacement histories is not proved here. The missing C-03 estimate remains the internal current-coordinate transfer (8)–(9), even if (13)–(15) help a scalar coupling projection.

## 7. A normalized flat output chart uniform in depth

The negative powers of \(\xi\) in (12)–(15) can be removed when both the primitive chart and the terminal minimizer tangent are measured in the source's normalized field coordinates. Keep the homogeneous, flat, unrestricted output and one-scale primitive norm of §6. This statement applies separately to each admissible output birth, regardless of its generation index. The birth may have been produced using inherited \(R'\). At this point its primitive bound is an input from the effective-density theorem.

**Primitive chart.** Put \(U=\exp(i\xi A)\) with flat real reference and take \(J\) independently. On a carrier \(X\) use the maximum of \(\|A\|_\infty,\|\nabla^\xi A\|_\infty,\|J\|_\infty\) on their defined stencils. Then for a fixed \(c>0\),
\[
 \max\{\|A\|_\infty,\|\nabla^\xi A\|_\infty,\|J\|_\infty\}<c h_n
 \quad\Longrightarrow\quad (U,J)\in\mathcal U_n^c(X,\alpha_{0,n},\alpha_{1,n}).
 \tag{16}
\]
Indeed, write \(K_0=\|A\|_\infty,\ K_1=\|\nabla^\xi A\|_\infty\). In an oriented plaquette, the signed sum of the four link potentials before multiplication by \(\xi\) is a finite difference of two parallel link pairs. Its norm is at most \(2\xi K_1\). Expanding the product to first order, the rest is at most \(C\xi^2 K_0^2\) for \(\xi K_0\le1\). Thus \(\|\partial U-1\|_\infty\le C\xi^2(K_1+K_0^2)\). Both the direct relative-potential requirements and the independent-current bound hold with the fixed smaller fraction of \(\alpha_{u,n}\) used in §6. The real reference is flat, and the smaller-space estimate of CMP109 p. 263 supplies the reconstructed requirements. CMP109, (1.11)–(1.16) and following estimates

**Physical current.** At the flat base, in the same coordinates, the source current \(J_\xi(U)=D_U^*\xi^{-2}\pi\,\operatorname{Im}(\partial U)\) satisfies
\[
 \|J_\xi(e^{i\xi A})-D_1^*D_1 A\|_\infty
 \le C(K_0K_1+K_0^3),\qquad \xi K_0\le c_* .
 \tag{17}
\]
Here the subscript 1 denotes the identity background with the source's lattice spacings and projections. One can equivalently use \(D J_\xi(1)[A]\) in (17). The equality of this linear term with the Maxwell difference is the linear part of CMP109 (3.11).

To verify uniformity, for each oriented plaquette use the analytic projected imaginary part \(\psi(P)=\pi(P-P^{-1})/(2i)\). Its expansion in the four signed link logs has a linear term \(\xi^2(d^\xi A)_p\), a quadratic term \(\xi^2 q_p(A)\), and remainder bounded by \(C\xi^3 K_0^3\). In \(q_p\) the coefficient is a fixed homogeneous polynomial in the four adjacent link potentials, including the signs and the order in the plaquette product. For similarly oriented adjacent translates \(p,p'\),
\[
 |q_p(A)-q_{p'}(A)|\le C K_0\xi K_1 .
\]
This follows by subtracting one polynomial argument at a time. In the flat divergence \(D_1^*\), neighboring plaquette contributions occur with opposite signs. Applying it to \(\xi^{-2}\psi(\partial U)\) leaves the Maxwell term, a quadratic correction at most \(CK_0K_1\), and an error at most \(CK_0^3\), since the divergence costs one power of \(\xi^{-1}\). The covariant divergence differs from the flat one by a finite sum of the same translated stencils times \(\xi^{-1}(\operatorname{Ad}_{U(b)}-I)\), or a bounded-length product of such transports according to the base-corner convention. Its operator norm on plaquette arrays is at most \(CK_0\), since \(\|e^{\pm i\xi A}-1\|\le C\xi K_0\). The plaquette array itself has norm at most \(C(K_1+K_0^2)\) by the preceding product estimate. This proves (17) also in the complex chart, with no volume factor or inverse power of \(\xi\). All bounds here apply to the full physical field. No localized walk term was assumed to satisfy a Landau equation. CMP109, (1.8), (3.10)–(3.14)

For the actual flat-base homogeneous minimizer let \(A_n(b)\) denote its Landau representative in \(U_n=\exp(i\xi A_n)\). CMP102 (19), (172)–(175), Proposition 9 gives the analytic bounds for \(A_n,\nabla^\xi A_n,D_1^*D_1 A_n\) on the fixed terminal ball. In the all-small determining geometry the sole layer is \(n\), with \(L^n\xi=1\), so all three output scale factors in (19) equal one. These functions vanish at zero. Radial Schwarz on a fixed smaller terminal ball, or choosing the parameter \(\varepsilon_1\) proportional to \(\|b\|_\infty\) in (172)–(173), bounds the three norms by \(C\|b\|_\infty\). Formula (17) now bounds the *physical* current by \(C'\|b\|_\infty\) independently of \(n\). The localized tangent estimates (190) have both output and input layer scale one in this geometry. At \(b=0\) the nonlinear error in (17) has zero derivative and the current tangent is exactly \(D_1^*D_1 D A_n(0)\). Therefore in all three norms of (16), the joint tangent from a terminal source at \(y\) is bounded on \(X\) by \(C e^{-c\,{\rm dist}(y,X)}\). CMP102, pp. 281, 305–309

Consequently (13)–(15) hold with the improved terminal radius
\[
 \widehat r_n=c h_n
   =c\min\{1,C_0 g_n(\log g_n^{-2})^{q_0},C_1 g_n(\log g_n^{-2})^{q_1}\}.
 \tag{18}
\]
For the local Hessian apply two-direction Cauchy to \((A,J)\mapsto F_{X,z}(\exp(i\xi A),J)\) on (16) in the normalized tangent norms. Its first jet vanishes at zero, so the preceding exponential tangent estimate proves (14) with \(\widehat r_n\). The same rooted sum then proves (15). This terminal estimate holds for the separately supplied primitive output norm and is independent of the age of any absorbed activity. It permits polynomial chart and tail costs in \(g_n^{-1}\) at all depths. The real pressure difference and the existence of a second, matched comparison birth after earlier absorptions are separate questions. In particular (18) makes no estimate for the internal effective exponent at an arbitrary selected fluctuation field.

## 8. Complex marginal transfer for carried physical \(R\) on the homogeneous chart

Consider the homogeneous terminal minimum \(U_k(b)\) of §7, with \(\|b\|_\infty\le Q\le c h_k\). For \(1\le j\le k\) write \(t=L^{j-k}\), \(\xi_j=L^{-j}\), and \(\eta=L^{-k}=t\xi_j\). In the primitive \(j\)-units let
\[
 f_{j,X}(b)=R^{(j)}(X,U_k(b),J_{\xi_j}(U_k(b)))-R^{(j)}(X,1,0),
 \qquad M_{j,X}=g_j^{\kappa_0}e^{-\kappa d_j(X)} .
\]
The current is the actual physical current in the units of the old action. Membership or differentiation of a primitive function below uses its true extended \((U,J)\) domain. The restriction to \(b\) here evaluates the full unlocalized minimizing field and its current. In this section \(X\) is an old source carrier. Denote by \(D_X\ge1\) an upper bound on its intrinsic path diameter in old spatial units and on the diameter of its one-stencil collar. One may take \(D_X=C(1+MR_j)(1+d_j(X))\) by following a tree through its face-connected carrier cubes and joining the endpoints inside the extreme cubes. CMP109, (0.24)–(0.26) CMP119, (2.30)–(2.32)

On the stated physical chart,
\[
 |f_{j,X}(b)|\le C M_{j,X}(1+D_X)^2 t^4 Q^2/h_j^2 . \tag{19}
\]
Its flat source Hessian, for terminal coordinate directions \(y,y'\), obeys the stronger localized estimate
\[
 |\partial_y\partial_{y'}f_{j,X}(0)|
 \le C M_{j,X}(1+D_X)^2 t^4 h_j^{-2}
 \exp[-c\,{\rm dist}_k(X,y)-c\,{\rm dist}_k(X,y')] . \tag{20}
\]
Here \({\rm dist}_k\) uses terminal spatial units. Fixed fine-neighbor enlargements are absorbed in \(C\). These bounds use CMP119 numerical comparability (2.6)–(2.7) for an admitted sequence of couplings.

**Proof of (19).** Write \(U_k=\exp(i\eta A_k)=\exp(i\xi_j A^{[j]})\). Then \(A^{[j]}=t A_k\), its first lattice derivative in old units is \(t^2\nabla^\eta A_k\), and \(J_{\xi_j}=t^3 J_\eta\) directly from the inverse powers in the current and the unchanged group parallel transports. By §7 these three quantities have norms at most \(C tQ,Ct^2Q,Ct^3Q\). The source's coupling and logarithm comparisons give \(h_k/h_j\le C(1+k-j)^{1/2}\), by applying the comparisons to each of the two running radii before taking the minimum with 1. Thus \(tQ\le Cc h_j\) uniformly. The original pair, in the flat charts of (16) at scale \(j\), is admitted with slack for small \(c\).

For a general primitive pair of normalized chart norm \(q\) inside (16), set \(F(A,J)=R^{(j)}(X,\exp(i\xi_j A),J)\). Its value is bounded there by \(M_{j,X}\) and its first joint jet at zero vanishes by constant color invariance and semisimplicity. Along \((\tau A,\tau J)\), the disc \(|\tau|<c_0 h_j/q\) is admitted. The maximum principle after division by \(\tau^2\) gives
\[
 |F(A,J)-F(0,0)|\le 2 M_{j,X}\,(q/(c_0 h_j))^2
\]
on a smaller chart. If \(D_X\ge c_2/t\), the original pair has \(q\le CtQ\le C'(1+D_X)t^2Q\). The radial estimate proves (19) in this case, including any winding support. Choose \(c_2>0\) small below a fixed fraction of the shortest terminal period, which is at least one in terminal lattice units.

For \(D_X<c_2/t\), lift the carrier and its one-stencil collar to one Euclidean coordinate box on the torus; the lift is immediate in infinite volume. Use an anchor \(x_0\) there. With \(a=A^{[j]}\) let \(v_\mu=a_\mu(x_0)\), \(T(x)=\sum_\mu(x_\mu-x_{0,\mu})v_\mu\), \(u(x)=e^{iT(x)}\). Coordinates in this formula are in old spatial units. Potentials of the transformed links \(u(x)U_\mu(x)u(x+\xi_j e_\mu)^{-1}\) have the form
\[
 G_\xi(T,v,a_\mu)=(i\xi)^{-1}\log\!\left(e^{iT}e^{i\xi a_\mu}e^{-i(T+\xi v)}\right),\qquad v=v_\mu,\quad \xi=\xi_j .
\]
This function has a removable singularity at \(\xi=0\), since the argument of the logarithm equals identity there. On fixed small balls for \(T,v,a_\mu\) its analytic derivatives up to second order in these arguments are uniformly bounded for \(0\le\xi\le1\), by the power series or the removable extension and compactness. In particular \(G_\xi(0,v,v)=0,\ G_\xi(T,0,0)=0\), \(\|\partial_{a_\mu}G_\xi\|\le C\), and \(\|\partial_TG_\xi\|\le C(|a_\mu|+|v|)\). This last estimate follows by integrating the mixed derivative in the last two arguments. The chosen lift has \(|T|\le CD_XtQ\le Cc_2 Q\). The gradient bound on \(a\) gives \(|a_\mu(x)-v_\mu|\le C D_Xt^2Q\) by a path in the collar or by the global field in the lifted box. Subtracting first the \(T\) argument and then \(a_\mu-v_\mu\) gives
\[
 \|a^u\|_X\le C D_X t^2(Q+Q^2),\qquad
 \|\nabla^{\xi_j}a^u\|_X\le C t^2(Q+Q^2).
\]
For the second estimate the change in \(T\) across one bond is \(\xi_j v_\nu\) and the change in \(a_\mu\) is at most \(C\xi_j t^2Q\). The transformed current is a pointwise adjoint of the previous current, so its supremum is at most \(Ct^3Q\) since \(\|u^{\pm1}\|\) is bounded. These estimates place the transformed pair in (16) with \(q\le C(1+D_X)t^2 Q\). This is at most a small multiple of \(h_j\) by \(D_X<c_2/t\) and the original choice of \(c\). The transformation is allowed by complex gauge invariance of the primitive activity. Its use here concerns scalar gauge-invariant activities, and involves no deformation of a marked integration cycle. The radial estimate proves (19).

**Proof of (20).** Use the same local gauge as a function of the external source, for the small carriers. Its linearization at zero maps a potential tangent \(\dot a_\mu(x)\) to \(\dot a_\mu(x)-\dot a_\mu(x_0)\). Its current tangent at zero is the original one since the base current vanishes. By (190) the original potential, gradient and current tangents have the three previous scale factors \(t,t^2,t^3\) times \(C e^{-c\,{\rm dist}_k(X,y)}\). Connecting \(x\) to the anchor within the carrier or its one-stencil collar preserves this distance bound up to constants and gives \(\|\dot a^u\|_X\le C D_Xt^2 e^{-c\,{\rm dist}_k(X,y)}\). At large carriers the original \(t\) bound is at most \(C D_Xt^2\), with the same distance tail. Apply two-direction Cauchy on (16) at old radius \(c h_j\) to the two joint tangent vectors. The first jet vanishes, so the Hessian of the physical pullback has no term involving the second derivative of the minimizing or gauge map. This proves (20).

For example, summing (19) per unit terminal volume cancels the \(t^{-4}\) old-site density in four dimensions and gives
\[
 V_k^{-1}\sum_{j,X}|f_{j,X}(b)|
 \le C Q^2\sum_{j\le k}(1+MR_j)^2g_j^{\kappa_0}h_j^{-2}
 \le C_\epsilon Q^2 g_k^{\kappa_0-8-\epsilon},\qquad \kappa_0>8+\epsilon .
 \tag{21}
\]
The first inequality overcounts by rooting each carrier at an old site and uses the remaining rooted exponential after its fixed support polynomial. The last uses \(h_j\ge c g_j\), \(R_j\le L(\log g_j^{-2})^r\), and the same six-power trajectory sum as Annex G (4.5). In particular this is a complex marginal bound for the specified physical pullback, retaining the original four-power compensation.

For the spatial projection in (20) set \(B_{j,k}=1+t MR_j\) and \(B_k=C(1+MR_k)\). By (2.9), \(B_{j,k}\le B_k\): the polynomial age growth of \(R_j/R_k\) is bounded after multiplication by \(L^{-(k-j)}\). The terminal diameter of \(X\) is at most \(C B_{j,k}(1+d_j(X))\). Reserve fixed fractions of the carrier and tangent exponents to pay \(|y-y'|/B_{j,k}\) and \(|z-y|/B_{j,k}\) for an old root \(z\in X\). Summing roots costs \(C(B_{j,k}/t)^4\) at old spacing \(t\), canceling the \(t^4\) in (20). The remaining rooted carrier sum is finite as above. Thus for the carried physical Hessian \(\Pi^R_k\),
\[
 |\Pi^R_k(y,y')|\le C_\epsilon B_k^4
    g_k^{\kappa_0-8-\epsilon} e^{-c|y-y'|/B_k},\qquad
 \sum_{y'} |y-y'|^2 |\Pi^R_k(y,y')|
 \le C_\epsilon B_k^{10} g_k^{\kappa_0-8-\epsilon}. \tag{22}
\]
The second sum is in four terminal dimensions. The inequalities also bound an eligible subsum over old birth indices or carriers. No translation invariance of an individual carrier is needed.

**Scope.** These are actual estimates for the carried physical \(R\) restricted to the flat homogeneous output chart on an admitted trajectory. They also apply to its flat curvature projection. They do not estimate the new effective birth produced by integrating the \(R\) fluctuation difference on a selected real fiber. The mixed local decoupling propagators in C-03 are absent from \(U_k(b)\), and the affine gauge was applied to the full homogeneous minimizing field. At a selected nonflat center, a single gauge frame with the tangent differences used in (20) has not been constructed. The full internal carrier and denominator transfer tests (8)–(9) stay open.

### 8.1 Higher physical-amplitude jets and relation to the regular-domain tests

Estimate (19) holds on a full complex terminal ball of common radius \(Q_*=c h_k\), independently of the old index, although its coefficient contains the *old* second-radius price \(h_j^{-2}\). Let \(b_0\) be any point with \(\|b_0\|_\infty\le Q_*/2\), real or complex. In normalized external directions \(b=b_0+g_k z\), apply Cauchy *before* the old sum to (19) on simultaneous \(m\)-direction polydiscs, with each scalar radius \(Q_*/(2mg_k)\). The sum (21) then gives
\[
 V_k^{-1}\sum_{j,X}
 \bigl\|D_z^m f_{j,X}(b_0+g_k z)|_{z=0}\bigr\|
 \le C_\epsilon Q_*^2 g_k^{\kappa_0-8-\epsilon}
 m!\left(\frac{2e g_k}{Q_*}\right)^m . \tag{23}
\]
Here the norm is the multilinear sup over \(m\) terminal directions of sup norm at most one. The derivative notation means the derivative of the composed map in \(z\). Cauchy costs \(m^m\le e^m m!\) and an external radius independent of the age inside that cost. Thus the same \(\kappa_0>8+\epsilon\) suffices for every order in (23). This is a volume-normalized external-amplitude assertion; it gives no separate spatial tree bound at order \(m>2\).

Annex Z distinguishes its anisotropic contour test (EC.3), nonlinear map term (EC.20) and all-order obstruction (EC.32)–(EC.34). In (23) the old-cell count and old chart factor have been paid at order two *before* external high derivatives. In (19), (21), (23) differentiation uses the full physical composition on a proved chart; at nonzero \(b_0\) no nonlinear chain-rule term was discarded. The spatially localized estimate (20) is at the flat point, where the first jet vanishes. Annex AA's (C3.1) already identifies the zero-free primitive normalizer; (5) of this note is an input with that provenance. Its (C3.4) still needs the joint independent-current localization on every point of the regular marginal's product support. The resummed-object derivative in (23) and the fresh-fiber comparison (4) do not verify that condition. Annex AB's scalar collar identity (CM.30) and Annex AC's normalized-history results keep the conditional incoming mark and its retained responses. None of these arguments replaces that mark by a fresh Gaussian observable.

## 9. A connected carrier expansion with independent current at a flat retained field

Fix a homogeneous all-regular determining geometry, retained links equal to identity, an admitted trajectory and one old primitive \(R^{(j)}(X;U,J)\) from (2.30)–(2.31) of CMP119. The free \(k\)-scale fluctuation coordinates are \(z=B\) of CMP116 (1.19). Define \(Q=g_k\|z\|_\infty\), and let \(0\le Q\le Q_* = c h_k\) with \(c\) sufficiently small and fixed. An old carrier absent for this geometry contributes zero. For the present carriers there is a connected local representation of the *actual* vacuum-subtracted pullback whose simultaneous contour includes these free coordinates and auxiliary complex localization parameters for an independent current. The following construction uses a choice of interpolation of the physical pullback. It does not identify its individual summands with those of an already prescribed interpolation.

### 9.1 The extended current

Use terminal spatial units with underlying mesh \(\eta=L^{-k}\). In these units the only layer weight \(L^k\eta\) equals one. Write \(\mathcal Q\) for the flat linear coarse average and \(G_0\) for the unconstrained inverse of the augmented flat quadratic operator. Write \(H_0=G_0\mathcal Q^*(\mathcal QG_0\mathcal Q^*)^{-1}\) and \(\mathcal G=G_0-H_0\mathcal QG_0\) for the constrained inverse. At the flat reference the linearizing \(H\) equals \(H_0\). Indeed, the corrections to the quadratic operators in CMP99 (3.120), (3.136) are proportional to the background current, which is zero, and (3.126) then agrees with CMP102 (129). Here and below fixed one-step normalization factors can be included in the coarse average. All formulas use the same terminal normalization. CMP99, pp. 420–423, (3.120)–(3.138) CMP102, pp. 297–300, (129)–(143)

Choose a connected seed \(X_0\) of terminal \(M\)-blocks covering the scaled \(X\) and its required finite fine-stencil collar. All \(M\)-blocks outside the seed carry masks \(s_\Delta\). Apply CMP116 (1.2)–(1.21) to the fixed flat propagators \(H,H_0,\mathcal G\), with this seed as in its discussion of (1.30). In the notation \(B'=\theta(z)=g_k C z-hD(g_k C z)\), the result has the exact form
\[
 A'_s=H_{0,s}\theta-\mathcal G_s V'_s(A'_s),\qquad
 A_s=A'_s-H_sD_s(A'_s).                                             \tag{24}
\]
The letters \(V'_s,D_s\) denote precisely the derivative of the transformed interaction and the solution of the linearizing equation with the source's masked \(H_s\), respectively. The local input \(\theta\) obeys \(\|\theta\|\le C Q\). For every fixed allowed \(\kappa_1\), on \(\max|s_\Delta|\le e^{\kappa_1}\) the functions in (24) are holomorphic in \(s,z\). Equations (1.14)–(1.21) and CMP102 Proposition 4 give
\[
 \|A'_s\|+\|A_s\|+\|\nabla^\eta A_s\|\le C Q,\qquad
 \|D_s(A'_s)\|+\|V'_s(A'_s)\|\le C Q^2.
\]
The constants here may depend on \(\kappa_1\); \(c\) is chosen after it. The source proves that at masks supported in selected components, the functions needed from (24) on each component depend only on that component, allowing a fixed collar for local operations. CMP116, pp. 2–9, (1.2)–(1.21), (1.30) CMP102, (97)–(98)

Let \(P=1-R\) be the scalar projection in CMP99 (3.21), \(K=DPD^*\), and let \(T=\Delta-K=D^*D+DRD^*\), with flat lattice covariant differences. Three fixed operators now suffice, \(T H_0,T\mathcal G,T H\). For each, denoted by \(S\), the terminal **unit cell** restrictions satisfy
\[
 \|\mathbf1_u S\mathbf1_v\|_{\infty\to\infty}
       \le C e^{-a\,{\rm dist}(u,v)},\qquad a>0 .                    \tag{25}
\]
To verify this, CMP99 (3.49) gives \(K\) an exponentially bounded kernel in the normalized fine counting measure. Each terminal cell has uniformly bounded normalized volume. CMP99 Theorems 3.1, 3.3, in particular (3.42), bound \(G_0,\Delta G_0\) from a unit-cell-supported bounded source into any terminal cell with exponential decay. Here \(G_0\) is the regular inverse in Theorem 3.3, to which (3.42) applies. CMP102 (130) gives the corresponding bounds for \(\Delta H_0\), and the undifferentiated bound follows from (3.133) of CMP99. The flat \(\mathcal Q\) has a fixed terminal-cell stencil and bounded normalized sup norm, by the linear block average along paths of terminal size one. Substitution into \(T\mathcal G=T G_0-(T H_0)\mathcal QG_0\) proves (25), since convolution of finitely many unit-cell exponentials is bounded by another exponential with a smaller exponent. This calculation neither estimates \(\Delta\) on arbitrary bounded fields nor applies the exceptional Laplacian clause for the perturbed Green operators of CMP99 Theorem 3.12. CMP99, pp. 397–399, (3.42)–(3.49), and p. 423 CMP102, pp. 297–299

For each ordered pair of terminal unit cells choose a shortest periodic Manhattan path of terminal \(M\)-blocks from their containing blocks, including the endpoints. Mask the cell matrix of each fixed \(S\) by multiplying \(\mathbf1_u S\mathbf1_v\) by the product of masks on that path outside \(X_0\), each included once. Write the resulting operator as \([S]_s\). The number of masks is at most \(c_d(1+{\rm dist}(u,v)/M)\). For \(M\ge 2c_d\kappa_1/a\), (25) bounds each masked cell norm by \(C e^{c_d\kappa_1}e^{-a\,{\rm dist}(u,v)/2}\). Summation gives a uniform sup norm, on all finite periodic boxes, for all three operators. The rule is applied to the *differentiated* cell kernels themselves. No lattice difference is taken across a mask. Define
\[
 \mathcal J_s=[T H_0]_s\theta
      -[T\mathcal G]_s V'_s(A'_s)-[T H]_sD_s(A'_s)+F_\eta(A_s),
 \qquad F_\eta(A)=J_\eta(e^{i\eta A})-D^*D A.                        \tag{26}
\]
The nonlinear term is a local stencil and (17) bounds it by \(C(Q^2+Q^3)\) on the whole mask domain. Thus \(\|\mathcal J_s\|\le C Q\) jointly in the two sets of variables. At \(s=1\) the first three terms sum to \(T A_1\) by (24), while the Landau condition \(RD^* A_1=0\) gives \(T A_1=D^*D A_1\). Consequently (26) equals the physical current exactly at \(s=1\). At other masks it is an independently constructed primitive current on the same complex chart. For masks zero outside a union of active components, the paths used by every nonzero \([S]_s\) stay in one component. The component separation of (24) therefore also holds for (26) on the seed, including the endpoints' local \(\theta\) stencil. A fixed terminal-unit collar of the active set suffices for the free-variable dependence.

### 9.2 Local coefficients and the native-coordinate derivative bound

In old units substitute \(a=t A_s\), \(\nabla a=t^2\nabla A_s\), \(J=t^3\mathcal J_s\), \(t=L^{j-k}\), into the actual primitive. With the vacuum value subtracted, call this function \(f_{jX}(s,z)\). The proof of (19) uses only the three joint component bounds and the independent primitive chart. In particular the patch gauge acts on the supplied \(J\) by its pointwise adjoint and requires no field equation there. Thus, for *all* the above complex \(s,z\),
\[
 |f_{jX}(s,z)|\le C g_j^{\kappa_0}e^{-\kappa d_j(X)}
                    (1+D_X)^2 t^4 Q_*^2/h_j^2.                       \tag{27}
\]
This is a bound for each old carrier including its marginal gain. The finite-volume fundamental theorem of calculus on the mask cube represents \(f_{jX}(1,z)\) as the sum over subsets \(S\) of the integrals over \([0,1]^S\) of \(\partial_S f_{jX}(s_S,0,z)\). Every derivative from a component detached from \(X_0\) vanishes by the preceding component argument. The resulting coefficient depends on \(z\) only in \(Y^+\), the fixed collar of the connected block union \(Y=X_0\cup S\). With \(m=|S|\) and \(\lambda_s=\log((e^{\kappa_1}-1)/2)>0\), Cauchy gives the additional factor \(e^{-\lambda_s m}\) in (27). The factor 2 leaves strict room around the entire real parameter interval. The sum reproduces the physical pullback at \(s=1\).

Here are sufficient entropy margins for the weighted sum. Write \(n=1+d_j(X)\). The ordinary \(d_j\) in the separated \(R\) estimate is in units of \(M\), including if a prior expansion used bigger cubes. LFR II explicitly passes to this size in (1.100). A traversal of a shortest tree of length \(M d_j\) can be covered by at most \(C n\) balls of radius \(M\), each meeting a bounded number of old \(M\)-cubes. Thus \(X\) contains at most \(C_d n\) old cubes. After scaling, the terminal \(M\)-blocks meeting them and a fixed stencil collar admit a connected cover of at most \(C_0 n\) blocks. One may use \(D_X\le C M n\) in (27) in this ordinary-size count. A connected collection of \(v\) blocks containing an anchor has at most \((2d)^{2v}\) choices by depth-first traversal of a spanning tree. Consequently the number of old \(X\) containing a given old root with \(p\le d_j(X)<p+1\) is at most \(C\exp(b_0(p+1))\) for a fixed \(b_0\), and the number of admissible \(S\) of size \(m\) for fixed \(X\) is at most \(\exp(b_1(C_0 n+m))\), \(b_1=2\log(2d)\), up to a constant. CMP109, pp. 256–258, (0.24)–(0.26) LFR II, p. 390, (1.98)–(1.100)

Choose \(M,\kappa,\kappa_1\) with the preceding kernel margin and, for example,
\(\lambda_s>b_1+4,\ \kappa>b_0+C_0(b_1+4)+4\).
These are sufficient inequalities on the construction constants for the next norm statement. For fixed terminal coordinate \(i\in Y^+\) and old root \(w\in X\), both \({\rm dist}(i,w)\) and \({\rm diam}(Y^+)\) are bounded by \(C_d M(C_0 n+m+1)\). Also \(|Y^+|\le C_M(C_0 n+m+1)\) when counting terminal free coordinates. Choose \(\gamma>0\) with \(2C_d M\gamma<1\). The amount \(e^{C_0 n+m+1}\) pays the two factors \(e^{\gamma {\rm diam}(Y^+)}e^{\gamma{\rm dist}(i,w)}\); another exponential of that size pays the fixed polynomial counts. Root the old carrier at any deterministic old site \(w\in X\) and overcount by all old sites at spacing \(t\). Their residual spatial sum \(\sum_w e^{-\gamma{\rm dist}(i,w)}\le C_\gamma t^{-4}\) cancels the \(t^4\) in (27). Applying the preceding two animal counts, then the old exponent sum of (21), gives the bound for the individual local summands \(F_{jXS}\) just constructed,
\[
 \sup_i\sum_{j,X,S:i\in Y^+}|Y^+| e^{\gamma{\rm diam}(Y^+)}
    \sup_{g_k\|z\|\le Q_*}|F_{jXS}(z)|
 \le C Q_*^2\sum_{j\le k}g_j^{\kappa_0}h_j^{-2}
 \le C_\epsilon Q_*^2 g_k^{\kappa_0-8-\epsilon}.
                                                                        \tag{28}
\]
Constants depend on the fixed choices, not on depth or volume. Restrict to \(g_k\|z_0\|\le Q_*/2\). The native chart has radius \(Q_*/(2g_k)\) there. Cauchy on the sum of \(p\) independent unit directions uses individual radii \(Q_*/(2p g_k)\). In the norm on the left of (28), the sum of the \(p\)-linear derivative norms is therefore bounded by the right side times \(p!(2e g_k/Q_*)^p\). In particular the row sum over two native-coordinate derivatives is bounded by
\[
 \sup_i\sum_l e^{\gamma {\rm dist}(i,l)}
     \sum_{j,X,S}\sup_{g_k\|z_0\|\le Q_*/2}
                    |\partial_i\partial_l F_{jXS}(z_0)|
 \le C_\epsilon g_k^{\kappa_0-6-\epsilon},
 \qquad \kappa_0>8+\epsilon.                                           \tag{29}
\]
Indeed only \(i,l\in Y^+\) contribute, and (28) has already paid the \(l\) count. An eligible subset of primitive birth indices/carriers obeys the same bound.

**Boundary of this result.** Equation (29) treats inherited, vacuum-subtracted \(R\) on the central free-coordinate window of the identity-retained, homogeneous regular fiber. All previous selectors that generated a primitive are included in its certified \((U,J)\) norm. Equation (26) keeps its coefficients fixed at the flat retained background. If the retained field varies, a matrix block \(\mathbf1_u T H_0(U)\mathbf1_v\), for example, can depend on \(U\) in blocks outside the selected path. A support proof then needs localized dependence of these differentiated kernels on *the retained field*, together with preparation maps satisfying the joint chart bounds at every point of the actual product. The argument above also has no comparison between the full cutoff radius and the central radius \(Q_*/2\), and does not treat a newly integrated birth or an arbitrary incoming mark. Annex AA (C3.4), Annex Z (EC.3), and the selected conditional-law requirements remain open.

### 9.3 Fixed flat torus holonomies and the cutoff comparison

The native-coordinate Hessian bound (29) also holds for a fixed homogeneous real flat background on a periodic torus with commuting toral holonomies. Take periods sufficiently large that the \(O(LM)\) regularity-test cubes are contractible. Use constant fine links \(\bar U_\mu=\exp(i\eta C_\mu)\), where the \(C_\mu\) commute and can be chosen bounded in terminal units by a group-dependent constant (choose bounded logarithms of the holonomies and divide by the corresponding periods). Take the corresponding retained averages and a source-admitted branch. This field has zero Wilson action and meets its coarse constraints by construction, so is a minimizing representative. Real periodic changes of frame give the same conclusions with the correspondingly transported free-bond charts. The retained holonomies are held fixed in all derivatives.

Indeed, covariantize (24)–(26) with this flat real connection. Its curvature and current vanish. The Hessian of the Wilson action is the flat covariant Maxwell operator, as one sees by a local parallel trivialization of each plaquette. The current-dependent differences between \(H,H_0\) vanish as above. The covariant Hodge identity \(D^*D+DD^*=\Delta_{\bar U}\) follows by trivializing the local stencil; transition functions between parallel frames are constant. Thus \(T=\Delta_{\bar U}-D P_{\bar U}D^*\) and the primary kernel bounds used in (25) hold by the same background-uniform theorems. The flat real connection transports isometrically. The covariant form of (17) on each local stencil follows by the same parallel trivialization, with its explicit constant unchanged. The source's background-covariant estimates for (24) bound \(A_s,\nabla_{\bar U} A_s,\mathcal J_s\) by \(CQ_*\), and \(s=1\) again gives the physical current. Components of the independently masked kernels still separate because the retained connection is fixed.

For an old carrier with \(D_X<c_2/t\), a lift and its required collar sit in a single nonwinding box. In a parallel frame the background is exactly identity on that box. Primitive gauge invariance, (27), and the original vacuum subtraction therefore apply verbatim. For \(D_X\ge c_2/t\) retain only the absolute primitive estimate \(2 g_j^{\kappa_0}e^{-\kappa d_j(X)}\). To see its domain, use \(\bar U\) as the real reference. On local test cubes it has a parallel frame, and the perturbing old potential and its covariant gradient are \(O(tQ_*)\) and \(O(t^2 Q_*)\). In the displayed constant-connection gauge its ordinary gradient also costs at most \(Ct^2 Q_*\), since the old connection coefficients are \(t C_\mu\). The perturbed plaquette estimate follows in a local frame and the independent current is \(O(t^3Q_*)\). The same smaller-parameter argument following CMP109 (1.16) verifies the primitive chart, with \(tQ_*\le c' h_j\) by §8. No vanishing first variation at a winding holonomy was used.

On this large-carrier branch \(t^{-4}\le C D_X^4\le C_M(1+d_j(X))^4\), so even this crude primitive estimate pays the old-site density from the remaining carrier polynomial margin in (28). Cauchy and the old sum give its additional Hessian contribution bounded by
\[
 C_\epsilon (g_k/Q_*)^2\sum_{j\le k}g_j^{\kappa_0}
 \le C_\epsilon g_k^{\kappa_0-6-\epsilon},
\]
using \(Q_*=c h_k\ge c' g_k\). This proves (29) with the same weak-coupling exponent for these fixed flat holonomies. The scalar estimate for winding terms before taking derivatives has an additional \(C\sum_j g_j^{\kappa_0}\). It need not vanish at zero free fluctuation, since a winding activity can detect a flat holonomy.

Finally let \(r_k\) be the product radius of Annex AA (C7.3) in its **native free coordinate**. In any of the flat subfamilies above the verified sufficient condition for (29) on the entire product is
\[
                         g_k r_k \le c h_k/2.                          \tag{30}
\]
Fixed bond norm equivalence factors are included in \(c\). In CMP119 the scaled variable is introduced before (3.15); (3.16) prints the threshold \(\delta_k= C g_k(\log g_k^{-2})^{p_0}\). If \(r_k=\delta_k\) literally for the scaled coordinate, then \(g_k\delta_k/h_k\le C' g_k(\log g_k^{-2})^{p_0}\to0\), so (30) holds. Under the alternative normalization \(g_k r_k=\delta_k\), a sufficient condition is \(\min(q_0,q_1)>p_0\) (or equality with sufficient coefficient slack), using (2.28). The explicit statement at CMP119 (2.28) gives \(q_u>1\) and sufficiently large coefficients. Annex AA flags the convention issue before (C7.1); the full-support conclusion here is expressed by (30) without selecting a new source threshold. Other curved data require an additional chart condition. Section 9.4 treats one such condition. Neither cutoff convention supplies a bound on summation over preparations. CMP119, pp. 259, 264, 267–268, (2.28), (3.15)–(3.16) 

### 9.4 Recentring an actual curved coarse input at the identity

There is a further extension when the *actual prepared coarse field* at the fluctuation input is small in a common representative. On the homogeneous determining geometry write that field as \(V^{(k)}=\exp(iv)\) on terminal bonds. Here \(v\) is the input to the scale-\(k\) fine minimizer, as it occurs in CMP119 (3.15); it can have nonzero plaquette curvature. In the chosen frame assume
\[
               \|v\|_\infty+g_k\|z\|_\infty \le c' h_k.              \tag{31}
\]
We first allow \(v\) to be an independent complex terminal-bond variable for estimating the pullback, and subsequently evaluate it at its actual prepared value. On this combined chart the inherited contribution admits a connected expansion as in (27)–(29). Its coordinate dependence is local jointly in \(v,z\), with a fixed \(L\)-scale collar. In particular the same estimate (29) holds with the supremum over a smaller instance of (31), and for mixed derivatives with respect to \(z\) and \(v/g_k\).

To prove this, use the source's exact current coarse field entering the minimizing map,
\[
       e^{i b(v,z)}=\exp(i\theta_v(z))\,e^{iv},
       \qquad
       \theta_v(z)=g_k C_v z-h_vD_v(g_k C_v z).                      \tag{32}
\]
The operators \(C_v,h_v\) here are the one-step exceptional-bond eliminations of CMP109, pp. 267–268. Their coefficients at a given bond depend on \(e^{iv}\) in the two adjacent \(L\)-blocks and their fixed paths. At \(v=0\) the matrix inverted by \(h_v\) is nonsingular. In a fixed smaller complex neighborhood it has a uniformly bounded analytic inverse by the Neumann series. All other operations in this change of variable are finite-dimensional analytic products, averages and local logarithms on these blocks of fixed side \(L\). The implicit equation \(D=C_{\rm nl}(B-hD)\) after (2.10) has \(C_{\rm nl}\) starting at second order with uniformly bounded local analytic norm. The excluded bonds belong to distinct inter-block corridors, with one distinguished bond for each coarse constraint. Paths in one constraint cross only its own corridor, so its implicit equation does not introduce new corridors. Equivalently, CMP116, pp. 3–4 calls \(B'\) a local function and (1.19)–(1.20) supplies its uniform bound. The implicit function theorem and boundedness on the fixed small chart therefore give \(\|\theta_v(z)\|\le Cg_k\|z\|\) with uniform holomorphy and a fixed localization collar in both inputs. The principal logarithm in (32) is local on each bond and has derivative bounded in that neighborhood. Hence \(\|b(v,z)\|\le C(\|v\|+g_k\|z\|)\). CMP109, pp. 266–268, (2.4), (2.10)–(2.12) CMP116, pp. 3–7, (1.19)–(1.21) CMP119, pp. 267–268, (3.15)

Use \(b(v,z)\) in place of \(\theta\) in (24), (26). This is legitimate because CMP116 obtains (1.17)–(1.18) with \(B'\) an independent input *before* (1.19) substitutes the fluctuation map. At unit masks the resulting field is the minimizing orbit with the exact coarse data on the left of (32). One can evaluate the gauge-invariant old primitive in this chart by uniqueness of the regular minimizing orbit at real small data, followed by analytic continuation on the common ball. In particular this step involves the nonlinear map of the **entire** coarse input; it does not add field perturbations from two separately minimized configurations. All interpolated operators again have the identity reference, so (25) continues to hold with no \(v\)-dependent distant coefficients. The component proof and (27) hold for \(Q\) replaced by \(C(\|v\|+g_k\|z\|)\), upon decreasing \(c'\). The old-site compensation and (28) are uniform on this same chart. Shrink (31) by a factor of two and apply Cauchy to \(z\) and to \(w\) in \(v=v_0+g_k w\); the available radius in either normalized variable is \(c'h_k/(2g_k)\) prior to dividing it among the directions. Since the additional coarse coordinates per block are bounded, (29) follows also for the combined row norm, with adjusted fixed constants. The actual incoming fluctuation difference subtracts the evaluation at \(z=0\) in (32). This contributes zero to derivatives containing a free \(z\)-index and at most a second copy of (28) to the value and retained-coordinate estimates.

Condition (31) concerns an identified source argument. A fixed real prepared \(V^{(k)}\) satisfying it can be substituted without differentiating its construction, giving free-coordinate estimates on this nonflat subfamily. An outgoing coordinate \(W\) enters through \(V^{(k)}=M^k(U_{k+1}(W))\) on the ordinary homogeneous branch. Locality proved here in \(v\) does not by itself yield locality or a uniform derivative bound in \(W\). For a retained derivative the concrete terms still to estimate are the compositions with \(D_W v\) and \(D_W^2v\), including \(D_v F\,D_W^2 v\) away from the joint vacuum. The outer-field-dependent preparations in a selected large-field geometry introduce additional such maps. Neither (31) nor the small-center estimates have been verified for all those data.

### 9.5 Free derivatives at an actual small real outgoing field

For fixed *real* outgoing \(W=\exp(iw)\) in the homogeneous branch, the free-derivative conclusion of §9.4 applies uniformly under the explicit outgoing-coordinate condition
\[
                    \|w\|_\infty+g_k\|z\|_\infty\le c'' h_k.          \tag{33}
\]
This statement concerns the ordinary real source coupling and all fixed branches for which the homogeneous minimizer exists, including curved \(W\). It uses no derivative of a gauge selected as a function of \(W\).

In units of the \(k+1\) terminal spacing let \(\eta=L^{-(k+1)}\). By CMP102 Proposition 9 at the identity the minimizing orbit has a real Landau representative \(\widetilde U=\exp(i\eta A)\) with \(\|A\|+\|\nabla^\eta A\|\le C\|w\|\). Put \(\alpha=C'\|w\|\). The plaquettes of \(\widetilde U\) then obey the bound \(C\alpha\eta^2\). The intermediate averaged fields have plaquette defects at most \(C\alpha (L^\ell\eta)^2\) at levels \(0\le\ell\le k\), by the intermediate-average estimate used following CMP109 (1.16). Its local-potential and first-derivative hypotheses hold here in the given global representative. To bound the averaged *links* themselves let \(b_\ell\) be their maximum bi-invariant real-group distance to identity. Initially \(b_0\le C\eta\|w\|\). For a single averaging step (0.4), the average link equals the straight \(L\)-link product times an exponential of a convexly weighted average of loop logarithms. Each comparison loop lies in the two adjacent \(L\)-blocks; it can be filled by at most \(C_L\) elementary plaquettes. The exact plaquette-product identity and invariance of the distance under real conjugation bound its distance to identity by \(C_L\alpha(L^\ell\eta)^2\). On the resulting small ball the logarithm is bounded by a fixed multiple of this distance. For prescription (0.12) the averaged paths at the endpoints differ from any one such path by the same bound, by (0.5)–(0.8) and local analyticity for the fixed one-step collection. The same estimate follows. Consequently
\[
 b_{\ell+1}\le L b_\ell+C_L\alpha(L^\ell\eta)^2,\qquad
 b_k\le L^k b_0+
 C_L\alpha\sum_{\ell=0}^{k-1}L^{k-1-\ell}(L^\ell\eta)^2
 \le C'_L\|w\| .                                                       \tag{34}
\]
The fixed-size loop fillings used here are in the periodic lift, and project to identities of link products on the torus. CMP109, pp. 253–254, 263, (0.4)–(0.12) and text after (1.16) CMP102, Proposition 9

The actual coarse center is \(V^{(k)}=M^k(U_{k+1}^{\rm ax}(W))\) by CMP109 (2.3). Gauge covariance at block endpoints of (0.4) or (0.12), iterated \(k\) times, identifies it with \(M^k(\widetilde U)\) up to a real coarse gauge. Thus one representative of the actual center has a global link logarithm bounded by (34). At this fixed \(W\), transformation of the relative free-bond charts is by the pointwise real adjoints in (2.16). This can also be seen directly from (32): simultaneous transformation of the total coarse links and the reference sends their relative link logarithm at \(b\) to its left-endpoint adjoint, and constraint elimination is equivariant by uniqueness. These maps are isometries of the invariant Lie-block norms and preserve the coordinate support, including the eliminated-bond set. The bounds (28)–(29) for the free variables in the representative of (34) therefore transfer to the actual free coordinates at \(W\), allowing fixed Lie-norm equivalences as before. The underlying old activities are gauge invariant. This proves (33) and, when (30) has adequate slack for \(\|w\|\), its entire-product version. Estimating retained derivatives in a \(W\)-dependent representative would also require estimates on the derivatives of the intervening chart and compact gauge. CMP109, pp. 265–268, (2.3), (2.16)

## 10. The summable independent-current and higher primitive jets of \(E\)

On the homogeneous charts in §§9.1–9.2, 9.4 fix an actual rooted \(E^{(j)}(X;U,J,x)\) with primitive bound \(M^E_{jX}=E_0 e^{-\kappa d_j(X)}\) of CMP119 (2.26)–(2.28). The same conclusions for free derivatives hold at real outgoing data in (33). The following is an exact splitting of this primitive after chart admission. The original vacuum and Wilson coupling subtractions of (2.25) keep their source values. In particular the splitting does not prescribe a new beta coefficient. CMP119, pp. 258–260, (2.25)–(2.29)

Use the affine chart on \(X\) from §8 for \(D_X<c_2/t\), and use the original admitted chart otherwise. Denote the resulting potential and independent current by \(a^u,I^u\), using \(u=1\) in the latter case. With \(\|\cdot\|_1\) the maximum of the sup potential and old normalized first difference, the joint bounds on the whole complex mask domain are
\[
     \|a^u\|_1\le C(1+D_X)t^2 Q_*,
       \qquad \|I^u\|\le C t^3 Q_*,
       \qquad q:=\max(\|a^u\|_1,\|I^u\|)\le c_0h_j/2.               \tag{35}
\]
The last estimate uses the actual \(CtQ_*\) bound at large carriers instead of the diameter upper bound. Define the scalar primitive in its analytic chart by \(e(a,I)=E^{(j)}(X;\exp(i\xi_j a),I,x)\). Its first joint jet vanishes by constant color invariance and semisimplicity. Write
\[
 e(a^u,I^u)-e(0,0)=P_{AA}(a^u,a^u)+N_{jX},\qquad
 P_{AA}(a,a)=\tfrac12D_A^2 e(0,0)[a,a].                            \tag{36}
\]
Here \(N_{jX}\) contains the mixed \(A,J\) and pure \(J,J\) quadratic jets and the entire joint Taylor remainder of degree at least three. Boundedness on the primitive ball (16), by one-dimensional radial Cauchy and geometric summation of degrees \(\ge3\), bounds that remainder by \(C M^E_{jX}(q/h_j)^3\). Two-direction Cauchy bounds the two other contributions by \(C M^E_{jX}h_j^{-2}(\|a^u\|_1\|I^u\|+\|I^u\|^2)\). In particular
\[
 |N_{jX}|\le C M^E_{jX}
 \left[(1+D_X)^3 t^6 Q_*^3 h_j^{-3}
       +(1+D_X)^2 t^5 Q_*^2 h_j^{-2}\right].                        \tag{37}
\]
The local gauge is itself analytic on the mask domain; it is computed from \(A_s\) and its anchor on the seed, and creates no distant free-variable dependence. Thus \(N_{jX}\) has the connected mask expansion in §9.2 with an extra \(e^{-\lambda_s |S|}\) per coefficient. All diameter factors in (37) are paid by the same exponential margin there, with fixed constants for the new polynomial degrees.

After the \(t^{-4}\) old-root count, the cubic sector retains \(t^2\), and each quadratic term containing the extended current retains at least \(t\). Write \(a_0=k-j\) for the age to avoid confusion with the potential. Using \(h_k/h_j\le C(1+a_0)^{1/2}\) from §8, the sum of the weighted native-coordinate value norms in (28), now for the local summands of \(N_{jX}\), is bounded by
\[
 C E_0\sum_{a_0\ge0}
 \left[L^{-2a_0}(1+a_0)^{3/2}(Q_*/h_k)^3
        +L^{-a_0}(1+a_0)(Q_*/h_k)^2\right]
 \le C' E_0(Q_*/h_k)^2.                                              \tag{38}
\]
In (2.26)–(2.27) the root \(x\in X\) may be part of the index; counting the remaining possibilities at a fixed old anchor costs at most a fixed polynomial in \(1+d_j(X)\), which is included in (38). Cauchy on the combined chart proves the weighted native Hessian bound \(C E_0(g_k/h_k)^2\), tending to zero at least as \(C'E_0(\log g_k^{-2})^{-2\min(q_0,q_1)}\). It also gives all fixed-order localized native derivative norms with the right side of (38) times \(p!(C g_k/Q_*)^p\). In particular, this bound on all the nonlinear primitive jets and all jets involving the independent current needs no age loss per differentiation. All derivatives act on the composed activity, and so include the Hessian of the nonlinear chart.

The unresolved homogeneous part of \(E\) after (36) is the sum of \(P_{AA}(a^u,a^u)\) on its actual nonlinear arguments, together with the true field-dependent Wilson subtraction. Its naive bound has \(t^4\) and loses all four powers in the old-root count, leaving \(C E_0 Q_*^2\sum_{j\le k}h_j^{-2}\). A uniform Hessian budget cannot follow from this majorant. Cancellation or additional spatial regularity in this specific quadratic sector is required. CMP109 §§4–5 analyzes the vacuum polarization and matches the source coupling through its Ward identities; using that cancellation on the actual localized composed functions requires its own quantitative estimate. Selected nonhomogeneous geometries have the further preparation and support requirements described above.

### 10.1 Localization of the remaining pure-potential bilinear to the curvature

Fix \(0<\beta<1/2\) in the admissible first-gradient Hölder norms of the homogeneous flat propagators. CMP116 (1.11), (1.16)–(1.18) preserves these norms for \(A_s\); the source uses them explicitly for second differences in CMP109 (3.32), (4.16)–(4.18). Thus \([\nabla^\eta A_s]_{\beta,{\rm loc}}\le C Q_*\) on fixed terminal unit cells and their fixed enlargements. Together with the sup norm this controls differences between more distant cells in the homogeneous geometry. In old units \(a=t A_s\) has \([\nabla^{\xi_j}a]_\beta\le C t^{2+\beta}Q_*\). Let the anchor \(x_0\) now be the old root \(x\) of (2.27), for all carriers meeting that root. CMP109, pp. 275–276, 284–285, (3.32), (4.16)–(4.18) CMP116, pp. 5–7

For \(D_X<c_2/t\) set \(b=a^u\) in the patch gauge of §8. Then \(b_\mu(x_0)=0\) exactly. Its old first difference has the bound
\[
 [\nabla^{\xi_j} b]_\beta \le C t^{2+\beta} Q_*                       \tag{39}
\]
within the lifted box. Indeed, write each first difference of \(G_\xi(T,v,a)\) by integrating its first derivatives along the bond segment. Its integrand is a sum of \(\partial_TG_\xi\,v_\nu\) and \(\partial_aG_\xi\,\nabla_\nu^{\xi_j}a_\mu\). The constant vector \(v\) is \(O(tQ_*)\). On the chart, \(\partial_T^2G_\xi=O(|a|+|v|)\) follows from \(G_\xi(T,0,0)=0\) and bounded higher derivatives; the other required first and second derivatives are uniformly bounded. Between points at distance \(r\le C/t\), \(T\) changes by \(O(tQ_*r)\) and \(a\) by \(O(t^2Q_*r)\). The new first-difference variation from coefficients is at most \(C t^3Q_*^2r\le C' t^{2+\beta}Q_*^2r^\beta\); variation of the \(\nabla a\) argument costs \(C t^{2+\beta}Q_*r^\beta\). This proves (39).

Put \(B_{\mu\nu}=\nabla_\nu^{\xi_j}b_\mu(x_0)\). Summing the first differences along coordinate paths, (39) shows that \(b_\mu\) differs from \(\sum_\nu B_{\mu\nu}(x-x_0)_\nu\) in the old \(\|\cdot\|_1\) norm by \(C(1+D_X)^{1+\beta}t^{2+\beta}Q_*\). The pure Hessian \(D_A^2 e(0,0)\) annihilates a discrete gradient in either slot. Differentiate the invariance of \(e(a,0)\) once in \(a\) and once in the local gauge parameter at zero; the term involving the derivative of the gauge tangent disappears by \(D_A e(0,0)=0\), leaving exactly this identity. On the lifted box the symmetric part of \(B\) gives such a discrete gradient: for a symmetric matrix \(S\) use the potential \(\tfrac12 x'^TSx'-(\xi_j/2)\sum_\mu S_{\mu\mu}x'_\mu\), \(x'=x-x_0\). Each entry here may take values in the Lie algebra. Hence only the antisymmetric slope contributes.

Choose the orientation \(F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+\cdots\), and define the old-scale normalized plaquette logarithm at the common anchor by
\[
 F_{\mu\nu}(x_0)=(i\xi_j^2)^{-1}\log \partial U_{\mu\nu}(x_0),\qquad
     U=e^{i\xi_j a}.
\]
It has norm \(O(t^2Q_*)\) by (16)–(17). At \(x_0\), \(u(x_0)=1\) and all outgoing \(b\)-links vanish. Thus the plaquette in the transformed gauge is exactly \(e^{i\xi_j^2 B_{\nu\mu}} e^{-i\xi_j^2 B_{\mu\nu}}\), and
\(\|F_{\mu\nu}(x_0)-(B_{\nu\mu}-B_{\mu\nu})\|
 \le C \xi_j^2 t^4Q_*^2\).
For an antisymmetric tensor \(F\) let \(a_F\) be the affine potential with slope \(B_{\nu\mu}=F_{\mu\nu}/2\), \(a_F(x_0)=0\), and define the scalar quadratic form \(q_{jXx}(F)=P_{AA}(a_F,a_F)\). This is defined by directional evaluation at zero; it does not require exponentiating a potentially large affine configuration. Its norm obeys
\[
 |q_{jXx}(F)|\le C E_0e^{-\kappa d_j(X)}(1+D_X)^2 h_j^{-2}|F|^2.     \tag{40}
\]
Combining the preceding affine error with (35), and using the Hessian bound for \(P_{AA}\) in (36), gives on the whole complex mask domain
\[
 |P_{AA}(a^u,a^u)-q_{jXx}(F(x))|
 \le C E_0 e^{-\kappa d_j(X)}(1+D_X)^{4+\beta}
                       t^{4+\beta}Q_*^2 h_j^{-2}.                      \tag{41}
\]
The plaquette logarithm error is higher order in \(t\) and is absorbed. On large nonwinding carriers choose a lift to define \(q\) when possible; one may use any fixed bounded-coordinate lift of diameter at most \(C D_X\). On winding carriers put \(q=0\). If \(D_X\ge c_2/t\), the crude bound \(C E_0 e^{-\kappa d}h_j^{-2}t^2 Q_*^2\) for \(P_{AA}\) in the ungauged chart is bounded by (41), since \((1+D_X)^{2+\beta}\gtrsim t^{-2-\beta}\). Bound (40) and the same size inequality absorb the corresponding \(q(F(x))\) when it is present. Thus (41) also covers large carriers without a global affine gauge.

The new remainder has the connected expansion of §9.2. Since \(\sum_{a_0\ge0}L^{-\beta a_0}(1+a_0)<\infty\), its aggregate weighted native Hessian is again bounded by \(C E_0(g_k/h_k)^2\), with the same factorial higher derivative estimate. At unit masks the subtracted marginal depends on the *same physical plaquette* for every \(X\) at a fixed old root, even though the off-unit interpolations used different seeds. Regroup only now, defining \(q_{j,x}=\sum_{X\ni x}q_{jXx}\). The sole unresolved expression of the homogeneous inherited \(E\) in this decomposition is consequently
\[
 \sum_{j\le k}\left\{\sum_{x\ {\rm old\ root}}q_{j,x}(F^{[j]}(x))
                            -\beta_j\,\mathcal A(\mathbf1,U)\right\} . \tag{42}
\]
In the actual fluctuation difference this expression is evaluated at both ends. Here \(\mathcal A(\mathbf1,U)\) is the original Wilson action with the homogeneous weight, in the source normalization. The old-site sampling and normalization of its local quadratic density must be retained when comparing the two terms. A restriction with \(\phi_j\ne1\) instead has the original \(\mathcal A(\phi_j,U)\) and boundary carriers. Estimate (41) establishes the reduction without equating a finite-period coefficient \(q_{j,x}\) to an infinite-volume beta function.

### 10.2 The homogeneous Wilson coefficient and the finite-period remainder

Take cubic compatible tori and a compact simple gauge algebra, as in the single-coupling Wilson projection. On the unrestricted homogeneous branch one may symmetrize the rooted primitive representation under translations and the hypercubic group. Average the contribution at \((X,x)\) over the transformed activities at \((rX,rx)\), pulling the arguments back by \(r\). The full rooted value on real physical minimizing configurations is preserved by (2.29). The compositions agree on the common holomorphic free/retained input chart by the identity theorem from its real open subset. This equality is not an identity between the old and symmetrized activities at arbitrary independent primitive currents. Bond reversal in the extended variables uses the inverse link and the signed link-transported current, an analytic finite-stencil map bounded on a fixed smaller near-flat chart. Thus the preceding estimates still hold. The rule to discard winding \(q\)'s is itself invariant; on nonwinding lifts, changing an affine origin or the basepoint of a reversed bond adds a constant link one-form, hence a gradient for its primitive Hessian.

After this choice \(q_{j,x}\) is independent of \(x\). Invariance under the compact adjoint representation on a simple algebra makes each of its color bilinears proportional to the invariant metric. Reflections in coordinate axes remove cross terms between distinct oriented planes, and permutation symmetry equates the diagonal coefficients. In the conventions of (2.25) write
\[
       q_{j,x}(F)=c_{j,P_j} w(F),\qquad
       |c_{j,P_j}|\le C E_0 h_j^{-2}.                                \tag{43}
\]
Here \(P_j\) is the side in the old lattice units, and \(w(F)\) is the quadratic part of the Wilson action per old unit cell in a uniform antisymmetric curvature \(F\). Its positive normalization is fixed by the source trace. The bound is (40) summed at the root. For several simple factors this argument gives one invariant coefficient per factor; a single-coupling conclusion requires the corresponding symmetry or projectors.

Partition the fine Wilson plaquettes into the old unit cells by their basepoints, with a fixed convention for boundaries. Let \(W_{j,x}(U)\) denote the actual Wilson contribution in the cell of \(x\). On the same mask chart one has
\[
 |W_{j,x}(U)-w(F^{[j]}(x))|\le C t^{4+\beta}Q_*^2 .                  \tag{44}
\]
To see this directly in the global near-flat frame, the old potential is \(a=tA_s\); its old gradient has sup \(Ct^2Q_*\) and Hölder seminorm \(Ct^{2+\beta}Q_*\). The normalized logarithm of a plaquette is its linear curl plus a bounded quadratic polynomial in translated old potentials and error \(O(\xi_j t^3 Q_*^3)\), by second-order expansion of its four exponentials. Between points in one old unit cell the linear curl changes by \(O(t^{2+\beta}Q_*)\), and the quadratic polynomial by \(O(t^3Q_*^2)\), by the first-difference bound. Therefore the normalized log on every fine plaquette of a fixed orientation differs from the value at the root by \(O(t^{2+\beta}Q_*)\). Its size is \(O(t^2Q_*)\). The Wilson action per fine plaquette equals its normalized quadratic value times \(\xi_j^4\), up to \(O(\xi_j^6t^6 Q_*^3)\) from its analytic Taylor remainder. Each old unit cell has \(\xi_j^{-4}\) fine plaquettes of each positive orientation. Summing gives (44). Replacing \(F\) by the curvature of the independent current is unnecessary; here \(F\) is the geometric plaquette of the specified link field.

For (44) the cell and required stencil are one connected seed, and the masked minimally reconstructed link is (24); hence the same connected mask expansion and spatial summation apply. Combining (41), (43), (44) shows that the homogeneous inherited \(E\) equals a sum of carriers obeying the weighted native Hessian budget \(C E_0 (g_k/h_k)^2\) plus the single explicit term
\[
              \left(\sum_{j\le k}(c_{j,P_j}-\beta_j)\right)
                                  \mathcal A(\mathbf1,U).              \tag{45}
\]
The vacuum term is restored as in (2.25) and cancels in the fluctuation difference. The normalized Wilson action itself, grouped into terminal unit cells on the chart, has a bounded weighted native Hessian of order \(C g_k^2\): each cell is bounded by \(C Q_*^2\) before Cauchy and has the same connected mask expansion. Thus a finite-period version of the bound contains in addition \(C g_k^2|\sum_j(c_{j,P_j}-\beta_j)|\). This term records the actual normalization used in the running coupling.

At each **fixed** old \(j\), the limiting value of \(c_{j,P_j}\) is the physical source projector \(\beta_j\). The following argument uses convergence of the total vacuum polarization in CMP109 (1.20)–(1.22), not equality of the numerical value of every short carrier on different tori. Let \(h_{P,x}(y,y')\) be the Hessian of the physical rooted \(j\)-th birth at the flat **native coarse** field, including the actual minimizing section and physical current. For fixed \(j\) it is bounded by \(C_j e^{-a_j(|x-y|+|x-y'|)}\), with a positive \(a_j\) independent of the period. This follows by applying (14) to individual carriers, reserving part of their rooted exponential to move each source-distance anchor to \(x\). Its sum in \(x\) is the finite-period physical polarization \(\Pi_{j,P}\).

For clarity take one integral Cartan direction, coarse field \(B_2(y)=y_1 H\) on the periodic lift, and zero other components. Let \(B_R\) agree with it in a ball of radius \(R\) about root 0 and vanish outside radius \(2R\), with magnitude at most \(C R\). For \(P\ge 8R\),
\[
 \left| \tfrac12 h_{P,0}[B_R,B_R]
                  -c_{j,P}\,w(F_{12}=H)\right|
               \le C_j(1+R)^{b_j}e^{-a'_j R}.                         \tag{46}
\]
Here the positive constants may depend on fixed \(j\). To verify (46), the derivative at zero of the flat minimizing section is the constrained linear lift \(H_0\). Its lifted potential, first difference and physical current have the cell exponential of (190). On a compatible torus these flat kernels are the periodizations of their infinite-volume counterparts: periodization solves the same linear system and constraints by covariance of the block averages, and the constrained solution is unique. Equivalently periodize the flat inverse and the inverse of the coarse restricted covariance in (129); both inverses are exponentially local, so the absolutely convergent periodization commutes with their convolution products. In infinite volume the affine Cartan source lifts to a fine affine potential of the same uniform curvature and zero linear current, up to a gradient and a constant one-form. Indeed its unperturbed covariant block averages of parallel paths have this affine coarse value up to a constant link offset; the fine Maxwell divergence and divergence of the affine transverse potential both vanish. Adding a constant fine one-form fixes a constant coarse offset. The normalized coarse average constraint and the stationary flat quadratic equation characterize the lift even for this polynomially growing trial function, by applying the exponentially decaying inverses to the two equations (all sums against the affine function converge). This is also the linearized stationary Cartan section used by the physical flux projector. It follows by the cell kernel bounds that on the ball of radius \(R/3\) the lifted tangent from \(B_R\) and its current differ from this affine solution and zero current, respectively, by \(C_j(1+R)^{b_j} e^{-a'_j R}\), in the potential, gradient and current sup norms, modulo the common gradient. The radial first primitive jet is zero, so only these *first* tangents enter \(h_{P,0}\). For old carriers contained in that ball the resulting quadratic comparisons sum by (40) and the joint Hessian bound. Other old carriers have \(d_j(X)\gtrsim R/M\), and their bounds, weighted by at most a polynomial in \(R+d_j(X)\), give the same error after summing. This proves (46). CMP102, (129)–(130), (190) CMP109, (4.35)–(4.40) Physical flux and Ward normalization in the coupling analysis

Along any increasing-period subsequence, extract limits of the bounded \(c_{j,P}\) and a diagonal subsequence of \(h_{P,0}(y,y')\). Denote the latter by \(h_0\). Exponential domination permits all the following sums, and translation covariance gives \(\Pi_j(0,v)=\sum_y h_0(y,y+v)\), using the source's thermodynamic limit of the total polarization. The Ward identity kills a constant 2-direction Cartan one-form in either input of \(h_0\): it is a gradient on the infinite lift, approximated on growing neighborhoods by compactly supported gradients with at most polynomial growth. First jets vanish, and exponential domination passes the finite-support Ward identity to the limit. Taking the period limit in (46) and then \(R\to\infty\) therefore gives, with Cartan color and 22-component understood,
\[
 \lim c_{j,P}\,w(F_{12}=H)
  =\tfrac12\sum_{y,y'} h_0(y,y')y_1y'_1
  =-\tfrac14\sum_v v_1^2\,\Pi_j(0,v).                                \tag{47}
\]
The second equality expands \((y'_1-y_1)^2\); the two diagonal squares vanish by the Ward identity. The source Ward and hypercubic relations in CMP109 §§4–5 identify this transverse second moment with its Wilson projector in (1.22). The normalization in (47) is fixed without a sign convention by applying the identical identity to the unit Wilson action, for which the left side is exactly \(w(F_{12}=H)\); CMP109 (4.39)–(4.42) gives the unit quadratic symbol. Thus every subsequential scalar limit is \(\beta_j\). CMP109, pp. 264, 290–298, (1.20)–(1.22), (4.37)–(4.45)

At fixed terminal depth \(k\), take the homogeneous thermodynamic limit along compatible covers first. Equation (45) then vanishes and all surviving inherited \(E\) carriers in this chosen representation have the small native Hessian budget and factorial higher derivatives above, on the restricted homogeneous charts. The estimates for those surviving carriers are uniform in depth on admitted trajectories. The argument does not give a jointly uniform finite-period rate for (45), does not treat a nonconstant \(\phi_j\) or an old large-field boundary, and does not differentiate the \(W\)-dependent gauge in (33). These distinctions are needed for C-02, C-04 and the finite-cutoff marked conditional law.

### 10.3 A real calibration bounds the finite-period remainder

There is also a uniform bound for (45) at finite compatible period. Choose a terminal torus of side at least 8 in terminal lattice units, as in the ordinary homogeneous construction, and put
\[
      s_k=c_1\min(h_k,\varepsilon_k),\qquad
      \varepsilon_k=g_k p_0(g_k),\qquad 0<\delta<1.                   \tag{48}
\]
Under the source admissibility assumptions for the homogeneous trajectory, the individual scalar in (45) satisfies
\[
 |c_{j,P_j}-\beta_j|
       \le C E_1\,t^\delta s_k^{-2}
                       + C E_0\,t^\beta h_j^{-2}.                     \tag{49}
\]
Here \(E_1\) is the constant in CMP119 Theorem 2 with exponent \(\delta\), and \(\beta\) is the first-gradient Hölder exponent in (39). The two exponents need not coincide. This uses (2.43) as a real estimate on one *specific* physical configuration; bounds on its complex continuation are unnecessary.

**Choice of calibration.** In the native coarse input to the layer \(k\) minimizer take \(V(\lambda)=\exp(i\lambda B)\), where \(B_2(y)=\cos(p y_1)H\) for a fixed unit Cartan generator and all other components vanish. Choose \(p=2\pi m/P_k\in[\pi/3,2\pi/3]\). Such an integer exists at every indicated period. This is a periodic background with continuously adjustable amplitude and no flux quantization. For real \(\lambda=s_k\) it lies on the regular branch used by (2.43): its coarse links and plaquettes have size \(O(s_k)\). The homogeneous minimizing section has normalized fine potential and first gradient \(O(s_k)\) by CMP102 (19); its fine plaquettes have size \(O(\eta^2 s_k)\). In a copied local good-plaquette test the internal links are identity and homologous crossings use the given coarse link, so the mixed-scale plaquettes are identity or conjugate to coarse plaquettes of size \(O(s_k)\). The local minimizing-field bound of CMP102 Theorem 1 gives the same \(O(s_k)\) normalized bound in the testing interior. Intermediate old normalized curvatures are at most \(C t^2s_k\le C'c_1\varepsilon_j\) by (2.8). Taking \(c_1\) small gives the regularity required in (2.43); there is no terminal exceptional region in this homogeneous test. One can equally apply the stated sufficiently regular minimizing-configuration form of Theorem 2. This choice tests the primitive on its \(k\)-scale determining field, independently of the later real/complex fluctuation to which (49) will be applied. CMP119, pp. 255–256, 263, (2.4)–(2.8), (2.43) CMP102, Theorem 1 and (19)

The actual Wilson action at this test obeys
\[
           \mathcal A(\mathbf 1,U_k(V(s_k)))/V_k\ge c_2 s_k^2          \tag{50}
\]
uniformly in terminal period and depth, where \(V_k\) in the denominator denotes the number of terminal sites. Here are details of the lower bound. At zero, let \(a\) be the fine normalized linear lift of \(B\) in the flat Landau representative. Modulo coarse gradients, the normalized linear block average of a one-form is a contraction from the fine normalized \(L^2\) norm to the coarse one. In fact, differentiating the one-step formula (0.4) or (0.12), the entry and exit contour sums have the form of a coarse gradient: the same average of paths from a block center to its sites is used at both ends. The remaining map in a direction \(\mu\), in potentials per unit physical length, is the positive average over \(x\) in the starting \(L\)-block and \(0\le r<L\) of \(a_\mu(x+r e_\mu)\). Jensen and summation over starting blocks give its norm at most one, since \(x\) ranges over all fine sites once before each fixed shift \(r\). The average sends fine gradients to coarse gradients, by telescoping the straight paths. Thus it induces a contraction on one-forms modulo gradients, as does its iteration. Any endpoint gauge returning the lift to the axial constraints changes the linear coarse form only by a gradient. Write \(a^\perp\) for the orthogonal complement to fine gradients. The coarse wave \(B\) is transverse, so we have \(\|a^\perp\|_{2,\mathrm{av}}\ge\|B\|_{2,\mathrm{av}}\ge c>0\), with norms normalized by volume.

Flat linear operators commute with translation by a terminal unit; hence \(a\) has only the terminal Bloch characters with momenta \(\pm p e_1\). Fine Fourier frequencies \(q\) in these characters obey \(q_1=\pm p\bmod 2\pi\) and can be taken in the fine Brillouin zone. The discrete derivative symbol \(2\eta^{-1}\sin(\eta q_1/2)\) has magnitude at least \(2|q_1|/\pi\ge 2/3\). On the orthogonal complement to gradients the squared curl symbol is the squared derivative-symbol length. Therefore \(\|d_\eta a\|_{2,\mathrm{av}}\ge c \|a^\perp\|_{2,\mathrm{av}}\ge c'\). This bounds the quadratic Taylor coefficient of the Wilson action per volume below by a positive construction constant. On a fixed complex \(\lambda\)-disc the minimizing section satisfies \(\|A\|+\|\nabla A\|\le C|\lambda|\), so each fine plaquette differs from identity by \(O(\eta^2|\lambda|)\). The analytic Wilson action divided by volume has sup \(C|\lambda|^2\) there, uniformly in the mesh after the \(\eta^{-4}\) fine-plaquette count. Cauchy bounds the Taylor terms of order at least three on a smaller disc by \(C|\lambda|^3\); this proves (50) for small \(s_k\). CMP109, (0.4), (0.12) CMP102, Proposition 9

**Comparison on the test.** In CMP119 (2.43) take \(\Omega\) to be the whole homogeneous torus and \(\phi=1\). Only the terminal determining layer \(n=k\) is present. Therefore the *real* \(j\)-th contribution after its true vacuum and Wilson subtractions is bounded per terminal site by \(E_1 t^\delta\). The decomposition (36)–(45) on the same input has \(Q=C s_k\). Before summing \(j\), the per-terminal-site absolute values of all its terms except \((c_{j,P_j}-\beta_j)\mathcal A\) are bounded by
\[
 C E_0\!\left[t^2s_k^3 h_j^{-3}
                 +(t+t^\beta)s_k^2 h_j^{-2}\right]
 \le C' E_0 t^\beta s_k^2 h_j^{-2}.
\]
This follows from (37), (41), (43)–(44) with the old count \(t^{-4}\). In the last inequality use \(s_k/h_j\le C(1+k-j)^{1/2}\) and \(t^{2-\beta}(1+k-j)^{1/2}\le C_\beta\). Now the triangle inequality and (50) give (49).

For each output cell use a separate copy of its localized Wilson action with coefficient \(c_{j,P_j}-\beta_j\). This keeps an age-by-age representation, and (49) supplies its complex norm after the real scalar was identified. Combining (37)–(44), (49), and the same mask expansions as (28) gives the complete **homogeneous inherited \(E\)** weighted free-coordinate Hessian bound on the half-sized central chart of (31),
\[
  C\left[E_0(g_k/h_k)^2+E_1(g_k/s_k)^2\right].                       \tag{51}
\]
The age sums are geometric for \(t^\delta\) and for \(t^\beta(h_k/h_j)^2\). In particular the result is uniform in the compatible finite torus and depth, under the source hypotheses, and tends to zero as a negative power of \(\log(g_k^{-2})\). All derivatives here are of actual composed activities on complex charts. An order-\(p\) weighted local norm is at most
\[
 C\left[E_0+E_1(h_k/s_k)^2\right]\,
                 p!(C' g_k/h_k)^p
\]
on that half chart, because all old sums have been paid at the value level before differentiating. Joint normalized \(v/g_k,z\) estimates follow from (31), and the free-coordinate version for a fixed real small outgoing \(W\) follows from (33). Taking \(Q_*\) proportional to \(s_k\) in the destination chart instead yields the corresponding smaller-chart prefactor \(C(E_0+E_1)\) and radius \(c s_k/g_k\). The result also applies to the difference of the two endpoints in the physical fluctuation action, with the same qualification about retained coordinates.

Equation (51) removes the need for any finite-volume convergence rate in (45) on this homogeneous subproblem. It does not prove the full C-02, C-03 or C-04 tests. A selected geometry has nonconstant \(\phi_j\), truncated primitive families and boundary data; the reduction to a *single constant Wilson coefficient* in (45) then has no justification. The outer preparation maps and arbitrary marked histories also remain outside the single homogeneous input chart.

## 11. A necessary current-radius test on a genuine free fiber

The following test distinguishes a missing estimate from a normalization that could make a blanket admission statement false. Work on the homogeneous fiber over identity, with a period compatible with the single blocking factor \(L\ge2\). Let \(B_2(y)=\cos(2\pi y_1/L)H\) for a nonzero fixed Cartan element and \(B_\mu=0\) in other directions. For small real \(s\), the one-step average satisfies \(M(\exp(isB))=1\) exactly. Within this Abelian line the logarithms and group averages on the near-identity branch reduce to ordinary sums. The averaged endpoint paths at the ends of a coarse bond cancel by \(L\)-periodicity; the mean straight path in direction 2 is zero on averaging over the first coordinate. Other straight paths are identity. Thus this configuration satisfies the nonlinear coarse constraint, not just its derivative. Its free \(z\) coordinates in (3.15) are bounded by \(C_L s/g_k\), since in these coordinates the distinguished bonds are uniquely recovered from the constraint and the nonlinear correction vanishes on the Abelian family. A fixed block-tree axial representative, if used for relative coordinates, is reached by bounded-length real block paths and changes this constant only. CMP109, (0.4), (0.12), (2.4), pp. 267–268 CMP119, (3.15)–(3.16)

For the true fine minimizer at this input, in \(k\)-terminal units,
\[
               \max_b\left|J_\eta(U_k(e^{isB}))(b)\right|
                              \ge c_L |s|,\qquad 0<|s|\le s_0(L).     \tag{52}
\]
Indeed its first tangent at zero has current \(d_\eta^* d_\eta H_0B\). The proof of (50) applies with the fixed nonzero Bloch momentum \(2\pi/L\) (use its Brillouin representative). On its transverse component \(|d_\eta(q)|\ge c_L\), and the coarse quotient-\(L^2\) contraction gives a uniform positive lower bound on the transverse tangent norm. Therefore the volume-normalized \(L^2\) norm of \(d_\eta^* d_\eta H_0B\), and hence its sup norm, is at least \(c'_L\). On a fixed complex disc in \(s\), §7 bounds the full physical current by \(C|s|\); its difference from its first term is uniformly \(O(s^2)\) by scalar Cauchy. Shrinking \(s_0\) proves (52).

The actual current in (52) is real in a compact frame. For such \(J\), a positive multiple of its compact norm squared is given by the invariant quadratic trace in a faithful unitary representation (or the compact Killing form). This invariant extends complex bilinearly, and its modulus at a complex vector is bounded by a fixed multiple of its complex norm squared. Consequently every complex conjugate of the current at a maximizing bond has norm at least \(c'_G c_L |s|\). The general bound in (1.14) is \(|J|<\gamma_0\); the two-parameter primitive domain used in (2.28) has \(\gamma_0=\alpha_{0,k}\) by CMP109 p. 263. Thus on a primitive carrier containing that bond the current must have norm less than \(\alpha_{0,k}\) in some representative. Taking \(s=c\min(g_k r_k,\varepsilon_k,s_0)\) keeps the free cutoff and small genuine coarse tests with slack. Thus a universal assertion that **all bonds** on the whole free product fall inside this primitive domain requires
\[
                     \min(g_k r_k,\varepsilon_k,s_0)
                                     \le C_{L,G}\alpha_{0,k}.          \tag{53}
\]
This real-point necessity already precedes choosing a complex bidisc. In the interpretation \(g_k r_k\asymp\varepsilon_k\), it rules out obtaining such an all-bond assertion solely by recentering when \(\varepsilon_k/\alpha_{0,k}\) diverges. The source has not here been shown to choose exponents with that divergent ratio. Equation (53) also does not prove that a specific nonzero primitive depends on the maximizing bond, or impose a corresponding necessary inequality for the distinct relative-potential radius \(\alpha_{1,k}\).

## 12. The coefficient defect from a truncated old carrier family

A part of the nonhomogeneous obstruction can be quantified at the primitive quadratic level. In CMP119 (2.26)–(2.27) the roots of \(E^{(j)}(\Lambda_j,U)\) lie in \(\Lambda_j^0\) and only carriers \(X\subset\Lambda_j\) enter. Consider the unrestricted old rooted family that gives (2.29), with the *same* coefficients and parameters, and denote by \(q^{\rm omit}_{j,x}\) the sum of (40) on its omitted \(X\ni x\). This is an estimate on the numerical tensors at vacuum and requires no continuation of exterior fluctuations across the boundary. For every such root, using the actual old distance,
\[
  \|q^{\rm omit}_{j,x}\|\le C E_0 h_j^{-2}
                e^{-c\,{\rm dist}_j(x,\Lambda_j^c)/M}.               \tag{54}
\]
If \(X\) meets the complement, a path through its connected old cubes has to travel this distance. The tree definition used above gives \(1+d_j(X)\ge c\,{\rm dist}_j(x,\Lambda_j^c)/M\). Reserve part of its exponential in (40) for that distance; the remaining exponential pays the anchored animal count and diameter factor. This proves (54). On roots with distance at least \(c M R_j\), the coefficient sum over old \(j\)'s is actually smaller than every fixed positive power of \(g_k\) under the admitted six-power trajectory sum: \(R_j\ge(\log g_j^{-2})^r\), \(r\ge2\), and \(h_j^{-2}\le C g_j^{-2}\). Thus \(e^{-cR_j}h_j^{-2}\le C_N g_j^{N+7}\) for any fixed \(N\) and small \(g_j\), which suffices after summation. The estimate does not assert the weighted *pullback* until its maps and local complex charts have been controlled. CMP119, pp. 259–260, 280–282, (2.25)–(2.29), (3.48)–(3.57)

There is a separate actual weight in that comparison: the Wilson subtraction is \(\beta_j\mathcal A(\phi_j,U)\) with \(\phi_j\) supported in \(\Lambda_j\) and equal to one in the source's inner region. Approximating it by old cell densities leaves weights given by the cell averages of \(\phi_j\), whereas the root sum in (2.26) has \(\mathbf1_{\Lambda_j^0}\). Any difference is an explicit collar-supported term. Equation (54) concerns missing carriers and gives no decay for a collar weight itself. At present the required current derivative bound for that weighted collar with the actual multiscale preparing maps is still unproved.
