# Compatible limits of homogeneous source calculations

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

**Gaussian calibration hypothesis (GC).** For the signed Gaussian increments of the actual stationary source section in its thermodynamic normalization, assume $\sum_{k<n}d_k^G=d_Bn+\vartheta_n$ with $d_B>0$ and $\sup_n|\vartheta_n|\le B_G$. The coupling and stopping conclusions use this calibration and the specified source readout and replay. A physical continuum limit also requires the stated uniform normalization and full-law hierarchy estimates.

## Result and its precise level

The actual stopped sequence of [A stopped sequence with a positive weak endpoint](positive_stopped_endpoint.md) has a subsequence on which the **unmarked homogeneous source calculation** has a compatible infinite-past limit. The objects that converge are its gauge-invariant physical coarse-field pullbacks, its literal finite-parameter analytic source probes, and the coarse integration/background kernels used with those probes. The limiting raw-E birth obeys the limiting homogeneous source formula, with the complete limiting R bank as a prescribed forcing. Its curvature projection is the limit of the actual projections, and it generates the limiting coupling array.

This result does not assert compactness of primitive functions on a fixed-dimensional fine-field space: those dimensions change with the microscopic cutoff. It does not identify two different native analytic extensions from agreement on the physical-current slice. It does not close the R-operation as a map of the homogeneous banks alone; the new R terms depend on the mixed-history state, whose limit has not been constructed here.

The actual recursion and its stopped sequence are supplied by the two stated B03 results, [Homogeneous feedback and the causal Wilson recursion](causal_coupling_recursion.md) (BP.17), (BP.20), and (BP.22)–(BP.31), and [The driven homogeneous coupling endpoint](driven_coupling_endpoint.md) (DE1). This note uses those results and the original source localization/minimizer inputs. It proves the additional old-age tails, the appropriate normal-family extraction, and the passage through the homogeneous raw map. The retained geometry labels form part of the limit. A one-sided label at a rounding threshold is not silently replaced by the canonical least rounded value at the limiting coupling.

## 1. The actual arrays and fixed physical lattices

Let the trimmed stopping depths in the positive-endpoint construction be \(K_n\to\infty\), the microscopic spacings be \(a_n=\ell _0L^{-K_n}\), and the physical tori be the original compatible cubes with side \(T_n\to\infty\). For each ultraviolet offset \(s\ge0\), put

\[
 j_n(s)=K_n-s,\qquad
 h_s=\ell _0L^{-s},\qquad
 Y_{s,n}=Y_{j_n(s)}^{(n)}.
 \tag{HS.1}
\]

For every fixed \(s\), these quantities are defined for all sufficiently large \(n\). The stopped-sequence estimates give constants \(0<Y_-<Y_+<\infty\) and \(0<a<D<\infty\), fixed independently of \(n,s\), such that

\[
 Y_-+as\le Y_{s,n}\le Y_++Ds.
 \tag{HS.2}
\]

The all-pair signed comparison has the more useful form

\[
 Y_{t,n}\ge c\,[Y_{s,n}+t-s],\qquad
 Y_{t,n}\le C Y_{s,n}+D(t-s),\qquad t\ge s,
 \tag{HS.3}
\]

after increasing the fixed weak threshold to absorb the bounded Gaussian coboundary. The common source chart exponent and the complete R exponent have already been fixed. In particular one does not increase either exponent along this subsequence.

Take a diagonal subsequence such that \(Y_{s,n}\to Y_s\) for every \(s\). At each fixed offset the compatible rounded radii, maturation decisions, averaging/partition phases, and the other integer source labels take only finitely many values. Refine the same diagonal so that each finite list is eventually constant. Denote the retained labels by \(\mathfrak d_s\). All lattices at offset \(s\) are identified with the same translated lattice of spacing \(h_s\); the original odd-\(L\) center convention and compatible cubic tori give these identifications.

Write \(H_{s,n}\) for the raw homogeneous E birth at \(j_n(s)\), and \(R_{s,n}\) for its complete raw-free R birth, before only the source-prescribed vacuum subtraction. Individual current-scale R terms may not yet be mature; their exact maturity flag is retained in \(\mathfrak d\). The word complete includes the source \(R''\) ordinary descendants, not only a freshly completed \(R'\).

## 2. A necessary correction to a naive Montel argument

The functions \(E^{(b)}(X,U,J)\) of CMP109 (1.7)–(1.16) and CMP119 (2.26)–(2.28) are functions of fields on the original fine lattice restricted to a birth-scale carrier. After rescaling a birth to unit scale, its microscopic spacing is \(\xi=L^{-b}\). Thus even when the physical offset and the physical carrier are fixed, the number of fine \(U,J\) coordinates grows as \(n\to\infty\). Boundedness of these functions is not a finite-dimensional Montel theorem, and no convergence on all their varying native spaces is claimed below.

There are two valid finite-dimensional objects instead.

**Physical pullbacks.** For a finite set \(D\) of bonds on the birth determining lattice, let \(V(v)\) be a regular coarse field in a fixed small chart, with finitely many complex parameters \(v\in\mathbb C^{d_D}\), equal to a fixed flat reference away from a slightly larger fixed set. Evaluate

\[
 \widehat H_{s,n;X,D}(v)
 =H_{s,n}\bigl(X;
        U_{j_n(s)}(V(v)),
        J_{j_n(s)}(U_{j_n(s)}(V(v)))\bigr).
 \tag{HS.4}
\]

The second slot is the **stored physical-current convention of that birth**, including its scale factors. It is not the current variable of a later output silently substituted into the older slot. Define the corresponding R pullback in the same way. The source minimizing map is analytic on a fixed coarse-field neighborhood at fixed offset, with a smaller common strict margin. This is the content of CMP102 Theorem 1 and Proposition 9, as used in CMP109 after (1.16). The composed functions (HS.4) therefore are holomorphic functions of a fixed finite number of variables, bounded by the original source carrier bound.

**Literal auxiliary probes.** A source localization can evaluate an old coefficient at an independently extended current or at an \(s\)-localized field which is not a global physical minimizing pair. Such a value is not defined by (HS.4). Retain instead the exact composite

\[
 \mathcal P_{s,t,\rho,n}(p)
  =H_{t,n}\!\left(X;
           \Phi_{s,t,\rho,n}(p)\right),
 \qquad t\ge s,
 \tag{HS.5}
\]

and its R version. Here \(\rho\) specifies a finite current-scale localization record and \(p\) is its actual finite list of coarse determining variables, current integration coordinates, interpolation parameters and localizer parameters. Its map \(\Phi\) is precisely the one used in the source calculation, including the gauges and the old native/current conversion. The uniform full-domain inclusion proved for the prescribed homogeneous calculation in BP.6–BP.17 supplies a fixed smaller polydomain for these parameters at every fixed finite record.

Fine microscopic propagator walks are **not** declared to be a finite set. Their already established, absolutely summed coarse-localized coefficient is kept intact in (HS.5). After bounding the old age, the current carrier and the number of current interactions, the external determining/current/localizer variables have a fixed finite dimension. The fine coefficients that remain inside a primitive scalar are never reopened for a coordinate count.

There are countably many such finite records and finite sets \(D\). Close the catalog under every finite composition of the actual source substitution and restriction operations; this retains the probe needed when an already evaluated birth is used at a later fixed physical scale. Include also the actual finite-parameter Cartan/periodic-flux families used in the source curvature readout, with their local carrier contours and thermodynamic localization convention. Exhaust the open parameter domains by countably many compact polydiscs. These are the normal families used below. The limiting state retains the auxiliary probes (HS.5); it does not reconstruct them from equality at \(s=1\).

## 3. Uniform old-E tail, before the cluster map

Fix a current scale and write \(a=k-b\ge0\) for an incoming E age. Pair every primitive raw birth with its own vacuum and Wilson subtractions. This pairing precedes every age sum. For one fixed \(0<\theta<1\), the source nearby Ward calculation gives a scale factor \(L^{-(5-\theta)a}\). The four-dimensional number of fine roots in a current cell is \(O(L^{4a})\). The fixed native-radius comparisons give only a fixed power of \(1+a\), because

\[
 \frac{g_k\ell_k^q}{g_b\ell_b^q}
 \le C_q(1+a)^{1/2}
 \tag{HS.6}
\]

on (HS.3), after the common ceiling is chosen for the already fixed \(q\).

Retaining the coefficient order in the finite Taylor/Ward power count is essential. An order-\(p\) Cauchy coefficient has field degree at least \(p\); the Wilson subtraction has coefficient order two. Thus the near bound is the birth-resolved version of BP.10–BP.11, and the far bound is the birth-resolved version of BP.12. In a fixed slightly reduced current carrier rate, the positive primitive load from ages \(a\ge A\) is bounded by

\[
 \begin{split}
 \|V^{E,\ge A}_{k}\|_{\rm prim}
 &\le C E_0\varepsilon_E(k)\,\mathsf T_E(A),\\
 \mathsf T_E(A)
 &=\sum_{a\ge A}
 \left[
   (1+a)^{d_E}L^{-(1-\theta)a}
   +(1+a)^{1/2}L^{3a}e^{-cML^a}
 \right].
 \end{split}
 \tag{HS.7}
\]

The fixed integer or half-integer \(d_E\) includes the source finite coefficient moments. In particular

\[
 \mathsf T_E(A)\le C_E(1+A)^{d'_E}e^{-c_EA}
   \longrightarrow0 .
 \tag{HS.8}
\]

For the renormalized action evaluated on a current regular field, the same proof omits the insertion derivative and its factor \(\varepsilon_E(k)\); the tail is \(CE_0\mathsf T_E(A)\) per current root. This is CMP119 (3.65)–(3.67) and its localized form (2.43), with the native degree ledger of E14.36–E14.38 retained. No infinite sum of the separate Wilson counterterms is formed. Those terms individually have no irrelevant age factor.

The estimates are uniform on the verified source parameter contours. They therefore bound the literal probes, not merely their physical values. Finite-order derivatives on a fixed smaller output chart inherit (HS.7) by Cauchy with the current radius. No inverse old radius is applied again after summation.

## 4. Uniform mature-R tail

The complete source input satisfies

\[
 |R^{(b)}(X)|\le g_b^\nu e^{-\kappa_s d_b(X)}.
 \tag{HS.9}
\]

The calculation on CMP119 p.283 immediately after (3.67), and the explicit native power count RM.5–RM.9, retain four physical scale powers before the old roots are counted. More explicitly, with \(\lambda=L^{-a}\), the conservative nearby bound is

\[
 C g_b^{\nu-5}\lambda^4 e^{-\kappa' d_b(X)}.
 \tag{HS.10}
\]

The \(O(\lambda^{-4})\) root count cancels that factor exactly. A far carrier supplies \(e^{-c/\lambda}\), which pays the same four powers and leaves a fixed carrier reserve. Thus one may retain the age in the pre-sum RM.9 majorant rather than use only its final all-age bound.

Fixed extra native-comparison or profile powers can be paid by a fixed reduction of \(\nu\). To see this explicitly, for fixed \(d,q\) and every fixed \(\epsilon>0\),

\[
 (1+a)^d(1+\log Y_b)^q\,g_b^{\nu-5}
 \le C_{d,q,\epsilon}
 (Y_k+a)^{-p},
 \qquad
 p=\frac{\nu-5}{2}-d-\epsilon,
 \tag{HS.11}
\]

using (HS.3). The initial source-exponent choice is made once so \(p>1\). Any larger prescribed fixed \(p\) can be accommodated in that initial choice; it is not adjusted after selecting the stopped sequence. Therefore

\[
 \boxed{
 \|V^{R,\ge A}_{k}\|_{\rm prim}
 \le C\sum_{a\ge A}(Y_k+a)^{-p}
 \le C_p(Y_k+A)^{1-p}.}
 \tag{HS.12}
\]

The same bound applies to vacuum-subtracted regular R action insertions. It is uniform in the subset of mature ages selected by the actual source flags. Recent R terms can also be retained separately; at a fixed finite age their periodic-grid labels stabilize, and their complete native bound is (HS.9).

This tail is for **actual complete R inputs as fixed source primitives**. It does not assert that a future R birth is determined by the homogeneous E/R banks without the mixed-history data. No such source closure is used here.

## 5. Coarse localization and the normal-family extraction

### 5.1 A common strict physical chart

At each fixed offset \(s\), the couplings and native radii stay in a compact positive interval. Choose a fixed smaller flat coarse chart \(\mathcal B_s\), with smooth finite-support perturbations measured in the source strong norm. The real reference is flat; the group chart is complexified as in the source. Its radius can be chosen to lie within the source admission margin for all sufficiently large \(n\). The profile comparison (HS.6), together with the actual \(L^{-a}\) reconstruction gain, also admits all fixed older determining evaluations needed at that current scale.

Only such jointly admitted charts are used. This argument does not claim that an arbitrary modified-domain point belongs to an unrelated strong affine ball, or that every independent fine current is represented by a physical determining field.

### 5.2 External-data collars have a uniform tail

The actual reconstruction rows, including the physical-current and gauge conversion used by a gauge-invariant scalar, have exponential decay in the source determining metric. CMP102 Proposition 9, (190), has exponent \(e^{-\delta_0 d/8}\); its physical input measure is retained. CMP99's common-walk localization and coincidence argument supplies the corresponding comparison of localized and unlocalized determining problems.

Here the required row is not just a bound for the potential and its first difference. CMP109 (3.13)–(3.17) and E14.41 retain all four output norms, including the componentwise covariant Laplacian and the actual projection term. The physical-current conversion is the local identity LC.16–LC.24, with the normalized current convention E14.45. In that notation the source extended current has the exact form

\[
 J_{\rm ext}=\tau J+
   (\Delta_{\rm cov}-\mathcal P_U+\mathcal L_U)A+F(U,A).
 \tag{HS.13a}
\]

The commutator term satisfies \(\|\mathcal L_U A\|\le Cb\|A\|\), and the nonlinear remainder obeys
\(\|F(U,A)\|\le C(b\|A\|+\|A\|\|\nabla_UA\|+\|A\|^3)\), with constants independent of the microscopic spacing. The explicit difference formulas, or Cauchy on their fixed smaller local chart, give the same Lipschitz bound in the four normalized output norms. Consequently an exponentially small row in those norms gives an exponentially small row for the physical current as well. The actual \(\tau\) is retained; changing length units gives \(J_\xi=(h/\xi)^3J_h\), not an unscaled copied current. For an independent-current probe, its \(\tau\,\delta J\) contribution is retained separately as prescribed by E14.45–E14.48.

Simultaneous gauge changes act covariantly on the physical pair and disappear from a gauge-invariant scalar. Where the literal auxiliary probe contains a conjugated independent current, CMP109 (3.26)–(3.28), E14.31 and E14.46 retain its bounded analytic conjugation and the term in which the gauge differentiates the current center. The fixed-reference inverse-gauge conversion is the source one, as in the accepted scalar K1/current transfer; no assertion that the raw axial potential itself obeys the Landau row is made. These facts establish the complete native pair norm needed for the following scalar Cauchy estimate.

For a fixed old/current age and a fixed scalar carrier \(X\), replace determining data outside a collar of \(T\) coarse blocks by the flat reference, with a fixed smooth transition inside the reserved chart. The row bound and the native Cauchy derivative on a strict margin give

\[
 \sup_K |\widehat F_n-\widehat F_n^{[T]}|
 \le C_{s,t,X,K}\,M_{s,t,X}\,
                 (1+T)^{d_0}e^{-c_0T}.
 \tag{HS.13}
\]

Here \(K\) is a fixed compact subset of the chosen coarse/source parameter domain, \(M_{s,t,X}\) is the original scalar carrier majorant, and the constant is independent of \(n\). The same estimate holds for the finite coarse matrix entries and gauge-invariant background kernels needed by a finite source record. The normalized input row measure prevents a factor equal to the number of microscopic sites. Gauge transformations are handled in the actual admitted source chart; no unproved strong norm for a raw axial potential is substituted for the scalar row estimate.

For completeness, the estimate follows by integrating the derivative with respect to the omitted coarse data along the interpolating chart segment. The omitted-data row sum is bounded by \(C(1+T)^{d_0}e^{-c_0T}\). The scalar derivative costs one inverse native margin, while the map variation is measured in that same native norm. At a fixed age those constants are fixed. The full \(s\)-localized version is obtained from the same admitted source rows and their printed common contour; it is not inferred from agreement at the physical point \(s=1\).

### 5.3 Extract whole coarse analytic functions, not fine-coordinate coefficients

For fixed \(s,t,X,T,\rho\), each localized pullback or probe is a holomorphic function of a fixed finite-dimensional parameter vector. The source uniform bound makes it a normal family. Montel's theorem gives compact convergence on every smaller compact polydomain. Apply a diagonal extraction to all integer labels, finite supports, finite source records and a countable compact exhaustion of their domains.

The result is simultaneous convergence of:

1. every gauge-invariant physical E/R pullback (HS.4);
2. every literal analytic auxiliary E/R probe (HS.5) used by a finite source calculation;
3. the finite coarse matrix/kernel functions, source coarea factors, explicit Wilson/Haar functions and background/refinement functions occurring in those calculations.

The same subsequence is used for all of them. Cauchy's formula gives convergence of every fixed finite derivative on a further smaller compact set. Source covariance, gauge invariance, reality and vacuum-subtraction identities pass as identities of these functions. Uniform bounds pass by pointwise limits; spatially weighted sums pass by Fatou and by a slightly smaller exponential rate.

Equation (HS.13) removes the collar truncation. Large source carriers are removed with the available fixed spatial reserve. At a fixed current root,

\[
 \sum_{Y\ni x,\ d(Y)\ge T}
   e^{\kappa_0d(Y)} M_Y
 \le C e^{-cT},\qquad \kappa_0<\kappa_s,
 \tag{HS.14}
\]

after the source rooted-domain entropy is paid. We require convergence at every fixed root and its finite neighborhoods. We do not infer uniform-in-position convergence from a pointwise diagonal when the chosen localization coefficients lack individual translation covariance. The uniform root bounds and the covariance of the unrestricted homogeneous sums remain valid in the limit and suffice for the local map and thermodynamic readout.

### 5.4 The classical coarse tower can be included

The same extraction applies to the coarse classical action and refinement maps; this prevents a hidden assumption that the minimizing kernels already have a separately proved continuum limit. On a compactly supported small coarse field, the source curvature row bound gives

\[
 |\log U_n(\partial p)|
 \le C a_n^2 h_s^{-2}\,r_s
      e^{-c\,d(p,D)/h_s}.
 \tag{HS.15}
\]

The analytic Wilson plaquette term begins at second order. Thus its absolute value is at most \(C a_n^4 h_s^{-4}r_s^2e^{-c d(p,D)/h_s}\). Summing plaquettes cancels the \(a_n^{-4}\) density and yields a locally uniform bound \(C r_s^2|D^+|_s\), independent of the microscopic mesh. This gives a normal family for

\[
 \mathfrak A_{s,n}(V)=A_{a_n}(U_{j_n(s)}(V))
                         -A_{a_n}(1).
 \tag{HS.16}
\]

Localize external data first if necessary, using (HS.13). The coarse refinement data are

\[
 \Psi_{s\to t,n}(V)
       =M^{j_n(t)} U_{j_n(s)}(V),\qquad t\ge s.
 \tag{HS.17}
\]

Their finite coarse coordinates and the needed actual gauge compensators have the same fixed-chart analytic bounds. Extract them jointly, without trying to extract every microscopic bond of the minimizing field.

The coarse covariance, constraint inverse and nonlinear coordinate functions used in a finite current integral may equivalently be retained directly as probe components. Their uniform real gap and holomorphic source bounds survive the limit. They are not replaced by an unproved identification with a prescribed continuum elliptic kernel.

## 6. Exact compatibility of physical determining fields

The physical nested-minimizer identity is useful, but its scope must be correct. Let \(b<k\) and let \(U_k(V)\) be an actual regular minimum. Fix its finer data \(W=M^bU_k(V)\). The constraint \(M^bU=W\) is a refinement of \(M^kU=V\), by the source nested averaging convention. The actual minimum is consequently also a minimum on that refined constraint set. Uniqueness of the regular critical orbit gives

\[
 [U_b(M^bU_k(V))]=[U_k(V)] .
 \tag{HS.18}
\]

Brackets mean gauge orbits. When evaluating a primitive scalar, its own physical-current expression transforms covariantly with the same gauge, so gauge invariance gives equality of the scalar values. The identity does not identify the independent-current extension off the physical slice.

In the notation (HS.17), for \(s\le u\le t\),

\[
 [\Psi_{s\to t,n}]
   =[\Psi_{u\to t,n}\circ\Psi_{s\to u,n}].
 \tag{HS.19}
\]

On strict source charts the inner images have a common admission margin. Compact convergence of the inner and outer maps therefore passes this composition identity. The actual gauge compensators can be retained if a gauge-fixed version of a record is required. Gauge-invariant scalar identities pass without selecting an unjustified raw-potential norm.

For auxiliary source probes, compatibility is obtained differently: keep their literal formulas and every exact finite-source identity before taking limits. Addition, products, a finite parameter integral, fixed-order differentiation on a strict margin and finite compositions are continuous under the simultaneous compact convergence just established. If a finite-source identity is an equality only after a sum of localizer coefficients at \(s=1\), it passes only as that summed identity. No assertion about individual offphysical coefficients is extracted from it.

## 7. Continuity of the actual homogeneous raw map

### 7.1 A primitive-load perturbation estimate

The source connected map acts on a primitive weighted carrier Banach space, including the full admitted native/source parameter supremum. Its Gaussian/coarea part is fixed when the primitive E/R load is varied. By the source positive majorant there is a fixed open ball \(\|V\|_{\rm prim}<\epsilon_0\) on which the connected numerator/denominator series is holomorphic and locally bounded, with the regenerated output rate. The actual load lies in a strict smaller ball, by the common B03 ceiling.

Let \(\mathcal C(V)\) denote its interaction-dependent output. If \(\|V\|,\|V+\Delta\|\le\epsilon_0/2\), then for each \(t\in[0,1]\) the line \(V+t\Delta+z\Delta\) is admissible for

\[
 |z|<\frac{\epsilon_0}{4\|\Delta\|}
 \tag{HS.20}
\]

when \(\Delta\ne0\). Indeed the real segment has norm at most \(\epsilon_0/2\) and the additional displacement has norm less than \(\epsilon_0/4\). Banach-valued Cauchy at each segment point bounds its \(t\)-derivative by a fixed multiple of \(\|\Delta\|/\epsilon_0\). Integrating from zero to one, or differentiating the normally convergent connected series termwise, gives

\[
 \|\mathcal C(V+\Delta)-\mathcal C(V)\|_{
                    \kappa_0,K}
       \le C_K\|\Delta\|_{\rm prim} .
 \tag{HS.21}
\]

All kernels and denominators here are the same source ones. This estimate is a statement about the actual analytic cluster map, not positivity of a complex synthetic probability. Its constants do not depend on the number of old ages. Removing an old age removes its already paired own-Wilson fluctuation family, so the primitive perturbation is exactly the one estimated in (HS.7) and (HS.12).

Hence the error in a current raw birth after discarding all incoming ages at least \(A\) is at most

\[
 C_K\left[
 E_0\varepsilon_E(k)\mathsf T_E(A)
       +(Y_k+A)^{1-p}\right].
 \tag{HS.22}
\]

### 7.2 A finite truncation really has fixed integration dimension

Fix the output offset and a compact external parameter set. First truncate incoming age at \(A\), the current source carrier diameter at \(T\), and the connected expansion order at \(m\). Retain whole primitive coefficients, including their already summed fine-field dependence. With these truncations there are finitely many coarse carriers and current integration coordinates near a fixed output root. Their dimensions depend on \(A,T,m\), but not on \(n\).

The free current supports are the literal source products. Their radii converge with the fixed-offset couplings. Rescale each finite list of free current coordinates to a fixed product of unit balls. The limiting real Gaussian precision retains the source gap, and its matrix entries, determinants, constraint/coarea functions and primitive probes converge on compact sets. Finite integration therefore passes by dominated convergence. On complex parameter compacts use the actual source absolute majorant. A normalizing logarithm is the source connected-series logarithm with its fixed branch; it is not selected anew from a possibly vanishing global integral.

The tail in connected order is uniform on the strict primitive ball. The tail in current carrier or external collar is (HS.13)–(HS.14), with the source kernel/localizer reserve. These bounds remove \(m,T\to\infty\). Finally (HS.22) removes \(A\to\infty\). This order of limits also removes finite-torus winding records: for bounded age and carrier they lie outside every fixed physical neighborhood once \(T_n\to\infty\), and their complementary sum is controlled by the same spatial tail. There is no need for a limit uniform in every old microscopic grade at once.

### 7.3 The resulting exact identity

Let \(\mathfrak G_s\) denote the jointly extracted coarse classical/Gaussian/constraint/coarea kernel data and \(\mathfrak P_s\) the retained literal auxiliary probe family. Let \(\mathsf{Mat}(s,t;\mathfrak d)\) be the stabilized maturity flag. Then the limiting raw birth satisfies

\[
 \boxed{
 H_s=\mathcal H^{\,\mathfrak d,\mathfrak G,\mathfrak P}_{s}
 \left(
     \{H_t,\mathcal P_tH_t\}_{t\ge s+1},
     \{R_t:\mathsf{Mat}(s,t;\mathfrak d)=1\}_{t\ge s+1};
     Y_{s+1}
 \right).}
 \tag{HS.23}
\]

The map in (HS.23) is defined by the literal source finite-record limits just described. Its incoming E terms retain their own vacuum and curvature subtractions. It is an exact equality of the limiting physical coarse germs and of the retained source output probes at their declared parameters. It is stronger than a scalar inequality or a diagonal sequence of unrelated numbers: consecutive physical scales are related by the same limiting normalized current construction, and all finite overlapping source records have compatible limits.

The auxiliary superscripts matter. The result is a **compatible source-probe/kernel state**. It is not a theorem that the physical restrictions \(H_t,R_t\) alone uniquely determine every offphysical localized extension. It also does not identify \(\mathfrak G_s\) with a separately prescribed continuum minimizing scheme. Both are retained, actual subsequential data.

## 8. The actual curvature projection passes to the limit

Fix an output offset \(s\). Its native radius is bounded below by a positive number on the stopped subsequence. The thermodynamic projector is the physical stationary-section projection, not a derivative along an arbitrarily chosen curve in a fine native extension. The following collar construction makes its passage explicit.

Use dimensionless Lie coordinates \(v_y\) for physical determining bonds near flat. The composed scalar is (HS.4), with its actual minimizing section and the birth's physical current. Its first endpoint derivative satisfies, on a common smaller coarse chart,

\[
 |D_{v_y}\widehat H_{s,n;X}|
 \le C_s r_s^{-1}M_X e^{-c\,d_s(y,X)}.
 \tag{HS.24a}
\]

This is the complete native-pair row of Section 5.2 followed by scalar Cauchy. A second, independently supported coarse-coordinate Cauchy circle has radius \(c r_s\), with no microscopic-coordinate count. It bounds the second derivative by the same exponential in \(y\). Reversing the two derivatives gives the bound with \(z\). Taking the smaller bound, and then half the rate, yields

\[
 \|D_{v_y}D_{v_z}\widehat H_{s,n;X}(0)\|
 \le C_s r_s^{-2} M_X
 e^{-c'[d_s(y,X)+d_s(z,X)]}.
 \tag{HS.24b}
\]

The minimizing-map and current second derivatives are already included: this differentiates the whole physical composite. It is not a partial derivative at a frozen native field.

Take the source infinitesimal Cartan flux mode in these coarse coordinates, centered on \(X\), and multiply it by a smooth cutoff which equals one on the \(T\)-collar and vanishes outside the \(2T\)-collar. Denote the resulting finite-support physical determining curve by \(V_{X,T}(\varphi)\). Its first and second coordinate jets at zero have a fixed polynomial bound in \(1+D_X+d_s(y,X)\). For each finite \(T\) this is a genuine finite-parameter physical family, with the actual section \(U_{j_n(s)}(V_{X,T}(\varphi))\). It was included in the normal-family extraction. A sufficient common \(\varphi\)-radius at that fixed \(T\) is
\(c r_s(1+D_X+T)^{-m_F}\), with a fixed \(m_F\); no radius uniform in \(T\) is required.

By (HS.24a)–(HS.24b), deleting the flux mode outside the \(T\)-collar changes its complete second jet by at most

\[
 C_s r_s^{-2}M_X
 (1+D_X)^{q_F}(1+T)^{q_F}e^{-c_FT}.
 \tag{HS.24c}
\]

The same estimate includes any source-explicit lower-jet term in the stationary-section convention. All constants and \(q_F\) are independent of \(n,T\). For fixed \(T\), first pass the physical finite-support jet by compact convergence and Cauchy. Then let \(T\to\infty\) using (HS.24c). This gives the source polarization second moment and its actual thermodynamic curvature readout. Equivalently the collar limit and these finitely many derivatives commute by this uniform jet tail; a global arbitrary fine-native flux curve is never postulated.

The remaining carrier sum is controlled by the familiar local Cartan bound: on a nonwinding carrier of diameter \(D_X\), its radius is \(c r_s/[M(1+D_X)]\), so its curvature readout costs at most

\[
 C r_s^{-2}(1+D_X)^2.
 \tag{HS.24}
\]

The polynomial is summable with the source rooted exponential. More generally, the fixed polynomial in (HS.24c) is also summable with a smaller rate. Remove the carrier truncation after the collar/readout step, and remove winding by the thermodynamic localization convention. Therefore

\[
 \beta_{s,n}:=\mathcal P_sH_{s,n}
       \longrightarrow\beta_s:=\mathcal P_sH_s.
 \tag{HS.25}
\]

This uses the actual source stationary-section/physical-current readout. It is not a finite-torus flux projector substituted for the infinite-volume one.

For each finite trajectory the actual coupling installation is

\[
 Y_{s,n}=Y_{s+1,n}-\beta_{s,n}.
 \tag{HS.26}
\]

Passing to the same subsequence gives the exact limiting relation

\[
 \boxed{Y_s=Y_{s+1}-\mathcal P_sH_s.}
 \tag{HS.27}
\]

The lower and upper signed slopes also pass. If the bounded Gaussian correctors are extracted along the same countable diagonal, writing them as \(q_s\), then

\[
 \beta_s=d_B+q_s-q_{s+1}+e_s,
 \quad |q_s|\le Q,
 \quad |e_s|\le C/Y_{s+1}.
 \tag{HS.28}
\]

Thus \(Z_s=Y_s+q_s\) satisfies \(Z_{s+1}-Z_s=d_B+e_s\). The terminal value \(Y_0\in[Y_-,Y_+]\) is finite and positive, and \(Y_s\to\infty\) at least linearly as \(s\to\infty\). This is a driven infinite-past weak coupling state with an emergent strictly positive terminal coupling \(g_0=Y_0^{-1/2}\).

## 9. Discrete thresholds and the precise remaining existence tasks

The discrete label \(\mathfrak d_s\) can be an upper one-sided choice at a threshold of the original rounding rule. On this fixed label branch the finite source formulas, cutoff radii and analytic inequalities have the limits just used. The common strict analytic/cluster margins are chosen before the limit, so equality in a numerical rounding inequality does not remove the analytic margin. We retain the compatible labeled grid as part of the state. We do not conclude that its label equals the canonical minimum obtained by rerunning the rounding rule at \(Y_s\).

The proven conclusion is exactly (HS.23)–(HS.28), with the accompanying probe and refinement compatibilities. Its limitations are substantive:

| Established here | Still separate |
|---|---|
| Actual stopped Wilson sequences, fixed-offset extraction, uniform old-E and mature-R tails | A prescribed terminal \(g_{\rm phys}\) or the full frozen B05 normalization at \(\ell_0\) |
| Compatible gauge-invariant physical coarse germs and literal finite-parameter source probes | Convergence on every varying fine-native field space, or uniqueness of a continuum native extension |
| Exact homogeneous raw-E map with complete R forcing and the actual curvature recurrence | A closed limiting equation for R births, which requires the mixed-history source state |
| Joint limits of the actual coarse kernels and their finite source identities | Identification with a preselected continuum classical/gauge-fixing scheme, or independence of the subsequence/rounding branch |
| Fixed-offset unmarked homogeneous source compatibility | Full Wilson measures, marked observables, reflection/Euclidean reconstruction and nontrivial Yang–Mills existence |

In particular a proof that the mixed-history R operation has a compatible limit would upgrade the forcing in (HS.23) to an endogenous state variable. A proof that the admissible one-sided grid branches define the same physical normalized map would remove the retained-label qualification. Neither conclusion follows from Montel compactness alone, and neither is used in (HS.23).
