# Full-law reset-jet bounds for moment-controlled marks on an admitted chart

**Annex AK.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

**Neither H-03 nor H-02 is completed by this note.** The new result removes a restriction from the previous native-chart reset theorem: the incoming marks need not be bounded or analytic in the native background. Their full-law moment bounds suffice for the newly generated kernel currents and for the entire frozen-input reset jet. The theorem uses the actual normalized old-component posterior and keeps its nonsmall self action. It does not replace that posterior by the fresh R reference.

The actual joined multiscale coordinate map, the pointwise regulator estimate and the sector/interface part of the M-03 norm remain additional requirements. The exact remaining requirements are listed in Section 6. In particular, closing the boundary reconstruction estimate (BM.24) would not, by itself, close all of H-03.

### 1. Source input and the full-law disintegration

We retain the fixed eligible component geometry of Annex AG. Write its actual posterior as

\[
 \pi_x(d\eta)
 =\frac{e^{H_x(\eta)}M_x(d\eta)}{M_x(e^{H_x})},
 \qquad
 H_x=\sum_{Y:\,i\in J(Y)}V_Y.
 \tag{HP.1}
\]

Here \(x\) contains the retained native data and the other components' variables, while \(\eta\) contains every variable and old-history label integrated by the component operation \(\mathsf T'_k(X_i)\). The self-component action from LFR II (1.69), the old characteristic functions, graph sums, reference factors and integration Jacobians are inside \(M_x\). No smallness of that self action is assumed. The law of \((x,\eta)\) is

\[
 d\mu(x,\eta)=d\nu(x)\,\pi_x(d\eta).
 \tag{HP.2}
\]

The primary input is LFR II, CMP 122 (1989), pp.379–380, (1.71)–(1.75). On the source's admitted fixed native domain the component integral is its real positive integral times a bounded analytic exponential. The dependence on the native \((U,J)\) variables occurs in the quadratic form and the self-component action; all the original integrated histories remain present. The source controls the variation of that large self action by its localized connections to the current input. Its normalized bound does not estimate the reciprocal of a small real component mass separately.

The exact defining representation of (1.73) permits the same domination argument for integrable marks. One must first verify that a proposed coordinate variation stays within the source domain (1.65). We assume such an admitted chart in Sections 2–4, and do not infer one from the completed regular R activity theorem.

For definiteness, let \(|z|<\rho\) parameterize one native direction at each real datum \(x\), with a common fixed support for \(\eta\). On a sufficiently small concentric disc the full posterior has the representation

\[
 \pi_{x,z}(d\eta)
 =r_{x,z}(\eta)\pi_x(d\eta),\qquad
 r_{x,z}(\eta)
 =\frac{e^{\theta_x(z,\eta)}}{\pi_x(e^{\theta_x(z,\cdot)})},
 \quad \theta_x(0,\eta)=0.
 \tag{HP.3}
\]

For the actual component operation, \(\theta\) is the recentered source exponential plus the change of \(H_x\). The quantitative radius of Annex AG, (HL.22), is one sufficient choice. If the parameter radius or the constants depend on \(x\), the conclusions below retain those costs pointwise. A numerical bound uniform in \(x\) requires the corresponding actual uniform domain estimate.

### 2. Domination gives kernel currents without analytic marks

#### Proposition HP.1 — a dominated complex posterior

Suppose throughout \(|z|<\rho\) that \(\theta_x\) is holomorphic in \(z\), measurable in \((x,\eta)\), and

\[
 \sup_{x,\eta,|z|<\rho}|\theta_x(z,\eta)|
 \le \log(3/2).
 \tag{HP.4}
\]

Then the denominator in (HP.3) has absolute value at least \(1/2\), and

\[
 |r_{x,z}(\eta)|\le3.
 \tag{HP.5}
\]

For every \(F(x,\cdot)\in L^1(\pi_x)\), regarded as frozen when \(z\) varies, the function \(\pi_{x,z}F\) is holomorphic and

\[
 \left|\left.\partial_z^q\pi_{x,z}F\right|_{z=0}\right|
 \le 3q!\rho^{-q}\pi_x|F|,
 \qquad q\ge0.
 \tag{HP.6}
\]

For the complete finite-difference current on the inner half-disc,

\[
 \sup_{0<|t|\le\rho/2}
 \left|\frac{\pi_{x,t}F-\pi_xF}{t}\right|
 \le\frac6\rho\pi_x|F|.
 \tag{HP.7}
\]

**Proof.** The inequalities

\[
 |\pi_x(e^{\theta_x})|
 \ge1-\pi_x|e^{\theta_x}-1|
 \ge2-e^{\log(3/2)}=\tfrac12,
 \qquad |e^{\theta_x}|\le\tfrac32
\]

give (HP.5). The integrable majorant \(3|F|\) justifies holomorphy of the integral, for example by Morera's theorem and Fubini, followed by continuity from dominated convergence. Cauchy's estimate on any circle of radius less than \(\rho\), then passage to the supremum radius, gives (HP.6). The positive majorant in (HP.6) is independent of the circle angle and of the order of differentiation. Expanding in powers of \(t\) gives

\[
 \left|\frac{\pi_{x,t}F-\pi_xF}{t}\right|
 \le3\pi_x|F|\sum_{q\ge1}\rho^{-q}|t|^{q-1}
 =\frac{3}{\rho-|t|}\pi_x|F|,
\]

which proves (HP.7). The normalizer and all its derivatives remain in the analytic density \(r_{x,z}\). \(\square\)

In particular, conditional Jensen gives the actual full-law estimate

\[
 \left\|\sup_{0<|t|\le\rho/2}
 \left|\frac{\pi_{x,t}F-\pi_xF}{t}\right|\right\|_{L^p(\nu)}
 \le\frac6\rho\|F\|_{L^p(\mu)},\qquad p\ge1.
 \tag{HP.8}
\]

This has no inverse real component mass. It is a bound for the new normalized-kernel current with the incoming expression frozen. It is not a bound on a moving hard selector or on a varying coordinate pullback outside the common chart. Direct differences and previously generated current records still follow the exact separate transport formula (M.30).

### 3. Entire reset jets with only full-law moment inputs

Let \(I\) be a set of \(m\) distinguished source labels. For every nonempty \(J\subseteq I\), let \(A_J(x,\eta)\) be the incoming logarithmic-jet coefficient, and suppose

\[
 \|A_J\|_{L^p(\mu)}
 \le C^{d+1}(d!)^{p_0}b^d p^{sd},
 \quad d=|J|,\quad p\ge1,
 \quad C\ge1,\ p_0\ge1,\ s\ge0.
 \tag{HP.9}
\]

All incoming higher vertices are retained. The source labels are distinguished before repeated field types are identified. Define the frozen-input reset coefficient by the finite formal identity

\[
 A_I^+(x,z)
 =\left.\partial_I
 \log\pi_{x,z}\exp\!\left(
        \sum_{\varnothing\ne J\subseteq I}t_JA_J\right)
        \right|_{t=0}
 =\sum_{\mathcal P\in\Pi(I)}
   \kappa_{\pi_{x,z}}(A_J:J\in\mathcal P).
 \tag{HP.10}
\]

No actual exponential integrability in the source variables is assumed: (HP.10) is a finite source jet.

#### Theorem HP.2 — full-law moment and kernel-derivative bounds

More generally suppose that (HP.3) is a holomorphic mass-one complex kernel with

\[
 |r_{x,z}|\le K,\qquad K\ge1,
 \tag{HP.11}
\]

on a uniform disc of radius \(\rho\). Set

\[
 B_{C,K}=C(1+2KC).
 \tag{HP.12}
\]

Then, for \(m\ge1\), \(p\ge1\) and \(q\ge0\),

\[
 \boxed{
 \bigl\|\partial_z^q A_I^+(\cdot,0)\bigr\|_{L^p(\nu)}
 \le q!\rho^{-q}B_{C,K}^{m}
       (m!)^{p_0}b^m(mp)^{sm}.
 }
 \tag{HP.13}
\]

The inner-half-disc finite-difference envelope satisfies the same inequality with \(q!\rho^{-q}\) replaced by \(2/\rho\). Proposition HP.1 supplies \(K=3\) for the actual old posterior on its admitted shrunken chart.

**Proof.** We first record the precise conditional-product estimate. Take coefficients \(F_1,\ldots,F_k\) of degrees \(d_1,\ldots,d_k\), with \(\sum_i d_i=m\), and a partition \(\pi\) of \(\{1,\ldots,k\}\). Conditional independent replicas of \(\eta\), one for every block of \(\pi\), give

\[
 G_\pi(x)=\prod_{B\in\pi}
               \pi_x\!\left(\prod_{i\in B}|F_i|\right).
\]

Jensen on this replicated conditional law, followed by Hölder with exponents \(m/d_i\), gives

\[
 \|G_\pi\|_{L^p(\nu)}
 \le\prod_{i=1}^k
        \|F_i\|_{L^{pm/d_i}(\mu)}.
 \tag{HP.14}
\]

Every individual conditional replica has the original full-law marginal \(\mu\). There is no product-law assumption on the original histories. By (HP.9), the right side is at most

\[
 C^{m+k}b^m(mp)^{sm}
          \prod_{i=1}^k(d_i!)^{p_0}.
 \tag{HP.15}
\]

We dropped only the factors \(d_i^{-sd_i}\le1\).

For the complex kernel, a product of moments occurring in a cumulant is bounded by \(K^{|\pi|}G_\pi\). Thus the cumulant coefficient sum costs at most

\[
 \sum_{\pi\in\Pi_k}(|\pi|-1)!K^{|\pi|}
 \le K^k k!2^{k-1}
 \le(2K)^k k!.
 \tag{HP.16}
\]

For the outer reset partitions of the source labels, the ordered-composition identity gives

\[
 k!\sum_{\substack{\mathcal P\in\Pi(I)\\|\mathcal P|=k}}
       \prod_{J\in\mathcal P}(|J|!)^{p_0}
 \le(m!)^{p_0}\binom{m-1}{k-1}.
 \tag{HP.17}
\]

Indeed, after ordering the blocks and their sizes, the left side is
\(m!\sum_{d_1+\cdots+d_k=m}\prod_i(d_i!)^{p_0-1}\), and each product is at most \((m!)^{p_0-1}\). Combining (HP.15)–(HP.17) bounds the \(L^p\) norm of (HP.10), uniformly on the disc, by

\[
 C^m(m!)^{p_0}b^m(mp)^{sm}
       \sum_{k=1}^m(2KC)^k\binom{m-1}{k-1}
 \le B_{C,K}^m(m!)^{p_0}b^m(mp)^{sm}.
 \tag{HP.18}
\]

Cauchy's formula and Minkowski's integral inequality prove (HP.13). To prove the supremum finite-difference statement without interchanging a supremum and an \(L^p\) norm, retain the positive conditional-product majorant before applying (HP.14). That single majorant controls every circle angle. Its Taylor-coefficient bounds sum to at most \(2/\rho\) times the same majorant on the inner half-disc, as in (HP.7). Applying (HP.14) afterward proves the asserted envelope estimate. \(\square\)

At a physical current-scale input budget \(b=h^{-4}\) and \(s=1\), the averaged value part of M-03 has exactly the factor \(h^{-4m}(mp)^m\). The new kernel derivative, with its explicit radius cost, also fits the averaged grade \(m+1/2\), because

\[
 \frac{(mp)^m}{[(m+1/2)p]^{m+1/2}}\le1
 \qquad(m,p\ge1).
 \tag{HP.19}
\]

This statement assumes the displayed current-scale input budget. If the input is a bare field with \(b=a^{-4}\), then the output still carries \(a^{-4m}\); no coarse-scale improvement has been obtained from conditional expectation.

### 4. Localization errors retain the same moment structure

Let \(E\) contain the source dependence of the component base and of the input coefficients. Let

\[
 R_x(z,\eta)
 =\sum_{\substack{Y:\,i\in J(Y)\\Y\not\subseteq E}}V_Y(z,x,\eta),
 \qquad
 \sup_{x,\eta,|z|<\rho_0}|R_x(z,\eta)|\le\lambda_E.
 \tag{HP.20}
\]

Interpolate the cross action by \(H_t=H^E+tR\), \(0\le t\le1\). Suppose the common analytic tube constructed in HL.6 is admitted, and denote its radius by \(\rho\). The same real posterior \(\pi_x=Q_{1,x,0}\) will be used in every full-law moment. On the real slice,

\[
 \frac{dQ_{t,x,0}}{d\pi_x}
 =\frac{e^{-(1-t)R_x(0,\cdot)}}
        {\pi_x(e^{-(1-t)R_x(0,\cdot)})},
 \qquad
 \left|\frac{dQ_{t,x,0}}{d\pi_x}\right|
 \le e^{2\lambda_E}.
 \tag{HP.21}
\]

Consequently the complex interpolated kernels are dominated by

\[
 |Q_{t,x,z}|\le K\pi_x,
 \qquad K=3e^{2\lambda_E}.
 \tag{HP.22}
\]

#### Theorem HP.3 — localized full-jet current errors with moment inputs

Under (HP.9), (HP.20) and the common-tube premise, let \(A_I^{+,1}\) and \(A_I^{+,0}\) denote the full and truncated frozen-input reset jets. There is an explicit constant \(D_{C,K}\), depending only on \(C,K\), such that

\[
 \boxed{
 \left\|\partial_z^q
       (A_I^{+,1}-A_I^{+,0})(\cdot,0)\right\|_{L^p(\nu)}
 \le q!\rho^{-q}\lambda_E
       D_{C,K}^{m+1}(m!)^{p_0}b^m(mp)^{sm}.
 }
 \tag{HP.23}
\]

The same inner-half-disc finite-difference envelope has \(2/\rho\) in place of \(q!\rho^{-q}\). In particular, for all sufficiently large truncation regions for which \(\lambda_E\le1\), one may use the fixed \(K=3e^2\), independent of \(E\).

**Proof.** The exact derivative of a normalized interpolated integral is

\[
 \partial_tQ_{t,x,z}F
 =Q_{t,x,z}(FR_x)-Q_{t,x,z}F\,Q_{t,x,z}R_x.
 \tag{HP.24}
\]

Equation (HP.22) and \(\|R_x\|_\infty\le\lambda_E\) give the pointwise majorant

\[
 |\partial_tQ_{t,x,z}F|
 \le K(1+K)\lambda_E\pi_x|F|.
 \tag{HP.25}
\]

Differentiate each product of moments in the cumulant formula. For a partition with \(r\) blocks, the extra factor is at most

\[
 rK^{r-1}K(1+K)\lambda_E
 =rK^r(1+K)\lambda_E.
\]

After its cumulant coefficient \((r-1)!\) is included, summing over partitions of \(k\) input coefficients costs at most

\[
 (1+K)\lambda_E K^k k!2^{k-1}.
 \tag{HP.26}
\]

Apply the conditional-product estimate (HP.14), the source partition count (HP.17), and integrate \(t\) from zero to one. For example,

\[
 D_{C,K}=2(1+K)C(1+2KC)
 \tag{HP.27}
\]

is more than sufficient. The positive conditional-product majorants remain independent of the circle angle, so Cauchy's formula and the same envelope argument as in Theorem HP.2 prove all the stated derivative and finite-difference bounds. \(\square\)

Theorem HL.9 supplies an actual source-coordinate bound for eligible components of the form

\[
 \lambda_E\le C\alpha(1+R_k)^d
    \exp\{-\omega[r-D_dR_k-2]_+\}
 \tag{HP.28}
\]

when \(E\) is the prescribed radius-\(r\) neighborhood. Choose

\[
 r_0=D_dR_k+2+
       \omega^{-1}\log^+\!\bigl(C\alpha(1+R_k)^d\bigr).
 \tag{HP.29}
\]

Then \(\lambda_E\le1\) for \(r\ge r_0\), and the localization error in (HP.23) has an exponential tail in \(r-r_0\), with a fixed factorial exponent. The radius \(\rho\) remains the actual chart radius from HL.22; (HP.28) is not a proof that its pullback to every retained M-03 coordinate is uniform.

### 5. A necessary distinction in the spatial carrier summation

The source-coordinate radial estimate (HP.28) is useful, but a particular radial truncation representation is not automatically summable in the strong M-03 carrier weight. That weight is

\[
 w_h(X)=\exp\{\kappa[|X|+\mathsf t_h(X)]\}.
 \tag{HP.30}
\]

If one assigns the \(n\)-th radial correction to an entire four-dimensional ball of radius \(r_0+n\), its size can be of order \((r_0+n)^4\). A bound of order \(e^{-\omega n}\) then only yields the numerical majorant

\[
 \sum_{n\ge0}\exp\{c\kappa(r_0+n)^4-\omega n\},
 \tag{HP.31}
\]

which diverges. Thus this route does not prove the desired uniform weighted carrier norm. This calculation says that the upper bounds do not sum; it does not claim that the actual corrections attain those upper bounds or that no other representation works.

A usable M-03 application must retain a suitably thin localized carrier expansion, prove a stronger volume estimate, or establish an equivalent controlled representation. The relative-tree estimate in LFR II (1.68) pays the exterior connections. It does not independently pay the volume of every newly included nonsmall component after its mass has canceled in the conditional posterior. The original factorization and geometry assumptions must remain in that argument.

This is separate from the joined-\(p\) reconstruction problem in C-05. A successful proof of the latter supplies domain and response information for the coordinate map; it does not by itself perform the strong marked carrier sum just described.

### 6. Exact remaining H-03 and H-02 obligations

The original H-03 test is a spatial estimate for the exact reset jet uniform in the remaining history, in the chosen current-scale framework. This note proves its averaged-moment and fixed-chart kernel-current part under explicit chart and source-localization premises. The following actual applications are still open:

1. **Prepared multiscale image and retained radii.** Compose the actual current/retained map into LFR II (1.65)–(1.75), including every independent-current argument and the nonsmall self action. Check the complete support and one uniform quantitative radius for the directions actually used. The regular integrated R activity is a different object.
2. **Pointwise regulator pushforward.** M-03 includes a supremum relative to the output regulator, as well as full-law moments. A sufficient pointwise estimate would control the conditional old regulator, its pulled-back input footprints and its path/difference costs in terms of the new regulator. For example, the schematic inequality
   \[
    \pi_x(\widehat R_{h,X}^{m})
       \le C^{m+1}(m!)^r\widehat R_{h',Y}^{m}
    \tag{HP.32}
   \]
 would require its actual scale factor, carrier \(Y\), degree and coordinate-map costs to be specified and proved. Conditional \(L^p\) contraction proves the averaged part, not (HP.32). This note does not assume (HP.32).
3. **Complete weighted carrier sum.** Retain insertion anchors and actual dependency footprints, and sum the value, direct-difference and separate kernel-current records with (HP.30). The radial bound alone does not prove this step.
4. **Sector changes and interfaces.** For a change that moves a hard selector or changes the common support, use the actual signed-kernel finite difference (M.29). The normalized analytic score on a fixed chart cannot replace that signed measure. If a smoother extension is used off the physical support, record it and prove that it agrees on the entire physical support with a sufficient reserve.
5. **Incoming scale budget.** The new theorem can use the full input jet and its decorated moment budget. That input must still be the actual transported current-scale jet. Its bare \(a^{-4m}\) budget is not relabeled \(h^{-4m}\).

For H-02, the primary source does prove the small factors and unnormalized component estimates in LFR II (1.79)–(1.89), including the recursive reserve for unrepaired regions. The estimate is unnormalized. These inequalities do not bound the normalized probability of an inherited low-margin event after conditioning on retained data. A local ratio/surgery theorem or an actual full-law marked insertion estimate is still needed, with the geometric and physical-scale losses included. None of those missing estimates follows from (HP.13).

### 7. Application conditions

| Item | Result |
|---|---|
| Actual old-component posterior and nonsmall self action | Retained exactly from (1.71)–(1.75) and Annex AG. |
| Kernel-current bound with only full-law \(L^p\) input | Proved in Proposition HP.1 and Theorem HP.2, on the admitted chart. |
| All generated higher input vertices | Included in the full reset formula (HP.10). |
| Localized kernel-current errors with the same moment budget | Proved in Theorem HP.3, with the actual discarded-carrier majorant and radius displayed. |
| Newly generated factorial loss from reset partitions | None beyond the stated \(p_0\); the moment factor \((mp)^{sm}\) remains explicit. |
| Strong pointwise/current/geometry carrier norm | Not proved; Sections 5–6 identify its remaining tests. |

Primary source: T. Balaban, *Large Field Renormalization. II. Localization, Exponentiation, and Bounds for the R Operation*, CMP **122** (1989), 355–392, pp.379–380 for the actual fixed-support tilt and normalization; pp.380–387 for the unnormalized large-field reserve. The finite probability, domination, combinatorial and moment arguments above are proved in this note. References to M-03 are to Annex Y.
