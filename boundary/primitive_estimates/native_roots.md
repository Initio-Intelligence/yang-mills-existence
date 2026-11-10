# Summation at a native root on a two-sided trajectory

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

This note concerns local native derivatives of the **unsubtracted** boundary scalar.

## 1. The target includes a purely native first direction

The C-04 statement asks for local source-derivative budgets in addition to the weighted current Hessian. C-05 asks for the same bounds for the actual B and boundary-induced activities. The explicit C-04 statement is DS.13–DS.16 in [Annex AH](../../foundations/Annex_AH.md) of the [construction manuscript](../../paper/LONG_MANUSCRIPT_CONTENTS.md).

Its perturbations are actual admitted slot directions
\[
 h_l=(h_l^z,h_l^b,h_l^J,h_l^s),
 \qquad
 q_l=\max\left\{
 \|h_l^z\|_\infty/r_z,
 \|h_l^b\|_{\rm native}/r_b,
 \|h_l^J\|_\infty/r_J,
 \|h_l^s\|_\infty/r_s\right\}.
 \tag{N1}
\]
No condition requires \(h_l^z\ne0\). The local jet estimate can be anchored on any one direction. The permitted support factor is the number of actual localization cells meeting that direction's support, with the admitted local stencil convention. It is not total torus volume.

BC16.17–BC16.18 instead apply to
\[
 W(z,\xi)=\sum_X[F_X(z,\xi)-F_X(0,\xi)].
 \tag{N2}
\]
The source note expressly says that \(F_X(0,\xi)\) remains in the outer marginal. Consequently a persistent term \(H(\xi)\) is invisible to all of those current-anchored estimates. It must be retained in a native-only proof whenever it is part of the boundary scalar under consideration.

The strong heterogeneous native field norm used by the later C-05 formulation is
\[
 \|E\|_{\mathfrak N}
 =\sup_n\alpha_n^{-1}\max\{
 h_n|E|,\ h_n^2|\nabla E|,
 h_n^3|D^*DE|\}.
 \tag{N3}
\]
The present conversion theorem is formulated in this stronger actual-layer norm. It does not replace it by a bare fine-link norm. The C-04 regular background norm is discussed separately in Section 7.

## 2. The correct sufficient analytic norm is pointwise in the common chart

Let \(F_\Gamma\) be the full scalar activity, including every native-dependent normalization response assigned to it, and let \(S_\Gamma\) be its actual native dependency footprint. Include the fixed chart, stencil and nodal dependency collars in that footprint. Let \(w_\Gamma\ge1\) be a parameter-independent spatial weight, for example the required weaker physical-diameter weight.

A sufficient native root norm is
\[
 \sup_{D\in\mathcal D^+}
 \sum_{\Gamma:S_\Gamma\cap S\ne\varnothing}
       w_\Gamma |F_\Gamma(D)|
 \le A_k\,N_{\rm nat}(S),
 \tag{N4}
\]
where \(N_{\rm nat}\) counts the actual native cells, not an arbitrary fine subdivision of a coarse cell. A sum of the separate holomorphic suprema is unnecessary.

### Lemma N1 — common-direction Cauchy retains the native root

Assume (N4) on the genuine common larger native chart. Fix admitted directions as in (N1), and take their affine finite-parameter pullback exactly as in DS.13. Suppose the actual support rule implies that a differentiated activity vanishes unless it meets every direction support. Then, for \(m\ge1\),
\[
 \sum_\Gamma w_\Gamma
 |D_{h_1}\cdots D_{h_m}F_\Gamma(D_0)|
 \le e^m m!\,A_k N_{\rm nat}(S_1)
             \prod_{l=1}^m q_l.
 \tag{N5}
\]
The first direction may have zero current component. In particular (N5) applies to \(H(\xi)\) itself.

**Proof.** First restrict to a finite activity family. Use the product circles \(|t_l|=(m q_l)^{-1}\), with the fixed inner/outer native margin included in the radii in (N1). Apply Cauchy componentwise, then the triangle inequality and Tonelli to the sum of absolute values. On every point of the **same** product torus, (N4) bounds the sum by \(A_kN_{\rm nat}(S_1)\). The derivative factor is \(m^m\prod q_l\le e^m m!\prod q_l\). Increasing finite subfamilies proves the assertion by monotone convergence. If a direction has \(q_l=0\), its derivative is zero. This proof never exchanges \(\sum\sup\) with \(\sup\sum\). \(\square\)

All prescribed localization and current disks remain the original ones. The native/core coefficient is chosen after their fixed constants. If a further nonlinear retained-data map is applied, its complete higher chain rule remains necessary; this lemma does not identify arbitrary raw directions with native slot directions.

## 3. A geometric conversion for a fresh scalar family at every birth

Fix one final admitted external determining history. Let \(Q\) be an actual native cell of grade \(n\), with its fixed local dependency enlargement. A birth-\(b\) scalar has a physical carrier, its declared surviving completed cores, and an actual surviving boundary/component port. The source support and history identities give
\[
 \text{port}\in Z_b,
 \qquad Z_b\subset\Omega_{b+1}^{c}.
 \tag{N6}
\]
A consumed record is already part of its new completed scalar; it is not simultaneously treated as an untouched old record. For a reconstructed old coefficient use its actual external history, as in Section 13 of `Conditioning, deletion and mass factors for the retained history`.

Assume that the fresh scalar theorem, at every birth \(b\), supplies the **same positive pointwise** activity family with the following weighted rooted estimate:
\[
 \sup_D\sum_{\Gamma\ni r}
   w_\Gamma e^{\lambda t_b(\Gamma)}
       |F_{b,\Gamma}(D)|\le K_b.
 \tag{N7}
\]
Here \(r\) is either a birth-\(b\) exterior cell or one actual declared component incidence; the number of fixed incidence conventions per cell is bounded. The metric \(t_b\) retains the required exterior travel. In particular, a path inside \(\Omega_n\), when \(b<n\), cannot be a free passage through a birth-\(\le b\) completed core. All such cores lie in \(Z_b\subset\Omega_{b+1}^c\). This clause holds both for a full physical tree and for a correctly defined quotient metric that contracts only those actual cores. The spare rate \(\lambda>0\) is essential in the next step.

### 3.1 Births no finer than the native cell: \(b\ge n-O(1)\)

A native grade-\(n\) cell meets only a fixed number of cells of the coarser birth-\(b\) grid. If such a covering cell is not wholly inside a declared core, it is an exterior-cell root in (N7). If it is wholly inside a core meeting \(Q\), use that actual component root instead. The final native partition and the disjoint-core convention give a bounded incidence multiplicity; a geometric cover cell is not independently counted once for each old history.

Thus
\[
 \sup_D\sum_{\Gamma:S_{b,\Gamma}\cap Q\ne\varnothing}
     w_\Gamma|F_{b,\Gamma}(D)|\le C K_b,
 \qquad b\ge n-c_0.
 \tag{N8}
\]
This is the regime where no factor \(L^{4(k-b)}\) occurs. The fixed native cell, rather than a current-lattice root followed by enumeration of every fine historical root, is the anchor.

### 3.2 Finer births: the bare support count is false, but the guard pays it

For \(b<n-c_0\), the bare assertion \(N_b(Q)\le C\) is false: a native cell contains \(O(L^{4(n-b)})\) finer birth cells. However the support cannot consist of arbitrary such cells. Its actual port lies outside \(\Omega_{b+1}\), while \(Q\) lies in \(\Omega_n\). The admitted consecutive-domain buffer and the fixed stencil reserve imply that the last part of a connecting path to \(Q\) has physical length at least \(c h_n\). For instance, when \(b\le n-2\), the port is outside \(\Omega_{n-1}\), and the buffer between \(\Omega_n\) and \(\Omega_{n-1}^c\) gives this estimate. The finitely many adjacent grades are absorbed into \(c_0\).

This final path segment is outside every declared birth-\(\le b\) core. In birth units,
\[
 t_b(\Gamma)\ge c L^{n-b}-C.
 \tag{N9}
\]
Root each contributing carrier at one of the fine birth cells meeting \(Q\), and spend the spare rate in (N7). This gives
\[
 \sup_D\sum_{\Gamma:S_{b,\Gamma}\cap Q\ne\varnothing}
     w_\Gamma|F_{b,\Gamma}(D)|
 \le C K_b L^{4(n-b)}e^{-c\lambda L^{n-b}}.
 \tag{N10}
\]
Any fixed polynomial number of endpoint/stencil choices is also absorbed by the last exponential. This argument does not need a current-age decay estimate for an arbitrary native direction. It uses the exact native support and the actual surviving port.

Consequently
\[
 A_k^{\rm fresh}
 \le C\left[
 \sup_{b\le k}K_b
       \sum_{a\ge1}L^{4a}e^{-c\lambda L^a}
       +\sum_{b\le k}K_b\right].
 \tag{N11}
\]
The first series is finite. For a general local support, partition it into the actual native cells and sum this bound. It gives precisely the local factor \(N_{\rm nat}(S)\) in (N4).

**Scope of the root convention.** Formula (N7) must hold on the actual final footprints and component incidences. An estimate rooted only at a bookkeeping cell chosen far from the activity's native arguments is insufficient. Likewise, an unweighted root estimate without the positive spare travel rate cannot pay the fine-cell multiplicity in (N10). These are explicit properties of the one fresh positive theorem, not an independent current-age hypothesis.

## 4. The retained two-sided AF envelope sums persistent fresh terms

The source construction's upper profile comparison alone does **not** imply the summability needed here. The input used in this paragraph is the two-sided AF envelope printed in CMP109 (0.31), p.259, in the consistent source coupling normalization. If \(K\) is the final scale, it says
\[
 t_K+a_{\rm AF}(K-j)\le t_j\le t_K+A_{\rm AF}(K-j),
 \qquad t_j=g_j^{-2},\quad
 0<a_{\rm AF}=\beta\log L\le A_{\rm AF}=\beta'\log L.
 \tag{N12a}
\]
CMP109 promises a separate proof of that trajectory assertion; the present argument retains it as an AF input, in the same sense as the stipulated AF trajectory in C-05. It does not derive it from CMP119 (2.6), from small coupling alone, or from Proposition G8. In particular no positive single-step drift is asserted. Put \(c_{\rm AF}=a_{\rm AF}/A_{\rm AF}\). For \(b\le k\), (N12a) gives the sufficient consequence
\[
 t_b\ge c_{\rm AF}t_k+a_{\rm AF}(k-b).
 \tag{N12}
\]
Indeed \(c_{\rm AF}t_k+a_{\rm AF}(k-b)\le c_{\rm AF}t_K+a_{\rm AF}(K-b)\le t_K+a_{\rm AF}(K-b)\le t_b\). This deduction is uniform in the terminal scale \(K\).

Suppose the fresh bound has the form
\[
 K_b\le C\,t_b^s(1+\log t_b)^q
                 e^{-a(\log t_b)^r},\qquad r>1.
 \tag{N13}
\]
This includes a fixed inverse-coupling loss and any fixed polynomial in \(R_b\), with \(R_b\asymp(\log t_b)^r\). Put
\(f(t)=t^s(1+\log t)^q e^{-a(\log t)^r}\).
For a sufficiently small common coupling ceiling, \(f\) is decreasing, because
\[
 \frac{t f'(t)}{f(t)}
 =s+\frac{q}{1+\log t}-ar(\log t)^{r-1}<0.
\]
Therefore
\[
 \sum_{b\le k}K_b
 \le C\left[f(c_{\rm AF}t_k)+a_{\rm AF}^{-1}
                    \int_{c_{\rm AF}t_k}^{\infty}f(u)\,du\right]
 =:C\mathcal T(t_k),
 \tag{N14}
\]
and \(\mathcal T(t_k)\to0\). The change of variable \(v=\log u\) turns the integral into
\[
 \int_{\log(c_{\rm AF}t_k)}^{\infty}
       (1+v)^q e^{(s+1)v-av^r}\,dv,
\]
which converges because \(r>1\). This is the elementary running-tail mechanism of Proposition G8, with the weaker consequence (N12) of the explicitly retained AF envelope substituted for that proposition's stronger one-step-type hypothesis. The common ceiling is reduced until \(c_{\rm AF}t_k\) lies beyond the monotonicity threshold.

Combining (N11)–(N14) proves
\[
 A_k^{\rm fresh}\le C\mathcal T(g_k^{-2}),
 \tag{N15}
\]
uniformly in cutoff depth and total volume. Apply Lemma N1 to obtain all local native jets of the **unsubtracted** fresh scalar sum. An unchanged \(H_b(\xi)\) retains its single birth coefficient \(K_b\); it is not charged once again at every subsequent scale. Its presence in the outer marginal is therefore harmless for this summation. No current derivative is used to remove it.

This proves a useful consolidation for the ordinary/completed native geometries. Section 5.3 below treats the possible coarsening of a native cell by an interrupted preparation: its extra factor is a fixed polynomial in the corresponding birth profile and is absorbed by increasing the logarithmic exponent in (N13). Once (N7) holds on the actual scalar family, persistent completed/failed-prefix native terms therefore need the same positive theorem and the explicit AF envelope, rather than an additional current-age hypothesis.

## 5. The ordinary full-tree native sum: a direct guard proof

CMP119 (2.40)–(2.42), printed p.261, writes the ordinary boundary scalar as a sum over births and full-tree carriers. The functions are analytic in the native \((U,J)\) space, simultaneously real-gauge covariant with the old adjoint slots, and bounded by \(B_0e^{-\kappa d_b(X)}\). The literal support conditions after (2.41) are \(X\cap\Omega_b\ne\varnothing\) and \(X\cap Z_b^{\sim}\ne\varnothing\): the second is a **positive halo intersection**, not necessarily a core intersection. Printed p.262 gives a further component-locality clause and states that a relative-boundary version of the induction may also be used.

The printed bound reads:
\[
 |B^{(j,n)}(U_k,A,\{S_i\})|
       \le B_1 2^{-(j-n)}|\Gamma_n|,\qquad j>n,
 \tag{N16}
\]
with the indicated boundary restriction of \(\Gamma_n\) in the diagonal case. Summation gives (2.48),
\[
 |B_k|\le 2B_1\sum_n|\Gamma_n|.
 \tag{N17}
\]
The immediately preceding proof uses the exponential carrier bounds to sum over carriers. Thus no cancellation of large complex coefficients is needed for that source estimate once its actual carrier classification is retained.

Nevertheless, (N17), or (N16) as a bound for an entire layer, is **not logically the local native root theorem** (N4). An extensive bound permits concentration of the total dependence at a small subset of native variables. For a local derivative, the root must be an actual argument affected by the direction, not merely a location at which the coefficient was created or an arbitrary site to which its value was assigned. The proof below therefore does not infer a local statement from (N17).

The required ordinary-source bound is
\[
 \sup_D\sum_{b,X:\,S_{b,X}\cap Q_n\ne\varnothing}
 e^{\gamma\operatorname{diam}_k S_{b,X}}
       |B^{(b)}(X;D)|\le C B_0
 \tag{N18}
\]
for every actual native cell \(Q_n\). The common native chart and the support convention are those of the full current/native extension.

### Lemma N2 — a surviving old native point remains protected from a newer ordinary small-field domain

Let \(q\) have final actual terminal grade \(n\). For an ordinary birth \(b\ge n+c_0\), let \(\Omega_b^{\rm src}\) be the ordinary primitive's actual source small-field domain, including the prescribed reconstruction of older action terms on a later external history. Then
\[
 \operatorname{dist}(q,\Omega_b^{\rm src})
      \ge c M R_bh_b.
 \tag{N19}
\]
The same statement holds after the fixed native-cell/stencil enlargement, by increasing the fixed grade allowance \(c_0\).

**Proof.** Immediately before the ordinary \(b\)-th transformation, the point lies in the surviving old region \(Z_{b-1}\): its terminal grade cannot have been larger earlier and then decreased. CMP119 (3.2)–(3.5), pp.264–265, first covers \(Z_{b-1}\) by the current \(MR_b\)-cubes and surrounds it by at least four such layers before defining \(\Omega_b\). Further selector restrictions shrink \(\Omega_b\). Thus (N19) holds for the ordinary birth history.

Check explicitly the effect of a later completed R operation at scale \(r\ge b\). LFR II (1.33) removes every older determining piece inside an attempted completed component \(C\) and puts \(C\) into the scale-\(r\) determining piece. If \(q\in C\), its terminal grade is promoted to at least \(r\), contradicting \(n<b\). Thus \(q\) lies in a different component of the current large-field region. Since \(q\in Z_{r-1}\), the same ordinary collar construction places a ball of radius \(cMR_rh_r\) around \(q\) inside its own component of \(Z_r\). Every other component \(C\), including the one being completed, is outside that ball. Changes to an older external small-field domain occur only inside these completed components, by (1.33) and the external-history deletion. Therefore such a change cannot put a new point of \(\Omega_b^{\rm src}\) closer than \(cMR_rh_r\) to \(q\).

The upper inverse-coupling drift gives the established physical-scale comparison
\(R_rh_r\ge c'R_bh_b\) for \(r\ge b\); this is the comparison proved in Corollary G10 of [C-05: a geometric argument after completed-component integration](geometry_and_scale_control.md). It follows equally from the fixed AF polynomial comparison and the exponential mesh ratio. Hence every later completed modification preserves (N19), with one fixed reduced constant. No factor is multiplied once per modification: take the distance to the union of all modified components.

An interrupted preparatory operation keeps the old action at its changed background and adds the separate preparation boundary coefficients, as in LFR I (1.61)–(1.70). Keeping the carrier condition does **not** by itself prove the native root bound after that change: the actual native determining cell may be coarser and overlap many old carrier cells. The proposition immediately below is first asserted for the ordinary/completed geometry, or for the nonexceptional cells of an interrupted geometry. Section 5.3 treats the precise extra case. In particular the stopped-prefix variables on LFR I p.191 are not declared to be hidden variables.

Finally a native cell and its fixed stencils meet only a fixed adjacent range of terminal levels. The large fixed block separation is chosen before these local collars; increasing \(c_0\) absorbs their endpoint conventions. This gives the enlarged-support form. \(\square\)

This is a statement about a point which is **still an external native variable**. It would be false to keep an old grade on a point after the completed component containing it has been integrated. The exact history deletion is essential.

### Proposition N3 — ordinary unsubtracted native activity bound before the prefix exception

Retain a positive tree-decay share after the bounded-degree carrier entropy and the desired physical spatial weight. For an activity of birth \(b\) meeting \(Q_n\), its source carrier intersects \(\Omega_b^{\rm src}\), by the support condition after CMP119 (2.41). In the coarse-birth regime of Lemma N2, its full tree therefore satisfies
\[
 d_b(X)\ge cR_b-C.
 \tag{N20}
\]
The fixed birth-scale dependency collar changes only \(C\). Rooting its carrier at one of the bounded number of birth cells meeting \(Q_n\), and using the elementary tree count of DS.3, gives
\[
 \sup_D\sum_{X:S_{b,X}\cap Q_n\ne\varnothing}
 e^{\gamma\operatorname{diam}_k S_{b,X}}
       |B^{(b)}(X;D)|
 \le C B_0 e^{-c'R_b},\qquad b\ge n+c_0.
 \tag{N21}
\]
For \(|b-n|<c_0\), the same rooted count without extraction gives \(CB_0\); there are only a fixed number of such births. In the finer-birth regime use the literal halo condition carefully. At the ordinary \(n\)-step, the protected native region is separated from the older core by \(cMR_nh_n\). The birth halo costs at most \(CMR_bh_b\). The upper AF comparison gives
\[
 \frac{R_bh_b}{R_nh_n}\le C L^{-(n-b)}(1+n-b)^p.
 \tag{N21a}
\]
Choose the fixed \(c_0\) large enough that the right side is smaller than the available guard fraction whenever \(n-b\ge c_0\). This is a **fixed** adjacent-grade allowance, not a band growing like \(\log R_b\). The same guard is preserved when the native cell is created by a completed operation: a surviving older core lies in another current component, and the ordinary current collar separates that component from the newly completed one. Thus the halo subtraction leaves a distance at least \(cMR_nh_n\), and in particular at least \(ch_n\), to the required birth halo. The finer-birth bound is
\[
 C B_0 L^{4(n-b)}e^{-c'L^{n-b}}
 \tag{N22}
\]
as in (N10). The carrier spatial weight is allowed because its physical diameter in current units is at most a fixed multiple of \(h_b(1+d_b(X))\), and \(h_b\le1\). Thus a sufficiently small fixed \(\gamma>0\) uses only a fixed share of the source tree exponent.

The sum of (N22) is finite. The sum of (N21) is bounded by the running-tail estimate (N14), now with \(s=q=0\), since \(R_b\ge c(\log g_b^{-2})^r\), \(r>1\). Consequently
\[
 A_k^{\rm ordinary}
 \le C B_0\left[1+
 f_0(c_{\rm AF}g_k^{-2})+a_{\rm AF}^{-1}
       \int_{c_{\rm AF}g_k^{-2}}^\infty f_0(u)\,du\right]
 \le C'B_0,
 \quad f_0(u)=e^{-a_0(\log u)^r},
 \tag{N23}
\]
uniformly in cutoff depth, total volume and the stated ordinary/completed histories. This is (N18) on that scope. The ordinary coefficient \(B_0\) itself has not been assigned a small running prefactor: the factor in (N21) comes from its **actual native root's geometric separation**, and the adjacent-grade contribution remains \(CB_0\).

The proof uses the original full-tree ordinary representation. A previously scalarized relative-carrier family cannot be substituted into (N20) by retaining its name; it instead uses the fresh positive theorem (N7), or a separately verified replacement. Keeping the original full-tree source representation until the complete component scalar integration makes these two uses unambiguous.

### 5.3 Interrupted preparation: the loss does not compound at a surviving native slot

Here the two uses of “large-field region” must be distinguished. The determining complement \(Z''_r\) after a long preparation can be much smaller than the originally attempted component \(P\). A failed attempt nevertheless retains the **whole original component** in the external large-field history. LFR I p.181, immediately after (1.22), explicitly calls the failed alternative a new large field, says condition (ii) is no longer satisfied, and excludes the whole component. The same exclusion is used after (1.23), (1.55), (1.75), (1.82), and (1.88). Most decisively, p.201 after (1.99) factors the remaining operations on the original \(Z_r\setminus Z\) and renames that external set as \(Z_r\); the attempted set \(Z\) there contains only the components surviving all the tests. This includes late failures after the entire preparatory determining set has become \(\mathfrak B''_r\). Replacing the failed footprint by the smaller \(Z''_r\) would invalidate the following proof.

**Lemma N4 (one exceptional preparation window).** Fix a surviving external native point of final grade \(n\), and follow it after its most recent completed replacement. Up to a fixed adjacent-grade endpoint allowance, there is at most one failed preparation containing this point whose preparation window \([r-N_r,r]\) contains \(n\). There is in particular at most one preparation which coarsens this native slot through an unbounded number of levels.

**Proof.** Ordinary T steps enlarge the retained external large-field set by compatible covers and buffers; they do not split a surviving connected component. Components can merge. A completed R operation removes an entire connected component; if it contains the point, the old native slot is consumed and the tracking starts again at its new grade, by LFR II (1.33). If it does not contain the point, it cannot remove a proper portion of the connected component containing it.

Suppose the first relevant attempt fails at scale \(r_0\). The whole original failed component and its newly bad event remain in the external history, by the preceding source identities. Every subsequent selected connected component containing the point contains this whole ancestor, even if other components have merged with it. Eligibility (ii), LFR I p.177, therefore requires \(r-N_r\ge r_0\). The determining-set formulas (1.11)–(1.17) leave the layers at or below this lower endpoint unchanged, including the explicit retained endpoint piece. The native grade created by the first attempt is at most \(r_0\). A later attempt consequently cannot coarsen it again. A fixed endpoint allowance gives at most a fixed number of exceptional events, all within that fixed grade band; it never gives a number proportional to the age. \(\square\)

If a completed operation intervenes, old internal records belong to its exact scalar integral. Reconstructed ordinary coefficients are evaluated on the new external history, with the consumed component deleted. They are not counted again as old untouched internal records. Thus the lemma concerns actual surviving slots and does not assert that a reconstructed coefficient's old formal birth label must change.

Here is the size of the sole exceptional loss. Write \(r_0=r-N_0(r)\) for the top-band threshold of LFR I (1.10)–(1.11). Below that threshold, the preparation changes \(\Omega_j\) to its five-layer enlargement. The ordinary construction (3.2)–(3.5) of CMP119 first adds four layers around the compatible cover of the previous large-field set, then one axial layer, one further fluctuation layer, and two more layers. The five-layer change therefore leaves a fixed positive guard. In this range the native grading changes only by a fixed adjacent allowance, and the fine-port proof of (N22) remains valid.

Only the top \(N_0(r)+O(1)\) layers can be collected into one much coarser native cell. For that cell, the number of finer carrier roots loses at most \(C L^{4N_0(r)}\), times fixed powers of \(1+N_0(r)\). The exact source relation on LFR I p.192 is
\[
 L^{N_0(r)-1}=R_{r-N_0(r)+1}
       \le (L+1)(N_0(r)+1)^{\beta_0}R_r,
 \qquad N_0(r)=O(\log R_r).
 \tag{N24}
\]
Hence the loss is a fixed polynomial in \(R_r\). This statement also covers finer birth carriers whose native root lies below the top band: write their root count as \(L^{4N_0(r)}L^{4a}\), and use the still-present last segment to pay \(L^{4a}\) by \(e^{-cL^a}\).

For later use it is harmless to retain a larger explicit polynomial
\[
 \mathcal P_r
  =(1+N_r)^2(1+N_0(r))^{4\beta_0+2}(1+R_r)^4.
 \tag{N25}
\]
Choose the waiting depth once in the form \(N_r\le C(1+\ell_r)^{p_N}\), with the fixed exponent and constant large enough for LFR I (1.94) and the other real preparation requirements. The source says these requirements can be met by a fixed positive power of \(\log g_r^{-2}\). Equation (1.94) concerns the real \(p_0,p_1,\delta'\) profiles; it does not impose a power involving the later analytic exponents \(q_0,q_1\). Thus this real waiting exponent is fixed before the logarithmic reserve \(Q\) below. The complex insertion proof uses the same preparation, with the \(\varepsilon\) bounds replaced by the \(\alpha\) bounds and the same fixed dyadic reserve. Neither choice is increased with derivative order.

There is a bounded-incidence version for a native cell and its stencils. The source graded partition admits a fixed enlargement on which the neighboring native meshes differ by only a fixed number of levels. Distinct surviving failed components have whole compatible footprints; a cell of their native grade meets only a fixed number of them. The pointwise lemma therefore gives a bounded number of exceptional factors \(\mathcal P_r\), rather than their product along a history.

The AF envelope and the source upper profile comparison imply
\[
 \ell_n\asymp\ell_r
 \quad\hbox{if }|r-n|\le N_r+O(1),
 \qquad
 R_r\le C R_b\quad(b\le r).
 \tag{N26}
\]
For the first assertion, \(N_r\) is polynomial in \(\ell_r\), whereas \(t_r=e^{\ell_r}\); the possible difference in inverse couplings over that window has only a polynomial additive cost, and the two-sided envelope permits only a fixed multiplicative comparison. For the second assertion use \(t_b\ge c_{\rm AF}t_r\), then the fixed collar rounding. These comparisons suffice; exact monotonicity of the sequence is unnecessary.

It follows that the fresh estimate (N15) persists on a stopped-prefix chart after replacing \(K_b\) by \((1+R_b)^D K_b\) for one fixed \(D\). The spare connector pays the residual fine-root count, and (N26) pays the exceptional polynomial. The replacement merely changes the fixed logarithmic power in (N13). This proves the fresh-sector extension promised in Section 4.

For an inherited relative-carrier output created during a partial preparation, retain the outer attempt \(r\), the actual localization grade \(m\), and the incoming whole-atom transport/birth label \(b\), where \(r-N_r\le m\le r\). An incoming \(b\)-atom remains one \(b\)-atom. A recent exterior atom can have \(b>m\); its old port need not have grade at most \(m\). It must not be subdivided into \(L^{4(b-m)}\) independent old inputs.

For a resident input with \(b\le h=r-N_r\), its old port has grade at most \(h\le m\), so the original \(m\)-grid conversion applies. For a recent exterior input with \(b>m\), separate the root alternatives before counting: a root on the old dependency block uses its actual \(b\)-port and \(b\)-grid bound, while a root on a genuinely new \(m\)-record uses that record's actual integration-strip endpoint, native measure, and connector. Source (1.63) new records meet the integration strip; the unchanged/all-empty old reference stays in the old \(b\)-catalog. Summation of the new map's intermediate coordinates uses its normalized endpoint row, and is not another enumeration of finer old atoms.

Thus the effective transport label for the combined nonempty record is \(q_*=\max(b,m)\), while its new pieces retain their actual \(m\)-labels. At a fixed native grade \(n\), the root conversion costs \(C\) for \(q_*\ge n-O(1)\), and
\[
 C L^{4(n-q_*)}e^{-cL^{n-q_*}}
 \tag{N26a}
\]
for \(q_*<n-O(1)\), apart from the sole top-band polynomial already identified. Before simplifying this bound, the two root alternatives have the \(b\)- and \(m\)-versions of the superexponential factor; each is bounded by a fixed multiple of the \(q_*\)-version. This conversion uses precisely the positive record norm and actual normalized map-row attachment in (N7); it does not manufacture a low-grade port for a high-grade old atom.

Sum the actual integration/localization labels at this fixed attempt by \(N_r^2\). Recent raw-slot creation labels, if explicitly enumerated as well, add at most one further factor \(N_r\); old labels outside this window remain summed in the admitted incoming rooted norm. Use the conservative \(N_r^3\) count. If the verified new-record amplitude is
\(\epsilon_r=Cg_r^{-u}\ell_r^A e^{-cR_r}\), its entire native sum is bounded by
\[
 C\sum_{r\le k}N_r^3(1+R_r)^D\epsilon_r,
 \tag{N26b}
\]
which is the AF tail in Section 4 with a larger fixed logarithmic power. No factor \(L^{4N_r}\) has been inserted. The later current endpoint estimate retains the actual localization grade \(m\) of each new piece and the \(b\)-label of the old block. Only after its full fresh estimate has been obtained may a new small failed-prefix response declare the original whole failed component \(P_r\) as a protected core. Its core birth is then \(r\), and a component-root sum is performed before that declaration; the unchanged old atom is not promoted.

### 5.4 Two fixed logarithmic radii give the required native jets

A uniform unsubtracted **value** norm at the exceptional cell has not been proved by the preceding argument: it can carry \(\mathcal P_r\). The local jet target has at least one derivative, so the useful statement is an oscillation or first-response bound.

Choose, once,
\[
 \alpha^-_{0,n}=C_0g_n\ell_n^q,\quad
 \alpha^-_{1,n}=C_1g_n\ell_n^q,\qquad
 \alpha^+_{a,n}=\ell_n^Q\alpha^-_{a,n}\quad(a=0,1).
 \tag{N27}
\]
Here \(q>p_0+r+2\) is the target exponent already needed for the real prefix centers. The additional integer \(Q\) is fixed before the coupling ceiling and before any derivative order. The source analytic proof is run with \(q+Q\); native test directions are measured with the original \(q\). CMP119 (2.28) allows fixed integer exponents greater than one. Raising both exponents preserves their required ratio hierarchy. The absolute source radii \(g_n\ell_n^{q+Q}\) and the fixed polynomial nonlinear errors still tend to zero, so the finite predecessor smallness conditions are met by one smaller common coupling ceiling. The defining analytic formulas are unchanged; only their verified domains are larger.

A sufficient conservative choice, for the scalar and quadratic sectors described here, is
\[
 Q>2p_N+4r+2p_0+3.
 \tag{N28}
\]
If a fixed stencil convention contributes another known logarithmic power, add it to the right side before choosing \(Q\). The powers of \(\log\ell_r\) in (N25) fit the displayed spare \(3\). No exponential in \(N_r\) is being hidden in this condition.

On the larger chart, the ordinary source sum at one native cell obeys
\[
 \sup_{D\in\mathcal D^+}
 \sum_{\Gamma:S_\Gamma\cap Q_n\ne\varnothing}
       w_\Gamma |F_\Gamma^{\rm ord}(D)|
 \le C\{B_0+C_0+P_n^2\}
          \left[1+\sum_{r\in E(Q_n)}\mathcal P_r\right]
       +C\mathcal T_{\rm ord}(g_k^{-2}),
 \tag{N29}
\]
where \(E(Q_n)\) is the bounded exceptional set of Lemma N4. The Gaussian and successful-prefix contributions to this formula are specified in Section 5.5. This is a **pointwise common-chart** norm. It is not a sum of separate holomorphic suprema.

First take a field/current direction \(h_1\) supported in one native cell of grade \(n\), with target norm \(q_1\). On the genuine larger chart its norm is at most \(Cq_1\ell_n^{-Q}\), including the fixed neighboring-grade stencil allowance. For the common finite-parameter Cauchy pullback use
\[
 |t_1|=\frac{c\ell_n^Q}{m q_1},\qquad
 |t_l|=\frac{c}{m q_l}\quad(2\le l\le m).
 \tag{N30}
\]
All remaining directions keep their actual target radii. In particular the current and preparation disks have not been enlarged or reduced as a function of age. Their fixed inner/outer margins, and the fixed native core coefficient after the source localization constants, are included in \(c\).

Apply componentwise Cauchy on this single product torus and then the pointwise sum (N29), as in Lemma N1. The first leg supplies \(\ell_n^{-Q}\). By (N26)–(N28), it pays every exceptional polynomial and \(P_n^2\). The result is
\[
 \sum_\Gamma w_\Gamma
 |D_{h_1}\cdots D_{h_m}F_\Gamma^{\rm ord}|
 \le C^{m+1}m!\,(B_0+C_0+1)
                 \prod_{l=1}^m q_l.
 \tag{N31}
\]
The constants are uniform in the history, native grade, cutoff and torus volume. The complete normalized scalar \(H(U,J)\), even if independent of every current coordinate, is included. No current subtraction has been used in this argument.

For a general local first direction, decompose it with a smooth graded partition of unity subordinate to the actual native cells and their fixed enlargements. Such cutoffs have first and second differences bounded by \(Ch_n^{-1}\) and \(Ch_n^{-2}\). The product rules for \(\nabla(\chi E)\) and \(D^*D(\chi E)\), together with (N3), show that each localized direction has norm at most a fixed multiple of the original norm. The number of pieces is \(C N_{\rm nat}(S_1)\); each point meets a fixed number of them. The independent-current coordinate requires only the corresponding bounded multiplier. Apply (N31) to each first-leg piece and use multilinearity. This gives the factor \(N_{\rm nat}(S_1)\) required by DS.16, without a fine-cell subdivision of a coarse native test.

This proves a derivative bound on the **original target native norm** \(\alpha^-\). It does not rename the stronger \(\alpha^+\) radius as the target native radius, and does not claim the exceptional unsubtracted value bound to be uniform.

### 5.5 Ordinary Gaussian factors and successful prefix coefficients

The ordinary scalar \(B_0\) input is not the complete unsubtracted native ledger. The remaining ordinary Gaussian factor has the exact Schur form of OR17.2–OR17.4. Its localized coefficients are the native analytic walk/tree family
\[
 -\tfrac12 a_x^{\mathsf T}S_{j,\mathcal W}(x,y;U,J)a_y,
 \qquad
 \sum_{\text{internal labels at a root}}|\cdot|
       \le C P_j^2e^{-\kappa t_j(\mathcal W)}.
 \tag{N32}
\]
These are the actual source \(C_j^*\Delta^{(j)}C_j\) and principal inverse coefficients, including their independent-current term, not a Gaussian replacement of the law. The source input is precisely the localized inverse/walk expansion in CMP99 Theorems 3.9, 3.10 and 3.15, as matched in OR17 Sections 4.1–4.2.

Both old endpoints lie in \(\Omega_{j+1}\cap Z_{j+1}\). Thus their carrier has both ports used in the ordinary proof: a point of the older regular domain and a point of the retained large-field set, with only a fixed grade offset. The coarse-birth native guard gives \(CP_j^2e^{-cR_j}\); the fine-birth guard gives \(CP_j^2L^{4(n-j)}e^{-cL^{n-j}}\). The source AF profile bounds \(P_j^2/P_n^2\) by a fixed polynomial in the grade difference. The second exponential pays that polynomial. The coarse-birth sum converges by Section 4, with the extra power \(\ell_j^{2p_0}\). Adjacent grades have coefficient \(CP_n^2\), exactly the term paid in (N28)–(N31).

The old adjoint fields are still fixed. Their nodal conversion is admissible on the larger chart for the same source reason used by OR17. In a preparation, an old \(A_j\) in a shell that has already been integrated is no longer a surviving slot. Any recent \(A_j\) still present is either in an unchanged deeper piece or has node mesh differing from the active prepared grade by at most the fixed endpoint allowance. The potentially very coarse merged top layer therefore does not leave a fine unresolved \(A_j\) node inside it. This follows from the actual shell integrations (1.15)–(1.17), not from declaring all prefix variables internal.

Next retain the successfully integrated prefix terms \(C_r^{(i)}\). For the **pure prefix forcing** and original full-tree inputs, LFR I (1.63) gives full-tree carriers of a localization grade \(m\) between the integration grade and \(r\); each carrier meets the actual integration strip and \(\Omega_m\). Formula (1.70) gives the uniform analytic coefficient \(C_0e^{-(1+3\beta)\kappa d_m(X)}\) on the modified prefix chart. There are at most \(N_r^2\) pairs of integration and localization grades. Keeping this crude factor is sufficient; no unexplained summation over these labels is omitted. If the canonical alternative (1.104) has already been used at earlier levels, a prefix descendant of a completed relative-carrier scalar is **not** assigned this full-tree bound. It retains its old atom, holes and norm and uses the same fresh positive attachment transfer (N7), now through the partial preparation. That transfer must carry the unchanged branch with coefficient one and give a summable small correction; a factor \(C^{N_r}\), or a new fractional-power loss at every inner integration, would not suffice.

For a native point in the preparation window of a failed component containing it, apply the full-tree argument to the pure forcing just specified, using Lemma N4 and the polynomial (N25). Native grades below the merged top band retain the positive guard after the five-layer enlargement; grades inside that band lose at most \(L^{4N_0(r)}\). This gives its exceptional term in (N29). All logarithms in the window are comparable by (N26). Relative-carrier descendants use their actual positive root norm instead; the native conversion does not recreate a full tree through their old cores.

For a later preparation containing the point but with \(h=r-N_r>n+O(1)\), every contributing localization grade satisfies \(m\ge h\). The carrier's \(\Omega_m\) port and the protected old native point give \(d_m(X)\ge cR_m\). Since \(r-m\le N_r\), (N26) gives \(R_m\ge cR_r\). Its total bound is \(C C_0\mathcal P_r e^{-cR_r}\), summable by Section 4. For a preparation in another component, the ordinary current-scale guard separates that component from the surviving old native point; the physical connector gives the same bound, with its residual finer-root count paid before the sum over \(m\). For a finer surviving failed component, the final native last-segment argument gives the superexponential fine-grade bound. If that failed component was consumed, its old prefix scalar is part of the new completed scalar and is counted in the fresh sector, rather than retained a second time.

The genuinely failed relocation terms are different. PF.17 and PF.20–PF.22 retain their full action difference and noncanceling Jacobian and already have the form
\(g_r^{-a}\ell_r^A e^{-cR_r}\), with the actual fine-root count paid by the full separation \(D_{r,t}\) before summing over \(t\). They belong to the fresh estimate (N7)/(N13), including their current-independent native scalar parts.

Ordinary determinants are not a missing extra factor: CMP119 p.254 after (1.30) assigns the fluctuation normalization to the E/action factors, as recorded in OR17 Section 4.3. Their bulk pieces use C-04 and their boundary pieces use the scalar families above. The exact raw averaging deltas, Haar factors and relocated selectors have fixed real retained arguments in the native extension; no hard selector is differentiated. None of these statements applies to a later map which moves those retained raw arguments.

### 5.6 Preparation directions are kept in their actual source role

The preceding logarithmic gain is a first **native field/current** gain. It must not be assigned to an arbitrary preparation parameter merely because both parameters are listed in DS.13.

For the actual retained prefix scalar, (1.61)–(1.63) and (1.70) have arguments \(U_r^{(n)}\), the independently extended current, and the prescribed old variables. Earlier localization parameters have already been integrated or set at the specified endpoints in the coefficient construction; they are not extra surviving independent raw data. This is the literal argument list in the source. It does not prove a theorem for a new family which artificially keeps arbitrary earlier localization parameters alive.

Current localization/preparation parameters subsequently introduced for a current pullback remain on their **full printed disks**. When their forcing is the relative current input, the exact source input vanishes at zero current and the prepared kernel preserves that identity for every parameter value; those directions act on the current-dependent scalar sector already estimated on its joint contour. A prefix relocation has a different, possibly nonzero forcing at current zero. Its full action/Jacobian contribution is kept in the fresh family just described, on its actual joint native/preparation contour. No zero-at-zero argument is applied to that different forcing.

More generally, if a declared surviving preparation parameter \(s\) enters an unchanged ordinary scalar through an actual map \(\Phi_s\), the required first-leg identity is
\[
 D_s\{F(\Phi_s)\}=DF(\Phi_s)\,D_s\Phi_s .
 \tag{N33}
\]
The native theorem (N31) applies after the actual native norm and local endpoint row of \(D_s\Phi_s\) have been verified on the full \(s\)-disk. It does not erase that map or assert the row for an unspecified family. The PF.2/PF.7 separation is the verified row for the failed relocation family, and its fine-root sum is PF.16–PF.22. Further nonlinear pullbacks retain all higher chain-rule terms.

## 6. Which persistent masses may legally stay outside this native estimate

The primary final alternative LFR II (1.103)–(1.104), pp.391–392, leaves factors \(T'_b(Y)1\) which depend only on the retained raw output field specified by the source. The native directions in DS.13 and the C-05 chart vary the admitted field/current/preparation slots, while those retained raw arguments are fixed. Such a primary raw mass has zero derivative in these native directions. Its constant contribution to the action can remain in the outer measure.

This is narrower than saying that every current-independent factor can be omitted. A native-dependent self term \(H(U,J)\), or a native-dependent normalizer before the exact scalar expansion, is part of the unsubtracted native scalar. If it is moved into a reference mass, its compensating scalar factor remains. The safe real reference is fixed at one native center; then the actual variation \(H(\xi)-H(\xi_*)\) is still retained. Positivity and normalization can bound that variation without a lower bound on the reference mass, but cannot make it disappear.

A physical derivative moving the retained raw field itself is a different pullback. DS.13–DS.16 explicitly do not identify arbitrary raw directions with native unit directions, and a later retained-data map must keep all its higher chain-rule terms. No raw-mass derivative theorem is obtained by calling that variation a native slot perturbation.

## 7. Norm scope and current status

In the regular C-04 theorem, \(b\) is the current-scale relative regular field with radius \(c\alpha_k\). E14.46 proves the corresponding old-scale transfer \(\|b_j\|\le C L^{j-k}\|b\|\). The heterogeneous norm (N3) allows more general local perturbations on an actual fine old layer. A proof in the former smooth current-scale norm must not be relabeled as the latter without this conversion. Conversely, a local theorem in (N3) supplies the regular directional statement after its actual norm embedding.

The conclusions of this note are:

1. The local jet target includes a purely native anchor and therefore includes persistent \(H(\xi)\).
2. The correct sufficient analytic norm is the uniform **pointwise** weighted \(\ell^1\) norm (N4), or its first-response version. A sum of individual holomorphic suprema is unnecessary.
3. A fresh scalar family satisfying (N7), with its actual final support and spare positive connector rate, has a uniform unsubtracted native value norm after the geometric conversion and the AF tail. A fixed prefix polynomial changes only the logarithmic exponent in its fresh coefficient.
4. The tail uses the **explicit retained AF envelope** CMP109 (0.31), through (N12). Neither the construction's upper profile estimate nor small coupling alone proves this input.
5. The nonsmall ordinary full-tree B and exact ordinary Gaussian families have a uniform native **derivative** norm. A failed preparation can cause a polynomial loss in the unsubtracted value norm; Lemma N4 prevents this loss from compounding, and the fixed analytic profile \(\alpha^+\) supplies the first-leg gain needed in the unchanged target profile \(\alpha^-\).
6. Pure successful-preparation forcing retains its full (1.63)/(1.70) source domains and explicit polynomial \(N_r^2\) label count. Descendants of earlier completed scalar atoms retain their relative geometry and require the shared positive transfer through partial preparations. Failed relocation forces and Jacobians retain the stronger fresh prefactor already proved in PF.
7. Canonical masses depending only on fixed retained raw fields can remain outer. Native-dependent scalar terms, normalizer responses and current-independent \(H(U,J)\) cannot be removed that way.

Combining the first-response theorem (N31) with the fresh pointwise norm and the common-direction Cauchy argument gives, for a first native field/current direction and arbitrary further admitted joint-slot directions,
\[
 \sum_\Gamma w_\Gamma
  |D_{h_1}\cdots D_{h_m}F_\Gamma|
 \le C^{m+1}m!\,
       [B_0+C_0+1+\mathcal T_{\rm fresh}(g_k^{-2})]\,
       N_{\rm nat}(S_1)\prod_{l=1}^m q_l.
 \tag{N34}
\]
This is the DS.16-type pure-native and mixed-slot estimate for the unsubtracted scalar, including \(H(\xi)\), in the declared strong actual-layer norm. It applies also when an activity has no current-bond incidence and when it was born at the present scale. There is no claimed volume-independent value bound for arbitrary prefix constants.

Preparation-only first directions are treated by their actual sector assignments in Section 5.6: present current forcing, fresh relocated scalar, or a verified native pullback with its local endpoint row. Historical localization integration labels are not silently promoted to new independent native coordinates. Likewise the theorem does not control arbitrary moving selectors or arbitrary raw retained-data pullbacks, which are outside the slot statement.

At this source and trajectory scope, the remaining native application input is the **same** fresh positive-root estimate (N7) with the actual final footprints and full joint contour. The note does not by itself establish that positive completed-scalar estimate or declare C-05 complete. The parameter choice (N27)–(N28), the explicit AF envelope, the successful-prefix label count and the actual preparation-slot assignments must all be retained in the final assembly.
