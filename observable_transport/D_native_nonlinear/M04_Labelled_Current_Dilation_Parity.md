# The actual dilation preserves parity for each owned smooth-current linear jet

This note extends SC's interacting quadratic comparison to the separate microscopic, old-kernel and new-kernel current origins of the actual three-layer smooth conditional. The proof uses the literal independent-copy amplitude of TR.27. It does not infer separate-origin cancellation from parity of the diagonal scalar alone.

Each origin's linear output jet is even in the auxiliary dilation parameter. Consequently its difference from its own inherited Gaussian linear-current transfer is of order `B_3 eta^2`, with the same `eta = C_L[g_2 P^3 + (1+E_2)g_2 P]` as SC. In particular the newly created outer-kernel current has a linear jet of this small order, because that origin is identically absent at the Gaussian endpoint. The incoming old-origin matrices are not automatically symmetric or transverse in both slots; FH contraction for every old label is therefore not asserted.

## 1. The actual two-layer independent-copy source

Let the block-summed microscopic source be
\[
 \mathfrak f_n(U)=h_0^4\sum_{x\in B_3(n)}
                   (\alpha\beta_0\sigma_{h_0}(x;U)-c).
 \tag{OP.1}
\]
Use the first and second smooth kernels and their exact source maps from TR, with their fixed couplings and product domains. Define the three-copy amplitude on the level-two lattice by
\[
\begin{split}
 \mathcal B_n(V_M,V_0,V_1)
 ={}&\int q_{1,A}(dz_1\mid V_1)
       \int q_{0,P}(dz_0\mid\Psi^{(1)}_{V_0}(z_1))\\
 &\quad\times\mathfrak f_n
    \bigl(\Phi_{\Psi^{(1)}_{V_M}(z_1)}(z_0)\bigr).
\end{split}
 \tag{OP.2}
\]
This is TR.27 stopped before the third integral. Its diagonal is exactly the incoming source of SC:
\[
 \mathcal B_n(V,V,V)=F_{n,2}(V).
 \tag{OP.3}
\]
The copies retain their literal ownership: M changes the microscopic reconstruction, 0 changes only the first normalized kernel and its own normalizer, and 1 changes the whole second normalized kernel and its own normalizer. In a copy derivative every displayed test is held fixed at the current parameter and the original free coordinates are held fixed, as in DP.5--DP.7. No zero-jet cancellation is used to reassign a derivative of an inverse normalizer.

### Lemma OP.1 — a fixed physical three-copy tube and separate first-jet zeros

At these two fixed levels, (OP.2) has a common supported holomorphic coefficient family for three independent physical raw-link charts of a fixed radius r. With the constant microscopic insertion removed, its anchored norm is at most
\[
 C_LM_2,
 \qquad M_2=L^{12}|\alpha|g_0^{-2}.
 \tag{OP.4}
\]
Every fixed number of physical derivatives and every fixed carrier moment obeys the corresponding Cauchy bound. Complete coefficients may be chosen so that each partial first jet at \((I,I,I)\) is zero:
\[
 D_{V_r}\mathcal B_{n,X}(I,I,I)=0,
       \qquad r=M,0,1.
 \tag{OP.5}
\]

**Proof.** PJ supplies the fixed physical native buffers for the actual source maps and the full force-containing raw pullbacks. For each occurrence in (OP.2), use its own critical-canceled normal form, as required in TR.27 and TC's independent smooth-copy construction. A physical perturbation of each of the finitely many copies changes every complete native input by at most \(C_Lr\); the fixed real capped innovations add \(C_L(g_0P_0+g_1P_1)\). Choose r inside the strict native buffers and then the weak-coupling ceiling. The full minimum, force, constraint, reference, target, inverse, determinant and Haar/coarea data therefore remain in the same common component family for all three copies. No density is re-expanded about the microscopic copy's different background.

The bounded microscopic Wilson source has holomorphic size \(C_LM_2\) on that whole domain. Its value bound does not compare the source's energy at one copy to the energy at another copy. Insert it before the two nested normalized component expansions, with the actual inverse-beta local source circle. Each kernel's source-zero integral is one for every independent argument. The same-gas root deletion consequently preserves the two exact denominators and gives (OP.4). Old normalized nodes are bounded uniformly in the later real variable before the later Gaussian is integrated. Independent copies do not create an extra later quadratic store per old occurrence. Ordinary local rank costs are paid by the same fixed-depth spare carrier margin. This is the bounded-source proof of PJ applied to the literal finite independent-copy formula, not an assertion about an arbitrary off-diagonal hard-Q law.

The amplitude is invariant under simultaneous global colour conjugation of all three arguments. For each real constant colour rotation the old free variables change by constant orthogonal adjoint maps, preserving their fixed domains and complete normalized kernels. All source maps and the scalar mark transform covariantly. Average each **complete scalar coefficient** over that compact global colour group. The sum, supports, copies and analytic bound are unchanged. At \((I,I,I)\), a derivative in any one copy is then an invariant linear functional on the adjoint representation. It is zero separately for that copy, proving (OP.5). This is stronger than the vanishing of the sum of the three first jets and uses only a constant real gauge transformation. \(\square\)

If one also uses EC's simultaneous local gauge projection, every determining gauge endpoint and the actual lifted reference data must be kept. Nothing in Lemma OP.1 requires separate gauge invariance in each copy, which is generally false.

## 2. A four-copy outer dilation with the origins fixed

Use SC's exact physical map \(\Xi\), full density \(D_t\), denominator \(Z_t\) and normalized outer conditional
\[
 q_{2,t,b_2}(dc)=Z_t(b_2)^{-1}\chi_P(c)D_t(c;b_2)\,dc.
 \tag{OP.6}
\]
All its inherited action pieces, force corrections, full soft gauge and measure factors are exactly those in SC.12. In particular only the outer classical and soft-gauge terms carry \(t^{-2}\), while the whole old radiative action is the fixed actual function at its dilated physical arguments.

For four independent normalized coarse copies \(\mathbf b=(b_M,b_0,b_1,b_2)\), put
\[
 V_{t,r}(c)=\Xi(e^{t g_2b_r},t g_2c),\qquad r=M,0,1,
 \tag{OP.7}
\]
and define
\[
\begin{split}
 \mathcal A_{n,t}(\mathbf b)
 =t^{-2}\bigl\{q_{2,t,b_2}[\,
       \mathcal B_n(V_{t,M},V_{t,0},V_{t,1})\,]
                     -\mathcal B_n(I,I,I)\bigr\}.
\end{split}
 \tag{OP.8}
\]
The subtracted quantity is one number. The outer kernel has mass one in its own variable and denominator, so this is equivalently its expectation of the constant-subtracted source divided by \(t^2\). The microscopic identity insertion cancels exactly at every t and for every copy.

At t=1, (OP.8) is the literal four-copy amplitude TR.27, apart from its displayed constant. A partial derivative in copy r is therefore the prescribed current origin r. In the diagonal current no partial parameter is silently moved to another factor.

The family has a removable value at t=0 by (OP.5). Indeed all three physical arguments in (OP.7) are \(O_L(|t|g_2P)\) from I. Its complete coefficient bound is
\[
 \sup_{|t|<R,\ \|b_r\|_\infty<4P}
       \|\mathcal A_t\|_\kappa\le C_L B_2P^2,
 \quad B_2=M_2g_2^2,
 \quad R=c/\eta>2,
 \tag{OP.9}
\]
\[
 \eta=C_L\{g_2P^3+(1+E_2)g_2P\}.
 \tag{OP.10}
\]
To prove this bound, use the joint second physical derivative of \(\mathcal B_n\) to cancel \(t^{-2}\) before taking absolute values. Then apply SC.2's actual large-disc ordinary and failed-P bounds and its same-gas normalized source insertion. Lemma OP.1 admits the three independent old copies throughout this disc. Every copy has \(|t|g_2P\le c/[C_L(P^2+1+E_2)]\), so all the physical admission and rank costs remain within the same fixed margins. This proves (OP.9), including complete normalization connectors and all fixed carrier moments at a smaller rate.

## 3. The owned currents and their exact sign identity

For a normalized direction h on the final coarse coordinate list define
\[
 j^r_{n,t}(b;h)
   =D_{b_r}\mathcal A_{n,t}(\mathbf b)[h]
                         \big|_{b_M=b_0=b_1=b_2=b},
       \qquad r=M,0,1,2.
 \tag{OP.11}
\]
For an old label, this is exactly
\[
 j^r_{n,t}(b;h)
  =t^{-2}q_{2,t,b}\!\left[
    D_{V_r}\mathcal B_n(V_{t,M},V_{t,0},V_{t,1})
                     [D_bV_{t,r}(c)[h]]\right]_{\rm diag}.
 \tag{OP.12}
\]
The derivative of \(\mathcal B\) in (OP.12) has precisely its literal microscopic/old-kernel ownership from (OP.2). For the new label it is
\[
 j^2_{n,t}(b;h)
  =t^{-2}(D_bq_{2,t,b}[h])
          [\mathcal B_n(V_t,V_t,V_t)],
 \tag{OP.13}
\]
where the displayed test is held fixed in that kernel derivative. Its exact normalized derivative is
\[
 D_bq_{2,t,b}[h]
   =Z_t^{-1}D_bN_t[h]
          -q_{2,t,b}Z_t^{-1}D_bZ_t[h],
 \quad N_t(dc)=\chi_P(c)D_t(c;b)\,dc.
 \tag{OP.14}
\]
Thus the full outer inverse normalizer, determinant, inherited action and coarea response belong to label 2. Its kernel derivative annihilates the constant test. The P domain is fixed and has zero physical shape derivative.

Define the linear output jet of each current by
\[
 \mathcal L^r_{n,t}(h,k)
    =D_b[j^r_{n,t}(b;h)]\big|_{b=0}[k]
    =\sum_{s=M,0,1,2}
       D_{b_s}D_{b_r}\mathcal A_{n,t}(0)[k,h].
 \tag{OP.15}
\]
The derivative in k is the variation of the physical diagonal field. It therefore differentiates all four copies, while the current direction h stays in its owned copy r.

### Lemma OP.2 — separate-origin parity

For each r,
\[
 \mathcal A_{n,-t}(-\mathbf b)=\mathcal A_{n,t}(\mathbf b),
 \tag{OP.16}
\]
\[
 j^r_{n,-t}(-b;h)=-j^r_{n,t}(b;h),
 \qquad
 \mathcal L^r_{n,-t}(h,k)=\mathcal L^r_{n,t}(h,k).
 \tag{OP.17}
\]

**Proof.** Under \((t,\mathbf b,c)\mapsto(-t,-\mathbf b,-c)\), every retained physical link and each physical outer fluctuation in (OP.7) is unchanged. Hence every argument of the old microscopic map and of each old normalized kernel is literally the same. The old innovation variables need not be changed: the physical data passed to their kernels already agree. The outer density and its denominator obey the exact identity SC.25. Its fixed P domain is centrally symmetric. The explicit \(t^{-2}\) is even. Changing the outer integration variable to minus itself proves (OP.16) for the entire independent-copy amplitude.

Differentiate this identity in its **specified copy r**, not in the sum of all copies. The chain rule gives the first identity in (OP.17). Differentiate next along the physical diagonal b at zero; the second sign cancels the first. This proves the evenness of each \(\mathcal L^r\) separately, with no exchange of labels or inverse-normalizer ownership. \(\square\)

For absolute coefficient bounds, apply the complete-scalar projection
\[
 a_{n,X}(t,\mathbf b)\ \mapsto\
 \tfrac12\{a_{n,X}(t,\mathbf b)+a_{n,X}(-t,-\mathbf b)\}.
 \tag{OP.18}
\]
The physical sum is unchanged by (OP.16); supports, copies and labels are unchanged. Each resulting mixed Hessian is even in t. Partial differentiation then produces a representation of every owned current with that property. Because the projection is made on the actual four-copy amplitude before its copy derivatives are taken, it is a common representation of all origins, rather than a separate value decomposition invented for each current.

Each current's constant value at b=0 is also zero. To see this directly, simultaneous global colour conjugation of all four copies and the corresponding constant real adjoint changes of all free variables leave (OP.8) invariant. A derivative in one copy at all zero arguments is an invariant colour covector, and vanishes. This observation is separate from parity and requires no cancellation between origins.

## 4. Identification of the Gaussian endpoint for each label

Let \(K_{rs}\), \(r,s\in\{M,0,1\}\), be the block Hessian at zero of
\[
 (u_M,u_0,u_1)\longmapsto
     \mathcal B_n(e^{g_2u_M},e^{g_2u_0},e^{g_2u_1}).
 \tag{OP.19}
\]
Its quadratic polynomial is
\[
 Q_n^{\rm cp}(u_M,u_0,u_1)
     =\tfrac12\sum_{r,s=M,0,1}K_{rs}[u_r,u_s].
 \tag{OP.20}
\]
The block transpose relation is \(K_{rs}=K_{sr}^{\mathsf T}\). The incoming diagonal quadratic of SC is \(Q_{n,2}(u)=Q_n^{\rm cp}(u,u,u)\).

At the flat endpoint, SC.14 gives a fixed centered Gaussian density with the fixed P domain, independent of every coarse b. SC.15 gives the common linearization \(Hb_r+\mathsf C_0c\) in each old source copy. Therefore
\[
 \mathcal A_{n,0}(\mathbf b)
   =\mathbb E_{\mu_{K_0}^{P}}
      Q_n^{\rm cp}(Hb_M+\mathsf C_0c,
                   Hb_0+\mathsf C_0c,Hb_1+\mathsf C_0c).
 \tag{OP.21}
\]
It is independent of b_2. Central symmetry removes all mixed b--c terms, and the purely fluctuating term is a constant independent of all four b's. It follows that
\[
 j^2_{n,0}(b;h)=0,\qquad \mathcal L^2_{n,0}=0,
 \tag{OP.22}
\]
and, for an old label r,
\[
 j^r_{n,0}(b;h)
     =\sum_{s=M,0,1}K_{rs}[Hh,Hb],
 \qquad
 \mathcal L^r_{n,0}(h,k)
     =\sum_{s=M,0,1}K_{rs}[Hh,Hk].
 \tag{OP.23}
\]
The sum over s is the linear jet of the incoming **same owned current r** along its diagonal. Equation (OP.23) therefore identifies its actual inherited Gaussian transfer. It is not an arbitrary split of the scalar Hessian. As in SC, truncation changes the Gaussian trace but not these formulas; the trace is constant and has zero owned current.

## 5. A two-power comparison for every physical current origin

Use the same positive carrier rate, with strict losses for incidence sums and any fixed spatial moment. Let \(\|\cdot\|_{\kappa,s}^{(2)}\) denote the anchored sum of the absolute bilinear matrix coefficients in the complete two direction lists, including moment \(1+\operatorname{diam}(X)^s\).

### Theorem OP.3 — actual per-origin linear-jet comparison

For every label \(r=M,0,1,2\) and every fixed s,
\[
 \|\mathcal L^r_1-\mathcal L^r_0\|_{\kappa,s}^{(2)}
        \le C_{L,s}B_2\eta^2.
 \tag{OP.24}
\]
Convert to the literal final normalized coordinate \(W=e^{g_3a}\), so \(b=\rho a\), \(\rho=g_3/g_2\). The physical current has one factor \(\rho\), and its linear field jet has two. Consequently
\[
 \boxed{\quad
 \|\mathcal L^{r,\mathrm{phys}}_{\mathrm{actual}}
            -\mathcal L^{r,\mathrm{phys}}_{\mathrm{Gauss}}\|_{\kappa,s}^{(2)}
        \le C_{L,s}B_3\eta^2,
 \qquad B_3=\rho^2B_2.\quad}
 \tag{OP.25}
\]
For the new outer-kernel label, its Gaussian term is zero, so
\[
 \|\mathcal L^{2,\mathrm{phys}}_{\mathrm{actual}}\|_{\kappa,s}^{(2)}
       \le C_{L,s}B_3\eta^2.
 \tag{OP.26}
\]

**Proof.** Two copy Cauchy derivatives of (OP.9), on smaller balls, cancel its factor \(P^2\). Summing coordinate lists and inserting a fixed spatial moment costs only fixed carrier polynomials. There are four copies and four terms in (OP.15), which are fixed constants. Thus \(\|\mathcal L^r_t\|_{\kappa,s}^{(2)}\le C_{L,s}B_2\) throughout \(|t|<R\), for every r. In the representation (OP.18) its Taylor series is even by Lemma OP.2. The same geometric Cauchy estimate as SC.33 gives
\[
 \|\mathcal L^r_1-\mathcal L^r_0\|_{\kappa,s}^{(2)}
    \le \frac{C_{L,s}B_2}{R^2-1}
    \le C_{L,s}B_2\eta^2.
 \tag{OP.27}
\]
The factors \(\rho\) for the direction and for the base field give (OP.25). Equation (OP.22) then gives (OP.26). These are estimates of each owned current before any sum over labels; no total-current cancellation is used. \(\square\)

There is also a direct fixed-slice bound on each complete current comparison:
\[
 \|j^r_1-j^r_0\|_{\kappa,\|b\|\le P}
       \le C_LB_2P\eta,
 \tag{OP.28}
\]
with the factor \(\rho\) in the physical a convention. It follows from one copy Cauchy derivative and the t-series beginning at degree one. It controls the actual smooth first-current function on that slice, not only its linear jet. Equation (OP.25) is stronger specifically at the linear jet because the second t sign is then available.

## 6. What this does and does not provide for M04

The result resolves the specific parity question for the actual smooth origin convention: microscopic, first-kernel, second-kernel and new third-kernel linear output jets each have the two-power interacting comparison. The newly created kernel current has no inherited Gaussian linear term at all. Every old label is compared with the Gaussian transport of its own incoming linear jet, with its literal old maps and normalizers.

This is not yet an irrelevant contraction for every label. A block row \(\sum_sK_{rs}\) of a multi-copy Hessian need not be symmetric, and a joint gauge identity need not make it transverse in its current-direction slot. Only the total diagonal scalar Hessian is automatically the two-sided Ward object used by FH. If simultaneous local gauge covariance of the independent-copy family is invoked, differentiating that identity gives the corresponding row Ward identity in the diagonal field slot; it does not supply the missing independent-copy gauge symmetry in the other slot. Additional analysis is needed before applying FH separately to those rows.

The theorem concerns fixed smooth P domains. A moving hard-Q boundary is not invariant under the auxiliary deformation with the same fixed real domain, and its owned shell currents are not included here. Nor does a fixed-depth per-origin jet estimate imply a uniform budget over arbitrarily many old origins. Finally, finite-torus winding pieces keep their actual exponential support bound; a pure curvature seminorm conclusion would need the topology qualification already made in SC.

Inputs are the PJ physical tubes and complete bounded-source envelopes, TC/TR's literal independent smooth-copy and ownership construction, SC's exact dilation and normalizer family, and EC's support-preserving complete-coefficient projection rules. This note proves the new separate-origin parity and its actual transfer formulas. It does not claim that M04 or Yang--Mills existence is proved.
