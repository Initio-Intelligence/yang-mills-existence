# Actual joined determining data and the selected source family

**Annex AO.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


This annex concerns the actual-model C-05 application. It identifies the determining-set operation declared in the source, proves consistency of true minima on that operation, and gives a bounded auxiliary reconstruction for a smooth true-minimizing family in an explicitly adopted symmetric source gauge. Section 7 identifies the corresponding mixed averaging and normalized inverse-gauge map; Section 9 proves its actual older-fluctuation nodal bounds on the full current support. C-05 is not completed by this annex alone.

### 1. Why the join in CMP119 (2.35) has a forced completion

Keep the level of each determining variable as part of its label. In CMP119 (2.2), a complete determining set consists of

\[
 \Gamma_0=\Omega_1^c,
 \qquad
 \Gamma_r=\Omega_r^{(r)}\setminus\Omega_{r+1}^{(r)},
 \quad 0<r<k,
 \qquad
 \Gamma_k=\Omega_k^{(k)}.
 \tag{JI.1}
\]

The source explicitly states that this set determines its domain sequence. Its minimal map \(U(B,V)\) in (2.12) is defined for such admitted determining histories. The nonlinear data are \(M^rU\) on the level-\(r\) determining bonds, by (2.11).

The lower family \(\Gamma_0,\ldots,\Gamma_{p-1}\) determines its depth-\(p\) completion uniquely. First \(\Gamma_0\) fixes \(\Omega_1\). Once \(\Omega_r\) is known, its level-\(r\) site set minus \(\Gamma_r\) fixes the site set of \(\Omega_{r+1}\). The source block alignment reconstructs the physical domain uniquely from that site set. Termination at depth \(p\) forces

\[
 \Omega^{[p]}_r=\Omega_r\ (1\le r\le p),
 \qquad \Omega^{[p]}_{p+1}=\varnothing,
 \qquad \Gamma^{[p]}_p=\Omega_p^{(p)}.
 \tag{JI.2}
\]

Every datum added in this completion is specified already by the displayed argument \(M^\bullet U\): its value is \(M^pU\). No new boundary value or free source coordinate is introduced.

The symbol combining this family with \(B_p(X)\) is the determining-set localization operation declared in (2.14), with its subsequent patchwise generalization. It is not a literal list of mutually overlaid constraints on different scales. Such a literal union need not be an admitted determining set: a local coarse determining cell can overlap an inherited finer determining cell, giving labels incompatible with a single disjoint terminal-block partition. The source has defined \(U(B,\cdot)\) on complete determining histories, and (2.14) specifies how to combine their interior with a local collar. No different constraint-union variational problem is introduced in (2.35).

The reversed order of the two entries does not define another operation. LFR II, printed pp.373–374, uses \(B(Y)\cup B_k\) for the same local determining history and identifies its interior as the region where the new and old determining sets coincide. Thus the combination in CMP119 (2.35) is obtained by completing the lower family as in (JI.2) and applying the previously declared localization operation to that completion.

This is an unpacking of the declared determining-set notation. It does not assume an unproved equality of minimizing fields, and it does not replace the source join by a pointwise intersection of arbitrary domain sequences.

### 2. Componentwise dictionary and the mesh bound

For an admitted boundary patch of \(X\) in old layer \(n\), set
\(r=\min(n,p)\). The depth of the completed old history on that patch is \(r\). Let \(I_r\) be its retained interior and \(C_r\) its collar, with the widths, scale and endpoint conventions of (2.14). Let \(\Lambda_i^{r,X}\) be the local determining sets of the source maximal-domain construction on that patch. The declared join has

\[
 \widehat\Gamma_i
 =\bigl(\Gamma_i^{[p]}\cap I\bigr)
  \cup\bigcup_{r\ge i}\bigl(\Lambda_i^{r,X}\cap C_r\bigr),
 \quad 0\le i\le p,
 \tag{JI.3}
\]

where \(I\) records the retained interiors with their proper-scale masks. The fixed level-zero exterior completes the local history. On a boundary meeting several old layers, each right-hand contribution is restricted to its source layer patch and the source instruction after (2.15) sums those restricted contributions. The admitted buffers and compatible partitions are retained; this formula does not authorize an arbitrary overlapping patch family.

There are three exhaustive cases for a terminal cell:

| Location | Level in the joined history |
|---|---|
| Retained old layer \(n<p\) in the interior | \(n\) |
| Retained old innermost truncated region \(\Omega_p\) | \(p\) |
| Proper-scale collar in old layer \(n\) | A level at most \(\min(n,p)\) |

Because the global odd-block partitions are nested, every smaller terminal cell is an aligned subcell of the old cell it replaces. At an old layer interface the source restricts the patch contributions before taking their union; an entry from the coarser patch is not assigned to the finer side. The determining bonds are then obtained by differences of bond stars. They are not the stars of the site-shell differences.

If \(s(x)\) is the joined terminal level and \(n(x)\) the old one, this gives

\[
 s(x)\le\min\{p,n(x)\},\qquad
 h_{s(x)}\le h_{\min(p,n(x))},
 \qquad
 \widehat\Omega_i\subset\Omega_i\quad(1\le i\le p).
 \tag{JI.4}
\]

The lattice spacing \(L^{-p}\) in the reconstructed map is a change of units on the same physical fine graph. It does not eliminate the smaller collar cells. In physical units, CMP119 (2.37) asks for a reconstructed current bound proportional to

\[
 h_n^{-2}h_{\min(p,n)}^{-1}.
 \tag{JI.5}
\]

In particular, an estimate with the original physical-current weight \(h_n^{-3}\) is sufficient. A generic inverse-collar current estimate is not substituted for it.

### 3. Exact preservation of the old constraints

The source bond convention matters. Write \(\operatorname{st}_rY\) for bonds at level \(r\) incident to \(Y\). A determining shell is

\[
 \operatorname{st}_r\widehat\Omega_r
 \setminus\operatorname{st}_r\widehat\Omega_{r+1}.
 \tag{JI.6}
\]

If a local competitor \(W\) has the same joined data as \(U\), clamp it to \(U\) outside the local fixed fine collar. The nonlinear support induction proved as Lemma JR.1 in gives

\[
 \operatorname{supp}(M^rW-M^rU)
 \subset\operatorname{st}_r\widehat\Omega_{r+1},
 \quad 0\le r\le p.
 \tag{JI.7}
\]

The induction uses the actual nonlinear average: an output bond depends on its two endpoint blocks and their connecting paths. It retains crossing bonds in the star support, then removes only the prescribed star difference. It does not assume support on bonds with both endpoints inside an inner domain.

For \(r<p\), (JI.4) makes the support in (JI.7) disjoint from the old level-\(r\) determining bond set. At \(r=p\), the next joined domain is empty, so every relevant \(p\)-th intermediate average agrees. Iteration of the actual one-step averaging operation then fixes every old higher-level constraint. Therefore the patched competitor satisfies

\[
 M_BW=M_BU.
 \tag{JI.8}
\]

This assertion is restricted to the dependency cones on which the old constrained averages are defined. It does not introduce higher averages in unrelated fixed large-field regions. Near a boundary crossing, the fine collar fixes the links required by every affected Wilson plaquette. At \(p=0\) the reconstruction is the fine-data identity. Components and holes carry their own fixed collars.

#### Corollary — real consistency of the actual critical orbit

Let \(U\) be the true regular Wilson minimum for the old determining history. The joined mesh is no larger, so the absolute regularity conditions of the local variational problem are satisfied. Any sufficiently small differentiable variation in the joined constraint fiber extends through the fixed collar to a variation in the old fiber by (JI.8). At finite cutoff, sufficiently small variations remain in the old open regular class. The old Wilson first variation therefore vanishes, and the fixed collar makes it equal to the local first variation. The uniqueness of the regular critical orbit in CMP102 Theorem 1 identifies the joined critical orbit with the restriction of the old one.

No assertion that every large joined competitor satisfies the old regularity conditions is needed. For complex inputs, this identity can be continued only on a common admitted holomorphic chart. Real equality alone does not supply the chart radius or the norm of a representative change.

### 4. The available source information about the gauge

The following primary statements are separate:

1. CMP119 p.256 initially denotes a minimal configuration as an element of the unique minimal orbit.
2. CMP109 (1.15) specifies that its reconstructed maps are in axial gauges. Thus arbitrary real representative freedom alone does not prove a bound in the complex B domain.
3. CMP109 (0.11) defines the symmetric averaged-contour transport. Its one-step gauge fixing in (0.14)–(0.19) uses these variables. At the real saddle, (2.2) identifies the axial representative by \(G(V)=0\).
4. CMP109 pp.253–254 states that the earlier averaging results remain valid for the symmetric average (0.12). This licenses using the corresponding corrected averaging operators for that average; it does not identify an old corrected operator numerically with a raw nonlinear derivative.
5. CMP99 (3.55) is an explicit hierarchical product of transports at successive averaged levels. Its estimates (3.57)–(3.59) control the relative transport on a terminal block by \(Ch_s\|A\|\), uniformly in its depth. The printed paragraph after (3.57) also bounds the coarse correction \(v_s(y)-1\) by that small quantity.

In particular, an unqualified claim that real unitarity and qualitative analyticity imply a uniform complex gauge bound is false. The analytic functions \(\exp(iNt)\) already disprove that inference.

### 5. The adopted symmetric axial slice

Use one explicit convention for all auxiliary reconstructed maps: the one-step axial condition is the zero of the symmetric source gauge-fixing function, and it is iterated only over the active blocks of the admitted determining history. This is the source-compatible symmetric convention defined by CMP109 (0.11), (0.14)–(0.19) and (2.2). It is not asserted to be a verbatim copy of every older relative AX formula.

For real unitary fields, each summand \(1-\operatorname{Re}\operatorname{tr}\mathfrak t\) in the gauge-fixing function has the same sign and vanishes precisely when its transport is the identity, using the source normalized trace. Thus the real condition \(G(V)=0\) in (2.2) is equivalent to setting each one-step averaged-contour variable (0.11) to one. The recursion (0.19), followed by the choice of the critical representative in (2.2)–(2.3), imposes this condition successively. On a mixed history it is imposed only in active blocks; determining roots and the fixed exterior are left fixed. The product description below records exactly those iterated conditions. On complex fields it is these individual holomorphic transport equalities that are used, not the scalar equation \(G=0\) by itself.

For a terminal block \(B^s(y)\) and a fine point \(x\) in it, let
\(x=x_0,x_1,\ldots,x_s=y\) be its nested block centers. Define

\[
 \mathcal T_U(y,x)
 =\prod_{r=s-1}^{0}
   \mathfrak t_{M^rU}(x_{r+1},x_r),
 \tag{JI.9}
\]

where \(\mathfrak t\) is the source one-step averaged-contour transport (0.11), and the product follows the root-to-point order. The group mean itself is not assumed multiplicative. The product in (JI.9) is the explicit hierarchical chain, matching the structure displayed in CMP99 (3.55).

Endpoint equivariance of each factor and gauge covariance of the averaging operation give

\[
 \mathcal T_{U^u}(y,x)
   =u(y)\mathcal T_U(y,x)u(x)^{-1}.
 \tag{JI.10}
\]

The absolute hierarchical slice is

\[
 \mathcal T_U(y,x)=1
 \quad\text{on every terminal block.}
 \tag{JI.11}
\]

Every real orbit of transformations fixed at the determining roots has a unique representative in this slice: take \(u(x)=\mathcal T_U(y,x)\), with \(u(y)=1\), and use (JI.10). The same algebra gives a holomorphic section on every domain on which the actual averages and group means are defined.

#### Heredity under aligned refinement

Suppose an admitted joined history refines the old one as in (JI.4). Its terminal block \(B^t(z)\) is an aligned subblock of an old \(B^s(y)\), with \(t\le s\). The point \(z=x_t\) is an intermediate center in the old chain. Associativity of the displayed product, not multiplicativity of the group mean, gives

\[
 \mathcal T_U(y,x)
   =\mathcal T_U(y,z)\mathcal T_U(z,x).
 \tag{JI.12}
\]

The first two factors on the two sides are one when the old slice condition holds. Hence \(\mathcal T_U(z,x)=1\). The absolute hierarchical slice is therefore hereditary under the actual aligned refinement.

Consequently, when the input minimum is itself in this slice, real consistency from Section 3 is equality of representatives, not merely equality of gauge orbits. It extends as an equality of holomorphic maps wherever both sides have been admitted.

The convention must be used consistently in the source construction and in the definitions of its auxiliary reconstructed maps. Changing only an auxiliary domain predicate and then importing an estimate for an unrelated legacy extension would be invalid. The assertion here is that the symmetric source construction permits the displayed choice, with its corresponding averaging/reference operators. No numerical equality of arbitrary off-physical extensions is claimed.

#### Important distinction: the primitive input is kept smooth

An absolute axial representative can have fine-edge potential spikes. Even in an Abelian block, moving a smooth coarse variation to an axial representative can put its whole coarse increment on one fine boundary link. Therefore (JI.11) is not used to replace the primitive input \(U\) in clause (2.39), nor to estimate its potential or first difference. It fixes only the auxiliary reconstructed representatives whose required outputs in (2.35) and (2.37) are curvature and physical current. Those outputs transform by conjugation, and the following argument bounds that conjugation directly.

### 6. Bounded auxiliary reconstruction on a smooth true-minimal family

Fix the admitted history and a real true minimum \(U_0\). Let

\[
 U(z)=e^{iaA(z)}U_0
 \tag{JI.13}
\]

be an actual smooth holomorphic minimizing family on the common original-geometry contour. For real parameters it is in the real old critical orbit for its own determining data. No assumption that a gauge change fixes those old numerical data is needed: gauge covariance transports the whole old constraint fiber. Assume the existing original-geometry bound on each terminal block is

\[
 \sup_{b\subset B^s(y)}|A(z,b)|\le u_n h_n^{-1},
 \qquad h_s\le h_n,
 \qquad \sup_n u_n\le u_*.
 \tag{JI.14}
\]

Here \(u_*\) is smaller than the fixed absolute map radius. The native field/current endpoint bounds are those already supplied by the original-geometry estimate; they are not conclusions of a bare supremum bound for \(A\).

For this auxiliary joined problem choose the fixed real gauge

\[
 g_0(x)=\mathcal T_{U_0}(y,x)
 \tag{JI.15}
\]

on each joined terminal block. It equals one at every determining root, is group valued, and sends the real reference to the chosen slice. Write \(\overline U_0=U_0^{g_0}\). The relative perturbation of \(U(z)^{g_0}\) is the adjoint transform of \(A(z)\), so its value and covariant norm bounds are unchanged. The fixed real transformation has no parameter derivative cost.

Now put

\[
 g(z,x)=\mathcal T_{U(z)^{g_0}}(y,x),
 \qquad W(z)=\bigl(U(z)^{g_0}\bigr)^{g(z)}.
 \tag{JI.16}
\]

The baseline transport is one. CMP99 (3.55)–(3.59), applied on this terminal block, gives the uniform analytic estimate

\[
 |g(z,x)-1|+|g(z,x)^{-1}-1|
   \le C h_s\sup_{B^s(y)}|A(z)|
   \le C u_n\frac{h_s}{h_n}.
 \tag{JI.17}
\]

The use of the symmetric averaging version is the one expressly allowed in CMP109 pp.253–254. The bound is independent of the number of fine bonds and of \(s\). No global path is used. A fixed reduction of \(u_*\) ensures that all these transport maps and their inverses lie in the same absolute analytic neighborhood.

Both \(g_0\) and \(g(z)\) fix every joined determining root. Every endpoint of a mixed determining bond is such a root, possibly at a finer level, by the nested-grid convention. Hence

\[
 M_{\widehat B}W(z)=M_{\widehat B}U(z),
 \qquad \mathcal T_{W(z)}(y,x)=1.
 \tag{JI.18}
\]

Here is the endpoint argument in full. If a level-\(r\) bond belongs to
\(\operatorname{st}_r\widehat\Omega_r\setminus
\operatorname{st}_r\widehat\Omega_{r+1}\), neither endpoint belongs to
\(\widehat\Omega_{r+1}\). An endpoint \(x\) on the level-\(r\) lattice therefore lies in a terminal site shell of some level \(t\le r\), unless it is in the fixed fine exterior. The level-\(r\) lattice is a subset of the level-\(t\) lattice, so \(x\) belongs to that shell's determining site set and is its terminal root. Exterior endpoints are fixed directly by the extension of the gauge as the identity there. This proves endpoint fixing also for a coarse bond whose second endpoint lies in an earlier finer shell; it is not an inference merely from proximity to a block center.

For real parameters, Sections 2–3 put \(U(z)\) in the joined critical orbit. Equations (JI.18) and uniqueness of the slice identify \(W(z)\) with the actual joined minimizing representative in the adopted convention.

#### Absolute admission precedes running-current estimates

The relative raw averages on the joined determining bonds have dimensionless increments bounded by \(C h_s\sup|A|\), from the local relative-average bounds used in (3.55)–(3.59), including the bounded coarse correction displayed after (3.57). The supremum here is over the actual two-endpoint-block dependency footprint, not only one bond. At a mixed interface the admitted separation prevents that footprint from reaching an old layer more than one step finer; the resulting fixed power of \(L\) and fixed adjacent-layer endpoint loss are included in \(C\). Thus the increments have supremum at most \(C u_*\), also at such interfaces. Choose \(u_*\) below the fixed absolute Proposition 9 radius before testing the running B-domain inequalities. The real reference data are already regular by the source variational theorem and the finer joined mesh. The source reconstructed branch and (JI.16) are then holomorphic on the common connected parameter chart. Their equality on its real open family extends to the complex chart.

This admission uses the absolute raw-data radius. It does not assume the stronger reconstructed-current conclusion in order to invoke that same conclusion.

#### Current and curvature bounds

Let \(F(U)=\partial U-1\) denote plaquette curvature, with its base point convention, and \(J(U)\) the physical Wilson current. Exact gauge covariance yields

\[
 F(W)=\operatorname{Ad}_{g g_0}F(U),
 \qquad J(W)=\operatorname{Ad}_{g g_0}J(U).
 \tag{JI.19}
\]

The real adjoint factor of \(g_0\) is isometric and the complex one of \(g\) is bounded uniformly by (JI.17). Consequently the old physical weights \(a^2h_n^{-2}\) and \(h_n^{-3}\) remain valid, with a fixed factor. Equation (JI.5) is weaker than the latter current weight.

For a marked current coordinate, the analyticity and uniform local bound for the transport map give

\[
 |g^{-1}\partial_i g|
 \le C h_s\sup_{B^s(y)}|\partial_iA|.
 \tag{JI.20}
\]

The source original-geometry endpoint estimate bounds the right-hand side by
\(C g_k(h_s/h_n)e^{-c d_\Omega(y,i)}\). The block diameter in the old inverse-mesh metric is bounded, since \(h_s\le h_n\); taking a supremum over that block changes only the fixed endpoint constant. Differentiating (JI.19) gives

\[
 \partial_i J(W)
 =\operatorname{Ad}_{g g_0}
   \left(\partial_iJ(U)+[K_i,J(U)]\right),
 \tag{JI.21}
\]

where \(K_i\) is \(g^{-1}\partial_i g\) conjugated by the fixed real \(g_0\), hence has the same norm. The commutator is bounded by the old current weight times \(C\alpha_n g_k e^{-c d_\Omega(y,i)}\), with no inverse-collar factor. The curvature derivative has the identical form, using \([K_i,1]=0\). Thus this auxiliary converter retains the original normalized endpoint response and the required reconstructed physical weights.

The primitive arguments remain the smooth \(U(z)\), its actual independent-current coordinate, and its specified old-field tuple. Neither (JI.16) nor (JI.19) applies a gauge transformation to those primitive arguments. The argument establishes the reconstructed-output part of their admission on a true-minimizing family; it is not yet a local analytic chart for every off-minimum native direction.

### 7. The actual symmetric relative-coordinate dictionary

The normalization needed for the Landau-to-axial map is displayed in an available primary formula, CMP99 p.418, (3.113). It need not be inferred from the unavailable formula (106) in the earlier averaging paper. Fix the following single operator family throughout:

| Object | Definition in this construction |
|---|---|
| Raw block average \(M\) | CMP109 (0.12) |
| Endpoint transport \(T_U(y,x)\) | The same symmetric averaged contour, CMP109 (0.11) |
| Corrected relative average | The endpoint correction displayed in CMP99 (3.113), using this same \(M,T\) |
| Averaging of a gauge transformation | The anchored logarithmic mean derived below from that correction |
| Axial slice | The iterated one-step condition on these same transports, Section 5 |
| Linearized \(Q,Q'\), remainders, kernels | Those associated with this corrected family, not an unmodified operator from a different path convention |

CMP109 pp.253–254 explicitly transfers the earlier averaging results to its symmetric construction. Its Section 2 then actually uses the axial/Landau reduction of CMP102 for that construction. These statements specify which associated operators are meant. They do not assert that the raw derivative of \(M\) equals a corrected \(Q\).

#### 7.1 Direct derivation of the one-step normalization

For a reference \(U\) and a nearby field \(W\), define the relative endpoint correction

\[
 R_y(W;U)
 =\exp\!\left[\sum_{x\in B(y)}L^{-d}
       \log\bigl(T_W(y,x)T_U(y,x)^{-1}\bigr)\right].
 \tag{JI.25}
\]

All logarithms are in the admitted principal neighborhood. Put \(\overline U=M(U)\). The corrected relative average at a coarse bond \(c\) is the source expression

\[
 \mathcal Q_U(W)(c)
 =R_{c_-}(W;U)^{-1}M(W)(c)\overline U(c)^{-1}
       \operatorname{Ad}_{\overline U(c)}R_{c_+}(W;U).
 \tag{JI.26}
\]

Let \(W=U^u\). Raw endpoint covariance gives
\(M(W)(c)=u(c_-)\overline U(c)u(c_+)^{-1}\). The transport in (JI.25) is
\(u(y)\operatorname{Ad}_{T_U(y,x)}u(x)^{-1}\). Using conjugacy of the principal logarithm gives the exact identity

\[
 R_y(U^u;U)=u(y)\bigl(\mathfrak R_Uu(y)\bigr)^{-1},
\]

where

\[
 \mathfrak R_Uu(y)
 =u(y)\exp\!\left[\sum_{x\in B(y)}L^{-d}
       \log\bigl(u(y)^{-1}\operatorname{Ad}_{T_U(y,x)}u(x)\bigr)\right].
 \tag{JI.27}
\]

Substitution in (JI.26) yields

\[
 \mathcal Q_U(U^u)(c)
 =\mathfrak R_Uu(c_-)
    \operatorname{Ad}_{\overline U(c)}
        \bigl(\mathfrak R_Uu(c_+)^{-1}\bigr).
 \tag{JI.28}
\]

This is exactly the calculation printed on p.418, now with the designated symmetric transport. It uses endpoint equivariance and local logarithms; it does not assume that a group mean is multiplicative. Its linearization is the source identity \(QD=D^{\rm coarse}Q'\). The corresponding nonlinear normalization is the iterate of (JI.27), with the successive reference averages, at each terminal determining root. It is not an independently chosen average over an entire large block.

#### 7.2 Uniform bound for the normalized converter

Annex AP, Section 9, constructs this exact normalized converter. In a reference frame in the hierarchical slice, put \(R_x=\mathcal T_L(y,x)\), for \(L=e^{iaA}U_0\) on a terminal block of size \(h_s\). The transport bounds give

\[
 |R_x-1|\le Ch_sK,\qquad
 |R_x-R_z|\le Ch_rK
 \quad(x\in B^r(z)\subset B^s(y)),
 \quad K=\sup_{B^s(y)}|A|.
\]

In this frame (JI.27) is the anchored mean
\(r_z\exp[L^{-d}\sum_x\log(r_z^{-1}r_x)]\). Its supremum-norm derivative at a constant identity tuple is the normalized arithmetic mean, of norm one. On one fixed neighborhood it is at most two. If \(E_r\) is the error between its \(r\)-fold iterate and the original value at that root, then

\[
 E_r\le2E_{r-1}+Ch_rK,
 \qquad E_r\le\frac{C}{1-2/L}h_rK.
 \tag{JI.29}
\]

The odd block size satisfies \(L\ge3\). A fixed smallness choice for \(h_sK\) therefore keeps every iterate in the same analytic neighborhood, independently of the depth. At the terminal root, the iterated value is \(F_s=1+O(h_sK)\). The root factor \(c_y=F_s^{-1}\) and
\(u(x)=c_yR_x\) satisfy both the source terminal normalization and the chosen axial condition, with

\[
 |u-1|+|u^{-1}-1|\le Ch_sK,
 \qquad |u^{-1}\dot u|\le Ch_s\|\dot A\|_{\infty,B^s(y)}.
 \tag{JI.30}
\]

The second bound follows by holomorphic differentiation on a smaller fixed absolute ball. It retains an endpoint bound when \(\dot A\) has one.

For a reference not already in the slice, the exact formula is

\[
 u(x)=\mathcal T_{U_0}(y,x)^{-1}
                  c_y\mathcal T_L(y,x).
 \tag{JI.31}
\]

The anchored mean is covariant under a simultaneous frame change of \(U_0,u\); this follows by conjugating each logarithm in (JI.27). Thus one may put the normalization equations in the hierarchical frame and pull the answer back. For a complex reference near a fixed real one, source transport comparison gives bounded frame factors and the same estimate (JI.30). No propagator or stationary equation is moved into a potentially spiky axial chart. All such operators remain in the admitted smooth reference chart. The frame change is used only in the algebraic normalization equations.

#### 7.3 Raw-data restoration on a mixed history

For the zero-data reconstruction around an arbitrary admitted \(U_0\), prescribe \(V=M_{\widehat B}U_0\). The identity relative field has every relative average and endpoint correction equal to one, so its corrected datum is exactly \(B=0\). This conclusion does not require the missing formula for a general nonzero relative datum.

Apply (JI.31) independently on the disjoint actual terminal blocks and set the gauge to one in the fixed fine exterior. This defines a single fine-lattice gauge, with one normalization at each terminal root at its own level. CMP102 Proposition 2 gives the correspondence between its nonlinear corrected fiber and the actual raw-data fiber, including the mixed crossing-bond convention. By uniqueness of that normalized inverse, the explicitly constructed gauge is the gauge in this correspondence. Thus a critical Landau correction on the zero corrected fiber produces the actual raw determining data \(V\). No numerical equality of independently prescribed coarse gauges \(v_r,v_t\) is needed at an interface.

This invocation is within the one associated symmetric family in the table above. The local identities (JI.25)–(JI.28), the source's symmetric transfer and the explicit use of the same reduction in CMP109 Section 2 provide its source dictionary. The weighted stationary and current estimates for this corresponding family are proved separately in Annex AP; they are not consequences of the gauge algebra alone. Joint analyticity on the absolute admitted neighborhood extends the real correspondence to its complex chart.

### 8. Old arguments cannot be discarded by invoking gauge invariance

CMP119 (3.15) evaluates inherited B with the new current insertion in its background argument and the old fluctuation tuple retained as written. A gauge used only to estimate a reconstructed-field/current norm need not be applied to that tuple. This is different from replacing the entire primitive argument by a gauge-transformed argument.

The latter operation must transform every old adjoint slot. Old \(A_{j-1}\) lives on a region of the \((j-1)\)-lattice inside \(\Omega_j\); its base points need not be level-\(j\) determining roots. Root fixing alone therefore does not prove its transformation is the identity. LFR II pp.373–374 explicitly retains the splice gauge because two field representations meet at the collar. No gauge-invariance argument here removes that factor.

#### 8.1 A rigorous smooth-chart pullback, when simultaneous covariance is used

This subsection is a conditional alternative only. CMP119 (2.34)–(2.42) supplies analyticity in the field/current pair with the older fields fixed; it does not supply the holomorphic old-field domain hypothesized below. The actual application uses the fixed-old-field replacement in Section 9 and AD17.3 instead.

There is nevertheless a valid way to use the covariance of the whole primitive function. State its contour premises first. Suppose the real physical family is written in an axial representative, and an actual analytic gauge \(u(z,\eta)\) carries it to a smooth relative-Landau representative \(U_L(z,\eta)\). Suppose \(u\) is group valued for real parameters and has bounded adjoint factors and marked derivatives on the common complex contour. Let \(\mathbf A\) denote the fixed old integration coordinates. Define directly

\[
 F_X^{\rm sm}(z,\eta)
 =b_X\bigl(U_L(z,\eta),
        J_L(z,\eta),
        \operatorname{Ad}_{u(z,\eta)}\mathbf A,\mathbf S\bigr),
 \tag{JI.22}
\]

where the current argument is transformed by the same actual gauge, including an independent-current displacement if present. The sign of \(u\) is fixed by \(U_L=U_{\rm AX}^{u}\). Require that every displayed argument lies in the source primitive domain with its specified margins.

Then (JI.22) is a holomorphic extension of the physical primitive pullback. For real parameters, the source's simultaneous group-valued covariance gives its equality with
\(b_X(U_{\rm AX},J_{\rm AX},\mathbf A,\mathbf S)\). Thus their physical parameter derivatives agree to every finite order. The proof does not invoke complex covariance at an axial point that may fail the relative-field condition (2.39); it defines the holomorphic extension using the admitted smooth-chart arguments. Nor does it change an old integration variable, selector or measure. It retains the explicit current-dependent argument of the primitive function.

#### 8.2 Old sup-norm slots have a uniform relative margin

For an old adjoint slot with analytic radius \(R_j\), assume
\(\|A_j\|\le(1-\sigma)R_j\), with one fixed \(\sigma>0\). If
\(\|u-1\|,\|u^{-1}-1\|\le\epsilon\) and \(\epsilon\) is a sufficiently small fixed multiple of \(\sigma\), then

\[
 \|\operatorname{Ad}_uA_j\|
 \le(1+\epsilon)^2(1-\sigma)R_j
 \le(1-\sigma/2)R_j.
 \tag{JI.23}
\]

Support is preserved exactly. For a marked current coordinate, the old input is fixed, and differentiation gives

\[
 R_j^{-1}\bigl|\partial_i(\operatorname{Ad}_uA_j)\bigr|
 \le C\,|u^{-1}\partial_i u|\,
                 \frac{\|A_j\|}{R_j}.
 \tag{JI.24}
\]

Thus the old logarithmic amplitude cancels against its actual analytic radius. If the source old-slot domain is a product of these balls, using the supremum of their normalized norms produces no factor equal to the number of old scales. An endpoint-local bound for \(u^{-1}\partial_i u\) remains an endpoint-local bound for this whole old-slot tangent.

Any additional old-field constraint or gradient clause must be checked in its actual definition. A gauge-covariant norm co-transformed with its background obeys the same adjoint estimate. A norm with a fixed reference background, or a noncovariant constraint chart, does not acquire that property merely from (JI.23). The source old-slot analytic radii and the required marked converter are separate application checks. This lemma therefore does not justify dropping an old argument or a relocation derivative.

### 9. Actual old-node gauge bounds on the full current support

The converter hypothesis in AD17.3 is supplied by the original-geometry response already proved in Annex AF, together with the normalized inverse gauge above. This section performs that application; it does not assume an independent bound on unknown gauge values.

Write

\[
 P_k=A_1\ell_k^{p_0},\qquad
 \alpha_n=C_\alpha g_n\ell_n^q,\qquad
 q>p_0,\qquad
 \vartheta_k=\frac{g_kP_k}{\alpha_k}
             =\frac{A_1}{C_\alpha}\ell_k^{p_0-q}.
 \tag{JI.32}
\]

The actual nonlinear constraint input is \(g_kCz-hD(g_kCz)\), not its linear approximation. The full current ball is \(\|z\|_\infty<2P_k\). Proposition E14.1 and the running-radius check E14.24 admit that input in the source's absolute map chart on this entire ball. The original-geometry estimate BM.10 then gives, on output layer \(n\le k\),

\[
 h_n\|A_{\rm L}(z)-A_{\rm L}(0)\|_{
        \infty,\Delta_n}
 \le C g_kP_k e^{-\gamma(k-n-c_0)_+}.
 \tag{JI.33}
\]

The same estimate holds for the other normalized output rows; BM.11 supplies the physical current row. The proof of BM.10 first retains the endpoint kernel and only then takes its normalized row sum. Consequently a single current coordinate also has

\[
 h_n|\partial_iA_{\rm L}(x)|
 \le Cg_k e^{-\delta d_\Omega(i,x)},
 \tag{JI.34}
\]

after the fixed absolute operator and native-radius reductions, with the current ball still \(\|z\|_\infty<2P_k\). The absolute map has the reserve exhibited in E14.8 before this running current radius is inserted. Constants include the actual constraint stencil and its fixed adjacent-layer enlargement. There is no factor equal to the number of fine bonds or to the current support volume.

The AF comparison used in BM.13 is
\(\alpha_k/\alpha_n\le C_{\rm AF}\sqrt{1+k-n}\). Therefore (JI.33) gives

\[
 \frac{h_n}{\alpha_n}
   \|A_{\rm L}(z)-A_{\rm L}(0)\|_{
       \infty,\Delta_n}
 \le C\vartheta_k\sqrt{1+k-n}
                 e^{-\gamma(k-n-c_0)_+}
 \le C'\vartheta_k.
 \tag{JI.35}
\]

Using BM.3, a fixed part of the endpoint exponent in (JI.34) pays this same square-root ratio. A positive endpoint rate remains:

\[
 \alpha_n^{-1}h_n|\partial_iA_{\rm L}(x)|
 \le \frac{C\vartheta_k}{P_k}
                   e^{-\delta' d_\Omega(i,x)}.
 \tag{JI.36}
\]

#### 9.1 From the Landau response to the actual fine gauge

Apply (JI.30), or RM.33 and RM.36, on each actual terminal block. Its side is \(h_n\), and its diameter in the source inverse-mesh metric is bounded. Enlarging to the fixed transport dependency neighborhood changes only the constants and the reserved positive endpoint rate. It follows that the actual normalized fine gauge has

\[
 \alpha_n^{-1}|\log u(x)|\le C\vartheta_k,
 \qquad
 \alpha_n^{-1}|\partial_i\log u(x)|
 \le\frac{C\vartheta_k}{P_k}
                 e^{-\delta''d_\Omega(i,x)}.
 \tag{JI.37}
\]

The logarithm and inversion use the same fixed small matrix neighborhood. If the convention calls the inverse gauge the axial-to-Landau converter, (JI.37) holds for that inverse as well. The estimate is on the actual fine-lattice values, not merely on their normalized average.

For a varying native reference, retain both inputs in (JI.31). Compare their transports with the fixed real reference \(U_*\), as in RM.35–RM.36. If the relative native reference has value radius \(r_b\alpha_n/h_n\), its contribution to the first inequality in (JI.37) is \(Cr_b\). The actual external source chart has that bound by E14.45–E14.48 and the same AF comparison; its fixed coefficient may be reduced after the constants in AD17.3 are known. Current derivatives still differentiate the current input alone, while native derivatives retain the reference term. No reference derivative is dropped. These statements are simultaneous with the independent current variable because the gauge formulas are analytic functions of the same admitted smooth output; the independent current is never identified with its physical value off the physical slice.

There are two distinct identifications here. On real retained determining data the source field is the true minimizing family, and the correspondence is physical. For an arbitrary admitted external native background, use exactly the formal family selected in E14: CMP102 (179)–(180), with its CMP116 (1.17) preparation. CMP102 p.307 defines its axial continuation by applying the normalized inverse gauge to its Landau expression; p.309 extends the operators and analytic estimates to admitted nonminimal external backgrounds. The converter above satisfies the actual same normalization and relative axial equations, so uniqueness of this algebraic gauge construction matches that formal continuation also. It does not assert that the formal continuation is a physical minimum off the minimal reference graph. This argument does not substitute the possibly different formal continuation (174)–(175). The latter is used elsewhere only to read a checked linear kernel. The auxiliary reconstructions required by the primitive B domain, on any such arbitrary smooth input, are the actual zero-data minima treated by NP.5 and RM.3.

For clarity about fixed real gauges, let \(t(z,b)\) be the full Landau-to-selected-axial converter, including the rooted reference factor in RM.37, and put \(t_*=t(0,0)\). The latter is real and fixed. Rewrite the whole primitive once by its real covariance, replacing its old fields by the fixed real tuple \(\operatorname{Ad}_{t_*^{-1}}\mathbf A\). The converter from the correspondingly transformed axial input to the smooth field is

\[
 \gamma(z,b)=t(z,b)^{-1}t_*.
 \tag{JI.38}
\]

It equals one at the center. Transport comparison proves (JI.37) for \(\gamma\), with the additional \(Cr_b\) term. The spatially varying fixed real gauge is not applied to the smooth input chart or to its propagators. Its only purpose here is the exact once-for-all rewriting of the real primitive and its fixed real older arguments. On a reference already in the adopted source slice this factor is simply the identity.

#### 9.2 Actual action on the older fluctuation nodes

The earlier field \(A_j\) is the logarithm of a quotient of two raw \(j\)-scale link configurations with the same endpoint covariance. Hence their quotient transforms by conjugation at the initial point, giving exactly CMP119 (1.17):

\[
 A_j(b)\longmapsto
 \operatorname{Ad}_{\gamma(b_-)}A_j(b).
 \tag{JI.39}
\]

Raw averaging restricts the fine gauge to the \(j\)-grid. The iterated mean \(\mathfrak R\gamma\) used to normalize a relative chart is not substituted for this restriction.

By the actual old-slot support and grading proved in AD17.19–AD17.19c, every such basepoint has terminal level \(n\in[j,j+2]\). Adjacent running radii and meshes have fixed comparison constants. Equations (JI.37)–(JI.39) therefore imply

\[
 \begin{split}
 |\log\gamma(x)|&\le C(\vartheta_k+r_b)\alpha_{j+1},\\
 \alpha_{j+1}^{-1}|\partial_i\log\gamma(x)|
 &\le \frac{C\vartheta_k}{P_k}
                   e^{-\delta'''d_\Omega(i,x)},
 \qquad x\in\mathcal N_j.
 \end{split}
 \tag{JI.40}
\]

Thus (AD17.20) and its current-endpoint version hold for the actual normalized fine converter. The first coefficient can be made smaller than any fixed required reserve: choose the native coefficient \(r_b\) first, then reduce the common coupling ceiling so that \(\vartheta_k\) is uniformly small. Neither choice depends on age, observable order, fine mesh or total volume.

#### 9.3 Fixed-old-field replacement

AD17.3 interpolates these actual nodal values by a smooth fine gauge \(v\), using disjoint bumps in fixed real local regular frames. It has \(v=\gamma\) at every older fluctuation basepoint, so real simultaneous covariance gives

\[
 B(U_{\rm AX},J_{\rm AX},\mathbf A)
 =B(U_{\rm L}^{v^{-1}},
       \operatorname{Ad}_{v^{-1}}J_{\rm L},\mathbf A)
 \tag{JI.41}
\]

after the fixed real convention change just described, if required. The right side has fixed real older fields. It is the admitted holomorphic extension on the contour once NP.5 and the explicit AD17.28 reserve are imposed. No complex old-field analytic radius is invoked. The bump construction retains the endpoint estimate; the curl/current row follows from exact current covariance and the local chart identity, as proved in AD17.25–AD17.27.

This bridge applies to the actual physical pullback and its admitted analytic continuation. It does not assert that a complex decoupled intermediate field is itself a physical minimum. A proof that uses a separately prescribed decoupling family must keep that family's own map identification; the direct endpoint summation BC16 does not require such a replacement. The complete boundary-sector and carrier assembly remains a separate final check.

### Primary sources used

- CMP119 (1988), 243–285, (2.2), (2.11)–(2.15), (2.34)–(2.39), (3.15).
- CMP102 (1985), 277–309, Theorem 1, Proposition 2, (124)–(127), (181), Proposition 9.
- CMP99 (1985), 389–434, (3.55)–(3.59) and (3.113); printed pp.401 and 418.
- LFR II, CMP122 (1989), 355–392, pp.373–375, (1.61)–(1.64), including the explicit warning about the retained splice gauge.
- CMP109 (1987), 249–301: (0.11)–(0.19), (1.15), (2.2)–(2.5), and the transfer statement for symmetric averaging on pp.253–254.

The geometry argument uses the source's admitted patch construction. It does not assert a theorem for arbitrary nonaligned overlapping domain families.
