# Current domains, preparation budgets and E/R arithmetic

**Annex H.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Result and scope

The complete-history C0 estimate is **not closed** in this argument. In particular, the fixed-radius extension to all complete histories (Annex B) is not used here; it is not justified.

Several narrower questions about the domains are settled here:

1. CMP102 (190) controls the covariant second-order outputs of the unlocalized minimizing-field derivative. The current is not an additional unknown derivative in that theorem.
2. The loss caused by the geometrical overlap depth \(N_0\) in one LFR preparation is explicitly logarithmic: \(N_0=O(\log\log g_k^{-2})\), and every fixed power of \(L_0^{N_0}\) has an explicit finite logarithmic bound.
3. The dyadic coefficients in the LFR complex domains have a uniform capacity if the admitted parameter satisfies \(\beta<1/4\). At the endpoint \(\beta=1/4\), one of the capacities need not have a uniform positive lower bound. This is separate from the distance of an actual real cutoff configuration to the boundary.
4. Global semisimple gauge invariance kills the first holomorphic jet of each original R activity at the identity. An admitted radial complex chart therefore gives a quantitative quadratic, or marginal, R bound. The required chart and current-carrier summation have not been proved for every complete-history decoupling contour.
5. A near/far old-scale split absorbs any fixed logarithmic prefactor in an E estimate, provided both a marginal analytic estimate and an irrelevant estimate are available on the same admitted current tube. Thus proving that every intermediate prefactor is bounded is stronger than necessary.

Here **P** denotes a proof in this note, **L** a primary result with its scope retained, and **O** an application still to be established. None of the arithmetic or algebraic results below completes a hypothesis of the Yang–Mills existence theorem.

### 2. What CMP102 actually controls

#### 2.1 The five outputs in (190) — L

Write \(h_j=L^j\eta\), where \(j\) is an output layer of the determining set. Proposition 9 of CMP102 concerns the analytic minimizing-field map \(\mathcal H(B;U)\), with a fixed admissible external background \(U\), and includes the kernel estimate (190). CMP102, p. 308, has five outputs:

\[
\frac{\delta\mathcal H}{\delta B},\qquad
\nabla^\eta\frac{\delta\mathcal H}{\delta B},\qquad
\left\|\zeta\nabla^\eta\frac{\delta\mathcal H}{\delta B}\right\|_\beta,\qquad
D_U^*D_U\frac{\delta\mathcal H}{\delta B},\qquad
\Delta_U\frac{\delta\mathcal H}{\delta B}.
\tag{2.1}
\]

Their scale factors are, respectively,

\[
C\left[
h_j^{-1},\quad
h_j^{-2},\quad
(\|\zeta\|_\beta+|\zeta|)h_j^{-2-\beta},\quad
h_j^{-3},\quad
h_j^{-3}
\right]h_{j'}^{-d}e^{-\delta_0d(y,y')/8}.
\tag{2.2}
\]

Here \(j'\) is the input layer. The input-cell volume in the source's functional-derivative convention compensates \(h_{j'}^{-d}\) when the kernel is integrated against a coarse field. The background-dependent operators in (2.1) are fixed while differentiating \(B\).

Proposition 9, printed p.309, explicitly includes analytic dependence on the external regular field. This is an unlocalized minimizing-field theorem on its stated regularity spaces. It is not a theorem that every independently decoupled random-walk term satisfies the same Landau-gauge identity.

#### 2.2 Finite differences within one admitted chart — P with L input

Suppose the line segment \(B_t=B_0+t(B_1-B_0)\), \(0\leq t\leq1\), stays in one chart to which (2.2) applies uniformly. For any of the linear, fixed-background operators in (2.1),

\[
\mathcal D\{\mathcal H(B_1)-\mathcal H(B_0)\}
=\int_0^1\mathcal D\,D_B\mathcal H(B_t)[B_1-B_0]\,dt.
\tag{2.3}
\]

Consequently, with the source's input-cell measure convention,

\[
\begin{split}
h_j^s\big|
\mathcal D_s\{\mathcal H(B_1)-\mathcal H(B_0)\}(x)
\big|
\leq C
\sum_{j'}\sum_{y'\in\Gamma_{j'}}
e^{-cd(y,y')}\,|B_1(y')-B_0(y')|,
\end{split}
\tag{2.4}
\]

where \(s=1,2,3\) for the field, first derivative, and either second-order output. The Hölder version follows with its displayed cutoff factor. In particular, perturbing one or two input coordinates gives a volume-independent estimate immediately, without first proving a row-sum estimate for an arbitrary extensive perturbation.

**Proof.** Apply the fundamental theorem of calculus in the finite-dimensional complex chart, move the fixed linear spatial operator under the integral, apply (2.2), and cancel the input-cell volume against \(h_{j'}^{-d}\). No extension beyond the admitted chart is involved. \(\square\)

This settles an input needed for a possible *pair-coordinate* Cauchy argument. A full polydisc in all free coordinates is a convenient sufficient condition for a Hessian bound, but a verified bidisc for each pair of differentiated coordinates would suffice.

#### 2.3 The unlocalized current and the localized current are different issues

CMP109 (3.11), printed p.272, writes the current of an inserted field in the form

\[
J(\exp(i\xi A)U)=J(U)+D_U^*D_U A+F(U,A),
\tag{2.5}
\]

where \(F\) is local and depends on \(U,\partial U,A,\nabla_U A\). Differentiating (2.5) with \(A=\mathcal H(B)\) gives

\[
D_BJ(\exp(i\xi\mathcal H(B))U)[v]
=D_U^*D_U D_B\mathcal H(B)[v]
+D_AF(U,\mathcal H(B))[D_B\mathcal H(B)[v]].
\tag{2.6}
\]

Thus (2.1) supplies the second-order output needed for the **unlocalized** current variation; the remaining term uses the first-order outputs and the displayed local function. There is no need to postulate an additional third spatial derivative of \(\mathcal H\) to obtain (2.6).

However, the same primary page explicitly explains why one must not apply this argument to each localized summand. The localized expansion has good covariant-Laplacian bounds, but does not retain the corresponding \(D^*D\) bounds term by term. The source uses the Landau identity before localization and replaces

\[
D^*D\ \longmapsto\ D^*D+DRD^*
=\Delta_U-P+\text{local lower-order terms}.
\tag{2.7}
\]

Its analytic extension (3.13) has an **independent current variable**. The admissible insertion norm (3.14) controls

\[
|A|,\quad |P_UA|,\quad|\nabla_UA|,\quad|\Delta_UA|.
\tag{2.8}
\]

This is the correct current mechanism for the localized activities. It is not legitimate to substitute the physical current of each localized field and invoke (190). Conversely, the failure of that substitution does not mean that the source lacks a complex-current mechanism: (2.7)–(2.8) are precisely that mechanism.

The remaining application is to bound the correctly extended current, and every reconstructed-field constraint, **on a quantitative current free-coordinate tube centered at each actual real cutoff point**. Neither (2.4) nor the existence of the extension alone specifies that tube.

### 3. Exact dyadic domain budgets

In this section, \(\beta\) is the source's domain-budget parameter, distinct from the Wilson inverse coupling. The notation is retained to permit checking the cited formulas.

#### 3.1 The CMP119 coefficient

The complete-history space on CMP119 p.261 uses

\[
s_{j,n}=1-\beta(1-2^{-(j-n)}).
\tag{3.1}
\]

Hence

\[
s_{j,n}\geq1-\beta,\qquad
s_{j,n}-s_{j+1,n}=\beta\,2^{-(j+1-n)}.
\tag{3.2}
\]

The second quantity is the *one-step capacity consumed at layer \(n\)*. A lower bound on the first quantity is not a lower bound on the margin of a particular field satisfying the strict domain inequality.

#### 3.2 The two-sum coefficient in LFR I — P

LFR I (1.64), printed p.190, contains

\[
\Theta_{m;h,j,k}
=1-\beta\sum_{i=h+1}^{j}2^{-|m-i|}
-\beta\sum_{q=m+1}^{k}2^{-(q-m)}.
\tag{3.3}
\]

For all permitted indices,

\[
\Theta_{m;h,j,k}\geq1-4\beta.
\tag{3.4}
\]

The corresponding coefficients in (1.66) and (1.68) satisfy the stronger lower bounds \(1-3\beta\) and \(1-2\beta\), respectively.

**Proof.** The sum over all integer \(i\) of \(2^{-|m-i|}\) is \(3\), while the one-sided strictly positive sum is \(1\). This proves (3.4). In (1.66) the first sum is one-sided with its endpoint included, so is at most \(2\); the second is at most \(1\). In (1.68), \(m>j\), so the first sum is at most \(1\), as is the second. \(\square\)

Consequently, for any fixed admitted \(0<\beta<1/4\), these *capacities* stay uniformly positive, independently of the number of preparatory integrations. No assumption on the logarithmic exponents is needed for this calculation.

The endpoint \(\beta=1/4\) requires care. If \(h<m\leq j\), the exact formula is

\[
\Theta_{m;h,j,k}
=\frac14\left[
2^{-(m-h-1)}+2^{-(j-m)}+2^{-(k-m)}
\right].
\tag{3.5}
\]

Taking \(m\) well inside a long interval \([h+1,j]\), with \(k-m\) large, makes this coefficient arbitrarily small. Thus the convenient example \(\beta=1/4\) in the source cannot be treated as giving a fixed positive capacity in every preparatory layer. One may use a smaller admitted \(\beta\), or keep the depth-dependent loss explicitly.

This does not show a defect in the LFR construction. The source requires descending domains and controlled successive changes, and its inequalities are compatible with small positive capacities. It does identify a loss that must not be suppressed in an additional Cauchy-radius argument.

#### 3.3 The actual R-preparation age decay

LFR I p.186, (1.47), proves for the preparatory geometry

\[
\exp[-\delta\,d(y,\Omega_{j+1}^{c}\setminus Z''_{j+1})]
\leq
\exp[-\delta(M/M_1)(j-i)]
\quad (y\in\Gamma_i'',\ i<j).
\tag{3.6}
\]

This is a proved geometrical inequality for that preparation. It should not be replaced by the unsupported assertion that every old large-field layer survives every later R map.

The arithmetic of paying a dyadic reserve is exact: if a layer change is bounded by

\[
A(1+t)^b e^{-\lambda t}\alpha_i,\qquad t=j-i,
\tag{3.7}
\]

then, for \(\lambda>\log2\),

\[
(1+t)^b e^{-\lambda t}
\leq K_{b,\lambda}\,2^{-t},\qquad
K_{b,\lambda}:=\sup_{t\geq0}(1+t)^b
e^{-(\lambda-\log2)t}<\infty.
\tag{3.8}
\]

Choosing the permitted small numerical factor \(A\) so that
\(AK_{b,\lambda}\leq\beta/2\) pays a reserve of size
\(\beta2^{-(t+1)}\alpha_i\). This proves the age-budget calculation. LFR I (1.46)–(1.48) applies this mechanism to its actual preparatory fields, using the coupling comparisons and the exponential (3.6).

What is not supplied by (3.8) is the analogous bound for *every complex decoupling parameter and every reconstructed constraint* of the current E/R activity. It is that map estimate, not the summability of \(2^{-t}\), that is still needed.

### 4. An explicit bound for the R overlap depth — P with L inputs

Put

\[
\ell_k=\log g_k^{-2}\geq1.
\]

CMP119 (2.5) chooses \(R_k\) to be the smallest power of \(L\) at least \(\ell_k^r\), so

\[
\ell_k^r\leq R_k<L\ell_k^r.
\tag{4.1}
\]

LFR I p.192 gives

\[
L^{N_0-1}=R_{k-N_0+1}
\leq(L+1)(N_0+1)^{\beta_0}R_k,
\qquad L_0^2\leq L/3.
\tag{4.2}
\]

These inequalities imply the sharper bounds

\[
N_0\leq C+\frac{2r}{\log L}\log\ell_k,
\tag{4.3}
\]

and, writing
\[
\sigma=\frac{2\log L_0}{\log L}\in[0,1)
\quad\text{for }1\leq L_0,
\]

\[
L_0^{2N_0}
\leq C\,\ell_k^{r\sigma}
(1+\log\ell_k)^{\beta_0\sigma}.
\tag{4.4}
\]

Here and below constants depend only on the fixed construction parameters.

**Proof.** Let \(a=\log L>0\), \(b=\beta_0\geq0\), and
\[
M_{a,b}:=\sup_{x\geq0}
\{b\log(x+1)-ax/2\}<\infty.
\]
Taking logarithms of (4.2) yields
\[
aN_0\leq\log[L(L+1)R_k]+b\log(N_0+1).
\]
By the definition of \(M_{a,b}\),
\[
N_0\leq
\frac2a\{\log[L(L+1)R_k]+M_{a,b}\}.
\]
Use (4.1) to obtain (4.3). Next raise
\[
L^{N_0}\leq L(L+1)(N_0+1)^{\beta_0}R_k
\]
to the power \(\sigma\) and use (4.1), (4.3). This proves (4.4). The endpoint \(L_0=1\), if used, has \(\sigma=0\) and is immediate. \(\square\)

Every fixed power of \(L_0^{N_0}\), and every fixed polynomial in \(N_0\), therefore costs only a finite power of \(\ell_k\), with at most a power of \(\log\ell_k\).

**Two limits of this result.** First, \(N_0\) is the *overlap depth*, not the full preparatory depth \(N\). The source explicitly takes \(N>N_0\) and eventually requires \(N\) substantially larger. Second, this calculation concerns one preparation; it does not permit multiplying losses from an unbounded number of histories and declaring the product logarithmic. A complete-history induction must reset the activity norm rather than accumulate an uncontrolled product of these constants.

### 5. The first R jet vanishes, and what that buys

#### 5.1 Semisimple gauge invariance — P

Let \(G\) be a compact connected semisimple group, and let \(f\) be holomorphic near the origin of a finite product of copies of \(\mathfrak g_{\mathbb C}\). Suppose \(f\) is invariant under simultaneous global adjoint action. Then

\[
Df(0)=0.
\tag{5.1}
\]

**Proof.** Write \(Df(0)[X]=\sum_b\lambda_b(X_b)\). Set all components except one equal to zero. Adjoint invariance gives
\(\lambda_b(\operatorname{Ad}_gX)=\lambda_b(X)\).
Differentiating at \(g=\exp(tY)\) gives
\(\lambda_b([Y,X])=0\). Since
\([\mathfrak g_{\mathbb C},\mathfrak g_{\mathbb C}]
=\mathfrak g_{\mathbb C}\),
each \(\lambda_b=0\). \(\square\)

For the original analytic R activity of CMP119 (2.31), global gauge transformations fix the identity configuration and zero current and act adjointly on the link logarithms and current variables. Consequently, its first joint holomorphic jet at that point vanishes. This fact does not require a perturbative expansion, hypercubic covariance, or a coupling subtraction.

#### 5.2 A quantitative radial bound — P

Suppose a gauge-compatible chart has norm \(q\), and the radial path of the chart through \((U,J)\) is admitted for complex parameter \(|t|<a/q\). Suppose the primitive activity has bound

\[
|R_X|\leq M_X,\qquad
M_X=g_j^{\kappa_0}e^{-\kappa d_j(X)}
\tag{5.2}
\]

throughout that radial disc and at the target configuration. Then

\[
|R_X(U,J)-R_X(1,0)|
\leq 2M_X\min\{1,q^2/a^2\}.
\tag{5.3}
\]

**Proof.** If \(a/q>1\), compose the activity with the radial path. The resulting holomorphic function minus its value at zero has a double zero by (5.1) and has modulus at most \(2M_X\). The maximum-modulus principle applied after division by \(t^2\), first on smaller circles and then in the limit, gives \(2M_X(q/a)^2\) at \(t=1\). If \(a/q\leq1\), the difference of the two admitted values is bounded by \(2M_X\). \(\square\)

In a scale-compatible local gauge, the desired marginal chart estimate has the form

\[
q\leq C\,P(|X|)(L^{j-k})^2 Q_k,
\tag{5.4}
\]

where \(P\) is a fixed polynomial in carrier size and \(Q_k\) bounds the current physical curvature/current amplitude. Inserting (5.4) into (5.3) yields

\[
|R_X-R_X(1,0)|
\leq C\,P(|X|)^2
(L^{j-k})^4
g_j^{\kappa_0}\frac{Q_k^2}{a^2}
e^{-\kappa d_j(X)}.
\tag{5.5}
\]

The factor \((L^{j-k})^4\) is exactly the one that compensates the old-cell count in four dimensions.

**Status of (5.4).** Equation (5.5) is a proved implication; (5.4) together with admission of its radial path has **not** been proved here for the independently extended currents on every decoupling contour. The real version is what CMP119 uses in its proof of the marginal R estimate on p.283. A complex version cannot be obtained by analytically continuing the inequality. It must use the actual extension (2.7), the corresponding local gauge and reconstructed fields, and a retained analytic margin.

This identifies the algebraic cancellation needed for R quite sharply. The missing R theorem is not the cancellation of the linear term. It is the uniform, localized complex realization of the chart estimate and its subsequent current-carrier summation.

### 6. E does not require every intermediate prefactor to be bounded

The Cauchy estimate retains a radius \(\epsilon_{1,k}/g_k\) and a prefactor \(K_k^E\). Combining a marginal estimate with an irrelevant estimate before summing over old scales avoids requiring both to be uniform.

#### Proposition: near/far summation — P

Let \(\ell\geq e\), \(q>0\), \(\lambda>0\), and \(D,b\geq0\) be fixed. Suppose nonnegative old-age contributions obey

\[
H_a\leq A(1+a)^b
\min\{\ell^{-2q},e^{-\lambda a}\ell^D\},
\qquad a=0,1,2,\ldots.
\tag{6.1}
\]

Then

\[
\sum_{a\geq0}H_a
\leq C A\,\ell^{-2q}
(1+\log\ell)^{b+1}
\longrightarrow0
\quad(\ell\longrightarrow\infty).
\tag{6.2}
\]

**Proof.** Set
\[
n=\left\lceil
\frac{D+2q+1}{\lambda}\log\ell
\right\rceil.
\]
For \(a\leq n\), use the first bound and sum
\((1+a)^b\), obtaining
\[
C A\ell^{-2q}(n+1)^{b+1}.
\]
For \(a>n\), the exponential tail gives
\[
\sum_{a>n}(1+a)^b e^{-\lambda a}
\leq C_{b,\lambda}(n+1)^b e^{-\lambda n}.
\]
Its contribution is therefore at most
\[
C A\ell^{-2q-1}(n+1)^b.
\]
Combining the two estimates proves (6.2). \(\square\)

The role in the E problem is concrete. A genuine marginal estimate on a current tube of free radius comparable to \(\ell_k^q\) would give the first branch of (6.1) after two Cauchy derivatives. The renormalized fifth-order/localization gain would give the second branch, with whatever *fixed finite* logarithmic loss the domain calculation actually produces. The coupling and radius comparisons in CMP119 (2.6)–(2.9) can contribute polynomial age factors, which are allowed in \((1+a)^b\).

Thus a finite logarithmic loss, including one of the form proved in (4.4), is not by itself fatal. Nor does the arithmetic require the unsupported choice \(q_1>p_0\). It requires \(q>0\) for an **actually proved** free-coordinate margin, and both bounds on the **same** localized activities and contours.

This proposition is not an E-bulk theorem. The complex marginal branch, the irrelevant branch with all radius costs, and their common tube still have to be obtained from the complete construction. It gives a less demanding numerical closing criterion than insisting on a bounded \(K_k^E\).

### 7. What remains for the actual complete-history C0 application

The unresolved step can now be stated without conflating algebra, geometry, or analyticity.

#### D1. Admission of the actual current-coordinate contours — O

For every positive history, every actual real free-field cutoff point \(z\), every old E/R activity that contributes, and every localization/decoupling parameter used in its expansion, prove an admitted complex contour for the differentiated current coordinates. A pair-coordinate bidisc is sufficient; a full polydisc is stronger.

The verification must include all of CMP119 (2.34)–(2.39): the field and real-reference plaquettes, independently extended current, every specified reconstructed field and current, local gauge, and relative complex field with its spatial norm. During R preparation it must include the modified LFR I (1.64)–(1.69) conditions.

The radius must be quantitative. Membership in an open set, uniform positivity of the coefficients in Section 3, or a small physical cutoff alone does not give a lower bound for the distance to its boundary. Recentring the real reference field may avoid imposing \(q_1>p_0\), but that procedure has not been verified simultaneously for all the reconstructed fields and decoupling maps.

#### D2. Radius-aware complex bulk majorants — O

On those admitted contours, prove the current-carrier norm estimates. For R, Section 5 supplies the first-jet cancellation; its scale-compatible complex chart, radial path, carrier entropy reserve and full localization still need proof. For E, either the resummed majorant with a controlled radius/prefactor ratio, or the two bounds in Section 6, would suffice.

The primitive bounds
\[
|E^{(j)}_X|\leq E_0e^{-\kappa d_j(X)},\qquad
|R^{(j)}_X|\leq g_j^{\kappa_0}e^{-\kappa d_j(X)}
\]
are not yet current-carrier bounds. Without the marginal scale factor, an old-cell multiplicity \(L^{4(k-j)}\) remains. Logarithmic asymptotic freedom cannot absorb that exponential multiplicity.

#### D3. Completing C0 requires the whole conditional law — O

Even after E/R bulk closure, the existing separate accounting of boundary terms, coordinate/Jacobian terms, real cutoff support and positive history conditioning must be joined with the classical-action estimate on the same law. The fixed-domain no-R theorem remains valid in its stated model. It must not be called the complete conditional law merely because the current large-field region is empty.

The inherited-R old-scale loss remains the six-power estimate printed in CMP119 (2.46). No result here changes that to two powers. The new logarithmic-overlap calculation also does not establish the independent AF trajectory or its Wilson normalization.

### 8. Primary-source estimates

| Source and printed location | Use and limit |
|---|---|
| CMP102, pp.307–309, (182)–(190), Proposition 9 | Five derivative outputs, including \(D^*D\) and \(\Delta\); unlocalized admitted minimizing-field chart |
| CMP109, pp.272–273, (3.10)–(3.17) | Physical-current formula, reason it fails termwise after localization, independent-current repair and insertion norm |
| CMP109, pp.262–264, (1.11)–(1.18) | Analytic activity domain includes reconstructed fields; fixed-parameter primitive E norm |
| CMP119, p.255, (2.4)–(2.7) | Exact \(\epsilon_j\), \(R_j\), coupling and logarithmic comparisons |
| CMP119, pp.259–261, (2.28), (2.31), (2.34)–(2.39) | Running radii, primitive complex R norm, all multiscale domain constraints |
| CMP119, pp.276–277, (3.43) and surrounding localization argument | Full-history localization transfer and dyadic domain reserve; no radius/prefactor uniformity inferred from the transfer sentence |
| CMP119, p.283 and (2.46) | Real marginal R factor and six-power old-scale loss |
| LFR I, pp.184–186, (1.31)–(1.48) | Actual preparatory current geometry; in particular the age-distance estimate (1.47) |
| LFR I, pp.190–192, (1.64)–(1.70) and following paragraph | Two-sum domain coefficients, preparation-map inclusion, overlap-depth and \(L_0\) inequalities |
| LFR II, pp.358, 367–368, 380, 390 | Complex reference denominator, examples of polynomial logarithmic costs, new-R complex bound (1.100); not a complete current-coordinate Hessian theorem |

CMP109: [DOI 10.1007/BF01215223](https://doi.org/10.1007/BF01215223).


### 9. Final conditions of the argument

**Closed:** the precise unlocalized current derivative input; the dyadic capacity arithmetic including its endpoint loss; the explicit finite logarithmic overlap loss; semisimple vanishing of the first R jet; and the near/far numerical criterion for absorbing logarithmic E prefactors.

**Not closed:** the simultaneous complete-history complex contour admission and the corresponding radius-aware, spatially weighted E/R bulk majorants. These are the remaining mathematical estimates, not bibliographic formalities. The current-coordinate C0 theorem, and consequently the full Yang–Mills existence target, cannot be asserted on the basis of this argument.


---
