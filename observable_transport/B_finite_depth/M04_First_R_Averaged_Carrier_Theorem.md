# The first R-averaged scalar: a positive ambient kernel and a full carrier estimate


## 1. The operation that is established

Fix the first ordinary Wilson step, its literal running parameters, and the globally P/Q-regular geometry \(\Omega _1\) equal to the full lattice. Sum **all** first R histories before normalization, and integrate their retained bad free coordinates against their actual joint masses. Undo every relocation and the complete source integration identities. The result is exactly

\[
 \overline Q_RF(V)
 =\frac{\int\chi_Q(z,V)D_V(z)F(\Phi_V(z))\,dz}
        {\int\chi_Q(z,V)D_V(z)\,dz}.
 \tag{RA.1}
\]

All first coarea, averaged soft-gauge, Haar, constraint, and action factors remain in \(D_V\). The equality is AS.6–AS.7 for the gauge-invariant microscopic marks treated here. The field \(\Phi_V(z)\) is in the source's post-gauge-insertion coordinates. For a general observable of the pre-insertion link state, the exact gauge preimage described below is also integrated. The identity is a mass-weighted average, not an unweighted average of normalized history outputs. The source-independent coarse weight outside this ratio is retained in the actual coarse density.

The native theorem QC.3 proves that the actual moving-Q operation (RA.1) differs from the all-R-good fixed-P operation by an exponentially small connected physical-carrier correction, with separate continuous coarse currents. Its native-domain statement alone did not provide a common kernel on every compact retained datum. This note supplies that extension and the resulting fixed-basis scalar extraction.

This changes the intermediate operation from retaining a particular R geometry to averaging it. It does not prove the contradicted original fixed-history norm, nor does it establish the complementary P/Q branches or later completed histories. ## 2. One compatible extended density and reconstruction

Choose the first-step source-independent positive Gram precision and complete interaction extensions from GM.28, now on the fixed enlarged free-coordinate domain required in QC.6. Write

\[
 d\mu_V(z)=d\mu_{C^{\rm ext}(V)}(z),\qquad
 K^{\rm ext}=\sigma I+(B^{\rm ext})^{\mathsf T}B^{\rm ext},
 \tag{RA.2}
\]

with its uniform positive gap, common restricted marginal family, and complete supported interaction \(W^{\rm ext}_V\). Its local retained guards and their derivatives are included. On active data it is the native first-step normal form. Outside that support it is a stated source-free extension; it is not obtained by substituting a nonstationary field into the Wilson action and dropping a force.

Choose the compact Hermitian reconstruction consistently with the minimum family used in the ambient frame analysis. This choice can be made explicitly. Let \(\Theta_{\rm bg}^{\rm ext}\) be that analysis's fixed, force-resolved common first-step background family. In the existing reconstruction family, subtract its zero-fluctuation coefficient before extending the fluctuation part, and put

\[
 \Theta_{\chi}^{\rm ext}(z,V)
 =\Theta_{\rm bg}^{\rm ext}(V)
       +\sum_X\eta_X(V)
          [\Theta_{\chi,X}(z,V)-\Theta_{\chi,X}(0,V)],
\]
\[
 \chi^{\rm ext}_e(z,V)
       =e^{i\Theta_{\chi,e}^{\rm ext}(z,V)}(Q^fV)_e.
 \tag{RA.3}
\]

Use the fixed common background coefficient choice everywhere thereafter. Equation (RA.3) is real compact, agrees with the original reconstruction on native data, and satisfies
\(\chi^{\rm ext}(0,V)=U_1^{\rm ext}(V)\) on all real data. The force-resolved background iteration has at least one local force factor in every nonzero term; the remaining nonlinear factors are uniformly small. It therefore preserves the local-energy budget (4.11), after the usual strict carrier-rate loss. The zero-subtracted fluctuation family has the original O(gz) and derivative bounds. Their sum consequently has the GM.31–GM.33 scalar root budgets, including its exact compact Wilson trace and its genuine old-link difference records. No observable is extended after integration.

The positive source-free free-coordinate law used for every mark will be

\[
 q_Q^{\rm ext}(dz\mid V)
 =\frac{\prod_e\rho_e^{\rm ext}(z_e,V)\,
             e^{W^{\rm ext}_V(z)}d\mu_V(z)}
        {\mu_V[\prod_e\rho_e^{\rm ext}e^{W^{\rm ext}_V}]},
 \tag{RA.4}
\]

For the post-gauge-insertion old state, the kernel is its pushforward by the one map (RA.3). If the old state is the original link configuration before the normalized Faddeev–Popov insertion, retain its exact center-fixed gauge preimage as well:

\[
 \widetilde q_Q^{\rm ext}(dz,du\mid V)
       =q_Q^{\rm ext}(dz\mid V)\,dH_0(u),\qquad
 \widetilde\chi^{\rm ext}(z,V,u)
       =\chi^{\rm ext}(z,V)^{u^{-1}}.
 \tag{RA.4a}
\]

Here \(dH_0\) is the normalized product Haar law of the source's center-fixed block gauge variables. The normalized insertion followed by the source change of variables makes this preimage factor independent of the post-insertion coordinates; it is not an extra gauge-fixing determinant. The block gauge preserves the coarse readout. It also preserves every gauge-invariant scalar mark used in this theorem, so all estimates below are identical in these two explicitly specified presentations. For arbitrary pre-insertion marks and their products, use (RA.4a), rather than invoking scalar gauge invariance to omit a map.

Products, constants and microscopic observables in the chosen presentation therefore use one common law and reconstruction. The comparison law \(q_P^{\rm ext}\), and its gauge-preimage version when needed, has exactly the same density and reconstruction, with every \(\rho_e^{\rm ext}\) replaced by \(\mathbf1_{B_P}\).

## 3. The actual local comparison needed off the active support

The separate [moving q ambient frame extension](moving_q_ambient_frame_extension.md) proves the following first-step input, with a fixed small geometric ceiling \(\gamma\).

For each literal source Q box choose a smooth guard \(\eta_\square(V)\), equal one below a local \(\gamma/8\) ceiling and supported inside a \(\gamma/4\) ceiling. Its entire raw footprint is the original determining box plus a fixed primitive halo. On its support the literal \(U_{1,\square}(V)\) is defined in a larger native tube, and

\[
 \|\Log(U_{1,e}^{\rm ext}U_{1,\square,e}^{-1})\|
       \le C\gamma e^{-\nu R_1}.
 \tag{RA.5}
\]

This holds even when all far retained data are arbitrary compact fields. The normalized summed derivative is \(Cg e^{-\nu'R_1}\).

The proof has two explicit ingredients. The first bare-step constraint solve is finite range, and its local Euler equation has the gapped local-lift precision, a small local force and a quadratic analytic nonlinearity. Common primitive inverse and Picard coefficients agree wherever their full carriers cannot see a boundary difference. The source's first-layer bond-complement convention keeps the exceptional variable for each incident coarse constraint available.

There is also a boundary-independent comparison. Restrict the global **independent coordinates** in a buffered inner window and solve the actual constrained Euler system there. This gives an auxiliary constrained field, whose coefficient family agrees with the global family in the common interior. Compare that field to the actual local Q minimum only in a smaller common interior. Their coordinate difference satisfies a finite-range mean-value Hessian equation with a uniform gap and O(\(\gamma\)) boundary data. The massive Dirichlet inverse gives exponential interior decay. Both fields satisfy the exact nonlinear constraints in this comparison; no Euler equation is applied to a clipped link logarithm with an uncorrected constraint defect. The same averaged block gauge is used on the common interior. The full argument and source incidence check are in the companion input proof.

The ambient global coefficient budget is O(\(\gamma\)), not O(gP). Consequently a local-frame displacement initially has the bound

\[
 g^{-1}\|\Log(U_1^{\rm ext}(s)(U_1^{D,\rm ext})^{-1})\|
       \le C(\gamma/g)e^{-cR_1}.
 \tag{RA.6}
\]

The actual source has \(R_1\asymp(\log g^{-2})^r\), \(r\ge2\), so

\[
 (\gamma/g)e^{-cR_1}\longrightarrow0.
 \tag{RA.7}
\]

The full Q defining box supplies the buffer; an additional initial halo of O(\(\log(1/g)\)) is still O(\(R_1\)) if needed. Only Q defects pay it. The outside grid remains fixed. The full initial volume remains O(\(R_1^4\)) per defect and is paid by \(e^{-cP^2}\), since \(P^2/R_1^4\to\infty\).

## 4. The positive cutoff and all of its guard currents

Use the explicit cutoff

\[
 \rho_e^{\rm ext}(z,V)=\mathbf1_{B_{3P}}(z)
 \prod_{\square\ni e}
 \left[1-\eta_\square(V)+\eta_\square(V)
  \mathbf1_{\{\|e^{igz}U_{1,e}^{\rm ext}
                U_{1,\square,e}^{-1}-I\|<2gP\}}\right].
 \tag{RA.8}
\]

A guarded local minimum is evaluated only on the guard's supported native neighborhood. The product is defined by zero extension of its guarded terms elsewhere; the guard support has a fixed buffer inside that neighborhood. Thus no global admission switch is present.

For every real compact V,

\[
 0\le\rho_e^{\rm ext}\le1,\quad
 \rho_e^{\rm ext}=1\text{ on }B_{3P/2},\quad
 \rho_e^{\rm ext}=0\text{ outside }B_{3P}.
 \tag{RA.9}
\]

The law (RA.4) is therefore positive and has a nonzero real normalizer on every retained configuration. On the actual source domain all guards are one, \(U_1^{\rm ext}=U_1\), and the outer \(3P\) cutoff is redundant. Hence (RA.4)–(RA.3) equal the exact R-averaged kernel in post-gauge-insertion coordinates. With (RA.4a) retained, the equality is also an equality of kernels for every pre-insertion mark and product. Formula (RA.1) is its gauge-invariant scalar readout.

For one slot, expand the bounded finite product over subsets J of the tests. Set

\[
 w_J(V)=\prod_{\square\in J}\eta_\square(V)
          \prod_{\square\notin J}(1-\eta_\square(V)),
 \qquad\sum_Jw_J=1.
 \tag{RA.10}
\]

For nonempty J let \(\rho_{e,J}\) be the selected intersection. On the support of its weight it lies between \(B_{3P/2}\) and \(B_{5P/2}\), so the outer \(3P\) cutoff can be omitted. For empty J set \(\rho_{e,\varnothing}=\mathbf1_{B_{3P}}\). The exact defect identity is

\[
 \rho_e^{\rm ext}-\mathbf1_{B_P}
       =\sum_J w_J
              (\rho_{e,J}-\mathbf1_{B_P}).
 \tag{RA.11}
\]

Every summand is a cutoff defect. In particular, a derivative of a guard is taken in (RA.11), so it still multiplies a defect outside \(B_P\). Estimating derivative terms before this identity and discarding \(\sum_JD w_J=0\) would lose the tail and would be invalid.

For nonempty J use the exact local-frame integral and annulus/boundary chain of QC.1–QC.2. Its domain is fixed in the outside parameters, and its displacement is controlled by (RA.6). For empty J use the fixed real annulus \(B_{3P}\setminus B_P\), with no frame transformation. The number of alternatives per slot is fixed. The domains, the weights and all their raw derivatives carry **all** original reference boxes in that slot, including boxes entering a factor \(1-\eta_\square\). These full footprints must not be reduced to the selected subfamily J.

The mixed enlargement and component construction of QC.7–QC.25 therefore apply unchanged. Guard derivative counts are at most a polynomial in the Q footprint, with normalized size O(g/\(\gamma\)) per affected local test. Domain changes are the real shells of QS.1. Every such loss is paid from the same defect tail. All complete Gaussian and interaction currents are those of the single law (RA.4).

## 5. Ambient scalar and separate-current theorem

Let \(\mathbf Q_Q^{\rm ext}\) and \(\mathbf Q_P^{\rm ext}\) denote the decorated scalar transports in the canonical two-copy presentation. Keep the same individual source/localization tags in their difference. Write \(\|\cdot\|_{h',\kappa}^{\rm cont}\) for the full physical-carrier norm with value and separate direct/kernel continuous records, with suprema over the entire real compact retained product and the native shifted local-energy regulators. Here \(h'=Lh\); this fixed geometry has no remaining R-history coordinates.

### Theorem RA.1 — first averaged operation on the full compact product

For the primitive microscopic scalar

\[
 F_h=\alpha\beta_0\sigma_h-c,\qquad
 b=|\alpha|+h^4|c|,
 \tag{RA.12}
\]

and the stated comparable first-step couplings, the explicit common extension (RA.2)–(RA.8) satisfies

\[
 \boxed{\quad
 \|\mathbf Q_Q^{\rm ext}F_h-\mathbf Q_P^{\rm ext}F_h
                \|_{h',\kappa}^{\rm cont}
       \le C L^4 b\,e^{-cP^2}.
 \quad}
 \tag{RA.13}
\]

The constants and positive rate are uniform in volume and sufficiently small g. The estimate is before cancellation among different tags and bounds the two canonical current pieces separately. On active data \(Q_Q^{\rm ext}\) is the exact R-averaged original operation.

**Proof.** The extended Gram/interaction/reconstruction inputs have the same uniform positive reserve and root budgets as GM.4. Equations (RA.5)–(RA.11) supply the only missing ambient inputs to QC.3. The exact finite expansion has the same regular and fixed failed-P registry for the two laws, and every source-containing logarithmic difference has a root and at least one new defect. The positive Gaussian marginal comparison costs a tunably small amount times local rank; fixed constants and boundary-area factors are charged only to the defect slots. The exponential tail pays their entire O(\(R_1^4\)) raw footprint, guard counts and initial halos. Fixed-grid outside localization gives a positive physical carrier rate independent of g. The full common kernel is used before normalization, and the connected logarithm supplies the exact normalized derivative.

For currents, differentiate or take divided differences of the same two-copy tag integrals. Insertion-copy motion is the exact reconstruction pullback. Density-copy motion includes the covariance, complete interaction, normalizer, local-frame coordinate map, sharp-domain shells and guard products. In particular, the coordinate motion induced by a varying Q frame is part of the density-copy current when the insertion copy is fixed. Each record has the QC.32 majorant, so their sum reproduces the exact finite difference tag by tag. Global compact-link energy comparisons give the same shifted regulators on all elementary unit paths. This proves (RA.13). ∎

Adding the first-clean GM.4 estimate gives

\[
 \|\mathbf Q_Q^{\rm ext}F_h\|_{h',\kappa}^{\rm cont}
       \le C L^4 b.
 \tag{RA.14}
\]

A primitive physical-pushforward presentation may file both newly proved contributions in its new kernel current and set its new direct coarse record to zero. That is a separate presentation for this primitive mark; it does not move inherited old B/J records or identify them termwise with the canonical filing.

## 6. Fixed-basis scalar and identity extraction

First use the energy-normalized coordinate \(\varphi_{h'}=\beta_1\sigma_{h'}\) of the F01 scalar direction, with the same all-identity and normalized one-link pulse extraction as GM.38. This is a coordinate for the calculation; the unchanged incoming normalization is restored explicitly below. The probe regulators are uniformly bounded, and their small-field values lie in the actual native domain at sufficiently small g. Extraction is a bounded linear operation on the supported tagged values, and its scalar finite-difference subtraction is assigned to the direct record as in GM.38–GM.39.

Consequently

\[
 Q_Q^{\rm ext}F_h
      =a_Q\varphi_{h'}+c_Q\mathbf1+\mathcal R_Q,
 \tag{RA.15}
\]

where \(a_Q,c_Q\) are field-independent numbers, and

\[
 |a_Q|+h'^4|c_Q|+\|\boldsymbol{\mathcal R}_Q\|_{h',\kappa}^{\rm cont}
       \le C L^4 b.
 \tag{RA.16}
\]

If \(a_P,c_P,\mathcal R_P\) are extracted from the fixed-P comparison law with the same probes and tags, then

\[
 |a_Q-a_P|+h'^4|c_Q-c_P|
   +\|\boldsymbol{\mathcal R}_Q-
             \boldsymbol{\mathcal R}_P\|_{h',\kappa}^{\rm cont}
       \le C L^4 b\,e^{-cP^2}.
 \tag{RA.17}
\]

The displayed \(a_Q,a_P\) are energy-coordinate coefficients, not functions of the retained field. If the fixed incoming normalization is \(z_S^{\rm in}\ne0\), retain the exact conversion of GM.40/LC.54:

\[
 a_Q\beta_1\sigma_{h'}
   =\widetilde a_Q\,z_S^{\rm in}\sigma_{h'},
 \qquad \widetilde a_Q=a_Q\frac{\beta_1}{z_S^{\rm in}},
 \tag{RA.17a}
\]

\[
 |\widetilde a_Q|\le CL^4b\frac{\beta_1}{|z_S^{\rm in}|},
 \qquad
 |\widetilde a_Q-\widetilde a_P|
   \le CL^4b\frac{\beta_1}{|z_S^{\rm in}|}e^{-cP^2}.
 \tag{RA.17b}
\]

When the given incoming centering/energy reserve supplies
\(b\le C|z_S^{\rm in}|/\beta_0\), the first bound is
\(CL^4\beta_1/\beta_0\), with the same rare factor in the difference.
Without that input reserve the explicit ratio in (RA.17b) is retained.
For a centered fixed basis \(z_S^{\rm in}(\sigma_{h'}-m_{\rm in})\),
the corresponding identity coefficient is
\(\widetilde c_Q=c_Q+a_Q\beta_1m_{\rm in}\); its bound keeps this
given centering factor, or uses its stated reserve. A zero scalar
input is the constant case and requires no division. The remainder
and its current filing are unchanged by this exact re-expression.
No final running normalization is assumed or adjusted to hide a
response term.

## 7. An actual small correction to the coarse density

The same construction at zero marked source gives an exact source-free logarithmic ratio

\[
 \delta E(V)=\log\frac{Z_Q^{\rm ext}(V;0)}
                         {Z_P^{\rm ext}(V;0)}
             =\sum_X\delta E_X(V_X),
 \tag{RA.18}
\]

with connected physical carriers. Its norm is anchored:

\[
 \sup_b\sum_{X\ni b}e^{\kappa(|X|+\mathsf t(X))}
  \left[\sup_V|\delta E_X(V)|+
   \sup_V\sum_d\sup_{0<|t|\le1}
             |\delta_{d,t}\delta E_X(V)|\right]
       \le C e^{-cP^2}.
 \tag{RA.19}
\]

An ordinary fixed loss of carrier rate pays the incidence/direction factors. The whole vacuum sum \(\delta E\) may be proportional to volume. Equation (RA.19), not a volume-independent bound on that whole sum, is the statement proved by the source-free connected cluster argument.

On actual active data this gives the exact identity of coarse densities

\[
 C_0(V)Z_Q(V;0)=C_0(V)Z_P(V;0)e^{\delta E(V)}.
 \tag{RA.20}
\]

Any Gaussian normalization factor moved between the displayed \(C_0\) and Z is kept consistently on both sides. Thus the first R average supplies an actual, supported, small unmarked correction to the regular coarse density. It also supplies the marked first derivative and its fixed-basis extraction above. This is stronger than a bound on one selected scalar value.

Equation (RA.20) is a viable new first-step operation on this P/Q-regular branch. It does not license continuing the old history-dependent future kernels after forgetting R. A continuation must use the resulting coarse density and its corresponding marked source density, or retain the exact posterior information required by future kernels. Likewise \(\log\int dV\,C_0 Z_Q(t)\) is the full outer generating function; averaging the conditional logarithm is not a substitute for it.

## 8. What remains before an existence proof

This note closes the first R-averaged moving-cutoff carrier estimate, on a specified full-compact extension, for a primitive microscopic scalar. It makes an explicit replacement for the failed first fixed-history support step while preserving the actual averaged law.

It does not close the original fixed-history M04 assertion. Remaining actual-law work includes the complementary P/Q components, retained-history or density-state compatibility at later operations, the complete inherited/residual source densities, uniform-depth normalization and field matching, and the final full-law connected kernels and continuum conditions. The density-weighted interface DW gives exact linear jet transport and a proved linked-cluster bridge under its explicit actual factorization hypotheses; those hypotheses must still be verified for the complete multiscale law.

The result here is a first-step theorem, not a completed proof of four-dimensional Yang–Mills existence.

## Companion proofs

* [M04 Averaged First Step Scalar](M04_Averaged_First_Step_Scalar.md): exact R-history sum, actual joint-mass energy reserve, flat consequence.
* [M04 Moving Q Cutoff Localization](M04_Moving_Q_Cutoff_Localization.md): native moving-Q integral localization, full support and current proof.
* [M04 Q Boundary Shells](M04_Q_Boundary_Shells.md): finite real shells and integrated holomorphic chains.
* [moving q reconstruction input analysis](moving_q_reconstruction_input_analysis.md): actual native minimum/carrier input.
* [moving q ambient frame extension](moving_q_ambient_frame_extension.md): local guarded comparison, exact auxiliary constrained field, and positive ambient cutoff.
* [ambient gaussian marginal](../A_support_and_normalization/ambient_gaussian_marginal.md) and [local extension kernel](../A_support_and_normalization/local_extension_kernel.md): common positive density, reconstruction and scalar root budgets.
* [M04 Density Weighted Transport Interface](../A_support_and_normalization/M04_Density_Weighted_Transport_Interface.md): exact density-jet transport and the distinct full connected-output gate.
