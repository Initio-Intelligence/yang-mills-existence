# Real Q-boundary currents and holomorphic integrated defect chains

This note proves the finite-dimensional boundary estimates needed after the exact first-R average. It keeps moving hard cutoffs as real domains. Holomorphy is asserted for an integrated contour functional, not for an indicator. The actual-source input is the first-step starred Q test on independent free bonds, with local comparison minima. A complete raw-supported localization of the surrounding density and reference maps remains a separate input.

## 1. Actual one-slot Q domains in a local reference

Fix the first globally \(P/Q\)-regular geometry and zero-source running parameters \(g,P\), with \(gP\to0\). For one independent nonexceptional bond \(e\), choose a real local reference \(U_{*,e}(V)\). The actual Q tests involving this bond have the form
\[
 \left\|\exp(igu)M_{\ell,e}(V)-1\right\|<2gP,
 \qquad
 M_{\ell,e}(V)=U_{*,e}(V)U_{1,\square_\ell,e}(V)^{-1}.
                                                               \tag{QS.1}
\]
Their intersection defines \(D_e(V)\). The number of tests containing one bond is bounded by a fixed source overlap constant \(J_*\). The entire raw footprint includes the full determining boxes of all displayed local minima and the chosen reference. It is not reduced to the bond's storage block.

For the source's admitted local comparison maps, (1.19) and the variational comparison bound give, after a sufficiently large buffer,
\[
 \|M_{\ell,e}(V)-1\|\le\epsilon_{\rm ref}gP,
 \qquad \epsilon_{\rm ref}\le1/10.                  \tag{QS.2}
\]
All statements below hold on real retained paths along which this same bound holds. The group norm may be the source operator norm or a fixed unitarily invariant matrix norm; the finite-dimensional constants change with its convention.

On the principal logarithm chart, for sufficiently small \(gP\),
\[
 B_{3P/2}\subset D_e(V)\subset B_{3P}.               \tag{QS.3}
\]
Repeated starred tests cause no coupling between different independent free coordinates: the whole Q domain is the product of these one-slot intersections. The nonlinear constraint correction acts only on the excluded exceptional bonds.

## 2. A real finite-difference shell bound

Let \(V,V'\) be two real retained inputs on the same chart and put
\[
 \eta_{\ell,e}=\|M_{\ell,e}(V')-M_{\ell,e}(V)\|.
\]
The group norm triangle inequality implies
\[
 \mathbf1_{D_e(V')}(u)-\mathbf1_{D_e(V)}(u)\ne0
 \ \Longrightarrow\
 \left|\|\exp(igu)M_{\ell,e}(V)-1\|-2gP\right|
           \le\eta_{\ell,e}                         \tag{QS.4}
\]
for at least one \(\ell\). With (QS.2), every point of this symmetric difference lies in
\[
 cP\le|u|\le CP                                     \tag{QS.5}
\]
for fixed positive constants, and more specifically inside the fixed \(3P\) buffer after harmless enlargement.

### Lemma QS.1 — shell volume and perimeter

Uniformly under (QS.2),
\[
 |D_e(V')\triangle D_e(V)|
 \le C P^{d_G-1}\sum_{\ell=1}^{J_*}\eta_{\ell,e}/g, \qquad
 \operatorname{Per}(D_e(V))\le CP^{d_G-1},           \tag{QS.6}
\]
where \(d_G=\dim G\) and the volume/perimeter are in the fixed real Lie-algebra coordinates.

**Proof.** Haar measure is invariant under the multiplication by \(M_{\ell,e}\). In a fixed small logarithm chart, its density relative to Lie-algebra Lebesgue measure is bounded above and below, and the map \(u\mapsto\exp(igu)\) contributes \(g^{d_G}\). A group-norm annulus at radius \(2gP\), of thickness \(\eta\), has Haar volume at most \(C(gP)^{d_G-1}\eta\). Pulling it back gives the first bound for one test, and the union bound gives (QS.6).

For clarity, the annulus assertion needs no smooth operator-norm sphere. Use norm-polar coordinates in the Lie algebra. Along each ray, the small-group norm of \(\exp(i rH)-1\) is increasing with a radial derivative bounded above and below by fixed multiples of \(\|H\|\), while \(r\|H\|\) stays small. For the operator norm this follows directly from \(2\sin(r\|H\|/2)\); for a fixed unitarily invariant norm it follows from the singular values \(2|\sin(r\lambda_j(H)/2)|\). Thus the radial interval corresponding to thickness \(\eta\) has length \(O(\eta)\), and the radius is \(O(gP)\). The finite cone measure of the norm sphere proves the volume bound. The same small-chart bi-Lipschitz change of variables bounds each boundary perimeter by \(CP^{d_G-1}\). The boundary of a finite intersection is contained, up to its measure-theoretic exceptional set, in the union of these boundaries. This proves the second estimate, including corners. ∎

If \(V'=V_t\) is one normalized elementary displacement, define the actual radius velocity
\[
 v_{e,d}=\sum_\ell\sup_{0<|t|\le1}
       \frac{\|M_{\ell,e}(V_t)-M_{\ell,e}(V)\|}{g|t|}. \tag{QS.7}
\]
Then (QS.6) is a genuine \(O(|t|v_{e,d})\) bound. The velocity requires the actual variational response of the local maps. At this first step their admitted local analytic/response estimates give at worst a fixed polynomial in \(R_1,P\), and their raw parameter directions lie in their declared determining boxes. No derivative in a physical link direction is obtained by dividing a bare \(O(1)\) value estimate by \(g\).

## 3. Complete native comparison laws have a tail surface density

Let \(\mu_B\) be any complete first-step product comparison law in AS.11, with a \(3P\) radius at the selected slot. It has its actual zero-source K, full W, and normalizer. The other coordinates are integrated; they are not pinned at an atypical retained array. The same statements hold under a sufficiently small quadratic tilt in any finite coordinate set.

Write \(p_e(u)\) for its one-slot marginal Lebesgue density in the interior of the \(3P\) ball. Then
\[
 p_e(u)\le C e^{-c|u|^2},\qquad
 |u|\le(5/2)P                                      \tag{QS.8}
\]
after changing fixed constants; the bound also holds on any fixed shell strictly inside the \(3P\) comparison ball.

**Proof.** Strong log-concavity of the full law passes to its marginal: subtract a fixed positive quadratic in \(u\) from the potential and apply convex marginalization, or use convex barriers. Its effective potential \(H_e=-\log p_e\) has Hessian bounded below by a fixed positive matrix. On interior points the exact score formula also gives
\[
 \nabla^2H_e
   =\mathbb E[\nabla_e^2 V_{\rm full}\mid u]
       -\operatorname{Cov}(\nabla_eV_{\rm full}\mid u)
   \le C I.                                       \tag{QS.9}
\]
The upper bound comes from the actual K diagonal and W Hessian row, with any small tilt included. AS.1 bounds the one-slot mean by a fixed constant. Here is a boundary-compatible proof that its mode \(u_*\) is also bounded. On the convex ball, the variational inequality gives \((u-u_*)\cdot\nabla H_e(u_*)\ge0\), including a possible boundary mode. The radial integration-by-parts boundary term has nonnegative outward sign, so
\[
 \mathbb E[(u-u_*)\cdot\nabla H_e(u)]\le d_G.
\]
The lower Hessian bound then implies \(\mathbb E|u-u_*|^2\le d_G/\lambda\). Convex-barrier approximation gives the same assertion without a smooth norm boundary. Thus \(|u_*|\le |\mathbb Eu|+\sqrt{d_G/\lambda}\), a fixed bound. A unit ball around that mode lies inside the \(3P\) domain for large P. The Hessian upper bound and normalization bound the density at its mode by a fixed constant. The lower Hessian bound then gives (QS.8). All comparison normalizers are retained. ∎

Combining (QS.6),(QS.8),
\[
 \int |\mathbf1_{D_e(V_t)}-\mathbf1_{D_e(V)}|
            p_e(u)\,du
 \le C|t|v_{e,d}\,P^{d_G-1}e^{-cP^2}.              \tag{QS.10}
\]
The polynomial can be absorbed by reducing \(c\). This is a finite-difference estimate, not a claim that the difference quotients converge in total variation to a surface measure. They may converge only weakly; the finite-current envelope is what is controlled.

For a prescribed actual R pattern one can retain its rarity by using the energy tilt in AS.17 before this marginal bound. Its event supplies \(E_D\ge c_*kP^2\); the tilted one-slot marginal still satisfies (QS.8), and the same partition function comparison is used. This proves the corresponding joint-mass boundary estimate with one conserved exponential reserve. Other hard selectors can be bounded by one for this absolute estimate. It does not permit treating their distributional derivatives as ordinary functions.

## 4. The exact holomorphic defect functional

The following lemma addresses complex decoupling of the density while the Q domains remain real.

Let \(D=D_e(V)\) for a fixed real V. Suppose \(F_s(u)\), depending holomorphically on decouplers s and on u in a complex neighborhood of \(\{|u|\le3P+2\}\), obeys
\[
 |F_s(u)-u|\le1,\qquad \|D_uF_s\|\le C             \tag{QS.11}
\]
uniformly on the prescribed decoupler polydisc. In the actual first chart the candidate is
\[
 F_{e,s}(u)=\frac1{ig}
  \operatorname{Log}\!\left(
    e^{igu}U_{*,e}(V)U_{1,e}(s;V)^{-1}\right).      \tag{QS.12}
\]
It depends only on its own free integration coordinate u. At the physical endpoint \(s=1\), it is the exact change from the local free-link frame to the original global-minimum frame.

For a holomorphic top-degree integrand \(\omega_s(z)=\Phi_s(z)\,dz_1\wedge\cdots\wedge dz_{d_G}\), define
\[
 \mathfrak D_{e,s}(\Phi_s)
 =\int_D\Phi_s(F_s(u))\det D_uF_s\,du
      -\int_{B_P}\Phi_s(z)\,dz.                    \tag{QS.13}
\]
Both terms are exact. No change is made to the source normalizer or the other factors inside \(\Phi_s\).

### Lemma QS.2 — annulus plus boundary chain

Let \(H_t(u)=u+t(F_s(u)-u)\). Then
\[
 \mathfrak D_{e,s}(\Phi_s)
 =\int_{D\setminus B_P}\Phi_s(u)\,du
   +\int_{[0,1]\times\partial D}H^*\omega_s,         \tag{QS.14}
\]
with the boundary orientation fixed by the homotopy formula. Each term is holomorphic in s. The first term has \(|u|\ge P\); on the second,
\[
 |\operatorname{Re}H_t(u)|\ge3P/2-1,\qquad
 |\operatorname{Im}H_t(u)|\le1.                    \tag{QS.15}
\]
The absolute chain Jacobian is at most a fixed constant times
\(|F_s(u)-u|\); its total parameter mass is at most \(CP^{d_G-1}\).

**Proof.** A holomorphic top form is closed. Apply the homotopy/Stokes identity between the real domain and its image under \(F_s\), and then subtract the integral over \(B_P\subset D\). The formula remains valid for the finite-perimeter intersection domain, by approximation or the pushforward current version of Gauss–Green. Its boundary mass is bounded by Lemma QS.1. Equation (QS.11) controls the homotopy and the determinant minors. The bounds in (QS.15) follow from (QS.3). Holomorphy follows by dominated integration on these fixed real parameter domains. It is not holomorphy of \(\mathbf1_D(F_s^{-1}z)\). ∎

For several distinct defect slots, use one such functional per slot. Their maps depend on disjoint integration coordinates, so their product is exact. Each slot contributes an annulus term or a boundary chain. There are at most \(2^n\) choices for n slots and no additional \(n!\). All Jacobians stay in the integrand.

## 5. Gaussian reserve on the product chains

Use the exact relative Gaussian marginal construction GM.16–GM.21, not only an abstract complex gap. Let \(p_s\) be its complex density, \(p_0\) its positive centered reference density, and \(u_m\to0\) the fixed-buffer covariance discrepancy in GM.17. For points \(z=x+iy\) on the product chains, y is supported on the n boundary-chain slots and \(|y|^2\le Cn\). The explicit quadratic formula and the relative determinant bound give
\[
 |p_s(x+iy)|
 \le \exp\{C u_m r_I+C u_m|x|^2+C|y|^2\}\,p_0(x).
                                                               \tag{QS.16}
\]
Indeed the imaginary part of the precision is \(O(u_m)\), because the reference precision is real. Its mixed x/y term is bounded by \(C u_m(|x|^2+|y|^2)\); the real y-square term has a fixed coefficient and costs only \(Cn\). More generally Young's inequality allows an arbitrarily small additional real tilt \(\delta|x|^2\), at the price of \(C_\delta n\). There is no new fixed \(C^{r_I}\) comparison constant.

Combine (QS.16) with the ordinary/root majorant \(a_I e^{b|z|^2}\), with b chosen within the spare reserve, and pay any distinct fixed failed-P slots by a small exponential Markov tilt. The positive real Gaussian after these tilts still has uniformly bounded covariance above and below. Its exact normalization costs \(e^{\eta r_I}\), where \(\eta>0\) can be chosen as small as required by first fixing b, the Markov tilt and any Young parameter, then enlarging the fixed marginal buffer. This order is independent of g and the total volume.

Integrate all ordinary real coordinates exactly. Only the marginal on the n defect slots remains, and it has density bounded by
\[
 C^n\exp\{-c\sum_{e\in S}|x_e|^2\}.
\]
Thus the fixed per-coordinate density constant is paid only on the defect set. Every annulus coordinate has norm at least P. Every boundary-chain coordinate has real norm at least \(3P/2-1\); its original parameter mass is bounded by (QS.6) and the homotopy Jacobian. Consequently the full estimate is
\[
 a_I e^{\eta r_I}
       \bigl(CP^{c_G}e^{-cP^2}\bigr)^n
 \le a_I e^{\eta r_I}e^{-c'P^2n},                  \tag{QS.17}
\]
with the usual additional failed-P factor on distinct slots. The small rank loss \(\eta r_I\) is paid from the existing strict primitive carrier margin. Defect-only constants, surface powers and logarithmic-halo volumes are paid by the defect reserve. An uncontrolled \(e^{C r_I}\) would not be a sufficient input for this conclusion and is not used.

Polynomial roots and fixed first currents consume a fixed further part of the same positive reserve. Source derivatives have their usual factorial bound from that one reserve; they do not change the domain or saddle.

This estimate concerns **integrated defects**. It avoids the false assertion that a hard moving Q indicator is holomorphic in the Gaussian decouplers.

## 6. Exact finite raw-current separation

For a real change \(V\to V_t\), compare (QS.13) in two pieces.

1. Keep the real domain D fixed while changing the integrand, reference map and Jacobian. Apply the exact chain identity to this whole difference. The annulus and boundary-chain localization retains its tail. Ordinary native coefficient/current bounds then estimate these smooth factors.
2. Keep the chosen endpoint integrand and map fixed while changing D. The difference is the signed integral on \(D(V_t)\triangle D(V)\). Lemma QS.1 gives its exact thickness bound, and its support lies at norm \(cP\). The Gaussian or complete-product marginal estimate gives (QS.10) and its reserve-weighted form.

This separation never differentiates a nonsmooth intersection boundary twice or treats its corners as smooth. It applies directly to divided finite differences with both endpoints and the path in the admitted real chart. Both pieces are in the new kernel-current record in the physical pushforward filing. Existing incoming direct/current records are transported separately.

The true raw footprint of the domain piece contains every local reference determining box in (QS.1). Its summed native direction cost is bounded by
\[
 C P^{c_G}e^{-cP^2}
       \sum_d v_{e,d}.                              \tag{QS.18}
\]
Once the actual local variational response gives a fixed polynomial bound for the last sum, the full \(R_1^4\)-sized footprint and direction count are paid by the source \(p_0\ge5r\) hierarchy. This is a density-boundary estimate; it does not on its own normalize a whole many-defect series.

## 7. Buffer choice must preserve a fixed carrier rate

To verify (QS.11), the unmarked reference construction must make the localized global minimum and the raw-local reference differ by at most \(cg\), uniformly on the decoupler polydisc. A primitive bound of the form
\[
 P^a\!\sum_{X:\,X\not\subset D}|c_X|e^{\nu|X|}
 \quad\hbox{with an exterior-distance tail}\quad
 CP^a e^{-\nu' \ell}
\]
is paid by an initial buffer \(\ell(P)=C_a\log P\).

The **outside decoupling grid must remain fixed**. If its cube side itself grew like \(\log P\), a fixed Cauchy factor per outside cube would not pay a fixed exponential physical-volume rate. Instead enlarge only the initial defect/reference set by \(\ell(P)\). Keep the fixed outside grid and its fixed polydisc. Every exterior carrier then has length at least \(\ell(P)\), while its outside-parameter count is still controlled by its physical carrier size with the original fixed constants. The mean tail is \(O(1)\), the outside carrier rate is unchanged, and the enlarged initial volume is paid by (QS.17).

The growing enlargement is charged only to the Q-defect species. If \(I_{\rm reg}\) is the union of ordinary Mayer and marked-root supports and \(S_Q\) the set of Q-defect slots, use the additive rule
\[
 D=D_m(I_{\rm reg})\ \cup\!
       \bigcup_{e\in S_Q}D_{\ell(P)}(Q\operatorname{foot}_e),
 \qquad
 |D|\le C m^4|I_{\rm reg}|
              +C|S_Q|(R_1+\ell(P)+m)^4.            \tag{QS.19}
\]
Here \(m\) is fixed, and every enlargement includes its fixed lift/gauge collar and is rounded to the same fixed outside grid. A logarithmic halo around every ordinary root or long unmarked carrier would cost \(\exp[C\kappa(\log P)^4|I_{\rm reg}|]\), which a fixed primitive carrier rate cannot pay. Formula (QS.19) avoids that loss. Since enlargement commutes with unions, it also preserves the required component construction.

For an R-sized raw Q box the growing enlargement costs at most \(C(R_1+\log P+m)^4\); a union of n such boxes costs their summed volumes. This is \(o(nP^2)\) in the source hierarchy. Exact restriction consistency and component factorization must hold for the chosen local reference family. A pointwise real decay estimate alone does not establish them.

## 8. Exact application boundary

The real shell estimate, the complete-product marginal tail and the integrated homotopy identities are proved above. The actual first-step starred-Q structure supplies the one-slot domains and their local comparison footprints.

A completed first-step carrier theorem still needs the source-verified simultaneous construction of the localized density and the \(U_1(s;V)\) entering (QS.12), with its restriction-consistent local reference, fixed-grid tail bound and full current certificate. The source gauge/coarea factors must stay inside the same holomorphic integrand. Smooth fluctuation cutoffs used to define Mayer vertices must be chosen coordinatewise and identically one on the complex tube traversed by each defect coordinate; one cannot analytically continue a smooth cutoff through the contour.

No exterior P-bad sector, inherited completed density or arbitrary history is treated here. The construction is specifically a possible analytic completion of the exact first-R average, not a replacement of the original Wilson measure.
