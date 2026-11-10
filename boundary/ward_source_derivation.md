# Ward estimates, cutoff residuals and polarization tensors

**Composed-response hypothesis (CR).** Each complete boundary conclusion below assumes the displayed native-chart and spatial response estimates for the actual iterated reconstruction, with the prescribed earlier innovations and raw variables fixed, uniformly over the admitted histories. A sufficient estimate for the latent contribution is (A.8) in [Conditional-law estimates and the continuum application](../continuum/conditional_to_continuum.md), refined for the anchored exterior derivative in PG.18–PG.20. The two endpoint bounds concern the identical Wilson-subtracted primitive, its actual cutoff and its independently extended current. A direct minimizing-field derivative alone does not establish this hypothesis. The application to every required original Wilson history remains open. Complete boundary estimates and their C06/C08 applications in this chapter are conditional on CR and the other displayed source, AF, domain and support assumptions. Exact density identities and abstract inequalities retain their individually stated hypotheses.

In the projective density formulation, a sufficient comparison is
\[
 \sup_{\zeta,x,a}\left|
 \log\frac{W_\zeta(x,a)W_0(x,a_*)}
               {W_0(x,a)W_\zeta(x,a_*)}
 \right|\le\delta_r<\pi/2,
\]
on the stipulated chart with the required uniform rates and actual fixed support. The composed ordinary response is the unresolved input in its derivation. The exact partial-gauge transport and the surviving fixed-exterior derivative are given in the chapter [Gauge covariance of partial integrals and exterior scores](../continuum/partial_gauge_transport.md), equations PG.2–PG.6 and the subsequent anchored-score criterion.

**Scope:** the ordinary inherited E sector in the boundary-induction proof.  
**conclusion on that proof:** OR.19 does not follow from the calculation printed before it. The source Ward gain is measured from the actual evaluation layer. The boundary-induction insertion of the integration layer into that gain has not been justified there. This analysis does not reopen the mass/normalization argument.

**Two-age implication.** Given both endpoint inequalities on the same fixed-raw composition (CR), the interpolation supplies the missing ordinary estimate.

This note records the primary-source facts, gives two exact sufficient estimates, and distinguishes their numerical summation from the remaining application to an arbitrary admitted stopped history. A sufficient estimate stated below is not itself a certification that all of its hypotheses hold in the Wilson construction.

## 1. Three distinct indices

Use the following notation throughout:

- `b`: birth index of an ordinary E contribution;
- `n`: actual native layer on which that contribution is evaluated;
- `j`: stage of the component integration whose variables change.

The disputed case is

\[
 b\le n<j,\qquad a=n-b,\qquad c=j-n.
 \tag{SA.1}
\]

The primary source uses `j` for the birth index in its own formulas. In this note that source index is renamed `b`; its actual layer index `n` remains `n`. This renaming prevents the source birth index from being confused with the current integration stage.

In [Primitive ordinary density variations and power counts](primitive_density_bounds.md), OR.14 is a degree-preserving radius decomposition. OR.15 then uses a factor \(L^{-(5-\vartheta)(j-b)}\). CMP119 (3.56)–(3.67) supplies \(L^{-(5-\vartheta)(n-b)}\), with the actual layer `n`. CMP119 p.276 expressly instructs the reader to make that replacement of the homogeneous scale by the actual layer scale. Therefore the boundary-induction argument has omitted a response estimate in the variable `c`. This is the precise objection; it is not evidence that the desired estimate is false.

## 2. What is the same Wilson-subtracted object?

CMP119 (2.24)–(2.28), printed p.259, fixes the birth contribution as

\[
 E^{(b)}(\Lambda_b,g_{b-1},U)
 -E^{(b)}(\Lambda_b,g_{b-1},1)
 -\beta_b(g_{b-1})A(\phi_b,U).
 \tag{SA.2}
\]

Here \(\beta_b\), \(\phi_b\), \(\Lambda_b\), and the primitive ordinary bank must remain those of this birth contribution. The current integration does not authorize replacing \(\beta_b\) by a coefficient extracted from the stopped endpoint, or replacing \(\phi_b\) by a more convenient current cutoff.

The E part is represented by

\[
 E^{(b)}(\Lambda_b,U)
 =\sum_{z\in\Lambda_b^0}E^{(b)}(\Lambda_b,U,z),
 \qquad
 E^{(b)}(\Lambda_b,U,z)
 =\sum_{X\ni z,\,X\subset\Lambda_b}E^{(b)}(X,U,z).
 \tag{SA.3}
\]

The first sum is over the interior set \(\Lambda_b^0\), obtained by removing a layer of \(MR_b\)-cubes. The second sum is over the source localization domains. The Euclidean covariance used to identify the marginal coefficient is a property of the unrestricted summed bank; it is not asserted separately for every individual domain `X`. This is stated immediately after (2.28), at (2.29).

CMP119 (3.65), printed p.283, gives the exact Wilson partition

\[
 A(\phi_b,U)=\sum_{z\in T^{(b)}} A(h_z\phi_b,U).
 \tag{SA.4}
\]

For \(z\in\Lambda_b^0\), the source states \(h_z\phi_b=h_z\). Consequently the precise interior root aggregate is

\[
 \mathcal R_{b,z}(U)
 =E^{(b)}(\Lambda_b,U,z)
  -E^{(b)}(\Lambda_b,1,z)
  -\beta_b A(h_z,U),
 \quad z\in\Lambda_b^0.
 \tag{SA.5}
\]

It is legitimate to use the same expression (SA.5) at both stopped configurations. It is not legitimate to apply the final Ward cancellation separately to every absolute primitive \(E^{(b)}(X,\cdot,z)\).

The source checks the coefficient identity. Equations (3.61)–(3.64) identify the coefficient obtained by the Ward/polarization calculation with the original \(\beta_b\). Equations (3.65)–(3.66) then cancel the marginal expression with that same coefficient. The paragraph before (3.67) states that the fluctuation expressions are obtained by differentiating the resulting irrelevant terms with respect to the parameter multiplying the fluctuation field. Thus differentiating after the matching cancellation is supported in the source's own family.

There is an exact remainder to (SA.5) when the entire cutoff is retained:

\[
 \begin{split}
 E^{(b)}(\Lambda_b,U)-E^{(b)}(\Lambda_b,1)
 -\beta_b A(\phi_b,U)
 ={}&\sum_{z\in\Lambda_b^0}\mathcal R_{b,z}(U)\\
 &-\beta_b\sum_{z\notin\Lambda_b^0}A(h_z\phi_b,U).
 \end{split}
 \tag{SA.6}
\]

Any repair that uses (SA.5) root by root must account for the last term of (SA.6). This is bookkeeping for the literal own cutoff, not a request for a different renormalization.

## 3. What the primary Ward estimate actually says

CMP119 p.276 discusses the generalized history. On a cube in a layer \(\Omega_n\setminus\Omega_{n+1}\), the regularity has the scale of a `U_n` configuration. The source says to replace the homogeneous mesh by the mesh of that layer in the Section 3–4 estimates. The same paragraph says that localization of the fluctuation field yields additional small factors through propagator and minimizing-field decay, and that the resulting terms contribute to the boundary sector. It does not identify those additional factors with a new Ward power of \(j-b\).

At pp.280–283 the source derives

\[
 |\mathcal R_{b,z}(U)|
 \le C\,L^{-\lambda(n-b)},
 \qquad \lambda=5-\vartheta>4,
 \tag{SA.7}
\]

with the source activity/radius constants restored as appropriate. This is (3.67). The irrelevant remainders in (3.56) carry the same actual-layer exponent. Far carriers are treated using (3.48).

The manuscript's E14.36–E14.38 supplies the intended running-radius bookkeeping:

\[
 |\mathcal R_{b,z}(U)|
 \le C_Q E_0(1+a)^s L^{-\lambda a},
 \tag{SA.8}
\]

on its specified common native contour. The important valid feature of that decomposition is that a coefficient of derivative order `p` keeps its \(\alpha_b^{-p}\) denominator and at least `p` field factors. In particular the Wilson coefficient costs \(\alpha_b^{-2}\), not \(\alpha_b^{-5}\) applied to a quadratic numerator. The decomposition is not an independent proof that a new stopped family lies on that contour.

For two endpoints that both meet the hypotheses with actual layers at least `n`, (SA.8) implies the endpoint estimate

\[
 |\mathcal R_{b,z}(U_1)-\mathcal R_{b,z}(U_0)|
 \le 2C_Q E_0(1+a)^sL^{-\lambda a}.
 \tag{SA.9}
\]

Using two valid endpoint bounds here does not require an analytic Ward estimate on the segment joining them. If their actual layers differ, `n` may be taken to be the smaller layer only after recording both endpoint admissions and absorbing the corresponding radius comparison. The indices cannot simply be relabeled because the stage is `j`.

### 3.1 The full-cutoff theorem is stronger than the displayed root formula

CMP119 Theorem 2, (2.43), printed p.263, bounds a localized sum of E roots minus the corresponding localized Wilson action. Its test domain satisfies \(\Omega\subset B^b(\Lambda_b^0)\); the source chooses a supported smooth \(\phi\) equal to one on \(\Omega\). The theorem gives

\[
 \left|\sum_{z\in\Lambda_b^0\cap\Omega}
 [E^{(b)}(\Lambda_b,U,z)-E^{(b)}(\Lambda_b,1,z)]
 -\beta_b A(\phi,U)\right|
 \le E_1\sum_{n\ge b}L^{-\beta(n-b)}|\Gamma_n\cap\Omega|,
 \tag{SA.10}
\]

for \(\beta<1\), with volumes measured on their actual native meshes. The source then takes \(\Omega=B^b(\Lambda_b^0)\), \(\phi=\phi_b\), and sums over births to obtain (2.45). The full cutoff is therefore included in the primary theorem. What does not follow merely by naming (3.67) is a pointwise Ward bound for each residual root in the last sum of (SA.6).

An argument that uses (SA.10) in place of rootwise (SA.7) must retain its exact localized subtraction and give the localization/partition identity needed for the physical-root count. An argument that uses (SA.6) must retain and bound its cutoff collar separately. Either is a viable organization; changing the cutoff without an equality is not.

## 4. What the actual response sources provide

### 4.1 Determining-data row

CMP102 Proposition 9, (190), printed pp.308–309, concerns the actual relative minimizing map and its analytic dependence on determining data and the admitted external field. Its derivative carries the input mesh density, output factors of physical orders one, two and three, and an exponential in the source distance. The input density must be paired with its actual input measure before counting root labels.

This is a primary-source statement. The manuscript's claim that its normalized, selective, fixed-old-variable continuation has that same row is an application that also uses the particular gauge and reconstruction interfaces. It is not literally Proposition 9's statement for arbitrary final fine-link perturbations.

### 4.2 Prepared annular separation

LFR I (1.44)–(1.47), printed p.186, compares the actual successive prepared configurations. Equation (1.45) bounds their response in the native output scale. Equation (1.47) retains an exponential in the number of annuli between the output layer and the forcing layer. It is the source of a factor of the form

\[
 e^{-\Gamma(j-n)},
 \tag{SA.11}
\]

after the native output is identified with the prepared layer `n`.

The source parameter order allows a prescribed finite annular rate. CMP119 p.245 fixes the variational block size \(M_1\), takes \(M_2=L^2M_1\), then chooses \(M\) much larger. LFR I p.186 explicitly enlarges \(M\) to obtain a lower bound on the coefficient of `j-i` in (1.47), and says these conditions are independent of all scales. Increasing a fixed rate also requires retaining enough ordinary carrier decay when an attachment is away from the root. It does not allow one to use decay already spent on carrier entropy a second time.

### 4.3 Modified domains

LFR I (1.64)–(1.69), printed pp.190–191, specifies the modified background/current domains, including the reconstructed-field tests. Inspection of p.190 is important: on earlier prepared layers the norms retain their own native scales and radii; the factor \(L_0^{2\max(0,n-k_0)}\) concerns the finite top band. It is not an uncontrolled enhancement through every old age `j-n`. Page 192 bounds the top-band powers by logarithmic factors.

Page 191 provides the inclusion for the composed fluctuation substitution in these descending domains. It also discusses components whose integration stops early. These facts support a stopped-domain argument. They do not explicitly state the additional common `n`-native derivative ball for a Wilson-subtracted root aggregate at all fixed raw anchors. That extra ball is one way to prove a marked Ward estimate, but is not needed by the alternative in Section 6.

### 4.4 RL.25 by itself is not the exponential

The exact displayed RL.25 is

\[
 \frac{Cg_jP_j}{\alpha_m^{++}}(h_m/h_n)^p A_X
 \le C(1+j-m)^v(1+\ell_r)^D A_X.
 \tag{SA.12}
\]

It handles radius, coupling and mesh conversions. Its right-hand side contains no annular exponential. The relevant exponential is retained separately in RL.8 and in the source row. A proof must use both and must identify the root, the attachment, and the actual prepared grade at the attachment.

## 5. A sufficient marked estimate and its exact sum

The cleanest sufficient statement, when it can be established on the same native chart, is

\[
 |\Delta_j\mathcal R_{b,z}|
 \le C_Q E_0(1+\ell_r)^D
 (1+a)^s(1+c)^t L^{-\lambda a}e^{-\Gamma c},
 \tag{SA.13}
\]

uniformly in the admitted history, fixed earlier raw variables, the relevant two endpoints, and the ordinary external complex parameters. Here \(\lambda>4\), \(\Gamma>4\log L\). Additional residual spatial/carrier weights must be retained for any subsequent localization sum.

After the worst four-dimensional old-root density the numerical sum is

\[
 \begin{aligned}
 &\sum_{a,c\ge0}(1+a)^s(1+c)^t
 L^{4(a+c)}L^{-\lambda a}e^{-\Gamma c}\\
 &\quad=
 \left[\sum_{a\ge0}(1+a)^sL^{-(\lambda-4)a}\right]
 \left[\sum_{c\ge0}(1+c)^t e^{-(\Gamma-4\log L)c}\right]\\
 &\quad<\infty.
 \end{aligned}
 \tag{SA.14}
\]

Thus the exact exponent \(L^{-\lambda(j-b)}\) used in OR.15 is unnecessary. A Ward factor in `n-b` and a response factor in `j-n` suffice. The remaining prefix-strip count and finite-window polynomial factors can then be handled by the already established OR.2–OR.3 bookkeeping.

One proof of (SA.13) would apply directional Cauchy to the **already subtracted same function** (SA.5) on a common `n`-native ball where (SA.8) holds, then multiply by the actual response in that norm. The elementary Banach-space Cauchy implication is sound. Its actual-history ball, fixed-anchor response, and full-cutoff accounting must be established; repeating the implication alone would not close OR.19.

## 6. A weaker alternative: two bounds on the same scalar difference

A promising alternative avoids differentiating the Ward cancellation. Suppose one has both

\[
 |\Delta_j\mathcal R_{b,z}|
 \le A_{a,c}:=C_AE_0 P(a,c)L^{-\lambda a},
 \tag{SA.15}
\]

and

\[
 |\Delta_j\mathcal R_{b,z}|
 \le B_{a,c}:=C_BE_0 P(a,c)e^{-\Gamma c},
 \tag{SA.16}
\]

where `P` is a fixed polynomial, and both bounds concern the **same** aggregate, fixed subtraction, endpoints, and root allocation. The first can be the sum of two endpoint Ward bounds. The second may estimate the primitive E differential and its own Wilson differential separately; it needs no Ward cancellation.

For \(0<\eta<1\),

\[
 \min(A_{a,c},B_{a,c})\le A_{a,c}^{\eta}B_{a,c}^{1-\eta}.
 \tag{SA.17}
\]

This is a numerical interpolation of positive upper bounds, not a modification of the activity. The old-root sum converges if

\[
 \eta\lambda>4,
 \qquad (1-\eta)\Gamma>4\log L.
 \tag{SA.18}
\]

There exists such an \(\eta\) precisely when

\[
 \Gamma>\frac{4\lambda\log L}{\lambda-4}.
 \tag{SA.19}
\]

For example, with \(\lambda=9/2\), \(\Gamma>36\log L\) is sufficient for this deliberately crude response bound. Fixed polynomial losses are absorbed by the two strict exponent margins. The homogeneity in \(E_0\) is preserved because \(\eta+(1-\eta)=1\).

If the rigorous response estimate retains an additional \(L^{-pa}\), replace (SA.18) by \(\eta\lambda+(1-\eta)p>4\). The threshold becomes \(\Gamma>4(\lambda-p)\log L/(\lambda-4)\). The robust choice `p=0` avoids a false identification of the root layer with the attachment layer.

### 6.1 The attachment layer cannot be silently identified with the root layer

In the primitive sum (SA.3), a differentiated variable can lie at a point `y` of `X` whose prepared grade `q` differs from the root's grade `n`. The source row pays `j-q`; it does not automatically pay `j-n`.

The natural repair retains a fraction of the primitive full-tree carrier from `z` to `y`. If `q≤n`, the row already pays at least `j-n`. If `q>n`, the carrier must pay the prepared annuli from `n` to `q`, while the row pays from `q` to `j` when `q≤j`. If `q>j`, the carrier alone must pay from `n` to `j`. This requires a geometric inequality of the form

\[
 \kappa_{\rm res}d_b(X)
 +\delta_{\rm res}d(y,S_j)
 \ge \Gamma(j-n)-C,
 \tag{SA.20}
\]

with additional decay left for summing `X` and the output attachment. For ordinary E primitives the actual connected physical carrier is available; no contraction through an old protected footprint is licensed. The inequality has to be checked on the actual stopped determining geometry. RL.8 is the manuscript's version of such a path allocation; its use here is an application, not a new statement printed in CMP102.

### 6.2 Cutoff collars still have to be included

The interpolation argument does not remove the last term of (SA.6). One cannot assign the rootwise endpoint bound (SA.15) to that isolated Wilson term. It may be included through the source's exact localized full-cutoff theorem (SA.10), or kept as a boundary contribution with an independently proved response/counting bound.

Nor does the bare nesting \(\Omega_1\supset\Lambda_1\supset\Omega_2\supset\cdots\), (2.1), imply that every old cutoff collar still has prepared grade `b` after later operations. CMP119 p.255 allows \(\Lambda_b=\Omega_b\) following an R operation; p.256 scopes its \(2MR_b\) boundary-separation statement to regions determined by renormalization steps rather than by the R operation. Any stronger collar-grade conclusion needs the actual preparation geometry or a retained boundary ownership argument.

## 7. Scope decomposition

| Item | Status established by this analysis |
|---|---|
| Source Ward exponent is `n-b`, not automatically `j-b` | Verified directly in CMP119 p.276 and (3.56)–(3.67). |
| Same birth coupling coefficient in the Ward and Wilson terms | Verified directly in (3.61)–(3.66). |
| Cancellation is an identity before fluctuation differentiation | Verified for the source family in the paragraph preceding (3.67). |
| Ordinary primitive radius/coupling conversion has no necessary inverse-coupling loss | RL.24–RL.25 gives the intended calculation; actual native row and margins must remain those of the construction. |
| Actual map row with native measures | Primary CMP102 Proposition 9/(190). |
| Actual prepared annular response | Primary LFR I (1.44)–(1.47), on its stated geometry. |
| Choosing a sufficiently large fixed annular rate | Permitted by the source parameter order, with carrier/entropy reserves also allocated. |
| Double-age numerical summation | Proved by (SA.14). |
| Minimum-of-two-bounds numerical summation | Proved by (SA.17)–(SA.19). |
| Rootwise estimate for an isolated Wilson cutoff collar | Not supplied by (3.67); the exact residual (SA.6) must be handled. |
| Uniform application of either sufficient estimate to every stopped history at fixed raw anchors | Requires the explicit native-chart/response and cutoff allocation described above. The boundary-induction OR.14–OR.19 text does not provide it. |

## 8. What this analysis permits one to claim

The boundary-induction proof's remaining objection is real and sharply localized. The matching Wilson cancellation itself is documented correctly in the primary source. The direct summation can be repaired without claiming a stronger Ward exponent than the source supplies. In particular, the minimum-of-two-bounds method reduces the analytic task: a crude directional response of the primitive bank and its own Wilson term can be enough when combined with two endpoint Ward estimates.

The general application still requires the bounds for one literal scalar difference, with the source cutoff retained, and verification of their uniform application on every admitted stopped configuration. Until that application is complete, this analysis does not certify C-05 closed. The normalization, final mass, and local cumulant arguments are unaffected.

## Primary sources

## Addendum A. Literal cutoff collars: a source-based split

This addendum addresses the residual in (SA.6) directly. It sharpens the caution in Section 6.2: the bounded-layer-gap assertion is generally unjustified for an arbitrary birth inside the active preparation window, but a logarithmic gap follows for births below that window. The recent births can instead be treated with the literal quadratic Wilson estimate.

### A.1 Which geometry belongs to the cutoff?

The ordinary bank at the start of an attempt is the canonical bank (SA.2) for the **current admitted** \(\Lambda_b,\Omega_b\). These need not be the regions that were present when the universal primitive coefficient was first generated. After a completed R operation the source reconstructs the canonical action: LFR II p.377 adds every missing E/R/boundary term intersecting the completed region and subtracts the same terms into the residual \(V(Y)\); pp.390–391, after (1.100)–(1.102), explicitly restores the representation and inductive assumptions of CMP119 Section 2. Thus one must distinguish an old universal primitive's birth index from an obsolete, consumed hole. The latter is not automatically a surviving ordinary cutoff of the current canonical E bank.

Fix the actual attempt lower endpoint \(h=r-N_r\). LFR I (1.11), p.179, explicitly keeps

\[
 \Omega_i^{\rm prep}=\Omega_i\quad(i\le h).
 \tag{SA.A1}
\]

The intermediate determining sets (1.15)–(1.17) change the successive window strata and retain those deeper strata. A component that stops changes fewer of them. Consequently (SA.A1) holds at both endpoints of every stopped prefix of this attempt. This is the place where the fixed earlier variables and the actual prefix window matter.

### A.2 Ancient collars have a logarithmic, not necessarily bounded, grade gap

Let `b<h` and take a residual root `z` with \(h_z\phi_b\ne0\), \(z\notin\Lambda_b^0\). By the definition of \(\Lambda_b^0\), there is a point `y` outside \(\Lambda_b\) at distance

\[
 |z-y|\le CMR_bh_b.
 \tag{SA.A2}
\]

The fixed-size support of \(h_z\) changes only the constant. The nesting in CMP119 (2.1) gives \(\Omega_{b+1}\subset\Lambda_b\), so

\[
 y\notin\Omega_{b+1}^{\rm prep}
 \tag{SA.A3}
\]

by (SA.A1). In particular there is a genuinely retained fine stratum outside the old cutoff. It has not been declared to have grade `b` by convention.

The general variational geometry in CMP102 (1), p.277, requires

\[
 \operatorname{dist}(\Omega_i^c,\Omega_{i+1})
 >R M_1h_i,
 \tag{SA.A4}
\]

where `R,M_1` are fixed source parameters. This is the admissibility condition for the actual determining sets; it is different from the stronger \(MR_b\) buffer that CMP119 p.256 scopes to freshly created regions. LFR I p.179 explicitly calls its prepared sequence admissible, and uses its intermediate determining sets in the same variational construction.

If an endpoint evaluates `z` on prepared layer `n≥b+2`, then `z` lies in \(\Omega_n^{\rm prep}\), while `y` lies outside \(\Omega_{n-1}^{\rm prep}\). Equations (SA.A2)–(SA.A4) imply

\[
 RM_1h_{n-1}\le CMR_bh_b,
 \qquad
 L^{n-b}\le C_{\rm geom}R_b.
 \tag{SA.A5}
\]

The cases `n=b,b+1` satisfy the same inequality after enlarging its fixed constant. It also holds for any point in the fixed Wilson footprint with a fixed change of that constant. Hence

\[
 n-b\le C+\log_L R_b.
 \tag{SA.A6}
\]

This proves the proposed logarithmic bound for ancient literal cutoff roots without identifying original and prepared grades. It applies separately at both endpoint geometries. It does not say that all later preparations preserve every old grade.

### A.3 The primitive Wilson response retains four scale powers

The required analytic estimate for a fixed Wilson root is simpler than a Ward remainder estimate. Let `n` be the actual output layer on its bounded footprint, using a bounded neighboring-layer cover at an interface. The regularity bound and the actual curvature response have the form

\[
 |F_p(U_t)|\le C\alpha_n(\eta/h_n)^2,
 \qquad
 |\partial_tF_p(U_t)|
 \le Cg_jP_j(\eta/h_n)^2e^{-\Gamma(j-n)}
 \tag{SA.A7}
\]

for `n≤j`, on the actual admitted interpolation, with the remaining spatial weight suppressed in this display. The second estimate is the physical-order-two component of the retained determining-data row, not a derivative of the Ward remainder. Its fixed-raw-variable application must be the same one used elsewhere in the ordinary response argument.

The analytic Wilson plaquette function has zero constant and linear terms in its curvature coordinate, so on the fixed small chart

\[
 |\partial_t W(F_p(U_t))|
 \le C|F_p(U_t)|\,|\partial_tF_p(U_t)|.
 \tag{SA.A8}
\]

The fixed cutoff \(h_z\phi_b\) is not differentiated. A birth-`b` Wilson root contains at most \(C(h_b/\eta)^4\) fine plaquettes. Retaining the own coefficient bound \(|\beta_b|\le CE_0\alpha_b^{-2}\), (SA.A7)–(SA.A8) therefore give

\[
 \left|\Delta_j\big[\beta_bA(h_z\phi_b,U)\big]\right|
 \le CE_0\frac{\alpha_n g_jP_j}{\alpha_b^2}
 L^{-4(n-b)}e^{-\Gamma(j-n)}.
 \tag{SA.A9}
\]

The coupling and profile ratios in (SA.A9) are polynomial in the age, with the fixed profile exponent entering the constant; this is the same degree-preserving cancellation used in OR.17–OR.18. No inverse coupling is created. The power `4` must be kept until the root count is applied. Replacing (SA.A9) by a bare scalar value bound would lose precisely the useful compensation.

The actual row in (SA.A7) is the only response input here. This addendum does not infer it from an unmarked endpoint Ward estimate. For a footprint crossing native interfaces, one must apply the row pointwise at the actual plaquette grade before summation; admissibility prevents an unbounded grade jump across a fixed birth-scale neighborhood contained in \(\Omega_b\). At an excluded boundary one retains the actual one-sided native chart.

### A.4 Recent and ancient sums

After the old-root count \(L^{4(j-b)}\), write `a=n-b`, `c=j-n`. The scale factors in (SA.A9) become

\[
 L^{4(j-b)}L^{-4(n-b)}e^{-\Gamma(j-n)}
 =e^{-(\Gamma-4\log L)c}.
 \tag{SA.A10}
\]

For `h≤b≤j`, there are at most `N_r+1` birth labels and at most that many choices of the actual layer before `j`. The unsuppressed `a` sum therefore costs only a fixed polynomial in `N_r`; it does not produce \(L^{4N_r}\). The `c` sum converges for \(\Gamma>4\log L\). Outputs above `j` use the coarse-containment row; the analogous compensation has an additional \(L^{-4(n-j)}\), or can be bounded by the finite window. The `b>j` branch is the existing own-cell/coarse-containment argument of OR.17–OR.18.

For `b<h`, put \(q=j-b\). By (SA.A6), `a≤C+log_L R_b`. With \(\gamma=\Gamma-4\log L>0\),

\[
 e^{-\gamma c}=e^{-\gamma(q-a)}
 \le C R_b^{\gamma/\log L}e^{-\gamma q}.
 \tag{SA.A11}
\]

The number of allowed `a` values costs \(C(1+\log R_b)\). Since `R_b` is a fixed power of the source logarithm up to its standard rounding, these factors are polynomial in \(\ell_b\). The running comparison used in OR.11,

\[
 \ell_b\le C+\ell_j+\log(1+j-b),
 \tag{SA.A12}
\]

turns them into a fixed power of \(\ell_r\) and a fixed polynomial in `q`. The remaining old-birth sum is then bounded by

\[
 C_QE_0(1+\ell_r)^D
 \sum_{q\ge0}(1+q)^s e^{-\gamma q}<\infty.
 \tag{SA.A13}
\]

The actual strip count and the spatial attachment sum remain those of the retained response row. This is a direct route for the cutoff residual; it does not assign the missing term to a boundary bank without an equality.

### A.5 Scope of the addendum

The geometric logarithmic bound for ancient collars follows from current canonical cutoff ownership, unchanged deep strata, and the primary admissibility condition. The summation of the literal Wilson residual follows from that bound and the primitive curvature response (SA.A7). This removes the need for a Ward estimate on an isolated cutoff collar. It does not establish a Wilson-subtracted marked derivative theorem for the interior bank, and does not replace verification of the ordinary actual-row continuation at fixed raw anchors. The minimum-of-two-bounds route in Section 6 remains the cleaner way to avoid that stronger interior derivative theorem.

## Addendum B. Explicit ordinary-domain reserve and final analysis of the repair

The preceding cautions about the boundary-induction argument should not be confused with an impossibility result. This addendum records a concrete domain choice that removes the forward-composition ambiguity, and gives the conclusion on the **combined** two-age route, including the actual row and cutoff calculations. The conclusion at the beginning of this file remains the conclusion on the one-age boundary-induction derivation (OR.19).

### B.1 Two ordinary profiles with a fixed reserve

Fix a nonnegative integer `d_prep` large enough for the top-band factors and the finite native map/chart conversions. It is chosen from the real preparation geometry before the phase-enlargement exponent `Q`. The source modified-domain clauses and their successive-insertion inclusion then bound all the required local regularity quantities on the actual composed family by a constant times \((1+\ell_r)^{d_{\rm prep}}\) times their auxiliary input profile. This follows from the displayed \(L_0\) powers in LFR I (1.64)–(1.69), their p.192 bound, and the fixed analytic map/norm comparisons. There is no multiplication of a new map constant at every integration stage.

Use

\[
 \gamma_n=C_\gamma g_n\ell_n^{q+Q},
 \qquad
 \alpha_n=C_\alpha g_n\ell_n^{q+Q+d_{\rm prep}+2}.
 \tag{SA.B1}
\]

The first is the auxiliary ordinary map/external `++` profile; the second is the ordinary primitive activity profile. The background/current pair of profiles has the fixed coefficient ratio required by the source. Run the independently controlled ordinary E family once at the latter profile. The auxiliary maps and successive-insertion theorem can be run at the former profile, because their admission does not use a bound on an interacting normalized density.

These are **ordinary source** choices. They do not request a new larger norm for the unknown completed relative family. A fixed increase of the ordinary base exponent can equivalently absorb the difference in (SA.B1) into the parameter decomposition.

For every `n≤r`, the retained AF comparison gives \(\ell_n\ge\ell_r-C_{\rm AF}\). Taking the common ceiling so that \(\ell_r\ge2C_{\rm AF}+2\),

\[
 \frac{(1+\ell_r)^{d_{\rm prep}}}
      {\ell_n^{d_{\rm prep}+2}}
 \le C_{d_{\rm prep}}\ell_r^{-2}.
 \tag{SA.B2}
\]

Consequently

\[
 C(1+\ell_r)^{d_{\rm prep}}\gamma_n
 \le c\alpha_n
 \tag{SA.B3}
\]

with any fixed requested `c>0` after lowering the common ceiling. This estimate is uniform over all earlier `n`, not only the recent window. It is independent of `Q`, apart from fixed constants and the once-selected ceiling, because the `Q` powers cancel at the same layer.

The real centers are covered separately. Actual prefix centers have the \(L_0^{2N_0}\varepsilon_n\) enhancement of PF.2; \(q>p_0+r_0+2\), where \(R_r\) grows like a fixed power \(\ell_r^{r_0}\), leaves a vanishing fraction of \(\gamma_n\). The real fluctuation input has size \(Cg_jP_j\), also a vanishing fraction of its auxiliary profile. Thus both actual endpoints and the native determining-data interpolation for the crude response retain fixed primitive margins on the \(\alpha\) profile.

PF.1 must be read in its actual direction: a smaller strong native core is contained in the modified prefix chart. Applying the source composed-insertion theorem there produces the modified output bounds. Equations (SA.B2)–(SA.B3) then place those **actual outputs** into the larger ordinary primitive chart. No claim is made that every point of the entire modified output space already belongs to the original strong input ball.

### B.2 The actual Ward endpoints and the ordinary path have different jobs

The endpoint Ward bound uses the literal stopped configurations, their actual layer `n`, the matching bank (SA.5), and the source's nearby/far calculation. The source allows an arbitrary regular complex prepared field in CMP109 (3.30)–(3.36); the complete native/background/current admission is the retained C-02 calculation E14.26–E14.49. It does not infer an identity for an arbitrary independent extension merely from equality on the physical-current graph: the independent current is introduced by the source's specified analytic preparation before the coefficient is evaluated. CMP119 p.276 transfers these bounds with the actual layer scale. The profile reserve (SA.B3) supplies the required primitive domain for both literal stopped evaluations.

The source's current substitution is explicit. CMP109 (3.13) contains the scaled independent current together with \(\Delta_U A-P_1A+F_1(U,A)\); hence potential and gradient control alone would be insufficient. The four strong output norms retained in C-02 and CMP102 (190) are used here. CMP109 Section 4/(4.3) takes the Taylor coefficients at \(U=1,J=0\), while the prescribed independent current subsequently enters the actual prepared field. The Ward identity is therefore an algebraic coefficient identity followed by that fixed analytic substitution. It is not a claim about arbitrary extensions that happen to agree on physical fields.

The primitive path used for the crude estimate has a weaker requirement. Interpolate the small determining-data inputs in their fixed chart, leaving the history labels and all unaffected earlier raw coordinates fixed. The real cutoff bounds give a fixed small data ball; the quadratic correction in the actual \(g_jCB_j-h\widetilde D(g_jCB_j)\) input remains inside that ball. A line or logarithmic group interpolation inside the smaller ball therefore admits the entire path. It need not remain inside the support of every real selector, since it is an analytic estimating path rather than a new probability integration; its coefficient and map formulas are defined on the admitted open ball. No hard selector is differentiated.

Apply ordinary primitive Cauchy on its remaining \(\alpha_b\) margin, then the actual determining-data derivative of CMP102 (190), in all native field/current slots. This is precisely the original bank path, with its own independent-current continuation. It does not replace either endpoint by a different localized minimizing representative. The gauge-invariant ordinary E and Wilson scalars can be evaluated in the source's smooth local gauge without changing the fixed raw tuple. Their covariance does not license changing the tuple; it removes an irrelevant choice of output representative.

After the native input measure is paired with the kernel density, the physical forcing factor is \(g_jP_j\). The ratio to \(\alpha_b\), together with \((h_b/h_m)^p\), has the RL.24–RL.25 bound and no inverse-coupling loss. The logarithmic exponent difference in (SA.B1) only improves it.

### B.3 Root-to-attachment geometry can pay any prescribed finite rate

There is a direct check of the carrier part of (SA.20). Let `z` have actual prepared grade `n`, and let a responding point `y` of its birth-`b` primitive carrier have grade `m≥n+2`. Then

\[
 z\notin\Omega_{n+1}^{\rm prep},\qquad
 y\in\Omega_m^{\rm prep},\qquad
 \Omega_{m-1}^{\rm prep}\subset\Omega_{n+1}^{\rm prep}.
\]

The primary admissibility separation (SA.A4) therefore gives

\[
 |z-y|\ge cM_1h_{m-1}.
 \tag{SA.B4}
\]

The full physical birth carrier contains both points, up to fixed endpoint collars, so

\[
 d_b(X)\ge c'(M_1/M)L^{m-b-1}-C
 \ge c''L^{m-n}-C
 \quad(b\le n).
 \tag{SA.B5}
\]

For every prescribed finite rate `G`, a retained positive fraction of \(e^{-\kappa d_b(X)}\) consequently satisfies

\[
 e^{-\kappa_{\rm res}d_b(X)}
 \le C_G e^{-G(m-n)}.
 \tag{SA.B6}
\]

The finite constant is allowed to depend on the once-selected source parameters and `G`; it is independent of all scales and histories. For `m≤n+1`, the actual response row already pays `j-n`, up to one fixed endpoint step. For `m>n+1`, combine (SA.B6) with the row's `j-m` factor; if `m>j`, the carrier alone pays the whole gap. The result is (SA.20), with separate carrier and spatial shares left.

This argument uses an actual grade-`n` root and the actual connected physical E carrier. It does not turn the birth label `b` into a fictitious grade-`b` port. It also avoids a claim that an arbitrary normalized coarse row remains summable after taking a fractional power: retain the pointwise exponential envelopes and choose the source rates for their **post-interpolation** values. The remaining source spatial row is summed in its original native measure.

### B.4 Provisional assembly and a newly identified cutoff-interface check

**The minimum-of-two-bounds route repairs the numerical old-birth ordinary E estimate once its endpoint value estimate is verified for the complete truncated birth bank.** It does not need a new Ward-response theorem on a common interpolating chart. An additional endpoint issue for recent old cutoffs, recorded below, must also be checked; the application is not claimed until that check is complete.

The verified chain is:

1. The same interior bank, including its unchanged \(\beta_b\), is used at both actual endpoints. Its endpoint gain is in `n-b`, exactly as in the source.
2. The enlarged ordinary primitive margin in (SA.B1)–(SA.B3) admits the actual native comparison path at fixed earlier raw variables. Ordinary primitive analyticity and the full actual source row bound its same scalar difference without invoking a Ward derivative estimate.
3. Equations (SA.B4)–(SA.B6) connect the response attachment to the actual root and recover the `j-n` exponent. The fractional-power spatial reserve is chosen before summation.
4. The min inequality is applied to the entire endpoint difference before distributing its positive response majorant over forcing leaves. This avoids assigning endpoint cancellation to an individual marked integral or to a synthetic hybrid endpoint.
5. The strict two-age inequalities (SA.18) give the convergent old-root sum. The literal Wilson cutoff residual is retained and summed by Addendum A; recent later births keep the separate coarse-containment branch.

No new probability-law bound, normalized C coefficient bound, or statement equivalent to OR.19 is assumed in these steps. The inputs remain the already declared source construction, AF trajectory, ordinary E induction, actual native-map theorem, and admitted determining geometry. Those construction hypotheses are the scope of C-01/C-02 and the source papers; this analysis does not prove them as an unconditional construction of Yang–Mills theory.

The additional issue is specific: when `h≤b≤n<j`, preparation can expand the determining domain through the old fixed boundary of \(\Lambda_b\). A root in \(\Lambda_b^0\) can then have a large prepared evaluation age although its distance to the old cutoff is only \(MR_bh_b\). Extending the restricted polarization-tensor sum over `X⊂Λ_b` to the Euclidean invariant whole-lattice tensor need not have the factor \(e^{-cL^{n-b}}\); its cutoff error may have only \(e^{-cR_b}\). The same-coefficient cancellation remains algebraically correct, but a pure endpoint bound \(L^{-\lambda(n-b)}\) has not yet been justified at such roots. Addendum A handles the isolated Wilson-cutoff residual; it does not remove this separate truncation error in the interior E tensor.

A potential repair is to retain both terms in the endpoint bound,
\[
 C E_0\operatorname{poly}(n-b)
 \bigl[L^{-\lambda(n-b)}+e^{-cR_b}\bigr],
\]
and choose the allowed real preparation parameters so that \(R_b\gg N_r\) on the recent window. The second term then pays its worst finite-window root count \(L^{4N_r}\), after the same min estimate and spatial reserve. Another repair would prove a marked marginal, dimension-four estimate for the truncated primitive bank and use the finite number of recent births. Either repair needs its explicit source/radius verification; it cannot be replaced by relabeling these roots as boundary terms.

Accordingly, the boundary-induction argument is invalid as printed. The cutoff-interface check identified in this subsection is resolved in Addendum C below, with an explicit additional rate allocation and the retained source waiting rule. This analysis does **not** independently certify every other clause of C-05, or any later existence, coercivity, or decay theorem. Those statuses must be inherited only from their separately verified arguments, with their own scope intact.

## Addendum C. The truncated polarization tensor and the recent cutoff tail

This is the final correction to the endpoint use of the Ward estimate. It is needed in addition to the isolated Wilson-cutoff residual of Addendum A. The two are different terms and are retained separately.

### C.1 Keep the restricted marginal tensor until its cutoff error is bounded

The Ward reduction in CMP119 (3.49)–(3.56) is performed for a primitive localization domain before the Euclidean invariant tensor is obtained. In schematic index notation, its marginal term is

\[
 \frac14\,\Pi_{b,X,z}^{\mu\nu\kappa\lambda}
     \operatorname{tr}(F_{\kappa\mu}(z)F_{\lambda\nu}(z)).
 \tag{SA.C1}
\]

The antisymmetry identities are per domain; Euclidean isotropy and the identification with \(\beta_b\) occur only after the whole-lattice sum in (3.57)–(3.64). The source's nearby-to-unrestricted comparison already has its separate far-domain error at scale `n`; that error retains the usual \(e^{-cL^{n-b}}\) or irrelevant bound.

For the actual truncated bank define

\[
 \Pi_{b,z}^{\Lambda}
 =\sum_{X\ni z,\,X\subset\Lambda_b}\Pi_{b,X,z},
 \qquad
 \Pi_b^{\infty}
 =\sum_{X\ni z}\Pi_{b,X,z},
 \qquad
 T_{b,z}^{\rm cut}=\Pi_{b,z}^{\Lambda}-\Pi_b^{\infty}.
 \tag{SA.C2}
\]

The full tensor \(\Pi_b^\infty\) is the one identified with the **unchanged** coefficient \(\beta_b\). Thus subtracting the literal own Wilson term cancels this full tensor and leaves (SA.C1) with coefficient \(T_{b,z}^{\rm cut}\), in addition to the irrelevant remainders. This is an analysis of the actual same bank; it neither changes its Wilson subtraction nor installs a new anisotropic counterterm in the action.

The coefficient is evaluated at the source Taylor reference \(U=1,J=0\). It therefore makes sense for every universal ordinary localization domain, including a domain not contained in the particular \(\Lambda_b\). No value of an inadmissible physical field outside \(\Lambda_b\) is used in (SA.C2).

Ordinary Cauchy and the fixed second spatial moments give

\[
 |\Pi_{b,X,z}|
 \le CE_0\alpha_b^{-2}(1+d_b(X))^s e^{-\kappa d_b(X)}.
 \tag{SA.C3}
\]

This is the second-order coefficient bound already underlying the source's \(|\beta_b|\) estimate. A lower-order chain-rule term, if displayed separately, is bounded by the same expression on \(\alpha_b\le1\). The vacuum is subtracted exactly before this step. There is no uncanceled constant term and no replacement of a second-order denominator by a fifth-order denominator.

For \(z\in\Lambda_b^0\), every domain in the omitted sum reaches from `z` to the complement of \(\Lambda_b\). The removed \(MR_b\)-cube layer therefore gives

\[
 d_b(X)\ge c_{\rm geom}R_b-C.
 \tag{SA.C4}
\]

The factor `M` cancels between the physical collar width \(MR_bh_b\) and the birth-carrier length unit \(Mh_b\). In particular \(c_{\rm geom}>0\) is a fixed geometric factor; it does not vanish when the source activity decay rate is increased.

Reserve carrier decay first for domain entropy and the fixed spatial moments, then retain a further fixed share for (SA.C4). Summing (SA.C3) gives

\[
 |T_{b,z}^{\rm cut}|
 \le CE_0\alpha_b^{-2}e^{-\kappa_{\rm tail}R_b}.
 \tag{SA.C5}
\]

The source parameter \(\kappa\) may be chosen sufficiently large before the common ceiling. After the fixed losses, \(\kappa_{\rm tail}\) can therefore be prescribed larger than any needed fixed threshold. This is the ordinary activity decay parameter discussed in CMP119 p.260 after (2.31), not a new history-dependent rate.

### C.2 The endpoint estimate has two terms

On an actual `n`-regular endpoint, curvature in birth units is bounded by \(C\alpha_nL^{-2(n-b)}\). Multiplying (SA.C5) by the curvature pair in (SA.C1) gives

\[
 |\text{cutoff marginal term at }z|
 \le CE_0\left(\frac{\alpha_n}{\alpha_b}\right)^2
 L^{-4(n-b)}e^{-\kappa_{\rm tail}R_b}.
 \tag{SA.C6}
\]

Both coefficient radii have physical numerator factors. The ratio is at most a fixed polynomial in `n-b` by the same-profile AF comparison. The source profiles in Addendum B supply the actual common admission; the selected logarithmic exponent changes fixed constants, not a power proportional to that exponent in the running logarithm.

Consequently the correctly retained endpoint estimate is

\[
 |\mathcal R_{b,z}(U^\epsilon)|
 \le C_QE_0\ell_r^{D_A}(1+a)^{s_A}
 \left[L^{-\lambda a}
       +L^{-4a}e^{-\kappa_{\rm tail}R_b}\right],
 \qquad \epsilon=0,1.
 \tag{SA.C7}
\]

The second term can conservatively be weakened by dropping \(L^{-4a}\). No derivative of this cutoff marginal term is needed for the argument below. The ordinary crude bound still concerns the complete original scalar difference.

For ancient `b<h`, there is a stronger geometric bound. Since \(\Omega_{b+1}\) is unchanged during the prefix and is contained in \(\Lambda_b\), a root of actual grade `n≥b+2` is separated from \(\Lambda_b^c\) by at least \(cM_1h_{n-1}\). Any omitted carrier then has

\[
 d_b(X)\ge cL^{n-b}-C.
 \tag{SA.C8}
\]

This replaces the cutoff tail by \(e^{-c' L^a}\), which is bounded by a fixed constant times \(L^{-\lambda a}\). Small `a` is absorbed into the fixed constant. Thus the original single endpoint Ward majorant is valid for ancient births after this explicit cutoff check. The extra recent tail is necessary only for births in the active preparation window.

### C.3 Apply the min bound to the sum of endpoint bounds

Write `A_W` for the two-endpoint irrelevant majorant and `A_T` for the two-endpoint cutoff-tail majorant from (SA.C7). Let `B` be the crude original-bank response bound. All three are bounds used for the same original difference, and

\[
 |\Delta\mathcal R_{b,z}|
 \le\min(A_W+A_T,B)
 \le(A_W^\eta+A_T^\eta)B^{1-\eta}.
 \tag{SA.C9}
\]

The last step uses \((x+y)^\eta\le x^\eta+y^\eta\), `0<η<1`. Then distribute the positive response majorant over forcing leaves, keeping the same fractional-power spatial reserve as before. The `A_W` contribution is exactly the convergent two-age sum of Section 6. This calculation does not assume a response estimate for a separately defined cutoff-error function.

### C.4 Keep the retained source waiting rule and allocate enough tail rate

The parameter analysis of LFR II p.384 identifies the retained choice \(N_r=R_r\), up to fixed rounding/comparison constants. There is therefore no need to replace the source waiting rule by a different linear-logarithm rule. Write the comparisons in the conservative form

\[
 N_r\le C_NR_r,\qquad
 R_b\ge c_RR_r\quad(r-N_r\le b\le r),
 \tag{SA.C10}
\]

with fixed positive constants. The second follows from the finite-window AF comparison and the source rounding of radii. The real exponents must also retain the source compatibility condition for this waiting rule; the theorem group records it as \(r_0/2<p_0-p_1-1\).

For a recent birth the total old-root density is bounded by \(L^{4(j-b)}\le L^{4N_r}\). After the physical-root spatial row, its cutoff-tail contribution in (SA.C9) is therefore bounded by a fixed polynomial in \(N_r\) and \(\ell_r\), times

\[
 \exp\{4N_r\log L-\eta\kappa_{\rm tail}\min_{b\in[h,r]}R_b\}.
 \tag{SA.C11}
\]

Choose the fixed tail rate after all carrier losses to satisfy

\[
 \eta\kappa_{\rm tail}c_R
 >4C_N\log L+\varepsilon_{\rm tail},
 \qquad \varepsilon_{\rm tail}>0.
 \tag{SA.C12}
\]

Then (SA.C11) is at most \(e^{-\varepsilon_{\rm tail}R_r}\), which pays every remaining fixed polynomial in the finite preparation window. The response-age factor only improves this bound. The rate (SA.C12) is separate from the condition \((1-\eta)\Gamma>4\log L\) for the two-age main term; both must be stated in the final parameter decomposition.

This is a permissible selection of the source constants, made before lowering the common coupling ceiling. It is not a restriction imposed separately on individual histories or an assertion that the previously used smaller rate already sufficed. The result is uniform over **every history admitted by this fixed choice of source parameters and the retained waiting rule**. It does not claim the same estimate for arbitrary parameter choices that omit the required reserves.

## Addendum D. Coarser output layers must keep their actual mesh

For completeness, the range `b≤j<n≤r` is distinct from the later-birth case `b>j`. It must not be covered by simply relabeling an actual grade-`n` point as a grade-`j` point in the carrier-bridge argument: such a point can lie inside \(\Omega_{j+1}\).

Use the proper `n`-cell cover in this range. An actual forcing `j`-cell belongs to only a bounded number of compatible coarser `n`-cells. The remaining `n`-cell positions are summed by the actual normalized source row and its retained spatial envelope. Inside each such `n`-cell the density of birth-`b` roots is

\[
 C L^{4(n-b)}.
 \tag{SA.D1}
\]

The endpoint Ward factor remains \(L^{-\lambda(n-b)}\). Combining it with the crude spatial response by the same min inequality leaves the convergent birth sum

\[
 \sum_{b\le j}(1+n-b)^sL^{-(\eta\lambda-4)(n-b)}<\infty.
 \tag{SA.D2}
\]

There are at most `N_r` choices of `n>j` in the current outer bank, so the remaining label count is a fixed window polynomial. No `j-n` decay is requested here. The recent truncated-tensor error uses the density \(L^{4(n-b)}\le L^{4N_r}\) and is paid by the separate tail-rate budget (SA.C12). For ancient births its stronger cutoff distance already folds it into (SA.D2).

The literal Wilson residual retains \(L^{-4(n-b)}\), cancelling (SA.D1). Recent births then give a finite window sum. Ancient births retain the indicator \(1_{L^{n-b}\le CR_b}\le CR_bL^{-(n-b)}\); the remaining old-birth sum converges after the running-logarithm comparison. For `b>j` the entire proper-`b` atom is instead kept and the existing coarse-containment argument applies; it is not subdivided into fine `j`-cells.

One may take the retained spatial weights to satisfy `0≤w≤1`, since fixed prefactors can be kept outside their pointwise exponential envelopes. Thus the uninterpolated Wilson row \(w^{1/(1-\eta)}\) may be weakened to `w` when applying the same physical-root sum.

With this actual-mesh treatment, the three ranges `b≤n≤j`, `b≤j<n`, and `j<b` cover the ordinary bank without an implicit interchange of birth, evaluation and forcing scales.
