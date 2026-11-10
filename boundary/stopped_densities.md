# Stopped densities and projective comparison

**Composed-response hypothesis (CR).** Each complete boundary conclusion below assumes the displayed native-chart and spatial response estimates for the actual iterated reconstruction, with the prescribed earlier innovations and raw variables fixed, uniformly over the admitted histories. A sufficient estimate for the latent contribution is (A.8) in [Conditional-law estimates and the continuum application](../continuum/conditional_to_continuum.md), refined for the anchored exterior derivative in PG.18–PG.20. The two endpoint bounds concern the identical Wilson-subtracted primitive, its actual cutoff and its independently extended current. A direct minimizing-field derivative alone does not establish this hypothesis. The application to every required original Wilson history remains open. Complete boundary estimates and their C06/C08 applications in this chapter are conditional on CR and the other displayed source, AF, domain and support assumptions. Exact density identities and abstract inequalities retain their individually stated hypotheses.

In the projective density formulation, a sufficient comparison is
\[
 \sup_{\zeta,x,a}\left|
 \log\frac{W_\zeta(x,a)W_0(x,a_*)}
               {W_0(x,a)W_\zeta(x,a_*)}
 \right|\le\delta_r<\pi/2,
\]
on the stipulated chart with the required uniform rates and actual fixed support. The composed ordinary response is the unresolved input in its derivation. The exact partial-gauge transport and the surviving fixed-exterior derivative are given in the chapter [Gauge covariance of partial integrals and exterior scores](../continuum/partial_gauge_transport.md), equations PG.2–PG.6 and the subsequent anchored-score criterion.

**Scale convention.** The Ward estimate uses the evaluation age $n-b$. When $b\le n<j$, one also needs decay in the forcing age $j-n$. The latter response for the actual composed field, with earlier innovations fixed, is conditional on CR. The two-age interpolation SR.12–SR.24 is used here in place of the one-age calculation of OR.19.

This note distinguishes algebra proved below from the primary-source facts checked directly. The companion rooted-load calculation supplies the source-specific incoming incidence estimate, and [Compatibility of normalized densities and geometric roots](density_root_compatibility.md) records its independent comparison with this density construction. Previous PASS labels are not premises.

The principal improvement over [ND.14–ND.27](primitive_estimates/native_domain_count.md) is to estimate a **projective logarithmic difference of the actual density**, after unrolling the current attempt and before fixing any of its earlier raw coordinates. This retains the moving normalizers exactly. Completed relative inputs need no third analytic radius: their incoming, running AF capacity tail makes their entire anchored response small on the radius already maintained.

## 1. Variables and the exact object

Fix an admitted outer history, an eligible component P at outer scale r, a branch on which its preliminary integration stops, and its actual free-coordinate presentation. Write h=r−N_r. The earlier/exterior tuple x includes every raw coordinate not being integrated in the operation under consideration, the deep T_h variables, and the already selected external discrete history. It is fixed before normalization.

Write a for the coordinates actually integrated by that stopped operation. At a fixed earlier history and fixed stopping branch, the source's simple last-N prefix has no hidden history sum from T_h: that earlier operation is fixed, and the current branch is fixed. If an implementation does genuinely sum an internal discrete label in this operation, it is part of a and its weight is retained. A term depending on such a label is not an external scalar, and the removed scalar in (SD.7) must be common to all those labels. All assertions below are on the actual selector support S_x after the source's changes of variables; no enlargement of the real support is made.

The density to be controlled is

\[
 p_\zeta(a\mid x)
 =\frac{W_\zeta(x,a)}{Z_\zeta(x)},\qquad
 Z_\zeta(x)=\int_{S_x}W_\zeta(x,a)\,m_x(da).
 \tag{SD.1}
\]

Here ζ denotes the native background, independently extended current and the permitted new localization variables. The measure m_x is fixed and positive. Any native-independent positive raw multiplier is included in m_x, even if it varies with a. This does not remove it from the law: it changes both the numerator and the normalizer in (SD.1). The mass Z_ζ and any scalar extracted from W_ζ remain in the scalar-action decomposition.

The only factors that can be canceled before forming (SD.1) are factors independent of **every** integrated coordinate and every internal summed label. A factor can depend on ζ and x and cancel from p, but its ζ derivatives then remain in the physical mass.

## 2. Exact cancellation of current-attempt intermediate masses

This calculation precedes all raw conditioning. It explains why an estimate for a post-integrated C coefficient cannot be substituted for an estimate of a density at fixed earlier raw variables.

Let the unrolled density for the current attempt be

\[
 M_0(\zeta;a_0,\ldots,a_{s-1},y).
\]

All selectors, coarea/Haar factors, Gaussian factors, incoming action terms and archived raw multipliers are included. The tuple y contains the variables left after this finite attempt. On a fixed selector branch define the successive unnormalized marginals by the literal integrations

\[
 M_{j+1}(\zeta;a_{j+1},\ldots,y)
 =\int M_j(\zeta;a_j,a_{j+1},\ldots,y)\,da_j.
 \tag{SD.2}
\]

Whenever these masses are nonzero, define the normalized kernels

\[
 k_j(\zeta;a_j\mid a_{j+1},\ldots,y)
 =\frac{M_j(\zeta;a_j,a_{j+1},\ldots,y)}
        {M_{j+1}(\zeta;a_{j+1},\ldots,y)}.
 \tag{SD.3}
\]

Then, as an identity of functions on the joint support,

\[
 M_s(\zeta;y)\prod_{j=0}^{s-1}k_j(\zeta;a_j\mid a_{j+1},\ldots,y)
 =M_0(\zeta;a_0,\ldots,a_{s-1},y).
 \tag{SD.4}
\]

Every denominator M_{j+1} cancels its identical occurrence in the next numerator. This is an algebraic cancellation before integration; it does not depend on independence, Gaussianity, positivity or a bound on the kernels. If the intermediate masses have not yet been proved nonzero on a complex chart, the equality is first used on the real positive slice and then for the original unnormalized expressions; no zero-free claim is inferred from the notation alone.

An extracted Wilson correction or other scalar in the source definition of C is included in the definition of the corresponding M_j. Restoring its opposite action factor makes (SD.4) literal. One must not cancel the logarithmic partition term while forgetting its matching Wilson or vacuum term.

Now fix any selected earlier raw tuple x among (a_0,…,a_{s−1},y), and integrate the remaining tuple a. Substitution into (SD.4) is legitimate pointwise, and the actual conditional density is

\[
 p_\zeta(a\mid x)
 =\frac{M_0(\zeta;x,a)}{\int M_0(\zeta;x,a')\,da'}.
 \tag{SD.5}
\]

The intermediate M_j have canceled as functions. The final stopped mass M_s has **not** been discarded: it is part of the exact product before the cancellation. If it depends on a variable still integrated after conditioning, it contributes to (SD.5); if it depends only on the fixed exterior tuple, it cancels from the conditional quotient and stays in the external mass. This rule also applies to any older archived mass. It is not permissible to cancel a mass solely because it was once called a normalization.

For comparison, differentiating the uncanceled product gives

\[
 D\log M_s+\sum_{j=0}^{s-1}D\log k_j=D\log M_0.
 \tag{SD.6}
\]

Thus cancellation removes no normalization derivative. It identifies exactly where those derivatives occur in the direct density.

### Consequence for the induction

The completed-relative contribution in the unrolled density is the **incoming relative action evaluated once on the full coordinate tuple**. New C_k^(n) terms created earlier during this same attempt are not separate incoming actions. They arose from the masses in (SD.2); reopening them as separate atoms while retaining the normalized kernels would count the same action twice. Older C terms inherited from preceding attempts remain incoming terms and retain their actual source labels and native charts.

This distinction permits a stopped-density estimate using the incoming capacity at r−1. It does not require an unproved bound for outgoing relative C terms from an intermediate stage of the very attempt being estimated.

### 2.1 Identification with the literal source operation

The generic symbols in (SD.2) can be matched to the printed one-step identity, rather than postulated for some replacement kernels. Let I_(n+1) denote the complete fluctuation integral called “the ∫ in (1.60)” in LFR I (1.62), with its printed A_j and B_j integration factors, its free-coordinate measures and z^(j) normalization. Keep the printed E_0^(j) and the corresponding vacuum/normalization update in their actual action positions. Write t_n=(g_k^(n)(·))^(−2) for the spatial coupling coefficient in the n-th effective Wilson action. Equation (1.62) states

\[
 C_k^{(n+1)}
 =\log I_{n+1}
   +A(t_{n+1}-t_n,U_k^{(n+1)}).
 \tag{SD.6a}
\]

Since the Wilson action is linear in its coefficient,

\[
 -A(t_{n+1},U_k^{(n+1)})+C_k^{(n+1)}
 =-A(t_n,U_k^{(n+1)})+\log I_{n+1}.
 \tag{SD.6b}
\]

On the other hand, (1.60) extracts the old E+R+B+B^(n) action at the same reference configuration U_k^(n+1), A_j=0. The exponent inside I_(n+1) contains its complete difference from the old action at the actual pulled-back field

\[
 U_k^{(n)}
 \!\left(\exp i[g_jCB_j-h\widetilde D(g_jCB_j)]V^{(j)}\right),
 \tag{SD.6c}
\]

and the displayed Wilson-coupling-difference subtraction. Thus the extracted action plus those differences is exactly the old action at the pulled-back argument. Equations (SD.6a)–(SD.6b) restore precisely the old Wilson coefficient. The P^(j), Gaussian, coarea/Haar and relocation terms are the remaining pieces of the exact change of variables. No factor from E_0^(j), z^(j), a gauge/coarea measure or a hard selector is being silently discarded.

In full-density notation, if Φ_j is this actual change of variables and J_j its actual density/Jacobian factor, the source one-step equality says

\[
 W_{j+1}(\zeta;y_{j+1})
 =\int J_j(\zeta;a_j,y_{j+1})\,
       W_j(\zeta;\Phi_j(a_j,y_{j+1}))\,da_j.
 \tag{SD.6d}
\]

All printed factors that are not conveniently expressed as a smooth action stay in J_j or the fixed positive coordinate measure. Therefore the normalized source kernel is exactly

\[
 \kappa_j
 =\frac{J_j\,W_j\circ\Phi_j}{W_{j+1}}.
 \tag{SD.6e}
\]

Multiplying the nested kernels and the final W_s cancels each W_j at its *identical intermediate source field*. The result is the pullback of W_0 multiplied by the product of the actual Jacobians. This is (SD.4) in common coordinates. It is not an assertion that unrelated Gaussian localization families are inverses, nor an identification of different native charts.

Restricting to a fixed stopping branch does not alter this functional cancellation. Each selected characteristic is kept in the corresponding full density. An indicator depending only on the remaining source variables multiplies both the numerator and the denominator at that stage; an indicator on the integrated variables restricts that stage's actual integration support. On a failed relocation branch, (1.59) provides the fixed coordinate support together with its action response. After the coordinate presentation is fixed, the identical characteristic factors cancel only where the density is nonzero; elsewhere both sides have zero measure.

The source also explains why a hidden moving selector does not appear when the whole successful part of a prefix is unrolled. LFR I pp.181–182 states that after n integrations the remaining background selector is χ_k^(n), together with the unchanged deep selector. The earlier background selectors have been removed using the exact identity (1.29) on the new free-coordinate cutoffs. At the next stage χ_k^(n+1) is independent of that integration's variables. Hence the final stopping selector is external to the integrated successful prefix; the still-live deep and failed-coordinate cutoffs remain literal parts of S_x. None of these hard selectors is differentiated.

## 3. A projective comparison lemma that survives fixed conditioning

The following result is stronger than the scalar operator bound used in earlier notes. It is also simpler to apply than deriving common domination from a phase cone after normalization.

### Lemma SD.1 — centered logarithmic comparison

Let W_0(x,a)>0 on the fixed support S_x, and let W_ζ be holomorphic in ζ on that support. Suppose that for each fixed x there is a scalar c_ζ(x), independent of a, such that

\[
 W_\zeta(x,a)=W_0(x,a)
             \exp\{c_\zeta(x)+\sigma_\zeta(x,a)\},
 \qquad |\sigma_\zeta(x,a)|\le\delta<\pi/2.
 \tag{SD.7}
\]

Then the actual normalized density satisfies

\[
 p_\zeta(a\mid x)
 =p_0(a\mid x)
       \frac{e^{\sigma_\zeta(x,a)}}
            {\mathbb E_{0,x}e^{\sigma_\zeta(x,\cdot)}},
 \tag{SD.8}
\]

\[
 \left|\mathbb E_{0,x}e^{\sigma_\zeta}\right|
 \ge\cos\delta\,\mathbb E_{0,x}e^{\Re\sigma_\zeta}>0,
 \tag{SD.9}
\]

and

\[
 |p_\zeta(a\mid x)|
 \le M(\delta)p_0(a\mid x),\qquad
 M(\delta)=e^{2\delta}\sec\delta.
 \tag{SD.10}
\]

Moreover the total-variation norm of the normalized complex functional is at most sec δ. The common positive domination (SD.10), rather than that weaker scalar norm, is the assertion needed for a sum of analytic suprema.

**Proof.** Equation (SD.8) is exact. Since |Im σ|≤δ, all e^σ lie in the common sector of half-angle δ. Taking real parts after a single common rotation proves (SD.9). Dividing pointwise, and using e^(Re σ(a))/E e^(Re σ)≤e^(2δ), proves (SD.10). Integrating the sharper sector inequality proves the stated functional bound. No smoothness of a, convexity of S_x, independence or moment estimate has been used. ∎

The scalar c_ζ is not lost:

\[
 \log Z_\zeta(x)-\log Z_0(x)
 =c_\zeta(x)+
       \log\mathbb E_{0,x}e^{\sigma_\zeta(x,\cdot)}.
 \tag{SD.11}
\]

Every current or native derivative of c_ζ belongs to the mass/action estimate. Only normalized insertions are invariant under changing it.

A convenient choice is any actual-support anchor a_*(x):

\[
 c_\zeta(x)=
   \log\frac{W_\zeta(x,a_*)}{W_0(x,a_*)},
\]

\[
 \sigma_\zeta(x,a)=
 \left[\log W_\zeta(x,a)-\log W_\zeta(x,a_*)\right]
 -\left[\log W_0(x,a)-\log W_0(x,a_*)\right].
 \tag{SD.12}
\]

The anchor need not be zero. In a failed annular selector, zero may not belong to the support. This anchor only removes a scalar; it changes neither the support nor the source coefficient catalog.

### Lemma SD.2 — restriction, marginalization and disintegration

Suppose (SD.7) holds for a joint density W_ζ(x,a,b), with the same scalar c_ζ(x) for the variables being averaged. Fix x, restrict to any fixed measurable selector, and integrate b. The resulting density ratio has the exact form

\[
 \frac{p_\zeta(a\mid x)}{p_0(a\mid x)}
 =
 \frac{\mathbb E_{0}[e^{\sigma_\zeta}\mid x,a]}
      {\mathbb E_{0}[e^{\sigma_\zeta}\mid x]}.
 \tag{SD.13}
\]

Consequently (SD.10) still holds with the same M(δ). The proof uses the same sector bound in the denominator and absolute bound in the numerator. Thus fixed raw conditioning is harmless **when the initial estimate is pointwise on that fixed fiber**. A bound only for an already integrated signed functional is insufficient.

If the removed scalar is c_ζ(x,b), it must remain inside the conditional expectations in (SD.13). This is the exact obstruction to an unjustified branchwise cancellation of history-dependent masses.

### Positive catalog transfer

For any nonnegative parameter-independent weights w_G and any common label union with absent coefficients set to zero,

\[
 \sum_Gw_G\sup_{\zeta\in\mathcal D_+}
    \left|\int p_\zeta(a\mid x)F_G(\zeta,x,a)\,da\right|
 \le M(\delta)\int p_0(a\mid x)
       \sum_Gw_G\sup_{\zeta\in\mathcal D_+}|F_G(\zeta,x,a)|\,da.
 \tag{SD.14}
\]

The exterior tuple x is fixed on both sides; its supremum is taken afterward. This estimate is valid directly on the working + contour. It does not shrink that contour and does not put a separate raw supremum inside the sum.

## 4. Exact derivative formula: the extra covariance is retained

Let H_ζ=log W_ζ in any fixed branch. For a bounded insertion F, differentiating (SD.1) gives

\[
 D\Pi_\zeta F
 =\Pi_\zeta(DF)
  +\Pi_\zeta(F\,DH_\zeta)
  -\Pi_\zeta F\,\Pi_\zeta(DH_\zeta).
 \tag{SD.15}
\]

If F is fixed, the second and third terms form the complete covariance. A global norm bound for Π cannot justify deleting it or replacing it by an ordinary conditional Gaussian covariance.

Under (SD.7) the scalar derivative Dc_ζ cancels between the last two terms, so DH_ζ can be replaced there by Dσ_ζ. For a real interpolation t between two actual potentials, the exact response is

\[
 \Pi_1F-\Pi_0F
 =\int_0^1
  \left[\Pi_t(\dot F_t)+
   \Pi_t(F_t\dot H_t)-\Pi_tF_t\,\Pi_t\dot H_t\right]dt.
 \tag{SD.16}
\]

These identities are consequences of the quotient. They hold at every fixed x and retain the moving mass. They will be used with a graph-resolved score difference, not with a fictional Gaussian conditional law.

## 5. Primary-source checks for the actual stopped support

The following source pages are used.

| Source | Checked statement | What it licenses here |
|---|---|---|
| LFR I p.177, eligibility (i),(ii), and p.178, (1.2) | The component is bounded at the current and relevant predecessor scales; no new large-field regions occur in the preceding N grades; the last N factors have the simple one-step form. | The actual eligible prefix and its finite graded strip. It does not bound arbitrary ancestral branching. |
| LFR I p.179, (1.10)–(1.14) | Z''_j=Z_j for j≤h; only the strips Z_(j+1)\\Z''_(j+1) are integrated for h≤j≤r−1; the deep operation is preserved. | Deep earlier raw variables stay as fixed parameters in the stopped prefix. |
| LFR I p.182, (1.25) | The next background selector χ_k^(n+1) is independent of the next integration variables. Components with its large-field complement stop. | One must freeze the actual branch before analyticity arguments. |
| LFR I pp.187–188, (1.53)–(1.59) | The B change of variables is performed; on failed branches the selector is relocated to an expression independent of the background. The change produces action terms. | A fixed support is available only with the full relocation Jacobian/action response retained. |
| LFR I pp.188–189, (1.60) | The pre-integration action contains the full difference of E_k+R_k+B_k+B_k^(n), the exact quadratic forms, P^(j), and the difference of Wilson actions with the actual coupling difference. | Every term of the stopped density can be listed before integration. The inherited E bank is E_r, not E_j. |
| LFR I p.189, (1.61)–(1.63) | B_k^(n)=Σ_(i≤n) C_k^(i), and C_k^(n+1) is the logarithm of the literal integral plus its Wilson-renormalization correction. | Current-attempt C terms are intermediate masses in (SD.2)–(SD.4); older C terms remain incoming actions. |
| LFR I p.191, paragraph after (1.69) | The actual insertion sends the next modified native space into the preceding one. If integrations stop, the accumulated B_k^(n) is left among boundary terms. | Pointwise composition on the source native chart is available; stopping does not delete the accumulated action. |
| LFR I pp.191–192, discussion preceding (1.70) | The accumulating C terms enter the fluctuation difference with a g_j factor; at most N0 top strips overlap; N0 δ'_j≤4N0 δ'_r. | The relevant pre-integration estimate is a fluctuation difference; an extensive unsusbtracted C sum is not the right estimate. |
| LFR II pp.379–380, (1.73)–(1.75) | A literal completed kernel is compared pointwise to its positive real version by a uniformly small exponential σ; the whole old self action is included. | Genuine completed kernels and their fixed fibers have RN domination by Lemma SD.2. This is stronger than a scalar operator bound. |
| LFR II pp.391–392, (1.103)–(1.104) | Second-class masses are retained as raw multipliers τ_Y(V_b), alongside selectors and gauge factors; they depend only on the new raw field V_b on Y. | Such a factor is never discarded. It is native-independent if its raw argument is held fixed. No arbitrary complex raw extension of τ is supplied. |

### Archived raw multipliers: the exact scope of the simplification

The statement that a raw mass is native-independent must be checked at its actual argument. If it is τ_b(V_b) with V_b retained as a fixed raw variable, D_ζτ_b(V_b)=0. If a proposed coordinate map instead changes its argument to Φ_ζ(x,a), then

\[
 D_\zeta\log\tau_b(\Phi_\zeta(x,a))
 \tag{SD.17}
\]

cannot be set to zero, and cannot be bounded by a theorem about native analyticity at fixed raw input. In that case the proposed parameterization has not established the required density estimate.

### Lemma SD.3 — recent raw renewal is excluded from a source eligible segment

An archived second-class multiplier born at b inside an eligible P cannot have h<b≤r while being swept by the preliminary strip transformation. At b=h it belongs to the preserved earlier operation T_h.

**Proof.** At LFR II p.378 the construction introduces, component by component, the decomposition χ_b(X,6)+(1−χ_b(X,6)). It explicitly puts the second-class components Y back into the new large-field domain, retaining the large-field characteristic χ_b^c(Y,6). Equations (1.103)–(1.104) retain that characteristic together with the new multiplier τ_b(V_b); the normalization does not cancel it. This is an actual new large-field selector at operation b, independently of the older first-large-field index j(Y) used in the suppression decomposition.

LFR I p.178 derives the simple last-N product (1.2) from condition (ii), and states that no large-field characteristic functions occur in those last-N one-step factors. A retained second-class selector at h<b≤r contradicts this property. Equivalently, the alternative multiplication operation T_b(Y) cannot be rewritten as the unchanged simple segment from h through b while retaining its new selector. Thus the source eligible segment begins after that event. For b≤h the factor lies in T_h; (1.11) sets Z''_j=Z_j at all j≤h, so the preliminary operations leave it untouched. ∎

This argument uses the actual new selector and exact simple-factor identity, not a purported reset of the old first-large-field index. LFR II pp.385–386 separately shows why those notions differ: even when a geometric successor remains S(Z_0), a new large field introduced during preparation supplies a renewed suppression, while the oldest index can stay unchanged in the later merger formula.

Consequently a retained raw mass in the preserved operation remains at its actual fixed raw argument during the preliminary strip integrations. The final completed integration is handled by the source's pointwise σ theorem, not by analytically continuing that raw argument. A component with such a recent renewed selector is not selected for this simple r-prefix until the source eligibility conditions hold; it stays in the exact unselected operation. No shortened substitute preparation is asserted, and applying the printed simple-prefix operation to a different last-N factorization is not licensed by the source.

## 6. Ordinary action: the pre-integration logarithmic oscillation

Let H_ord denote the ordinary part of log W after the identity (SD.4). Remove only a scalar independent of all current integration variables. The source expression has the exact structure

\[
 H_{\mathrm{ord},\zeta}(x,a)
 =-q_\zeta(x,a)+P_\zeta(x,a)
       +\sum_\gamma G_\gamma(\zeta;x,a).
 \tag{SD.18}
\]

The quadratic q includes principal/Schur pieces, actual linear forces from fixed exterior coordinates and every retained cross term. P includes the nonlinear constraint/coarea/Haar factors, the classical Wilson remainder and failed-relocation terms. The G_γ are **pre-integration** scalar fluctuation differences of the complete E/R/B action, including older incoming C terms.

Choose the ordinary source profile α_j^(++)=ell_j^Q α_j^(+) once. It is used only for the independently controlled ordinary family. For each fixed real tuple (x,a), compose the literal source insertion maps before taking Cauchy estimates. LFR I's successive-insertion inclusion is the relevant admission statement. One does not infer analyticity in a raw coordinate that the source keeps merely measurable.

### 6.1 The regular E bank, including births later than the integration grade

At stage j the bank is the whole inherited E_r. Its fluctuation difference is exactly

\[
 E_r(U^{[j]}_\zeta(x,a))-E_r(U^{[j+1]}_\zeta(x,a)).
 \tag{SD.19}
\]

For the whole prefix these differences telescope in the literal order, retaining all own vacuum and Wilson subtractions. Terms depending on earlier current-attempt variables are not external scalars until all such variables have actually been fixed or integrated.

For births b≤j, the source nearby Ward calculation keeps a coefficient of derivative order p with its actual field degree d≥p. On the selected running radius this gives

\[
 C E_0(\alpha_b^{++})^{-p}(Q_j^{++})^d,
 \qquad 2\le p\le5,\quad d\ge p,
 \tag{SD.20}
\]

with the matched marginal term canceled before summing b. The single-age expression L^{−(5−θ)(j−b)}, 0<θ<1, requires the evaluation grade to equal j. In general the Ward gain uses n−b; use the two-age SR.12–SR.24 under CR for the missing j−n decay. The fifth-order tail has p=d=5; the Wilson subtraction has coefficient order two and its actual field degree. Replacing all denominators by the fifth power while retaining a quadratic numerator is invalid.

The AF comparison gives α_j^(++)/α_b^(++)≤C sqrt(1+j−b), with C depending on the one selected exponent but without a new running power proportional to Q. The near and far old-birth sums are thus bounded by

\[
 S_{\rm near}=\sum_{u\ge0}(1+u)^{b_*+5/2}L^{-(1-\theta)u},
\]

\[
 S_{\rm far}=\sum_{u\ge0}\sqrt{1+u}\,L^{3u}e^{-cML^u}.
 \tag{SD.21}
\]

These are the four-dimensional root counts performed **after** the source degree and map factors, not an extra unweighted fine-volume factor. Both sums converge.

The primary anchor is CMP116 Lemma 1, (1.33)–(1.36): it is a localized pre-integration fluctuation action on the joint native/current/B chart. CMP119 pp.275–277 transports it to the mixed actual layers. The running-radius decomposition, including its common-domain proviso, is spelled out in retained E14.33–E14.51. Its use here is restricted to this actual ordinary E family, not a synthetic coupling-inconsistent reset bank.

For b>j there are at most N_r relevant births. Each is retained as a whole proper-b primitive together with its own Wilson subtraction. Cauchy gives

\[
 |\beta_b|\le C E_0(\alpha_b^{++})^{-2}.
 \tag{SD.22}
\]

On one proper b-cell, the source curvature clause and the quadratic zero of the Wilson action give

\[
 |A(\phi_b,U;\text{one b-cell})|
       \le C(\alpha_b^{++})^2.
 \tag{SD.23}
\]

The number of fine plaquettes contributes (h_b/η)^4 and their squared curvature contributes (η/h_b)^4, so they cancel. Therefore |β_b A|≤CE_0 per b-cell. This is why no separate boundedness assumption β_b=O(1) is needed.

A genuine grade-j insertion is assigned to its actual j-cell. For b>j, that cell lies in a bounded number of proper b-cells. The remaining remote b-cells are summed with the actual normalized reconstruction row before positions are counted. Hence this branch costs C D_j per b, not D_j L^{4(b−j)}. Together with the at most N_r birth labels it contributes at most C N_r D_j to the ordinary oscillation bound. No birth j<b≤r has been omitted.

### 6.2 Boundary, older C, explicit and quadratic terms

CMP119 (2.41)–(2.42) supplies the ordinary B full-tree coefficient bound at fixed real raw data. An actual direct A_j slot forces a birth at least j+1. The source (1.63) labels an older C term by its integration and proper support grades; there are at most polynomially many such recent labels. Their rooted full-tree sums are performed before the finite coordinate count. Older native-response terms are treated by their actual reconstruction row and own-grade carrier; they are not counted as a full old fine lattice inside P.

LFR I (1.60) subtracts the reference action before integration. Therefore the accumulated C terms occur as fluctuation differences. The discussion on pp.191–192 supplies their small g_j insertion and controls the N0 overlapping top strips. The top-band factors L0^{O(N0)} are polynomial in R_r by the formula following (1.70). The exponent is fixed before Q is selected.

The exact Gaussian/coarea coefficient rows have fixed absolute native domains. At fixed actual cutoff tuple their complex coefficient changes are bounded by C α_r^(+) times a fixed polynomial. Each stage has D_j≤C(LMR_(j+1)+1)^4 actual free coordinates, with both A_j and B_j counted on the j mesh, and |a_j|≤P_j. Thus their summed projective logarithmic difference is bounded by C g_r ell_r^(d_1). Fixed exterior fields in the quadratic linear force remain in this estimate; they are not set to zero.

New complex localizers are outside the full protected collar. The source row change then has a genuine walk from an integrated endpoint to the complement of that collar. This supplies C g_r^(−u) ell_r^(d_3) exp(−cR_r) on the full chosen localization disks. No claim is made for arbitrary complex decouplings inside P.

### 6.3 Cauchy on the *projective* ordinary difference

For the actual-support anchor a_* define

\[
 D_{\rm ord}(\zeta;x,a)
 =H_{\mathrm{ord},\zeta}(x,a)-H_{\mathrm{ord},\zeta}(x,a_*).
 \tag{SD.24}
\]

The preceding local sums give, for the scalar terms on the admitted ordinary ++ contour,

\[
 \sup_{++}|D_{\rm scalar}(\zeta;x,a)|
       \le C(Q)\ell_r^{d_0}.
 \tag{SD.25}
\]

The exponent d_0 incorporates actual strip counts, actual recent labels and the top-band map polynomial. It is fixed before Q. This bound is for a pre-integration difference. A bound only for C_k^(n) after integration would not prove (SD.25).

On the finite window, ell_j/ell_r=1+O(1/ell_r), so for each chosen Q its power is bounded by a fixed constant after lowering the coupling ceiling. Cauchy along the common external native line, using the actual map margin, gives

\[
 |D_{\rm scalar}(\zeta;x,a)-D_{\rm scalar}(0;x,a)|
 \le C(Q)\ell_r^{d_2-Q}.
 \tag{SD.26}
\]

Combining the exact quadratic/explicit difference and the remote localizer estimate yields

\[
 |\sigma_{\mathrm{ord},\zeta}(x,a)|
 \le\delta_{\rm ord,r}
 :=C g_r\ell_r^{d_1}
    +C(Q)\ell_r^{d_2-Q}
    +C g_r^{-u}\ell_r^{d_3}e^{-cR_r}.
 \tag{SD.27}
\]

Choose Q>d_2+2, then the common ceiling. This is a bound on the full complex projective difference, not merely its imaginary part. It directly supplies RN comparison with the actual real-center density.

**Source-status qualification.** The algebra and summations above identify how to derive the estimate from the actual local source families. The nontrivial source inputs are the common composed ordinary ++ domain, the actual mixed-history coefficient rows, and the original source E Ward remainder with its own subtraction. They are the declared C01/native-map/source inputs, not a new assumption of the desired stopped-density phase. If those inputs are weakened to a post-integrated C bound alone, (SD.25) is not established. The exact source-reference distinction is retained here deliberately.

## 7. Relative action on its existing chart: the running-tail improvement

The actual completed-relative inputs are not assumed to exist on the ordinary ++ profile. They remain on the maintained + chart.

After the exact unrolling (SD.4), let the incoming relative action be

\[
 V_{\mathrm{rel},\zeta}(x,a)=\sum_G F_G(\zeta;x,a).
 \tag{SD.28}
\]

Do **not** sum the full values of all atoms that have any nonzero native dependence on a. A remote native map tail can make infinitely many distant atoms genuinely vary, while only their differences have a summable response. Instead form the complete anchored response of each incoming atom:

\[
 D_G(\zeta;x,a,a_*)
 =F_G(\Phi_\zeta(x,a),{\rm raw}(x,a))
  -F_G(\Phi_\zeta(x,a_*),{\rm raw}(x,a_*)).
 \tag{SD.29}
\]

The notation includes the full prescribed native/current argument map and all actual raw arguments. The response has two exact kinds of record: a direct raw-coordinate difference, and a native map difference with its actual first forcing leaf. The latter retains the map path from the incoming atom to the changed strip; it is not replaced by twice the full atom value.

Use the incoming actual incidence decomposition with its precise norm order:

\[
 \sup_x\sup_{a,a_*\in S_x}
       \sum_G\sup_{\zeta\in\mathcal D_+}
                |D_G(\zeta;x,a,a_*)|\le K_r.
 \tag{SD.30}
\]

The raw suprema are outside the sum. No sum of independent raw suprema is asserted. The history labels and output weights are fixed before applying this norm, and absent records are zero in a common label union. Summing these complete responses gives

\[
 |V_{\mathrm{rel},\zeta}(x,a)-V_{\mathrm{rel},\zeta}(x,a_*)|
 \le K_r.
\]

Consequently its contribution to (SD.12) obeys

\[
 |\sigma_{\mathrm{rel},\zeta}(x,a)|\le2K_r.
 \tag{SD.31}
\]

This uses only the existing + contour. It requires no analyticity in the raw variables and no native Cauchy estimate of an unknown relative family on a larger chart.

### Several simultaneous components use one common raw reference

For the componentwise local part, first classify the literal unrolled records by **all actual integrated dependencies**, including dependence through the prescribed native maps. A record enters the local reference for P only when those live integrated dependencies are all in P. A common independent native pair ζ is external; an integrated raw variable of another component is not. Cross-component raw, Gaussian and native-map responses remain in the marked interaction before this factorization.

Choose one admissible global reference tuple a_*=(a_P^*)_P on the source's actual componentwise support. In a truly local P record, replacing a_P by a_P^* gives the same value as replacing the whole live tuple by this one global a_*, because that record is independent of the other live components. Therefore the positive sum is still evaluated at common tuples, namely a and a_*. This is the reason the source component factorization and the actual dependency classification must precede centering.

It would be invalid to evaluate a global incoming family at a different full raw tuple for each P and then apply its single-raw-tuple catalog bound. Native map tails connecting P to another live component cannot be suppressed by a claim of formal locality; their actual first forcing-leaf records, with their crossing guard, belong to the remote interaction estimate. This convention is also required when the local cumulant sums from several P are combined at one physical root.

### AF tail calculation

Put Y_b=g_b^(−2), ell_b=log Y_b. Suppose the retained two-sided envelope gives

\[
 Y_b\ge c\{Y_r+(r-b)\}\qquad(b\le r),
 \tag{SD.32}
\]

and one creation-sector capacity has the profile

\[
 a_b\le C\ell_b^d e^{-c_0\ell_b^p},\qquad p>1.
 \tag{SD.33}
\]

For every 0<c_1<c_0, after adjusting fixed constants and the ceiling,

\[
 \sum_{b\le r}a_b
 \le C_1e^{-c_1\ell_r^p}.
 \tag{SD.34}
\]

**Proof.** The finite multiplicity of operation sectors is absorbed in C. The eventual decreasing envelope is compared to the integral

\[
 \int_{cY_r}^{\infty}(\log u)^d
                e^{-c_0(\log u)^p}\,du
 =\int_{\log(cY_r)}^{\infty}
        t^d e^{t-c_0t^p}\,dt.
 \tag{SD.35}
\]

Since p>1, the linear exponent t and any polynomial factor are absorbed by any fixed loss in c_0. A tail integration, or monotonicity of c_0pt^(p−1)−1, proves (SD.34). The shift log c changes lower-order powers only and is absorbed by the same fixed rate loss. ∎

This is sharper than replacing all historical capacities by a fixed small ball A_*.

The incoming rooted-load calculation, RL.4–RL.11, establishes

\[
 K_r\le Cg_r^{-u_*}\ell_r^{d_*}\sum_{b\le r-1}a_b
 \le C'e^{(u_*/2)\ell_r}\ell_r^{d_*}e^{-c_1\ell_r^p}
 =o(1).
 \tag{SD.36}
\]

A direct old raw slot is rooted on its actual integrated strip coordinate. A relative atom entering only through a native reconstruction response retains the corresponding deep-to-strip path. A protected footprint alone is not a genuine endpoint. Fine-cell density is paid by the original proper-root/age estimate before the current physical root is used. The old native grade is handled by a Banach directional supremum and the source mesh suppression, as independently checked in DR.17; it does not add an internal fine-coordinate sum. These are the substantive root assignments in the companion calculation; (SD.36) is not inferred from a scalar operator norm.

The displayed inverse coupling is allowed in this relative estimate because the incoming tail absorbs it. It is not allowed to migrate into the ordinary bound (SD.25), where the actual physical \(g_jP_j\) fluctuation must cancel the native inverse radius before the external logarithmic Cauchy gain is used.

All factors arising from unchanged transport of one original creation are paid once by its original mark. A repeated factor 1+Cg_r poly(ell_r) at every ordinary UV step would not be AF-summable and is **not** used. By contrast, the relative-tilt factor e^(CK_r) is AF-summable because of (SD.34).

## 8. Actual-density conclusion of the induction step

At a stage with the actual incoming rooted bound (SD.36), combine the exact pre-integration ordinary estimate with the incoming relative action and the positive native-independent raw factors. Equations (SD.12), (SD.27) and (SD.31) give

\[
 |\sigma_\zeta(x,a)|\le\delta_r,
 \qquad
 \delta_r=\delta_{\rm ord,r}+2K_r.
 \tag{SD.37}
\]

The bound is uniform at each fixed earlier/exterior tuple x, throughout the actual support, and on the same maintained + contour. With the common ceiling chosen so that δ_r<π/4, the actual stopped density has the common positive comparison

\[
 |p_\zeta(a\mid x)|
 \le e^{2\delta_r}\sec\delta_r\ p_0(a\mid x).
 \tag{SD.38}
\]

This is the required stronger transfer for a positive analytic catalog. It includes the full ordinary tilt, the incoming completed-relative action, actual selectors, coarea factors, all retained quadratic responses and archived multipliers. Intermediate normalizers cancel only by (SD.4), and the final mass obeys (SD.11).

The proof is an induction step from incoming capacities. It does not assume the outgoing C05 estimate to control its own density. For a bare Wilson start the completed-relative capacity is zero; the ordinary density is the base step. Remote new creations use the rooted new-load estimate and the two source connected extractions. Unguarded local nonlinear outputs instead use their positive multiset cumulant estimate, with their actual quadratic capacity and explicit diameter/count costs. The running-tail induction treats these two sectors separately and gives the same superlogarithmic capacity profile.

The companion rooted-load proof supplies the physical current-root conversion and one-time lineage bookkeeping, and [Complete boundary activities and normalized component induction](boundary_induction.md) assembles them with the running-tail induction. The result in this note removes the need to assume the actual completed-relative action has a second larger source chart, and removes the illegal use of a post-integrated coefficient bound to justify fixed-raw normalization.
