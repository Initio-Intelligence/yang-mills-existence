# Protected-core moments and rooted regular transport

## Part I. Uniform all-order protected-core moments

**Status:** A proved extension of the source large-field budget on a precisely specified carrier. All moment orders use one coupling threshold. The result concerns the actual old variables integrated by a matched core operation; it does not by itself control all mixed histories or the full normalized Schwinger hierarchy.

### 1. The quantifier problem and the new stopping rule

The preceding finite-degree theorem paid the engineering growth of a product of marks by adding its total dimension to the cost of every occupied component-step. For \(m\) dimension-four marks this meant a cost proportional to \(4m\), so its admissible coupling threshold depended on \(m\). That theorem was useful for S2 but did not give the route's all-order bound.

For separated roots there is a different allocation. Charge a root's engineering growth only while its unresolved component contains that root alone. Stop the charge just before the first step at which the component contains another root. A component containing several roots has already acquired physical extent at least their separation. A reserved part of its geometric penalty pays the scale powers of all the roots stopping there, with factorial growth in their number.

The source budget is enlarged by **two fixed constants**: one engineering charge per component-step and one geometric reserve. Neither depends on the number of roots.

The minimum separation used below is

\[
\delta=\min\{1,\min_{i\ne j}|x_i-x_j|\}>0.
\tag{PC1}
\]

Lengths are measured in units of the terminal physical scale \(\ell_0\); restoring units replaces the dimensionless factors by the corresponding powers of \(\ell_0\). Torus distances may be used, with the source's component geometry. The theorem is off the coincidence diagonals. No estimate at \(\delta=0\) is asserted.

### 2. The source cost controls physical diameter

For an active unresolved component \(Z\) at scale \(h_j=aL^j\), set

\[
q_j(Z)=M^dR_j^{d+1}d'_j(Z).
\tag{PC2}
\]

Here \(d'_j\) is the source's ordinary geometric tree size in \(MR_j\)-block units. It is not the distance in which a large-field component has been collapsed to a point. LFR II, printed p.380, explicitly identifies this convention in its bound on the normalization and vacuum terms. The resulting positive overhead is displayed in (1.79), printed p.383.

The active components have thickness greater than \(20MR_j\); see LFR I, printed p.177. In particular, their tree size is bounded below by a fixed positive constant. A connected union of these blocks satisfies

\[
\operatorname{diam}_{\rm phys}Z
 \le C_{\rm geo}\,h_jMR_j\bigl(d'_j(Z)+1\bigr)
 \le C'_{\rm geo}\,h_jMR_jd'_j(Z).
\tag{PC3}
\]

Since \(M,R_j\ge1\), (PC2)–(PC3) give constants independent of the scale and the number of roots such that

\[
q_j(Z)\ge c_0>0,
\qquad
q_j(Z)\ge c_1\frac{\operatorname{diam}_{\rm phys}Z}{h_j}.
\tag{PC4}
\]

Changing the convention for a one-block tree changes only these fixed constants. The thickness bound prevents a zero cost for an active component. The tree that joins the blocks gives (PC3): a path through that tree joins any two blocks with length bounded by its total length plus two block diameters.

The second inequality in (PC4) is stronger than merely bounding diameter by \(h_jR_j\) times a dimensionless tree length. The extra powers of \(R_j\) already present in the positive source overhead pay that loss. No order-dependent absorption of \(R_j\) is needed here.

### 3. A geometric exponential moment of the history budget

Let \(\omega\) denote an admissible unresolved history contributing to a matched core operation \(\mathcal T'_k(X)\) of LFR II (1.71). Its active components at scale \(j\) form a family \(\mathscr C_j(\omega)\). Write

\[
\mathcal Q(\omega)=
 \sum_{j=1}^{k}\sum_{Z\in\mathscr C_j(\omega)}q_j(Z).
\tag{PC5}
\]

The positive integral estimates and history counting that precede source (1.79) replace the remaining regular factors by an overhead bounded by \(C_0\mathcal Q\), together with the displayed birth and failed-reset penalties. The future-budget induction (1.80)–(1.88) then controls that overhead. Its proof works with any prescribed finite enlargement of \(C_0\), after decreasing the common upper bound on the effective couplings. This is the parameter robustness already proved in the preceding finite-degree module.

#### Lemma PC-A: fixed weighted history budget

Fix numbers \(\Delta>0\) and \(\Lambda>0\). Let \(a_j(Z)\ge0\) be a history-dependent charge satisfying

\[
a_j(Z)\le \Delta\log L
\quad\text{for every active component-step}.
\tag{PC6}
\]

Choose the source small-coupling threshold once, with overhead

\[
C_* = C_0+c_0^{-1}\Delta\log L+\Lambda+C_{\rm fin}\kappa_*.
\tag{PC7}
\]

Here \(C_{\rm fin}\) is a fixed geometric constant such that, for the ordinary final component or a fixed admitted buffer of it,
\(d_k(X)\le C_{\rm fin}q_k(X)\). Indeed, refining each \(MR_k\)-block to \(M\)-blocks bounds \(d_k(X)\) by \(C R_k^d(d'_k(X)+1)\), and active-component thickness removes the additive 1. The last term in (PC7) explicitly pays for inserting \(e^{\kappa_*d_k(X)}\) into the positive majorant. A positive fraction of the final \(p_0\) penalty is reserved separately. Then the positive majorant of the matched operation obeys

\[
\int \exp\!\left\{
 \sum_{j,Z}a_j(Z)+\Lambda\mathcal Q(\omega)
 \right\}\,d\mathfrak M_{k,X}(\omega,u)
 \le C e^{-c p_0(g_k)}e^{-\kappa_*d_k(X)}.
\tag{PC8}
\]

The notation \(d\mathfrak M_{k,X}\) denotes the same positive integrals and history sums bounded in source (1.79). It is not a new probability measure and is not divided by a global partition function. Where the source states only its general-region boundary convention, retain that convention instead of the ordinary final factor in (PC8).

**Proof.** By (PC4) and (PC6), the inserted exponent is at most

\[
\bigl(c_0^{-1}\Delta\log L+\Lambda\bigr)\mathcal Q.
\tag{PC9}
\]

Also insert \(e^{\kappa_*d_k(X)}\), using the final-component comparison just proved. Apply the positive integral and history-counting estimates with both multipliers retained. The resulting version of (1.79) has \(C_*\), rather than \(C_0\), in its positive overhead. Rerun (1.80)–(1.88) with that coefficient. At birth the \(p_0^2(d'+1)\) reserve pays the larger future cost; at a clean step the cost is subtracted; a failed reset contributes a new \(p_0\) reserve; and the merger surplus pays the fixed geometric overhead. The sufficient inequalities have the same form as before,

\[
p_0(g_j)\ge H_* R_j^{d+2},
\qquad
c_{\rm birth}A_1^2p_0(g_j)^2
 \ge H_*R_j^{d+2},
\tag{PC10}
\]

where \(H_*\) is fixed by \(C_*\), the geometry, and the retained margins. The source parameter condition \(p_0(g)/R(g)^{d+2}\to\infty\) permits one threshold satisfying (PC10) at every scale. There is no root count in \(C_*\) or \(H_*\). The completed reset has zero remaining future horizon; the separately reserved penalty and spatial factor give (PC8). This argument is valid whether the source bound is written as a sum or, after the history entropy estimate, as the supremum in (1.79). In the latter form it is the same history-by-history enlargement before taking that supremum. \(\square\)

This lemma does not assert a stochastic independence of the successive components. It uses the actual birth, merger, and failed-reset bookkeeping. In particular, no total-age bound is substituted for the source's clean lookback window.

### 4. Protected roots and first meetings

Consider bounded gauge-invariant old seeds \(F_i\), \(i=1,\ldots,m\), with roots \(x_i\) and

\[
|F_i|\le A_i a^{-\Delta}.
\tag{PC11}
\]

For every history included in the selected coefficient, require the following conditions:

1. Every variable used by each seed is among the old variables integrated by the chosen operation. Its full support is retained in an unresolved ancestry from its incoming scale to the final core operation.
2. A seed's root belongs to its active ancestor at each intermediate scale. Marked ancestors coarsen and merge; they do not release a marked variable through an earlier successful reset.
3. At the final scale all \(m\) roots lie in the same component \(X\). The roots are distinct as in (PC1).

These are the protected-core conditions already used for the finite-degree result, now imposed on an arbitrary finite set of roots. They concern the actual old variables. Replacing the seeds by observables of the newly sampled replacement configuration is not part of the argument.

For each root define

\[
\tau_i=\min\{j\ge1:
 Z_j(i)\text{ contains at least two of the marked roots}\},
\qquad s_i=\tau_i-1.
\tag{PC12}
\]

Here \(Z_j(i)\) is the component containing \(x_i\). For \(m\ge2\), condition 3 ensures \(\tau_i\le k\). If several roots already belong to one component at the first source step, their meeting time is 1 and their stopping scale is the incoming scale 0. This convention costs at most one factor \(L^\Delta\) per root in the estimate below.

Charge root \(i\) at the steps \(1,\ldots,s_i\). At any charged component-step that component contains exactly one marked root. Consequently the total charge there is at most \(\Delta\log L\), irrespective of \(m\). With the charges in (PC6) chosen in this way,

\[
\sum_{j,Z}a_j(Z)=\Delta\log L\sum_{i=1}^m s_i.
\tag{PC13}
\]

It is important to stop **before** the first meeting step. If many singleton ancestors merge at once, charging the output component for all of those final steps would introduce a cost proportional to their number. Our convention instead retains the single factor \(L^\Delta\) in the geometric estimate.

Group roots by their first meeting event \(e=(j,Z)\):

\[
I_e=\{i:\tau_i=j,\ Z_j(i)=Z\},
\qquad n_e=|I_e|.
\tag{PC14}
\]

The nonempty \(I_e\)'s partition \(\{1,\ldots,m\}\), and different events are different component-steps. An event can have \(n_e=1\), when a new singleton joins a component containing roots that stopped earlier. Nevertheless its component contains at least two distinct roots, so

\[
q_j(Z)\ge c_1\delta/h_j.
\tag{PC15}
\]

This is the only spatial information needed for the factorial estimate. If finite stencils are used, the root points themselves must remain in the retained component; otherwise enlarge the component by the fixed stencil support before invoking (PC3). The fixed enlargement changes constants, not the moment-order dependence.

### 5. The elementary optimization that gives a fixed factorial power

#### Lemma PC-B: a meeting pays every finite multiplicity

For every integer \(n\ge1\), every \(h,\delta>0\), and fixed \(\Delta,c>0\),

\[
h^{-\Delta n}e^{-c\delta/h}
 \le \left(\frac{\Delta}{c}\right)^{\Delta n}
 (n!)^\Delta\delta^{-\Delta n}.
\tag{PC16}
\]

**Proof.** Put \(u=\delta/h\). The supremum of \(u^{\Delta n}e^{-cu}\) is attained at \(u=\Delta n/c\), and equals \((\Delta n/(ce))^{\Delta n}\). The inequality \(n!\ge(n/e)^n\) proves (PC16). \(\square\)

Apply (PC16) at each first meeting, using (PC15) and \(h_{s_i}=h_j/L\) for \(i\in I_e\). Since \(\mathcal Q\) includes all these different events,

\[
\begin{aligned}
\left(\prod_i h_{s_i}^{-\Delta}\right)
 e^{-\Lambda\mathcal Q}
&\le \prod_e
 \left[L^{\Delta n_e}h_j^{-\Delta n_e}
 e^{-\Lambda q_j(Z)}\right] \\
&\le C_\Delta^m\delta^{-\Delta m}
 \prod_e(n_e!)^\Delta \\
&\le C_\Delta^m(m!)^\Delta\delta^{-\Delta m}.
\end{aligned}
\tag{PC17}
\]

The last inequality follows because \(m!/\prod_e n_e!\) is a positive integer. There is no sum over partitions in (PC17): each history determines its meeting groups. The history sum has already been retained in (PC8), so the argument does not incur an additional Bell-number cost.

The optimization is over the physical ratio \(\delta/h\). It never maximizes an order-dependent inverse coupling against a logarithmic rare-event penalty. It therefore avoids the superfactorial obstruction of the observable route.

### 6. The all-order protected-core theorem

#### Theorem PC-C

Fix \(\Delta>0\), the source parameters, and the protected-core conditions of §4. There exist constants \(C,c,\kappa_*>0\) and one admissible upper coupling threshold, all independent of \(m\), the microscopic cutoff, the history depth, and the torus, such that for every \(m\ge2\),

\[
\boxed{
\left|\mathcal T'_k(X)\prod_{i=1}^{m}F_i\right|
\le C^{m+1}(m!)^\Delta
 \left(\prod_i A_i\right)
 \delta^{-\Delta m}
 e^{-c p_0(g_k)}e^{-\kappa_*d_k(X)}.
}
\tag{PC18}
\]

The usual source restriction on the final ordinary geometric factor is retained. For \(m=1\), the same threshold yields the current-scale estimate

\[
\left|\mathcal T'_k(X)F_1\right|
 \le C A_1h_k^{-\Delta}
 e^{-c p_0(g_k)}e^{-\kappa_*d_k(X)}.
\tag{PC19}
\]

**Proof.** For a fixed history, (PC11) gives

\[
\prod_i|F_i|
 \le \left(\prod_i A_i\right)
 \left(\prod_i h_{s_i}^{-\Delta}\right)
 \exp\!\left\{\Delta\log L\sum_i s_i\right\}.
\tag{PC20}
\]

Multiply and divide the right side by \(e^{\Lambda\mathcal Q}\), then use (PC17). The remaining positive integral is precisely bounded by (PC8), with (PC13). This proves (PC18). For one root, charge it through scale \(k\); there is still at most one charged root per active component-step. Equation (PC8) with \(\Lambda=0\), or with its extra reserve unused, proves (PC19). The choices of source constants depend on \(\Delta\), never on \(\Delta m\). \(\square\)

For the unrenormalized Wilson/clover family, the earlier pointwise bounds provide \(\Delta=4\) and fixed \(A_i\) depending only on the fixed gauge group and the chosen finite family. Hence (PC18) gives factorial exponent four and singular order \(4m\) for every protected multi-root core coefficient at one common threshold.

The result extends to the source's analytic background domain when the seeds remain functions only of the integration variables. Source (1.73) bounds the analytically continued operation by its positive counterpart with \(e^{|\sigma|}\); the source's fixed analytic reserve controls that factor. Absorb its fixed cost into (PC7) and the separately retained margins. If the seed itself depends on the continued background, its corresponding analytic seed bound is required. A real sup norm does not automatically control that dependence.

### 7. Incoming normalization and a small increase of singular order

Suppose a common deterministic field normalization and subtraction give an incoming bound

\[
|F_i^{\rm ren}|\le A\,a^{-4}
 \bigl(1+\log(\ell_0/a)\bigr)^r
\tag{PC21}
\]

with fixed \(A,r\). Such a bound must first be proved for the chosen running normalization; it is not supplied by positivity alone. For any fixed \(\varepsilon>0\),

\[
(1+t)^r\le C_{r,\varepsilon}e^{\varepsilon t},
\qquad t\ge0.
\tag{PC22}
\]

Thus (PC21) is an incoming bound of dimension \(\Delta=4+\varepsilon\), with one fixed constant per field. Theorem PC-C then yields

\[
\left|\mathcal T'_k(X)\prod_iF_i^{\rm ren}\right|
 \le C_\varepsilon^{m+1}(m!)^{4+\varepsilon}
 \delta^{-(4+\varepsilon)m}
 e^{-c p_0(g_k)}e^{-\kappa_*d_k(X)},
\tag{PC23}
\]

in terminal-scale units. One may replace the factorial exponent by the next larger integer if desired. The route permits a fixed singular order linear in \(m\), so this is compatible with its OS target. The supremum in (PC22) is taken once, before raising the estimate to the \(m\)th power.

The same reasoning applies to a fixed power of \(g(a)^{-1}\) once the admitted AF trajectory supplies the required logarithmic comparison. An unknown or root-dependent normalization cannot be folded into this corollary.

### 8. Relation to normalized clusters and to the full M theorem

Equation (PC18) controls an **unnormalized matched core operation**, with the small core mass retained. Dividing by \(\mathcal T'_k(X)1\) would remove that small mass and is not an allowed way to claim the same bound for every posterior ratio. In the full construction these coefficients enter normalized connected polymer expansions, as in the preceding finite-degree analysis.

Two facts make (PC18) useful for that next step:

- For every subset of roots in a protected component, it supplies a common factorial budget. The global minimum separation may replace the subset's larger separation.
- Factorial weights of exponent at least one are stable under the partition operations converting moments to connected coefficients, provided the required activity sums and normalization bounds are available on the same law.

For clarity, the latter statement has a short independent proof. If \(|M_I|\le B^{|I|}(|I|!)^p\delta^{-\sigma|I|}\), \(p\ge1\), and \(M_\varnothing=1\), the formal cumulant coefficient satisfies

\[
|C_{[m]}|
 \le B^m\delta^{-\sigma m}
 \sum_{\pi\in\mathcal P_m}(|\pi|-1)!
 \prod_{B\in\pi}(|B|!)^p
 \le (2B)^m(m!)^p\delta^{-\sigma m}.
\tag{PC24}
\]

Indeed \(\prod_B|B|!\le m!\), and the number of ordered positive compositions of \(m\) into \(r\) parts is \(\binom{m-1}{r-1}\). Summing first over partitions with \(r\) blocks gives

\[
\sum_{\substack{\pi\in\mathcal P_m\\|\pi|=r}}
(r-1)!\prod_{B\in\pi}|B|!
 =\frac{m!}{r}\binom{m-1}{r-1},
\tag{PC25}
\]

and summing \(r\) bounds this by \(2^{m-1}m!\). This proves (PC24). The identity is finite algebra; it makes no assertion about an exponential source series with a radius independent of \(m\).

It would nevertheless be premature to apply (PC24) to the full YM moments. Several inputs remain distinct:

1. Marks leaving a core, entering it after previous regular transport, or crossing its boundary need compatible incoming current-scale norms and anchored decompositions.
2. Roots ending in different components require the connected expansion joining those components and its full spatial and activity weights.
3. The outer operations acting on the component gas, and the covariance or higher cumulants of its conditional means, remain part of the actual positive history law.
4. All generated mixed regular/core source coefficients must share one normalization and one all-order induction norm.

The present theorem closes the **uniform-in-order age absorption problem for protected old cores**. It does not assert that these four interfaces have already been established.

### 9. The remaining scale sum also closes for this component class

The preceding estimate does not leave an order-dependent optimization over the reset scale. Assume the route's admitted AF comparison in the quantitative form

\[
x_j=g_j^{-2}\ge x_K+c_-(K-j),
\qquad
p_0(g_j)\ge c_p(\log x_j)^P,
\qquad P>1.
\tag{PC26}
\]

Then, at the same common threshold,

\[
\sum_{j=1}^{K}e^{-c p_0(g_j)}
 \le 1+\frac1{c_-}\int_{x_K}^{\infty}
 e^{-cc_p(\log x)^P}\,dx
 =:C_{\rm age}(x_K)<\infty.
\tag{PC27}
\]

The inequality may use a fixed enlarged first term when comparing the sum with the integral; this changes no parameter dependence. The integral converges because the substitution \(y=\log x\) gives the exponent \(y-cc_p y^P\). A bound tending to zero as \(x_K\to\infty\) follows by keeping the actual first term instead of 1. This is a uniform depth bound, with no dependence on \(m\).

Choose the separately retained final tree-decay rate strictly above the anchored animal-counting rate. The sum of \(e^{-\kappa_*d_j(X)}\) over ordinary source localization domains containing a fixed root is then bounded uniformly in \(j\). Summing (PC18) first over these domains and then over reset scales proves the absolute majorant bound

\[
\sum_{j,X\ni x_1}
\sup_{\text{admitted exterior}}
\left|\mathcal T'_j(X)
 \left[\prod_{i=1}^{m}F_i;
 \text{all roots protected and ending in }X\right]\right|
\le C^{m+1}(m!)^\Delta
 \left(\prod_i A_i\right)\delta^{-\Delta m},
\quad m\ge2.
\tag{PC28}
\]

As throughout this note, the ordinary-domain restriction matters: a collapsed boundary metric cannot be used for this animal count without its own geometry theorem. A geometry selector in the square brackets simply restricts the source's positive history sum and is allowed in (PC8).

Thus both the geometric optimization and the scale sum in the observable route's repair of that obstruction close for the specified protected-core component terms. If such terms have been placed in an actual normalized kernel representation with these same absolute weights, the route's coincidence-flat kernel-to-test-function theorem applies with fixed factorial exponent \(p=\Delta\) and singular order \(\sigma=\Delta\), or any larger fixed exponents. This last placement still requires the normalized connected expansion and outer-law identities listed in §8; (PC28) does not perform them implicitly.

### 10. Source anchors

The source formula (1.79) and the definition of \(d'_j\) are those printed on pp.380 and 383. The first-meeting allocation and its factorial optimization cover in particular an initially multi-root component, one new root joining an already marked component, simultaneous mergers of many singleton components, and the placement of the single-step factor \(L^\Delta\).

Primary source inputs:

- **Balaban, LFR I**, CMP 122 (1989), 175–202, printed p.177: active-component thickness and the distinction between clean reset eligibility and total age.
- **Balaban, LFR II**, CMP 122 (1989), 355–392, printed pp.379–380, (1.71)–(1.75): matched old-variable operation, positivity, and its analytic continuation; printed p.380: ordinary \(MR_j\)-block tree-size convention; printed pp.383–387, (1.79)–(1.89): positive history overhead and the birth/clean-step/failed-reset/merger budget.
- **[Yang–Mills existence through observable derivatives](../observable_route.md)**, §§5–6: one fixed factorial budget off the coincidence diagonals, the quantifier order, and the inverse-coupling obstruction.

The new stopping rule, the retained geometric exponential moment, and (PC17)–(PC23) are derived here. They are not attributed to the source as previously stated observable theorems.

---

## Part II. Normalized connected core coefficients and scale summation

**Status:** A uniform all-order theorem for the actual normalized component gas on a carrier with **no remaining unprocessed exterior large-field components** (\(Y_i=\varnothing\)), with its exterior variables held fixed. The proof combines the first-meeting bound with the actual R-operation expansion in a finite source algebra. It includes different-core connections. Cumulants of the remaining exterior conditional means, core exits, and general mixed-history insertions are not included.

### 1. The carrier and what is normalized

Let \(\Xi_k\) be the full component gas inside the braces of LFR II (1.72), after the matched operation \(\mathcal T'_k(X)\) has been defined in (1.71), on an admitted carrier for which the source's remaining unprocessed large-field regions \(Y_i\) are absent. All variables and histories on which the still-unperformed outer operations act are held fixed. Freeze the unmarked forward reset kernels, normalizers, cutoff choices, and coupling trajectory. This is an actual specialization of the source integral, not a gas formed by deleting unwanted activities.

The condition \(Y_i=\varnothing\) is necessary for the ordinary-distance estimate below. With remaining \(Y_i\), source (1.97) also produces activities carrying only its boundary smallness and a geometry in which those regions are collapsed. The full conditional cumulant on such a carrier is outside this theorem.

Insert distinct labels \(t_1,\ldots,t_m\) into the **old** component integrals. A label is admitted only when its seed has the protected-core property from Theorem PC-C: its complete support remains among the unresolved old variables up to this component integration.

To make the selection consistent across all moments, define one history selector \(\chi_i(\omega)\in\{0,1\}\) for each root. It is one precisely when the seed's complete support and root remain protected and have a unique owning component at the present operation, and zero otherwise. In every contributing history insert the single product

\[
 \prod_{i=1}^{m}\bigl(1+t_i\chi_i(\omega)F_i\bigr).
 \tag{CG0}
\]

The selectors are fixed functions of the old variables and component histories; they do not depend on the subset of labels whose coefficient is extracted. For a specified owning component, its selector is determined by that component's own integrated ancestry and the fixed exterior data. An additional nonlocal history event is not multiplied into the selector. This preserves the localization of the matched operation. Labels assigned to a given component use the actual product of its selected seeds. Components are disjoint, so a label is never assigned twice. A seed outside this class gives a zero selected mark, while its other physical contributions remain to be treated separately.

The resulting \(\Xi_k(t)\) has the exact normalized generating expression

\[
\frac{\Xi_k(t)}{\Xi_k(0)}.
\tag{CG1}
\]

Equivalently, before the cluster expansion, (CG1) is the expectation of (CG0) under the positive conditional old-field/history measure at this fixed exterior data. At this conditioning level, the full-label coefficient of \(\log\Xi_k(t)-\log\Xi_k(0)\) is therefore the joint cumulant of the selected variables \(\chi_iF_i\). It includes the terms in which the labels are in different cores, joined by the component expansion. The convergent expansion defines its analytic continuation on complex admitted exterior configurations. No subset-dependent selection of moments is used.

The outer operations act on \(\Xi_k\). They cannot subsequently be cancelled as scalar factors. Therefore the coefficient in (CG1) is not identified with the full physical-output cumulant after those outer operations. This is the same conditioning distinction used in the earlier two-root analysis.

All lengths below are in terminal-scale units, \(h_k\le1\), and

\[
\delta=\min\{1,\min_{i\ne j}|x_i-x_j|\}>0.
\tag{CG2}
\]

### 2. A finite algebra that preserves every source coefficient

For a fixed arbitrary integer \(m\), use the commutative finite-dimensional algebra

\[
\mathcal A_m=\mathbb C[t_1,\ldots,t_m]/(t_1^2,\ldots,t_m^2).
\tag{CG3}
\]

Write \(t_I=\prod_{i\in I}t_i\). For \(r>0\), define

\[
\left\|\sum_{I\subset[m]}a_I t_I\right\|_r
 =\sum_{I\subset[m]}|a_I|r^{|I|}.
\tag{CG4}
\]

This norm is submultiplicative:

\[
\|ab\|_r\le\|a\|_r\|b\|_r.
\tag{CG5}
\]

Indeed, the coefficient of \(t_I\) in a product sums over disjoint pairs of label sets whose union is \(I\). The product of the norms includes all of those nonnegative terms and possibly more. Also,

\[
|[t_{[m]}]a|\le r^{-m}\|a\|_r.
\tag{CG6}
\]

These are finite algebra identities. No nonzero complex-source radius uniform in \(m\) is postulated. In particular, all repeated appearances of distinct labels and all mixed product coefficients are kept exactly.

When coefficients are bounded functions of unintegrated variables or analytic functions on a source background domain, use the coefficientwise supremum norm \(\sum_I r^{|I|}\|a_I\|_\infty\). It also satisfies (CG5). This stronger convention is used in every operation and activity estimate below, so no interchange of a coefficient sum with a supremum is needed.

### 3. One smallness threshold for every marked component

Fix \(\Delta\ge1\). Suppose every incoming seed has the bound
\(|F_i|\le A a^{-\Delta}\), with fixed \(A\), and satisfies the protected-core conditions. Enlarge constants to include \(A\). Theorems PC-C and PC-A give, for each subset \(I\), coefficients of the actual matched component operation bounded by

\[
\begin{aligned}
|\mathcal T_{k,\varnothing}(X)|
 &\le C\eta_k e^{-\kappa_0d_k(X)},\\
|\mathcal T_{k,I}(X)|
 &\le C^{|I|+1}(|I|!)^\Delta
 B_k^{|I|}\eta_k e^{-\kappa_0d_k(X)},
 \qquad I\ne\varnothing,
\end{aligned}
\tag{CG7}
\]

where

\[
\eta_k=e^{-c p_0(g_k)},
\qquad
B_k=\max\{h_k^{-\Delta},\delta^{-\Delta}\}.
\tag{CG8}
\]

For one label use (PC19); for at least two labels use (PC18), with the global separation replacing the subset's possibly larger separation. The constants and the threshold in (CG7) do not depend on \(|I|\).

The same bounds hold for the norm of the marked operation applied to an additional bounded integrand. Its absolute supremum multiplies the right side. The first-meeting proof used the pointwise seed bounds before positive integration, so it remains valid with this additional factor. This is the form needed when the source's scalar Mayer factors are present.

Choose one sufficiently small \(\varepsilon\in(0,1/2)\), independent of \(m,k\), and set

\[
r_k=\frac{\varepsilon}{C B_km^\Delta}.
\tag{CG9}
\]

Summing all nonempty source coefficients in the algebra norm gives

\[
\begin{aligned}
\sum_{I\ne\varnothing}
C^{|I|}(|I|!)^\Delta B_k^{|I|}r_k^{|I|}
&\le\sum_{s=1}^m
 \binom ms(s!)^\Delta\frac{\varepsilon^s}{m^{\Delta s}}\\
&\le\sum_{s=1}^m\varepsilon^s
 \le\frac{\varepsilon}{1-\varepsilon}.
\end{aligned}
\tag{CG10}
\]

For the second inequality use \(\binom ms\le m^s/s!\) and \((s!)^{\Delta-1}\le m^{(\Delta-1)s}\). Thus each component's complete source-algebra norm is bounded by its unmarked positive majorant times one fixed factor. This is a comparison of majorants, not a division by the actual unmarked component integral. Its marked part retains a factor \(\eta_k\).

The small parameter \(r_k\) is only a coefficient-weight choice in a finite algebra. It changes neither the physical seed nor the unmarked RG transformation. Its dependence on \(m\) is explicitly paid when extracting the final coefficient.

### 4. The actual R expansion accepts these algebra-valued operations

LFR II (1.90)–(1.91) expands ordinary scalar interactions into Mayer factors and combines them with the localized operations \(\mathcal T'_k(X)\). Its estimate (1.92) uses the positive majorants of those operations. Products of operations assigned to disjoint components, sums over admissible families, and scalar Mayer expansions are all compatible with the algebra (CG3).

Repeat those finite expansions with \(\mathcal A_m\)-valued operations. At each estimate apply (CG5), followed by (CG7)–(CG10). The source's unchanged scalar estimates still bound every interaction factor. For an operation applied to an algebra-valued additional integrand, expand its coefficient convolution, apply the bounded-integrand version of (CG7) to each coefficient, and sum with the weights \(r_k^{|I|}\). Submultiplicativity gives exactly the same fixed operation majorant. Thus this step estimates the actual operations; it does not hypothesize bounds for already constructed marked activities.

This reproduces source (1.92) with fixed slightly enlarged constants. In its subsequent estimate (1.95)–(1.97), the number \(q\) of core operations in every activity is at least one when \(Y_i=\varnothing\). Each carries the enlarged majorant \(C\eta_k[1+\varepsilon/(1-\varepsilon)]\). Extract one reserved rare-core factor and use the unchanged source sums for all remaining components, scalar Mayer links, and extensions. The fixed extra factor per core is absorbed by the same unused \(p_0\) reserve that pays the source's geometric enlargement costs. Choose the coupling threshold once so these constants and the fixed localization reserves fit. The resulting explicit activity bound is

\[
 \|\zeta_k(t;Y)\|_{r_k,+}
 \le C_0\eta_k e^{-\kappa_{\rm act}d_k(Y)}.
 \tag{CG10a}
\]

Here \(c\) in \(\eta_k=e^{-c p_0(g_k)}\) may be reduced by a fixed amount, \(\kappa_{\rm act}\) lies strictly inside the ordinary source exponent, and every constant is independent of \(m\). This is source (1.97) on the stated carrier, with the complete finite-algebra norm in place of the scalar absolute value.

Choose an ordinary connected-polymer length \(\ell_k(Y)=d_k(Y)+\omega\), including a fixed additive constant so connected unions satisfy \(\ell_k(\cup_iY_i)\le\sum_i\ell_k(Y_i)\). The source's separate boundary/collapsed metrics are not substituted for this ordinary length. Let \(n(Y)\le c_n(d_k(Y)+1)\), and bound the number of domains containing a specified block with \(j\le d_k(Y)<j+1\) by \(C_AA_A^{j+1}\). Choose \(a_0,\lambda>0\) with strict reserve

\[
 \kappa_{\rm act}-\lambda-a_0c_n
 >\log A_A+\nu,\qquad \nu>0.
 \tag{CG10b}
\]

The source permits this choice by fixing its geometric exponent sufficiently large. The explicit geometric series obtained from (CG10a) then gives

\[
 \sup_b\sum_{Y\ni b}
 \|\zeta_k(t;Y)\|_{r_k,+}
 e^{a(Y)+\lambda\ell_k(Y)}
 \le C_1\eta_k,\qquad a(Y)=a_0n(Y).
 \tag{CG10c}
\]

Every domain incompatible with \(X\) contains a block in a fixed neighboring set of at most \(c_{\rm touch}n(X)\) blocks. Taking \(C_1c_{\rm touch}\eta_k\le(1-\theta)a_0\), uniformly in \(k\), proves the weighted KP inequality

\[
\sum_{Y\not\sim X}
 \|\zeta_k(t;Y)\|_{r_k,+}
 e^{a(Y)+\lambda\ell_k(Y)}
 \le(1-\theta)a(X),
\qquad a(X)=a_0 n(X).
\tag{CG11}
\]

All extension and animal-counting costs, including the KP weight on every extension block, are included in this inequality. Equations (CG10a)–(CG10c) display the conversion from the source activity bound to that full weighted norm.

For a specified label, say \(t_1\), write

\[
 \zeta_k^{[1]}(Y)
 =\zeta_k(t;Y)-\zeta_k(t_1=0,t_2,\ldots,t_m;Y).
 \tag{CG11a}
\]

This projection keeps exactly the coefficients containing label \(1\), so its coefficientwise norm is no greater than that of \(\zeta_k(t;Y)\). Every surviving term contains the actual component owning root \(x_1\), and the source localization domain contains that entire component. Consequently \(\zeta_k^{[1]}(Y)=0\) unless \(Y\) contains the prescribed coarse root carrier. Applying (CG10c) at one fixed block of that carrier proves the full anchored bound

\[
 \sum_Y
 \|\zeta_k^{[1]}(Y)\|_{r_k,+}
 e^{a(Y)+\lambda\ell_k(Y)}
 \le C_1\eta_k.
 \tag{CG11b}
\]

The root carrier and any fixed protective enlargement are part of the actual source support. This proof does not attach an unweighted root to an otherwise unanchored activity.

The smallness choices in (CG11) are independent of \(m\): (CG10) is the step that ensures this. Neither an order-dependent change of the physical trajectory nor an order-dependent tightening of the source constants is used.

### 5. Connected normalization and spatial decay

The KP tree induction applies in any commutative normed algebra with a submultiplicative norm. Taking the norm term by term gives the usual scalar positive tree majorant. In a nonzero product, at most one activity can carry \(t_1\), because \(t_1^2=0\). Hence the difference of logarithms below has exactly the standard one-root expansion, with \(\zeta_k^{[1]}\) as its distinguished activity and all other activities bounded by (CG11). The rooted-tree induction bounds all attached descendants of a fixed root polymer \(Y_0\) by \(e^{a(Y_0)}\), already paid in (CG11b). Therefore the connected expansion for

\[
\mathcal L_k(t)=\log\Xi_k(t)
 -\log\Xi_k(t_1=0,t_2,\ldots,t_m)
\tag{CG12}
\]

is absolutely convergent in (CG4), with an anchored local decomposition. Its total weighted norm is at most \(C\eta_k\). The difference in (CG12) removes the extensive vacuum contribution before using the anchored estimate.

The coefficient of \(t_{[m]}\) in (CG12) is the same as in \(\log\Xi_k(t)\). Every term contributing to that coefficient has a connected support containing all roots. The ordinary localization geometry therefore gives

\[
\ell_k(Y)\ge c\frac{\delta}{h_kR_k}-C.
\tag{CG13}
\]

Fixed factors of \(M\), fixed buffers, and the one-block length convention are included in the constants. This deliberately conservative profile permits the source's \(R_k\) enlargement. It is not inferred from a distance that collapses an unresolved exterior region.

Extract the full coefficient with (CG6) and use
\(m^{\Delta m}\le e^{\Delta m}(m!)^\Delta\). The actual conditional connected coefficient of the selected core marks satisfies

\[
\boxed{
|\kappa^{\rm core}_{m,k}(x_1,\ldots,x_m\mid\mathrm{exterior})|
\le C^{m+1}(m!)^\Delta B_k^m\eta_k
 \exp\!\left[-c\frac{\delta}{h_kR_k}\right],
\quad m\ge2.
}
\tag{CG14}
\]

This estimates same-core products and different-core connections in one normalization. It is a theorem on the actual restricted component gas, with the exterior held fixed. An arbitrary probability average of these conditional absolute bounds is legitimate. Replacing that average by the full higher cumulant, without adding the cumulants of conditional means and the other law-of-total-cumulance terms, is not legitimate.

### 6. Converting the profile to one all-order off-diagonal bound

Assume the route's quantitative AF comparison and the source's polylogarithmic choice of \(R_k\), along one prescribed terminal matching trajectory. The constants may depend on its fixed terminal matching coupling \(x_K=g_K^{-2}\), or on a prescribed bounded matching range. That trajectory/range is fixed before varying \(m\). For each fixed \(\epsilon\in(0,1)\) there is then a fixed constant \(C_\epsilon\) such that

\[
R_k\le C_\epsilon h_k^{-\epsilon},
\qquad 0<h_k\le1.
\tag{CG15}
\]

For example, if \(g_k^{-2}\le C(1+\log(1/h_k))\) and \(R(g)\le C(1+\log g^{-2})^{r_0}\), take the supremum of that fixed logarithmic function times \(h^\epsilon\) once. The constant in this AF upper bound already includes the prescribed terminal matching range. At \(h_K=1\), (CG15) is not a uniform assertion over arbitrarily large \(x_K\). Do not optimize the logarithmic comparison separately against a degree-\(m\) penalty.

Set \(\alpha=1-\epsilon\). For \(h_k\le\delta\), (CG14) uses \(B_k=h_k^{-\Delta}\), and (CG15) gives

\[
h_k^{-\Delta m}
 \exp[-c\delta/(h_kR_k)]
\le h_k^{-\Delta m}e^{-c_\epsilon\delta h_k^{-\alpha}}.
\tag{CG16}
\]

Put \(u=\delta h_k^{-\alpha}\). The same elementary maximization as in Lemma PC-B proves

\[
h_k^{-\Delta m}e^{-c_\epsilon\delta h_k^{-\alpha}}
\le C^{m}(m!)^{\Delta/\alpha}
 \delta^{-\Delta m/\alpha}.
\tag{CG17}
\]

For \(h_k\ge\delta\), \(B_k=\delta^{-\Delta}\), and (CG17)'s larger singular power already bounds the factor needed in (CG14). Consequently, at every scale,

\[
\boxed{
|\kappa^{\rm core}_{m,k}(X\mid\mathrm{exterior})|
\le C^{m+1}(m!)^{p_*}
 \delta^{-\sigma_*m}\eta_k,
\qquad
\sigma_*={\Delta\over1-\epsilon},
\quad p_* =\Delta+{\Delta\over1-\epsilon}.
}
\tag{CG18}
\]

Both exponents are fixed before \(m\) is varied. In particular:

| Incoming seed bound | Parameter choice | Fixed singular order | Fixed factorial exponent |
|---|---|---:|---:|
| \(A a^{-4}\) | \(\Delta=4,\ \epsilon=1/5\) | \(\sigma_*=5\) | \(p_*=9\) |
| \(A a^{-4}(1+\log(1/a))^r\), fixed \(r\) | First use (PC22) with \(\Delta=9/2\); then \(\epsilon=1/10\) | \(\sigma_*=5\) | \(p_*=19/2\le10\) |

The second row presupposes the stated common incoming normalization bound; it does not prove that normalization. These exponents are convenient sufficient values, not claims of optimality.

Finally, the same AF hypothesis and \(p_0(g)\gtrsim(\log g^{-2})^P\), \(P>1\), give (PC27). Summing (CG18) over all reset scales yields

\[
\sum_k\sup_{\rm admitted\ exterior}
|\kappa^{\rm core}_{m,k}(X\mid\mathrm{exterior})|
\le C^{m+1}(m!)^{p_*}\delta^{-\sigma_*m}.
\tag{CG19}
\]

This is an all-order absolute bound for the normalized restricted core-gas coefficients, with one fixed trajectory threshold. If these coefficients are included in a larger exact kernel decomposition, (CG19) supplies their contribution to the route's absolute certificate (36).

The route's coincidence-flat continuity theorem then controls the distributions represented by this component contribution. For the bare first row of the table one may take \(p=9\), \(\sigma=5\), no polynomial spatial growth, and any fixed integer \(q>5\), such as \(q=8\), in its Schwartz seminorm of order \(qm\). No extension to arbitrary coincidence tests is being asserted.

### 7. What this advances and what is still outside the theorem

On the stated carriers with \(Y_i=\varnothing\), this theorem closes more than a fixed-degree core estimate. It proves a common factorial budget for all marked component moments, performs their connected normalization in the actual source algebra, includes different-core connections, and sums their physical localization profiles over the reset scales. The source threshold and terminal matching trajectory/range are fixed once for the entire hierarchy.

The full M theorem still needs the other sectors and their exact composition. A root can enter a core after regular transport, leave a core through a reset, cross a regular/core boundary, or interact with a remaining exterior large-field component. Those events require the common anchored norm and its boundary estimates. In addition, after the component gas has been normalized, the outer conditional means and all law-of-total-cumulance terms must be controlled under the same complete history law.

The local algebra proved here is compatible with that larger induction. It does not identify the selected component contribution with the entire Yang–Mills Schwinger function.

#### Sources and verification

The first-meeting theorem supplies (CG7), including the source overhead enlargement. The algebra-valued extension follows LFR II (1.90)–(1.97): the expansion is multilinear in the matched core operations, and its estimates use exactly the positive majorants preserved by (CG5). On the explicitly restricted \(Y_i=\varnothing\) carrier, every activity contains a core operation; (CG10a) retains its rare-core factor. The explicit animal sum (CG10b)–(CG10c) pays all output and KP weights, while the label projection gives the anchored bound (CG11b). The KP step is then the positive rooted-tree induction used for the one-root theorem, with the coefficientwise algebra norm in place of absolute value.

The normalization in (CG1), consistent history selectors in (CG0), the conditioning level and \(Y_i=\varnothing\) restriction, the \(m\)-dependent coefficient weight, the extra factorial cost in (CG17), and the increased singular order in (CG18) are explicit. These details prevent the finite-degree theorem from being silently relabeled as an all-history result.

---

## Part III. The normalized rooted regular operation

**Status:** A concrete restricted version of the generic-root estimate AO3 is proved below. Its input is a localized bounded fluctuation insertion, holomorphic in the complete source background variables, or a local analytic chart function composed with the actual nonlinear minimizing-field response. The proof keeps the small factor \(g r_\chi\), controls all localization derivatives of the insertion, and sums the full root extension, animal, and KP weights. It uses the regular small-field construction of CMP **116**, rather than assuming a marked activity estimate. It does **not** establish that every previously transported point insertion returns to this same chart class, and it does not settle the source-profile, auxiliary-current, gauge-atlas, or mixed-history interfaces needed for a complete S2 induction.

The rooted regular operator uses the contraction estimate below.

### 1. Source conventions and the exact operation

The principal source is T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. II. Cluster Expansions*, Commun. Math. Phys. **116** (1988), 1–22:

<https://doi.org/10.1007/BF01239022>.

The relevant inputs are the nonlinear switched response in §1, equations (1.3)–(1.21); the localized potential class in Lemma 2; the real-contour conditional Gaussian construction (2.1)–(2.26); and Lemma 3, equation (2.38). The direct one-insertion formula in CMP **119**, (3.44)–(3.47), provides the same rooted normalization algebra. We give the estimates here because that particular insertion formula alone does not prove a bound for an arbitrary analytic mark.

Fix an admitted full-torus regular carrier. Write its unnormalized fluctuation integral, in the independent real coordinates \(A\), as

\[
 Z_0(U,J)=\int_{D_\chi}d\mu_{C(U,J)}(A)
       \exp\!\left\{\sum_Y V_Y(U,J,A)\right\}.
 \tag{RX1}
\]

Here \(D_\chi\) is the actual product cutoff domain, \(U,J\) are the complete source background and auxiliary variables, and every source potential has its prescribed local background domain. The sign of \(V_Y\) follows the convention of (RX1). All bounds below are unchanged if an action is written with the opposite sign. For complex backgrounds the measure in (RX1) need not be positive. The cluster construction, rather than a complex probability inequality, defines its normalized analytic continuation.

The physical forward kernel, all running couplings, the minimizing-field maps, \(C\), and \(D_\chi\) remain fixed. A parameter \(t\) below is only a source in the integrand. Thus

\[
 \left.\partial_t\log Z(t;U,J)\right|_{t=0}
 =\frac{\int_{D_\chi}d\mu_C\,I\,e^{\sum V_Y}}
        {\int_{D_\chi}d\mu_C\,e^{\sum V_Y}}
 =:\mathcal T_k I(U,J).
 \tag{RX2}
\]

There are no derivatives of a source-dependent physical kernel in this identity. In particular, this is not a replacement of the frozen transport by differentiation of a renormalized coupling.

For the final construction the independent-coordinate radius is the radius explicitly printed in LFR I, (1.8)–(1.9), namely \(r_{\chi,k}=g_k^{-1}\delta_k\). The displayed mismatch with CMP **119**, (3.16), is analysed in [Hard cutoffs, connected insertions and marginal normalization](connected_insertions.md), Part II.B. The present proof can use any background-independent radius admitted by the unmarked regular construction; its only new small-fluctuation requirement is stated explicitly below. No mixed R region or outer-stratum boundary is added to the carrier by this note.

### 2. A usable bounded-potential insertion class

Use the source connected localization domains \(Y\in\mathfrak D_k\), with size \(d_k(Y)\). Let \(n_k(Y)\) count its \(M\)-blocks. Constants in

\[
 d_k(Y)\le n_k(Y),\qquad
 n_k(Y)\le c_n(d_k(Y)+1)
 \tag{RX3}
\]

are fixed geometric constants; the source's more precise comparison is (2.30). We retain these constants whenever volume and tree size are compared. The blocks here are \(M\)-blocks, not \(MR_k\)-blocks.

The source potential class splits a localized term into a controlled quadratic part and a bounded remainder. Only the latter is changed here. Fix the source constants with a strict reserve in that bounded remainder:

\[
 \|B_Y\|_+\le b_0e^{-p d_k(Y)},\qquad
 b_0+b_*\le b_{\rm adm},\quad b_*>0,
 \qquad p=(1-2\delta)\kappa.
 \tag{RX4}
\]

The norm \(\|\cdot\|_+\) is the supremum over the enlarged background domain used for localized potentials and over the **real retained cutoff coordinates** on the support. The constants can be fixed by performing the original source estimates with a larger allowed \(E_0\), and then making the analytic fluctuation parameter sufficiently small. This does not change the unmarked integrand. It merely leaves a known open neighborhood of that integrand inside the estimates. The ratio of the eventual activity constant to \(b_*\) is finite and independent of volume, scale, and \(g\), after this choice.

A bounded-potential root family at \(x\) is a collection \(\mathbf I=\{I_Y\}\) with these properties:

1. \(I_Y\) is local in the source variables \(U,J,A\) on \(Y\), and every nonzero \(I_Y\) contains the prescribed root \(x\), or a fixed finite protected carrier containing it.
2. \(I_Y\) is holomorphic in the same enlarged local \(U,J\) domain as \(B_Y\), uniformly for real \(A\in D_{\chi,Y}\). Measurability and boundedness in those real \(A\) variables suffice for the last Gaussian step.
3. Its explicitly defined potential norm is finite:

\[
 \mathcal N_p(\mathbf I)
 :=\sup_{Y\ni x}e^{p d_k(Y)}\|I_Y\|_+<\infty.
 \tag{RX5}
\]

A stronger weighted sum norm can of course replace (RX5). For a single insertion on \(X\), (RX5) equals \(e^{p d_k(X)}\|I_X\|_+\). The use of a local background domain is substantive: being bounded only on real physical backgrounds would not suffice for the analytic conclusion.

The source constant \(\kappa\) is chosen large enough that \(p>\log A_{\rm in}+\eta_{\rm in}\), where \(C_{\rm in}A_{\rm in}^{m+1}\) bounds the number of input localization domains containing the root with \(m\le d_k(Y)<m+1\). Thus a finite supremum norm (RX5) also gives absolute convergence of the rooted input sum. This is an input entropy reserve, separate from the output reserve (RX11).

#### Why analyticity in the fluctuation variable is not needed at this last step

Lemma 2 in CMP **116** supplies fluctuation analyticity because its potentials were produced by the preceding nonlinear localization. The proof of the final expansion needs less from the **bounded part** of a potential:

- In (2.1), the Mayer parameters multiply the local potential. They do not differentiate its \(A\) argument.
- The active support \(Y_0\) retains the factor \(\chi_{Y_0}\), as in (2.3). Hence a bounded part supported in \(Y_0\) is evaluated only on its real retained cutoff.
- In (2.5)–(2.6), the variables inside the active domain are integrated on their original real contour. The linear covariance change concerns the exterior Gaussian variables.
- The later Gaussian switches in (2.8) are outside the active carrier \(Z_0\). They enter the covariance and the conditioning operators; they do not enter a previously localized \(I_Y(U,J,A)\) with \(Y\subset Y_0\subset Z_0\).
- The estimates (2.15)–(2.26) first take an absolute bound on the bounded local potential, then estimate the remaining real Gaussian integral. The eventual Gaussian completion is a calculation of that positive majorant, not a contour shift of \(I_Y\).

Consequently the same finite-volume algebra and majorants apply to the class above. Holomorphy in \(U,J,t\) follows by dominated integration on the real contour and uniform convergence. This observation is what permits the bound on an insertion to use its actual cutoff scale \(g r_\chi\), instead of requiring the same small bound on the much larger analytic fluctuation ball of radius \(\epsilon/g\).

### 3. A source-parameter proof of the fully weighted one-root bound

For \(\mathcal N_p(\mathbf I)>0\), set

\[
 R=\frac{b_*}{2\mathcal N_p(\mathbf I)},\qquad
 V_{Y,t}=V_Y+tI_Y.
 \tag{RX6}
\]

For \(\lvert t\rvert\le2R\), (RX4) holds with \(b_{\rm adm}\) in place of \(b_0\). The quadratic potential is unchanged. Therefore the source's final expansion constructs analytic activities \(H_t(Z)\) satisfying

\[
 |H_t(Z)|_+\le h_* e^{-\beta d_{k+1}(Z)},
 \qquad
 \beta=(1-8\delta)\frac L2\kappa,
 \tag{RX7}
\]

uniformly on this entire \(t\)-disc. This is the bound of CMP **116**, Lemma 3, with the reserved bounded-potential constants. The factors from complex Gaussian normalization have already been included in \(h_*\) and the displayed exponent. In the source proof their local form is \(\exp[O(\alpha_5)|Z|]\), and the choice of constants at (2.37)–(2.38) pays them from the exponent. There is no estimate by a whole-torus density ratio.

Define the actual root activity

\[
 J_{\mathbf I}(Z)=\left.\partial_tH_t(Z)\right|_{t=0}.
 \tag{RX8}
\]

Cauchy's formula on \(\lvert t\rvert=R\) gives

\[
 \|J_{\mathbf I}(Z)\|_+
 \le\frac{2h_*}{b_*}\mathcal N_p(\mathbf I)
          e^{-\beta d_{k+1}(Z)}.
 \tag{RX9}
\]

The factor \(\mathcal N_p(\mathbf I)\) is retained exactly. The bound is homogeneous in the insertion, even if the insertion is not itself small.

#### Exact anchoring

In the Mayer construction, \(t\) occurs only in potentials \(I_Y\) whose supports contain \(x\). An activity can have a nonzero derivative only if its active potential family contains at least one such \(Y\). Its initial carrier contains \(Y\), its prescribed coarse carrier contains the corresponding coarse cover \(\bar Y\), and all subsequent Gaussian localization domains contain that carrier. Thus \(J_{\mathbf I}(Z)=0\) unless \(Z\) contains the coarse root. For a single source on \(X\), it contains the protected coarse cover \(\bar X\). This is a statement about the actual expansion, not an imposed re-labeling of an unanchored bound.

Repeated appearances of \(t\) in the exponential cause no problem: the derivative at zero selects exactly one insertion. In particular, disconnected components that do not meet it are precisely the unmarked components. They will cancel through the logarithm below.

#### Paying extension counting and the entire KP factor

Choose a polymer length

\[
 \ell(Z)=d_{k+1}(Z)+\omega,
 \tag{RX10}
\]

where the fixed \(\omega\) is large enough that \(\ell(\cup_iZ_i)\le\sum_i\ell(Z_i)\) for a connected union. The source union inequality (2.27) permits the conventional additive constant \(5\); enlarging it only changes fixed constants.

There are constants \(C_A,A_A\), independent of scale and volume, such that the number of connected coarse domains containing a fixed block and with \(m\le d(Z)<m+1\) is at most \(C_A A_A^{m+1}\). One proof chooses a canonical spanning tree of the block adjacency graph and records a depth-first traversal. Bounded graph degree bounds the number of words exponentially in the number of visited blocks; (RX3) converts block count to \(d(Z)+1\).

Take \(a(Z)=a_0n_{k+1}(Z)\), with \(a_0>0\), and a desired output exponent \(\lambda\) satisfying

\[
 \gamma:=\beta-\lambda-a_0c_n
       >\log A_A+\eta
 \qquad(\eta>0).
 \tag{RX11}
\]

Then

\[
 \begin{aligned}
 \sum_{Z\ni\bar x}
  e^{a(Z)+\lambda\ell(Z)}\|J_{\mathbf I}(Z)\|_+
 &\le
 \frac{2h_*}{b_*}\mathcal N_p(\mathbf I)
 e^{a_0c_n+\lambda\omega}
 C_A A_A\sum_{m\ge0}e^{-(\gamma-\log A_A)m}\\
 &\le C_{\rm root}\mathcal N_p(\mathbf I).
 \end{aligned}
 \tag{RX12}
\]

This sum includes the KP exponent on **every extension block**, the counting of every extension animal, and the output localization weight. A bound with merely \(\beta>\lambda\) would not establish (RX12).

The same sum without the factor \(2\mathcal N_p/b_*\) gives a uniform unmarked sum per coarse block. A polymer incompatible with \(Z\) meets one of at most \(c_{\rm touch}n(Z)\) adjacent blocks. Hence

\[
 \sum_{W\not\sim Z}|H_t(W)|_+
       e^{a(W)+\lambda\ell(W)}
 \le h_*C_{\lambda,a}\,c_{\rm touch}n(Z).
 \tag{RX13}
\]

Choose \(h_*\) sufficiently small that the right side is at most

\[
 (1-\theta)a(Z),\qquad \theta\in(0,1).
 \tag{RX14}
\]

This is strict weighted KP, uniformly in \(t\). The source permits the necessary choice of its small analytic fluctuation parameter after the localization constants have been fixed. For its usual choice

\[
 \delta=\tfrac1{10}(1-2/L),
 \qquad
 p=(0.8+0.4/L)\kappa,
 \qquad
 \beta=(0.1L+0.8)\kappa,
 \tag{RX15}
\]

there is substantial exponent reserve. The actual choice of \(L,\kappa,\lambda,a_0\) must still obey (RX11), including the geometric constants. The result does not assert preservation of an arbitrary preassigned exponent.

#### Exact normalization

The derivative of the absolutely convergent connected expansion for \(\log Z(t)\) is

\[
 \sum_{n\ge0}\frac1{n!}
 \sum_{Z_0,\ldots,Z_n}
 \phi^T(Z_0,\ldots,Z_n)
 J_{\mathbf I}(Z_0)\prod_{i=1}^n H_0(Z_i).
 \tag{RX16}
\]

The standard rooted tree induction under (RX13)–(RX14) bounds the sum over all polymers attached to fixed \(Z_0\) by \(e^{a(Z_0)}\). For completeness, majorize the connected coefficient by its rooted-tree expansion. The sum of descendant trees attached to a polymer \(Z\) is bounded inductively by

\[
 \exp\!\left\{
 \sum_{W\not\sim Z}|H_0(W)|_+
 e^{\lambda\ell(W)}e^{a(W)}\right\}
 \le e^{a(Z)}.
 \tag{RX17}
\]

Finite tree depth gives the induction; monotone convergence of the positive majorants gives the infinite-depth bound. The connected-union inequality (RX10) pays the output weight in (RX16). Grouping terms according to the connected union \(Y=\cup_i Z_i\) gives a local analytic decomposition

\[
 \mathcal T_k\Bigl(\sum_Y I_Y\Bigr)
 =\sum_{Y\ni\bar x}\mathcal E_{\mathbf I}(Y),
 \qquad
 \boxed{\displaystyle
 \sum_{Y\ni\bar x}e^{\lambda\ell(Y)}
       \|\mathcal E_{\mathbf I}(Y)\|_{\rm out}
 \le C_{\rm root}\mathcal N_p(\mathbf I).}
 \tag{RX18}
\]

This proves a fully weighted, normalized one-root operation on the class (RX5). It is stronger than assuming an individual-root activity norm: (RX12) derives that norm directly from the unmarked source expansion and an explicitly checkable input bound.

If the input potentials are jointly gauge invariant, the scalar source perturbation preserves that property. The source localization and Gaussian expansion are gauge covariant, so each coefficient in (RX18) is invariant in the same joint background atlas. Noninvariant local analytic insertions also satisfy the norm estimate; gauge invariance is needed only for later projection arguments.

### 4. Localizing an actual nonlinear minimizing-field insertion

The preceding theorem requires a local fluctuation insertion. This section proves that requirement for a useful nontrivial chart class, including finite-support observables evaluated on the actual minimizing-field response.

#### 4.1 Explicit input chart class

Let \(X_0\) be a connected protected carrier, a union of \(M\)-blocks, containing the support of an analytic function

\[
 E_X(U,J,a).
 \tag{RX19}
\]

It depends only on the restrictions of \(U,J,a\) to \(X_0\). Include in \(X_0\), once and for all, every fixed protective layer needed for the original support and for the local map \(A\mapsto B'\). Subsequent extension thickening must then be charged to extension blocks, rather than silently multiplying the prescribed-root footprint. Its norm is

\[
 M_X:=\sup_{(U,J)\in\mathcal D_X^+,\,
                     \|a\|_{\mathcal V(X_0)}<r_A}
       |E_X(U,J,a)|.
 \tag{RX20}
\]

Here \(r_A>0\) is fixed, and \(\mathcal V\) is the collection of field/regularity norms used in the source response theorem. The domain is an actual product chart tube, including all required \(J\) variables, not merely a smaller symbolic parameter label. Its background conditions are chosen to contain restrictions of the enlarged source domains on every larger localization support. Functions depending only on a fixed collection of links and plaquettes, evaluated as \(f_X((\exp i\eta a)U)\), are examples whenever their indicated tube norm is finite. Gauge-invariant examples are useful for the YM mark.

For a rooted sum of such cylinders, choose a fixed \(p_{\rm in}>p+\log C_a+1\), where \(C_a\) is the connected-extension counting constant below. A sufficient explicit norm is

\[
 \|\mathbf E\|_{\mathscr C_{p_{\rm in}},x}
 =\sum_{X\ni x}e^{p_{\rm in} n_k(X_0)}M_X.
 \tag{RX21}
\]

One may increase \(p_{\rm in}\) to pay polynomial support factors. If a different convention leaves a further multiplicative protective cost \(C_{\rm prot}\) outside \(X_0\), use \(p_{\rm in}>C_{\rm prot}p+\log C_a+1\) instead. Since \(M\) is fixed, a prescribed carrier of \(n\) blocks contains at most \(C M^4n\) independent coordinates. This is the precise support cost used below.

#### 4.2 The source switched response

In the source notation, the nonlinear minimizing-field response is

\[
 \mathcal H_k(B')
 =H_0B'+A_0-H D(H_0B'+A_0).
 \tag{RX22}
\]

The functions \(D,A_0\) solve local nonlinear equations with propagators \(H,H_0,G\). Assign a parameter \(\sigma_\Delta\) to each \(M\)-block outside the protected carrier \(X_0\). Multiplying each generalized random-walk term by the product of the parameters belonging to blocks that it visits defines \(H(\sigma),H_0(\sigma),G(\sigma)\), and hence \(\mathcal H_k(\sigma,B')\).

The proof of CMP **116**, (1.11)–(1.21), gives, for

\[
 |\sigma_\Delta|\le R_\sigma=e^{\kappa_1},
 \qquad
 B'=g_k C A-\mathfrak hD(g_k C A),
 \tag{RX23}
\]

the bound

\[
 \|\mathcal H_k(\sigma,B')\|_{\mathcal V}
 \le C_H g_k\|A\|,
 \qquad C_H=4B_0C_1e^{16\kappa_1},
 \tag{RX24}
\]

provided \(e^{32\kappa_1}g_k\|A\|\) is sufficiently small. The operator constants are uniform in the admitted complex \(U,J\) domains. The source's \(B'\) is local in \(A\). If a fixed local enlargement is needed for that locality, include it in \(X_0\).

The result is not restricted to a cubic seed. Source §1 first considers a protected cube, then explicitly uses the smallest localization domain containing a general \(X\) in the paragraph preceding (1.30). For a connected protected union, the same construction fixes its internal switches to one. Since \(1\le R_\sigma\), the operator majorant is unchanged. The local fixed-point equations continue to split along disconnected switch components.

That splitting is crucial. If all switches outside \(X_0\cup P\) are zero, the restriction of the nonlinear solution to the component meeting \(X_0\) depends only on fields and switches in that component. A mixed derivative involving a switch in another component is therefore zero. This is the actual nonlinear component argument of (1.9)–(1.10), not an inference from linear propagator decay alone.

#### 4.3 The small difference is localized as a whole

Define

\[
 F_X(\sigma;U,J,A)
 :=E_X\bigl(U,J,\mathcal H_k(\sigma,B')\bigr)
      -E_X(U,J,0).
 \tag{RX25}
\]

Suppose

\[
 C_H g_kr_{\chi,k}\le r_A/4,
 \qquad e^{32\kappa_1}g_kr_{\chi,k}\le\epsilon_H.
 \tag{RX26}
\]

A directional Cauchy estimate in the entire perturbation direction gives

\[
 \sup_{|\sigma|\le R_\sigma,\ A\in D_\chi}
 |F_X(\sigma;U,J,A)|
 \le C\frac{C_H g_kr_{\chi,k}}{r_A}M_X.
 \tag{RX27}
\]

There is no factor equal to the number of coordinates: restrict the holomorphic function in (RX20) to the one-dimensional line through its vector argument. The retained factor comes from the full difference (RX25), before any derivative is taken.

For finite volume the fundamental theorem of calculus gives exactly

\[
 F_X(\mathbf1)
 =\sum_{P\subset\sigma_0}
 \int_{[0,1]^P}
  \partial_{\sigma_P}
  F_X(\sigma_P,0_{P^c})\,d\sigma_P.
 \tag{RX28}
\]

Disconnected terms vanish by the component argument above. For a surviving set \(P\), let \(Y=X_0\cup P\), with the prescribed local thickening if required, and denote its coefficient by \(I_{X,Y}\). Cauchy's formula in each parameter on a circle of radius \(R_\sigma-1\) about its real value in \([0,1]\) yields

\[
 \boxed{\displaystyle
 \|I_{X,Y}\|_+
 \le C\frac{C_Hg_kr_{\chi,k}}{r_A}M_X
               (R_\sigma-1)^{-|P|}.}
 \tag{RX29}
\]

Every derivative hitting the insertion, every chain-rule term through the nonlinear solution, and all mixed derivatives are included in this one multivariate Cauchy estimate. There is no separate Leibniz sum to estimate. In particular, they cannot erase the factor \(g_kr_{\chi,k}\).

For a fixed \(X_0\), a support \(Y\) fixes \(P=Y\setminus X_0\); if the convention uses a fixed protective thickening, at most an exponential fixed-geometry multiplicity is introduced. Write \(c_{\rm loc}\) for that possible exponent. Since

\[
 d_k(Y)\le n_k(X_0)+c_{\rm loc}|P|+c_{\rm loc},
 \tag{RX30}
\]

choosing

\[
 \log(R_\sigma-1)>p c_{\rm loc}+c_{\rm mult}+\eta_1
 \tag{RX31}
\]

gives the pointwise potential bound

\[
 \sup_Y e^{p d_k(Y)}\|I_{X,Y}\|_+
 \le C\frac{g_kr_{\chi,k}}{r_A}
       e^{p n_k(X_0)}M_X.
 \tag{RX32}
\]

The constant includes \(C_H\) and fixed protected-layer factors. For the simplest union-of-blocks convention one may take \(c_{\rm loc}=1\) and \(c_{\rm mult}=0\).

Absolute reconstruction also needs extension counting. A connected protected set of \(n_0\) blocks has at most \(C_a^{n+n_0}\) connected extensions of \(n\) blocks. To see this, mark a spanning tree of the union, rooted at a specified block in \(X_0\), and record its depth-first traversal. Its length is at most \(2(n+n_0-1)\), and each step has a bounded number of choices. This deliberately coarse bound is sufficient. Increase the right side required in (RX31), if necessary, by \(\log C_a\). The resulting geometric series proves absolute convergence of (RX28), uniformly in volume. Its prescribed-root factor is paid by the exponential weight in (RX21), enlarged by a fixed amount if required. No extension factor is charged to the prescribed root.

Now sum the localized coefficients over the original cylinders \(X\). Equations (RX21) and (RX32) give

\[
 \mathcal N_p(\mathbf I)
 \le C\frac{g_kr_{\chi,k}}{r_A}
          \|\mathbf E\|_{\mathscr C_{p_{\rm in}},x}.
 \tag{RX33}
\]

This explicitly verifies the input norm needed in (RX18) for the nonlinear composed difference.

#### 4.4 The resulting actual regular estimate

Combine (RX18) and (RX33). Since \(E_X(U,J,0)\) is independent of the fluctuation coordinates, it exits the normalized integral exactly. We obtain

\[
 \boxed{\displaystyle
 \left\|\mathcal T_k
    \sum_X E_X\bigl(U,J,\mathcal H_k(B')\bigr)
            -\sum_X E_X(U,J,0)\right\|_{\lambda,\bar x}
 \le C\frac{g_kr_{\chi,k}}{r_A}
             \|\mathbf E\|_{\mathscr C_{p_{\rm in}},x}.}
 \tag{RX34}
\]

The output norm is the weighted local sum in (RX18). It includes full complex-background control. It is uniform in volume and UV depth on the stated regular carrier. All constants may depend on the once-fixed source constants, protected-layer conventions, and chart radius. With the final construction's polylogarithmic \(r_{\chi,k}\), the displayed perturbation tends to zero at weak coupling.

The background-dependent subtraction in (RX25) and (RX34) has **not** been thrown away as a vacuum constant. If \(E_X(U,J,0)\) depends on \(U,J\), it remains part of the transported observable. If a later renormalization removes its identity or curvature coefficients, those coefficients must be recorded separately.

The estimate is for the raw transport. A dimension-four engineering-rescaled one-step map has an additional factor \(L^4\), absorbed only into the once-fixed one-step constant. For a block of \(N\) steps, compatible input/output chart domains and local norms are required at every intermediate step, or a corresponding joint construction must be made. In a telescoping estimate the honest small parameter is

\[
 \max_{k\le j<k+N}g_jr_{\chi,j},
 \tag{RX35}
\]

and the engineering factor is \(L^{4N}\). A one-step theorem alone does not prove the return of arbitrary aged coefficients to the chart class needed for its iteration.

### 5. A concrete physical scaling check

Consider a fixed-support Wilson or clover polynomial evaluated in the minimizing-field chart. The holomorphic Wilson plaquette expression can be written using

\[
 1-\frac1{2N_c}\operatorname{tr}(P+P^{-1}).
 \tag{RX36}
\]

It has zero constant and first terms at \(P=1\). Let \(a_{\rm fine}\) be the fine mesh, \(h\) the current physical mesh, and \(\eta=a_{\rm fine}/h\). On a local chart with the source curvature and first-derivative regularity, a plaquette of \((\exp i\eta a)U\) differs from the identity by at most

\[
 C\eta^2(\alpha+r_A+r_A^2).
 \tag{RX37}
\]

This follows by multiplying its four links: the first potential differences form a discrete curl and carry the extra \(\eta\), while commutators are quadratic. Taylor's formula for (RX36) therefore gives

\[
 a_{\rm fine}^{-4}\left|1-\frac1{2N_c}
                  \operatorname{tr}(P+P^{-1})\right|
 \le C h^{-4}(\alpha+r_A+r_A^2)^2.
 \tag{RX38}
\]

Thus the chart norm of this actual insertion has the required current physical factor \(h^{-4}\), uniformly in the fine mesh. A fixed finite combination has the same bound. Applying (RX34) gives a rooted analytic estimate for its actual one-step fluctuation correction, with the \(h^{-4}\) factor retained.

This example concerns the observable evaluated on the minimizing field at the current step. At the initial step it includes the original local microscopic Wilson insertion. At subsequent steps it must not be identified with the previously transported insertion without proving that the latter has a representation in the chart class (RX20)–(RX21). That representation, together with its marginal normalization, remains part of the induction problem.

### 6. A general switched-value localization lemma

The same proof can retain a classical irrelevant gain, if that gain is uniform throughout the switch polydisc. This is useful for matching the companion classical contraction analysis, but the matching of complete domains is a separate check.

Suppose \(G_{N,X}(\sigma;B')\), formed from the source nonlinear response at depth \(N\), satisfies:

\[
 \sup_{|\sigma|\le R_\sigma,\ B'\in\mathcal B_\rho}
 |G_{N,X}(\sigma;B')|\le\mathfrak g_N(X),
 \tag{RX39}
\]

and has the component-locality property used in (RX28). Then its exact rooted localization has coefficients

\[
 \|G_{N,X;Y}\|
 \le\mathfrak g_N(X)(R_\sigma-1)^{-|P|},
 \qquad Y=X_0\cup P.
 \tag{RX40}
\]

For any output tree weight \(\lambda\) satisfying the extension-counting version of (RX31),

\[
 \sum_Y e^{\lambda d_{\rm out}(Y)}
           \|G_{N,X;Y}\|
 \le C\mathfrak g_N(X)e^{c_\lambda n_{\rm out}(X_0)}.
 \tag{RX41}
\]

The proof is exactly the Cauchy estimate and the counted geometric series above. It does not rely on every switched configuration being an actual minimizer; it uses the stated value bound and the decoupling property of the response equations.

In particular, if the complex axial-gauge/Taylor argument establishes

\[
 \mathfrak g_N(X)
 \le C\,L^{-(5-\varepsilon)N}P(d_{\rm in}(X))M_X
 \tag{RX42}
\]

uniformly on the switch polydisc, then (RX41) retains that exact gain in a tree-weighted expansion. The prescribed carrier can be coarsened by the elementary spanning-tree cover argument:

\[
 n_{\rm out}(X_0)
 \le C_d\bigl(1+L^{-N}d_{\rm in}(X)\bigr).
 \tag{RX43}
\]

Traverse a spanning tree of the input support twice, divide the traversal into segments of at most \(L^N\) input-block edges, and cover each segment by a dimension-dependent number of output blocks. Fixed protective layers change only \(C_d\). This applies to the prescribed support; the random extensions have already been paid in (RX41).

Consequently a strict input exponent reserve pays \(P(d_{\rm in}(X))\) and the coarsened footprint factor. After the engineering factor \(L^{4N}\), (RX42) gives a factor \(L^{-(1-\varepsilon)N}\), with constants uniform in \(N\) whenever the value estimate and source norms are uniform in \(N\).

The needed regularity link has a concrete source basis. CMP **99**, (3.133), and Theorem 3.12 include the field, first derivative, and localized Hölder-gradient bounds for \(H,H_1\). CMP **116**, (1.18), retains the admissible norms under its nonlinear switch construction. Before (1.19), \(B'\) is an arbitrary small variable. These facts permit the companion analysis to test (RX42) for a small complex classical input. They do not, by themselves, identify every domain and gauge transformation needed for a closed marked iteration.

#### Two interfaces that must remain visible in a joint contraction claim

First, the quantum output in (RX18) is a function of the full source pair \(U,J\). CMP **109**, (1.8), supplies a local covariant physical current \(J(U)\), and its simultaneous invariance makes \(E_X(U,J(U))\) a local invariant function on any chart where that substitution stays in the source domain. On a fixed unit lattice, a sufficiently small link chart provides such a tube, with only a fixed plaquette-ring support enlargement. The unresolved issue is the uniform pullback at arbitrary source birth depth, \(E_X(U_j(V),J_j(U_j(V)))\), in the same weighted chart norm.

The current involves a divergence of curvature. A general \(C^{1,\beta}\) field bound, with \(\beta<1\), does not give a uniform second-difference bound as the fine mesh tends to zero. CMP **99**, Theorem 3.12, explicitly excludes the covariant-Laplacian estimate for the relevant general propagators; (3.133) gives value, gradient, and Hölder-gradient control for \(H\). Thus (RX24) must not be read as an automatic uniform bound on \(J(\mathcal H_k(\sigma,B'))\). A classical contraction theorem must retain the independent auxiliary current with its correct scaling, or construct a current-preserving physical pullback/localizer. Merely omitting \(J\) changes the norm.

Second, source termwise gauge invariance is invariance in the joint background atlas: a background \(U_0\) and its perturbation transform together. Freezing \(U_0=1\) and viewing a switched response as a function of \(V=\exp iB'\) does not automatically give invariance of each coefficient under arbitrary inhomogeneous transformations of \(V\). The total unswitched physical observable remains invariant. A closed space of individually invariant localized coefficients requires either an equivariant coarse localizer or retention of the full joint atlas.

If a chosen class does have individually invariant pieces and a bounded common projection \(\Pi\) with root-local embedding \(\iota\), an insertion in \(\ker\Pi\) can be decomposed piecewise as \(f_X-\iota\Pi f_X\), because the summed extracted coefficients vanish. This observation is useful only after those boundedness and invariance statements hold. It cannot remove the linear bond jet of a noninvariant piece merely by subtracting curvature-quadratic coefficients.

### 7. Why a support cost cannot simply be dropped

There is an elementary obstruction to replacing the above support-weighted input class by arbitrary bounded functions on the real cutoff while demanding a support-independent complex-background bound.

For one real variable on \([-r,r]\), set

\[
 z_\epsilon(r)=\int_{-r}^r
       e^{-a^2/2}e^{i\epsilon a^2/2}\,da,
 \qquad
 d\mu_\epsilon(a)=z_\epsilon(r)^{-1}
       \mathbf1_{|a|\le r}e^{-(1-i\epsilon)a^2/2}\,da.
 \tag{RX44}
\]

For sufficiently small nonzero real \(\epsilon\), \(z_\epsilon\ne0\), and strict triangle inequality gives

\[
 |z_\epsilon(r)|<z_0(r).
 \tag{RX45}
\]

On \(N\) independent variables take

\[
 F_N(a)=\exp\!\left(-\frac{i\epsilon}{2}
                  \sum_{j=1}^N a_j^2\right).
 \tag{RX46}
\]

Its real-cutoff supremum is one, but

\[
 \left|\mathbb E_{\mu_\epsilon^{\otimes N}}F_N\right|
 =\left(\frac{z_0(r)}{|z_\epsilon(r)|}\right)^N
 =e^{c_{\epsilon,r}N},\qquad c_{\epsilon,r}>0.
 \tag{RX47}
\]

A radius-only weight \(e^{\lambda R}\) cannot uniformly absorb this for a filled support with \(N\asymp R^4\). This is why the local Gaussian volume factor and the corresponding input support norm in the preceding proof are meaningful.

The example is **not** a counterexample to every fixed complex physical-field norm. Writing (RX46) as \(f(gA)\) requires frequency proportional to \(g^{-2}\); the norm of that \(f\) on a fixed complex field tube can already be exponentially large. What fails is the overly broad real-cutoff-supremum-to-radius estimate. The explicit chart class (RX20) also controls a complex tube and is not refuted by this example.

### 8. What this closes and what it leaves

The following are proved on the stated full-torus regular carrier:

1. The final Gaussian/polymer construction gives a bounded normalized one-root map for the explicitly defined local bounded-potential class (RX5), including full complex-background control and every extension/KP weight.
2. The actual nonlinear minimizing-field response maps local chart cylinders to that class, with all insertion derivatives controlled and the factor \(g_kr_{\chi,k}\) retained.
3. Their composition yields (RX34), a concrete version of the analytic quantum-smallness estimate needed in the old-mark induction strategy. It is not a new abstract AO3 hypothesis.
4. The switched-value lemma (RX39)–(RX43) converts a uniform classical value gain into a tree-weighted localization bound. It identifies a direct way to reconcile the classical Hölder argument with the support cost of the quantum expansion.

The remaining work needed before applying these results to the full old-point-insertion induction is now more specific:

- Prove return to one common chart/domain norm, including the physical auxiliary-current pullback and gauge-atlas issue described above.
- Verify the complete classical irrelevant estimate in that same norm, and the bounded marginal projection and embedding used with it.
- Treat the spatial source-profile kernel, root phase, and common deterministic marginal normalization. The normalized map (RX34) does not make a point-root marginal coefficient independent of its block position.
- Extend the regular estimates to the actual mixed-history domains and compose the retained-core R bounds with the exterior conditional means.
- Carry the resulting old-insertion estimates through the S2 summation and the separate continuum reconstruction requirements.

A precise strategy for the current interface is to localize the pair consisting of the constrained minimizer and its Euler–Lagrange multiplier/current. The local constrained equations could define an analytic current extension throughout the switch polydisc, agreeing with \(J(U_j)\) at the physical unswitched point. That would avoid applying an uncontrolled extra difference to a field bounded only in \(C^{1,\beta}\). This pair-localizer is a proposed next lemma, not a result of the present note.

No claim of a full Yang–Mills existence or mass-gap proof follows from this note alone.

---

## Part IV. Complex classical contraction and the physical pullback

**Relation to Part VI:** The full current/gauge interface is formulated here. Part VI subsequently proves its current-domain and rooted-localization components on the flat-reference orbit atlas, including the joint classical gain. The invariant coarse-section return and nonflat extension remain open.

### 1. Results and scope

This note proves a complex version of the classical dimension-five gain on an explicit, restricted background domain. It does not deduce a complex bound from a bound on real fields.

The principal input is **CMP102, Proposition 9 and (190), pp.307–309**. Besides holomorphic dependence, (190) controls the first spatial derivative and its local Hölder seminorm for the response of the minimizing field. Integrating this response on a complex tube supplies the regularity needed for a direct axial-gauge calculation.

The completed results are:

1. A uniform complex \(4+\beta\) gain, \(0<\beta<1\), for a localized invariant insertion after its identity and all 21 curvature-quadratic coefficients are removed.
2. A classical contraction with gain \(L^{-(1-\epsilon)N}\), for every \(0<\epsilon<1\), in one fixed **radially weighted analytic norm**. The input and output analytic radii are the same. Constants are independent of the scale separation \(N\), once \(N\) exceeds one fixed threshold.
3. A separate analysis of the earlier minimizing-insertion Hessian estimate HT54. On a fixed admitted real regular background, its internal complex-fluctuation argument is supported by Proposition 9 and does not require the arbitrary-mark complex contraction in AO11.
4. A stronger rooted **tree-norm transfer estimate** for invariant local input pieces, using the switched nonlinear minimizing map already constructed in CMP116. The complex gain holds throughout its switch polydisc, so localization preserves that gain. Section 11 makes the input/output and gauge-domain qualifications explicit.

The classical theorem uses the coarse tube \(V=\exp(iB)\), \(\|B\|_\infty<\rho\), about the trivial coarse configuration. It is a theorem for the actual analytic minimizing map on this tube. It does not establish a uniform atlas covering every source-admitted coarse background or every history. The stronger estimate in Section 11 removes the radial-versus-volume size obstruction for the specified local input class. Matching the invariant decomposition and the source's joint background/current atlas remains necessary before combining it with the quantum theorem. Therefore the original full analytic old-mark induction is not declared closed.

### 2. The source estimate gives regularity on the complex tube

Let the coarse lattice spacing be one and the fine spacing be

\[
\lambda=L^{-N}.
\tag{CC1}
\]

Work first on a full torus admitting the source's fixed localization-block partitions, with coarse side at least four and one fixed rooted coordinate chart; constants below are independent of its volume within that admitted class. The side-length condition alone is not a substitute for compatibility with the fixed large block size \(M\). The same local statements apply in a fixed interior patch where the source hypotheses hold.

Take the reference configuration \(V_0=1\), whose minimizing field is \(U_0=1\). In the notation of CMP102 Section G, the Landau-gauge representative of the analytic minimizing field is

\[
U_N(e^{iB})=\exp\big(i\lambda\mathcal H_N(B)\big)
\quad\text{up to a gauge transformation}.
\tag{CC2}
\]

Choose one absolute radius \(\rho>0\), sufficiently small that \(\|B\|_\infty<2\rho\) lies strictly inside (172) and the smallness restrictions used by Proposition 9. This choice is independent of \(N\), the volume, and the running coupling. The group exponential is interpreted in the complexified matrix group.

In the full-torus specialization of (190), set the source's fine spacing \(\eta=\lambda=L^{-N}\) and the only block indices \(j=j'=N\). Then \(L^j\eta=L^{j'}\eta=1\). The powers \((L^j\eta)^{-1}\), \((L^j\eta)^{-2}\), and the volume factor \((L^{j'}\eta)^{-d}\) in that exact display are consequently fixed constants. The distance \(d(y,y')\) there is the block distance in these coarse units; changing to the periodic physical distance used below changes only fixed constants. The first, second, and third entries of (190) supply respectively the value, spatial-gradient, and localized Hölder estimates. For a coarse bond \(c\), the source therefore gives, with suitable fixed local cutoffs,

\[
\begin{aligned}
|D_{B_c}\mathcal H_N(B;x)|
+|\nabla_\lambda D_{B_c}\mathcal H_N(B;x)|
&\le C e^{-m d(x,c)},\\
[\nabla_\lambda D_{B_c}\mathcal H_N(B)]_{\beta;\,O(x,1)}
&\le C_\beta e^{-m' d(x,c)}.
\end{aligned}
\tag{CC3}
\]

The local Hölder estimate follows from the third entry in (190), using fixed cutoffs and, when necessary, a finite cover of the local patch. A fixed reduction of the exponential rate pays the distance between the cutoff patch and its center. These are estimates on the complex domain: Proposition 9 explicitly summarizes the preceding analytic construction and includes (190).

Since \(\mathcal H_N(0)=0\), integrate (CC3) along \(tB\), \(0\le t\le1\). The coarse-bond sum of the exponential kernel is bounded uniformly on the torus. Thus

\[
\boxed{
\|\mathcal H_N(B)\|_\infty
+\|\nabla_\lambda\mathcal H_N(B)\|_\infty
+[\nabla_\lambda\mathcal H_N(B)]_{\beta;\,\mathrm{loc}}
\le C_\beta\|B\|_\infty.
}
\tag{CC4}
\]

No real-slice maximum principle is being used. This integrates a source derivative bound already valid for complex \(B\).

For later localization, (CC3) also gives

\[
|D_{B_c}\log U_N(e^{iB})_b|
\le C\lambda e^{-m d(\lambda b,c)}
\tag{CC5}
\]

in the representative (CC2). The holomorphic principal logarithm is valid because this representative lies near the identity. Gauge-invariant insertions may be evaluated in this representative.

### 3. Direct complex axial-gauge estimate

Write \(A=\mathcal H_N(B)\). In fine lattice coordinates, let \(\mathbb B_R\) be the bond ball of radius \(R\) about the marked site. Assume

\[
\lambda(R+2)\le c_0
\tag{CC6}
\]

for a fixed small number \(c_0\). Use coordinate-ordered rooted paths to put the field in axial gauge in this ball. The transformed link is a rooted loop holonomy. Its loop has an exact factorization into at most \(C(R+1)\) elementary plaquette holonomies, conjugated by transports of length at most \(C(R+1)\). This is the discrete rooted-tree/plaquette identity, valid equally for complex matrices.

Let

\[
F_{\kappa\mu}(0)
=(\nabla_{\lambda,\kappa}A_\mu)(0)
-(\nabla_{\lambda,\mu}A_\kappa)(0)
+i[A_\kappa(0),A_\mu(0)]
\tag{CC7}
\]

with the sign convention associated with \(U=\exp(i\lambda A)\). Changing a lattice convention only changes the corresponding fixed affine map below. For a fine bond \(b=(x,x+e_\mu)\), denote the rooted axial affine field by

\[
a_F(b)=\sum_{\kappa<\mu}x_\kappa F_{\kappa\mu}(0).
\tag{CC8}
\]

The precise order of the coordinate paths fixes (CC8); a different fixed axial ordering gives an equivalent projection.

From (CC4), expansion of one complex plaquette gives

\[
\log U(\partial p)
=i\lambda^2F_{\kappa\mu}(0)
+O_\beta\!\left(
\rho\lambda^{2+\beta}(1+R)^\beta
\right)
\tag{CC9}
\]

for a plaquette within \(O(R)\) fine bonds of the root. Indeed, the linear part is the discrete curl, its variation is controlled by the Hölder bound in (CC4), and the remaining exponential-product terms are bounded by \(C\rho^2\lambda^3\). The latter are included in (CC9) for \(0<\beta<1\), \(\rho\) small, and (CC6).

A transport along the relevant paths differs from one by at most \(C\rho\lambda(R+1)\) and has uniformly bounded inverse. Its conjugation changes the leading curvature in (CC9) by at most \(C\rho^2\lambda(R+1)\). This too is bounded by the stated Hölder-scale error. The product of the at most \(C(R+1)\) plaquettes has a logarithm whose nonlinear product error is at most \(C\rho^2\lambda^4(R+1)^2\). Consequently, if

\[
b^{\rm ax}_N=\frac1i\log U_N^{\rm ax},
\]

then

\[
\boxed{
\begin{aligned}
\|b^{\rm ax}_N\|_{\mathbb B_R}
&\le C\rho\lambda^2(1+R),\\
\|b^{\rm ax}_N-\lambda^2a_F\|_{\mathbb B_R}
&\le C_\beta\rho\lambda^{2+\beta}(1+R)^{1+\beta}.
\end{aligned}}
\tag{CC10}
\]

All transports and logarithms used here are holomorphic and uniformly bounded on \(\|B\|_\infty<2\rho\). The proof uses their matrix norms, not unitarity. The constants in (CC10) do not depend on \(N\).

The gauge transformation can be defined by these rooted transports inside \(\mathbb B_R\) and set to one just outside a slightly larger ball. At the interface its logarithm is at most \(C\rho\lambda(R+1)\). If this quantity is sufficiently small compared with \(\rho\), the entire transformed configuration, including the interface bonds, remains in the input logarithm ball of radius \(\rho/2\). The interpolation obtained by exponentiating a fraction of the site's logarithmic gauge transformation remains in the same domain. Thus the use of holomorphic gauge invariance is legitimate, even for an insertion with small tails outside the axial patch.

### 4. Analytic norm and curvature projection

For a function of unit-mesh link logarithms, write

\[
f=\sum_{R\ge0}f_R,
\qquad \operatorname{supp}f_R\subset\mathbb B_R,
\]

where \(f_R\) is holomorphic on the sup-norm ball

\[
\mathcal D_\rho=\{a:\ \|a\|_\infty<\rho\}.
\]

Define the radial analytic norm

\[
\|f\|_{\rho,\kappa}^{\rm rad}
=\inf\sum_{R\ge0}e^{\kappa R}
\sup_{\mathcal D_\rho}|f_R|.
\tag{CC11}
\]

The localized pieces need not individually be gauge invariant. **The complete function is required to be gauge invariant** wherever both sides and a connecting gauge path lie in the domain. An analytic extension of a real gauge-invariant insertion has this property for small complex gauge transformations: first continue the identity in the fields, then in the gauge parameter.

Allowing noninvariant localized pieces is deliberate. Truncating external link coordinates gives simple localizers that are not individually gauge invariant, while the complete classically transported function is invariant. Global gauge invariance is sufficient for the Taylor cancellations used below.

For a compact simple gauge group, invariance under constant conjugation implies

\[
Df(0)=0.
\tag{CC12}
\]

Every individual bond coefficient of this differential would otherwise be a nonzero invariant linear functional on the Lie algebra. Define

\[
Q_f(F)=\tfrac12D^2f(0)[a_F,a_F].
\tag{CC13}
\]

Although \(a_F\) grows linearly in distance, (CC13) is well-defined on (CC11): for a piece of radius \(R\), directional Cauchy estimates bound its contribution by

\[
C\rho^{-2}(1+R)^2
\sup_{\mathcal D_\rho}|f_R|\,|F|^2.
\tag{CC14}
\]

The exponential norm absorbs this polynomial. On a torus use the fixed rooted fundamental coordinate chart; the small patches used in (CC10) do not wrap. The far-support estimate (CC14) is uniform for this convention.

Constant-conjugation invariance reduces the color tensor in (CC13) to the invariant bilinear form of the simple algebra. The remaining symmetric form on the six curvature labels has **21 coefficients**. No Euclidean invariance of the point mark is assumed.

There is a bounded local projection \(P\) with range consisting of the identity and these 21 coefficients. To construct it, represent each curvature label by a fixed rooted plaquette logarithm, or another holomorphic covariant plaquette field with the same linear jet, and use their invariant bilinear products. These representatives have fixed support and reproduce (CC13). Together with (CC14), this proves

\[
\|Pf\|_{\rho,\kappa}^{\rm rad}
\le C_{\rho,\kappa}\|f\|_{\rho,\kappa}^{\rm rad},
\qquad P^2=P.
\tag{CC15}
\]

The constants are independent of \(N\) and volume. The kernel condition is

\[
f(0)=0,\qquad Q_f=0.
\tag{CC16}
\]

These are the identity and all 21 curvature jets, not all quadratic bond derivatives.

### 5. Complex value gain

#### 5.1 Finite-support insertion

Suppose first that \(f\) is supported in \(\mathbb B_R\), is gauge invariant, and satisfies (CC16). Evaluate it in the axial gauge of Section 3. Its linear Taylor term vanishes by (CC12). Directional Cauchy estimates on the input ball give a cubic remainder bounded by

\[
C\sup_{\mathcal D_\rho}|f|
\lambda^6(1+R)^3.
\tag{CC17}
\]

Replacing \(b_N^{\rm ax}\) by \(\lambda^2a_F\) in its quadratic Taylor term costs, by (CC10), at most

\[
C_\beta\sup_{\mathcal D_\rho}|f|
\lambda^{4+\beta}(1+R)^{2+\beta}.
\tag{CC18}
\]

The remaining quadratic term is \(\lambda^4Q_f(F)=0\). Thus

\[
\boxed{
\sup_{\|B\|_\infty<2\rho}
|f(U_N(e^{iB}))|
\le C_\beta\lambda^{4+\beta}(1+R)^{3+\beta}
\sup_{\mathcal D_\rho}|f|.
}
\tag{CC19}
\]

The displayed polynomial has been harmlessly enlarged. For any fixed \(R\), the constants are independent of \(N\); the required lower threshold for \(N\) makes the gauge and Cauchy margins in Section 3 valid.

#### 5.2 Exponentially localized insertion

Let now \(f\) satisfy (CC11), gauge invariance, and (CC16). Choose

\[
R_N=\lceil aN\rceil,
\qquad
\frac{\kappa a}{2}>(4+\beta)\log L.
\tag{CC20}
\]

For one fixed sufficiently large \(N_0\), every \(N\ge N_0\) satisfies \(\lambda(R_N+2)\ll1\). Apply one common axial gauge inside \(\mathbb B_{R_N}\), extending it to the identity outside the patch as above. The transformed whole configuration remains in \(\mathcal D_{\rho/2}\).

For pieces with \(R\le R_N\), expand in this common axial field. The pieces need not separately have zero linear jet: their sum's linear term is minus the tail's linear term, by (CC12), and that tail is bounded using Cauchy and the input exponential weight. Similarly,

\[
\sum_{R\le R_N}Q_{f_R}(F)
=-\sum_{R>R_N}Q_{f_R}(F)
\tag{CC21}
\]

because \(Q_f=0\). Identity coefficients cancel in the same way. The tail costs at most

\[
C\sum_{R>R_N}(1+R)^2
\sup|f_R|
\le C_\kappa e^{-\kappa R_N/2}
\|f\|_{\rho,\kappa}^{\rm rad}.
\tag{CC22}
\]

The sum of the small-support Taylor errors in (CC17)–(CC18) is bounded by the same norm times \(C_{\beta,\kappa}\lambda^{4+\beta}\), because its exponential weight absorbs every fixed power of \(R\). Equations (CC20)–(CC22) prove

\[
\boxed{
\sup_{\|B\|_\infty<2\rho}
|f(U_N(e^{iB}))|
\le C_{\beta,\kappa}\lambda^{4+\beta}
\|f\|_{\rho,\kappa}^{\rm rad},
\quad N\ge N_0.
}
\tag{CC23}
\]

This is an actual complex-domain gain with an \(N\)-independent constant. Its derivation uses (CC3), complex plaquette algebra, and complex Cauchy estimates, rather than the real estimate (3.67).

### 6. Closing the classical radial norm with the same radius

Set

\[
G_N(B)=f(U_N(e^{iB})).
\]

For a coarse bond \(c\), (CC5) and a directional Cauchy estimate for \(f_R\) on the input ball imply

\[
|D_{B_c}(f_R\circ U_N)|
\le C\lambda\rho^{-1}\sup|f_R|
e^{-m d(c,\lambda\mathbb B_R)}.
\tag{CC24}
\]

There is no factor equal to the number of fine bonds: the norm of the differential as a functional on the sup-norm ball is bounded by \(C\sup|f_R|/\rho\). Equivalently, the sum of its component derivative norms is controlled by a dimension-independent directional Cauchy estimate, up to the fixed Lie-algebra dimension.

Let \(B^{[s]}\) retain only coarse bonds in the rooted ball of radius \(s\), setting the others to zero. The line segment between \(B\) and \(B^{[s]}\) remains in the coarse tube. Summing (CC24) over removed bonds, and splitting the input supports at \(R=s/(2\lambda)\), yields

\[
\sup_{\|B\|_\infty<\rho}
|G_N(B)-G_N(B^{[s]})|
\le C_\kappa e^{-\sigma s}
\|f\|_{\rho,\kappa}^{\rm rad}.
\tag{CC25}
\]

The constants can be chosen with a fixed \(\sigma>0\) determined by the response rate in (CC5), once \(N_0\) is large enough that \(\lambda\) is sufficiently small relative to \(\kappa\). Polynomial lattice-volume factors in the coarse-bond sum are absorbed by a fixed decrease of \(\sigma\). This remains uniform on finite tori.

Use the telescoping localizers

\[
g_{N,s}(B)=G_N(B^{[s]})-G_N(B^{[s-1]}),
\qquad s\ge1,
\tag{CC26}
\]

with the initial truncated field chosen to be zero. A harmless fixed shift of the radius includes endpoint bonds. Since \(f(0)=0\), \(G_N(0)=0\), and the sum of (CC26) is \(G_N\). Each term has coarse support radius \(s+O(1)\) and is holomorphic on \(\mathcal D_\rho\).

By (CC23) and (CC25), each term is bounded both by

\[
C\lambda^{4+\beta}\|f\|_{\rho,\kappa}^{\rm rad}
\quad\text{and by}\quad
C e^{-\sigma s}\|f\|_{\rho,\kappa}^{\rm rad}.
\]

Interpolating these two numerical bounds gives, for \(0<\theta<1\),

\[
\sup|g_{N,s}|
\le C\lambda^{(4+\beta)(1-\theta)}
e^{-\sigma\theta s}\|f\|_{\rho,\kappa}^{\rm rad}.
\tag{CC27}
\]

Given \(0<\epsilon<1\), take

\[
\beta=1-\epsilon/2,
\qquad
\theta=\frac{\epsilon/2}{5-\epsilon/2},
\qquad
0<\kappa<\sigma\theta/2.
\tag{CC28}
\]

Choose \(N_0\) after these parameters; this removes the apparent dependence of the achievable decay rate in (CC25) on a small input \(\kappa\). Then summation of (CC27) in the same radial norm proves

\[
\boxed{
\|G_N\|_{\rho,\kappa}^{\rm rad}
\le C_\epsilon\lambda^{5-\epsilon}
\|f\|_{\rho,\kappa}^{\rm rad},
\qquad f\in\ker P,\quad N\ge N_0.
}
\tag{CC29}
\]

Both norms use the same fixed radius \(\rho\). The source map is evaluated on the larger coarse tube \(2\rho\); its fine image is strictly inside the input radius \(\rho\) for \(N\ge N_0\). Thus no analytic-radius loss accumulates under iteration of the fixed classical block.

The full \(G_N\) is gauge invariant by the source covariance (181), even though its localizers (CC26) are not separately invariant. More precisely, use a small coarse gauge path remaining in the tube. Source (181), including its stated analytic continuation on p.307, says that the derivative of the minimizing field along this path is a fine gauge tangent. At every point the representative (CC2) is in the interior of the input analytic domain, so the gauge differential of \(f\) annihilates that tangent. Integration along the path proves the invariance of \(G_N\). This argument does not assume that an arbitrary finite block-constant gauge transformation keeps every fine link inside the small logarithm ball. The separate axial gauge used in Sections 3 and 5 does have the explicit small path verified there.

Apply the bounded projection (CC15), and restore the engineering factor \(\lambda^{-4}\). For

\[
\widehat T^{(N)}_0f=\lambda^{-4}f\circ U_N,
\]

one obtains the restricted classical operator theorem

\[
\boxed{
\|(1-P)\widehat T^{(N)}_0|_{\ker P}\|_{
\rho,\kappa}^{\rm rad}
\le C_\epsilon L^{-(1-\epsilon)N}.
}
\tag{CC30}
\]

The constants are fixed before \(N\) is chosen. Hence one fixed sufficiently large block really does make this operator norm smaller than \(1/2\).

#### Finite torus conventions

Every \(\mathbb B_R\) means its intersection with the finite torus, measured in periodic rooted distance. Once \(R\) exceeds the diameter, it is the whole lattice. Use fixed fundamental representatives for the affine test (CC8), assigning a value to every bond, including wrapping bonds. On a piece of radius \(R\), these values still satisfy \(|a_F|\le C(1+R)|F|\), so (CC14) and every tail bound are unchanged. The axial patch \(R_N\) is nonwrapping because \(\lambda R_N\ll1\) and the coarse side is at least four. Output truncations (CC26) stop once the whole coarse torus has been retained. This proves volume uniformity without postulating an affine nonzero-curvature periodic connection.

### 7. What this closes, and why the stronger norm is still a task

Equation (CC30) is an actual same-radius classical contraction on its stated complex tube and radial Banach space. It establishes a restricted form of the classical estimate sought in AO11. It also gives a uniform complex estimate for every fixed finite source footprint through (CC19).

There are three distinct extensions that it does not establish.

**The source background atlas.** The tube is based at \(V_0=1\). Proposition 9 also allows increments about a real admitted minimizing background. Its covariant response and the real background's local regularity are promising inputs to corresponding local value estimates. A single compatible analytic atlas, its localization maps, and the transition/gauge estimates for every source-admitted background have not been constructed here. In particular, small plaquettes on a torus do not by themselves imply a global small-link chart about the identity.

**The precise old-scale map.** The proof uses the explicit minimizing map \(U_N\) of the variational problem. In the full source induction, an old variable can instead be an average \(M^jU_k\) of a minimizing field of the original finer action. Applying this theorem to each such map requires verifying the corresponding analytic averaging/map identification and the uniform form of (CC3)–(CC5). This is not supplied by simply calling a repeated classical coarse minimization the same map. The theorem applies to any identified family satisfying these displayed estimates, and its radius/norm constants then do not accumulate.

**Compatibility with the quantum insertion norm.** The currently established generic complex root estimate has a prescribed-support cost of the form \(e^{p d(X)}\), where \(d(X)\) is a connected localization-block tree size. For a filled four-dimensional ball this can be of order its volume, \(R^4\). The radial weight \(e^{\kappa R}\) cannot absorb that available bound for arbitrary ball-supported pieces. Thus (CC30) plus that quantum estimate is not a closed induction in one norm.

The complex truncated-Gaussian example discussed in the companion work shows that a generic estimate based only on the real-cutoff supremum can indeed have exponential volume cost. Its test insertion has a growing supremum on a fixed complex fluctuation tube; it therefore does not, by itself, prove that every stronger holomorphic input-field norm with analytic reserve has an unbounded quantum operator. The conclusion used here is the precise one: **the available quantum support bound does not close the radial classical norm**.

### 8. A concrete route from radial response to rooted trees

The stronger classical localization should be attacked through the implicit minimizing equation, not by repeatedly differentiating the single response bound (190) with an unweighted Cauchy estimate.

The direct higher-response program below remains useful for more general charts and maps. Section 11 records an additional source-specific advance: CMP116 has already constructed a switched version of this implicit equation, sufficient for a strong localized transfer estimate on the restricted tube used here.

#### 8.1 The actual equation and its differentiated vertices

CMP102, pp.305–307, gives

\[
\mathcal H(B)=a_0+H_0B-H D(a_0+H_0B),
\tag{CC31}
\]

with \(a_0\) solving (180). Put \(X=a_0+H_0B\). At a fixed reference background, (180) has the form

\[
X+G V'(X)=K B,
\qquad K=(I+GA^{(2)})H_0,
\tag{CC32}
\]

using the source's already modified \(G\). The simpler Landau representation (174)–(175) has the corresponding formula with its own \(G,H_1\). Here \(V\) is the actual nonlinear action remainder used in the variational equation, and \(D\) is the analytic constraint-linearizing correction; they are not arbitrary newly introduced potentials.

Let

\[
R_X=(I+GV''(X))^{-1}.
\]

Then

\[
DX=R_XK,
\tag{CC33}
\]

and repeated differentiation gives, for \(m\ge2\),

\[
D^mX
=-R_XG
\sum_{\substack{\pi\text{ a partition of }\{1,\ldots,m\}\\|\pi|\ge2}}
V^{(|\pi|+1)}(X)
\big[D^{|B_1|}X,\ldots,D^{|B_{|\pi|}|}X\big].
\tag{CC34}
\]

The derivative labels in each block of the partition are retained. The output map (CC31) adds the analogous partitions for \(D^{(q)}(X)\) followed by the exponentially localized operator \(H\).

The source establishes the small inverse used here at first-response order in (186)–(190). The analytic averaging correction itself obeys the earlier implicit linearization equation, of the form

\[
D(X)=\mathcal C(X-H D(X)),
\tag{CC35}
\]

where \(\mathcal C\) is the nonlinear part of the group averaging operation. Its differentiated inverse and vertices must be included in the tree construction; omitting them would replace the actual constraint by its linearization.

#### 8.2 The specific estimates to prove

A rooted-tree proof needs uniform, normalized spatial multilinear bounds for:

- The edges \(G,H,H_0,K,R_XG\), in the source's weighted block-field norms.
- The averaging vertices \(\mathcal C^{(q)}\), including all normalized fine-bond sums inside one current block.
- The action vertices \(V^{(q+1)}\), with their plaquette, averaging, and constraint-correction dependence retained.
- The resulting \(D^{(q)}\) vertices in (CC31).

The desired bound has factorial analytic control and a connected spatial tree through the output and all input labels. Fine lattice sums must use the source's normalization so that no factor \(\lambda^{-d}\) remains merely because a coarse block contains many fine bonds. Iterating (CC34) then sums rooted trees; an analytic majorant controls their order factorials. A fixed small field radius provides the smallness for the nonlinear inverse.

This is a concrete finite list of vertices and inverses tied to the actual source equation. **The all-order tree bounds for this list are not proved by (190) alone.** Cauchy estimates applied to a single exponentially localized response preserve decay to a selected derivative label, or after symmetrization the farthest label. They do not automatically produce the tree length joining every label.

#### 8.3 Combining strong localization with the value gain

Suppose the resulting rooted localization gives linear localizers \(\mathscr L_Y\) with

\[
\|\mathscr L_Y G\|\le C_{\rm loc}^{|Y|}\sup|G|
\tag{CC36}
\]

and an independent tree-locality bound

\[
\|\mathscr L_Y(f\circ U_N)\|
\le C\|f\|_{\rm in} e^{-a d(Y)}
\tag{CC37}
\]

with the necessary input-support weights and constants uniform in \(N\). Möbius-type finite-set localizers have a bound of the form (CC36); the substantive missing result is (CC37) with sufficiently large decay reserve for the actual nonlinear minimizer.

Combining (CC23), (CC36), and (CC37) by numerical interpolation preserves a slightly weaker power \(\lambda^{5-\epsilon}\), while yielding the decay exponent

\[
a\theta-(1-\theta)\log C_{\rm loc}
\tag{CC38}
\]

per localization size, before paying set entropy and the desired output weight. One must verify this exponent is large enough, for example by the source's choice of localization blocks and analytic smallness. This states the needed norm balance explicitly; a small bound on the total function does not by itself make each localized activity small.

For maps without an applicable switched construction, this remains an identified proof task. For the specific map on the trivial-background tube, the source's switched construction gives the more direct estimate proved in Section 11.

### 9. Direct justification of the minimizing-mark Hessian HT54

#### 9.1 What Proposition 9 actually asserts

The source's final statement on p.309 says that the minimizing field has a holomorphic extension in small complex coarse increments \(V'\), that the relative field in Landau gauge is \(\exp(i\eta\mathcal H(B))\), and that its functional derivative satisfies (190). It also describes analytic dependence on an external regular background, but that latter extension is not needed for the internal Hessian estimate at a fixed real carrier.

Take a fixed admitted real regular background \(U_0\). Choose an absolute small source parameter \(\epsilon_1\) that bounds its regularity and allows a fixed complex increment tube. The source can be applied with this upper bound even when the actual background regularity \(\epsilon_{\rm bg}\) is much smaller. The constants remain fixed. The actual background's smallness need not be artificially used as the radius of the perturbation tube.

The independent fluctuation coordinates enter through the analytic source map

\[
B'(A)=g C A-hD(g C A).
\tag{CC39}
\]

Its analyticity, bounded constraint embedding, and localized derivative are separate previously checked inputs from CMP109/116. To make the domain statement explicit, choose a fixed \(\epsilon_{\rm ana}>0\), small relative to the absolute source constants, such that

\[
\|A\|_\infty<\rho_A:=c\epsilon_{\rm ana}/g
\quad\Longrightarrow\quad
\|B'(A)\|_\infty<C_1\epsilon_1
\tag{CC40}
\]

inside (172), with a fixed margin. Also require \(\epsilon_{\rm bg}\le c'\epsilon_{\rm ana}\). On the actual real cutoff, \(r_\chi\le\rho_A/4\) follows for small coupling from the later source's polylogarithmic radius. These inclusions must be made for the same real carrier and coordinate map; they are not an assertion about every mixed-history chart.

#### 9.2 The complex plaquette estimates needed here

Let \(a\) be the physical fine spacing and \(h\) the current coarse spacing, and set \(\eta=a/h\). The value and first spatial derivative entries of (190), together with the fixed real background's regularity, imply on (CC40)

\[
|P_x(A)-I|\le C\epsilon_{\rm ana}\eta^2,
\qquad
|\partial_{A_i}P_x(A)|
\le Cg\eta^2 e^{-c d(x,i)/h}.
\tag{CC41}
\]

For clarity about the first estimate, integrate the complex response from \(A=0\) and combine it with the admitted background plaquette bound. For the second, take the plaquette product derivative: opposite edges cancel the constant increment, leaving its discrete covariant derivative and bounded commutator terms. Both are controlled by the first two entries of (190). Compose with the localized derivative of (CC39). Products and conjugations are uniformly bounded on the fixed small complex tube. No Hölder estimate, arbitrary-input renormalization, or real-to-complex inference is required for (CC41).

For the scalar Wilson insertion, the holomorphic continuation is

\[
F_x(A)=a^{-4}\left[N_c-\tfrac12\operatorname{tr}
\big(P_x(A)+P_x(A)^{-1}\big)\right].
\tag{CC42}
\]

Its differential is bounded by \(Ca^{-4}|P-I|\,|\dot P|\). Equations (CC41) therefore give

\[
|\partial_{A_i}F_x(A)|
\le Cg\epsilon_{\rm ana}h^{-4}e^{-c d(x,i)/h}
\tag{CC43}
\]

throughout a fixed smaller complex polydisc. The same argument applies to the source's clover/leaf quadratic invariant insertions using their holomorphic plaquette fields.

Cauchy in coordinate \(A_j\), with radius a fixed fraction of \(\rho_A\), proves on the real cutoff

\[
|\partial_{A_j}\partial_{A_i}F_x|
\le Cg^2h^{-4}e^{-c d(x,i)/h}.
\tag{CC44}
\]

Exchange \(i,j\), use symmetry of the Hessian, and use
\(\tau(x,i,j)\le2\max\{d(x,i),d(x,j)\}\). This gives exactly the form

\[
\boxed{
|\partial_{A_j}\partial_{A_i}F_x|
\le Cg^2h^{-4}e^{-c'\tau(x,i,j)/h}.
}
\tag{CC45}
\]

#### 9.3 Status of HT54

HT54 is supported for the **actual minimizing insertion at a fixed admitted real regular background**, provided the explicit coordinate-domain inclusion (CC40) and the already checked coordinate-map bounds hold. This justification uses Proposition 9 in its stated complex increment domain. It does not rely on the unproved extension of AO11 to arbitrary rooted marks over a complete background atlas.

The sharper moment and covariance corollaries of HT54 keep their other hypotheses: the complete regular carrier's drift and coercivity bounds, its actual cutoff, and the matching mark/background coordinates. This justification does not promote HT54 to an old transported mark, to arbitrary coarse-background derivatives, or to every multiscale history.

### 10. Source record

- **Balaban, CMP102 (1985), 277–309**: Theorem 1, (8)–(10), p.279; relative-field conditions (19)–(21), p.281; analytic increment domain (172), p.305; implicit minimizing equations (174)–(180), pp.305–306; complex gauge covariance (181), p.307; response equation and inverse (182)–(188), pp.307–308; response bounds (190), p.308; Proposition 9, p.309.
- **Balaban, CMP119 (1988), 243–285**: (3.67)–(3.72), pp.283–284, gives the earlier real-background mechanism and the rooted axial-gauge strategy. The complex proof here instead starts from the explicit complex response bound in CMP102.
- **Balaban, CMP99 (1985), 389–434**: Theorem 3.10 and (3.107)–(3.108), pp.415–416; the value/gradient/Hölder estimate (3.133), p.422; Theorem 3.12, p.423, and the explicit discussion of Hölder-dependent constants on p.424. These identify the regularity norms in the switched construction.
- **Balaban, CMP109 (1987), 249–301**: (1.8)–(1.19), pp.261–263, defines the physical current, its joint gauge action, and the invariant analytic orbit domain; p.263 explains the inclusion of sufficiently regular physical pairs and uses absolute analytic constants in the full-torus small-field construction. This is the source interface used in Section 12.
- **Balaban, CMP116 (1988), 1–22**: Section 1, especially (1.2)–(1.18), constructs the switched nonlinear minimizing map with an arbitrary small input \(B'\). Substitution of the independent fluctuation map occurs only in (1.19). Equations (1.9)–(1.10) give rooted component localization. These are the additional inputs used in Section 11.
- The independent-coordinate map and its regular analytic domain are the inputs verified in the cutoff-covariance, Hessian-transport, and cutoff-radius parts (Parts I, III and II.B) of [Hard cutoffs, connected insertions and marginal normalization](connected_insertions.md).

**Remaining bridge:** verify the actual map/atlas at each old scale, the coarse-gauge interpretation of localized coefficients, and its compatibility with the quantum insertion theorem. The restricted complex classical contraction itself, including its uniform constants and fixed radius, is proved above; a strong localization upgrade for the specified input class follows next.

### 11. Matched switched construction: a stronger tree-norm transfer

#### 11.1 The source's switched map matches the required regularity

CMP116 (1.2)–(1.4) explicitly takes the nonlinear minimizing map from CMP102 Section G. It replaces its propagators by their random-walk expansions with switches outside a protected root. The input \(B'\) is arbitrary and small at this stage; the fluctuation substitution (1.19) has not yet been made. Thus, with reference \(U_0=1\), \(B'=B\), \(k=N\), and fine spacing \(\eta=L^{-N}\), this is the same map used above, now denoted

\[
\mathcal H_N(s,B).
\tag{CC46}
\]

The source bounds this map uniformly for \(|s_\Delta|\le e^{\kappa_1}\), provided \(e^{32\kappa_1}\|B\|\) is sufficiently small. The bound is of size \(C e^{16\kappa_1}\|B\|\) in all admissible regularity norms. The needed Hölder norm is specifically among them: CMP99 (3.133) controls \(H,\nabla H,\zeta\nabla H\) in the \(\beta\)-Hölder norm, and Theorem 3.12 transfers the random-walk construction of Theorem 3.10 to these minimizer operators. All block-scale powers are one when \(j=j'=N\), \(\eta=L^{-N}\).

Choose \(\kappa_1\), the localization-block size, and then one fixed \(\rho\) satisfying these switched-domain restrictions. On \(\|B\|<2\rho\), the analogue of (CC4) holds for every allowed complex switch configuration, with a fixed larger constant \(C_{\beta,\kappa_1}\). Therefore the axial-gauge and Taylor argument of Sections 3 and 5 works **throughout the switch polydisc**. The switched field need not itself be a constrained minimizer: those arguments use the verified complex \(C^{1,\beta}\) bound and the gauge invariance of the input function, not the variational equation of the switched field.

For a root-supported invariant input \(q_X\) with \(Pq_X=0\), and with radius small enough compared with \(\lambda^{-1}\), this gives

\[
\sup_{s,B}|q_X(e^{i\lambda\mathcal H_N(s,B)})|
\le C\lambda^{4+\beta}(1+\operatorname{diam}X)^q
\sup_{\mathcal D_\rho}|q_X|,
\tag{CC47}
\]

for a fixed polynomial power \(q\). The constants are independent of \(N\). The lower threshold for \(N\) is chosen after the fixed switched constants.

#### 11.2 Cauchy preserves the gain on connected activities

Let \(S_N(X)\) be a connected protected set of current localization blocks covering the rescaled input support and a fixed collar. Let \(n_0=|S_N(X)|\). Apply the source fundamental-theorem-of-calculus switch expansion outside this protected set. The source's component argument implies that derivatives in components not connected to the protected set vanish. This statement extends from its displayed protected cube to a connected union of protected blocks: omitting additional switches does not worsen the complex operator bound, and the separated component equations remain the same.

For a set \(P_s\) of \(n\) differentiated switches connected to the root, Cauchy's formula, centered at the real interpolation points in \([0,1]\), gives

\[
\|K_{X,P_s}\|
\le G_N(X)(e^{\kappa_1}-1)^{-n},
\tag{CC48}
\]

where \(G_N(X)\) is the uniform value bound in (CC47), or the trivial bound when the input support is too large for that estimate. The integration lengths are one and each switch is differentiated once. There is no derivative factorial in this bound.

Counting connected extensions and paying a fixed output tree weight gives

\[
\sum_Y e^{\kappa d_{\rm out}(Y)}
\sup_{\mathcal D_\rho}|K_X(Y)|
\le C e^{p n_0}G_N(X),
\tag{CC49}
\]

once \(\kappa_1\) and the block size are fixed sufficiently large. The constants \(p,C\) include the root footprint, set entropy, collar enlargement, and the prescribed output exponent. All are fixed before \(N\). This is the source's root-connected localization mechanism applied to the gained integrand, rather than localization of a large bound followed by an inference from cancellation of the total sum.

#### 11.3 Input support weights pay the protected footprint

Suppose the input has a rooted decomposition into **individually gauge-invariant** analytic pieces,

\[
f=\sum_{X\ni0}f_X,
\qquad
\|f\|_{\rho,\kappa}^{\rm tree,inv}
=\inf\sum_X e^{\kappa d_{\rm in}(X)}
\sup_{\mathcal D_\rho}|f_X|.
\tag{CC50}
\]

Here the connected input supports are measured in fixed old-scale localization blocks. At the output scale the same block size is used. A connected geometric tree covering an input support, rescaled by \(\lambda\), gives

\[
n_0\le C_0\big(1+\lambda d_{\rm in}(X)\big).
\tag{CC51}
\]

To verify (CC51), cover the rescaled connected tree by current blocks. The number of distinct blocks met by a connected curve is bounded by a constant times one plus its length in current-block units; a fixed collar changes only the constant. This bound also covers filled supports, since a connected spanning tree has length comparable with their block count. It does not assume that every support is a filled cube.

When \(Pf=0\), replace each piece by

\[
q_X=(1-P)f_X.
\tag{CC52}
\]

Their sum is still \(f\), and each piece now has the vanishing jets needed in (CC47). The projection only adds a fixed local rooted support and a polynomial cost in \(d_{\rm in}(X)\), as follows from (CC14). This polynomial will be paid by the scale change; one need not assert that the termwise operation is bounded on the unmodified weighted decomposition before scaling.

Choose \(N_0\) large enough that

\[
p C_0 L^{-N}\le\kappa/4,
\qquad N\ge N_0.
\tag{CC53}
\]

Split supports at \(d_{\rm in}(X)=aN\), with \(a\) fixed and sufficiently large.

For \(d_{\rm in}(X)\le aN\), the input support fits in the small physical axial patch when \(N\ge N_0\). Apply (CC47). Its polynomial support factors, the projection cost, and \(e^{p n_0}\) in (CC49) are bounded by a constant times the available \(e^{\kappa d_{\rm in}(X)}\) weight, using (CC51)–(CC53). The result retains \(\lambda^{4+\beta}\).

For \(d_{\rm in}(X)>aN\), use the trivial analytic bound for \(q_X\circ U_N(s)\). The input exponential weight left after (CC53) and the projection polynomial contributes

\[
e^{-\kappa aN/2}\le L^{-(4+\beta)N}
\tag{CC54}
\]

if \(a\) was chosen accordingly. Thus these supports also give the required gain.

Summing the resulting connected activities yields the strong transfer estimate

\[
\boxed{
\|f\circ U_N\|_{\rho,\kappa}^{\rm tree,out}
\le C_{\beta,\kappa}\lambda^{4+\beta}
\|f\|_{\rho,\kappa}^{\rm tree,inv},
\qquad Pf=0.
}
\tag{CC55}
\]

The output norm is the infimum over the rooted localized activities just constructed. Without an additional coarse-gauge identification, the notation does **not** require each activity to be separately invariant under inhomogeneous transformations of \(V=e^{iB}\) at fixed reference \(U_0=1\). The total function is invariant. Equation (CC55) is therefore stated as a transfer estimate between precisely specified input and output classes.

After applying the bounded physical curvature projection to the total function and restoring the engineering factor, the corresponding estimate is \(C_{\beta,\kappa}L^{-\beta N}\). Taking \(\beta=1-\epsilon\) gives the sought exponent without the small interpolation loss used for the radial theorem.

#### 11.4 What remains before calling this one closed source norm

The source switch construction is covariant in its **joint** external background variables and relative fluctuation. It is not automatic that its individual activities, restricted to the section \(U_0=1\), are invariant under every inhomogeneous coarse transformation of \(V=e^{iB}\). Such a transformation changes the reference background as well. A common invariant-decomposition norm must either keep that joint atlas, use a verified covariant localizer, or prove a compatible conversion of decompositions. The strong activity estimate (CC55) does not silently supply this identification.

There is also a useful partial observation about the auxiliary current \(J\). On a genuine **unit-mesh** chart, the physical map \(U\mapsto J_{\rm unit}(U)\) is finite-range and holomorphic, with

\[
\|J_{\rm unit}(e^{ia})\|\le C\|a\|,
\tag{CC56}
\]

for small \(a\). Therefore a local analytic source \(E_X(U,J)\) may be pulled back to \(f_X(U)=E_X(U,J_{\rm unit}(U))\) after choosing \(\rho\) inside the joint domain. The physical gauge covariance of \(J\) makes this pullback gauge invariant, and its support enlarges by only a fixed collar. In a nonwrapping chart, with the affine field (CC8) extended across the entire current stencil, its constant linearized curvature gives zero linearized current. Thus the full-21 physical projection remains the appropriate local quadratic projection for this pullback; the direct Taylor proof includes its current dependence. Wrapping supports use the finite-torus and tail qualification stated in CC59 and made explicit in Part VI after CP28.

This unit-mesh observation does not justify replacing a physical current containing inverse powers of an underlying spacing \(\xi\) by a uniformly bounded map on an arbitrary link polydisc. For source activities whose \(U\) still lives on \(\xi\ll1\), the current-unit/minimizer chart must first be matched. The source's actual minimizing field has additional current estimates in (19) and (190), but one must not infer all of them for arbitrary switched fields solely from (3.133): CMP99 explicitly excepts certain covariant-Laplacian estimates. The present strong gain needs only the verified \(C^{1,\beta}\) norm for physical unit-link insertions.

**Net advance:** the complex value gain and a rooted tree-localization estimate have now been proved together on the explicitly matched trivial-background tube. The remaining issue for the full old-mark induction is the uniform physical pullback specified next, rather than an unspecified lack of any complex classical power gain.

### 12. The remaining physical atlas estimate, with the birth index retained

#### 12.1 Established unit-current pullback lemma

At mesh one, the physical current is a fixed-range holomorphic expression in the links and their inverses: take the source covariant divergence of the Lie-algebra projection of the antisymmetric plaquette part. The latter is continued as \((P-P^{-1})/(2i)\). Each bond current is a sum of a fixed number of these terms and their bounded transports. Consequently, for one absolute small \(\rho_0\),

\[
\sup_{\|a\|_\infty<\rho}|J_{\rm unit}(e^{ia})|
\le C\rho,
\qquad 0<\rho\le\rho_0,
\tag{CC57}
\]

with constants depending only on the fixed dimension and group. The map enlarges support by a fixed plaquette collar and is covariant under the source's local gauge transformations. These statements follow directly from the finite expression; no continuum estimate is required.

If \(E_X(U,J)\) is holomorphic and gauge invariant on a joint domain containing these pairs, then

\[
f_X(a)=E_X(e^{ia},J_{\rm unit}(e^{ia}))
\tag{CC58}
\]

is holomorphic, gauge invariant, and satisfies

\[
\sup_{\mathcal D_\rho}|f_X|
\le\sup_{\mathcal D_{\rm joint}(X^+)}|E_X|.
\tag{CC59}
\]

The gauge statement uses the physical current identity in CMP109 (1.8), (1.10), and (1.19), rather than treating \(J\) as a gauge-independent scalar. Its linearization is the lattice divergence of the linearized curvature. It vanishes on an affine constant-curvature test in a nonwrapping chart. Thus the full physical curvature-quadratic projection remains the 21-component projection used above. Wrapping tests retain the finite-torus convention and tail qualification already stated after (CC30).

This proves the local unit-current pullback needed for sources already expressed in a genuine unit-mesh chart. It does not substitute mesh one into a physical current defined on a finer lattice.

#### 12.2 The actual-minimizer pullback that would close the interface

For a source born at scale \(j\), retain its birth index and write the physical function as

\[
(\mathscr P_jE_X)(V_j)
=E^{(j)}_X\big(U_j(V_j),J_j(U_j(V_j))\big).
\tag{CC60}
\]

Here \(U_j\) is the **actual** minimizing field from the original finer lattice and \(J_j\) has the source's physical normalization at that scale. The desired statement is the following uniform, gauge-covariant localization estimate:

\[
\mathscr P_jE_X
=\sum_{Y\supset\mathrm{root}(X)}F^{(j)}_{X,Y},
\tag{CC61}
\]

where each coefficient is a gauge-invariant function of the current coarse field restricted to \(Y\), holomorphic on the same prescribed current-unit tube, and

\[
\boxed{
\sum_Y e^{\kappa d_j(Y)}
\sup_{\mathcal D_{\rho,j}(Y)}|F^{(j)}_{X,Y}|
\le C e^{p d_j(X)}
\sup_{\mathcal D^{\rm source}_j(X)}|E^{(j)}_X|.
}
\tag{CC62}
\]

The constants \(C,p,\kappa\) and the usable coarse analytic radius must be independent of \(j\), the ultraviolet cutoff, the volume, and the admitted real reference background within the stated regular class. The source domain must contain every *physical pair* in (CC60) with a fixed analytic margin. For a version of the source atlas whose radii depend on \(g_j\), a specified normalized radius and its interscale ratios must replace an unverified fixed radius; no inverse-radius loss may be hidden in the constant.

The output in (CC61) must have individually invariant localized pieces in the correct coarse gauge action, not merely joint covariance in an unpulled-back background and an independent auxiliary current. This is precisely the property required for its output to be an input of (CC50) and the generic quantum rooted estimate. A fixed stronger input exponent can pay the \(e^{p d_j(X)}\) footprint, provided the source construction regenerates that same reserve at each scale; it cannot be allowed to diminish after every step.

Proposition 9's **actual-minimizer** bounds, including the last entries of (190) and the current-related regularity in (19), are suitable inputs for the domain part of (CC62). They do not by themselves give its termwise invariant tree localization. The source's switched maps are suitable for localization, but a physical-current estimate for them cannot simply be inferred from their verified \(C^{1,\beta}\) bound. Establishing (CC61)–(CC62) with both properties on the same maps is the remaining concrete lemma.

Once this lemma and the required block-map identification hold, the analytic sources returned by the quantum step can be pulled back to the current-unit class, the strong classical estimate (CC55) applies, and the pullback returns to the same source atlas. This states an exact proposed closure mechanism without declaring the missing physical-current/invariant-localizer estimate proved.

---

## Part V. Source profiles and common normalization

### 1. Result and source scope

The hat functions in Balaban, CMP119 (1988), printed p.275, equation (3.40), determine an exact stochastic-rounding operator. Its zero-total-mass spatial profiles contract by exactly \(L^{-1}\) in the Kantorovich–Rubinstein norm. Its iterates satisfy an exact refinement identity. These are proved below, including vector-valued profiles for the fixed 21-dimensional quadratic sector.

That contraction does not, by itself, make the marginal mass of every point root evolve by the same matrix. We give a positive, local, periodically covariant counterexample whose uniform-source action density has exactly the correct bulk transformation, but whose point-root masses differ by a growing power of the ultraviolet scale interval. This identifies a specific missing source identity.

Two sufficient repairs are proved: a phase-independent column-sum identity, and a bounded source-gradient coboundary with controlled residuals and endpoints. Both use one common deterministic matrix normalization. Neither permits a normalization chosen separately for each point or geometrical history.

The source's actual statement is narrower than a general marked-kernel theorem. Equation (3.40) defines

\[
 h_z(x)=\prod_{\mu=1}^{d}h(x_\mu-z_\mu),
 \qquad h(t)=\max\{1-L^{-1}|t|,0\},
 \qquad \sum_z h_z(x)=1.
 \tag{SP1}
\]

Here \(x\) is a fine-lattice site and \(z\) a coarse-lattice site. Equation (3.41) uses these hats to assign already constructed bond/action densities to coarse roots, together with the adjacent-bond normalization terms. Equation (3.42) says that summing the assigned densities recovers the logarithm under study. The accompanying paragraph states Euclidean covariance on the whole coarse lattice. It does not state a phase-independent column-sum identity for the complete transport of an arbitrary old point insertion. The distinction between those statements is essential here.

All references in this part are to CMP119 or to the companion notes of this chapter. No claim is made that a hypothesis about the full old marked kernel follows merely from (3.40)–(3.42).

### 2. Exact classical profile transport

After rescaling the coarse lattice \(L\mathbb Z^d\) back to \(\mathbb Z^d\), put

\[
 p_L(n\mid x)
 =\prod_{\mu=1}^d
       \left(1-\left|x_\mu/L-n_\mu\right|\right)_+,
 \qquad
 (P_L\mu)(n)=\sum_xp_L(n\mid x)\mu(x).
 \tag{SP2}
\]

For real \(\xi\in\mathbb R^d\), also put

\[
 \rho_\xi(n)=\prod_{\mu=1}^d(1-|\xi_\mu-n_\mu|)_+.
 \tag{SP3}
\]

Thus \(p_L(\,\cdot\mid x)=\rho_{x/L}\). The kernel is nonnegative, has total mass one, and has barycenter \(x/L\). Its support consists of at most the \(2^d\) corners of the coarse cell containing \(x/L\). Its compatible translation identity is

\[
 P_L\tau_{Lm}=\tau_mP_L.
 \tag{SP4}
\]

It does not commute with every unit translation in the same form.

#### Theorem SP-A: exact Wasserstein contraction and refinement

Use the \(\ell^1\) metric on the rescaled lattice. Then

\[
 W_1(P_L\delta_x,P_L\delta_y)=L^{-1}|x-y|_1,
 \qquad
 P_L\rho_\xi=\rho_{\xi/L},
 \qquad
 P_L^N\delta_x=\rho_{x/L^N}=P_{L^N}\delta_x.
 \tag{SP5}
\]

In particular, for every zero-total-mass signed profile \(\nu\) of finite first moment,

\[
 \|P_L\nu\|_{\mathrm{KR}}
 \le L^{-1}\|\nu\|_{\mathrm{KR}}.
 \tag{SP6}
\]

These conclusions hold componentwise for profiles in any fixed finite-dimensional normed space \(E\), including \(E=\mathbb R^{21}\), with the vector-valued KR norm defined below.

**Proof.** In one dimension, stochastic rounding of a real number \(u\) can be written

\[
 R(u,U)=\lfloor u\rfloor+
             {\bf1}_{\{U< u-\lfloor u\rfloor\}},
 \qquad U\ \hbox{uniform on }[0,1].
 \tag{SP7}
\]

For each fixed \(U\), this is nondecreasing in \(u\), and its mean is \(u\). Consequently the common-\(U\) coupling satisfies

\[
 \mathbb E|R(u,U)-R(v,U)|=|u-v|.
\]

Use independent uniforms for the \(d\) coordinates. This gives the upper bound in the first identity of (SP5). The barycenters give the matching lower bound: a linear function with coordinate slopes equal to the signs of \(x_\mu-y_\mu\) is 1-Lipschitz for the \(\ell^1\) metric.

For refinement, in one dimension \(\rho_\xi\) is supported on the two adjacent integers bracketing \(\xi\). Dividing either integer by \(L\) and rounding yields integers among the two endpoints bracketing \(\xi/L\). The resulting distribution has mean \(\xi/L\), so it is precisely \(\rho_{\xi/L}\). If \(\xi/L\) is an integer, the distribution is the corresponding point mass. Products of these one-dimensional identities prove the second identity, and iteration proves the third.

For a finite-dimensional vector measure, define

\[
 \|\nu\|_{\mathrm{KR}}
 =\sup_{\substack{\varphi:\mathbb Z^d\to E^*\\
                   \operatorname{Lip}(\varphi)\le1}}
       \left|\sum_x\langle\varphi(x),\nu(x)\rangle\right|,
 \qquad \sum_x\nu(x)=0.
 \tag{SP8}
\]

The zero-mass condition removes arbitrary additive constants. The coupling just constructed gives
\(\operatorname{Lip}(P_L^*\varphi)\le L^{-1}\operatorname{Lip}(\varphi)\),
also for \(E^*\)-valued \(\varphi\). Duality proves (SP6). \(\square\)

#### Consequence for a moving point root

For a microscopic root \(x\), use the deterministic current center
\(\xi_k=x/L^k\) and the canonical injection

\[
 \iota_{k,\xi_k}v=\rho_{\xi_k}v.
 \tag{SP9}
\]

Then \(P_L\iota_{k,\xi_k}=\iota_{k+1,\xi_{k+1}}\) exactly. Choosing a nearest coarse lattice point instead would introduce an unnecessary order-one profile remainder.

The KR norm measures cancellation and first spatial moments. It does not contain an exponential support or polymer-tree weight. In a full marked analytic norm, those localization bounds must be supplied in addition to (SP6). The theorem is compatible with such an augmented norm only if the actual kernel preserves its tail weights.

### 3. A sufficient common-cocycle theorem

Let \(\mathsf K_k\) be the actual dimensionless coefficient-profile transport after any needed elimination of genuine irrelevant field modes. Its entries may be \(21\times21\) matrices. This phrase is a hypothesis: the source's hat redistribution of an action is not an identification of this full marked kernel.

For a root center \(\xi\), decompose a profile as

\[
 \mu=\rho_\xi m+\zeta,\qquad
 m=\ell\mu:=\sum_x\mu(x),\qquad \ell\zeta=0.
 \tag{SP10}
\]

The full profile norm is
\(\|\mu\|_\xi=\|m\|+\|\zeta\|_{\mathrm{st},\xi}\).
Here the stable norm may be KR alone for the abstract spatial theorem, or a stronger anchored norm if all the stated bounds hold in that norm.

#### Theorem SP-B: exact column balance

Assume, uniformly in root position, scale, ultraviolet cutoff, and volume:

1. The actual kernel has the column-sum identity
   \[
   \sum_z\mathsf K_k(z,x)=A_k
   \quad\hbox{for every }x,
   \qquad \|A_k-I\|\le C_A t_k,
   \qquad t_k=g_k^2.
   \tag{SP11}
   \]
   The matrices \(A_k\) depend only on the deterministic coupling trajectory.
2. On zero-mass profiles, \(\mathsf K_k\) contracts the stable norm by \(q<1\).
3. The injection defect
   \[
   C_{k,\xi}v
   =\mathsf K_k(\rho_\xi v)-\rho_{\xi/L}A_kv
   \tag{SP12}
   \]
   has zero mass and norm at most \(c_C\|v\|\). The stronger estimate
   \(c_C=O(t_k)\) is useful but not necessary.
4. The weak-coupling threshold is chosen so that
   \(q\sup_k\|A_k^{-1}\|<1\).

Then a point source evolves by

\[
 m_{k+1}=A_km_k,\qquad
 \zeta_{k+1}=D_{k,\xi_k}\zeta_k+C_{k,\xi_k}m_k,
 \tag{SP13}
\]

where \(\|D_{k,\xi_k}\|\le q\). There is a uniformly bounded graph
\(\zeta_k=S_{k,x}m_k\) for the point-seed family, with

\[
 S_{0,x}=0,\qquad
 S_{k+1,x}=(D_{k,\xi_k}S_{k,x}+C_{k,\xi_k})A_k^{-1}.
 \tag{SP14}
\]

In particular,

\[
 \sup_{k,x}\|S_{k,x}\|
 \le
 \frac{c_C\sup_k\|A_k^{-1}\|}
      {1-q\sup_k\|A_k^{-1}\|}.
 \tag{SP15}
\]

Write \(P_{j,k}=A_{k-1}\cdots A_j\). The single normalization
\(Z_K=P_{0,K}^{-1}\), applied on the right to the same microscopic vector family at every root, gives

\[
 m_k=P_{k,K}^{-1}v,\qquad
 \zeta_k=S_{k,x}P_{k,K}^{-1}v.
 \tag{SP16}
\]

There is no root-dependent marginal normalization in (SP16).

**Proof.** Summation of the actual kernel gives the first recurrence in (SP13) by (SP11). Projection off \(\rho_{\xi_{k+1}}\) gives the second. The graph recurrence and its geometric-series bound follow directly. Finally
\(P_{0,K}=P_{k,K}P_{0,k}\), which proves (SP16) without any commutativity assumption. \(\square\)

The graph can depend on the deterministic root trajectory and hence on its blocking phases. That dependence is a representation of the stable part of the same field, not a change in its normalization.

Under the admitted asymptotically free spacing

\[
 x_k=t_k^{-1},\qquad
 0<c_-\le x_k-x_{k+1}\le c_+,\qquad x_K\ge x_*,
 \tag{SP17}
\]

the common product in (SP16) has the remaining-scale polynomial bound established in (CV12)–(CV15) of [Hard cutoffs, connected insertions and marginal normalization](connected_insertions.md), Part VII.B:

\[
 \|\mu_k\|_{\xi_k}\le
 C\left(\frac{x_k}{x_K}\right)^s\|v\|
 \tag{SP18}
\]

for a fixed finite \(s\). The ultraviolet part of the matrix product cancels exactly. If engineering dimension four is restored, the corresponding field bound carries \(h_k^{-4}\).

If a separate irrelevant field block has nonzero reverse mixing into the quadratic sector, its graph correction must first be included in \(\mathsf K_k\) or in \(A_k\). Declaring that reverse mixing absent is not justified by the spatial profile theorem.

#### Summably small column defects

Suppose instead

\[
 \sum_z\mathsf K_k(z,x)=A_k+e_k(x).
 \tag{SP19}
\]

A useful defect estimate is

\[
 \sup_x\|e_k(x)\|+\operatorname{Lip}e_k\le\eta_k.
 \tag{SP20}
\]

The Lipschitz bound is essential for a KR norm: it bounds
\(\|\sum_xe_k(x)\zeta(x)\|\) by
\(\operatorname{Lip}e_k\|\zeta\|_{\mathrm{KR}}\).
A supremum bound alone does not control arbitrary signed zero-mass profiles of large total variation.

Subtract the root-anchored rank-\(21\) correction
\(\rho_{\xi/L}\sum_xe_k(x)\mu(x)\) from \(\mathsf K_k\mu\).
The resulting comparison map has exact column balance and differs from the actual map by an operator of norm \(O(\eta_k)\). Assume its stable block and injection satisfy Theorem SP-B, and that all these estimates hold in the same augmented profile norm.

Let \(p\) be a forward bulk-propagator exponent and \(s\) the exponent in (SP18). The forced-cocycle argument (MR54)–(MR59) then gives, for the actual and balanced evolutions with the same initial normalization,

\[
 \|\mu_k-\mu_k^{\mathrm{bal}}\|_{\xi_k}
 \le C\left(\frac{x_k}{x_K}\right)^s\|v\|\,
       e^{C\sum_{j<k}\eta_j}
       \sum_{j<k}\eta_j
              \left(\frac{x_j}{x_k}\right)^{p+s}.
 \tag{SP21}
\]

This is a genuinely common normalization. No column is normalized separately.

Super-logarithmically small defects satisfy the weighted summability in (SP21) for every fixed finite \(p+s\), as proved in (MR47)–(MR53). A power estimate
\(\eta_k=O(x_k^{-r})\) suffices by this bound when \(r>1+p+s\). Ordinary scalar or commuting interaction-picture bounds can improve that sufficient condition. A bare statement that an error is summable must not hide a noncommuting bulk-conjugation loss.

### 4. Why action covariance and \(O(g^2)\) phase control are insufficient

The next example already occurs in one scalar channel. It can be tensored with the identity in the other 20 channels and with ordinary hats in the other spatial directions.

Fix \(L\ge4\), and choose \(r\in\{1,\ldots,L-2\}\). Define an \(L\)-periodic real function \(b\) by

\[
 b(0)=0,\qquad b(r)=b(r+1)=1,
 \qquad
 b(s)=-\frac{2}{L-3}
 \quad(s\notin\{0,r,r+1\}).
 \tag{SP22}
\]

Thus \(\sum_{s=0}^{L-1}b(s)=0\). For small positive \(t_j\), define

\[
 \mathsf K_j(n,x)
 =p_L(n\mid x)\,[1+t_j b(x\bmod L)].
 \tag{SP23}
\]

This is a nonnegative, local coefficient kernel. It is a small perturbation of hats and has the same coarse-compatible translation covariance. It is not a probability kernel; a marginal operator coefficient need not have column mass one.

Its column mass is

\[
 \sum_n\mathsf K_j(n,x)=1+t_jb(x\bmod L).
 \tag{SP24}
\]

Nevertheless its uniform-source row sum is exactly unchanged:

\[
 \sum_x\mathsf K_j(n,x)=L.
 \tag{SP25}
\]

Indeed, for each residue \(s\), the two possible fine points with that residue contribute weights \(1-s/L\) and \(s/L\) to a fixed row; their sum is one. Thus
\(\sum_xp_L(n\mid x)b(x\bmod L)=\sum_sb(s)=0\).
After the usual density-volume conversion, the uniform action source has precisely the identity bulk map.

Now compare root \(0\) with

\[
 x_N=r\,\frac{L^N-1}{L-1}.
 \tag{SP26}
\]

Root \(0\) stays at \(0\), and its total coefficient mass stays one. By refinement, after \(j<N\) classical steps, the support of the second root is among

\[
 n_j=r\,\frac{L^{N-j}-1}{L-1},\qquad n_j+1.
 \tag{SP27}
\]

These sites have residues \(r,r+1\), on both of which \(b=1\). Consequently the perturbed evolution is exactly

\[
 \mathsf K_{N-1}\cdots\mathsf K_0\delta_{x_N}
   =\left[\prod_{j=0}^{N-1}(1+t_j)\right]\rho_{x_N/L^N}.
 \tag{SP28}
\]

Choose the admissible weak-coupling-scale behavior
\(t_j=\epsilon/(x_*+N-j)\). Then

\[
 \prod_{j=0}^{N-1}(1+t_j)
 \asymp
 \left(\frac{x_*+N}{x_*}\right)^\epsilon,
 \tag{SP29}
\]

with constants uniform in \(N\), for fixed \(x_*,\epsilon\). This follows from
\(\log(1+t)=t+O(t^2)\), harmonic-sum bounds, and the uniformly finite sum of \(t_j^2\).

The two roots remain within a fixed physical interval: with
\(a_N=\ell_0L^{-N}\), one has
\(a_Nx_N\longrightarrow \ell_0r/(L-1)\).
This is not an example obtained by sending a root to spatial infinity.

On each natural two-corner moving-root fiber, the projected zero-mass block of (SP23) still contracts by \(L^{-1}+O(t_j)\), uniformly in \(N\) and the root. The fiber diameter is at most one, so this is a finite-dimensional operator estimate. No global boundedness of multiplication by \(b\) on every unweighted KR profile is being assumed.

Thus exact classical contraction, a small stable perturbation, an \(O(g^2)\) phase-dependent mass, positivity, and the correct uniform-action row sum do not imply a common nondegenerate point normalization. The common bulk normalization selected by the uniform source is the identity in this example and leaves (SP28) unbounded. A scalar normalization that bounds the growing branch forces the mass at root \(0\) to tend to zero. It cannot make both roots have the same nonzero limiting field strength.

This is an obstruction to an inference, not a counterexample to Yang–Mills. The actual model has additional translation and source identities that (SP23) need not satisfy.

### 5. The bounded-coboundary repair

A more flexible sufficient identity uses a corrected marginal functional. Seek matrix weights \(W_k(x)\), uniformly close to the identity in supremum and Lipschitz norms, and one common matrix \(M_k\), such that

\[
 \boxed{
 \sum_z W_{k+1}(z)\mathsf K_k(z,x)
     =M_kW_k(x)+R_k(x).
 }
 \tag{SP30}
\]

Then the corrected coefficient mass

\[
 u_k=\sum_xW_k(x)\mu_k(x)
 \tag{SP31}
\]

satisfies the exact forced common recurrence

\[
 u_{k+1}=M_ku_k+\sum_xR_k(x)\mu_k(x).
 \tag{SP32}
\]

The weights \(W_k\) are coordinates for the source/gradient decomposition. They must not be used as an unannounced root-dependent multiplication of the original observable.

#### First-order cohomological equation

Suppose

\[
 \mathsf K_k=P_L\otimes I+t_kB_k+O(t_k^2),\qquad
 b_k(x)=\sum_zB_k(z,x),
 \tag{SP33}
\]

with uniform local operator bounds on the displayed kernels. Put
\(M_k=I+t_k\overline B_k\) and \(W_k=I+t_kH_k\).
The required first-order cancellation is

\[
 \boxed{
 b_k(x)-\overline B_k
   =H_k(x)-(P_L^*H_{k+1})(x).
 }
 \tag{SP34}
\]

Here the \(H_k\) must have a uniform supremum and Lipschitz bound over all roots and ultraviolet depths. A bound depending on the number of preceding scales is inadequate.

If \(t_{k+1}-t_k=O(t_k^2)\), (SP34) yields
\(\|R_k\|_{\infty}+\operatorname{Lip}R_k=O(t_k^2)\),
provided the kernel remainders and products have the same uniform local bounds. To check this explicitly, the linear difference in (SP30) is

\[
 t_k[b_k-\overline B_k-H_k+P_L^*H_{k+1}]
 +(t_{k+1}-t_k)P_L^*H_{k+1};
\]

the remaining cross terms are
\(t_kt_{k+1}\sum_zH_{k+1}(z)B_k(z,x)
-t_k^2\overline B_kH_k(x)\), plus the stated second-order kernel remainder.
Every displayed term is uniformly \(O(t_k^2)\).

An \(O(t_k^2)\) residual is ordinarily summable. In a general 21-channel matrix theorem, the weighted condition in (SP21), or a sharper interaction-picture estimate, is still necessary. If the bulk polynomial exponent is too large, construct the coboundary to a higher order or use channel symmetry to remove the conjugation loss.

#### Why the counterexample has no bounded corrector

If (SP34) held with uniformly bounded \(H_k\), follow the classical stochastic-rounding chain \(X_j\). Taking expectations and summing gives

\[
 \sum_{j=0}^{N-1}\mathbb E[b_j(X_j)-\overline B_j]
   =H_0(X_0)-\mathbb E H_N(X_N).
 \tag{SP35}
\]

For (SP22), the sum of \(b\) along root \(0\) is zero, whereas along root \(x_N\) it is \(N\). Subtracting these two identities cancels the common \(\overline B_j\) and would bound \(N\) by \(4\sup_{k,x}\|H_k(x)\|\). This is impossible uniformly in \(N\).

KR contraction controls Lipschitz seminorms modulo constants. It does not supply the required uniform supremum bound on a corrector. A formal sum of iterated \(P_L^*b\) can have bounded Lipschitz seminorm while growing like \(\log(2+|x|)\); microscopic roots representing a fixed physical point have \(|x|\) of order \(L^N\). Such a corrector would hide precisely the ultraviolet growth that needs to be removed.

#### Endpoint compatibility for one actual field normalization

There is a second, independent condition. For a bare point seed
\(\mu_0=\delta_x Z_Kv\), corrected initial mass is \(W_0(x)Z_Kv\). If
\(P_{0,K}=M_{K-1}\cdots M_0\) and the one common normalization is
\(Z_K=P_{0,K}^{-1}\), the terminal corrected mass, even with \(R=0\), is

\[
 P_{0,K}W_0(x)P_{0,K}^{-1}v.
 \tag{SP36}
\]

Therefore a sufficient endpoint condition for the same nonzero limit at every root is

\[
 \sup_x
 \left\|P_{0,K}\bigl(W_0(x)-I\bigr)P_{0,K}^{-1}\right\|
 \longrightarrow0.
 \tag{SP37}
\]

Uniform boundedness of the expression gives a weaker uniform-bound statement. It does not alone identify the same limiting field at all roots.

In one scalar channel, or when the endpoint correctors commute with the bulk product, \(W_0-I=O(t_0)\) implies (SP37). In the full matrix problem this implication is false without additional structure. For example, if
\(P_{0,K}=\operatorname{diag}(R^a,R^{-a})\) and
\(W_0-I=t_0E_{12}\), the conjugated error is \(t_0R^{2a}E_{12}\). With
\(t_0\asymp N^{-1}\) and \(R\asymp N\), it need not tend to zero. Products with this polynomial condition number are compatible with \(I+O(t_k)\) one-step matrices.

The full sufficient coboundary theorem is consequently:

* (SP30) holds in the dual of one common localized profile norm;
* the corrected stable subspace \(\ker(\sum W_k\mu)\), measured in the full mass-plus-stable norm, contracts uniformly and admits bounded canonical injections;
* residuals obey the weighted forcing bound of (SP21);
* the initial microscopic family satisfies the common endpoint condition (SP37), or an explicitly proved weaker condition appropriate to the claimed result.

Under these hypotheses, apply (SP32), the stable graph recurrence, and the forced-cocycle theorem of [Hard cutoffs, connected insertions and marginal normalization](connected_insertions.md), Part VII. This proves one common normalization with the corresponding remaining-scale bounds. The corrected stable subspace need not have zero ordinary mass, so a KR norm defined only on zero ordinary mass must not be applied to it without first passing to the full norm from (SP10).

### 6. A direct smooth-source theorem from row balance

There is a constructive route that does not require a pointwise column-sum theorem. It proves the common normalization in a test-function norm. This can support a direct distributional S0 construction, provided the remaining marked moment and reconstruction estimates are proved in that norm.

The volume factors matter. A point-field smearing has the form
\(h_k^d\sum_x\phi(h_kx)F_{k,x}\). If the point coefficient kernel is
\(\mathsf K_k(z,x)\), its induced source map is

\[
 (\mathsf S_k f)(z)
   =L^{-d}\sum_x\mathsf K_k(z,x)f(x).
 \tag{SP39}
\]

Use column vectors for source coefficients; all matrices below act on their left.

If one starts instead with a column of field components and writes
\(\mathcal T F_k(x)=\sum_z A_k(x,z)F_{k+1}(z)\), the kernel in (SP39) is
\(\mathsf K_k(z,x)=A_k(x,z)^{\mathsf T}\), with the transpose determined by the source-field pairing. It is the coefficient kernel, rather than the untransposed field kernel, that appears in the following ordered products.

Set \(h_{k+1}=Lh_k\). Assume the actual rooted kernel has the uniform-source row identity

\[
 L^{-d}\sum_x\mathsf K_k(z,x)=M_k,\qquad
 \|M_k-I\|\le C_Mt_k,
 \tag{SP40}
\]

where the matrix \(M_k\) is common to every output root and geometrical carrier covered by the theorem. Define

\[
 \mathsf E_k(z,x)=\mathsf K_k(z,x)-p_L(z\mid x)M_k.
 \tag{SP41}
\]

The hat row sums are \(L^d\), so \(\sum_x\mathsf E_k(z,x)=0\).

For a deterministic coefficient kernel satisfying the literal coarse-translation identity
\(\mathsf K_k(z+m,x+Lm)=\mathsf K_k(z,x)\), absolute row summability already implies that the row matrix is independent of \(z\): change variables in the sum and define
\(M_k=L^{-d}\sum_x\mathsf K_k(0,x)\).
This applies, for example, to a translation-covariant marginal jet extracted at a translation-invariant reference background, once its actual kernel is constructed. Covariance that also translates a nonconstant background or a geometrical history does not by itself give a constant row sum with that background held fixed.

The concrete locality hypothesis is the first physical moment

\[
 L^{-d}\sum_x\|\mathsf E_k(z,x)\|
           |h_kx-h_{k+1}z|_1
       \le C_Et_kh_k
 \quad\hbox{uniformly in }z.
 \tag{SP42}
\]

Constants may depend on fixed \(L,d\) and the fixed finite marginal dimension, but not on the ultraviolet depth or volume.

Let

\[
 (\mathsf Q_kf)(z)=L^{-d}\sum_xp_L(z\mid x)f(x),\qquad
 \mathsf U_k=M_k\mathsf Q_k,\qquad
 \mathsf R_k=\mathsf S_k-\mathsf U_k.
 \tag{SP43}
\]

The row-normalized hats are a probability average. On a full or periodic lattice they contract both the supremum norm and the physical Lipschitz seminorm. To see the latter, write the row as a common distribution of fine-grid offsets from the coarse root and use the same offset for two coarse roots.

Row cancellation gives the exact identity

\[
 (\mathsf R_kf)(z)
 =L^{-d}\sum_x\mathsf E_k(z,x)
       [f(x)-f(Lz)].
 \tag{SP44}
\]

Consequently

\[
 \|\mathsf R_kf\|_\infty
 \le C_Et_kh_k\operatorname{Lip}_{h_k}(f).
 \tag{SP45}
\]

There is also a useful operator bound that follows from the same moment, with no separate total-variation hypothesis. Every off-center fine site is at least \(h_k\) away from \(h_{k+1}z\). Its total absolute kernel mass is therefore at most \(C_Et_k\). The center coefficient is the negative sum of the off-center coefficients. Hence

\[
 L^{-d}\sum_x\|\mathsf E_k(z,x)\|\le2C_Et_k,\qquad
 \|\mathsf S_k\|_{\infty\to\infty}
 \le1+(C_M+2C_E)t_k.
 \tag{SP46}
\]

This argument allows arbitrary root dependence of the error rows. Translation covariance of the error is unnecessary for the theorem.

#### Theorem SP-C: a common normalization for smooth source coefficients

Assume (SP17), (SP40), and (SP42), and choose the one weak-coupling threshold so that every \(M_k\) is invertible with
\(\|M_k^{-1}\|\le\exp(2C_Mt_k)\).
Put

\[
 P_{j,k}=M_{k-1}\cdots M_j,\qquad
 Z_K=P_{0,K}^{-1},
 \qquad
 \phi_0(x)=\phi(h_0x),
 \tag{SP47}
\]

for a bounded Lipschitz \(E\)-valued test function \(\phi\). Evolve the actual source from \(Z_K\phi_0\). Then for every \(k\le K\),

\[
 \boxed{
 \left\|
 \mathsf S_{k-1}\cdots\mathsf S_0(Z_K\phi_0)
 -P_{k,K}^{-1}\mathsf Q_{k-1}\cdots\mathsf Q_0\phi_0
 \right\|_\infty
 \le
 C\left(\frac{x_k}{x_K}\right)^s
       \frac{h_k}{x_k}\operatorname{Lip}(\phi).
 }
 \tag{SP48}
\]

Here \(s=2C_M/c_-\), and \(C\) is independent of the ultraviolet cutoff and volume. In particular, the actual source coefficient is bounded by

\[
 C\left(\frac{x_k}{x_K}\right)^s
 \left[\|\phi\|_\infty+
               h_kg_k^2\operatorname{Lip}(\phi)\right].
 \tag{SP49}
\]

One common matrix \(Z_K\) suffices even when the matrices at different scales do not commute.

**Proof.** Write \(\mathsf S_{j,k}=\mathsf S_{k-1}\cdots\mathsf S_j\), and similarly for \(\mathsf U\). The exact telescoping identity is

\[
 \mathsf S_{0,k}-\mathsf U_{0,k}
 =\sum_{j=0}^{k-1}
       \mathsf S_{j+1,k}\mathsf R_j\mathsf U_{0,j}.
 \tag{SP50}
\]

The future propagator is the actual one; the past propagator is the balanced bulk one. This ordering avoids assuming a Lipschitz bound on the actual evolved source.

Equation (SP46) and (SP17) give

\[
 \|\mathsf S_{j+1,k}\|_{\infty\to\infty}
 \le \left(\frac{x_j}{x_k}\right)^p,
 \qquad p=(C_M+2C_E)/c_-.
 \tag{SP51}
\]

The scalar spatial hats commute with every common matrix. The matrices need not commute with one another. The exact product identity is

\[
 \mathsf U_{0,j}(Z_K\phi_0)
   =P_{0,j}P_{0,K}^{-1}\mathsf Q_{0,j}\phi_0
   =P_{j,K}^{-1}\mathsf Q_{0,j}\phi_0.
 \tag{SP52}
\]

Its physical Lipschitz seminorm is at most
\((x_j/x_K)^s\operatorname{Lip}(\phi)\).
Substituting (SP45), (SP51), and (SP52) into (SP50) bounds its norm by

\[
 C_E\left(\frac{x_k}{x_K}\right)^s
 \operatorname{Lip}(\phi)
 \sum_{j<k}t_jh_j
       \left(\frac{x_j}{x_k}\right)^{p+s}.
 \tag{SP53}
\]

For \(n=k-j\), \(h_j=h_kL^{-n}\) and
\(1\le x_j/x_k\le1+c_+n/x_k\).
Therefore, for every fixed finite \(w\ge0\),

\[
 \boxed{
 \sum_{j<k}t_jh_j
       \left(\frac{x_j}{x_k}\right)^w
 \le
 \frac{h_k}{x_k}
 \sum_{n\ge1}L^{-n}
       \left(1+\frac{c_+n}{x_*}\right)^w
 \le C_{L,w,x_*}\frac{h_k}{x_k}.
 }
 \tag{SP54}
\]

This geometric factor beats every fixed polynomial bulk loss. Equations (SP48)–(SP49) follow. \(\square\)

At \(k=K\), the error is \(O(h_Kg_K^2\operatorname{Lip}\phi)\). At a fixed physical matching scale it is a controlled local source-gradient term, not an assertion that the term vanishes there. The bound becomes small upon moving the matching scale toward the ultraviolet along the admitted trajectory.

The scale sum also has an all-order-compatible quantifier. If a separately proved degree-\(m\) marked theorem has bulk exponent \(w_m\le rm\), with fixed integer \(r\ge1\), then the constant in (SP54) can be chosen to obey

\[
 C_{L,w_m,x_*}\le C^{m+1}(m!)^r.
 \tag{SP54a}
\]

Indeed, for \(\lambda=\log L\), fixed \(c=c_+/x_*\), and an integer \(q\),
\[
 \sum_{n\ge1}e^{-\lambda n}(1+cn)^q
 \le C^{q+1}q!.
\]
For \(c>0\), use \(y^q\le q!\theta^{-q}e^{\theta y}\) with
\(\theta=\lambda/(2c)\); the remaining geometric series converges. The case \(c=0\) is immediate. Take \(q=rm\) and use
\((rm)!\le r^{rm}(m!)^r\), which follows by bounding one multinomial coefficient by the sum of all such coefficients. This adds a fixed factorial power and no order-dependent coupling threshold. It does not supply the separate degree-\(m\) marked kernel estimate.

#### A larger, nonsummable small first moment is enough at fixed degree

The defect moment need not itself be \(O(g_k^2)\). Keep the common row matrix in (SP40), but replace (SP42) by

\[
 L^{-d}\sum_x\|\mathsf E_k(z,x)\|
       |h_kx-h_{k+1}z|_1
 \le C_E\epsilon_k h_k,
 \qquad
 0\le\epsilon_j\le\epsilon_k\le\epsilon_*
 \quad(j\le k).
 \tag{SP54b}
\]

For example, \(\epsilon_k=g_kr_{\chi,k}\) is suitable whenever it is increasing along the admitted weak-coupling trajectory. Without monotonicity, use \(\sup_{j\le k}\epsilon_j\) in the resulting estimate.

Choose one threshold with \(2C_E\epsilon_*\le\frac12\log L\). Row cancellation still gives total variation at most \(2C_E\epsilon_k\). The actual future propagator therefore satisfies

\[
 \|\mathsf S_{j+1,k}\|
 \le
 \left(\frac{x_j}{x_k}\right)^{C_M/c_-}
 \exp\{2C_E\epsilon_*(k-j)\}.
 \tag{SP54c}
\]

Apply the same ordered identity (SP50); its bulk past remains exactly (SP52). For \(n=k-j\), the geometric factor is now at most \(L^{-n/2}\), and the error is bounded by

\[
 \boxed{
 C\left(\frac{x_k}{x_K}\right)^s
       h_k\epsilon_k\operatorname{Lip}(\phi).
 }
 \tag{SP54d}
\]

The proof is the convergent series
\(\sum_{n\ge1}L^{-n/2}(1+c_+n/x_*)^{C_M/c_-+s}\).
Thus the phase-dependent local first moment may be as large as
\(g_kr_{\chi,k}\). Sharpening it to \(g_k^2\) is unnecessary for this one-root smooth-source theorem. The common row matrix is still required to have its stated deterministic bulk bound; no row defect is normalized separately.

The weighted version below holds for each fixed Schwartz order after replacing \(C_E\) by the corresponding fixed weighted-moment constant. This is a fixed-degree assertion. In a joint degree-\(m\) kernel, a crude future bound \(\exp(Cm\epsilon_*(k-j))\) would require an \(m\)-dependent threshold to be absorbed by the single factor \(L^{-(k-j)}\). One cannot use this argument to claim an all-order result from only the one-root estimate. A per-root product test norm, with a gradient factor propagated in its own stable source coordinate and other roots normalized by their common bulk coordinates, is a possible remedy. Its connected multiple-root bounds must be proved; they are not supplied by (SP54d).

#### Even the common matrix can use a small fixed engineering reserve

For the fixed-degree distributional normalization, an \(O(g_k^2)\) bound on the common matrix is also stronger than necessary if a small fixed increase in the physical bound is allowed. Suppose instead

\[
 \|M_k-I\|\le C_M\epsilon_k,\qquad
 0\le\epsilon_k\le\epsilon_*,
 \tag{SP54e}
\]

with the first-moment bound (SP54b), and with the classical marginal coordinates chosen so that the reference matrix is \(I\). For \(C_M\epsilon_*\le1/2\), set

\[
 s_\epsilon=\frac{2C_M\epsilon_*}{\log L},
 \qquad
 p_\epsilon=\frac{(C_M+2C_E)\epsilon_*}{\log L}.
 \tag{SP54f}
\]

Then
\(\|P_{k,K}^{-1}\|\le(h_K/h_k)^{s_\epsilon}\), and
\(\|\mathsf S_{j+1,k}\|\le(h_k/h_j)^{p_\epsilon}\).
These are simple bounds on the ordered products; no commutativity is used.
Choose one threshold satisfying \(p_\epsilon+s_\epsilon<1\). The same telescoping identity now gives

\[
 \boxed{
 \left\|\mathsf S_{0,k}(Z_K\phi_0)
   -P_{k,K}^{-1}\mathsf Q_{0,k}\phi_0\right\|_\infty
 \le
 C\left(\frac{h_K}{h_k}\right)^{s_\epsilon}
     h_k\epsilon_k\operatorname{Lip}(\phi).
 }
 \tag{SP54g}
\]

The scale sum is
\(\sum_{n\ge1}L^{-n(1-p_\epsilon-s_\epsilon)}\).
For weighted source norms, replace \(C_E\) by the required fixed weighted-moment constant and make the same once-only choice of threshold.

Restoring a dimension-four field gives a bound of physical order
\(h_k^{-(4+s_\epsilon)}\). At the incoming scale, the one common normalization has
\(\|Z_K\|\le(h_K/a)^{s_\epsilon}\), so an \(Aa^{-4}\) bounded seed becomes an
\(Ah_K^{s_\epsilon}a^{-(4+s_\epsilon)}\) bounded seed. In terminal-scale units this is an \(A'a^{-(4+s_\epsilon)}\) bound. A common subtraction needs its corresponding bound as usual. Thus the protected-core theorem can use the fixed dimension
\(\Delta=4+s_\epsilon\). One may choose the threshold so that
\(s_\epsilon\le1/2\), without depending on the moment order.

This corollary can avoid a sharp loop calculation merely to obtain an admissible common normalization and a finite physical singular order. It does not prove the actual kernel or its reference-matrix matching, return to the analytic marked class, an all-order source theorem, or nontriviality of the limiting Schwinger functional.

#### Schwartz weights and the remaining locality requirement

The unweighted first-moment condition alone gives the supremum theorem above. It does not ensure an integrable tail of the output for a compactly supported test function: many distant rows could each send a small amount of mass into the same compact input set. A distributional construction must keep a spatial tail norm.

A sufficient strengthening, for each needed fixed integer \(N\), is

\[
 L^{-d}\sum_x\|\mathsf E_k(z,x)\|
    |h_kx-h_{k+1}z|_1
    (1+|h_kx-h_{k+1}z|_1)^N
 \le C_Nt_kh_k.
 \tag{SP55}
\]

An exponential local kernel bound with an appropriate first-moment factor implies this. Use the norm
\(\|f\|_{\infty,N,h}=\sup_x(1+|hx|_1)^N\|f(x)\|\).
The same cancellation and the inequality
\(1+|y|\le(1+|y-u|)(1+|u|)\) give weighted versions of (SP45) and (SP46). The hat averaging has weighted norm at most
\(\exp(C_Nh_k)\). Its composition has a uniform factor because
\(\sum_{j<k}h_j\le h_k/(L-1)\le\ell_0/(L-1)\).
The bulk past can be represented by convolution with a bounded-support probability distribution, so its weighted physical gradient seminorm is bounded by the corresponding Schwartz seminorm of \(\phi\), with constants depending on \(\ell_0,N\), not on the ultraviolet depth.

Repeating the ordered telescoping proof yields (SP48) in weighted supremum norm, with its right side replaced by

\[
 C_N\left(\frac{x_k}{x_K}\right)^s
 \frac{h_k}{x_k}
 \sup_{y\in\mathbb R^d}
       (1+|y|_1)^N\|\nabla\phi(y)\|.
 \tag{SP56}
\]

The forward exponent \(p\) may become \(p_N\); (SP54) still holds for every fixed \(p_N+s\). For \(N>d\), this weighted bound also controls the physical discrete \(L^1\) norm, since
\(h_k^d\sum_z(1+|h_kz|)^{-N}\) is uniformly finite for \(h_k\le\ell_0\).

There is an additional quantifier to check in an all-order Schwartz statement. Taking \(N\) proportional to \(m\) in (SP55) does not automatically make \(p_N\) linear in \(m\): the constants \(C_N\) could grow exponentially or factorially. A useful formulation instead uses the product weight
\(\prod_{i=1}^m(1+|x_i|)^{N_0}\), with one fixed \(N_0>d\) per insertion. If the actual multiple-root kernel has tensorized local weighted bounds whose logarithmic per-step cost is at most \(C m t_k\), the bulk exponents are linear in \(m\), and (SP54a) applies. This product weight is bounded by
\((1+|(x_1,\ldots,x_m)|_1)^{N_0m}\), which is an allowed Schwartz order linear in \(m\). Establishing those multiple-root bounds, including connected corrections, is a separate theorem; it is not inferred from the one-root estimate.

The periodic counterexample (SP23) satisfies (SP40) and (SP42), with constants depending only on \(L\) and \(b\). Thus it simultaneously has uncontrolled individual point masses and controlled smooth-source coefficients. This proves that the distributional route is a substantive alternative, not a restatement of the pointwise column theorem.

For Yang–Mills, (SP42)/(SP55) must be verified for the actual normalized rooted marked kernel and its full finite mixing, with the old numerator retained. The source-free action's row identity alone supplies no absolute first-moment bound. Irrelevant field tails, multi-source connected estimates, large-field exits, boundary terms, and OS reconstruction remain separate tasks. The theorem establishes the common-normalization part of a direct smooth-source route under explicit kernel estimates; it does not by itself prove all S0 axioms.

### 7. A constructive source-gradient route to the missing identity

The counterexample makes the required computation more specific. It is unnecessary to prove an abstract theorem saying every small phase error disappears: that assertion is false. The task is to prove that the actual phase error lies in a controlled source-gradient or coboundary sector.

Introduce the full slowly varying 21-component source before performing the fixed, positive RG operation. Keep the discrete source-gradient coefficients together with the genuine irrelevant field modes. A neighboring point-source difference is a discrete derivative of the same local observable; its expected engineering dimension is one higher. The crucial marked Ward/localization estimate is that this derivative sector remains local and contracts after the actual transport, including normalized kernel-score and cutoff contributions.

A precise sufficient structural version is the following. Let \(\mathcal D_k\) embed the localized source-gradient sector in the marked operator space, and let \(\mathcal T_k\) be the actual normalized old-mark operation. Prove

\[
 \mathcal T_k\mathcal D_k
   =\mathcal D_{k+1}\mathcal Q_k+\mathcal R_k,
 \qquad
 \|\mathcal Q_k\|\le q<1,
 \tag{SP38}
\]

with \(\mathcal R_k\) obeying the weighted summable bound. Also prove that the classes of the microscopic root family in the quotient by this stable sector have the same \(E\)-coordinate, uniformly in the blocking phase. The induced quotient map is then a common matrix. A finite local source stencil or a local conjugacy supplies its embedding into the full marked space. Changing the embedding produces the coboundary in (SP34).

For an exact invariant gradient sector, the quotient argument is elementary: point-source differences lie in the stable sector; their images do also by (SP38) with \(\mathcal R=0\); therefore every point root has the same marginal class. For a summably imperfect sector, the discarded quotient defect is a forcing of the type (SP21). This is a common field normalization, because the quotient coordinate is fixed once for the entire source family.

The useful concrete targets are therefore:

1. Compute or bound the actual one-step rooted quadratic kernel, including reverse mixing from its already eliminated stable field part.
2. Establish its phase-independent column sum (SP11), or identify the phase-dependent coefficient \(b_k(x)\) and prove (SP34) with a uniformly local bounded corrector.
3. Establish the endpoint matching for the original microscopic point family. If only matrix norm bounds are available, retain the conjugation condition (SP37); if symmetry gives commuting channels, prove that reduction.
4. Bound residuals in the full localized profile norm, with enough order to satisfy (SP21). A scalar \(O(g^4)\) cancellation need not be advertised as a fully general 21-channel result without this check.

Full microscopic translation covariance is a plausible source of these identities once source gradients and irrelevant tails are retained. Source-free covariance of the summed effective action alone is insufficient, as (SP25) shows. The missing step is a quantitative local Ward/intertwining estimate, not an arbitrary choice of a different normalization at each blocking phase.

Randomizing a global blocking origin is not used here. A common random origin can create a common global fluctuation, and reverse conditional origin weights need not be uniform. Averaging an unnormalized mass therefore does not establish the desired absolute two-root estimate. A finite shrinking local source stencil or the explicit gradient intertwining above is the more directly checkable route.

### 8. What is established and what remains

**Established in this note:** the exact stochastic-rounding realization, sharp Wasserstein/KR contraction, refinement identity, canonical moving-root injection, the common-cocycle theorem under column balance, the weighted perturbation reduction, the local positive counterexample separating row balance from column balance, the bounded-coboundary criterion with its first-order calculation, the endpoint obstruction for noncommuting finite mixing, and the smooth-source row-balance theorem with an explicit \(h_kg_k^2\) error and one common matrix normalization. The fixed-degree version also allows a first-moment error \(h_k\epsilon_k\), including \(\epsilon_k=g_kr_{\chi,k}\), at one weak-coupling threshold.

**Still a source-specific theorem:** verify the actual normalized rooted kernel and either its column balance, its uniformly bounded source-gradient coboundary, or its row balance with the localized first-moment bound needed for the direct distributional route; prove compatible analytic localization and, where the coboundary route is used, endpoint matching. The source estimate (3.40)–(3.42) supplies the classical hats and summed-action localization, but does not by itself discharge those marked estimates.

This leaves a concrete calculation and norm estimate. It does not leave permission to normalize histories or point roots separately.

---

## Part VI. Current-carrying localization and joint classical gain

### 1. Purpose and conclusion

The obstruction isolated in CC62 is that a switched minimizing connection has useful complex first-derivative and Hölder bounds, while the physical current contains a second spatial derivative. Taking that derivative after switching need not preserve its source bound.

This note constructs a different off-section object: a pair

\[
(U_s,J_s),
\]

where \(U_s\) is a switched connection and \(J_s\) is obtained from a localized **coarse Lagrange multiplier**. The auxiliary current is not required to equal the physical current of \(U_s\) when the switches are different from one. The source atlas explicitly permits \(J\) as an independent variable. At the unswitched point the pair agrees with the actual minimizing field and its physical current.

The algebraic identities and norm estimates below give an \(N\)-uniform pair construction on a full-torus small complex increment domain about the trivial reference field, using the source's localized operator bounds and its analytic fixed-point estimates. It does not use a second spatial derivative of a switched field. The resulting rooted expansion is covariant in the **joint reference-background/increment atlas**. Its conversion to a decomposition invariant under the inhomogeneous coarse gauge action at a fixed reference section remains a separate step; this note does not declare the entire CC62 interface closed.

### 2. Normalization and the linear constrained inverse

Use current coarse units. The coarse spacing is one, the fine spacing is

\[
\eta=L^{-N}.
\tag{CP1}
\]

Fine-field pairings include \(\eta^d\); coarse pairings use the unit-lattice counting measure. All transposes below are transposes for these bilinear pairings, continued analytically to complex fields. They are not conjugate transposes of complex-valued switch parameters.

At the flat reference, let \(\Delta\) be the quadratic Wilson operator, \(Q\) the linear averaging operator in current units, and \(D R D^*\) the source Landau gauge-fixing operator. Define

\[
\begin{aligned}
\mathcal L&=\Delta+DRD^*,\\
G&=(\mathcal L+aQ^*Q)^{-1},\\
S&=QGQ^*,\qquad W=S^{-1},\\
H_0&=GQ^*W,\\
C&=G-GQ^*WQG,\\
\Delta_c&=W-aI.
\end{aligned}
\tag{CP2}
\]

The source chooses \(a=1\) in current units; keeping \(a\) visible makes the Schur-complement identities transparent. The notation \(C\) here denotes the constrained Green operator, not the independent-coordinate embedding used in the fluctuation integral.

For prescribed \(f,b\), consider

\[
\mathcal L A-Q^*\Lambda=f,
\qquad QA=b.
\tag{CP3}
\]

Direct substitution gives

\[
\boxed{
A=Cf+H_0b,
\qquad
\Lambda=-H_0^*f+\Delta_cb.
}
\tag{CP4}
\]

For example, \(QH_0=I\), \(QC=0\), and

\[
\mathcal L H_0=Q^*\Delta_c,
\qquad
\mathcal L C=I-Q^*H_0^*.
\tag{CP5}
\]

These verify both equations in (CP3). With the conventional symmetric KKT matrix \(\bigl(\begin{smallmatrix}\mathcal L&Q^*\\Q&0\end{smallmatrix}\bigr)\), its multiplier is \(-\Lambda\); its inverse has lower-right block \(aI-W\). This records the sign explicitly.

The constrained inverse is well-defined although the unconditioned Wilson Hessian has gauge directions. The coarse constraints and the source gauge-fixing term are included before inversion. No claim of invertibility of the bare Wilson Hessian is used.

### 3. Source support and uniform linear norms

The relevant source identifications are:

- CMP102 (129) and (131), pp.297–298, give \(H_0\) and the constrained projection, hence \(C=GP_0^*\).
- CMP99 (3.126), (3.129), and (3.132), pp.420–422, give the corresponding minimizing operators and the exponential bound for \(W=(QGQ^*)^{-1}\). The discussion on p.422 extends the operator analysis to this inverse. Theorem 3.14 and its discussion on p.427 explicitly include this operator type in the domain-localized random-walk framework.
- CMP102 Proposition 4, (97)–(98), p.293, bounds the nonlinear force in the norm of a dimension-three field using only the field and its first spatial derivative.
- CMP102 (44)–(49) and (72), pp.285–289, give the nonlinear averaging remainder and its normalized local derivative.

In the full-torus specialization \(j=j'=N\), \(L^j\eta=L^{j'}\eta=1\). Thus all source scale factors for these current-unit norms are fixed. Write

\[
\|A\|_1=\max\{\|A\|_\infty,\|\nabla_\eta A\|_\infty\},
\qquad \|F\|_3=\|F\|_\infty
\tag{CP6}
\]

in these units, adding the fixed local Hölder seminorm when needed for the connection atlas. The subscript 3 records physical scaling, not a third derivative in this definition.

The source bounds imply

\[
\begin{aligned}
\|H_0 b\|_1&\le K\|b\|_\infty,&
\|Cf\|_1&\le K\|f\|_3,\\
\|H_0^*f\|_\infty&\le K\|f\|_3,&
\|\Delta_cb\|_\infty&\le K\|b\|_\infty.
\end{aligned}
\tag{CP7}
\]

The transpose estimate deserves attention. A representative kernel has exponential decay in current physical distance. In \(H_0^*f\), the fine-site sum carries \(\eta^d\). The number of fine sites in one current block is \(O(\eta^{-d})\), and these factors cancel. Thus the transpose bound has no hidden \(L^{dN}\) factor. The same normalization is used in (CP2) and in the averaging-derivative adjoint below.

The source random-walk localizations may be assigned one common system of switches. This includes \(W\): CMP99 p.426 explicitly lists \((QGQ^*)^{-1}\) among the operators of Theorem 3.14, and its proof on p.427 expressly uses their random-walk expansions and cancellation of terms whose localization domains remain inside the common region. Thus this is an operator-localization input from the source, rather than an inference from a bare entrywise inverse bound. Assign each walk the product of the switches on its localization domains, using the same switches for every block of the constrained inverse.

With protected root blocks and \(|s_\Delta|\le e^{\kappa_1}\), the corresponding operators have bounds of the form (CP7) with a larger fixed constant \(K_s\). Choose the localization-block size after \(\kappa_1\), as in CMP116 (1.7), (1.11). Terms in \(W\), products in \(C\), and the local diagonal term in \(\Delta_c\) are localized before the nonlinear fixed point is solved. Finite products have the union of the factors' localization domains; their bounds follow by summing the normalized exponentially decaying intermediate kernels. Enlarging these domains by a fixed collar supplies the separation needed by the local nonlinear vertices.

At switches different from one these blocks need not obey every inverse identity (CP5). That is not assumed. They have the same localization, analyticity, and bounded mapping properties, and recover the exact inverse blocks at \(s=1\).

### 4. The actual nonlinear constrained equation

Let \(A'\) denote the source variable in which the constraint is linear. Its physical connection variable is

\[
A=K(A')=A'-H D(A'),
\qquad
D(A')=\mathcal C(A),
\tag{CP8}
\]

where \(\mathcal C\) is the nonlinear part of the averaging map. In current units,

\[
\mathcal Q(A)=QA+\mathcal C(A),
\qquad QH=I,
\qquad \mathcal Q(K(A'))=QA'.
\tag{CP9}
\]

These are source (44)–(49), not a truncation of the nonlinear constraint.

At the flat reference the transformed action has the form

\[
\widetilde S(A')=S(K(A'))
=S(0)+\tfrac12\langle A',\Delta A'\rangle+V(A'),
\tag{CP10}
\]

where \(V\) includes the full constraint correction. The small background-current quadratic correction vanishes at this reference. Proposition 4 provides

\[
\|V'(A')\|_3\le C_V\|A'\|_1^2,
\qquad
\|V'(A'_1)-V'(A'_2)\|_3
\le C_V r\|A'_1-A'_2\|_1
\tag{CP11}
\]

on a sufficiently small complex ball \(\|A'\|_1\le r\). The Lipschitz estimate follows by Cauchy on the same analytic ball, as in the source's fixed-point proof. It involves no second spatial derivative of \(A'\).

For the actual minimizing configuration, CMP102 (127) gives stationarity against every variation with \(Q\delta A'=0\), after the source removes the artificial restriction on the gauge variation. Consequently

\[
\Delta A'+V'(A')=Q^*\Lambda,
\qquad QA'=B.
\tag{CP12}
\]

The actual solution is also in Landau gauge, so \(DRD^*A'=0\). Applying (CP4) gives the exact formulas

\[
\boxed{
\begin{aligned}
A'&=H_0B-CV'(A'),\\
\Lambda&=\Delta_cB+H_0^*V'(A').
\end{aligned}}
\tag{CP13}
\]

This is the multiplier counterpart of the alternative equation (143) and its specialization (180). The source warns on p.300 that the alternative fixed-point equation alone should not be treated as a proof of Landau gauge. The identification here instead uses the already constructed physical minimizing solution, its stationarity (127), and the small-solution uniqueness from the source's fixed-point estimates. Thus no missing gauge equation is being discarded.

Write \(U_N^{\rm L}\) for this Landau representative of the actual minimizing orbit. After CMP102 (179)–(180), the source also changes to an axial representative and reuses its minimizing-field notation. Literal equalities below refer to \(U_N^{\rm L}\); the final source representative is related by the same fine gauge change applied to both connection and current. A gauge-invariant joint insertion has identical values in either representative.

### 5. A switched multiplier without a switched second derivative

Use the same switched local force \(V'_s\), averaging correction, and operator bounds as in the source construction, enlarged by the coarse inverse/multiplier blocks in Section 3. Here \(V'_s\) means the source's **rearranged analytic force formula**, estimated in CMP102 (85)–(98), with its operator entries localized as prescribed in CMP116 after (1.14). The latter explicitly retains Proposition 4 for these modified operators. It does not mean freshly differentiating \(S\circ K_s\) and subtracting an unswitched quadratic form: the inverse identities used in that cancellation need not hold off section. The source rearrangement is what retains the \(C^1\)-to-force bound (CP11). At \(s=1\) it equals the actual transformed-action derivative. Define

\[
\begin{aligned}
A'_s&=H_{0,s}B-C_s V'_s(A'_s),\\
\Lambda_s&=\Delta_{c,s}B+H_{0,s}^*V'_s(A'_s),\\
A_s&=A'_s-H_s D_s(A'_s),\qquad
U_s=\exp(i\eta A_s).
\end{aligned}
\tag{CP14}
\]

The first equation is contractive on \(\|A'_s\|_1\le 2K_s\|B\|\) if \(\rho\) is fixed small enough and \(\|B\|<2\rho\). CMP116 (1.3)–(1.18) proves precisely the needed holomorphic fixed-point stability when localized propagators replace the original ones. The additional inverse blocks only enlarge the fixed constants. Uniformly on the complex switch polydisc,

\[
\|A'_s\|_1+\|A_s\|_1\le C_s\|B\|,
\qquad
\|\Lambda_s\|\le C_s\|B\|+C_s\|B\|^2.
\tag{CP15}
\]

The constants are independent of \(N\) and volume. Their dependence on the fixed switch radius, block geometry, Hölder exponent, and analytic margins is retained.

The multiplier is computed from bounded coarse operators and a bounded nonlinear force. In particular, (CP14) does **not** evaluate \(\Delta A'_s\) to find \(\Lambda_s\).

### 6. Recovering the current algebraically

Define the pointwise differential-of-exponential map by

\[
\delta e^{i\eta A}e^{-i\eta A}
=i\eta\mathcal E_A(\delta A),
\qquad
\mathcal E_A=
\int_0^1 e^{it\eta\operatorname{ad}A}\,dt.
\tag{CP16}
\]

For \(\eta\|A\|\) small, \(\mathcal E_A\) and its inverse are bounded holomorphic pointwise maps. Source (26)–(28) identify the left-trivialized variation of the Wilson action with the physical current \(J(U)\). Therefore

\[
\nabla_A S(e^{i\eta A})=\mathcal E_A^*J(U),
\qquad
\nabla_{A'}\widetilde S
=K'(A')^*\mathcal E_A^*J(U).
\tag{CP17}
\]

Equation (CP8) is equivalent to \(A'=A+H\mathcal C(A)\). Differentiating gives

\[
(K'(A')^*)^{-1}
=I+\mathcal C'(A)^*H^*.
\tag{CP18}
\]

At the actual solution, use \(\nabla_{A'}\widetilde S=Q^*\Lambda\) from (CP12) and \(H^*Q^*=I\). This proves the exact nonlinear identity

\[
\boxed{
J(U_N^{\rm L}(e^{iB}))
=(\mathcal E_A^*)^{-1}
\big(Q+\mathcal C'(A)\big)^*\Lambda.
}
\tag{CP19}
\]

All nonlinear constraint terms are retained. This is also the chart form of the intrinsic stationarity statement that the physical current lies in the adjoint range of the differential of the nonlinear averaging constraint.

For arbitrary switches, **define** the independent atlas current by

\[
\boxed{
J_s=(\mathcal E_{A_s}^*)^{-1}
\big(Q+\mathcal C'(A_s)\big)^*\Lambda_s.
}
\tag{CP20}
\]

The evaluator \(\mathcal C'\) here is the actual local nonlinear averaging derivative at the connection \(A_s\); it is not a second spatial derivative of that connection. It need not be replaced by the derivative of a switched physical current. The definition is permitted because the source treats \(J\) as an independent analytic variable off the physical section.

At \(s=1\), equations (CP13) and (CP19) show

\[
(U_1,J_1)=\big(U_N^{\rm L}(e^{iB}),J(U_N^{\rm L}(e^{iB}))\big).
\tag{CP21}
\]

### 7. Uniform current bound and the source atlas

The local averaging derivative bound (72) controls \(\mathcal C'(A)\) as a normalized kernel. In the full current-unit specialization its scale factor is one. Transposing with the source pairings yields

\[
\|Q^*\Lambda\|_3\le C\|\Lambda\|,
\qquad
\|\mathcal C'(A)^*\Lambda\|_3
\le C\|A\|_1\|\Lambda\|.
\tag{CP22}
\]

The derivative is supported in a fixed number of current averaging blocks. More explicitly, the normalized kernel in CMP102 (72) is bounded by \(C\|A\|_1\ell^{1-d}\), where \(\ell=L^j\eta\). For \(j=N\), \(\ell=1\). At a fixed fine bond the adjoint sums over only a bounded number of coarse averaging bonds. Therefore the pointwise estimate in (CP22) follows without summing over the \(\eta^{-d}\) fine bonds in a block. The estimate for \(H_0^*\) in (CP7), in contrast, does involve a fine sum; there the factor \(\eta^d\) is essential. These two adjoint estimates use different sums and neither introduces a volume or ultraviolet factor.

Combining (CP15), (CP16), and (CP22) proves

\[
\boxed{
\|J_s\|_3\le C_s\|B\|,
\qquad
\|A_s\|_1+[\nabla A_s]_\beta\le C_{s,\beta}\|B\|.
}
\tag{CP23}
\]

If the current coarse spacing is restored to \(h\), the physical connection bound is of order \(h^{-1}\), and the physical current bound is of order \(h^{-3}\). Equivalently, normalize the constraint as \(QA=h^{-1}B\) as in the source, so its multiplier has current dimension three. The bounds in this note are for the associated dimensionless current-unit quantities.

The first estimate in (CP23) supplies the missing independent-current bound. The connection estimate gives the plaquette and first-derivative conditions in the source joint atlas. Choose \(\rho\) after the fixed switch radius so these bounds have strict margins inside the fixed \(\alpha_0,\alpha_1,\gamma_0\) domain of the full-torus small-field source. CMP109 pp.262–263 explains that the hierarchy condition follows from these regularity conditions with smaller constants. Thus the pair, including its independently defined current, lies in that admitted joint domain throughout the complex switch polydisc.

This argument does not assert \(J_s=J(U_s)\) for \(s\ne1\). That equality is unnecessary and would reintroduce the uncontrolled differentiation that the construction avoids.

### 8. Rooted localization and its exact covariance scope

At switches vanishing between components, the localized inverse blocks separate into those components. The local nonlinear vertices and the averaging-current evaluator have fixed current-block range; collars are included in the protected/component geometry. The fixed-point solutions \(A'_s\), \(A_s\), and \(\Lambda_s\), and then \(J_s\), restricted to a component depend only on inputs in that component. This is the source component argument, now applied to the augmented pair.

Let \(E_X(U,J)\) be a localized holomorphic source with supremum \(M_X\) on the joint atlas. Evaluate it on (CP14), (CP20). The preceding domain check gives the uniform bound \(M_X\), including on complex switches. The usual rooted FTC expansion and Cauchy estimate yield

\[
E_X(U_1,J_1)=\sum_YF_{X,Y},
\tag{CP24}
\]

and, with fixed decay reserve,

\[
\boxed{
\sum_Ye^{\kappa d(Y)}
\sup_{\|B\|<\rho}|F_{X,Y}(B)|
\le C e^{p d(X)}M_X.
}
\tag{CP25}
\]

Here \(d(Z)\) is the size of a smallest connected hull in current localization blocks containing the indicated support and its protected root. The root footprint and connected-set entropy are included in \(p\). Constants do not depend on \(N\) or volume. The supports are in current localization blocks, with the fixed averaging collar included.

The source coefficients, all inverse blocks, and the averaging maps are covariant under the **simultaneous** gauge transformation of the reference background and the relative variables. For the construction proved here, this covariance is asserted on the gauge orbit of the trivial reference: transport the flat-reference operators and increments together, and use the corresponding orbit chart. It does not extend the proved norm estimates to arbitrary nonflat reference fields. In this joint action, \(\Lambda_s\) transforms in the coarse adjoint representation, and (CP20) transforms as the fine current. Thus composing with a gauge-invariant \(E_X(U,J)\) gives jointly gauge-invariant localized coefficients on that flat-reference orbit atlas.

At a fixed section with reference \(U_0=1\), an inhomogeneous gauge transformation of the physical coarse field also changes that reference section. It has not been proved here that the individual coefficients in (CP24), with the reference held at one, are invariant under that inhomogeneous coarse action. Nor has reference independence of these individual localizers been established. The full unswitched sum has the required physical invariance by (CP21).

Consequently, (CP25) establishes the **uniform current-domain and tree-bound parts** of the proposed pullback near the flat reference, with joint covariance. It does not yet establish the individually physical-coarse-invariant decomposition demanded in the strongest version of CC62. A common joint-atlas norm with a verified return map, or an intrinsic covariant localization of the augmented constrained equations, is still needed for that last identification.

### 9. Extension of the complex classical gain to joint marks

The pair construction also permits the previous classical gain to be applied to a mark that depends on the independent current. Let

\[
f_X(U,J)
\]

be a holomorphic, gauge-invariant mark on a genuine old unit-mesh joint chart, with fixed analytic margin and supremum \(M_X\). Write \(\lambda=L^{-N}\). The physical current defined by CMP109 (1.8) has one covariant difference and two inverse powers of lattice spacing. Consequently changing from current coarse units to the old unit-mesh units gives

\[
J_{\mathrm{old},s}=\lambda^3J_s.
\tag{CP26}
\]

This is a change of units; it does not assert a physical-current identity for switches different from one. At \(s=1\), (CP21) makes it exactly the physical current on the old lattice. The connection link itself is \(U_s=\exp(i\lambda A_s)\).

Use the same local axial chart as in (CC46)–(CC47), on a support with old-lattice radius \(R\) and \(\lambda(1+R)\) below a fixed small geometric constant. The chart and its complex gauge path stay inside the source domain after fixing a smaller \(\rho\). The bounds (CP23) give, uniformly in switches,

\[
\begin{aligned}
a_s^{\mathrm{ax}}&=\lambda^2a_F+r_s,
&\|r_s\|&\le C_\beta\rho\lambda^{2+\beta}(1+R)^{1+\beta},\\
\|a_s^{\mathrm{ax}}\|&\le C\rho\lambda^2(1+R),
&\|J_{\mathrm{old},s}^{\mathrm{ax}}\|&\le C\rho\lambda^3.
\end{aligned}
\tag{CP27}
\]

The last estimate uses only the bounded adjoint transport by that small axial gauge. It needs no spatial derivative or Hölder bound on \(J_s\).

For a compact simple gauge group, simultaneous constant-gauge invariance at \((U,J)=(1,0)\) kills the linear jets in both the link and current variables: the adjoint Lie algebra has no invariant linear functional. Subtract the constant and all 21 curvature-quadratic coefficients from the link-link jet. Taylor expansion in the two variables now has the following orders:

| Term | Order under (CP27) |
|---|---|
| Curvature-curvature quadratic jet | Removed by the full 21-component projection |
| Link-link error from \(r_s\) | \(\lambda^{4+\beta}\) times a fixed polynomial in \(1+R\) |
| Link-current quadratic jet | \(\lambda^5\) times a fixed polynomial in \(1+R\) |
| Current-current quadratic jet | \(\lambda^6\) |
| Total Taylor degree at least three | At least \(\lambda^6\) times a fixed polynomial in \(1+R\) |

The Taylor estimates follow from the fixed joint complex margin. In particular, for \(0<\beta<1\),

\[
\boxed{
\sup_s\left|((1-P)f_X)(U_s,\lambda^3J_s)\right|
\le C_{\beta,\rho}(1+R)^{q_\beta}
\lambda^{4+\beta}M_X.
}
\tag{CP28}
\]

Here \(P\) is the constant-plus-full-curvature-quadratic projection, represented by the same fixed Wilson seeds as in the earlier note. Its curvature coefficients use only the link-link jet at \(J=0\). In a nonwrapping chart, with the affine constant-curvature test extended across the **entire current stencil collar**, this is also the projection of the physical old-unit pullback \(f_X(U,J_{\rm unit}(U))\): the linearized current vanishes on that test, and the current linear jet of \(f_X\) is zero.

The qualification about the stencil is necessary. A periodic sawtooth version of an affine field can have a nonzero linearized current at its seam. For genuinely wrapping supports, retain the stated joint-jet projection and the finite-torus convention of CC59; do not assert exact equality with the physical-pullback projection on that test. The difference of the two quadratic projections has a fixed polynomial support bound: the unit current has finite range and bounded first derivative, while the chosen affine test has norm at most \(C(1+R)\). Cauchy estimates therefore bound the difference by \(C_\rho(1+R)^2M_X\). Such supports belong to the large-support tail in (CC51)–(CC54); their exponential input reserve pays this polynomial and the required scale power. Thus the local projection identity is used only on the nonwrapping small supports where it is exact, and wrapping corrections are controlled as tails.

Applying the rooted FTC/Cauchy construction of Section 8 to (CP28) retains this value gain. The small-support/large-support split and exponential reserve in (CC51)–(CC54) then give the same tree transfer estimate as (CC55), now for individually invariant **joint** input marks. After the engineering factor \(L^{4N}\), the remainder contracts by \(CL^{-\beta N}\), or \(CL^{-(1-\epsilon)N}\) with \(\beta=1-\epsilon\). The constants are independent of \(N\) and volume on the matched flat-reference joint chart.

The output class still has the covariance scope stated in Section 8. Thus this closes the independent-current and joint-Taylor portions of the complex classical argument on that chart; it does not turn the transfer estimate into a closed, individually coarse-invariant source norm without the remaining atlas identification.

One concrete continuation is to keep a joint-atlas source norm throughout the intermediate classical and quantum steps. In that norm, \(J\) remains an independent dimension-three variable and localizers transform the reference, relative connection, and current together. The pair construction then provides the current part of the return map without taking physical-current derivatives after localization. What remains is a **return and gluing theorem**: on overlapping admitted reference charts, the physical-section sums must agree; their local decompositions must admit uniformly bounded conversion into the next-scale joint norm; and the conversion must preserve the support-weight reserve and all 21 marginal coefficients. This is a precise alternative to demanding invariant pieces at a fixed reference from the outset. Those overlap and conversion bounds are not proved by the present flat-orbit construction.

### 10. Sources and limitations

| Ingredient | Status in this note |
|---|---|
| KKT inverse and multiplier formula | Exact algebra, (CP2)–(CP5), (CP13) |
| Nonlinear physical-current identity | Exact chain rule plus source linearization, (CP17)–(CP19) |
| Uniform multiplier and independent-current bounds | Derived from source bounded operators, Proposition 4, and averaging derivative (72) |
| Uniform switched joint domain near the flat reference | Obtained by choosing a fixed small increment radius after the switch radius |
| Rooted tree localization of the augmented pair | Same component/Cauchy construction, with the multiplier blocks included before the fixed point |
| Complex classical gain for joint connection/current marks | Derived in (CP26)–(CP28); current has dimension three, so no new marginal jet is introduced |
| Second spatial derivatives of switched connection | Not used |
| Arbitrary nonflat reference and mixed histories | Requires the corresponding augmented inverse and domain analysis; not asserted here |
| Individual coarse-gauge-invariant output at fixed reference | Not proved; joint covariance and invariance of the full sum are proved |
| Full CC62 / old-mark induction | Still requires the last gauge-atlas identification and matching at actual birth indices |

For nonflat reference fields the quadratic operator acquires the constraint-Hessian correction involving the reference multiplier. The source constructs related operators, but its projected and unprojected inverses must not be conflated. The flat-reference proof above is the completed scope; the same block strategy gives a precise extension target, rather than an automatic all-history assertion.

### 11. References and source clauses

- Balaban, **CMP102 (1985), 277–309**: action/current pairing (26)–(28), p.282; nonlinear averaging and constraint linearization (44)–(49), pp.285–286; local derivative estimate (72), p.289; nonlinear force bound Proposition 4, (97)–(98), p.293; stationarity without the artificial gauge-variation restriction (127)–(128), p.297; \(H_0\), projection, and alternative equation (129)–(143), pp.297–300; physical minimizing-section equations (170), (178)–(180), pp.305–306.
- Balaban, **CMP99 (1985), 389–434**: minimizing operators and coarse inverse (3.126), (3.129), (3.132), pp.420–422; regularity/random-walk Theorems 3.10–3.14; unit precision identity (3.156), p.428.
- Balaban, **CMP116 (1988), 1–22**: (1.2)–(1.18), switched nonlinear fixed point, analytic bounds, and component separation.
- Balaban, **CMP109 (1987), 249–301**: (1.8)–(1.19), pp.261–263, independent-current orbit atlas and the physical section.

The construction is confined to the source-admitted full-torus geometry, including its fixed localization-block partition. Bounds for arbitrary domains or histories require their own compatible operator geometry.

---
