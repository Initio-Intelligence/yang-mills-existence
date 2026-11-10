# All finite conditional source jets of the first R-averaged correction

This note proves a native-domain, all-finite-order extension of the first R-averaged moving-Q calculation. The resulting connected correction has a fixed factorial class \((q!)^2\), a genuine connected physical-carrier expansion, and compatible first coarse currents. It keeps one exponentially small defect factor after all source orders are paid. It does not assert a common nonzero physical-source radius as the coupling tends to zero, a bound on the total vacuum logarithm independent of volume, or an all-depth RG theorem.

The inputs are the actual first-step constructions AS, the native QC/QS theorem, and the primitive first-clean LC/GM source, reconstruction and current estimates. The ambient theorem RA gives a compatible positive kernel, but the unweighted estimates below are deliberately restricted to the native coarse-field domain and its stated buffered unit paths. The global compact-domain energy regulator is not replaced by a native polylogarithmic bound.

## 1. Exact source definitions

Fix the first homogeneous step, \(h'=Lh\), all zero-source running parameters and maps, and the globally P/Q-regular geometry. Let
\[
 F_j(U)=\alpha_j\beta_0\sigma_h(x_j;U)-c_j,
 \qquad b_j=|\alpha_j|+h^4|c_j|,
 \qquad j=1,\ldots,m,
 \tag{FJ.1}
\]
be primitive microscopic scalar marks. The anchor convention is the original fine stencil and its fixed coarse carrier. All gauge-preimage factors of RA.4a may be retained; these marks and their products are gauge invariant, so that normalized Haar factor changes none of the formulas below.

Let \(Z_Q(V;\mathbf t)\) be the exact first-R-averaged integral with its literal Q cutoffs, and \(Z_P(V;\mathbf t)\) the same complete density and reconstruction with the fixed P product. Thus
\[
 Z_\eta(V;\mathbf t)=
   \int\chi_\eta(z,V)D_V(z)
         \exp\!\left[\sum_{j=1}^m t_jF_j(\Phi_V(z))\right]dz,
 \qquad \eta\in\{P,Q\}.
 \tag{FJ.2}
\]
Every action, soft-gauge, Haar, coarea, exceptional-coordinate and normalization factor is the same one as in AS and QC. The domains and the reconstruction are specified at physical source zero. No derivative of an adaptive running map is included.

Write
\[
 \delta E(\mathbf t;V)=\log Z_Q(V;\mathbf t)-\log Z_P(V;\mathbf t),
\]
\[
 \mathcal D(\mathbf t;V)
       =\delta E(\mathbf t;V)-\delta E(\mathbf0;V).
 \tag{FJ.3}
\]
The branches are those given by the convergent source expansion at zero. For any multiindex \(\mathbf n=(n_1,\ldots,n_m)\) with total order \(q=\sum_jn_j\ge1\),
\[
 \Gamma_{\mathbf n}(V)
     :=\partial_{\mathbf t}^{\mathbf n}\mathcal D(\mathbf0;V)
     =\kappa_Q(F_1^{[n_1]},\ldots,F_m^{[n_m]})
        -\kappa_P(F_1^{[n_1]},\ldots,F_m^{[n_m]}).
 \tag{FJ.4}
\]
Here repeated labels mean repeated arguments of the conditional cumulant, not an independent approximation to the same field. At order one this is the scalar correction already proved in QC/RA.

The subtraction at \(\mathbf t=0\) is indispensable. The unmarked vacuum difference has a uniform anchored polymer norm, but its sum may be extensive. Only the source-containing difference \(\mathcal D\) has a total rooted absolute bound independent of total volume.

## 2. A native bounded source-species budget

Put
\[
 M_j=b_jh^{-4}P^2.
 \tag{FJ.5}
\]
A zero \(b_j\) gives a zero mark and can be omitted. More generally a purely constant mark has zero contribution to \(\mathcal D\) in every positive order involving that label.

Factor the common deterministic value
\(F_j(\Phi_V(0))\) from both integrals. It cancels exactly in (FJ.3), including its first retained variation. Define the actual fluctuation defect
\[
 f_j(z,V)=F_j(\Phi_V(z))-F_j(\Phi_V(0)).
 \tag{FJ.6}
\]
Use its supported primitive expansion \(f_j=\sum_Xf_{j,X}\), with every X containing the full j-th insertion stencil. It can be chosen coefficientwise zero at z=0 by constructing this difference before localization.

### Lemma FJ.1 — uniform native source coefficients

At a fixed positive primitive carrier rate, reduced once if necessary,
\[
 \sum_{X\supset x_j}e^{\nu n(X)}
     \left[\sup |f_{j,X}|+
          \sup\sum_d|D_df_{j,X}|\right]
       \le C M_j,
 \qquad n(X)=|X|+\mathsf t(X).
 \tag{FJ.7}
\]
The suprema include the stated native retained buffer, the fixed enlarged free-coordinate chart, and the complex coordinate tubes used by QC. The first variation is the normalized coarse variation, with all couplings specified. The analogous finite-difference bound holds along buffered unit paths.

**Proof.** The exact Wilson scalar defect rows of LC.35/GM.31–GM.33 give a majorant of the form
\[
 Cb_jh^{-4}a_{j,X}
   \left[\sqrt{E_X(V)}\,\|z_X\|+\|z_X\|^2\right],
 \tag{FJ.8}
\]
and a first normalized current majorant bounded by the same weighted coefficient class times
\(b_jh^{-4}[1+E_X(V)+\|z_X\|^2]\).
The exact local-lift/force construction and the actual native coarse regularity give
\(E_X(V)\le CP^2(1+|X|)\), since the first background factor \(P_0/P\) is a fixed source constant. On the fixed \(4P\) chart,
\(\|z_X\|\le CP\sqrt{1+|X|}\), including bounded imaginary displacements at defect slots. Thus both displayed quantities are at most \(CM_j(1+|X|)a_{j,X}\), with the corresponding derivative coefficient sequence. Its polynomial is paid from a strict part of the primitive carrier rate. The normalized direction and local rank counts are the already proved first-step ones. Integrating along a buffered elementary path gives the finite version. No arbitrary old-coordinate rank is introduced at this first step. ∎

As in QC, extend each source coefficient to the untruncated comparison integration by a **coordinatewise** smooth cutoff: one through \(7P/2\), zero from \(4P\), with the native analytic coefficient available on a slightly larger fixed chart. Write the resulting coefficient as \(\widetilde f_{j,X}\). On either physical P or Q support it equals the original coefficient. On a moved Q-defect coordinate its cutoff is identically one on the full contour tube. Other coordinates stay real, so no smooth cutoff is analytically continued. Its uniform bound is still (FJ.7).

For any fixed vector of nonnegative polyradii \(\mathbf r=(r_1,\ldots,r_m)\), write
\[
 \mathcal P(\mathbf r)=\{\mathbf t:\ |t_j|\le r_j\ \text{for every }j\}.
\]
For the source Mayer species
\[
 v_{j,X}(\mathbf t)=e^{t_j\widetilde f_{j,X}}-1
\]
we therefore have, for a fixed sufficiently small \(\eta>0\),
\[
\sum_{j,X}e^{\nu' n(X)}
       \left[\sup_{\mathbf t\in\mathcal P(\mathbf r)}\sup|v_{j,X}|+
             \sup_{\mathbf t\in\mathcal P(\mathbf r)}\sup\sum_d|D_dv_{j,X}|\right]
 \le C\sum_j r_jM_j\le C\eta
 \tag{FJ.9}
\]
whenever \(\sum_jr_jM_j\le\eta\). These polydiscs lie in the closure of the weighted source ball
\[
 \mathcal U_\eta
       =\{\mathbf t\in\mathbb C^m:\ \sum_j|t_j|M_j<\eta\}.
 \tag{FJ.10}
\]
The inequality follows directly from \(|e^u-1|\le |u|e^{|u|}\) and (FJ.7), using the fixed monotone envelope \(r_j\) for each source species. Its constants do not grow with m or q. The fixed-polydisc order of quantifiers matters: taking the supremum over the whole weighted source ball separately for each source tag would not give this bound. The product of these species reconstructs the original exponential on the physical supports. One may first truncate the absolutely summable coefficient registry and pass to its limit under the common majorants.

The radius here shrinks as \(P^{-2}\). No fixed physical-source analyticity radius is being assumed.

## 3. The source-containing defect expansion, with one current

Use the same exact Q/P species registry as QC.22, the same fixed outside grid, and the mixed enlargement
\[
 D=D_m(I_{\rm reg})\cup
       \bigcup_{e\in S_Q}D_\ell(Q_e).
 \tag{FJ.11}
\]
The regular support now includes every chosen source-coefficient carrier and every fixed failed-P slot. Its collar remains fixed. Only Q-defect slots receive the growing halo.

Introduce a common insertion copy and a kernel copy of the retained data, and define the two-copy version of (FJ.3) by
\[
 \mathcal H(\mathbf t;V_{\rm ins},V_{\rm ker})
 =\log q_{Q,V_{\rm ker}}
        e^{\sum_jt_jF_j(\Phi_{V_{\rm ins}}(z))}
  -\log q_{P,V_{\rm ker}}
        e^{\sum_jt_jF_j(\Phi_{V_{\rm ins}}(z))}.
 \tag{FJ.12}
\]
At the diagonal it equals \(\mathcal D\). At zero source it is zero in both copies. Both copies remain in the native bounded chart used in Lemma FJ.1. The compact pre-gauge presentation gives the same expression for these gauge-invariant marks.

For each analytic connected tag \(H_a\), define its direct and kernel-copy finite records exactly by
\[
 B_{a,d,\tau}(\mathbf t;V)=
 \frac{H_a(\mathbf t;V_\tau,V_\tau)
                  -H_a(\mathbf t;V,V_\tau)}{\tau},
\]
\[
 J_{a,d,\tau}(\mathbf t;V)=
 \frac{H_a(\mathbf t;V,V_\tau)
                  -H_a(\mathbf t;V,V)}{\tau},
 \qquad V_\tau=\tau_{d,\tau}V.
 \tag{FJ.13}
\]
The native unit paths and the two rectangular paths must stay inside the stated buffered domains. Their sum is the diagonal finite difference tag by tag. For higher coefficients these are the compatible canonical records of the conditional source-log jet; no record of an inherited input is reassigned.

### Lemma FJ.2 — total rooted analytic estimate

There are fixed \(\eta,\kappa,c,C>0\) such that, for every fixed vector of polyradii with \(\sum_jr_jM_j\le\eta\), the expansion
\(\mathcal H=\sum_aH_a\) converges normally on a spare neighborhood of \(\mathcal P(\mathbf r)\) and obeys
\[
 \sum_a e^{\kappa n(Y_a)}
 \left[
  \sup_{\mathbf t\in\mathcal P(\mathbf r)}\sup|H_a|
  +\sup_{\mathbf t\in\mathcal P(\mathbf r)}
     \sup_V\sum_d\sup_{0<|\tau|\le1}
        (|B_{a,d,\tau}|+|J_{a,d,\tau}|)
 \right]
 \le C e^{-cP^2}.
 \tag{FJ.14}
\]
The constants are independent of the chosen polyradii, the number and location of source labels, volume, and sufficiently small g. The individual tag majorants are the monotone absolute Mayer majorants evaluated at this one fixed vector \(\mathbf r\). Each tag contains at least one source species and one actual Q-defect species, and its physical carrier is connected. A tag depends only on source labels that occur in its source species.

**Proof.** Choose \(\eta\) so that (FJ.9) consumes only a fixed part of the strict small-activity margin of the existing first-clean expansion. This choice is independent of the number of sources because their **total** weighted activity is bounded. The ordinary and failed-P activities keep their original reserve. Lemma QC.2 supplies \(e^{-c_0P^2}\) per Q defect, after full initial footprints, surface factors, determinant losses and fixed-grid localization are paid. The added source factors are bounded Mayer species on the same chart; their total norm is \(O(\eta)\), and they are holomorphic on every moved coordinate tube.

The two logarithms share the ordinary, source and fixed failed-P registry. Their difference contains a Q defect. Subtracting the zero-source difference removes exactly the clusters with no source. This can be done at the tag level, because every source Mayer factor vanishes at \(\mathbf t=0\).

For completeness, the absolute estimate uses the usual two-distinguished-species version of the already established rooted cluster sum. Mark one source species and one Q-defect species. Sum the remaining convergent cluster majorant with its strict spatial slack. The defect activity has anchored norm \(Ce^{-cP^2}\); the total rooted source envelope on this polydisc is bounded by \(C\sum_jr_jM_j\). The possible incidences with the distinguished source carrier cost a fixed polynomial in that carrier, paid from the spare rate in (FJ.9). The resulting bound is
\[
 C e^{-cP^2}\sum_jr_jM_j.
 \tag{FJ.15}
\]
One may equivalently obtain the distinguished defect by interpolating its activity amplitude from zero to one. The same bound follows, without division by the ordinary smallness parameter. Normal convergence of the tagged majorants proves the value part of (FJ.14).

For the insertion-copy current, (FJ.9) gives the differentiated source species with the same total bound. For the kernel-copy current use the exact determinant/inverse score, complete interaction response, contour-coordinate response and real-shell estimate of QC/QS. A differentiated ordinary species has its own verified budget; it is not divided by its undifferentiated value. A differentiated Q defect retains a tail, and a derivative at any other position still leaves the original Q defect in the cluster. Every tag also retains a source, since the source-free subtraction was made before differentiation.

The single distinguished current position costs only the usual local-rank and carrier polynomials, paid by the fixed rate slack. Any fixed surface or P/R polynomial is paid by reducing the defect exponent once. Source derivative positions are controlled by the total norm in (FJ.9), not by the number of labels. Real shell differences are uniform in \(\mathbf t\) on this polydisc, and their majorants commute with the outside localization. Taking \(\eta\) smaller than the allowed activity margin by a fixed factor gives the stated spare neighborhood. This proves both separate current bounds and (FJ.14). The logarithms are those of the exact integrals because the expansion exponentiates to them at the physical endpoint. ∎

No extensive clean-event probability is divided out in this proof. Its nonvanishing statement can also be checked at real retained data directly from the bounded source exponent on the actual positive P and Q laws; physical-carrier bounds still require the connected expansion above.

## 4. A fixed factorial class at every finite order

Let the tags for \(\Gamma_{\mathbf n}\), \(B^{\mathbf n}\) and \(J^{\mathbf n}\) be obtained by taking \(\partial_{\mathbf t}^{\mathbf n}\) of the same tags in (FJ.13). No aggregation by physical carrier is performed before taking absolute majorants.

### Theorem FJ.3 — all finite connected correction jets

For every multiindex of total order \(q\ge1\),
\[
 \begin{split}
 h'^{4q}\sum_a e^{\kappa n(Y_a)}
 \bigg[\sup|\Gamma_{\mathbf n,a}|+
 \sup_V\sum_d\sup_{0<|\tau|\le1}
       (|B^{\mathbf n}_{a,d,\tau}|+|J^{\mathbf n}_{a,d,\tau}|)
 \bigg]
 \le C^{q+1}(q!)^2 L^{4q}
          \prod_j b_j^{n_j}\,e^{-c'P^2}.
 \end{split}
 \tag{FJ.16}
\]
Every nonzero differentiated connected tag contains the full insertion footprints of all labels with \(n_j>0\), as well as a Q defect. All constants and the positive physical rate are independent of q, volume and sufficiently small g. The sufficiently small coupling threshold does not depend on q.

**Proof.** Omit labels with \(n_j=0\). For the others take the multivariate Cauchy radii
\[
 r_j=\frac{\eta n_j}{2qM_j}.
 \tag{FJ.17}
\]
Their closed polydisc lies strictly inside (FJ.10), because \(\sum_jr_jM_j=\eta/2\). Apply Cauchy to every individual value and current tag. Formula (FJ.14) gives the bound
\[
 C e^{-cP^2}
     \prod_j n_j!r_j^{-n_j}
 \le C e^{-cP^2}
          (2q/\eta)^q\prod_j M_j^{n_j},
 \tag{FJ.18}
\]
since \(n_j!\le n_j^{n_j}\). The same estimate holds for finite current envelopes: Cauchy is applied to their analytic numerator difference at fixed real displacement, followed by the already uniform sum and supremum.

Now use, for every integer \(q\ge1\) and \(x\ge0\),
\[
 q^q\le e^q q!,\qquad
 x^q e^{-(c/2)x}\le q!(2/c)^q.
 \tag{FJ.19}
\]
The second inequality is the q-th positive term of the exponential series. With \(x=P^2\), these bounds turn (FJ.18) into
\[
 C^{q+1}(q!)^2 h^{-4q}
        \prod_j b_j^{n_j}\,e^{-(c/2)P^2}.
\]
Multiplying by \(h'^{4q}\) gives (FJ.16). Only one fixed part of the tail is spent on the cutoff power; a positive rare factor remains. There is no assumption that q is small compared with \(P^2\).

If a tag does not contain a given source label, its derivative in that label is zero. Each surviving source species contains its insertion footprint, and the logarithmic cluster carrier is connected. This proves the support assertion. The finite-record identity follows by differentiating (FJ.13), justified by normal convergence. ∎

In particular the fixed physical-carrier weight implies an exponential tree-separation bound for the displayed conditional connected corrections. This is the massive **first-step conditional** statement; it is not a long-distance full-law correlation estimate after the outer coarse field is integrated.

## 5. Exact full-jet and density identities

Define the normalized conditional full jets
\[
 G_\eta(\mathbf t;V)=Z_\eta(V;\mathbf t)/Z_\eta(V;\mathbf0).
\]
At every finite source order,
\[
 G_Q(\mathbf t;V)=G_P(\mathbf t;V)
                         e^{\mathcal D(\mathbf t;V)},
\]
\[
 R_Q(dV)=R_P(dV)e^{\delta E(\mathbf0;V)},
 \qquad
 R_Q(dV)G_Q(\mathbf t;V)
   =R_P(dV)G_P(\mathbf t;V)
         e^{\delta E(\mathbf0;V)+\mathcal D(\mathbf t;V)}.
 \tag{FJ.20}
\]
Here \(R_\eta\) is the actual unnormalized first coarse contribution, including its common \(C_0\), the original Wilson normalization convention, and the outer selectors belonging to the branch. These are exact algebraic identities; the density is included once.

The finite formal exponential of \(\mathcal D\) preserves the fixed Gevrey-2 coefficient class. For q labeled derivatives its coefficient is a sum over partitions of products of the connected coefficients. The elementary bound
\[
 \sum_{\pi\in\mathcal P_q}\prod_{B\in\pi}(|B|!)^2
       \le C^q(q!)^2
 \tag{FJ.21}
\]
follows from DW.14, or by bounding one factorial product by \(q!\) and summing the other with the ordered-composition identity. Each nonempty partition product has at least one factor \(e^{-c'P^2}\); keeping one of these factors proves the same rare coefficient class. A single finite current differentiates one partition block at a time, adding at most a fixed exponential-in-q combinatorial cost.

This exponential statement has a **forest** carrier interpretation. Distinct connected blocks of a partition may have disjoint, widely separated supports. Their products do not acquire an unpaid connected carrier joining those supports. The complete source density (FJ.20) keeps these products and the common density exactly once. An outer connected-density construction must provide the actual connecting factors later.

Likewise, the anchored smallness of \(\delta E(\mathbf0)\) does not imply a volume-independent total-variation comparison of the two whole coarse laws. Its extensive vacuum contribution is retained in (FJ.20), not reset to one or divided away.

## 6. Scope and use

The theorem gives all finite conditional scalar-source corrections, compatible first native coarse currents, a fixed factorial exponent, and exact density/full-jet identities for the original first R average on the globally regular P/Q branch. Every source order uses the same specified maps and actual cutoffs. The rare factor is a defect estimate for this actual operation, not a probability assigned to a signed activity.

The unweighted bound uses the native inequality \(E_X\le CP^2|X|\). It is not asserted on arbitrary compact retained fields, whose energies can instead be of order \(g^{-2}\). No uniform physical-source radius or infinite analytic source series is inferred from the resulting Gevrey-2 finite coefficients.

The calculation does not control complementary P/Q sectors, already transported old scalar inputs, residual histories, repeated RG depth, final running normalization, or the outer connected logarithm. In particular, it does not show that one may erase R and then apply the original history-dependent future kernels unchanged. Equation (FJ.20) is the exact source density from which a new continuation must proceed, or against which retained-history sufficiency must be proved.

This supplies a concrete first-step finite-jet input to the density-weighted interface. Its downstream factorization and uniform-depth conditions remain genuine tasks.
