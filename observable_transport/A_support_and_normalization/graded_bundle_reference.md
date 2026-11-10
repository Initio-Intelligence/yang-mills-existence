# One graded bundle reference for the mixed determining geometry

This note constructs a single local reference on the scale-separated mixed determining geometry. The two-level lemma MI.1 is used to estimate local loops, not iterated to construct the field. Thus its constants are paid once on each bounded star. The projection, SU reduction and complex comparison are the explicit formulas of BR.1.

The asserted input is the actual regular determining data on the source support, including its regular fine boundary collar. Arbitrary exterior specified values beyond that support are copied exactly; they are not required to satisfy a new small-field condition. The full old Schur/coarea/cross conditional density and the microscopic marked budget remain separate problems.

## 1. Geometry, locality scale, and source admission

Use microscopic mesh η and let `ℓ_j=L^jη`. The nested domains have the source block alignment and separation

\[
 \operatorname{dist}(\Omega_j^c,\Omega_{j+1})
       \ge R M_1\ell_j.
 \tag{GR.1}
\]

The determining sets are the literal source sets, with the site and bond conventions applied separately,

\[
 \Gamma_0=\Omega_1^c,\qquad
 \Gamma_j=\Omega_j^{(j)}\setminus\Omega_{j+1}^{(j)},
 \qquad \Gamma_k=\Omega_k^{(k)}.
 \tag{GR.2}
\]

See CMP96 p.224 (2.1)–(2.4), CMP102 (1), and CMP119 p.255 (2.2). A bond belongs to the lower shell only when it is not a bond of the next domain. Therefore no lower determining bond touching that next domain is prescribed. The endpoints of a higher crossing bond outside its own domain belong to the immediately lower determining grid, on the bounded neighborhoods used below.

Fix all geometric construction constants first. The source separation is taken larger than `C_*L`, where `C_*` is the fixed largest relative halo needed for the graph paths, partitions and averaging stencils below. This is a further finite choice of the source localization constants, independent of depth, coupling and volume. It is not an age-dependent separation requirement.

The consequence used repeatedly is this: every such local halo at its largest mesh sees at most two adjacent determining levels. It cannot meet both boundary components of an intervening shell, since (GR.1) separates them by more than the halo diameter. An outer interface of a j-scale patch meets level `j−1`, not an arbitrarily fine level. This is the same geometric fact behind the two-shell regularity cubes in CMP102 p.279.

The data are regular in the source sense on the support of the determining set: the mixed plaquette expression (7) of CMP102 is small. At a missing higher bond this expression uses the actual average of lower data. The primitive data on the fine exterior collar are also regular. CMP119 p.255 defines the support as `Ω_1` with a small `M_1`-cube neighborhood; p.256 specifies regular determining data for the variational map. Far exterior values that do not enter this support are not included in this regularity assertion. The first-step geometric buffer is explicit in (1.10).

For exposition use one uniform small ε. Bounds with scale-dependent ceilings use their maximum on the two adjacent levels of each local halo. The source adjacent-scale estimates (2.6)–(2.9) give a fixed comparison of those ceilings. No product over the number of levels is taken.

## 2. The mixed edge graph and its exact transports

Start with the geometric straight segments of all determining bonds and all their endpoints. A higher determining edge can overlap a chain of lower determining edges only on its outer part: its inner endpoint lies in a higher block, where those lower bonds are not prescribed. The source separation ensures that this lower chain is on the immediately preceding grid.

Subdivide every higher edge at the lower determining vertices on that outer part. Keep each lower subedge with its given matrix. The remaining inner connector has no prescribed lower matrix. Assign its transport as the quotient which makes the product along the whole original higher edge equal to its given matrix. For example, if the original edge runs from the inner endpoint i to the outer endpoint j, and its outer lower chain from x to j has transport `h_{xj}`, assign

\[
 u_{ix}=V_{ij}h_{xj}^{-1}.
 \tag{GR.3}
\]

Reverse orientations use inverses. There is one free connector on such an edge. If both endpoints are in the higher domain, the edge has no lower determining vertices in its interior and is kept unchanged.

These assignments are consistent. The free inner portions of two distinct determining edges have no overlapping segment. Their intersections are endpoints; any intersection with a lower determining vertex was already subdivided. The block alignment gives these facts directly: the inner half of a crossing edge lies in its inner endpoint block, while lower determining vertices lie outside that block union. The outside part is a chain of the actual lower edges. No matrix is assigned twice with inconsistent values.

The resulting graph has uniformly bounded degree, with constants depending on L and dimension. Near a transition its edge lengths are comparable to either of the two adjacent meshes, with fixed ratio bounds depending on L. The product on every original determining edge is exactly the given V. All subedge transports are unitary, determinant one, and covariant under independent gauge transformations at the mixed determining vertices. For (GR.3), covariance follows by canceling the gauge at j between the two factors.

Every graph vertex is an actual determining vertex; no field-dependent auxiliary frame is introduced. Its assigned mesh is the level of its determining shell. For cover construction enlarge that mesh, if necessary, to the largest length of an incident graph edge. This changes it by at most a fixed L-dependent factor.

## 3. Uniform local connectivity and small loop defects

There are short graph paths between nearby vertices in an overlapping star. One concrete way to see the uniform bound is to work at the larger of the two local meshes. A lower vertex is connected to the center of its outside larger block by a lower-grid path. Adjacent larger centers are connected either by their higher edge/connector chain or, when both are outside the higher domain, by the lower straight chain. A bounded number of these moves joins the vertices. Thus the path stays in a fixed halo and uses at most `C_L` graph edges. Choose one such path deterministically from the geometry; use its reverse for the reverse pair and use the single graph edge for actual neighboring endpoints.

Let `g_ab` denote these path transports. They are local analytic functions of the raw mixed data. To estimate a triangle of such paths, its full halo has only one adjacent-scale interface. Apply the construction of MI.1 on that halo to obtain its auxiliary field W on the lower of the two grids. This is a comparison field only.

On every lower graph edge, W agrees with its given value exactly. On an original higher edge, the W straight transport differs from the prescribed value by `C_Lε`: MI.4–MI.5 compare W to the step lift, whose higher straight transport is exact. On a connector, cancel the identical outer lower chain in this comparison; its error is again `C_Lε`.

Consequently each chosen bounded graph path differs from the corresponding W path by `C_Lε`. A loop of those W paths is contained in a fixed lower-grid box with a bounded number of elementary plaquettes; MI.6 bounds every such plaquette. Therefore

\[
 \|g_{ab}g_{bc}-g_{ac}\|\le C_L\varepsilon.
 \tag{GR.4}
\]

More precisely the right side is bounded by a fixed sum of the actual mixed plaquette defects and the lower plaquette defects in that halo. The comparison is invariant under the local block gauge used in MI.1. It is not an assumption that the three given higher averages were straight transports.

The finite local graph also admits a coarse axial gauge making all its bounded path transports `I+O(C_Lε)`. To construct it, select one root and transports from that root along the same bounded graph paths. Equation (GR.4), or the corresponding loop filling just proved, bounds the remaining edges. This gauge is only used in norm estimates and has a fixed local footprint.

## 4. A smooth graded partition with the exact graph-edge property

The projection requires smooth nonnegative weights `w_a` such that `Σw_a²=1`, with only the two endpoint weights nonzero on a graph edge. The following explicit construction supplies them.

Choose a smooth geometric vertex bump `b_a`, positive on a ball covering every incident edge and the block belonging to a, supported in a fixed larger ball of radius `C r_a`, where `r_a` is the enlarged local mesh from Section 2. Such balls have bounded overlap: a local halo contains at most two adjacent meshes, so it contains at most a fixed number of determining vertices after rescaling by its smallest mesh.

For each vertex a, multiply its bump by the following finite collection of factors:

- A smooth nonnegative factor vanishing exactly at every other graph vertex in its enlarged support.
- A smooth nonnegative factor vanishing exactly on every nearby graph edge not incident to a.

All these factors are positive away from their stated zero set, flat there, and equal to one outside a fixed neighborhood. They can be written explicitly. For a vertex use a smooth flat function of its squared distance. For an axis-parallel segment `e=[c,d]`, use a smooth nonnegative defining function

\[
 q_e(x)=|x_\perp-c_\perp|^2+
ho(c_\parallel-x_\parallel)^2
                         +\rho(x_\parallel-d_\parallel)^2,
 \tag{GR.5}
\]

where `ρ(t)=0` for `t≤0`, is positive for `t>0`, is smooth and flat at zero, and is rescaled by the local mesh. This function vanishes precisely on e. Composing it with another smooth flat function gives the required factor. Only the finitely many vertices and edges meeting the chosen enlarged support enter. Call the resulting product `φ_a`.

The sum `Σφ_a²` is positive everywhere on the region covered by these stars. Off the graph all its factors are positive for a covering bump. On the interior of an edge, the endpoint bumps are positive and no nonincident edge crosses that point. At a vertex a, only `φ_a` survives and it is positive; all edges through that point are incident to a, since subdivision was performed first. Set

\[
 w_a=\phi_a\bigl(\sum_b\phi_b^2\bigr)^{-1/2}.
 \tag{GR.6}
\]

The weights are smooth, have the desired edge and vertex properties, and have bounded overlap. The denominator and derivative bounds are uniform, not merely positive separately in each volume. After translating and rescaling any local halo by its smaller mesh, all vertex and edge positions lie in a bounded subset of the fixed L-grid; only finitely many two-level geometric patterns can occur. On each such compact pattern the denominator is positive by the preceding argument. Its minimum over this finite collection is therefore a fixed positive number. It follows that

\[
 \sum_a|\partial^q w_a(x)|\le C_q h(x)^{-q},
 \tag{GR.7}
\]

where h is either of the two comparable local meshes, after changing the fixed L-dependent constant. These constants can be large, but are independent of depth and volume. They are chosen before the small-field ceiling.

This construction imposes the exact edge condition; ordinary unrestricted smooth vertex bumps would not suffice.

## 5. One projection, one SU connection

Use the same formulas as BR.1, now with the mixed vertices and weights:

\[
 P_{ab}(x)=w_a(x)g_{ab}w_b(x),\qquad
 \Pi=\frac{1}{2\pi i}\oint_{|z-1|=1/4}(z-P)^{-1}dz.
 \tag{GR.8}
\]

Only a bounded number of local rows is active. Equations (GR.4) and (GR.7) give

\[
 \|\partial^q(P^2-P)\|\le C_q\varepsilon h^{-q}.
 \tag{GR.9}
\]

The local gauge comparison makes P close to `ww^T⊗I`; hence Π has rank N and the uniform spectral gap required by the fixed contour. Use BR.11–BR.20 to define the dual frames, exact SU transition functions and traceless connection. The proofs there are finite local algebra and apply without alteration. The flat comparison cancels the order-one partition derivatives, yielding

\[
 |F|\le C\varepsilon h^{-2},\qquad
 |\nabla^q F|\le C_q\varepsilon h^{-q-2}.
 \tag{GR.10}
\]

At every mixed vertex a the canonical frame is its fixed inclusion `e_a`. Along a subdivided graph edge only the endpoint weights survive, so BR.22 gives exactly its prescribed graph transport. The product along every original determining edge is therefore its original V, including the higher edge subdivided in Section 2.

No successive interpolation was performed. The same projection (GR.8) covers all scales, and every estimate uses a local pattern with at most two levels. In particular there is no factor `C_L^k`.

Define the microscopic link field by fine parallel transport in geometrically selected local frames. Its actual footprint is the fixed local graph halo met by that segment. It is a function of raw determining entries at their true levels, not of an independently variable global background.

## 6. The actual mixed regularity and averaged-data conditions

For a microscopic plaquette belonging to `Ω_j`, every local mesh entering its halo is at least `ℓ_{j−1}`. By (GR.10),

\[
 \|U_{\rm ref}(\partial p)-I\|
      \le C_L\varepsilon\eta^2\ell_j^{-2},\qquad
 \|D^*\partial U_{\rm ref}\|
      \le C_L\varepsilon\eta^3\ell_j^{-3}.
 \tag{GR.11}
\]

The possible factors `L²,L³` arise only from one adjacent outer level. Deeper inner levels give stronger bounds. These are the source regularity conditions (2) with a fixed constant.

For an original determining bond c at level j, the full footprint of the j-fold averaging lies in its two endpoint j-blocks. The source separation puts this footprint and its fixed halo in levels at least `j−1`. Thus (GR.11), with its fixed L-dependent constant, holds throughout that averaging footprint. The recurrence BR.24–BR.26 applies there after rescaling by `ℓ_j`, while the connection's straight transport along c is exactly V_c. Therefore

\[
 \|\mathcal M^j(U_{\rm ref})_c-V_c\|
       \le C_L\varepsilon,
 \qquad c\in\Gamma_j.
 \tag{GR.12}
\]

For `j=0` this is equality, not merely an estimate: each prescribed fine edge is itself a graph edge. This supplies CMP102 (14) on the actual mixed determining support.

The reference's normalized Wilson force is also `O(ε)` in the mixed source norm, by (GR.11) and its next fixed covariant difference. Its precise dependence is local in the raw mixed data. The actual force term is retained in the variational equation.

## 7. The fine exterior and exact specified entries

The source support is `Ω_1` with its stated regular fine collar. Construct the bundle connection only on that support, enlarging the fixed collar by the construction halo within the admitted regular buffer. Include every fine vertex and edge of `Γ_0` met by this collar. Their interpolated link transports equal the original prescribed fine matrices exactly.

Outside this collar set `U_ref=V_0` on the specified fine edges, without any projection. On the overlap the two definitions agree edge by edge, because the interpolation already reproduces those very fine edges. Hence no smoothing seam or artificial small-curvature requirement is introduced into the distant specified field.

The microscopic edges touching the active regular domain are defined by the connection and have the bounds (GR.11). The specified values farther away do not enter the variational minimum's local support, except as the unchanged additive exterior part of its action. This distinguishes the regular `Γ_0` support collar from arbitrary specified variables beyond that support. The latter are not an obstruction to the construction and are not claimed to be regular.

## 8. Native complex coordinates and the mixed fixed point

The graph transports, the dual frames and every matrix function are holomorphic in the raw complexified determining entries on a uniform local domain. Their coefficients are evaluated on bounded graph halos, so their raw coordinate counts per halo are bounded by the fixed L-dependent geometric constants.

For two nearby admitted raw data sets apply the local Kato formula BR.28 to their graded projections, then correct the small determinant as in BR Section 8. It is identity at **every mixed determining vertex**, since the projection there is the same fixed `e_a e_a*`. The connection difference satisfies the scale-weighted bounds

\[
 |a'-a|\le C\delta h^{-1},\qquad
 |\nabla(a'-a)|\le C\delta h^{-2},
 \tag{GR.13}
\]

and the corresponding fixed higher bounds. The induced fine gauge is local and fixes all determining vertices. Thus this comparison lies in the actual mixed native complex field domain; it does not produce a spurious `η^{-1}` loss at an interface. If the fine specified entries are held fixed, their interpolated values are held fixed exactly as well.

Use this reference, its actual force J, and its actual mismatch fields in CMP102 (111)–(121), or the equivalent source equations with the required gauge condition retained. Their primitive nonlinear maps are local at their native mixed scales. Every primitive propagator coefficient depends on the reference restricted to its full source domain; composition with (GR.8) enlarges it by only the fixed graded halo.

The generalized mixed-scale walks of CMP99 and the CMP116 decoupling procedure therefore give a common raw-determining family. Source buffers are chosen larger than the added local halo. Setting the decouplers outside a component to zero separates the equations exactly. The force-containing contraction is uniform after fixing the enlarged parameter radius and then choosing the geometric ceiling ε. Cauchy and connected-set counting give actual raw-determining carrier coefficients, as in BR Section 9. Their native physical footprints must still be converted and counted in the particular M-03 current-scale application.

### Theorem GR.1

On the actual scale-separated, regular mixed determining support, with the fixed construction collars admitted as above, there is a single raw-local regular reference satisfying CMP102 (14) and preserving every specified fine determining entry exactly. Its constants are independent of the number of scales, and its native complex comparison is local and center-fixed. The force-containing source fixed point consequently has genuine raw-determining component expansions. No recursive loss in depth and no global gauge are used.

This theorem concerns the primitive variational map. It is not a completed estimate for an old conditional quotient. The actual full old precision, determinant/coarea and cross factors, their small relative comparison to a bounded-core reference, the current physical carrier cost and the incoming marked transport budget must still be verified in that application.

## Mathematical sources

- CMP96 (1984), p.224, (2.1)–(2.4): determining shells as site and bond sets and scale separation.
- CMP102 (1985), pp.277–280, (1), (2), (7), (14), and the two-shell regularity cubes; (111)–(121): the actual force-containing fixed point.
- CMP119 (1988), pp.255–256, (2.2), (2.6)–(2.12): actual determining support, regular determining data and adjacent-scale bounds; p.248 (1.10): the first explicit exterior regular buffer.
- [two level mixed reference](two_level_mixed_reference.md): the actual interface comparison used solely to verify the local path cocycle.
- [local bundle reference](local_bundle_reference.md): finite local projection and dual-frame algebra, SU reduction, exact graph-edge transport and local Kato identification.
