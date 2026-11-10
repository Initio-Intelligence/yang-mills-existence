# Conditioning, deletion and mass factors for the retained history

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

This is a supporting proof and source-matching note. It does not assert completion of C-05.

**Reading guide.** The main source-history and canonical-mass arguments are Sections 13.1-13.4. The restricted composed-scalar age lemma is Section 13.10. Section 14 shows that the same true-grade argument works in the weaker original quotient norm. Section 13.6 is a conditional closed-ball induction; its unproved final positive transfer is stated as FH in Section 13.9, with a weaker sufficient alternative in Section 14.3. The generic tangent argument in Section 13.8 is not used in that generality; the exterior-halo-grade, particular-history monotonicity, and mass-cancellation discussions in Sections 12.3, 12.6, and 12.9 are replaced by Section 13 and are not used. The unsubtracted pure-native C-05 clause remains open independently of the positive transfer.

## 1. Exact issue and the stronger geometric observation

The disputed CR.22d estimates records by their original birth and tries to pay a factor L^{4(k-b)} before a new current-root resummation. The source, however, first resums native scalar terms and has substantially more geometric information than a small interaction coupled to a pointlike component.

LFR II, printed p.377, immediately before (1.68), states that a nonself localization domain Y contains every component of Z^~ which it intersects. Formula (1.67), printed p.376, defines d_{k,Z}(Y) by the length of a connected tree in Y visiting all exterior M-cubes. Its length inside Z is counted; only the obligation to visit every cube inside Z is absent.

Thus an interaction incident to a completed component contains its whole exterior halo. Two interactions sharing that component share exterior cubes as well. A normalized component cannot be treated as a bare zero-cost connector after this additional information is retained.

The following lemmas quantify two consequences. They require full halo support. Per-attachment smallness without this support does not imply them.

## 2. Definitions

Work temporarily on a fixed birth lattice and use M as length unit. Let H_v be disjoint eligible components. For the source application they are rectangular parallelepipeds whose side lengths lie between c_0 R and C_0 R. The upper bound and rectangular geometry are on LFR I p.177. The lower bound follows from the ten-layer construction described there: adding ten layers in every coordinate gives a lower side bound, not merely a bound on the longest side.

Let H_v^+ contain an exterior collar of at least one M-cube around H_v, or the M-cube cover of a smaller positive collar. The source localization domains are unions of M-cubes, so a positive collar crossing a grid-aligned face forces the corresponding exterior M-cubes into such a domain. Set C_v=H_v^+\H_v. We assume a one-layer subcollar can be chosen outside the other H_w. At one source birth scale this follows when distinct eligible components have separation at least M R and R is larger than a fixed constant.

For a scalar interaction e, let I_e be its set of integrated component slots and S_e its localization domain. The **whole-halo condition** is

    v in I_e  =>  H_v^+ subset S_e.

For a collection H of retained components, define t_H(S) to be the infimum of M^{-1} times the length of a connected rectifiable tree contained in S which visits each M-cube of S\union(H). Paths through H count with their ordinary physical length. No interior cube-coverage condition is imposed inside H. On the source grid the usual connected block-tree convention gives an equivalent quantity with fixed constants; one must choose a single convention before fixing the decay rate.

This is a connecting-tree metric, not the quotient metric which assigns zero length to travel through H.

## 3. A whole halo pays arbitrary finitely many interior ports

### Lemma 1: shell lower bound

For the preceding rectangular components in dimension four, there is c_s>0 such that every connected tree visiting all exterior M-cubes of all the halos in an interaction satisfies

    M^{-1} length(T) >= c_s sum_{v in I_e} R_v^3.                 (H1)

The constant depends only on the fixed side and separation conventions. It is independent of volume, the number of components, and the history depth.

**Proof.** On an exterior face of H_v choose an M-cube in every third tangential grid position, avoiding a fixed-width edge strip. Because every side has length at least c_0 M R_v, this gives at least c R_v^3 cubes. After reducing c, their closed M/4-neighborhoods are disjoint. The subcollar separation allows the same selection for different components with disjoint neighborhoods.

A connected tree meeting all selected cubes has to leave the neighborhood of each visited cube, apart from the vacuous one-cube case. Each such exit uses length at least c'M within that neighborhood. Summing these disjoint local lengths proves (H1). Equivalently, one may use the standard minimum spanning-tree lower bound for a uniformly separated family. The finitely many R_v below the asymptotic counting threshold are absorbed by decreasing c_s. On a torus this argument uses collars not identified across the period; any wrapping case must be handled by the actual periodic component convention. In particular a component whose dilation is the entire torus has no nonself exterior interaction of the type under consideration. □

### Lemma 2: bounded port extension

Suppose at most p_* extra points in each H_v must be attached to T. There is a connected extension T' containing those points with

    M^{-1} length(T') <= M^{-1} length(T) + D p_* sum_v R_v.     (H2)

Consequently, for every epsilon>0, choosing

    R_min^2 >= D p_* /(c_s epsilon)

gives

    length(T') <= (1+epsilon) length(T).                       (H3)

**Proof.** Pick a fixed exterior halo cube c_v. The old tree meets it. Connect each specified point of H_v to that meeting point along a path within H_v^+ of length at most D M R_v; rectangularity and the upper side bound give D. Summing gives (H2), and (H1) gives (H3). □

For a coefficient with a source factor exp[-(1+2 beta) kappa t], take epsilon<=beta/2. Then imposing the full connector weight exp[kappa t'] leaves at least

    exp[-(3 beta/2) kappa t].                                 (H4)

The cost is paid by a reserve in the same occurrence of the interaction. There is no repeated replacement kappa -> c kappa.

This lemma pays connector lengths of order R. It does not pay a tree visiting every interior M-cube, whose cost can be order R^4. The latter is neither established nor needed for this connecting-tree statement.

## 4. Normalized component integration preserves full connector lengths

### Lemma 3: common exterior anchor

Consider q interaction occurrences e_1,...,e_q. Repeated labels are allowed. Let their graph connect two occurrences when they share an integrated component. Suppose this graph is connected and the whole-halo condition holds. Let T_a be a source connecting tree for occurrence e_a. Then their support union S has a connected tree visiting every exterior cube of S and satisfying

    t_H(S) <= sum_{a=1}^q t_H(S_{e_a}) + c_d(q-1).              (H5)

Here H is the union of all component interiors involved in the tuple. If some T_a also visits cubes removed from the union's exterior requirement, retaining those visits only strengthens the conclusion.

**Proof.** Choose a spanning tree on the q occurrence vertices. Label each edge (a,b) by one component v in I_{e_a} intersection I_{e_b}. Fix, once for this v, an exterior cube c_v in its halo. Both T_a and T_b meet c_v by the whole-halo condition. Join their meeting points within that cube at cost at most sqrt(4) M in Euclidean length, or the corresponding fixed lattice constant. Carry this out for q-1 edges. The resulting graph is connected and visits every required exterior cube. Deleting cycles yields a tree without increasing its length. This proves (H5). No path across H_v has been declared free. □

If a normalized kernel has native dependence in a fixed enlargement of H_v beyond the halo already present in S_e, enlarge the declared halo and source support to include that footprint. Either every incident source domain contains this enlarged halo, or its missing connector must be included and paid using Lemma 2. That domain identification is part of the actual source application.

### Consequence for a convergent normalized cluster expansion

Suppose the source interaction has a Banach algebra norm bound

    ||V_e|| <= alpha_e exp[-(1+2 beta) kappa t_e],

and each normalized kernel has operator norm at most M_v. The exact cumulant expansion is connected in the occurrence graph. Weighting a q-th connected term by exp[kappa t_H(S)] is, by (H5), bounded by multiplying each occurrence by

    exp[kappa t_e + c_d kappa].

Thus the weighted expansion is controlled by the same rooted tree majorant as the unweighted expansion with interaction weights

    a_e = alpha_e exp[c_d kappa] exp[-2 beta kappa t_e]
          product_{v in I_e} M_v.                             (H6)

Any extra finite component-incidence exponential from the tree criterion can be included in a_e. Lemma 1 supplies an exponential exp[-c beta kappa sum R_v^3] to pay that incidence factor and the fixed joining cost. A disjoint component normalization does not require an interior tree spanning all its cubes.

This is a stronger spatial conclusion than a quotient-metric cumulant theorem. It follows from the actual whole-halo incidence information, not from normalization alone.

## 5. Rooted incidence sum at one source scale

At a fixed scale assume the actual source coefficient list is indexed by scalar localization domains (after the source's stated resummations), with the uniform (1.68) bound on those coefficients. Let v be a newly integrated eligible component. Fix one exterior halo cube c_v.

Every incident domain contains c_v. Encode an exterior visiting tree by a grid walk traversing a spanning tree twice, recording the finite cube choices. The usual source lattice-animal count gives at most C_d^{n+1} supports at length n, with the source's retained volume and tree reserves paying the multiplicities. There is no enumeration of interior cubes of the fixed H_v.

Keeping a positive part of the shell lower bound separate gives a bound of the form

    sum_{e:v in I_e} a_e exp[a |I_e|]
        <= C alpha_* exp[-c beta kappa R_v^3],                (H7)

provided the remaining tree decay exceeds the fixed lattice-animal entropy rate. The constants depend on the declared source norm convention and the already fixed decay parameters. Formula (H7) is a one-scale consequence of a genuinely resummed interaction list. It cannot be applied to an unresummed list with arbitrarily many duplicate activities per identical support unless their total coefficient norm is included.

At most one fixed scalar norm is charged for each source interaction occurrence. Newly normalized operations supply M_v factors; already integrated old components represented by scalar coefficients do not supply another M_v merely because an old label is visible.

## 6. What the source theorem supplies, and what must still be identified

LFR II Theorem 1 (p.355) asserts the form and all conditions/bounds of CMP119 Section 2 for all effective densities while the coupling remains in the specified small interval. CMP119 p.262 explicitly allows a relative boundary representation. LFR II p.392 says that (1.104) can be used in the inductive effective-action description. These are all-history native scalar assertions; it is unnecessary to demand a separate original-birth theorem merely to justify their stated scalar conclusion.

The common-halo argument applies directly to the fresh V(Y) of (1.68). At both Mayer and logarithmic exponentiations, output supports are unions of their input supports. Therefore, for a fixed completed normalization, the whole-halo incidence property survives both expansions. Equations (H5)-(H7) show that the absence of a tree covering a fixed component's interior does not force the absence of a full physical connecting tree between its exterior attachments.

For the repeated-history application one must distinguish two objects:

1. An unchanged old coefficient, with its old source label, support, and active retained slots.
2. A newly localized difference or normalized connected output, whose scalar coefficient is resummed in the current source lattice.

The following source facts are the basis of that distinction:

* LFR II p.369, after (1.49), splits action terms according to whether their localization domains meet the attempted component set Z.
* pp.372-377 localize the differences and explicitly resum their old indices and domains into V(Y).
* p.377 then adds back the action appropriate to the **new** determining history and subtracts the same expressions in V(Y). Its A'_k contains old-age terms on that new history.
* Self terms with Y equal to one component of Z^~ are put inside the literal T'_k operation. Nonself terms retain (1.68).
* pp.391-392 applies the normalized operations to the entire boundary exponential and retains the raw multiplier T'_k(Y)1.

Accordingly the algebraic identity is history-aware:

    B_old(U_old, eta_old)
      = B_new(U_new, eta_surviving) + Delta B_current.

It is not correct simply to say that every old-age expression meeting Z vanishes. A coefficient in B_new cannot depend on an eliminated slot, but it can remain an old-age scalar on the new determining geometry. This distinction must be reflected in any final induction.

## 7. How the shell lemma repairs the potentially lost port

The source's (1.66), on p.376, retains a factor

    exp[-beta kappa d_j(X)]

from the old carrier, in addition to the current-scale tree, the scaled-distance kernel, and localization-volume factors. For j<k its current-scale tree gain comes from the scale factor L^{k-j}; for j=k it uses the improved (1+4 beta) kappa decay after the ordinary T operation.

If d_j(X) is replaced by a full connecting-tree norm which omits only eligible component interior cube coverage, the possible new task is connecting an actual map attachment point inside such a component to the exterior tree. Lemma 2 pays that connector from an arbitrarily small fixed share of the retained old-tree reserve, because the same coefficient contains its whole birth halo and hence satisfies (H1).

The port count must be justified geometrically, not by saying that four map formulas occur. A single map localization can have many derivative sites. Here the source's **final** majorant (1.66) contains exactly one distance d(X,Sigma_i0), for the first nonempty localization domain. Choose endpoints x in X and y in Sigma_i0 attaining that distance, or approaching its infimum. Only x needs to be connected to the old carrier tree. If x lies inside an old eligible hole, one halo-to-x connector suffices. The subsequent localization domains have their own connecting current-grid volume factors; the source's derivation of (1.67) explicitly uses their connections to Lambda and the one distance factor connecting X to the first nonempty domain. Consequently p_*=1 for this old-carrier bridge. This is not a bound on the number of native derivatives or integration-by-parts terms.

This is a valid repair of a **local connector inequality**. It uses the surface cost R^3 versus the port distance R and so has no fixed rate loss on repetition. It also shows why a proof which remembers only a contracted point-component and its size misses useful information.

Two checks are essential before promoting it to the all-history theorem:

* The source's unchanged/reconstructed old coefficients must retain the whole halo terminal set of each still-active eligible slot, or carry an explicit replacement terminal set with the same paid port property. It is not enough that their final carrier contains the component interior.
* The old-tree reserve in (1.66), after its actual current-scale resummation and the input's own earlier normalization, must be the full connecting-tree reserve just used. A generic weaker scalar bound in a different relative norm is not a substitute.

The graph proof shows preservation through the two explicit exponentiations. The ordinary T support check can also be made directly. CMP119 pp.276-277 directs the old B differences to (3.6)-(3.7) and then to the localization construction. CMP116 p.8, immediately below (1.29), defines X_0 as the smallest current localization domain containing the original X and takes decoupling cubes disjoint from its interior. Every output support Y contains X_0 and hence the original X; unchanged first terms retain X. Thus this ordinary T localization does not trim an old halo. Mayer and logarithmic support unions afterward preserve it as well.

The remaining source-matching point is the exact current/new-history metric and quantitative resummation of reconstructed old coefficients. Whole-halo support and a full physical connecting tree are now available, but a full physical tree is not automatically the scaled-distance age bound needed for every birth-root count. In particular, the coarse current-volume part of (1.66) cannot be charged once per historical grade. The source's scalar resummation may bypass that stronger per-birth demand, but the matching of its actual output root norm must be completed.

## 8. Mixed-mesh scaling without filling hole interiors

### Lemma 4: nested-grid carrier scaling

Let the b- and k-grids be compatible nested cubical grids with cell side lengths a_b=M h_b and a_k=M h_k=L^{k-b}a_b. Let X be a union of b-cells. Its carrier must contain each declared hole H that it touches as a hole, together with a positive exterior neighborhood of that hole. The finite closed holes are disjoint with positive gaps. Let X_0 be the union of k-cells whose interiors intersect the interior of X. This is the minimal compatible coarse-cell cover; merely touching a face does not add an extra coarse cell.

Call a cell required if it is not wholly contained in the union of the declared holes. Then every required k-cell C of X_0 contains a required b-cell Q of X.

**Proof.** Since the grids are nested and C has positive-interior intersection with X, C contains some b-cell Q_0 of X. If Q_0 is required, there is nothing to prove. Otherwise its interior lies in one hole H: a connected open cell cannot be partitioned among finitely many closed holes with positive gaps. Because C is required, C is not wholly contained in H. Choose a path in C from an interior point of Q_0 to a point outside H, perturbing it off the grid faces if necessary. At the first exit from H it enters a positive gap before it can meet another hole. A point in this gap sufficiently close to H is in X by the positive-halo assumption. Choose it off the b-grid faces. Its b-cell Q lies inside C, belongs to X since X is a union of b-cells, and is not wholly in the union of holes. □

Every b-grid connecting tree in the definition of t_b^H(X) therefore visits every required k-cell of X_0. The same tree lies inside X_0 and has the same physical length. Taking infima proves

    t_b^H(X) >= L^{k-b} t_k^H(X_0).                           (H8)

The actual old holes remain physical sets; they are not replaced by a single large union in which travel is free. Removing additional visited-cell obligations for old holes wholly contained in a new attempted component only weakens the required output tree condition. Retained holes outside the attempt keep their physical footprint and halo.

The minimal-cover operation is precisely the one used on CMP116 pp.8-9 before (1.30)-(1.32), and on LFR II p.376 before (1.66). Equation (H8) is the mixed-hole substitute for the source's fundamental scaling inequality (CMP116 (1.31)).

### Lemma 5: a rooted carrier count with fixed holes

On one grid suppose the active holes have bounded aspect ratio and the separation condition dist(H,H')>=c_sep max(diam(H),diam(H')), as in the eligible-component geometry. Domains are grid-cell unions and are saturated by the whole halo of every hole used as a slot. For sufficiently large a there is C_a, independent of the positions and number of fixed holes, such that

    sum_{X contains Q} exp[-a t_H(X)] <= C_a                 (H9)

for a fixed grid cell Q, with the standard source connectivity convention. The sum is over localization domains, not over multiple unresolved coefficient labels with the same domain.

**Proof structure.** If Q is not inside a hole, the visiting tree is already rooted at Q. If Q is inside a hole, attach Q to a halo point. For holes of radius r in current-cell units, the shell lower bound and the inequality

    D r <= epsilon c_s r^3 + C_epsilon

show that this costs at most epsilon times the visiting-tree length plus a fixed additive constant. Thus a root at an interior cell costs a fixed factor and an arbitrarily small fractional tree reserve, not a factor depending on the hole diameter.

Round the resulting tree to the grid with fixed distortion and encode it by an Euler walk. Every exterior cell of X is visited. A hole containing at least one full grid cell can be filled at no combinatorial cost once its exterior collar is specified: the hole is fixed data. At most O(n) distinct such holes can occur along a walk with n visited cells, by separation and the disjoint collar selections. Choosing which are filled adds at most another fixed exponential in n. Holes too small to contain any full grid cell remove no cell from the visiting requirement and create no independent domain choices. Hence the number of domains encoded with n steps is at most C^n, uniformly in the fixed history. For a large enough residual exponent the geometric series converges. This proves (H9), with all fixed norm-equivalence constants included before choosing a. □

If a source coefficient is still a sum of many terms with the same X, its **sum of absolute coefficient norms** must be used in (H9). Spatial domain counting does not remove multiplicity of unresolved functional labels. Source (1.68) is already after the stated sums over old domains, old indices, and types; it is the appropriate scalar coefficient list for this application.

### Volume costs

An omitted hole volume is not linearly bounded by t_H. In four dimensions a hole of radius r has volume O(r^4) but shell cost O(r^3). For a fixed polynomial power p, however,

    |X|^p <= C_p (1+t_H(X))^{4p/3}

after including the exterior volume and using the shell count; a fixed exponential reserve pays this polynomial. This observation does **not** pay an exponential exp[c |H|] from t_H. Such an exponential would invalidate the transfer. The source's second exponentiation explicitly counts exterior volume, excludes interior-domain enumeration for fixed completed components, and includes one normalized-operator cost per newly touched component; see LFR II pp.391-392 and its modification of (1.92)-(1.95). Those exact conventions must be retained. Ordinary T integrations do not add a fresh integral over an already fixed old component merely because it appears in a scalar coefficient.

## 9. Separation of the four source-estimate uses

The potentially different roles of a full tree in LFR II (1.66)-(1.68) can now be separated.

| Source use | Mixed-hole replacement | What is retained |
|---|---|---|
| Old-to-new carrier projection | Lemma 4, (H8) | Exact L^{k-b} physical scaling; no interior volume filling. |
| First nonempty localization connection | One endpoint port, Lemma 2 | The source's actual scaled-distance factor d(X,Sigma_i0); no claim that four formulas bound the number of analytic derivatives. |
| Rooted carrier entropy | Lemma 5, (H9) | Absolute coefficient sums, actual fine roots, and the source's normalized kernel rows. |
| Connected component exponentiation | Lemma 3, (H5)-(H7) | Whole halos, complete normalized kernels, and the exterior volume factors. |

The old-index sum must still be evaluated with the source's own scaled kernel and local measures. The geometric lemmas do not justify replacing it with a new unweighted fine-site count. Conversely, once that native scalar resummation has been performed, multiplying its output by L^{4(k-b)} again would recount sites already summed in the coefficient.

At a source induction step the preserved scale inequality provides the same old-to-new gain as the original proof, while a small fixed share of the old-tree factor pays the new port and rooting costs. For current-born input the published (1+4 beta) kappa improvement supplies that reserve. Unchanged first terms retain their original native coefficient bounds and spend no additional reserve merely by being evaluated at a later background. Newly localized differences are resummed and receive a fresh current-scale output bound. This is the correct mechanism for avoiding a decay rate multiplied by a factor less than one at every history step.

The source's old boundary support condition is also part of the invariant: CMP119 (2.40)-(2.42) requires each surviving B^(j)(X) to meet both Omega_j and Z_j of the **current admitted determining history**. P.369 reconstructs the action on the new determining history, and p.377 adds its necessary old-age terms. These support clauses should therefore be applied to B_new using the new Z_j, not to obsolete original birth anchors. A replaced old raw slot cannot be retained as an invented current anchor.

The lemmas supply the geometric and scalar entropy changes needed for a transfer of the source majorant. Before a final C-05 declaration, the actual scalar interaction list and current/native maps still have to be checked against these hypotheses, especially for added-back old terms, failed preparation branches, and the original native-rooted derivative scope.

## 10. Ordinary Gaussian and normalized self responses

The argument retains all self actions in T'_k. It does not freeze any ordinary Gaussian or Schur coefficient. For an ordinary retained Gaussian term with precision K, integrated block I, retained block O, Schur complement S, and extension E a=(-K_II^{-1}K_IO a,a),

    D[-a^T S a/2] = -(E a)^T (D K)(E a)/2.

That response belongs in the actual scalar coefficient before the cluster weighting.

Likewise for normalized component kernels the current or native derivative differentiates the full normalized operator. On the fixed reference chart supplied by LFR II (1.71)-(1.75), write

    Pi_xi F = mu_0(e^{sigma_xi} F)/mu_0(e^{sigma_xi}).

All old self actions remain in mu_0 and sigma_xi. The cancellation (D Pi_xi)1=0 leaves (D Pi_xi)(e^V-1), rather than making D Pi_xi vanish. The separate primary-source analysis derives operator-norm holomorphy from the source's pointwise sigma bound.

## 11. Status

**Partial status, without Section 13.** The following paragraph states what holds without the retained K_1 and the external-history deletion of Section 13. Section 13 gives the main formulation of the scalar argument.

Proved here: the whole-halo shell toll; bounded interior-port restoration; full exterior connector preservation under connected normalized integration; nested-grid carrier scaling with mixed physical holes; a rooted carrier entropy bound for fixed separated holes; the corresponding one-scale rooted incidence estimate when applied to the actual resummed coefficient list; and the exact distinction between old-history, new-history, and freshly rebased coefficients.

Source-established: the native scalar all-history induction at its printed scope, fresh whole-halo support, the pointwise completed-component deformation, and the exact normalized marginal.

Not asserted here: a completed all-history C-05 derivative budget, the exact fixed-current load after every reconstructed-history map, or the pure native-rooted estimates of the full C-05 statement. The remaining source-matching items in Section 7 must be checked before those conclusions are made.

## 12. The retained outer reconstruction factor and the age estimate

This section records the strongest later development. The geometric lemmas above supply the appropriate old-carrier connector. The missing source factor is the **outer** reconstruction in (1.61), which is present even when the first nonempty localization has index 3 or 4.

### 12.1 Exact outer map

Write C_1=Y_1\Y_1^0. On printed LFR II p.373, (1.61) is of the form

    U_k^0 = U(B''_k(Y_1), D_{C_1}(U_1,H''_k,u_k^0), D_fixed).

All dependence on U_1 and H''_k in that formula is in the determining data on C_1. The gauge factors u_k^0 also occur **inside those data**; there is no separate output gauge factor bypassing the outer reconstruction. The remaining determining data displayed in (1.61) are the fixed V'', U_0^(AL), and their indicated restrictions.

Denote the derivative of the outer map with respect to its C_1 data by K_1. The exact chain rule therefore retains K_1 in all three cases:

    i_0=2:  K_1 D D_{C_1} D H''_k,
    i_0=3:  K_1 D D_{C_1} K_2 D D_{C_2} D H_{B_1},
    i_0=4:  K_1 D D_{C_1} K_2 D D_{C_2} K_3 D D_{C_3} D H_k.

These displays suppress additional local derivative factors, but not a dependence route. An empty earlier localization increment evaluates that earlier map at its unlocalized value. It does not remove its outer reconstruction derivative from the chain rule for a later increment.

For value differences one uses the fundamental theorem of calculus along the admitted interpolation in the changing determining data. The factor K_1 is consequently available **before** taking Cauchy estimates in source-localization parameters. Its endpoint decay is not a claim about a future observable derivative.

### 12.2 The actual determining geometry of K_1

LFR I p.192, following (1.71), identifies the double-prime notation with the completed N-step preparation: the superscript (N) is replaced by a double prime and U''_k=U_k^(N). Its determining set is therefore B_k^(N), explicitly constructed in (1.15)-(1.17), printed p.180. The original blocks below h=k-N are unchanged. At the endpoint h the retained part is Gamma_h intersection Z''_{h+1}. Formula (1.76), p.194, retains the deep integral over V_h|Z_h unchanged and separate from the shell integrations.

The geometry in (1.10)-(1.12) has one prepared M-layer between consecutive recent levels. The older unprepared collars are larger. LFR I p.186, formula (1.47), gives the concrete source comparison

    exp[-delta d(y, Omega_{j+1}^c\Z''_{j+1})]
        <= exp[-delta (M/M_1)(j-i)]

for y in the indicated Gamma''_i, i<j, with distance measured in the source M_1-block convention. This is the source's prepared-history grade estimate; no running R is assigned to the recent one-M collars.

The local splice B''_k(Y_1) agrees with B''_k on Y_1^0 and changes the determining data only in C_1, of width at most 2M_1 in its proper scale. Since Y_1 contains the whole attempted eligible component Z that it meets, a path from a resident old component to C_1 crosses the recent prepared annuli before reaching this splice. The fixed-width terminal convention changes the number of complete crossings by at most a fixed integer.

The starting native kernel bound is CMP102 Proposition 9, (190), pp.308-309. Visual checking gives exp[-delta_0 d/8], not exp[-delta_0 d/2]. The displayed row is for the Landau-gauge H(B) reconstruction. To obtain the actual axial-gauge U row in (1.61), compose it with the analytic block-local gauge reconstruction of CMP98 (104)-(106). Its footprint remains within the output determining block; the normalized path lengths over the nested averaging scales form a geometric sum, and the small-chart products have a uniform bound. This changes the fixed prefactor and endpoint rate, but creates no long path bypass. The output factors in (190) are h_n^{-1}, h_n^{-2}, h_n^{-2-beta}, and h_n^{-3} for the field, derivative, Holder and second-order outputs. Its input factor h_{n'}^{-4} cancels the actual input measure h_{n'}^4. After this transfer, physical normalizations, and an endpoint reserve, it gives

    ||K_1(x,dy)||_normalized <= C exp[-delta_* d_{B''(Y_1)}(x,y)] d nu(y),

with a uniform normalized row bound. Here d nu denotes the actual normalized determining-data counting/integration convention, not an unweighted sum over fine coordinates. The metric reference is CMP96 (2.46); the cross-reference (2.36) printed in some later texts is the indexing error identified in Annex BM.

The local averaging and u_k^0 derivatives in C_1 have fixed normalized bounds on the admitted common chart. They change the row constant and finitely many endpoint offsets, not the retained long K_1 path. The corresponding spatially prepared bounds use the endpoint reserve of the source walk expansion and the common complex domain (1.65).

### 12.3 A true resident port

**Remark (replaced by Section 13.2).** Section 13.2 uses an actual interior point of a surviving component, the exact source support/nesting identities, and the paid shell-to-interior connector. That argument replaces the more delicate exterior-halo native-grade discussion in this subsection.

The following qualification is indispensable. The point which anchors an old tagged record must be a point on its **actual retained** native/physical support, not a subsequently promoted abstract component label.

For a completed tag born at m, retain one genuine exterior birth-halo port q_m. The next ordinary T step surrounds the retained whole component by the source's buffers, so this port has native grade at most m plus a fixed endpoint allowance on later untouched histories. When that component is resident in an eligible k-component, condition (ii) on LFR I p.177 gives m<=h. For m<h the relevant determining blocks are unchanged by (1.15)-(1.17). For m=h, the positive birth halo remains in the retained endpoint region: the preceding ten-layer growth, minus the five-layer preparation trimming in (1.11), still leaves a full one-M_h halo. This uses the physical inequality M R_{h+1} h_{h+1}>=M h_h, which follows from the compatible running cube choices. The exact source buffer inclusion must be used at this endpoint, rather than declaring every point of an old component to have its birth grade.

If an old scalar coefficient was formed at a later scale b>=m and still depends on this tag, keep q_m as a port in its carrier record. A point in an older tiny component need not be rediscovered from the coarse support alone. Retaining one actual port adds at most a fixed current-cell connector if the component is small in the coefficient's birth units, and Lemma 2 pays it from the halo reserve if it is large. Thus the port can be included in the strengthened full-connector majorant with a fixed constant and an arbitrarily small reserved exponent loss. A tag which is consumed is not used as such a port afterward; its response is part of the new exact component operation and its freshly generated scalar outputs.

This explicit port convention is needed: a coarse cube which contains a tiny old tag does not identify the tag's original native grade merely because an unmarked tree visits that cube.

### 12.4 Joint old-tree and K_1 inequality

Let an incoming scalar record have current birth label b<k, full physical connector T_b in birth-b units, and a retained resident port q of grade at most b+c_0. Let x be the point where its native argument is changed. Attach x to T_b if necessary using the whole-halo port lemma. Let C_1 be the outer reconstruction boundary in (1.61).

Concatenate a path in the augmented old connector from q to x with a K_1 path from x to C_1. Every path from the resident core to C_1 crosses the prepared grades above b, apart from a fixed number of endpoint layers. For the part of this concatenated path carried by T_b, retain only its segments in grades r>=b. On these segments the weighted density is at most C/h_b (or C/(M_1 h_b) in the M_1 convention). Their weighted length is bounded by C(M/M_1)t_b plus the paid port constant. The portions carried by K_1 retain their actual weighted length. Consequently

    C_T (M/M_1) t_b + d_{B''(Y_1)}(x,C_1)
       >= c_T (M/M_1)(k-b-c_1)_+ - C_T'.                    (H10)

The point of this proof is that an old-tree segment is used only where its grade is at least b. Fine pieces below b do not need to be paid by a birth-b Euclidean length. The nested prepared annuli force the missing higher-grade crossings regardless of repeated exits or the positions of lower-grade holes. Their old physical connector lengths remain charged. A source current-grid volume is not used to pay any historical grade.

If X already reaches C_1, choose x there. Then the old connector alone supplies the necessary crossings. If every active anchor of a record lies outside the attempted component while X meets it, the carrier must instead cross the source separation from that whole component to the outside active component. The full physical connector and its true endpoint ports pay that separation in birth-b units. This is at least the corresponding required age cost after using physical scale conversion; it does not contract the attempted component before estimating its nonself contribution.

Splitting the old-tree and K_1 exponents into fixed shares gives

    exp[-kappa_res t_b-delta_res d_{B''(Y_1)}(x,C_1)]
        <= C exp[-Gamma (k-b)]                              (H11)

with Gamma a fixed positive multiple of min(kappa_res,delta_res M/M_1). Independent positive shares remain for carrier entropy, spatial output weight, normalized rows and component collars. Choose kappa, the localization parameters, and then M/M_1 in the source's order so that Gamma exceeds the fixed fine-root density and native-profile losses. The coupling ceiling is decreased afterward. No parameter depends on the number of previous histories.

### 12.5 Suppression before localization-parameter Cauchy

Represent an old scalar difference on the common complex chart by the integral of its native differential along the actual field-data interpolation. Keep K_1 in that differential by Section 12.1. Native Cauchy bounds the scalar differential by the old coefficient norm divided by its admitted native radius. The normalized map row and (H10) bound the change in its argument. The resulting **value** majorant therefore contains exp[-Gamma(k-b)] before source-decoupling derivatives are taken.

For a branch with first nonempty localization index 3 or 4, the intervening K_2,K_3 and local factors have bounded normalized rows. They do not remove K_1 or move its input C_1. Thus their composition changes the fixed row constant and profile factors, while (H11) survives. The actual gauge response is already in D D_{C_1} and hence also passes through K_1.

The common complex-domain statement (1.65) is used here on the entire interpolation family, not only at a real endpoint. Localizer Cauchy then spends its own fixed volume/walk reserve. One must not first sum an unweighted family of old births and only afterward ask a current derivative to restore the age decay.

### 12.6 Root count and the repaired recurrence

**Remark (not used in the main argument).** The particular-history monotonicity stated below is not needed and must not be used for reconstructed add-backs. Sections 12.8 and 13.6 replace it by the generation-b supremum over the source-constructed admitted histories, after the structural port class is proved.

Let A_{b,k-1} be the rooted sum of the actual frozen birth-b coefficient majorants in the strengthened full-connector/true-port norm. For the unchanged subfamily this norm is carried without multiplication, so A_{b,k}<=A_{b,k-1}. Consumed records are assigned to the exact fresh operation, not counted as untouched records with fictitious old ports.

At a fixed current root, the actual birth-b cell count is bounded by C L^{4(k-b)} times the spatially normalized root sum. The finite native-profile, gauge and AF comparisons contribute a fixed polynomial (1+k-b)^s and, if the chosen domain convention requires it, one explicit fixed exponential rate Gamma_dom. Equations (H10)-(H11) give

    contribution_{b->k}
      <= C(1+k-b)^s L^{4(k-b)}
           exp[-(Gamma-Gamma_dom)(k-b)] A_{b,k-1}.             (H12)

Choose the fixed reserve so that

    Gamma-Gamma_dom > 4 log L + lambda + 2.

Then (H12) is bounded by C exp[-lambda(k-1-b)] A_{b,k-1}. This is the intended CR.22d conclusion with its actual fine-root density retained. The factor is supplied by the old full connector plus the always-present K_1, not by the final coarse volume penalty.

Let F_0 be the existing ordinary/full-tree source allowance and let

    Abar_k=sum_{b<=k} exp[-lambda(k-b)] A_{b,k}.

Using the component rooted expansion of Sections 4-5, the newly generated completed outputs have

    A_{k,k} <= C_fresh zeta_k (F_0+Abar_{k-1}),

where zeta_k includes the actual fresh nonself and failed-prefix small factors. The already supplied source estimates have the form

    zeta_k <= C g_k^{-2}(1+ell_k)^A exp[-c R_k],
    R_k >= ell_k^r,  r>1.

The preceding halo estimate can improve parts of this bound, but no improvement is required. Thus sup zeta_k tends to zero at a smaller common coupling ceiling. The monotone carried part gives

    Abar_k <= (exp[-lambda]+C_fresh zeta_k) Abar_{k-1}
              +C_fresh F_0 zeta_k.

After C_fresh sup zeta <= (1-exp[-lambda])/2 this is a genuine uniform contraction. It closes the scalar repeated-record norm once the coefficient-level port assignment and the native K_1 family in Sections 12.2-12.5 have been matched for every source branch.

### 12.7 Remaining verification for C-05

The exact K_1 factor is visible in (1.61), its complex native kernel and normalized rows are primary inputs, and the prepared age estimate is explicit in LFR I (1.47). The geometric lemmas now provide the missing full physical connector and the true port needed to concatenate it with K_1.

It must still be verified that every record used in the frozen A_b recurrence has the true retained port described in Section 12.3, including records with older outside tags after a newer successful operation; that its field-data interpolation keeps the fixed data of (1.61) fixed in precisely the way used in the derivative chain; and that consumed/add-back terms are grouped into the fresh operation without counting a new old-age coefficient in the monotone subfamily. These are coefficient and representation identities, not a remaining generic cluster-expansion theorem. In particular, the phrase "four map stages" cannot substitute for the exact K_1 chain, and a coarse support cube cannot substitute for a true native port.

### 12.8 A safer induction variable for reconstructed old histories

The frozen-record formulation in Section 12.6 is not necessary. It can be replaced by a birth-generation supremum, which is better suited to the source's add-back action on a changed history.

For each b define A_b^* as the supremum of the absolute rooted birth-b scalar norm over **all admitted depth-b determining histories**, retained real data, and the common native complex charts specified in the theorem. The norm includes the full physical connector and one genuine surviving component/boundary port. All normalizations and source-operation identities are those of the actual construction. The induction proves a bound for this supremum at the time generation b is constructed.

A later B_new^(b) in A'_k uses an admitted depth-b truncation of the new determining history. Therefore its bound is A_b^*, whether or not its coefficient list is literally a sublist of the previously encountered history. This does not identify two different conditional densities. It is a uniform bound on both members of the admitted input class.

Put

    Abar_k^* = sum_{b<=k} exp[-lambda(k-b)] A_b^*.

Then the carried contribution satisfies the exact identity

    Abar_k^* = exp[-lambda] Abar_{k-1}^* + A_k^*.

The K_1 age estimate (H12), applied separately on each actual old/new admitted history, bounds the incoming total by F_0+C Abar_{k-1}^*. The fresh component and prefix estimates therefore imply

    A_k^* <= C_fresh zeta_k(F_0+Abar_{k-1}^*),

and the same contraction follows. No monotonicity claim about a particular changed-history record list is required.

The all-history quantifier matters here. If the source coefficient theorem covered only one realized sequence, this supremum could not be introduced without proving the extra histories are admitted. In the stipulated C-01/Balaban source class the induction is over the admitted determining sequences, as in CMP119 Section 2 and LFR II Theorem 1. A source add-back term must be matched to that class before invoking its A_b^* bound.

This also clarifies consumed ports: an eliminated old component is not assigned its old grade in the new history. Its old-history contribution occurs on the incoming side of the exact operation; the reconstructed new-history coefficient is a separate member of the class, with its own actual surviving support and port. New normalized outputs are assigned the current generation k.

### 12.9 A concrete true-port assignment for the normalized scalar expansion

**Remark (replaced by Section 13).** In particular, the algebraic cancellation at the end of this subsection is not a quantitative justification for changing a canonical mass. The main proof uses exact deletion of the internal old history, keeps every canonical tau unchanged, and uses a single-port supremum rather than an uncharged list of all fine ports.

Keep the following metadata until after the positive majorant has been summed: an interaction's scalar birth label, its actual retained eligible components, one original exterior halo port for each such component that is needed as an anchor, and a connecting tree which visits those ports as well as the required exterior carrier cells. Original fine ports are retained as physical points when a carrier is covered by coarser cells. This adds no new field variable, changes no activity, and is not an extra conditioning of the measure.

The exact source operations allow the following assignment.

1. **Ordinary T.** An old first term is the same native scalar function evaluated at the next background; (3.15), CMP119 p.268, displays this split. Its physical port remains on the same retained component. Every localized difference contains the old support in its compatible coarse cover, as checked in Section 7. Retain the old physical tree and port in the union, not merely its new cover cell.
2. **Preparation or a failed prefix.** Whole-component exclusions keep the old raw component inside the unreplaced attempted region. LFR I (1.15)-(1.17) and (1.76) leave the deep raw operation unchanged. Keep its original port; do not replace it by the center of a promoted over-carrier. The native grade used by K_1 is that of this actual port in the admitted prepared determining geometry.
3. **Fresh completed scalar output touching a retained Y component.** In (1.103), a connected logarithmic term which genuinely uses one of the newly normalized retained operations has support containing its whole halo. Assign a new port of that Y at the current birth k. The common-halo tree construction visits it. All still-relevant older exterior raw-component ports in its inputs can also be retained in the support union.
4. **Fresh output with an older exterior component but no new retained Y.** Retain a port of that older component from the input which makes the output depend on it. Its birth m is at most the new scalar birth k. The old physical tree is part of the connected union, so the port is retained even when its old halo is smaller than one current cell. It is not reconstructed afterward from coarse carrier geometry.
5. **No surviving eligible component.** Successful components have the explicit source factor which pays restoring the full interior carrier tree: LFR II p.389 compares the successful-component suppression to exp[2 kappa (100 R_k)^4] before (1.95). All consumed old components are contained in the newly treated whole component, so restoring that component covers their interiors as well. Such an output belongs to the source's full-tree/regular sector rather than the retained-tag norm. It needs no nonexistent old port.

The factorization and the source's fixed-footprint rules make these cases exhaustive for the newly normalized scalar terms. A scalar term independent of every newly integrated slot is separated as an external term before the normalized expansion; the identity Pi 1=1 does not create a new cluster or a new birth for it. If its old geometric component is removed, its source action contribution must be grouped with the successful-operation reconstruction, rather than carried under an obsolete boundary label.

The following algebraic identity was considered as an initial possible implementation. It is **not used as a quantitative rebasing step in the final formulation in Section 13**. If C_new is independent of the variables integrated by a component operation, then

    exp(C_new) Pi[exp(V_old-C_new)] = Pi[exp(V_old)].

The source provides the relevant independence where A'_k is placed outside the literal T'_k operations in (1.72), pp.378-379: such a coefficient is external to their eliminated variables and internal history sums. A self add-back assigned instead to V(X^~) changes the kernel reference and its raw mass. In that case perform the cancellation at the **complete unnormalized marginal**,

    exp(C_new) T'[exp(V_old-C_new)] = T'[exp(V_old)],

or retain both the normalized numerator and every changed tau=T'1 factor. Replacing Pi while omitting the mass change would be incorrect. Combine the entire relevant add-back scalar before assigning output birth labels. A factor which still depends on an integrated slot remains inside the complete operation and is not pulled out.

Although that equality is exact, it does not by itself preserve the chosen scalar norm: changing a self add-back changes the canonical raw mass and may simply move C_new into log tau. The source-history support argument below avoids this issue and keeps every canonical mass unchanged. Also, the port norm must use a supremum over one selected true port per scalar occurrence, or an already paid input-tree union; it must not add arbitrarily many tiny historical ports for a single fixed constant.

## 13. Source-history deletion, canonical masses, and the strengthened scalar induction

This section is used in place of the add-back cancellation of Section 12.9. It gives an actual source classification, rather than declaring the class of admissible reconstructed coefficients by assumption. Its source-history and port conclusions are unconditional within the admitted source construction. The scalar closed-ball argument is conditional on the final positive halo-completion majorant stated precisely in Section 13.9; it must not be described as an actual completed C-05 recurrence before that transfer is proved. The pure-native clause of the complete C-05 statement is a separate open issue.

### 13.1 Exact deletion of the older internal history

The relevant source identities are as follows.

1. CMP119 p.254, (2.1), has the exact nested sequence

       Omega_1 superset Lambda_1 superset Omega_2 superset Lambda_2
                superset ... superset Omega_k superset Lambda_k.

   CMP119 p.255, (2.3), defines Z_j=Lambda_j^c. Hence, on each one admitted history,

       Z_b subset Z_k,       Z_b subset Omega_{b+1}^c.        (H13)

2. LFR II p.365, (1.33), defines the new determining set by

       Gamma_j^new = Gamma_j'' intersection Z^c,   j<k,
       Gamma_k^new = Gamma_k'' union Z^(k).                  (H14)

   Thus no old determining layer survives inside an attempted completed component. The new coarse field there is the field explicitly defined in (1.34), and the new background is (1.35).

3. LFR I p.201, after (1.99), explicitly replaces the external Z_k by Z_k\Z and factors the old sequences restricted to each attempted component into that component's operations. These are the internal history sums in LFR II (1.71)-(1.72). Consequently, before the final failed components Y_i are inserted at the current level, the external reconstructed action has

       Z_k^ext = Z_k^old\Z,
       Z_b^ext subset Z_k^ext,  b<=k.                       (H15)

   This is not an inference that a determining set alone fixes every fluctuation region: the external Z_k identity and the componentwise history factorization supply the large-field-set statement as well as (H14).

4. CMP119 (2.41) requires every nonzero boundary coefficient B^(b)(X) on that history to satisfy X intersection Z_b nonempty. LFR II p.377 reconstructs precisely the action on the new determining history in A'_k. Therefore every reconstructed B_new^(b)(X) which meets the attempted region Z also satisfies

       X intersection (Z_k^old\Z) nonempty.                (H16)

An old boundary add-back cannot be confined to a consumed component. It must extend to a genuinely surviving exterior large-field region. This includes the boundary terms of the current ordinary T operation in the reconstructed action, although their birth index is k and they need no age estimate. The final failed Y_i are added only at current level in (1.101)-(1.104); they do not resurrect an internal old Z_b in A'_k.

The preparation coefficients with modified native indices are a separate family. LFR II p.369 identifies the additional boundary term in (1.49) as the sum produced by the N preliminary integrations. These coefficients enter the expressions localized into V; they are not newly added old-generation coefficients in A'_k. Their native mesh index must not be confused with the generation label in the recurrence. They retain the accepted preparation/prefix majorant, including its full sum over the allowed intermediate indices.

### 13.2 A true port without a promoted-center assumption

Use the source construction's following two scalar sectors.

* The ordinary sector has a connected physical tree visiting every carrier cell. It has no omitted interior cells, and retains the existing source majorant.
* A completed-component scalar has an explicitly declared finite family of actual surviving completed components H. Its carrier includes each such component and its original positive halo. The tree visits all cells not wholly inside these components, but its whole physical length is charged.

An omitted component H born at m is an actual retained large-field region in Z_m, not an abstract tag created only by coarse covering. Choose a single physical native port q inside H. By (H13), its determining grade is at most m. If H is resident in an eligible attempted component at time k, eligibility gives m<=h=k-N. LFR I (1.10)-(1.17) has Z_h''=Z_h and the prepared nested sequence Z_h subset Z_{h+1}''. Hence the port remains in an unchanged deep layer when m<h and in the retained Gamma_h intersection Z_{h+1}'' when m=h. Choosing an interior port removes the need to prove that a particular thin exterior halo stays in one grade. The shell-port lemma pays the physical path from the exterior visiting tree to q.

If the scalar was born later, at b>=m, then grade(q)<=m<=b. No fine port is reconstructed from a coarse cell center. If the scalar is a reconstructed old add-back, (H15)-(H16) place its surviving components and boundary anchors outside the attempted Z. If it has no omitted component, it remains in the ordinary full-tree sector.

This classification is proved inductively from the operations, rather than imposed on an unknown class. The base action has no completed holes. Ordinary unchanged terms preserve their actual supports and retained components. Localized differences retain the original carrier under the compatible cover, so the physical hole and its positive halo remain attached. Support unions preserve them. During a completed operation, components inside Z disappear from the external older history by (H14)-(H15). New normalized scalar outputs either contain a new retained Y_i with its whole halo, retain an older exterior hole from an input carrier, or contain no surviving omitted hole. These are the exhaustive alternatives. In the last alternative, the successful-component factor pays the restored interior tree as in LFR II p.389, before (1.95); (1.99)-(1.100) explicitly gives the full-tree regular bound. A failed-prefix operation has not completed the replacement and retains its old component and old history; its accepted prefix bound is carried with that actual port.

### 13.3 The single-port norm and multiplicity

For a carrier X with declared holes H, let t_b(X;H,q) be the minimum physical length, in birth-b M-cell units, of a connected tree visiting all required cells and the selected true point q. Define

       t_b^bullet(X;H) = sup_{q in P(X)} t_b(X;H,q),         (H17)

where P(X) is the set of allowed actual single ports in the declared surviving holes. This is a supremum, not a sum over ports. A coefficient can therefore use whichever actual resident or exterior port is relevant to a later estimate without paying an unbounded fine-tag multiplicity.

For any one q in a hole of radius r in b-cell units, the shell/port estimates give

       t_b(X;H,q) <= (1+eta)t_b(X;H)+C_eta.                 (H18)

If the hole is tiny, the cost is a fixed number of current-cell lengths; if it is large, its R^3 exterior-shell reserve pays the O(R) path. The constants are uniform in the number of other holes. The same bound holds for the supremum (H17). A selected native evaluation point adds at most one further port, so the proof of the age inequality has a fixed two-port cost, not one cost for every derivative in a localization expansion.

Under a connected expansion, a chosen output port lies either in one input carrier or in a newly retained component. In the first case use the tree with that one port for that input and unported trees for the others. In the second case attach the chosen port to the fresh common halo. The occurrence spanning tree then gives

       t_out^bullet <= sum_a t_a^bullet + C(q_occ-1)
                         + paid fresh port cost.           (H19)

Only one selected port is inserted into this proof. No sum over all historical tiny components is hidden in C. The original paid input-tree union can alternatively be retained; the supremum formulation is a convenient uniform notation for exactly the estimate needed later.

### 13.4 Canonical self masses are unchanged

Keep the literal T'_k in LFR II (1.71), its canonical tau_Y=T'_k(Y)1, and its normalized Pi_Y=tau_Y^{-1}T'_k(Y). In particular, do not move an old self add-back between A'_k and log tau.

The dangerous hypothetical consumed-only old B_new does not occur, by (H16). Incoming old boundary contributions located inside the completed component remain in the actual V(Y^~) self action. Reconstructed ordinary E/R self terms and the explicit Gaussian/Wilson terms are precisely the regular terms already present in (1.71). Every surviving old B_new which meets Z is an exterior bridge and is estimated with its real exterior port/full tree. Thus the structural proof needs no change of the canonical kernel or its mass.

The exact relative-mass estimate is still useful and must include all self responses. On the source chart of pp.379-380, write the unchanged canonical measure as

       T'_xi F = tau_0 mu_0(exp(sigma_xi) F),
       tau_xi/tau_0 = mu_0(exp(sigma_xi)).                  (H20)

Here mu_0 is the normalized positive real reference and sigma contains the full quadratic and V(Y^~) deformation. If ||sigma||_infty<=epsilon<log 2, then

       |tau_xi/tau_0-1| <= exp(epsilon)-1,
       |log(tau_xi/tau_0)|
          <= -log(2-exp(epsilon)).                         (H21)

These are quantitative bounds for the canonical relative response, irrespective of how small tau_0 is. They do not identify a different mass with the source mass, and they do not erase a current or native response of tau. The appropriate conditional/full-density bookkeeping must retain that response in whichever part of the C-05/C-06 interface actually contains the canonical mass. The operator estimate for Pi follows from the same formula and is proved separately in the primary analysis.

### 13.5 The positive majorant with an age reserve

For completed-hole old coefficients, retain the outer K_1 chain of Section 12 before localization-parameter Cauchy. On the true port just constructed, (H10)-(H11) apply. For reconstructed old add-backs, (H16) instead forces an exterior bridge. The full old physical connector crosses from that actual exterior owner to the attempted component; its birth-scale length pays the age cost. In the exceptional branch with all localization increments empty, terms wholly contained in one Z^~ enter the self action, as stated on pp.376-377. A nonself exceptional term must have an exterior carrier, and the same old connector pays the crossing. The cell convention matters here: Z is a union of compatible current cells, so the minimal current-cell cover of a fine-cell carrier contained in Z remains contained in Z. An exterior cell of Y_0 cannot be created merely by a face-touching cover convention. No K_1 difference is claimed in this all-empty branch.

The decay allocation can be made with fixed positive reserves. Let beta be a sufficiently small fixed fraction of the source's improvement parameter. For b<k the coarse-cover lemma gives the exact factor L^{k-b}; reserve the old beta*kappa tree factor in (1.66) in four positive shares for fine-carrier entropy, age, ports, and fixed polynomial losses. The remaining old-tree factor supplies the improved current connector because

       (1-beta)L >= 1+3 beta

after the source's fixed large L choice (or after reducing this reserve fraction). The genuinely retained K_1 kernel may be split into positive shares for the age path, the source first-nonempty spatial connection, and normalized row sums. Use a reduced fixed endpoint rate from CMP102 (190), including the block-local axial-gauge transfer; all such choices are independent of depth.

For clarity, the physical **pre-completion** output estimate, for the localization carrier Y_4 on p.376 before the last halo completion on p.377, has the form

       t_k(Y_4) <= L^{-(k-b)} t_b(input)
           + C(M_1/M) d_chain + C sum_i M^{-4}|Y'_i|
           + C(number of new incidence joins).              (H22)

The first term is the exact same-tree nested-cover inequality. The second follows because physical length on every grade r<=k, divided by M h_k, is at most (M_1/M) times its native scaled length. The third visits the current localization domains, whose components and overlaps are the ones specified in (1.61)-(1.64). The incidence joins use paid shared exterior cells. Thus one can retain this pre-completion carrier rate by choosing M/M_1 larger than the fixed connector coefficient divided by the reserved kernel rate, and kappa_1 larger than the fixed current-domain/tree and entropy constants. These are the existing source large-parameter choices, with stronger fixed inequalities. They do not change a coupling or a depth-dependent parameter.

At b=k, the ordinary-T input has (1+4 beta_source)kappa decay, explicitly stated before (1.66). This supplies its current output and finite port/cluster reserves; there is no old-age sum for that family. Newly produced coefficients are assigned the full invariant rate kappa. Unchanged old coefficients spend no reserve merely by being copied. Therefore a factor (1-beta) is not multiplied into the retained rate at each later operation.

On the source's common interpolation chart (1.65), normalized native derivative/Cauchy profile factors contribute the fixed polynomial (1+k-b)^s and any explicitly chosen fixed exponential profile rate Gamma_dom. With the true age reserve and the actual fine density, the completed-hole contribution satisfies

       C(1+k-b)^s L^{4(k-b)}
         exp[-(Gamma-Gamma_dom)(k-b)] A_b^*
       <= C exp[-lambda(k-1-b)] A_b^*,                     (H23)

provided Gamma-Gamma_dom>4 log L+lambda+2. The original h_{n'}^{-4} reconstruction density is paired with its native measure before this root count. The factor L^{4(k-b)} is the remaining actual count of birth roots in a current cell, not a second multiplication of a source sum already absorbed in a resummed coefficient. Interior history multiplicity is inside the normalized positive reference measure; it is not enumerated again as independent scalar labels.

### 13.6 Noncircular all-history induction

For each b, construct the actual coefficients by the source operations and decorate their carriers by the rules in Sections 13.1-13.3. The base has no omitted holes. The operation-by-operation argument proves the port and support class at generation b before taking its supremum. Let A_b^* be the rooted absolute norm at rate kappa, with (H17), supremized over these actual admitted depth-b histories and the stipulated native charts.

An old B_new^(b) in A'_k is a coefficient of an admitted depth-b truncation of the reconstructed external history. The established generation-b bound therefore applies. This does not assume the port property recursively: its membership follows from the exact deletion (H14)-(H16) and the previously constructed generation-b class. In particular, no new coarse anchor is substituted for an old consumed one.

Do not infer a globally linear dependence of the fresh output on its old norm from the first cluster expansion. The source (1.97) uses alpha^(1/3), and the second expansion can spend another fixed positive power. The appropriate induction is a closed-ball estimate.

Fix a finite A_*>0, and suppose

       Abar_{k-1}^* = sum_{b<k} exp[-lambda(k-1-b)] A_b^*
                    <= A_*.

Put K=F_0+A_*, where F_0 is the already controlled ordinary full-tree source allowance. Equations (H22)-(H23), together with the actual preparation/prefix majorant, bound the pre-completion positive sums by a finite constant depending only on K and the fixed parameters. **Assume here the final positive halo-completion transfer in Section 13.9.** Its final nonself small coefficient must have the form

       alpha_hat_k(K) <= C_K g_k^{-a}(1+ell_k)^p
                              exp[-c R_k],

with fixed a,p,c>0. All fixed positive roots spent in the two source expansions can be retained as one exponent a_0>0. Consequently their final fresh rooted majorant has a bound of the form

       A_k^* <= f_k(K),
       f_k(K) <= C_K [alpha_hat_k(K)]^{a_0},                (H24)

after the component incidence hypotheses are imposed. The statement only requires a fixed positive a_0; it does not replace alpha^(1/3) by alpha or assert an unproved Lipschitz estimate in K. Identical carrier labels are combined by absolute coefficient sums before spatial entropy is used.

There is no circular invocation of those incidence hypotheses. First work under the input bound Abar_{k-1}^*<=A_* and retain the **separate exact canonical self-deformation estimate** of (1.71)-(1.75) on the admitted chart, giving one fixed operator bound for each normalized kernel. The deliberately crude g_k^{-a} loss in the nonself age bound (H36) is not a replacement for that sharper self estimate: g_k^{-a}A_* alone would not tend to zero. The primitive incidence sums then tend uniformly to zero by alpha_hat_k(K) and the shell/incidence reserves. Reduce the common ceiling to meet the quantitative component criteria. Only afterward apply the two connected expansions and obtain (H24).

Because R_k>=ell_k^r with r>1, for fixed K one has sup_k f_k(K) tending to zero as the common coupling ceiling tends to zero, despite every displayed fixed inverse power of g and logarithmic prefactor. Choose the ceiling so that

       sup_k f_k(F_0+A_*) <= (1-exp[-lambda]) A_*/2.

Then the exact carried identity gives

       Abar_k^* = exp[-lambda] Abar_{k-1}^* + A_k^*
                <= (1+exp[-lambda]) A_*/2 < A_*.

With a base generation bounded by A_*, this proves the stated **conditional** uniform closed-ball invariance. It is a valid nonlinear induction; no global linear contraction of the fresh coefficient map is asserted. Its application to the actual current route requires the positive halo-completion transfer as well as the composed-scalar/native-chart interface discussed next. Once both hold, the component-root bound feeds the current-root estimate through the actual current localization maps and normalized-operator derivative layers, as specified in the separate primary analysis.

### 13.7 Exact remaining interfaces and scope

The purely native part of the full C-05 statement is a further issue. A bound for the current-anchored scalar B(z,xi)-B(0,xi), even with arbitrarily many mixed native derivatives, does not bound the unsubtracted B(0,xi). The present scalar history argument and canonical relative-kernel estimates do not license dropping that term. C-05 remains open unless the unsubtracted native-rooted activity bound is independently supplied on the actual native footprint system. This limitation is separate from the repeated-component age/root repair.

### 13.8 The composed scalar row: the precise predecessor invocation

**Restricted scope; see Section 13.10.** The directional AD17 statement cited here is valid, but H25-H28 must not be applied to arbitrary data in the localized alpha_s norm when the localized determining history refines the original output grading in C_1. Section 13.10 supplies the whole-carrier near/far argument, uses an absolute input row only in the unchanged-output region, and keeps its fixed g_k^{-a} prefactor. That is the composed-scalar argument used here.

Let v be a variation of the determining data in (1.61), supported on C_1, measured by the dimensionless running radius alpha_s at its actual input grade s. On the common smaller (1.65) chart, the Landau representation of CMP102 (190) yields, for each of its normalized field, gradient, and current rows at output grade n,

       normalized |D U_Lv|
       <= C integral_{C_1} [alpha_s/alpha_n]
                    exp[-delta d(x,y)]
                    [|v(y)|/alpha_s] d nu(y).              (H25)

Here delta is a positive reduced share of delta_0/8, and d nu includes the actual determining-data measure canceling h_s^{-4}. This is an operator row, not a sum of counting-matrix entries over fine bonds. The source AF comparison bounds alpha_s/alpha_n by a fixed polynomial in 1+(s-n)_+. For s<n the running profile is monotone at a sufficiently small common ceiling; for s>=n, JI.35 uses the explicit square-root bound. The admitted source grade-distance estimate absorbs this fixed polynomial in a reserved share of exp[-delta d]. Reserving a further share for the row sum gives

       normalized |D U_Lv|
           <= C ||v||_alpha exp[-delta_1 d(x,C_1)].         (H26)

For an older primitive's innermost region, its birth-grade weight is no larger than the corresponding coarser-output estimate after the physical h_b/h_n factors are included; these are exactly the common profile comparisons in BC16.21-BC16.23. No raw unit fine-link direction is treated as normalized.

The actual normalized inverse-gauge row RM.36 has the unambiguous form

       |u^{-1} D u|(x) <= C h_n sup_{Delta_n(x)} |D A_L|.

The actual terminal block and its fixed transport dependency neighborhood have bounded diameter in the scaled metric. Applying (H26) gives the same endpoint exponential for this fine gauge. JI.38 retains the fixed real reference factor, so this is the converter of the actual selected source family, not an independently chosen axial representative.

Apply AD17.26-AD17.27 to this family with the parameter direction v. Its proof is an analytic directional chain rule; it is not specific to the name of a current coordinate. The nodal interpolation matches the converter at all old fluctuation basepoints and, by CR.2, at both endpoints of every retained raw bond. Consequently the earlier fields remain the original fixed real arguments. The strong relative field/gradient/curl-current tangent satisfies

       ||D Phi_X[v]||_native
           <= C ||v||_alpha exp[-delta_2 d(X^+,C_1)],       (H27)

where X^+ is a fixed birth-scale collar and the interpolation supports have bounded overlap. The physical current row follows from exact current covariance as in AD17.27, not from a third derivative of an axial gauge potential. The independent-current slot is transformed by the same actual converter.

NP.5 and AD17.28 put this family in a genuine primitive native ball and retain an affine disc of a fixed radius r_nat/2. Cauchy on that disc therefore proves, for the actual primitive scalar E_X with fixed earlier arguments,

       |D(E_X composed with Phi_X)[v]|
         <= C ||E_X|| ||v||_alpha
                    exp[-delta_2 d(X^+,C_1)].              (H28)

This is the desired composed DE*K_1 estimate. It is not an assertion that the axial potential itself obeys the strong native norm. The collar enlargement in X^+ is paid by a fixed carrier/port reserve. Every radius and conversion constant in this predecessor application is independent of k-b. Thus it introduces no exponential domain-loss rate: Gamma_dom=0 for this admitted scalar family. Fixed polynomial factors from other explicitly retained source comparisons may still be included in s in (H23), and are absorbed by the unused age exponent.

For i_0=3 or 4, the boundary-data maps and K_2,K_3 are composed before (H28); their normalized rows on the same (1.65) family have uniform constants after the same AF/row reserve. K_1 and its input support C_1 remain, by the exact chain in Section 12.1. Integrate (H28) along the actual determining-data interpolation to get a scalar **value** bound; only then apply the source localization-parameter Cauchy estimates. Those estimates spend their explicit localization-volume/walk factors, not a new age-dependent native radius.

This predecessor invocation has a precise scope requirement: the localization family must be the actual (1.61)-(1.64) family on (1.65), with the selected source gauge and the retained variables used in AD17/CR.2. It does not admit an unmatched new decoupling family, a different axial convention, arbitrary moving raw data, or a pure-native unanchored perturbation. Subject to that already specified family, (H25)-(H28) supply the quantitative composed-scalar interface needed by (H23), rather than leaving Gamma_dom as an arbitrary unspecified constant.

### 13.9 A two-majorant lemma and the exact final-halo transfer still required

The following elementary lemma combines an age estimate with a final-halo estimate without pretending that the pre-carrier already paid the added halo cells.

**Lemma (positive-majorant interpolation).** Fix a finite cutoff, a birth b, and a root r. Let E_{b,r} be a finite or countable family of actual final carrier/occurrence labels. Let mu_e>=0 be their genuine combinatorial weights, p_e>=0 their positive analytic majorants, t_e>=0 the final full physical connector length, and u_e>=0 any further desired incidence factor. For 0<theta<1 and K>0, set kappa=theta K and suppose

       H_b(r) = sum_e mu_e p_e u_e^(1/theta) exp[K t_e]
                    < infinity,
       Q_b(r) = sum_e mu_e p_e < infinity.

Then

       sum_e mu_e p_e u_e exp[kappa t_e]
          <= H_b(r)^theta Q_b(r)^(1-theta).                (H29)

**Proof.** For a finite subfamily write each summand as the product of

       [mu_e p_e u_e^(1/theta) exp[K t_e]]^theta
       [mu_e p_e]^(1-theta)

and apply Holder with exponents 1/theta and 1/(1-theta). Increasing finite subfamilies gives the countable statement by monotone convergence. Integrals over real hidden variables are included by the same proof on their actual positive reference measure. No cancellation is used, and no new independent measure is assigned to a historical component. The usual 1/q! occurrence factors may be included in mu_e. QED.

For example, if H_b(r)<=H(K_*) uniformly on an input ball of size K_* and

       Q_b(r) <= C (1+n)^s L^{4n} exp[-Gamma n] A_b^*,
       n=k-b,

then (H29) leaves the rate (1-theta)(Gamma-4 log L) and the power (A_b^*)^(1-theta). To sum births, put a_b=exp[-lambda n] A_b^*. If sum_b a_b<=A_*, another application of Holder gives

       sum_b (1+n)^{s(1-theta)}
          exp[-(1-theta)(Gamma-4 log L-lambda)n]
          a_b^(1-theta)
       <= A_*^(1-theta)
          [sum_{n>=0}(1+n)^{s(1-theta)/theta}
           exp[-((1-theta)/theta)(Gamma-4 log L-lambda)n]]^theta.
                                                               (H30)

The last series is finite when Gamma>4 log L+lambda. A strict extra reserve gives any smaller desired output age rate. The interpolation changes only fixed fractions of the spatial and age rates and fixed positive powers of small amplitudes. These losses fit the closed-ball induction; no global linearity is required.

The important source-matching condition is that H_b and Q_b bound the **same positive birth-resolved coefficients**. A bound for the norm of a signed sum V(Y) does not automatically bound the sum of the absolute birth-resolved contributions. Nor may a final (1.68) proved under the original full-tree input simply be relabeled as a theorem for arbitrary strengthened tagged input.

For the present repair, the remaining final-halo statement can be formulated precisely as follows:

> **FH.** On a fixed input ball Abar<=A_*, perform the literal localization and last resummation of LFR II pp.376-377, retaining the positive absolute majorants and the old birth label until the majorant is summed. All old bounded completed components inside attempted Z are already part of the self/nonself completed operation; old completed components outside Z remain declared physical holes with their positive halos. The resulting final coefficients satisfy a rooted bound H_b(r) of the type in (H29), with the final connector visiting every required cell outside those old holes and the current attempted holes, and with enough fixed reserve to pay u_e^(1/theta). Its constants and small coefficient must be uniform in the actual external history, cutoff, depth, old births, and the number of hidden internal histories, with the input dependence permitted to be a finite function of F_0+A_*.

The shell, port, common-halo, and exact same-tree cover lemmas establish the geometry needed for FH. Source (1.68) establishes its unstrengthened native final-halo analogue; source pp.391-392 establishes the alternative scalar representation at its stated inductive scope. These notes have **not yet supplied a complete term-by-term proof that the source's final halo-completion estimate persists in the positive birth-resolved form FH for every mixed old-hole input outside Z**. This is the narrow remaining fresh-majorant transfer, not a failure of the external-history deletion or true-port lemma.

Consequently the status is: the coarse-volume age argument, which is invalid, has a source-based replacement through the always-retained K_1 and actual true ports; the final weighted scalar recurrence is a proved implication of FH, with an explicit closed-ball induction; FH itself remains to be checked at the source's final completion step. The independent unsubtracted native-rooted C-05 requirement remains open as described above. This note alone does not change the status of C-05.

### 13.10 Whole-carrier split for the scalar K_1 row

This subsection addresses the localized-history refinement problem explicitly. It replaces the overly broad arbitrary-data formulation in Section 13.8.

Work on the declared common **strong core** supplied by the AO-AR/PF predecessor charts, simultaneously with the source localization parameters. CMP116 (1.11), (1.18) has the fixed localization enlargement e^{16 kappa_1}; choose the auxiliary native radius after that fixed constant, then use q>p_0+r+2 and the common coupling ceiling to pay the prefix real-center enhancement while retaining the physical current contour. This costs a fixed radius, not a factor shrinking with k-b. PF.1 gives strong-core inclusion in the modified source domain; it does not identify every point of that entire modified domain with a point of NP.5's fixed ball. The latter broader assertion is neither needed nor made here.

Let X^+ contain the old primitive carrier and the fixed dependency collars needed for its old-node interpolation and local stencils. Use the actual source determining blocks in defining the enlarged outer collar of the attempted Z. The enlargement includes the incident determining blocks at C_1 and its fixed stencils. It can remove only a fixed number of complete top-scale prepared collars from a path to the outer boundary; it is not a contraction of the attempted component.

**Near/bridge case.** Suppose X^+ reaches that outer collar or the exterior of Z. A true resident port lies in an actual completed component of birth at most b. Its old connected physical tree reaches the selected point of X^+, up to the fixed paid port/collar cost. Hence the tree alone crosses the prepared grades through k-O(1), and

       t_b^bullet(X) >= c(k-b)-C.

For a reconstructed old add-back this conclusion instead follows from its actual exterior owner and (H16). Use directly the scalar value bound on the source (1.65) interpolation family:

       ||E_X(Phi_1)-E_X(Phi_0)|| <= 2 ||E_X||.              (H31)

The reserved old-tree factor supplies the full age decay in this case. There is no invocation of a refined-output derivative row, no independent fine-data perturbation, and no claim that an axial potential satisfies the old strong norm. The subsequent source localization Cauchy argument is applied to this already suppressed holomorphic value bound.

**Interior/core case.** Otherwise the whole primitive dependency collar lies inside the attempted component and away from the localized-history disagreement. On these output points B''_k(Y_1) equals B''_k. Preparation only coarsens the original grading there: if i is the primitive's original native output grade and n its prepared grade, then i<=n. The primitive's inner-region convention also caps i at its birth b. There is no artificial refinement of the output in this case.

The exact C_1 data family lies on the fixed absolute determining-data chart used in CMP102 Proposition 9 and LFR II (1.65), restricted to that common strong core. The relative data increment, including its displayed splice gauge and averaging factors, has a fixed absolute dimensionless bound. Use the **absolute** normalized row (190), pairing h_s^{-4} with its actual source measure. CMP96 Lemma 2.1, (2.59)-(2.61), supplies the absolute native-center exponential row sum on the admitted geometry. This gives each smooth output row, of physical order p=1,2,3,

       h_n^p |D output_p(x)|
          <= C exp[-delta d(x,C_1)],                       (H32)

up to fixed constants for the finite intermediate map chain. No alpha_s input assumption is needed. Since x is inside Z, LFR I (1.47) gives

       d(x,C_1) >= c(M/M_1)(k-n-c_0)_+-C.                 (H33)

Converting (H32) to the old primitive native normalization multiplies it by alpha_i^{-1}(h_i/h_n)^p. The admitted AF comparison gives, for a fixed exponent s_0,

       alpha_i^{-1}(h_i/h_n)^p
          <= C g_k^{-1}(1+k-i)^{s_0} L^{-p(n-i)}
          <= C_p g_k^{-1}(1+k-n)^{s_0}.                    (H34)

The second inequality uses i<=n, p>=1, and the finite supremum of (1+n-i)^{s_0}L^{-p(n-i)}. The fixed polynomial in k-n is paid by a reserved share of (H33). The harmless fixed inverse power of g_k is retained in the fresh coefficient; it must not be omitted or called a uniform constant. The finitely many map/profile conversions can increase this to g_k^{-a} for one fixed a, which is allowed by (H24).

For the actual fixed-old-variable gauge correction, the old nodes in this interior case have the required native meshes. Recent old A_j in the integrated preparation collars have been integrated out. For the borderline surviving A_{h-1}, its actual support is Omega_h intersection Z_h. Because Z_h=Z_h'' subset Z_{h+1}'', it remains outside Omega_{h+1}'' and has terminal grade at most h, up to the fixed endpoint convention. Its node grid h_{h-1} therefore differs by at most a fixed number of levels. Deeper old adjoint nodes remain in unchanged deep grades. Surviving raw endpoints retain the actual one-sided grade relation used in CR.2.

CMP102 Proposition 2, p.281, treats the nonzero corrected fiber Q(U_0,eta A)=B with the same terminal normalization R_0u_j=1. The normalized inverse-gauge formulas RM.26-RM.36 are algebraic in that normalization and do not assume B=0. Thus they apply to this actual K_1 relative family with its fixed real reference. The argument does not replace K_1 by an unrelated localized H_i(s) formal extension. Its fine gauge row, followed by the actual old-node interpolation AD17.26-AD17.28, transfers the smooth rows (H32)-(H34) to the scalar with the original old variables fixed. At those old nodes the grade discrepancy is fixed, so there is no missing h_i/h_n factor in a nodal gauge value.

If the prepared output grade n exceeds the scalar birth b, the old connector from its true port to that output pays the remaining grades b through n; if n<=b, (H33) already pays k-b. Therefore

       kappa_res t_b^bullet + delta_res d(x,C_1)
                    >= Gamma(k-b)-C                      (H35)

with independently reserved positive shares. Apply the genuine native directional Cauchy disc from NP.5/AD17.28 to the composed scalar, integrate the actual selective interpolation, and only then take the source localization-parameter Cauchy estimates. This gives the corrected scalar value gain

       ||Delta E_X|| <= C g_k^{-a}(1+k-b)^s
                    exp[-Gamma(k-b)]
                    (remaining old carrier majorant).     (H36)

The first nonempty localization may be 2, 3, or 4: the K_1 factor remains in every interior case by Section 12.1; the finite intermediate absolute rows change only the fixed a,s,C. The all-empty branch is treated by the scalar near/bridge/self classification in Section 13.5.

The quantitative conclusion is therefore an age gain with a displayed fixed inverse-coupling prefactor, not a generic arbitrary refined-data tangent theorem. Together with the actual L^{4(k-b)} root density, it gives (H23) after a strict age reserve and the corresponding enlargement of the fresh g_k^{-a} prefactor. This resolves the specific graded-output mismatch in H25; it does not prove the distinct final-halo positive-majorant transfer FH.

## 14. A weaker quotient norm: what the new grade lemma does prove

The stronger full-halo-visiting norm is not essential to the new age argument. It may be preferable to finish the source transfer in the original CR quotient/outside norm instead. This section states exactly how far that alternative can presently be justified.

### 14.1 Zero jumps in true old components do not erase newer grades

Let a birth-b carrier have a quotient connecting tree in which traversal of each **actual surviving completed component** H_m, m<=b, has zero cost. Keep the actual physical components; do not replace them by arbitrary later coarse covers or enlarged current components before the nonself estimate. By (H13), every point of H_m is outside Omega_{m+1}, hence has native grade at most m. In an eligible attempted component, m<=h and the preparation retains that low-grade region as proved in Section 13.2.

Take a quotient-tree path from a genuine resident component to an output x, followed by the actual K_1 path to C_1. Replace each zero jump inside H_m by an arbitrary physical path inside H_m. The replacement exists because the eligible component is connected. Every point on that replacement has grade at most b. Consequently no grade-r crossing with r>b is supplied by a zero jump. All the higher-grade annular crossings are on either the charged exterior tree or the K_1 path.

Thus the same annular ledger gives

       C(M/M_1) ell_b(X) + d(x,C_1)
             >= c(M/M_1)(k-b-c_0)_+-C,                    (H37)

where ell_b is the quotient/outside connecting length. No interior-port payment and no R^3 shell lower bound is needed for this inequality. The near/bridge alternative in Section 13.10 also works: the charged exterior portions of a path from a true low-grade component to the attempted outer boundary pay every newer grade. The whole-component containment rule excludes a surviving old component that straddles that boundary.

This is a substantive repair of the original age mechanism: it shows precisely why contraction of a true old component cannot remove a newer native grade. It does not apply to a promoted artificial tag containing current high-grade points, nor does it assign the old grade to a component that has already been consumed.

### 14.2 Physical diameter and decorated halos

For the actual separated core components, the original CR.1 argument remains valid:

       diam_phys X <= C [M h_b(ell_b(X)+1)+s_max],           (H38)

with s_max the largest physical component size. Charge each traversed core diameter, except one, to the preceding exterior gap using relative separation. The current shielding collar pays the remaining largest diameter in the physical current-root theorem. This is compatible with the two-root KP/operator formulation.

A deterministic halo can instead be recorded as a fixed **support footprint** D(H), with diam D(H)<=C diam H, while the quotient metric continues to collapse only H itself. The diameter of the union of the footprints then differs from that of its cores and active cells by at most a fixed multiple of the largest footprint diameter. This bookkeeping does not require a tree to visit every added halo cube. It is geometrically a sufficient alternative to the stronger full-halo-visiting invariant.

However, making every enlarged halo a zero-cost region is not justified by core separation alone. For example, equal boxes of diameter D with gaps epsilon D are relatively separated; halos expanded by more than epsilon D/2 overlap along an arbitrarily long chain. Collapsing their union permits a zero-cost traversal of diameter of order nD, which cannot be paid by a single largest-component term in (H38). The exact source construction may supply additional separation in a particular case, but it must be proved. Fixed support decoration and free traversal are different operations.

### 14.3 The remaining positive pushforward in the weaker norm

The sufficient weaker replacement for FH is concrete. Retain a positive atomic decomposition before the last support saturation on pp.376-377, with each atom carrying:

* its genuinely variable exterior-cell carrier;
* the actual component slots it uses;
* fixed halo support footprints for the normalized kernels and completed outputs;
* its birth label until the positive age sum has been performed.

Prove that the source's final resummation and both connected expansions push these atoms forward with a uniformly small component-root norm and a fixed-current-root norm in the quotient metric, charging footprint diameters by (H38) and the current collar. Identical deterministic halo labels must not create domain entropy; any edge introduced by overlap of different support footprints must either be absent from the actual dependence graph or carry its genuine exterior/diameter payment. The canonical masses and their actual operator layers remain those of (1.71)-(1.75).

The new source-history deletion and (H37) remove the false native-grade assumption from this route. They do not, by themselves, prove the stated positive pushforward. The final coefficient's dependence on its whole normalized-kernel footprint cannot simply be discarded by relabeling the footprint as decoration. Likewise one cannot identify a positive birth-resolved atom sum with a signed final coefficient bound without justification.

Accordingly, a complete positive pushforward in this weaker norm would avoid the excessive R^3 demand of FH and would suffice for the current route. It is a viable, narrower alternative, but it has not been completed in this note. The final status is unchanged: actual history/grade structure and the restricted scalar K_1 age channel are established; the final strengthened or weaker positive scalar transfer and the unsubtracted pure-native clause of C-05 remain open.
