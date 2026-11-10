# Continuity of finite-volume mixed kernels

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

The compact-state construction in *Composition of mixed kernels on a compact state* supplies the positive-kernel composition on the enlarged bounded state. The continuity tests below explain why tightness of the smaller state alone does not imply composition.

## Assumptions and conclusions

The active survival reserve proves tightness of the finite-volume active raw state, including its bounded-age geometry. It does **not**, by itself, prove compactness in total variation of the full mixed integration kernels or permit dominated-convergence passage through their canonical boundary expansions.

The obstruction is narrower than a lack of any old-history control. The source keeps recent raw multiplier functions
\[
\tau_b(V_b)=T'_b(Y_b)1
\tag{FK.1}
\]
and recent boundary coefficients which can already contain arbitrarily old completed history. Bounding the age of the explicit raw slot \(V_b\) does not bound the depth of the history already integrated into the function \(\tau_b\). C05 gives a uniform native/current analytic norm at fixed raw arguments, not a cutoff-uniform continuity modulus in every raw \(V_b\) or old \(A_j\) argument.

The complete source branch does keep the mass factors needed to avoid division by tiny component masses. The mass-weighted continuity lemma MW.1–MW.9 is correct and applies after that complete grouping. What is still needed is convergence, or a sufficient common-reference approximation theorem, for the actual mass-retaining measures and raw-dependent insertions. Native positive domination at each cutoff does not already establish that cross-cutoff statement.

A fixed finite-dimensional constrained-reference envelope is a plausible and sharply formulated intermediate target. Section 5 separates its already verified pieces from its unverified common-coordinate passage. No full mixed-kernel closure is claimed on the strength of that target.

## 2. What the survival event really bounds

Let \(V\) be a fixed terminal volume and let \(\mathcal C_k\) be H2S.2's active chronological cost, with the renewal convention of H2S §2. On
\[
\mathcal C_k\le M,
\tag{FK.2}
\]
the oldest currently unintegrated lineage has age at most \(A_M=M/c_*+O(1)\). The number of occupied actual native cells is at most \(CM\), and the finitely many current regular cells add a fixed \(V\)-dependent number.

The indexing padding matters: a surviving \(A_j\) is supported in \(Z_{j+1}\cap\Omega_{j+1}\). Its raw creation age is bounded with at most one extra native grade. It is not assigned a fictitious current grade.

At a completed second-class operation the old internal genealogy ends. LFR II (1.101)–(1.104), pp.390–392, leave the whole original retained \(Y_b\), its coarse \(V_b\), and the multiplier \(\tau_b(V_b)\). That is a **new active birth \(b\)**. Its actual mass reserve pays the subsequent survival cost. The deeper completed archive is not counted again. Thus a still-explicit \(V_b\) or \(\tau_b(V_b)\) at scale \(k\) forces an active age at least \(k-b\).

For a fixed \(M,V\), stabilized grids and fixed physical output offset, these statements leave:

* finitely many native grades and geometry labels;
* finitely many group and free-coordinate slots;
* finitely many source preparation stages, since their coupling interval is compact;
* compact group variables and tight ordinary Euclidean coordinates, by the actual cutoff or NR20.1a's Schur energy.

The full normalized tail is
\[
\mathbb P_k(\mathcal C_k>M)\le e^{C_uV-uM}.
\tag{FK.3}
\]
This is enough to remove a finite-volume active-state truncation after extracting its finite-dimensional laws. It is not a tail for all histories already hidden inside the retained multiplier functions.

### 2.1 There are three relevant kinds of old data

The assertion that all older completed ancestry sits in the mature raw-free \(E/R\) banks is too strong. LFR II p.392 explicitly places previous large-field contributions both in the boundary terms and in the functions \(T'_b(Y_b)1\).

| Old data | Available control | What is not automatically supplied |
|---|---|---|
| Raw-free regular \(E\), paired with its own Wilson subtraction, and mature \(R\) | HS's birth-age tails and finite-parameter analytic probe extraction | An autonomous \(R\)-birth law from homogeneous inputs alone |
| Boundary scalars in the actual C05 positive catalog | Strong summed native/current suprema; actual creation-budget tails; fixed-raw uniformity | General equicontinuity in every old raw argument |
| Retained multipliers \(\tau_b(V_b)\) | Positivity and pointwise source upper bound, with the same literal self normalization | Total-variation compactness of the archived raw-\(V_b\) function or of its conditional internal law |

The explicit footprint of the last two rows has finite recent age on (FK.2). Their already integrated archive need not.

## 3. Two genuine old-tail statements, and their limits

### 3.1 Regular banks

The HS estimates control the old regular fluctuation primitives after the source cancellations. Schematically,
\[
\mathcal T_E(A)
 \le C\sum_{a\ge A}
 \left[(1+a)^{D_E}L^{-(1-\theta)a}
       +(1+a)^{D'_E}L^{3a}e^{-cML^a}\right]\to0,
\tag{FK.4}
\]
and, after choosing the fixed \(R\) power sufficiently large,
\[
\mathcal T_R(A)\le
 C\sum_{a\ge A}(Y_k+a)^{-p}
 \le C'(Y_k+A)^{1-p}\to0,\qquad p>1.
\tag{FK.5}
\]
These are primitive estimates at their retained source scope. The fixed connected map is Lipschitz on a strict small ball, so they control the effect of old regular inputs in that map.

### 3.2 The additional relative-boundary catalog

C05 keeps a separate positive budget for each genuine creation event, including its once-only transport reserves. With \(\sigma_r\) AF-summable and
\[
f_r\le C[g_r^{-u}(1+\ell_r)^v e^{-cR_r}]^{1/18},
\tag{FK.6}
\]
the total surviving budget from creation events before \(k-A\), in the same actual positive norm, is at most
\[
e^{C\sum_r\sigma_r}\sum_{r\le k-A}f_r.
\tag{FK.7}
\]
The monotone AF envelope makes the right side tend to zero uniformly in cutoff. For example it is bounded by a fixed constant times
\[
\int_{cY_k+c'A-C_0}^{\infty}
 t^{u'}(1+\log t)^{v'}e^{-c'(\log t)^{r_0}}\,dt,
\qquad r_0>1.
\tag{FK.8}
\]
The fixed-power/log factors and the conservative fractional exponent have been included in \(u',v',c'\). On a fixed finite-volume, bounded-age geometry, the finite native-root count turns this into a value bound with a constant depending on \(M,V\).

This is a tail of the **additional catalog's retained creation budgets**, with its canonical operations kept literal. Linear transport does not count an old family again as a new event. It does not assert that every internal history in \(\tau_b\) was an independently small nonself creation. The wholly contained self action belongs to the canonical operation. In particular (FK.7) is not a theorem allowing one to delete an arbitrary deep portion of \(\tau_b\)'s defining integral.

## 4. Exact source mass cancellation and the MW lemma

LFR II (1.103) writes the second normalized expansion in the form
\[
\left(\prod_{i=1}^m\tau_i\right)
 \left[\left(\prod_{i=1}^m\Pi_i\right)e^{B'}\right],
\qquad
\Pi_i=\tau_i^{-1}T'_i,\quad \tau_i=T'_i1.
\tag{FK.9}
\]
The product includes the actual component self actions, selectors and old normalizers in the positions defined by (1.71)–(1.72). As a complete expression,
\[
\left(\prod_i\tau_i\right)
 \left[\left(\prod_i\Pi_i\right)F\right]
  =\left(\prod_iT'_i\right)F.
\tag{FK.10}
\]
Any unused component still carries its scalar mass. This identity requires no componentwise lower bound on \(\tau_i\).

The literal operations on disjoint regions factor as in CMP119 (2.19); their chronological order inside a region is the one in (2.20)–(2.22). One must not flatten an overlapping ordered history into independent slots. On the fixed disjoint current component family in (FK.9), however, the complete unnormalized product is exactly the product measure used by (FK.10).

For finite positive \(\mu,\nu\) on a common raw space and bounded insertions, the stated MW theorem gives
\[
\begin{split}
&\left|
 \mu(1)\kappa_{\mu/\mu(1)}(F_1,\ldots,F_m)
 -\nu(1)\kappa_{\nu/\nu(1)}(F_1,\ldots,F_m)
 \right|\\
&\qquad\le
 2^m m!\,\|\mu-\nu\|_{\mathrm{TV}}
                   \prod_i\|F_i\|_\infty.
\end{split}
\tag{FK.11}
\]
The value at zero mass is zero. The proof differentiates a partition monomial
\[
\mu(1)^{1-r}\prod_{B\in\pi}\mu(F_B);
\]
its \(r\) moment derivatives and \(r-1\) mass derivatives leave no inverse mass after positivity bounds the undifferentiated moments. The sum of the resulting coefficients is at most \(2^m m!\).

Consequently:

* A complete mass-retaining connected coefficient is stable under an absolute positive-history truncation, if its total-variation error is proved.
* Vanishing component branches can be passed without a positive lower bound on every rare \(\tau_i\).
* The isolated logarithmic boundary coefficient in (1.104) is not automatically mass-weighted. Its normalized cumulant cannot be assigned (FK.11) after discarding the outside masses.
* For physical branch integrals it is often preferable to use (FK.10) directly and divide only by the full partition function, whose finite-volume lower bound is H2S.14a.
* Unbounded observables require an actual joint uniform-integrability estimate before removing a truncation. MW does not replace such an estimate.

The common-sector complex version of MW is available only when the two measures have the same pointwise phase cone on a common reference. Separate native operator bounds or separately nonzero masses are insufficient.

## 5. The proposed finite-dimensional reference, with exact scope

### 5.1 Verified source structure

CMP119 p.258, (2.21), has an unrestricted-group factor of the form
\[
dV_j\,
 \delta(\overline V_jV_{j+1}^{-1})\,
 \zeta(\Omega_{j+1}^{\,c}),
\tag{FK.12}
\]
and an actual free-coordinate factor
\[
dA_j\,\chi(\cdots)\,
 \exp\!\left[
  -\tfrac12\langle A_j,K^{\rm Schur}_jA_j\rangle
 \right].
\tag{FK.13}
\]
The source explicitly says that after an \(R\)-operation this general form remains, with changed characteristic functions and possibly empty free-coordinate region. Cross-component quadratic terms are assigned to \(B\), rather than pretending the original Gaussian factorizes on arbitrary disjoint supports.

On a bounded-age finite geometry, the list of variables in (FK.12)–(FK.13) is finite. Actual regular free-coordinate parametrizations have the retained positive precision and fixed small-domain coarea bounds. Source \(E/R/B\) value estimates give an upper action bound by a constant times the finite native-volume count, apart from the nonpositive Wilson part. The remaining normalization logarithms have bounded grades and couplings. The current retained \(\tau_b\)'s have pointwise upper bounds. These observations strongly suggest a uniform upper envelope for a **complete branch**, even without raw equicontinuity of each \(\tau_b\).

### 5.2 A product-Haar assertion would be wrong

The joint raw variables in (FK.12) satisfy averaging constraints. They need not have a density with respect to the product Haar measure of all old and new bonds. Treating the delta functions as bounded factors would be invalid.

A correct fixed-geometry reference must instead be one of:

1. the literal finite Haar/averaging-constraint measure with its free adjoint coordinates; or
2. an explicitly constructed parametrization of that measure by a fixed finite list of independent Haar/free variables, including the actual coarea factors.

The averaging maps are source-defined and the source preserves their normalization. For the pure compact hierarchy without a moving regular boundary, one can orient the reference chronologically and integrate each constrained coarse variable first. On a mixed geometry, the boundary/regular-field support conventions and the finite gauge/free-coordinate charts must be retained in the same construction. The convergence of their actual pullbacks, not just the number of variables, is the needed common-reference statement.

The physical-state argument still requires a full cutoff-independent parametrization of every such mixed constrained branch, including all failed preparations and its moving regular boundary. It therefore does not certify a blanket product-space \(L^\infty\) bound for every full mixed kernel.

### 5.3 What the envelope would prove, once this exact reference is supplied

For clarity, the functional-analytic step is elementary. Suppose a fixed branch has been put on one finite measure space \((\Omega_\gamma,\lambda_\gamma)\), with complete densities
\[
0\le w_{n,\gamma}\le C_{M,V}
\quad \lambda_\gamma\hbox{-almost everywhere}.
\tag{FK.14}
\]
Then a subsequence converges weak-* in \(L^\infty(\lambda_\gamma)\):
\[
w_{n,\gamma}\stackrel{*}{\rightharpoonup}w_{\infty,\gamma},
\qquad
0\le w_{\infty,\gamma}\le C_{M,V}.
\tag{FK.15}
\]
Thus the complete branch measures converge against each fixed \(L^1(\lambda_\gamma)\) test and their limits remain absolutely continuous. Finitely many branch labels can be handled simultaneously; the uniform normalized tail (FK.3) then removes the active-cost truncation at fixed volume.

This proves weak compactness of complete measures. It does not prove convergence in total variation, convergence of individual raw multiplier functions, or continuity of nonlinear products of separately weak-* convergent coefficients. It is not a dominated-convergence theorem unless almost-everywhere or sufficiently strong convergence of the actual integrands is additionally supplied.

## 6. Why native domination is not the missing raw theorem

C05 uses one positive real-center reference for a fixed actual kernel and a common admitted native/current chart:
\[
|d\Pi_{n,\xi}|\le M\,d\mu_{n,0}.
\tag{FK.16}
\]
The construction is uniform in \(n\), but the reference \(\mu_{n,0}\) can vary with the cutoff and its already integrated history. It also treats the external real raw tuple as fixed. Equation (FK.16) is not a convergence theorem for that raw tuple or for the sequence \(\mu_{n,0}\).

A simple example isolates the missing logical implication. On a raw coordinate \(x\in[0,1]\), let
\[
\tau_n(x)=a\left(1+\tfrac12\cos(2\pi n x)\right),
\qquad 0<a\ll1.
\tag{FK.17}
\]
These are uniformly positive, uniformly bounded rare mass functions, independent of every native parameter. Their native response is zero and a trivial normalized inner kernel can have the same domination constant for every \(n\). Nevertheless they have no \(L^1\)-convergent subsequence: their weak limit is \(a\), while the oscillating part has a fixed nonzero \(L^2\) norm and uniform \(L^\infty\) bound. An \(L^1\) limit would therefore force an \(L^2\) limit, a contradiction.

Moreover
\[
\tau_n^2\stackrel{*}{\rightharpoonup}
 a^2(1+\tfrac18)\ne a^2.
\tag{FK.18}
\]
Thus separate weak-* extraction does not commute with products. This is a counterexample to an inference from the available norm statements, not a claim that the actual Yang–Mills masses have this behavior.

The complete branch-density extraction avoids this particular product mistake by keeping the whole product together. It produces a measure-level limit. To identify its factors as the canonical limiting source functions, one needs a raw modulus, strong convergence, or a larger jointly retained kernel/probe state with a proved composition theorem.

## 7. Hard selectors require their actual constrained boundary test

Suppose (FK.14) is available and a hard selector is
\[
\chi_n=\mathbf1_{\{f_n\le t_n\}}.
\]
If \(f_n\to f\) in measure on the common reference, \(t_n\to t\), and
\[
\lambda_\gamma\{f=t\}=0,
\tag{FK.19}
\]
then \(\chi_n\to\mathbf1_{\{f\le t\}}\) in \(L^1(\lambda_\gamma)\). Hence
\[
\left|\int(\chi_n-\chi)G\,w_{n,\gamma}\,d\lambda_\gamma\right|
 \le C_{M,V}\|G\|_\infty\|\chi_n-\chi\|_{L^1}
 \longrightarrow0.
\tag{FK.20}
\]
This is a valid way to remove selector boundaries without asking for a conditional lower mass.

The source tests which are literal norms of unconstrained free coordinates have the required zero-measure boundaries in their actual Lebesgue parametrization. For example a positive-radius Euclidean norm sphere is null. A nonconstant real-analytic selector function also has a null level set on a smooth finite-dimensional reference chart, provided it is not identically at the threshold on a connected chart component.

Those hypotheses must be checked for the actual selector. A constraint can make an ambient variable constant on its integration fiber. The localized-minimizer tests also involve their actual varying fine supports; convergence of a fixed list of coarse analytic probes alone does not prove convergence of every fine supremum test. Finally, finite-cutoff nondegeneracy is not enough if the limiting test becomes identically equal to its threshold.

Absent (FK.19), one may retain selector labels in the limiting state, as LC.1 does. That gives a legitimate labeled probability limit but not the assertion that the labels equal a recomputation of the canonical selector from the limiting raw fields.

## 8. Exact next theorem which would upgrade the result

A sufficient finite-volume bridge would establish, for every fixed active-cost truncation and finite source window:

1. A common actual free-coordinate/constrained reference for all admitted mixed branches, with all gauge/coarea factors included and a uniform complete-branch envelope as in (FK.14).
2. Simultaneous convergence of the literal finite-parameter classical/Gaussian/constraint maps on these branches, including the support needed by each hard test, and the boundary-null statement (FK.19) where a canonical selector is to be recomputed.
3. A strong approximation theorem for the recent raw-dependent archived kernels and bounded insertions, or an explicitly defined jointly retained measure-valued probe family whose composition identities pass without multiplying unrelated weak-* limits.
4. The exact mass retention (FK.9)–(FK.10), followed by the global denominator. MW then removes the small-component-mass obstruction; (FK.3) removes the active truncation.
5. For physical unbounded insertions, a separate joint uniform-integrability bound. The contact-flat microscopic estimate and the very-old active-sector estimate can supply particular tails, but do not give every required off-diagonal observable bound.

Items 1–3 are genuine remaining source-interface requirements. The existing C05 common chart, H2S normalized survival reserve and HS homogeneous probe limit make them concrete, but do not already prove them.

## Remaining conditions

The following statements are established here or directly source-verified:

* renewal-corrected bounded age/count of explicit active raw slots on a cost sublevel;
* the exact distinction between active genealogy and archives inside recent \(\tau_b\);
* the regular-bank and C05 positive-creation tail scopes;
* literal retention and cancellation of canonical masses in a complete source branch;
* the mass-independent continuity theorem's valid application boundary;
* the weak-* and selector-passage implications of a correctly supplied common constrained reference.

The following are deliberately left open:

* a complete common-reference/coarea construction for all truncated mixed branches;
* the necessary raw-variable compactness or joint measure-valued composition theorem for archived recent \(\tau_b/B_b\);
* every minimizer-selector boundary condition needed to recover the canonical mixed map.

Accordingly physical-state tightness does not promote local active-state tightness to a proved full mixed \(R\)-kernel limit, and does not claim Yang–Mills existence.
