# Completed R components and the uniform repeated carrier norm

**Annex AU.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).

**Scope of the inference.** The endpoint, stopped-prefix and repeated positive carrier estimates on actual all-history data are assumptions in this application. The native estimates cited below apply on their own admitted domains. In particular a derivative of an isolated minimizing map does not establish the derivative of a composed field at fixed older variables.


The scalar carrier argument uses the final majorant of LFR II and the stated birth-index recurrence. Its application to the complete conditional law assumes the relative positive carrier estimates on every repeated history, with the actual support, tag and connector costs.

### 1. The exact source alternative

LFR II, pp.391–392, applies the normalized component operations to the **whole boundary exponential which depends on their variables**:
\[
 \prod_{Y\in\mathcal Y_j}(T'_j(Y)1)\,
 \left[
 \prod_{Y\in\mathcal Y_j}
       (T'_j(Y)1)^{-1}T'_j(Y)\,
       \exp\!\left(\sum_X B_j(X)\right)
 \right].
 \tag{CR.1}
\]
The source constructs a convergent exponentiated expansion of the bracket. Its new scalar activities are denoted here by \(\widehat B_j(X)\). The remaining multipliers \(T'_j(Y)1\) depend only on the raw field \(V_j\) restricted to \(Y\); printed p.392 explicitly says that they do not participate in the next renormalization transformation.

This is an exact source-free change of representation. It does not replace \(T'_j(F)\) by \(T'_j(1)F\). If an observable is present, it must be transported through the same positive normalized operation, with the boundary exponential included in the baseline conditional law. No estimate for such transported marks follows from this algebraic identity. The separate marked-history obligations remain.

The change of representation also changes the convenient carrier estimate. The source retains decay outside the fixed eligible components, with no requirement to cover every \(M\)-cube inside one of them by a decay tree. Thus the full primitive estimate (2.42) cannot simply be reused with an unchanged full-tree norm.

The exact printed input to the alternative exponentiation is the modified polymer estimate (1.95): \(\widehat\beta=\beta/4\), \(\widehat\alpha=Cc_1\), and the two decays
\[
 \exp\{-(1+\widehat\beta)\kappa
           d_j(X'\setminus\cup Y)\},
 \qquad
 \exp\{-c_d\widehat\beta\kappa M^{-d}
           |X'\setminus\cup Y|\}.
 \tag{CR.2}
\]
The normalized-operation factors \(e^{3N_Y}\) arise in the modified (1.92); they are not omitted from the subsequent majorant. The paper states that the corresponding modifications give the convergent logarithmic expansion. A precise weighted anchored bound for that expansion must retain the exterior-volume factor and the attachment count. A pointwise contracted-distance bound alone is not a substitute.

### 2. Actual component geometry

Put \(h_j=L^{j-k}\) in the current \(k\)-coordinates and \(s_j=MR_jh_j\). An eligible component at birth \(j\) is a **whole component of the pre-R large-field region**, not one of its smaller preparatory internal regions.

The following source facts have been checked:

- LFR I p.177 defines eligibility by containment in a cube of side \(100MR_j\), and takes a union of whole selected components.
- The pre-R domains produced by the \(j\)-th T operation are unions of \(MR_j\)-cubes; CMP119 p.256 and the explicit construction (3.20) retain that grid.
- Preparatory exclusions remove whole originally selected components. The internal domains used in the minimizing maps may shrink, but this does not shrink the original component footprint used by the final \(X_i,Y_i\) split; LFR II p.378.
- The connectivity convention joins intersecting **or touching** domains; LFR II p.386. Distinct selected closed grid components consequently have distance at least one grid cell, up to one fixed norm convention.
- The eligible footprints have bounded aspect ratio. Their last \(N\) histories are rectangular parallelepipeds, and the ten-layer construction gives every side a lower bound \(cMR_j\), while eligibility gives the upper bound \(100MR_j\); LFR I p.177. This lower-side bound is needed when resolving small old tags into current mesh cells.

Therefore, with fixed constants \(D,c_{\rm sep}>0\),
\[
 \operatorname{diam}Y\le D s_j,\qquad
 \operatorname{dist}(Y,Y')\ge c_{\rm sep}s_j
       \quad(Y\ne Y',\hbox{ same birth }j).
 \tag{CR.3}
\]
The AF calculation (AB17.23b) gives
\[
 R_jh_j\le B_{\rm AF}R_k,\qquad B_{\rm AF}\le5/4.
 \tag{CR.4}
\]
No factor \(R_j\) is replaced by \(R_k\) before physical rescaling.

#### Active tags through further steps

Keep a tag for every fixed eligible footprint whose raw multiplier has not yet been integrated by a later complete operation. A later attempted R component is a whole component of the current pre-R large-field region. Hence it contains each older intersected tag in its entirety. It is disjoint from the other tags.

After the nonself estimate for an attempted component has been established, all older tags it contains may be promoted to that whole component as an over-carrier on a retained or failed branch. This is legitimate even on a preparatory failure: the original footprint remains in the large-field region, though some shell integrations or lower-layer geometries have already changed. Promotion enlarges the free set and never strengthens an assumed exterior decay. It does not by itself prove a statement about the changed kernel or selectors. Promoting before the nonself estimate would incorrectly erase a connector needed in Section 7 below.

When a complete successful branch removes such a component, the component's physical size is still bounded by (CR.3). The source's small factor \(e^{-p_0(g_j)}\) pays the restoration of every \(M\)-cube in it: LFR II p.389 explicitly compares that factor with
\(\exp\{2\kappa(100R_j)^d\}\) before (1.95)–(1.100). Restoring old free subregions contained in that component costs no more than restoring the whole component.

For two surviving tags of different births, use the grid at the later attempted component. Its separation from the current component containing the older tag is at least \(c s_{\rm later}\). By (CR.4) on those two scales, \(s_{\rm older}\le B_{\rm AF}s_{\rm later}\). Thus the active tags form an antichain with
\[
 \operatorname{dist}(Y,Y')
 \ge c_*\max(s_Y,s_{Y'}),\qquad
 \operatorname{diam}Y\le D s_Y.
 \tag{CR.5}
\]
This is the geometry needed below. It does not collapse an arbitrary, possibly enormous, unreplaced large-field component into a free atom.

### 3. Diameter control without a full-tree conversion

Let \(X\) be a connected carrier which either contains or misses each of its fixed tagged components. Let \(\ell(X)\) be the length, in units \(Mh_j\), of a connecting tree **after assigning zero traversal cost inside the tags**. This is a conservative cost: a source outside-tree length which also charges travel through a tag is no smaller.

Let \(s_{\max}\) be the largest physical \(s_Y\) among tags contained in \(X\), with \(s_{\max}=0\) if none occurs.

#### Proposition CR.1 — the diameter estimate

For the separated tags (CR.5),
\[
 \operatorname{diam}_k X
 \le C\{Mh_j[\ell(X)+1]+s_{\max}\}.
 \tag{CR.6}
\]
The constant depends only on \(D,c_*\) and the fixed lattice conventions.

**Proof.** Follow a simple path in the contracted connecting tree between two points of \(X\). Consecutive tagged components on this path are separated by at least \(c_*\) times the larger of their size parameters. Charge the diameter of every component except the first to the preceding outside connecting segment. A component at an endpoint can be included in the same bound, leaving at most one uncharged diameter. The outside portions have total length at most \(Mh_j\ell(X)\). The first component contributes at most \(D s_{\max}\); cube/plaquette endpoints contribute \(CMh_j\). Replace each zero-cost traversal by a path of length at most its component diameter. Taking the supremum over the endpoints proves (CR.6). No traversal tree visiting every cube inside a tag is introduced. \(\square\)

If the actual source length \(d_j(X\setminus\cup Y)\) controls a connected tree visiting all exterior cubes, the sharper bound
\[
 \operatorname{diam}_kX
 \le Mh_j d_j(X\setminus\cup Y)+2Ds_{\max}+CMh_j
\]
is available directly. The weaker (CR.6) suffices for the current-position estimate.

#### The collar is extracted before choosing an interior root

All surviving tags are in the old large-field set. The current support is separated from their union by the actual growing collar. A current-to-carrier kernel and the exterior carrier connections can be joined at the **first** tagged component they reach. No traversal of that component's free interior is needed to reach the old large-field set.

Consequently a fixed share of their combined decay supplies
\[
 e^{-c_{\rm col}R_k}.
 \tag{CR.7}
\]
The age connector is handled by the same rule: before the path first reaches an old tagged component, all crossed newer layers are outside that component. The proof of the \(n>j\) age payment in BC16 therefore uses the exterior part of the carrier.

Choosing a canonical point deep inside a component first would be incorrect: it would subtract \(O(100MR_jh_j)\) from the source guard. The free diameter is paid **after** (CR.7) has been extracted, with a separate, arbitrarily small final spatial rate.

### 4. Raw retained variables and the nodal extension

The alternative representation has integrated the fine hidden variables inside the completed component operation. It may still contain the raw \(V_j\) restricted to its tagged \(Y\), as a retained argument or in the multiplier. These raw variables are not assigned a new complex ball.

Extend the node list in AD17.3 to include both endpoints of each retained raw bond used by a primitive, as well as the basepoints of its old adjoint fields. At a raw endpoint \(x\) of mesh \(h_b\), the surviving support lies outside the subsequent small-field domain. Its actual terminal grade \(n(x)\) therefore satisfies
\[
 b\ge n(x)-c_0
 \tag{CR.8}
\]
with one fixed star/endpoint allowance \(c_0\). This is the needed one-sided relation: the node grid is no finer than a fixed multiple of the native local mesh. No lower bound on \(n(x)-b\) is needed.

#### Proposition CR.2 — sparse raw endpoints cause no new interpolation loss

The AD17.3 nodal construction and its value, first-gradient and curl-current estimates remain valid for this enlarged list, with fixed \(L^{c_0}\)-dependent constants.

**Proof.** Merge repeated nodes; all targets are the same actual fine gauge \(u(x)\). At nodes whose native grades differ by at most one, (CR.8) and nesting of the odd grids imply separation at least \(L^{-(c_0+2)}\) times the larger native mesh. At larger grade separation, the admitted history buffers give the same fixed separation as in AD17.3. Thus disjoint bumps with radii a fixed fraction of the native mesh can be used. The interpolation is performed in fixed real local regular gauges exactly as in AD17.3; its estimates depend on the native mesh and the target \(u(x)\), not on the possibly coarser raw grid.

Raw averaging covariance is the endpoint action
\[
 V_b(x,x')\longmapsto
       u(x)V_b(x,x')u(x')^{-1}.
 \tag{CR.9}
\]
Matching \(v=u\) at both endpoints therefore cancels the entire raw transformation, while matching the basepoint cancels the adjoint transformation of an old fluctuation. The two real covariance identities give the same fixed-old-variable scalar extension as in AD17.3. The independent-current and physical-current estimates use that proposition's exact current identity. Nodes in the fixed exterior, where the actual converter is the identity, require no bump. \(\square\)

This proposition concerns the scalar activities after the completed integration. It is not a pointwise covariance theorem for an unintegrated, partially prepared kernel.

### 5. Which carrier norm the derivative theorem actually needs

The following formulation exposes the precise remaining quantitative input. Let \(b_{j,X}\ge0\) be the **absolute cluster majorants** of the scalar completed-R activities on their common native contour. They must include the normalized-kernel factors and all sums over the internal polymer expansion. They are not just pointwise values assigned after cancellation.

For some fixed \(\lambda>0\) and integer \(s\), the sufficient anchored input is
\[
 \sum_{X:\,\text{root}=r}
 b_{j,X}\,
       e^{\lambda\ell(X)}
 \le C B_R(1+R_j)^s.
 \tag{CR.10}
\]
Here a root is an exterior \(M\)-cube or one actual fixed component; the latter is not enumerated as a free polymer. The right side permits its genuine polynomial attachment cost. A constant total-volume factor, an exponential in \(R_j^4\), or an uncounted number of component attachments is not permitted.

The modified source bound (CR.2) is the appropriate starting point for (CR.10). Keeping a slightly smaller positive rate in the original exterior-tree and exterior-volume majorants is essential. An exterior cube can border only a bounded number of the resolved large fixed components, and a whole root component has \(O(R_j^d)\) initial attachment sites. Components too small to remove an exterior \(M\)-cube do not create additional zero-cost cubes; their geometric slots are fixed rather than independently selected.

These facts remove an interior-domain entropy. They do **not**, by themselves, prove (CR.10) after logarithmic clustering. In particular many activities can overlap in one fixed component. The nonnegative weighted cluster majorant and quantitative smallness estimate in Section 7 justify this additional passage.

#### Proposition CR.3 — a polynomial root cost is sufficient for the full current hierarchy

Assume (CR.10), the genuine common native contour, and the actual current first-endpoint bound
\[
 |\partial_i F_{j,X}|
 \le \frac{C\theta_k}{P_k}\,
 (1+k-j)^b e^{-\Gamma(k-j)}
 b_{j,X}\,e^{-c d(i,X)} .
 \tag{CR.11}
\]
Retain in their combined decay the current collar (CR.7), and assume the fixed age rate has the usual \(L^{4(k-j)}\) root-count reserve. Then the completed-R boundary family satisfies the same current hierarchy as (AB17.5), with a constant independent of volume and history and fixed factorial power five. Its weighted Hessian contribution is \(o(1)\).

**Proof.** Current Cauchy on the full \(2P_k\) contour gives
\[
 |D_{i_1}\cdots D_{i_m}F_{j,X}|
 \le C^m(m-1)!P_k^{-m}\theta_k
 (1+k-j)^b e^{-\Gamma(k-j)}
 b_{j,X}e^{-c\max_\nu d(i_\nu,X)}.
 \tag{CR.12}
\]
This differentiates the complete scalar activity and its nonlinear argument map.

By (CR.6) and (CR.4), the current coordinates at distance at most \(R\) from the carrier number at most
\[
 C\{Mh_j[\ell(X)+1]+C MR_k+R+1\}^4.
 \tag{CR.13}
\]
A sufficiently small fixed final spatial rate costs at most an exponential in the bracket's first two terms. Spend a fixed share of \(\lambda\ell(X)\) on the first and a fixed share of the already extracted collar on \(MR_k\). The rate is chosen independently of the source entropy exponent; no \(\exp(+\kappa R_j)\) is introduced.

For the \(m-1\) summed current coordinates, layer-cake counting raises the bracket in (CR.13) to \(N=4(m-1)\). Use the remaining three decays in the **single power estimate**
\[
 \sup_{u,v,w\ge0}
 (u+v+w+1)^N e^{-a u-a v-a w}
 \le C_a^{N+1}N!.
 \tag{CR.14}
\]
For example \(t^Ne^{-at/2}\le N!(2/a)^N\) with \(t=u+v+w\); the remaining half-decay is retained for the corresponding sums or integral. Take \(u\) proportional to \(\ell(X)\), \(v=R_k\), and \(w=R\). Because \(h_j\le1\), all their coefficients are uniformly bounded. This gives **one** \(N!\), not a product of a carrier factorial and a second collar factorial.

The polynomial root factor in (CR.10) is bounded by a fixed age polynomial times a fixed power of \(R_k\), using AF comparison. A further fixed collar share pays that power. Including it in (CR.14) changes \(N\) by a fixed integer and hence changes only \(C^m\).

For each current anchor, the actual root-grid count is at most \(CL^{4(k-j)}\) times an anchored exponential sum. The unused age rate sums that factor and every fixed age polynomial. The remaining factorial satisfies
\[
 (m-1)!\,[4(m-1)+s']!
 \le C_{s'}^{m+1}(m!)^5
\]
for every fixed \(s'\). This proves the claimed hierarchy. At \(m=2\), its prefactor can be bounded by \(C B_R\theta_k\) after the collar and age sums, so division by \(P_k^2\) tends uniformly to zero. Mixed native jets use the same smaller genuine native ball as in AB17.6. \(\square\)

### 6. Scope of the scalar carrier theorem

The following are now established at their stated scopes:

1. The final source representation removes the hidden completed-R integral while retaining its full boundary exponential and its raw multiplier.
2. Eligible component footprints have the required bounded size and separation. Their active-tag promotion/consumption bookkeeping does not require a new full-tree estimate inside a retained component.
3. The sparse raw endpoint extension of nodal interpolation is valid under the actual support inequality (CR.8).
4. A polynomial anchored cluster norm (CR.10) is sufficient, and its current all-order summation has factorial power five with no extra diameter or volume factor.

Section 7 gives the weighted cluster summation for (CR.10) under its positive primitive attachment, decay and prefix hypotheses. Its use for actual repeated histories requires those uniform input estimates.

The complete application also requires the separately proved **partially failed preparation branch** estimates. Whole-component promotion controls their carrier geometry. It does not certify their changed density, their hard-selector localization, or their current-coordinate dependence. LFR I pp.200–201 explicitly retains intermediate forms of the operation on excluded components. The supporting note Annex AV supplies their actual matching and the exterior relocations in (1.56)–(1.59); the ordinary coefficient responses are treated in Annex AT and the combined application.

The full boundary derivative estimate additionally requires control of all sectors on the same conditional representation, as stated in Annex AW.

### 7. Weighted cluster completion

This section uses Proposition OT.4 of Annex AT. Its source input is the **final printed** (1.68), on the completed domain \(Y\). Charging added halo cubes with the pre-carrier \(Y_4\)'s p.376 rate is not valid and is not used. The source and analysis rate parameters below are kept separate; neither is repeatedly halved.

#### 7.1 The fresh primitive coefficient is exponentially small in the eligible size

After the self terms have been assigned to the positive component operation, the final (1.68) applies to a completed remaining carrier containing a whole positive dilation of an eligible component. Its opposite exterior \(M\)-cubes are separated by \(cMR_j\). The relative tree in the **final** bound must connect them and counts its length through \(Z\). Put \(\beta_{\rm a}=\beta_{\rm s}/2\), where \(\beta_{\rm s}\) is the fixed source parameter. Then
\[
\begin{aligned}
 |V(Y)|
 &\le \alpha
 e^{-(1+2\beta_{\rm s})\kappa d_{j,Z}(Y)}\\
 &\le
 \left[\alpha e^{-c\beta_{\rm s}\kappa R_j}\right]
 e^{-(1+2\beta_{\rm a})\kappa d_{j,Z}(Y)} .
\end{aligned}
\]
The primary common ceiling bounds \(\alpha\) by a fixed constant. Thus the weaker analysis coefficient obeys
\[
 \alpha_j\le C e^{-cR_j}.
 \tag{CR.15}
\]
Self terms are excluded from this estimate. They remain inside \(T'_j\), whose normalized analytic operator norm is bounded by the source (1.75).

The first cluster expansion uses \(c_{1,j}=\alpha_j^{1/3}\), and the second replaces its small primitive constant by \(Cc_{1,j}\). Every fixed positive root required by the two source resummations can be retained in a single coefficient
\[
 \varepsilon_j^{\rm R}
 \le C(1+\ell_j)^A e^{-c_{\rm R}R_j},
 \qquad c_{\rm R}>0,
 \tag{CR.16}
\]
with fixed \(A\). This is stronger than a qualitative assertion that a coefficient tends to zero. In particular
\[
 \sup_j(1+R_j)^s\varepsilon_j^{\rm R}\longrightarrow0
 \tag{CR.17}
\]
for every fixed \(s\), as the common coupling ceiling is decreased.

For repeated tagged input, there are two checks before using (CR.15). First, every active tag was created by a new large-field alternative: either the retained \(Y_i\) alternative on LFR II p.378, or an excluded whole component during the preparatory decompositions. A later eligible component has had no such birth during its preceding \(N\) steps, by condition (ii) on LFR I p.177. Its contained active tags therefore have ages at least \(N\). For \(a\ge N\), the already checked AF estimate gives
\[
 \frac{s_{\rm old}}{s_j}
 \le L^{1-a}(1+\beta_0)(1+a)^{\beta_0}.
 \tag{CR.18}
\]
The source preparation depth \(N_0=N_0(j)\) depends on the coupling: it is defined on LFR I p.179 by \(L^{-N_0+1}MR_{j-N_0+1}=M\), and grows with \(\log R_j\). The waiting depth \(N=N(j)\) is also the actual scale-dependent source choice, with \(N>N_0\), not a universal fixed integer. A fixed additional separation in that admitted rule makes the largest old free diameter less than a fixed fraction of the new component's \(20MR_j\) span. No constant in this note counts all \(N(j)\) levels as a fixed number.

Second, rearranging Proposition CR.1 shows that a tree connecting the two opposite halo points, even with the earlier tags contracted, has charged length at least
\[
 c\{20MR_j-Ds_{\rm old,max}\}\ge c'MR_j.
 \tag{CR.19}
\]
The new-T guard gives the same lower bound by stopping at the first old tag. Thus the fixed analysis weight tested on the full-rate source records retains the fresh connector. The attempted current component is made free only after this estimate. The primary full-rate source norm remains the inductive input; the weaker bound extracted here is not substituted back as the next source rate.

#### 7.2 Primitive attachment sums

Retain the nonnegative connected-expansion majorant before replacing it by a crude pointwise bound. In particular retain:

- the product of the small primitive coefficients in the modified (1.92);
- the exterior-tree reserve and the exterior-volume reserve in (CR.2);
- the factors \(e^{3N_Y}\) from the normalized complex component operations.

The invariant output weight is \(e^{\kappa\ell}\), with the **same fixed \(\kappa\)** as the source induction. The printed \((1+\widehat\beta)\kappa\) outside-tree rate and the exterior-volume rate leave positive reserves after that weight is inserted. Use those reserves for entropy, the site penalties below, and a separate smaller positive analysis rate \(\lambda<\kappa\). The contracted size is no larger than the source tree size before contraction and is subadditive on a connected union. Thus the primitive and both connected sums below are estimated with the full invariant weight, not only with an analysis weight which would be too weak for the next source scale conversion.

For a primitive rooted at an exterior cube, ordinary nearest-neighbor tree encoding gives at most \(C_d^{\,n+1}\) choices for a connected tree of integer length \(n\) through its exterior cubes. One rounds the connecting segments to the \(M\)-grid and traverses the rounded tree twice; choosing a subset of the visited cubes changes only \(C_d\). Interior cubes of a fixed component are not enumerated.

For a primitive rooted in one fixed component, the first exterior attachment has at most \(C(1+R_j)^d\) possibilities. A subsequent distinct component requires an outside connector of length at least \(cR_j\), or the corresponding graded size in a mixed-age family. A reserved connector exponential pays its polynomial attachment choices. Equivalently, the exterior cube at an entrance meets only a bounded number of resolved tagged components, by (CR.5). Very small tags that remove no whole \(M\)-cube introduce no additional exterior-domain choices; their slots are fixed.

These bounds apply to the **primitive source tree** and its retained product coefficients. They are not a count based only on the contracted length of a final cluster. Multiple branches meeting the same component retain their separate small primitive factors.

Resolve incidence supports at the current birth mesh before counting them. A tag which removes whole current \(M\)-cubes is retained as an atom. A finer tag which removes no such cube is assigned to its occupied current \(M\)-cells, and overlap inside it is enlarged to ordinary cell overlap. By the actual lower-side and upper-side bounds in Section 2, failure to contain a full current cell forces all its side lengths to be at most a fixed multiple of the current mesh. It therefore meets only boundedly many cells. Diameter and separation alone would not justify this assertion for an arbitrarily thin long region. Many tiny tags in one cell create only that cell's incompatibility, not one new incidence penalty each. The normalized \(e^{3N_Y}\) factors apply only to the **newly integrated eligible components**, whose diameters exceed \(20MR_j\); all of them are resolved. Earlier tiny tags already belong to scalar activities and introduce no new \(e^3\) factor at this integration.

Consequently the elementary interaction majorants \(\mathfrak a_j(Y)\), including their Mayer factor and normalized-operator factors, satisfy
\[
\begin{split}
 \sup_{c\ {\rm exterior}}\;
 \sum_{Y\ni c}\mathfrak a_j(Y)
       e^{\,\kappa\ell(Y)+4a_0 n(Y)}
   &\le C\varepsilon_j^{\rm R},\\
 \sup_{Q\ {\rm tagged}}\;
 \sum_{Y\ {\rm uses}\ Q}\mathfrak a_j(Y)
       e^{\,\kappa\ell(Y)+4a_0 n(Y)}
   &\le C\varepsilon_j^{\rm R}(1+R_j)^s .
\end{split}
 \tag{CR.20}
\]
Here \(n(Y)\) is the number of exterior cells plus **resolved** tagged atoms in that incidence support, \(a_0>0\) is fixed and small, and \(s\) is one fixed geometric exponent. It does not count every hidden fine tag. Larger fixed powers from a root convention may be included in \(s\). The exterior-volume term pays \(4a_0\) per exterior cell. The connector reserve pays the atom penalties and the \(e^3\) factors for additional atoms; the first atom is included in the constant. No factor \(e^{C R_j^d}\) is discarded.

By (CR.17), the common ceiling can make the right sides at most a fixed \(\delta\), with \(\delta< a_0/16\), uniformly over the actual component family.

#### 7.3 Two connected sums and the rooted logarithmic bound

For completeness, the elementary rooted-tree argument behind the use of (CR.20) is given here. Regard an exterior cell and a fixed tagged component as incidence sites. Two objects are incompatible when their incidence supports overlap. If nonnegative activities \(w(P)\) satisfy
\[
 \sum_{Q\sim P}w(Q)e^{a_0 n(Q)}
 \le a_0 n(P),
 \tag{CR.21}
\]
the rooted-tree iteration
\[
 T_0(P)=w(P),\qquad
 T_{r+1}(P)=w(P)
     \exp\!\left(\sum_{Q\sim P}T_r(Q)\right)
\]
obeys \(T_r(P)\le w(P)e^{a_0n(P)}\), by induction. The exponential accounts for unordered offspring with their \(1/q!\) factors. Every rooted connected family has a spanning rooted tree, so its absolute sum is bounded by this iteration. In the logarithmic hard-core polymer expansion, the alternating connected graph coefficient has the usual tree bound: order the vertices, assign each connected graph its ordered exploration tree, and group the graphs with the same tree; optional extra edges give factors \(1-1\) or \(1\). Thus its absolute coefficient is at most the number of compatible spanning trees. This is precisely the same majorant.

Summing (CR.20) over incidence sites of \(P\) proves (CR.21), with a strict reserve. Apply the iteration first to the connected Mayer families which form the polymer activities in the modified (1.91). It uses at most one of the allocated \(a_0 n\) shares and gives a site-rooted polymer norm at most \(2\delta\). Apply it a second time to the logarithmic polymer expansion (1.98). The remaining shares give its site-rooted absolute norm at most \(4\delta\). The contracted weight is preserved at both stages by subadditivity:
\[
 \ell\!\left(\bigcup_\nu X_\nu\right)
       \le\sum_\nu\ell(X_\nu)
\]
for an overlapping connected family, where overlap inside a tagged atom is allowed.

This proves the desired anchored norm (CR.10), and in fact the stronger bound with \(\lambda\) replaced by the full source rate \(\kappa\). Its right side can retain \(C\varepsilon_j^{\rm R}(1+R_j)^s\). That stronger output is retained for the next source induction; the fixed smaller \(\lambda\)-weight is used only in the separate derivative/counting argument. Arbitrarily many branches at one large component are summed by the rooted iteration. They are not estimated by claiming that a bare final pointwise bound has no attachment entropy.

#### 7.4 Preservation through the next source operations

The norm just proved is a norm of the absolute convergent majorant, not a cancellation-dependent final coefficient. It is preserved by the actual carrier operations as follows.

An ordinary T step leaves tagged raw multipliers fixed and acts outside their large-field regions. Its Gaussian/localization paths retain their usual decay. Multiplication or connected joining uses subadditivity of the contracted tree size; every new localization path pays its own charged outside length. Rescaling uses the physical tag sizes and the original layer kernel measures. No fine bond count is substituted for a normalized source row sum.

At a completed R step, new retained eligible components absorb every older tag they contain. The union of the free regions can only enlarge on that branch, which weakens the exterior weight. The source's normalized-kernel factors are exactly the factors retained in (CR.20). On a successful removed component, old holes disappear; the lost interior cell coverage costs at most the whole component volume and is paid by the existing \(e^{-p_0(g_j)}\) reserve, as explained in Section 2. This does not require restoring a large full-tree weight using the much smaller current collar.

On a preparatory failure, promote the whole attempted component **after** the available nonself estimate. Already generated boundary terms keep their genuine source majorants; assigning the over-carrier only weakens their geometric weight. The original tag masses inside the deep untouched factor remain positive raw multipliers. LFR I (1.76), p.194, explicitly keeps the \(V_h,T_h\) factor separate from the preparatory shell integrals. The source eligibility condition places the earlier tag births in that deep factor. Their geometry is consequently not partly erased by an interrupted shell integration.

These carrier rules are compatible with the primary alternative induction on CMP119 p.262 and LFR II p.392, but retain more information: only actual bounded active tags are free. They do not replace every arbitrary unreplaced large-field component by one atom.

#### 7.5 A uniform birth-index invariant

Subadditivity alone would not exclude a factor \(C^{k-b}\) after many steps. The invariant uses the source's actual birth labels and its unreduced absolute localization records:

1. Ordinary full-tree B families remain a separate summand, with their source bounds. Only fresh R-connected scalar families enter the normalized cluster bound above.
2. For a family born at \(b\), keep its scalar function, its **original birth-scale anchor and carrier dependency set**, its fixed assigned absolute majorant, and the slots it actually uses. CMP119 (2.40)–(2.41) writes precisely such a family \(B^{(b)}(U_k,\mathbf A,\ldots)\). An untouched later T step changes its admitted arguments, not that scalar function or its assigned majorant. The embedding uses the original global source map, not a product of one-step norm constants. A promotion to a larger active tag does not regroup these records under the promoted component's anchor.
3. Use the literal add-back convention of the source. An inherited first term reconstructed in LFR II pp.373–375 keeps its old record only when that record's actual slots and boundary anchor survive; the source's domain inclusion gives an admitted image for its arguments. Ordinary full-tree reference terms on the new history stay in the ordinary source family. Differences created by the source identities and the new normalized-R output receive the current birth label. A record whose old variables or supporting tag are actually consumed is retained in that complete integral until the exact output (CR.1) is formed. If its output still uses another surviving tag, including an older tag outside the attempted component, it is a fresh tagged record anchored at such a survivor; its old holes are not restored without payment. The primary classification (1.99)–(1.100), p.390, gives a full-tree \(e^{-p_0}\) bound only after **all** free holes in that output are absent or paid by the actually removed components. It is then a new ordinary B term if it still meets the surviving ordinary large-field set, and a regular R term if it misses the whole new large-field set. “Surviving tag” here includes every active earlier eligible footprint, not only the newly retained \(Y_i\) at this R step. The final paragraph on p.392 isolates the earlier-large-field dependence in boundary activities and their raw multipliers; iterating it retains the older surviving tags in that classification. Thus a weak-tag record with a deleted anchor is not carried under the old birth label. No old-B self term is moved into \(T'_j\) merely to simplify a label, and no external factor is silently multiplied into a mass whose raw locality is used. The primary masses in (1.104) are unchanged.
4. A genuinely fresh scale-\(k\) output uses a **current \(k\)-grid incidence root**: a resolved active atom, or a current cell meeting an unresolved older tag. It does not inherit that tag's finer birth-grid multiplicity. Tiny tags meeting the same current cell share its incidence convention, as in Section 7.2. This rule is distinct from the original-anchor rule for untouched old records.
5. At every fresh scale, retain the full source rate \(\kappa,\beta_{\rm s}\) before extracting the fixed analysis reserve. CMP119 p.262 gives the new T-created B terms the \(1+4\beta_{\rm s}\) improvement. LFR II p.376 supplies the \(1+3\beta_{\rm s}\) scale conversion for older records. This conversion also holds for their retained tagged records: with the original holes physically fixed, the length of the same charged physical path in \(Mh_b\) units is \(L^{k-b}\) times its length in \(Mh_k\) units. Infimizing over the original paths can only increase the old-to-new bound; rounding to current cells has fixed allowances paid by the reserved tree/cell factors. Newly added or promoted holes only weaken the **output** cost. Thus the old \((1-\beta_{\rm s})\kappa\) path share gives the required current \((1+3\beta_{\rm s})\kappa\) share, with \(L\ge3\) and the fixed small source \(\beta_{\rm s}\), while \(\beta_{\rm s}\kappa\) remains for the old-root sums. This does not identify a contracted old size with the literal uncontracted definition (1.67). The fixed weaker analysis weight is tested against the retained original records; it is never fed back as a smaller source rate.

Here is the numerical invariant. Let \(A_{b,k}\) be the anchored sum of the **frozen birth majorants**, including their fixed root polynomial, for the still-carried records born at \(b\). Its anchors, attachment convention and carrier dependency sets are the original birth-\(b\) ones. It is not the norm obtained by aggregating all those records at a subsequently promoted tag. The assigned majorants remain valid because each actual later argument is admitted into the same original analytic domain; they are not replaced by suprema over different evolving subsets.

For a prefix eligible at step \(k\), the contained completed-tag births obey \(b\le h=k-N(k)\). The source keeps the deep \(T_h,V_h\) factor and the histories at levels at most \(h\) unchanged. The old record's slots and native gauge convention therefore remain available. If a later complete integration consumes those slots, its record belongs to the exact fresh integral/output and is no longer treated as an untouched old record. The scalar first terms which the primary construction explicitly retains use its p.375 domain inclusion.

Removing consumed records cannot increase the nonnegative sum in this fixed birth-anchor convention. Hence
\[
 A_{b,k}\le A_{b,k-1}\quad (b<k)
 \tag{CR.22}
\]
for the carried subfamily. This assertion concerns unchanged records, not a re-expansion of their whole function at each step.

The source differences and pre-exponentiation resummations are linear in the incoming **action** families. The required age gain in their values is not obtained from a future-current derivative estimate. It comes from the explicit value localization factors in (1.66), as follows.

#### The value connector for an incoming birth-\(b\) record

Keep the original birth carrier \(X\), its original anchor in \(Z_b\), and its original tree/localization record. A later promoted component is **not** substituted for that original record's holes when estimating the old residual factor. Such a substitution could erase the very \(b\)-to-\(k\) collars being counted. Promotion is used only for the incidence convention of the future fresh cluster.

There are three cases in the source reconstruction.

- An unchanged first term is carried under (CR.22); it is not part of the fresh value forcing.
- An exceptional term with empty new localization domains which stays inside one component is a source self term. It remains in the literal primary component operation and is not assigned the nonself estimate.
- Every fresh nonself contribution retains a connector from its original carrier to the active boundary. If \(X\) already reaches outside the relevant component, its old tree contains the crossing. If \(X\) stays inside it, a nonempty localization is necessary: the first nonempty domain \(Y'_{i_0}\) in (1.66) meets the source localization collar and contains its mandated \(\Lambda\)-component, by pp.373–374. Retain both the factor involving the scaled distance from \(X\) to that collar and the connecting part of \(Y'_{i_0}\). If the old anchor is outside the attempted component but its carrier meets it, the carrier crosses the corresponding distinct-component gap. Again the old tree supplies that crossing.

In the nonempty case it is not sufficient to call an arbitrary collar point a level-\(k\) regular point. The **whole** source connector, including its \(Y'_{i_0}\) path to the mandated current-scale region, is retained. Source (1.66), and the residual exponential displayed immediately below (1.67), retain fixed positive shares of
\[
 \beta_{\rm s}\kappa\,d_b(X),\qquad
 \delta\,d_\Omega(X,\Sigma_{i_0}),\qquad
 \sum_{i=2}^4(\kappa_1-1)M^{-4}|Y'_i|.
 \tag{CR.22a}
\]
Here \(\Sigma_{i_0}=(Y_{i_0}^{\,0})^c\cap
Y_{i_0}\cap Y'_{i_0}\), in the source notation. The volume factor pays a connecting path through the corresponding \(M\)-cubes. When there is no localization domain, the old tree supplies the full connector instead. These are factors of an absolute **value** majorant.

For the contained-anchor case, stop the connector at its first exit from the whole selected current component. The source \(Y_1\) contains every current \(Z\)-component it meets, and the later \(Y_i\) enlarge it. Therefore a retained path from \(X\) to the first nonempty localization collar reaches this exterior boundary, up to the fixed \(2M_1\) allowance, even if its ultimate collar endpoint lies in another proper-scale region. If \(X\) already exits, the old tree provides this portion. This is the boundary crossing used in the age estimate.

Split this connector where it first enters each actual determining layer. If the point at which it leaves the old carrier has grade \(n\), its old tree part crosses at least \((n-b-c_0)_+\) collars, while the retained localization part crosses the remaining \((k-n-c_0)_+\) collars. The metric here is the actual metric of the corresponding original or prepared map. LFR I p.179 gives **one \(M\)-cell layer** in the recent prepared history; it does not give \(MR_r\) there. The uniform physical lower width valid for both histories is therefore \(cMh_r\). Measured in the old carrier unit \(Mh_b\), its old-tree cost is at least \(c\) for \(r\ge b\); measured in the source scaled metric, its kernel part has cost at least \(cM\). The retained localization walk/volume part pays its corresponding current-scale connector with its own fixed \(\kappa_1-1\) reserve. Original unprepared portions have larger guards, but that improvement is not assigned to prepared portions. For \(n\le b\), the localization part alone pays the age. The fixed \(c_0\) includes the source star, endpoint and collar conventions.

The same path argument applies with the original record's free components: by (CR.5), every noninitial free traversal is charged to an adjacent outside segment with one fixed factor. Start at the first exit from the old anchor set, so no artificial canonical interior-root diameter is subtracted. The new attempted component is not yet contracted. For nested older tags, eligibility and (CR.18) give the same separation, as in (CR.19). Thus, with fixed \(c_*,C_*>0\), a reserved part \(\mathscr L_{b,k}\) of (CR.22a) obeys
\[
 \mathscr L_{b,k}\ge
 c_*\min\{\beta_{\rm s}\kappa,\delta M,
                    \kappa_1-1\}(k-b-c_0)_+,\qquad
 \mathscr L_{b,k}\ge c_*\rho_k(r,X)-C_*,
 \tag{CR.22b}
\]
where \(r\) is the actual current root/attachment being summed, and the second estimate is used with another fixed share. These inequalities are the source layer-crossing argument of BC16.29–30 applied to a **value-localization path**. No observable mark or derivative occurs in their proof.

After retaining the full invariant output weight and the primitive entropy shares, choose the admitted source block and localization parameters \(M,\kappa,\kappa_1\), in their original order, so that the remaining value-age rate \(\Gamma_{\rm v}\) satisfies
\[
 \Gamma_{\rm v}>4\log L+\lambda+\lambda_{\rm pol}+2.
 \tag{CR.22c}
\]
Here \(\lambda>0\) is the chosen age weight, and \(\lambda_{\rm pol}>0\) is any fixed rate paying the finite AF/prefix polynomials. CMP119 p.260 immediately after (2.31) states the freedom to take the fixed decay parameters arbitrarily large, with the other parameters chosen accordingly. CMP116 (1.7), (1.11) supplies the corresponding block-size/decoupling reserve: choose \(\kappa,\kappa_1\) first and then \(M\) so that they occupy only the chosen fixed fraction of the available \(\delta_1M\). Thus the minimum in (CR.22b) can exceed the fixed threshold in (CR.22c). This choice is made once, before the coupling ceiling or any derivative order. It uses positive fixed shares of (CR.22a), not a larger derivative rate or a fictitious running prepared collar. The source normalized kernel row sums control the attachment integration. The original root density is \(L^{4(k-b)}\). Consequently the contribution of the incoming anchored birth-\(b\) family to a fixed new root is bounded by
\[
 C(1+k-b)^B L^{4(k-b)}
       e^{-\Gamma_{\rm v}(k-b)}A_{b,k-1}
 \le C e^{-\lambda(k-1-b)}A_{b,k-1}.
 \tag{CR.22d}
\]
Summing this inequality over \(b<k\) is the value estimate which supplies the age-weighted input. The inherited ordinary source family has its separate fixed norm; it is not obtained by assigning a new small coefficient to every unchanged old scalar.

Let that ordinary E/R/full-tree B forcing constant be \(F_0\ge1\). The pre-exponentiation bounds are then at most a fixed multiple of \(F_0+\mathcal A_{k-1}\). The source's positive-root weakenings, such as \(c_1=\alpha^{1/3}\), do not preserve literal linearity. This causes no loss: on a fixed bootstrap interval for \(\mathcal A\), every fixed positive root \(0<r\le1\) satisfies
\((F_0+\mathcal A)^r\le F_0+\mathcal A\).
The corresponding root of the exponentially small coefficient is already included in (CR.16). Once the resulting elementary norm is below the fixed rooted-tree threshold, the two iterations in Section 7.3 change it by at most a fixed multiplier.

#### Chronological prefix forcing and the recurrence

The partially failed-prefix estimates are applied **before** the current completed-R output is constructed. Eligibility puts its **resident tag masses** at births at most \(h=k-N(k)\), in the untouched deep factor (1.76). Scalar families born outside the attempted component at an intermediate scale can have tails reaching it; those remain earlier-birth inputs \(b<k\), with their full carrier connectors. They are not assigned the stronger resident-tag restriction. Both classes are controlled by the induction hypothesis. The fresh prefix, failed-action and failed-Jacobian contributions have the bound proved in PF.22,
\[
 \varepsilon_k^{\rm PF}
 \le C g_k^{-2}(1+\ell_k)^{A_{\rm PF}}e^{-c_{\rm PF}R_k}.
 \tag{CR.22e}
\]
They multiply at most \(F_0+\mathcal A_{k-1}\). The coefficient may be weakened once to cover the finitely many positive roots in the ensuing connected sums; it still has the form (CR.22e), with fixed changed constants. It never uses the same-birth completed output as an input. Failure promotions change geometry only after these estimates.

Put
\[
 \zeta_k=
   \varepsilon_k^{\rm R}(1+R_k)^s
   +\varepsilon_k^{\rm PF}.
 \tag{CR.22f}
\]
The admissible \(R_k\ge\ell_k^r\), \(r>1\), makes \(\sup_k\zeta_k\to0\) when the common ceiling decreases. The fresh tagged and prefix contributions, followed by the successful normalized scalar output, therefore satisfy
\[
 A_{k,k}\le C_{\rm fresh}\,
      \zeta_k
      (F_0+\mathcal A_{k-1}).
 \tag{CR.23}
\]
The constant \(C_{\rm fresh}\) depends on the fixed source parameters and the chosen norm reserves. It does not depend on how many times an untouched record has previously been evaluated. The source's full-scale resummation in (1.49)–(1.68) supplies the linear incoming-action sum; the resolved atom/cell count in (CR.20) and the two rooted sums supply the additional tagged norm. Removed-component coverage is paid by the already present \(e^{-p_0(g_k)}\) term, so it adds no multiplicative factor to a carried family.

Take one fixed \(\lambda>0\) from the available age reserve, after the \(L^{4(k-b)}\) root count and fixed age polynomials have been paid, and define
\[
 \mathcal A_k
   =\sum_{b\le k}e^{-\lambda(k-b)}A_{b,k}.
\]
Use the total \(\zeta_k\) in (CR.22f). Equations (CR.22)–(CR.23) give
\[
 \mathcal A_k
 \le \bigl(e^{-\lambda}+C_{\rm fresh}\zeta_k\bigr)
             \mathcal A_{k-1}
       +C_{\rm fresh}F_0\zeta_k.
 \tag{CR.24}
\]
Choose the common ceiling so that
\[
 C_{\rm fresh}\sup_k\zeta_k
       \le\tfrac12(1-e^{-\lambda}),
 \qquad
 \rho:=\tfrac12(1+e^{-\lambda})<1.
\]
Then
\[
 \mathcal A_k\le\rho^k\mathcal A_0+
       \frac{C_{\rm fresh}F_0\sup_b\zeta_b}{1-\rho}.
 \tag{CR.25}
\]
Starting with no completed-R tagged families gives \(\mathcal A_0=0\); choose the ceiling once more to place this bound inside the fixed elementary threshold used in (CR.23). This closes the chronological induction, including the prefix forcing. The forcing tends to zero by (CR.17) and (CR.22e). There is no uncontrolled multiplication by \(C_{\rm fresh}\) at each age step, no repeated loss of the source rate, and no dependency on the same-birth completed output.

Old tags outside a new R component introduce no fresh integration factor: their scalar records are carried under (CR.22). Old tags inside it are included once in that component's complete positive operation and the fresh localization under (CR.23). On a failed prefix their original birth records remain in the explicitly untouched deep factor or in its already generated ordinary boundary terms; they are not counted again as newly normalized kernels. Promotion changes the incidence convention for a **future fresh** cluster; it does not enlarge the old scalar dependency sets or the old nodal gauge list. In the final current application the original root density \(L^{4(k-b)}\) is paid explicitly by the age reserve. If one instead collected every old record at a promoted root, monotonicity in (CR.22) would be false; that convention is not used.

Under the repeated-component and prefix majorants, the anchored norm (CR.10) and the derivative estimate of Proposition CR.3 apply to the scalar completed-R family with its actual tags. The complete conditional boundary estimate also requires the ordinary and unreplaced sectors.
