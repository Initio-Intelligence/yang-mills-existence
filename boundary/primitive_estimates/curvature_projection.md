# Curvature projection in a positive diameter norm

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

**Relation to the later coupling proof.** This note isolates a bounded readout and explains why C05 alone cannot supply the bulk reset feedback. The separate transfer requirement stated in Section 5 is proved in [Homogeneous feedback and the causal Wilson recursion](../../physical_scale/causal_coupling_recursion.md); its zero-marker endpoint and actual causal application are treated there and in [The driven homogeneous coupling endpoint](../../physical_scale/driven_coupling_endpoint.md). The projection lemma itself retains exactly the subspace and hypotheses below.
title: "B03: bounded curvature projection and the unresolved reset-feedback input"

---

# Finding

A positive carrier norm with a paid **physical diameter** suffices for the local curvature projection on a raw-free, gauge-invariant homogeneous or periodic activity family. A full physical interior-volume weight is not needed for that linear readout. The projection costs the expected inverse native radius squared; the old-grid root density is canceled by four physical spacing powers. This is proved below.

This does **not** yet apply the projection to the complete C05 boundary bank as if that bank were the old-reset difference of the bulk \(E\) action. These are different source objects. The actual all-depth bulk \(E\)-feedback estimate required in [Reset remainders](../../coupling/reset_remainders.md), target (6), remains an input to be proved. The new C05 theorem takes the ordinary \(E\) bank as admitted forcing and does not preserve a reset-dependence mark through its homogeneous recursion.

The AF comparisons used below are conditional comparisons on an already admitted signed prefix. They do not prove that the physical Wilson trajectory satisfies those hypotheses.

## 1. The source quantity being projected

CMP119, printed pp.278–279, constructs the interior \(E^{(k+1)}\) terms from (3.37)–(3.47). Terms whose localization domains lie in the regular interior agree with their whole-lattice counterparts. The remaining terms are assigned to \(B^{(k+1)}\). The coupling subtraction is then taken from the vacuum-subtracted regular \(E^{(k+1)}\), not from an arbitrary sum of boundary scalars on a retained history.

The quadratic curvature coefficient is the gauge-invariant second-order marginal obtained through (3.49)–(3.56), or equivalently by the compatible small-flux readout in the retained coupling analysis. Mature reset contributions may enter the regular \(E\)-producing operation. Once they have done so, later ordinary bulk steps propagate them through the same \(E\) recursion as all other regular fields.

Thus the relevant reset error is a difference such as
\[
 \Delta H_{k+1}
 =
 H_{k+1}(E_{\le k}^{\rm actual},R_{\rm mat};Y_{\le k})
 -
 H_{k+1}(E_{\le k}^{0},0;Y_{\le k}),
 \tag{CP.1}
\]
with the prescribed comparison and its actual own vacuum/Wilson subtractions specified. It is not just the current mature-\(R\) insertion while keeping the incoming \(E\) identical. The direct latter difference is already bounded by (D) in [Reset remainders](../../coupling/reset_remainders.md).

The source's full \(E\) bounds and C05's full boundary bounds separately control the two sides of various identities. Such control does not give a small bound for the history-dependent difference (CP.1).

## 2. A linear projection lemma in the weaker diameter norm

Here is a sufficient readout theorem that separates its genuine hypotheses from the reset-feedback estimate.

Fix a birth scale \(b\) with physical mesh \(h_b\), a later reference scale \(k\) with \(h_k\ge h_b\), and \(r_b>0\), the dimensionless native analytic radius at scale \(b\). Work with the source local dimensionless link coordinates and their fixed strong derivative/current companions. Let
\[
 F_b(U,J)=\sum_{\Gamma\in\mathfrak G_b}F_{b,\Gamma}(U,J)
 \tag{CP.2}
\]
be a raw-free gauge-invariant family with homogeneous or a fixed compatible periodic covariance. Each activity has an actual dependency footprint \(S_\Gamma\). It may contain bounded declared cores, but its whole physical diameter is retained:
\[
 D_\Gamma=1+\frac{\operatorname{diam}S_\Gamma}{h_b}.
 \tag{CP.3}
\]
The fixed \(M\), field stencil and local gauge collar can be incorporated into \(D_\Gamma\) and fixed constants.

Assume the following.

1. **Flat local chart.** The activity is holomorphic and bounded by \(M_\Gamma\) on the genuine source native neighborhood of the flat configuration on its dependency footprint and fixed collar. The local affine Cartan curvature curve used for the source readout is admitted there at dimensionless birth flux
\[
 |f_b|\le \frac{c\,r_b}{D_\Gamma}.
 \tag{CP.4}
\]
The field and gradient pieces satisfy this by the actual affine Cartan potential; its abelian physical current vanishes in the interior. This condition is a source-chart assertion, not a consequence of boundedness around an arbitrary nonflat retained history.

2. **Positive rooted diameter norm.** There is a permitted birth-cell anchor for each activity, chosen on an actual exterior cell or a genuine component slot, with
\[
 \sup_{x\in\mathbb L_b}
 \sum_{\Gamma:\,a(\Gamma)=x}
       e^{\sigma D_\Gamma}M_\Gamma\le A_b.
 \tag{CP.5}
\]
Rooting at every actual incident birth cell is stronger and also suffices. A component slot is resolved by its actual birth cell. Arbitrary hidden fine labels are not counted as new anchors.

3. **Source local thermodynamic compatibility.** The finite-volume coefficients agree with the limiting local coefficients away from the boundary/winding sector, with the same positive bounds. Equivalently, use the infinite-volume local activity family on which the frozen coupling projector is defined. This is the ordinary localization/whole-lattice identification used at CMP119 pp.278–279. No projector on one finite torus is silently substituted for it.

Let \(\mathcal P_k\) be any fixed scalar linear combination of the constant-Cartan-curvature Hessian components per current-scale volume, with the Wilson normalization constants retained. Then
\[
 \boxed{\quad
 |\mathcal P_k F_b|
 \le C_{\sigma}\,r_b^{-2}A_b .
 \quad}
 \tag{CP.6}
\]
The constant depends on the fixed group, tensor projection, source block parameters and \(\sigma\), but not on \(b,k\), the number of activities, the torus volume, or the volumes of the declared cores.

### Proof

Let \(\varphi\) be the dimensionless curvature at scale \(k\). The same physical curvature has birth plaquette flux
\[
 f_b=\left(\frac{h_b}{h_k}\right)^2\varphi.
 \tag{CP.7}
\]
Choose the local Cartan gauge centered in \(S_\Gamma\). The dimensionless potential on that footprint is bounded by \(C|f_b|D_\Gamma\); its first difference is \(O(|f_b|)\), and the abelian current is zero. By (CP.4), the activity is holomorphic on the disc
\[
 |\varphi|\le
 c r_b\left(\frac{h_k}{h_b}\right)^2D_\Gamma^{-1}.
 \tag{CP.8}
\]
Second-order Cauchy gives
\[
 \left|\frac12D_\varphi^2F_{b,\Gamma}(U_\varphi,J_\varphi)
                           \big|_{\varphi=0}\right|
 \le C r_b^{-2}
     \left(\frac{h_b}{h_k}\right)^4D_\Gamma^2 M_\Gamma.
 \tag{CP.9}
\]
The scalar coupling combination changes only a fixed constant.

For a compatible physical torus let \(V_b,V_k\) be its birth/current cell counts. They satisfy
\[
 \frac{V_b}{V_k}=\left(\frac{h_k}{h_b}\right)^4.
 \tag{CP.10}
\]
Since \(\sup_{D\ge1}D^2e^{-\sigma D}<\infty\), (CP.5) bounds the sum of \(D_\Gamma^2M_\Gamma\) by \(C_\sigma A_bV_b\). Divide (CP.9) by \(V_k\) and use (CP.10). This proves (CP.6) before the source thermodynamic local-coefficient limit. The same bound and spare diameter exponential give dominated convergence in that limit; winding contributions are removed with the source localization limit, not with an unproved exchange of flux quantization and derivatives.

Gauge invariance and the raw-free argument list are essential to the use of a different centered local gauge for each activity. The estimate has not filled a core interior with a new activity tree. Only its physical diameter appears in the Cauchy radius. \(\square\)

### Periodic coefficients and divided tensor projections

If the coefficient has a compatible birth-grid period, average the local Hessian over one period before taking the scalar contraction. The same proof applies because (CP.5) is uniform in the root and the average has total weight one. There is no extra period-volume factor.

This statement does not itself prove the fractional periodic cancellation of [Reset remainders](../../coupling/reset_remainders.md) §2. That cancellation concerns the marginal tensor left after its correct subtraction inside a localized transfer. It remains necessary where the iteration requires a small irrelevant gain rather than a bounded final readout.

## 3. Several native grades and creation times

Suppose a sum has source families at grades \(m\), each satisfying the hypotheses of the lemma with radius \(r_m\), and
\[
 \sum_m r_m^{-2}A_m<\infty.
 \tag{CP.11}
\]
Then the projected series is normally convergent and
\[
 \left|\mathcal P_k\sum_mF_m\right|
 \le C\sum_m r_m^{-2}A_m .
 \tag{CP.12}
\]
The cancellation of root density is grade-by-grade. There is no \(L^{4(k-m)}\) left in (CP.12).

A new prefix contribution can have a source grade \(m\) different from its chronological creation event \(r\). It must retain that grade in this readout. If the actual construction gives
\(m\in[r-N_r-C,r+C]\), with \(N_r\) a fixed logarithmic power, the admitted signed-prefix upper slope implies
\[
 Y_m\le Y_r+C N_r+B\le C'Y_r,\qquad
 r_m^{-2}\le C r_r^{-2}(1+\ell_r)^{C'}
 \tag{CP.13}
\]
at one sufficiently large lower ceiling. Here \(Y_j=g_j^{-2}\) and the radius exponents are fixed. One can therefore sum the finitely many true prefix grades at a fixed creation event at the cost of a fixed logarithmic power. This is not permission to replace a fine root by a coarse one before (CP.9)–(CP.10).

The new C05 creation profiles have the form
\[
 f_r\le C Y_r^{u}(1+\log Y_r)^v
                 \exp[-c(\log Y_r)^s],\qquad s>1,
 \tag{CP.14}
\]
with fixed exponents, after its finite fractional powers and norm reserves. If a raw-free homogeneous subfamily satisfies (CP.4)–(CP.5) with total grade contribution at event \(r\) bounded by \(f_r\), then (CP.12) and (CP.13) give its curvature readout with only fixed inverse-coupling/logarithmic losses.

On an already admitted prefix, the lower AF comparison
\[
 Y_r\ge cY_k+a(k-r)
 \tag{CP.15}
\]
makes the readout summable. For every \(N>0\), the function
\(Y^{u+1}(1+\log Y)^{v+C'}e^{-c(\log Y)^s}\)
is bounded by \(C_NY^{-N-2}\) for large \(Y\). Hence
\[
 \sum_{r\le k}r_r^{-2}(1+\ell_r)^{C'} f_r
 \le C_N\sum_{j\ge0}(cY_k+aj)^{-N-2}
 \le C_N'Y_k^{-N-1}.
 \tag{CP.16}
\]
All exponents are fixed before the ceiling. This is a conditional consequence of (CP.15), not a derivation of the physical AF trajectory. It could be used inside a stopped-prefix bootstrap after the actual marked source estimate has been proved.

## 4. Why the C05 bank cannot simply be substituted into the lemma

There are three separate issues.

### 4.1 Different argument and symmetry class

A general C05 activity retains older raw group/adjoint slots and a fixed nonhomogeneous history. Its native analyticity holds on that actual admitted source chart. Simultaneous gauge covariance in the native field and the raw/adjoint arguments does not imply gauge invariance in the native field alone with those arguments held fixed.

The source curvature projector acts on the homogeneous regular \(E\) family. Its local Cartan gauge change is legitimate because that family has no retained old raw argument and the whole-lattice covariance is known. For a general boundary activity, neither a flat chart with the same fixed raw history nor the independent local gauge change used in (CP.8) follows from C05. The C05 local-native jet is a theorem at its admitted real center; it is not automatically a small-flux theorem at a different flat center.

Thus (CP.6) is a bounded projection on an explicitly identified subspace. It is not a map from every C05 history scalar to the physical coupling.

### 4.2 The causal reset label has been lost in the ordinary forcing bank

The new C05 history induction keeps completed/failed relative scalar records and their new responses under exact normalizations. It also invokes the source regular \(E/R\) families as ordinary inputs with their admitted native majorants. In that use, \(E_0\) is a forcing budget. The proof does not bound the derivative of \(E\) with respect to a marker multiplying every earlier mature reset.

A mature reset can change a homogeneous \(E\) birth. At later steps that change has no required surviving large-field owner port. It evolves in the ordinary bulk, so the C05 current-to-large-field collar cannot be assigned to it. The term is not restored to the fresh boundary bank merely because a reset caused it historically.

Consequently C05 does not prove that the difference (CP.1) has a small \(A_m\) in (CP.11). Assigning its two individually bounded \(E_0\) banks a difference bound gives only \(2E_0\); after the readout this costs \(Cr_m^{-2}\), which is insufficient for the B03 remainder.

### 4.3 A conditional AF tail is not a physical trajectory proof

Even if one identifies a small raw-free family, (CP.16) uses exactly the admitted two-sided/signed-prefix comparisons. B03 has to prove that the actual Wilson output continues to satisfy a closed quantitative recurrence. The C05 use of these comparisons cannot be run backwards to establish them.

A stopped-prefix argument may use them up to the first possible exit and estimate one provisional output. That is the appropriate logical order for the synthetic-marker comparison in the reset-remainder reduction.

## 5. The remaining source estimate in an actionable form

Let \(H_j(z)\) be the single-complex-marker family defined in [Reset remainders](../../coupling/reset_remainders.md) §4: keep the numerical \(Y_i\) prescribed, multiply the actual mature reset inputs by \(z\), and use each synthetic \(H_i(z)\) with its own vacuum and Wilson subtraction. The compensating Wilson term keeps the prescribed principal coupling. At \(z=1\) it agrees with the actual bulk construction.

The exact missing positive/analytic input can be stated in either of two forms.

**Native-ball form.** For one common marker disc \(|z|\le A_k\) and all precursor steps, prove the actual raw \(E\) output estimate on an invariant genuine native chart,
\[
 \sup_{x}\sum_{\Gamma:a(\Gamma)=x}
    e^{\sigma D_\Gamma}
    \sup_{\mathcal D^+_{j},\,|z|\le A_k}
               |H_{j,\Gamma}(z)|\le C E_0.
 \tag{CP.17}
\]
The incoming subtractions, the fixed numerical Gaussian/coupling array, the simultaneous source localizer domain and the cutoff are those of the synthetic construction. A signed summed value bound without this source chart is insufficient.

**Marked-difference form.** Prove directly that the transported reset-dependent homogeneous family has
\[
 \sum_m r_m^{-2}A_m^{\rm reset}\le C Y_k^{-1}
 \tag{CP.18}
\]
or the smaller readout error required by the selected coupling coordinate, with actual local flat charts and covariance. This can be obtained from a marker amplification estimate or an actual signed-prefix sensitivity/renewal theorem.

Once (CP.17) is established on \(|z|\le A_k\), the projection lemma and a single marker Cauchy estimate give
\[
 |\mathcal P H_{k+1}(1)-\mathcal P H_{k+1}(0)|
 \le \frac{C r_k^{-2}E_0}{A_k-1},
 \tag{CP.19}
\]
with any fixed source/logarithmic projection loss included explicitly. There is only one inverse native-radius loss in this final readout; it is not multiplied at every age. This recovers the useful implication (6)\(\Rightarrow\)(7) of the reset-remainder reduction with the weaker diameter-norm variant proved above.

The remaining work is therefore not a missing elementary curvature projection bound, and not a demand to charge every fixed core's full interior volume. It is the **uniform marked homogeneous \(E\) transfer on its actual invariant native chart**, including the own Wilson subtractions and prescribed-coupling compensation, or an equivalent direct bound for that same feedback difference. The source analysis of this transfer is given separately in [Homogeneous feedback and the causal Wilson recursion](../../physical_scale/causal_coupling_recursion.md). No B03 or B05 completion follows from this note alone.

# Sources

- Bałaban, CMP **119** (1988), pp.278–283, (3.47)–(3.67): interior-to-whole-lattice identification, coupling subtraction, and the curvature marginal.
- [Positive attachment bounds and the quotient forest](quotient_forests.md) §§18–19, and [Summation at a native root on a two-sided trajectory](native_roots.md): new positive actual-history norm and its retained ordinary-forcing scope.
