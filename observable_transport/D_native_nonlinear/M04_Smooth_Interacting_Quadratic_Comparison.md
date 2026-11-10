# An actual smooth interacting step and its inherited Gaussian quadratic part

This note compares the actual third homogeneous smooth conditional in TC/TR with its inherited flat Gaussian quadratic transfer. The incoming observable is the actual twice transported microscopic local source. The comparison retains the exact constrained reconstruction, the inherited force-corrected classical action, the full averaged soft gauge, the inherited analytic action, Haar/coarea factors and every conditional denominator.

There are two conclusions. On the native small-link slice the full vacuum-subtracted scalar differs from its inherited Gaussian quadratic expression by a supported small nonlinear error. At the flat field its actual Hessian differs from that Gaussian expression by a **two-coupling-power** error. The second conclusion uses a concrete auxiliary dilation and its exact parity, rather than estimating a first perturbation in absolute value. It yields an actual interacting quadratic version of FH's irrelevant gain. It does not prove the full nonlinear M04 norm, moving-Q transfer, or an induction uniform in depth.

## 1. The actual third input and the observable

Use precisely TC's convention
\[
 \rho_{\mathrm{aux},2}(V)
 =\chi_2(V)c_{\mathrm{vac},2}
     \exp\{-g_1^{-2}A(U_2(V))+\mathcal A_2(U_2(V),J_2(V))\}.
 \tag{SC.1}
\]
Write
\[
 \mathscr S(V)=A(U_2(V)),\qquad
 \mathscr E(V)=\mathcal A_2(U_2(V),J_2(V)).
 \tag{SC.2}
\]
Thus \(\mathscr E\) includes the earlier Gaussian normalization, all inherited analytic pieces, the complete measure/coarea contributions assigned to that action, and any retained signed polarization discrepancy. It is not a bare Wilson action. Let \(E_2\) denote a uniform native analytic coefficient bound for this fixed two-level action. TC.1 supplies it independently of volume and weak coupling, with constants allowed to depend on the two fixed levels.

At a final level-three block n put
\[
 F_{n,2}(V)
   =h_0^4\sum_{x\in B_3(n)}(q_{1,A}q_{0,P}F_x)(V),\qquad
 F_x=\alpha\beta_0\sigma_{h_0}(x)-c.
 \tag{SC.3}
\]
This is the sum of the actual level-two local marks over the level-two blocks in the final block. Its third smooth transfer is exactly SW's mark
\[
 \Phi_{n,3}(W)=q_{2,A,W}F_{n,2}.
 \tag{SC.4}
\]
All maps and couplings used to define these conditionals are the zero-source ones. Constants in \(F_{n,2}\) transport exactly and disappear from every subtraction below.

PJ's proof stopped after two integrations gives, on a fixed physical tube and with all fixed carrier moments,
\[
 \|F_{2}^{\alpha}\|_{\kappa,r}\le C_LM_2,
 \qquad M_2=L^{12}|\alpha|g_0^{-2}.
 \tag{SC.5}
\]
Complete scalar coefficients may be compact-colour averaged, or use EC's full gauge projection, so that each has zero first jet at identity. Define
\[
 Q_{n,2}(u)=\frac12D_u^2F_{n,2}(e^{g_2u})\big|_{u=0}[u,u],
 \quad B_2=M_2g_2^2,
 \quad \rho=g_3/g_2,
 \quad B_3=\rho^2B_2.
 \tag{SC.6}
\]
The notation on the right means the quadratic Taylor polynomial in the normalized variable u. In particular its coefficient norm is \(O_L(B_2)\). The physical constant c is not included in this bound because it has no field jets.

The same proof applies to this actual mark minus a fixed gauge-invariant Wilson counterterm whose quadratic coefficient is \(O_L(B_2)\). That is a subtraction from the observable with its stated coefficient, not a change of the conditional law or of a running coupling.

## 2. An exact physical-coordinate form of the outer conditional

Let \(\Xi(W,B)\) be the source's exact constrained reconstruction from the independent **physical** Lie-algebra coordinates B on the next-average fiber. It includes the fixed-target exceptional solve and the specified averaged-gauge representative. Thus
\[
 \Psi_W(c)=\Xi(W,g_2c),\qquad V_*(W)=\Xi(W,0).
 \tag{SC.7}
\]
The map \(\Xi\) itself is a function of physical coordinates. The explicit \(g_2\) in (SC.7) is their normalization. It is not a new source-dependent map.

Let \(\mathscr G_W(\Xi(W,B))\) be the complete physical soft-gauge potential, with the source's positive fixed normalization absorbed into it. It vanishes, together with its first fiber derivative, at \(V_*(W)\). Its quadratic is the full averaged sampler from TC.7. Let \(\mathfrak J(W,B)\) be the complete Haar, nonlinear averaging and exceptional-bond coarea density after the common coordinate power \(g_2^d\) has been removed. Here d is the number of independent real coordinates. All these factors are retained; the removed common power and any retained-only factor multiply both numerator and denominator of the conditional.

With the exact auxiliary product domain
\[
 \chi_P(c)=\prod_{e\ {\rm free}}\mathbf1_{\{|c_e|\le P_2\}},
 \tag{SC.8}
\]
the actual conditional may be written
\[
 q_{2,A,W}H
 =\frac{\int dc\,\chi_P(c)D_1(c;W)H(\Xi(W,g_2c))}
        {\int dc\,\chi_P(c)D_1(c;W)},
 \tag{SC.9}
\]
where, up to a common constant that cancels exactly,
\[
\begin{split}
 D_1(c;W)={}&\frac{\mathfrak J(W,g_2c)}{\mathfrak J(I,0)}\,
 \exp\bigl\{-g_1^{-2}[\mathscr S(\Xi(W,g_2c))-\mathscr S(V_*(W))]\\
 &\hspace{21mm}-g_2^{-2}\mathscr G_W(\Xi(W,g_2c))\\
 &\hspace{21mm}+\mathscr E(\Xi(W,g_2c))-\mathscr E(V_*(W))\bigr\}.
\end{split}
 \tag{SC.10}
\]
This is TC.6 before its quadratic and remainder are separated. The constant \(\mathfrak J(I,0)\) is positive in the real chart and only sets the flat measure convention. If a zero-fluctuation Jacobian is assigned instead to TC's retained prefactor \(C_2(W)\), multiplication of numerator and denominator by that same factor recovers (SC.10). The full density retains \(C_2(W)\), including its classical background action and previous normalization. Its cancellation in a conditional ratio does not remove it from that density.

The source derivation is CMP109, printed pp.265--268, (2.3)--(2.13): the full nonlinear constraint is solved before the physical fluctuation is scaled, the constraint-force term occurs in its quadratic form, and the inherited action is evaluated on the actual minimizing-field response. The old selector is redundant on the admitted fiber as in BA/TC. Outside that admitted region the displayed smooth coefficient family is used only as its already constructed analytic continuation.

## 3. The exact dilation family

It is convenient to use \(b=\rho a\), so that the final physical link is
\(W=e^{g_3a}=e^{g_2b}\). For a complex scalar t set
\[
 W_t(b)=e^{t g_2b},\qquad
 V_t(b,c)=\Xi(W_t(b),t g_2c),\qquad
 V_{*,t}(b)=\Xi(W_t(b),0).
 \tag{SC.11}
\]
For \(t\ne0\) define
\[
\begin{split}
 D_t(c;b)={}&\frac{\mathfrak J(W_t,tg_2c)}{\mathfrak J(I,0)}\,
 \exp\bigl\{-t^{-2}g_1^{-2}[\mathscr S(V_t)-\mathscr S(V_{*,t})]\\
 &\hspace{21mm}-t^{-2}g_2^{-2}\mathscr G_{W_t}(V_t)\\
 &\hspace{21mm}+\mathscr E(V_t)-\mathscr E(V_{*,t})\bigr\},
\end{split}
 \tag{SC.12}
\]
and use the **same** domain (SC.8) and the exact denominator
\[
 Z_t(b)=\int dc\,\chi_P(c)D_t(c;b).
 \tag{SC.13}
\]
Only the outer classical and soft-gauge physical terms have the displayed \(t^{-2}\) prefactor. The whole inherited radiative action \(\mathscr E\), including its earlier determinant and counterterm pieces, is kept as the fixed actual function and is evaluated at the dilated physical arguments. It is **not** multiplied by \(t^{-2}\). All Jacobian and coarea factors are evaluated at those same arguments. In a derivation starting with physical-coordinate volume, the factor \(t^d\) is common to numerator and denominator and is canceled before defining the holomorphic family (SC.12).

This is an auxiliary interpolation of one fixed physical conditional. At t=1 it is exactly that conditional. The supplied couplings and the inherited action are never retuned. The ratio \((g_2/g_1)^2\) in its limiting classical precision is therefore still the literal one. Any constant used to normalize the original soft-gauge insertion is also common to numerator and denominator, and cancels before (SC.12); it is not a new analytic assumption about that constant at t=0.

### Lemma SC.1 — the removable flat endpoint

The density in (SC.12) has a holomorphic extension to t=0, and
\[
 D_0(c;b)=e^{-\frac12c^{\mathsf T}K_0c},\qquad
 K_0=K_2(I)
 =\mathsf C_0^*\{(g_2/g_1)^2\Delta_{2,\mathrm{cl}}(I)
             +c_{\mathrm{gf}}\tau_0^*\tau_0\}\mathsf C_0.
 \tag{SC.14}
\]
The limiting density and its domain are independent of b. The covariance of this Gaussian is the inherited constrained Schur covariance. It is not the bare one-step Wilson covariance.

**Proof.** Let H be the derivative at identity of \(W\mapsto V_*(W)\), expressed in link-angle coordinates, and let \(\mathsf C_0\) be the derivative of \(B\mapsto\Xi(I,B)\). Analyticity of the actual maps gives
\[
 \log V_t(b,c)
   =t g_2(Hb+\mathsf C_0c)+O_L(t^2g_2^2(\|b\|+\|c\|)^2).
 \tag{SC.15}
\]
The criticality of \(V_*(W_t)\) holds on the exact nonlinear fiber at every t. The first classical fiber variation therefore vanishes before expansion in t. The quadratic is the constrained Hessian, including the multiplier paired with the second derivative of the constraint. Its flat mixed pairing between the minimizing lift Hb and the constraint tangent \(\mathsf C_0c\) is zero. Consequently
\[
 g_1^{-2}[\mathscr S(V_t)-\mathscr S(V_{*,t})]
  =\frac{t^2}{2}c^{\mathsf T}
       \mathsf C_0^*(g_2/g_1)^2\Delta_{2,\mathrm{cl}}(I)
        \mathsf C_0c+O(t^3).
 \tag{SC.16}
\]
The full averaged soft gauge has zero background value and zero first fiber derivative. Its quadratic gives the second term in (SC.14), also with a factor \(t^2\). This uses the actual nonlinear sampler and exceptional solve; dropping their second derivatives would not reproduce the constrained Hessian away from flat background.

The inherited difference tends to zero because both its arguments tend to I. The normalized complete Jacobian tends to one. Thus both apparent \(t^{-2}\) singularities are removable, and their limits are independent of b. This proves (SC.14). TC.8 and the actual source gap bound this precision above and below. \(\square\)

The complete real Haar variables associated with the preimage gauge may be integrated out here because \(F_{n,2}\) is gauge invariant; they have their source-normalized mass. This does not remove the Haar density or coarea factors already present in \(\mathfrak J\).

## 4. Actual small interaction bounds on a large t-disc

Choose \(P\ge\max(1,P_2)\) with the actual source polylogarithmic growth. We evaluate coarse b in a ball \(\|b\|_\infty\le P\), and use a fixed multiple of this ball for Cauchy estimates. Put
\[
 \eta=C_L\{g_2P^3+(1+E_2)g_2P\}.
 \tag{SC.17}
\]
The fixed constant is chosen below once, to include the finite-depth maps, bounded adjacent coupling ratios and strict carrier margins. For weak coupling \(\eta\to0\). Merely having \(g_2P\to0\) would be insufficient.

### Lemma SC.2 — an actual jointly analytic normalized family

For a fixed sufficiently small c and
\[
 R=c/\eta>2,
 \tag{SC.18}
\]
the complete third smooth component family and its normalized local marked insertions are jointly holomorphic for \(|t|<R\), \(\|b\|_\infty<4P\). Their ordinary carrier bounds have strict margins independent of the volume. They use exactly (SC.12)--(SC.13).

**Proof.** Since \(|t|g_2P\le c/[C_L(P^2+1+E_2)]\), every complete physical input lies in a fixed smaller tube. PJ's physical raw admission, TC's actual force-containing minimum and the finite-depth inherited action apply uniformly. This remains true for all common component restrictions; a new independent reference is not selected after a decoupling.

Separate the flat precision in (SC.12):
\[
 D_t(c;b)=\exp[-\tfrac12c^{\mathsf T}K_0c+\mathcal V_t(c;b)].
 \tag{SC.19}
\]
The actual localized envelope of \(\mathcal V_t\), on the capped coefficient domain, is at most \(C|t|\eta\). To verify this, the complete constrained precision changes from \(K_0\) by \(O_L(|t|g_2P)\). Its quadratic contribution on \(|c|\le P\) is \(O_L(|t|g_2P^3)\). The physical classical fiber remainder begins at order three; after the \(t^{-2}g_1^{-2}\) factor its cubic term has the exact prefactor \(t g_2^3/g_1^2=t(g_2/g_1)^2g_2\). The gauge cubic term has its own \(tg_2\) prefactor. Higher terms are bounded by a convergent geometric series in \(|t|g_2P\). The inherited action difference is bounded by \(C_LE_2|t|g_2P\) from its fixed physical analytic class. The complete log Haar/coarea density contributes at most \(C_L|t|g_2P\). These are the terms in (SC.17); none has a surviving negative power of t or of the integrating coupling. Native coefficient localization and PJ's supported substitutions give these bounds before absolute summation.

If the Gaussian normal form is first written with its actual varying precision \(K(W_t)\), its inverse and determinant are continued together. Rewriting it as (SC.19) is the exact identity
\[
 d\mu_{K(W_t)}(c)
  =\left(\frac{\det K(W_t)}{\det K_0}\right)^{1/2}
       e^{-\frac12c^{\mathsf T}(K(W_t)-K_0)c}d\mu_{K_0}(c).
 \tag{SC.20}
\]
The determinant ratio cancels only as the common outer conditional normalization; earlier determinants remain inside \(\mathscr E\). The same precision supplies the quadratic and the determinant in every component. Its complex comparison costs are \(e^{C|t|g_2P\,r}\) for local rank r, with one fixed positive Gaussian reserve. Ordinary ranks are bounded by fixed-buffer carrier volume. Choosing c small pays these costs in the strict spatial margin. No hard-Q cores enter this family.

The fixed-P failures have their usual Gaussian-small fugacities \(Ce^{-c_0P_2^2}\). The original P domain is never allowed to vary with t or b. The complete ordinary vertex activities are bounded by \(C|t|\eta\), and the failure activities are small at the source radii. CMP116's component construction therefore has a strict common KP margin throughout the disc. Its exact denominator is (SC.13). CN's root-deletion identity and formula (CN.11) cancel the same unmarked components, including their covariance, determinant, Jacobian and supports. They give a nonzero normalized local analytic family, without a lower bound on the probability of a whole-volume P event.

Analytic coefficient caps, when used to extend an ordinary Gaussian coordinate outside the fixed P domain, are chosen real, independent of t and b, and equal to identity on the full physical domain. They do not alter (SC.9) or its domain. The proof keeps all complete old inputs and old normalizers inside the incoming \(F_{n,2}\) and \(\mathscr E\); it does not integrate an old copy with an extra parent quadratic store. This establishes the joint family. \(\square\)

## 5. A removable source and an exact parity identity

For \(t\ne0\) set
\[
 H_{n,t}(b,c)=t^{-2}[F_{n,2}(V_t(b,c))-F_{n,2}(I)],
 \tag{SC.21}
\]
\[
 \mathcal F_{n,t}(b)
    =Z_t(b)^{-1}\int dc\,\chi_P(c)D_t(c;b)H_{n,t}(b,c),
 \qquad
 \widehat{\mathcal F}_{n,t}(b)=\mathcal F_{n,t}(b)-\mathcal F_{n,t}(0).
 \tag{SC.22}
\]
The source has a removable value at t=0 because its first raw jet vanishes. From (SC.5), (SC.15) and physical Cauchy,
\[
 \|H_t\|_{\kappa,\mathrm{root}}\le C_LB_2P^2
 \quad (|t|<R,\ \|b\|_\infty<4P).
 \tag{SC.23}
\]
The \(t^{-2}\) in this bound is canceled before estimating. Equivalently integrate the physical second derivative of \(F_{n,2}\) along the segment from I to \(V_t\); each of its two arguments is \(O(|t|g_2P)\). The complete carrier substitutions have the same strict rate loss as in PJ.

Insert (SC.21) with a local source circle of radius \(c/(B_2P^2)\) into the family of Lemma SC.2. CN's same-gas normalized root bound gives
\[
 \sup_{|t|<R}\|\widehat{\mathcal F}_t\|_{\kappa,4P}
      \le C_LB_2P^2.
 \tag{SC.24}
\]
This is an anchored carrier estimate, not an extensive-source estimate. It keeps every normalization connector. At \(\alpha=0\) all these field-subtracted functions are zero.

### Lemma SC.3 — parity and the flat Gaussian expression

The exact identities are
\[
 D_{-t}(c;-b)=D_t(-c;b),\qquad
 H_{n,-t}(-b,c)=H_{n,t}(b,-c),
 \tag{SC.25}
\]
and consequently
\[
 \widehat{\mathcal F}_{n,-t}(-b)=\widehat{\mathcal F}_{n,t}(b).
 \tag{SC.26}
\]
At the flat endpoint,
\[
 \widehat{\mathcal F}_{n,0}(b)=Q_{n,2}(Hb).
 \tag{SC.27}
\]

**Proof.** In (SC.11), changing \((t,b,c)\) to \((-t,-b,-c)\) leaves the retained physical links and the physical independent fluctuation unchanged. Therefore it leaves the exact reconstruction, every force and target, the inherited action, the Haar/coarea density and the averaged soft gauge unchanged. Both explicit \(t^{-2}\) factors are even. This proves (SC.25) directly from (SC.12) and (SC.21), without an assumption about analyticity or parity of any running coupling. The old radiative action is the same fixed function on the identical physical field. The fixed domain (SC.8) is invariant under \(c\mapsto-c\), whose real integration Jacobian has absolute value one. Hence the exact denominators transform in the same way, and (SC.26) follows.

At t=0 Lemma SC.1 gives a law and a fixed domain independent of b. It is centrally symmetric even though a product-P truncation generally changes its covariance. By (SC.15),
\[
 H_{n,0}(b,c)=Q_{n,2}(Hb+\mathsf C_0c).
 \tag{SC.28}
\]
The mean of c is zero. Thus its mixed term has zero expectation and its purely fluctuating quadratic term is a constant independent of b. Subtracting the same expectation at b=0 removes that constant exactly, proving (SC.27). This is why no additive Gaussian-tail error is required for the vacuum-subtracted quadratic transfer. The failure tails are still required to obtain the uniform analytic coefficient bound in Lemma SC.2. \(\square\)

For coefficient norms use a parity-compatible representation. If \(f_{n,X}(t,b)\) are complete scalar coefficients for (SC.22), replace them by
\[
 \frac12\{f_{n,X}(t,b)+f_{n,X}(-t,-b)\}.
 \tag{SC.29}
\]
The normally convergent physical sum is unchanged by (SC.26). Complete supports and anchors are unchanged, the norm does not increase, and every coefficient Hessian at b=0 is even in t. This explicit projection is necessary: parity of a total sum alone would not justify coefficientwise cancellations inside an absolute carrier norm. It is applied only to complete scalar coefficients, not to overlapping factors of an unnormalized integrand.

## 6. The actual comparison theorem

For a coefficient family use the anchored physical carrier norm of PJ. Fixed spatial moments can be inserted by a strict further rate loss. First derivatives are summed over the complete raw determining lists with deterministic Cauchy envelopes. Let the coarse field lie on the actual admitted small-link slice, and choose P so that \(\|\rho a\|_\infty\le P\). The larger complex ball used above is the coefficient continuation, not an assertion about retained selectors there.

### Theorem SC.4 — nonlinear scalar comparison and two-power Hessian comparison

There is a supported representation of the actual third smooth mark for which
\[
 \Phi_{n,3}(e^{g_3a})-\Phi_{n,3}(I)
       =Q_{n,2}(\rho Ha)+\mathcal R_{n,3}(a),
 \tag{SC.30}
\]
and
\[
 \|\mathcal R_3\|_{\kappa,P}
       \le C_LB_2P^2\eta,
 \qquad
 \|D_a\mathcal R_3\|_{\kappa,P}
       \le C_L\rho B_2P\eta.
 \tag{SC.31}
\]
At the flat field the stronger bound is
\[
 \boxed{\quad
 \sup_n\sum_{X\ni n}e^{\kappa n(X)}
  (1+\operatorname{diam}(X)^s)
  \sum_{d,e}|D_{a_d}D_{a_e}\mathcal R_{n,X}(0)|
       \le C_{L,s}B_3\eta^2 .\quad}
 \tag{SC.32}
\]
This holds for every fixed moment order s. The leading small factor is of order \(g_2^2P^6\), with the explicit additional \((1+E_2)\) terms in (SC.17). No term of order \(g_2P^3\) survives in the Hessian comparison.

**Proof.** At t=1, (SC.22) is precisely the actual mark minus its value at identity; its incoming constant cancels. Equation (SC.27) identifies the t=0 expression. Apply one-variable Cauchy to (SC.24): the coefficient series of \(\widehat{\mathcal F}_t-\widehat{\mathcal F}_0\) starts at t, so its value at t=1 is bounded by \(C_LB_2P^2/(R-1)\). Cauchy on a smaller b polydisc gives an extra factor \(P^{-1}\) per direction. The number of directions and each fixed spatial moment are polynomial in the complete carrier size and are paid by a strict rate margin. Since \(D_a=\rho D_b\), this proves (SC.31) with the literal normalization ratio.

Now let \(J_{n,X}(t)=D_b^2\widehat{\mathcal F}_{n,X,t}(0)\), in the representation (SC.29). The same b Cauchy estimate bounds its summed-coordinate and fixed-moment norm by \(C_LB_2\) for all \(|t|<R\). It is even in t. Therefore its difference at one and zero is bounded by the geometric even series
\[
 \|J(1)-J(0)\|_{\kappa,s}
  \le C_LB_2\sum_{j\ge1}R^{-2j}
  =\frac{C_LB_2}{R^2-1}
  \le C_LB_2\eta^2.
 \tag{SC.33}
\]
Multiplying the two coordinate derivatives by \(\rho^2\) gives (SC.32). This argument uses the actual normalizer at every t, so it also controls the effect of the interacting denominator on the Hessian. No term is discarded because it is a vacuum term until the explicit subtraction in (SC.22). \(\square\)

The first-current bound in (SC.31) is for the actual composite raw variation of the smooth output. It includes variation of the inherited observable, reconstruction and new normalized kernel. Cauchy envelopes also bound its prescribed finite normalized paths in the buffered slice. The theorem does not assign a contraction separately to the original microscopic/background/old-kernel/current-origin labels. The parity projection is a scalar representation choice and does not by itself prove those separate labelled bounds.

## 7. Consequence for an actually interacting irrelevant Hessian

Apply the theorem to the actual incoming mark after its fixed local Wilson subtraction. Let its summed incoming quadratic kernel be \(K_{2,\mathrm{irr}}\), with the Maxwell coefficient removed by WQ/NW. The subtraction uses the full gauge-invariant Wilson density, so the physical input remains gauge invariant. The actual output is gauge invariant as well. Its summed Hessian, and the Gaussian lift of the incoming Hessian, obey the linear Ward identity; their difference does too.

The map H in (SC.15) is the derivative of the actual two-level constrained minimum followed by one more average. In curvature it is exactly FH's inherited minimizing lift with b=2. Scaling the classical action by the positive factor \((g_2/g_1)^2\) leaves this minimizing lift unchanged. The full averaged-gauge representative may add a gradient, which is annihilated by the Ward kernel. Thus FH, including its inherited Schur shape, applies to the first term in (SC.30).

For the small difference kernel, (SC.32) gives the weighted coefficient and moment bound. WQ's quadratic Ward estimate, with its Maxwell part retained when bounding the whole difference, bounds its quadratic form by \(C_LB_3\eta^2Q_W(a)\). Full hypercubic and reflection covariance are those of the actual SW maps, the fixed product balls, and the fixed Wilson subtraction. On the infinite lattice, using SW's embedded-tag limit of the actual coefficient family, one obtains
\[
 \left|\frac12D_a^2\sum_n\Phi^{\mathrm{irr}}_{n,3}(I)[a,a]\right|
 \le
 \left\{C\rho^2L^{-2}\|K_{2,\mathrm{irr}}\|_{\mathrm{Ward}}
              +C_LB_3\eta^2\right\}Q_W(a).
 \tag{SC.34}
\]
The norm in the first term is the exponential/moment norm required in WQ and FH. It is an input norm of the actual incoming quadratic kernel, not a bare-coarse-Wilson substitution. Fixed source and trace conventions must be the same on both sides, as in FH.1.

Equation (SC.34) is a genuine one-step interacting quadratic estimate. For a fixed choice of L the second term is made arbitrarily small by weak coupling; the Gaussian term retains the two spatial powers. It is not a claim that an arbitrary complete nonlinear marked field already satisfies the curvature-energy norm in M04. In particular a scalar small-link value error does not automatically give a native curvature-regulator estimate on all holonomy sectors.

The finite-volume statement needs its usual topology qualification. Periodizing the infinite-lattice Ward kernels preserves (SC.34). The actual torus kernels need not equal those periodizations: SW controls the remaining winding tags exponentially in the shortest period, rather than setting them to zero. In particular a winding holonomy Hessian can be nonzero on a constant link field while its lattice curl is zero. Thus (SC.34) is not asserted without that explicit winding remainder on arbitrary finite tori. The actual finite-volume supported comparison (SC.30)--(SC.32) remains valid; converting it to a pure curvature seminorm is precisely where this qualification enters.

## 8. Scope and remaining gates

The proof uses the actual third smooth conditional, the fixed two-level incoming analytic action and the actual twice transported microscopic source. It introduces no assumed fourth action and no generic hypothesis equal to the desired transfer estimate. The source coefficient \(\beta_0\), the output ratio \(g_3/g_2\), the classical ratio \((g_2/g_1)^2\), all inherited normalization factors, the full constraint force and the averaged soft gauge remain explicit.

The following tasks are separate.

* A support-preserving gauge-invariant completion can transfer the small-link Taylor information to portions of the native weak-curvature class. Its topology, large-carrier and energy-footprint estimates must be proved in their own right. Flat torus holonomies cannot be removed by assuming a global small-link gauge.
* Moving hard-Q core integrals are not the fixed symmetric product domain (SC.8). Their boundary currents and their interacting comparison are not proved by this dilation argument.
* The output current estimate here is a composite derivative. M04's separately retained physical origins require their own estimates; scalar parity does not distribute itself across an arbitrary preassigned split.
* Constants and spare carrier margins in this note are fixed-depth constants. An all-depth inductive budget, including radiative marginal extraction and the complete native nonlinear source norm, remains open.

Primary inputs: CMP109 (2.3)--(2.13), CMP116 Lemmas 1--2 and (2.5)--(2.26), with restoration of the Gaussian normalization on printed pp.21--22; the literal fixed-depth constructions BA, TC, TR and SW; PJ's actual physical source tubes and jets; EC's complete scalar projection; CN's exact same-gas normalization; and the WQ/FH quadratic statements.
