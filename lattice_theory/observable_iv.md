# Normalized early births, causal stencils, and restart histories

**Status.** This note obtains two further normalized inputs from the actual source construction. First, it identifies the soft Faddeev–Popov variables as predictable normalized gauge innovations, distinct from the fresh R-reset fluctuations of H8. Second, it traces ordinary P/Q/R births on unchanged causal patches to original Wilson plaquettes or those gauge innovations. This closes a growing prefix of later births. Restarting the H8 geometry after that prefix allows arbitrary ordinary births and preparation failures during the prefix, followed by clean unresolved evolution with arbitrary mergers. The result includes an ordinary-size exponential moment, a selected terminal old-field second moment, and the sharp two-root scale sum for this enlarged sector. There is also an all-depth conditional estimate for the explicit small-canonical-fluctuation part of Q/R births.

The length of the prefix tends to infinity as the microscopic coupling tends to zero, but is only a fixed small multiple of \(\log\log(g_0^{-2})\). No all-depth bound for later births or persistent failed preparations is asserted. The last section explains why the same argument does not remove that restriction.

All probabilities are under the frozen positive lift \(\Pi\). No history is divided by its own posterior mass. A gauge-fixing identity is used as a normalized auxiliary realization of the original source operation; the physical field, running couplings, and R-reset kernel are not replaced.

### 1. Units and source conventions

Put

\[
\beta=g_0^{-2},\qquad
h_j=aL^j,\qquad
s_j=Mh_jR_j,\qquad
Q=p_0(g_0)^2.
\tag{H9.1}
\]

Here \(R_j\) is the source radius, whereas the ordinary bad-fluctuation set is denoted below by \(R_j^{\rm bad}\) when a distinction is needed. The source parameters obey

\[
p_0(g)=A_0(\log g^{-2})^P,\quad P\ge5r,\quad r\ge2,\qquad
R_j\asymp(\log g_j^{-2})^r,\qquad
\varepsilon_j=g_jp_0(g_j),\quad
\delta_j=\frac{A_1}{A_0}\varepsilon_j .
\tag{H9.2}
\]

All constants may depend on the fixed group, \(L,M,M_2,A_0,A_1\), and the fixed logarithmic order of the observable. They do not depend on the cutoff, torus volume, or depth.

There is a source convention that matters here. The later LFR I formulas (1.8)–(1.9), printed p.178, use \(\exp(ig_jA_j)\) and the ordinary independent-coordinate radius \(g_j^{-1}\delta_j\). The detailed source chain identifies this with the inherited ordinary family. The literal earlier display CMP119 (3.16) has a rescaling mismatch; it is not silently read as a different cutoff. The first-step offset in CMP119 (1.18) is harmless below, since \(g_j^{-1}\delta_j\to\infty\): a threshold \(g_j^{-1}\delta_j-M_0\) is at least \(\delta_j/(2g_j)\) at the same sufficiently weak endpoint. None of these radii is the distinct preparatory \(\delta'_j/g_j\) radius or the true fresh-reset denominator radius of H8.

An ordinary birth at depth \(j\ge1\) means one of the source P/Q/R flags introduced in the transformation from \(V_{j-1}\) to \(V_j\). Its test cube has current physical size \(O(h_jR_j)\). An **unchanged causal patch** includes all original-field arguments of the deterministic block averages needed for that cube and its prescribed source enlargement. None of these arguments may have undergone a current-field replacement. This excludes the current-field integration in LFR I (1.76), including branches whose later preparation fails, as well as an accepted final R reset. Other histories outside the patch are unrestricted. This condition is imposed before taking probability; no conditional Wilson measure given this event is used.

This stronger condition has a source-level forward meaning. In the operations up to (1.71)–(1.75), the current \(V_k\) remains an external argument; the displayed integrations concern older fields, gauge variables, and exact changes of integration variables. Retaining the original mark under these transformations gives a positive lift whose current-coordinate kernel is the point mass at the same \(V_k\), up to gauge. LFR I p.193 explicitly identifies these as equalities for the density at fixed \(V_k\). The first current-field replacement is (1.76), where \(V_k|_\Lambda\) is integrated and the source switches to equality of total integrals. The later failures (1.82) and (1.88) can occur after that integration; p.200 says that some failed components retain operations of the form (1.76). They must not be treated as current-field pass-through steps. By induction, on the unchanged causal patch the actual \(V_j\) equals the ordinary \(j\)-fold block average of the original field, up to gauge. This conclusion uses the retained current-coordinate kernel, not equality of partition functions alone.

As in H8, the cofinal source tori are taken large enough for the fixed enlarged geometric neighborhoods to be contractible. This is a fixed enlargement of the source size condition, not an assumption that a winding flat connection has a global small-link gauge.

### 2. A threshold version of the original Wilson estimate

The H7-E proof works at any small threshold \(t>0\), not only \(t=\varepsilon_0\).

#### Lemma H9-A: specified original plaquettes

There are fixed \(c,C,t_*>0\) such that, for any family of distinct fine plaquettes \(\mathcal P\),

\[
\mu_0\!\left(\bigcap_{p\in\mathcal P}
 \{|U_0(\partial p)-1|\ge t\}\right)
\le \exp[-c\beta t^2|\mathcal P|]
\quad\text{if }0<t<t_*,\quad
\beta t^2\ge C(1+\log\beta).
\tag{H9.3}
\]

**Proof.** Use the literal source torus and fixed vertex tiles of side \(L\); the number of tiles in every direction is even. Among finitely many tile phases, a fixed fraction of the specified plaquettes can be assigned to distinct tiles in whose interiors they lie. The loss is a fixed constant depending on \(L,d\). In a tile use the reflection-invariant event that some wholly internal plaquette has defect at least \(t\). The completely disseminated event has Wilson action at least \(c t^2\) per tile. The all-link Haar-ball lower bound gives \(\log Z_\beta\ge-CN(1+\log\beta)\), and \(N/N_{\rm tile}=L^d\) is fixed. Wilson reflection positivity and the block chessboard inequality therefore give a cost \(c\beta t^2-CL^d(1+\log\beta)\) per selected tile. The stated hypothesis absorbs the second term and the finite extraction losses. This proves the claim. \(\square\)

This is the same original Wilson theorem as H7-E. It neither assumes nor proves reflection positivity of an effective or reset law.

The original marginal of \(\Pi\) is \(\mu_0\), so (H9.3) remains true with \(\Pi\) on the left. In particular it can be multiplied by restrictions on later histories and then used as an upper bound.

### 3. The actual soft gauge-fixing law

CMP119 (1.5), printed p.247, inserts an identity at each block point \(x\ne y\), where \(y\) is its block center. For fixed pre-gauge field \(V\), write

\[
r_x=V^u(y,x)=V(y,x)u(x)^{-1},\qquad u(y)=1 .
\tag{H9.4}
\]

Gauge covariance of the averaged contour variable follows from its endpoints. Haar invariance changes the integration variable \(u(x)\) into \(r_x\). Thus the identity is precisely the product of the probability measures

\[
d\nu_g(r)=z_g^{-1}
1_{\{|r-1|<\varepsilon\}}
\exp[-g^{-2}(1-\operatorname{Re}\operatorname{tr}r)]\,dr,
\qquad
z_g=\int 1_{\{|r-1|<\varepsilon\}}
e^{-g^{-2}(1-\operatorname{Re}\operatorname{tr}r)}\,dr .
\tag{H9.5}
\]

Here \(\varepsilon=\varepsilon_k\), \(g=g_k\) in the \(k\)-th ordinary step. The domain where the gauge-fixing identity is inserted is determined before this draw, after the P classification. In particular the normalized product law is valid conditionally on the entire physical past and that domain.

#### Lemma H9-B: normalized gauge innovations

There exist fixed \(c_1,C_1>0\) such that, uniformly at weak coupling,

\[
z_g\asymp g^{\dim G},\qquad
\int \exp\!\left[c_1\left|\frac{\log r}{g}\right|^2\right]
\,d\nu_g(r)\le C_1.
\tag{H9.6}
\]

Consequently,

\[
\nu_g(|r-1|\ge ug)\le C_1e^{-c_1u^2}.
\tag{H9.7}
\]

**Proof.** The cutoff is eventually inside a fixed exponential chart. In that chart the Wilson one-link function is bounded above and below by positive constants times \(|\log r|^2\), and the Haar Jacobian is bounded above and below. A ball \(|\log r|\le cg\) lies inside the cutoff because \(\varepsilon/g=p_0(g)\to\infty\), and gives the lower bound on \(z_g\). The full Gaussian integral gives its upper bound. Rescale \(\log r=gX\); the resulting normalized density is bounded by \(Ce^{-c|X|^2}\), proving both estimates. \(\square\)

For a specified space-time family of distinct, predictably used gauge coordinates, the tail estimates multiply by the tower property, even when their locations belong to different scales. If \(B_a\) is the specified large-innovation event and \(H_0\ge0\) is measurable before all the draws, then

\[
\mathbb E_\Pi\!\left[H_0\prod_a1_{B_a}\right]
\le
\mathbb E_\Pi H_0\prod_a q_a,
\qquad
q_a=C_1e^{-c_1u_a^2}.
\tag{H9.8}
\]

Coordinates not used in the actual source gauge-fixing domain can either be assigned event value zero, or furnished with unused independent copies of (H9.5). The latter is only an auxiliary realization and does not change a physical kernel.

The variables in (H9.5) are gauge innovations. They are not fresh R-reset fields, and a general failed preparation is not identified with them.

### 4. Deterministic pullback on an unchanged patch

The following deliberately coarse bounds keep their depth losses visible. An optimal curvature contraction is unnecessary for the finite prefix.

#### 4.1 One block average

There are fixed \(K_L,A_L\ge2\) and a small \(\epsilon_*>0\) with two properties for the source averages.

* If all plaquettes in the fixed \(O(L)\) determining neighborhood of a coarse plaquette have defect at most \(\epsilon<\epsilon_*\), then the coarse plaquette has defect at most \(K_L\epsilon\).
* If all input links in a fixed gauge have distance at most \(b\) from the identity, then all output links have distance at most \(A_Lb\), as long as the displayed bound remains in the fixed analytic chart.

For the first assertion, choose a coordinate-tree gauge on the finite contractible determining neighborhood. Every transformed link is a product of at most \(C_L\) transported elementary plaquettes, so its defect is at most \(C_L\epsilon\). The source contour averages and the finite group mean are analytic near the identity, preserve the identity, and are gauge covariant. Their derivative is bounded on one fixed smaller neighborhood. This gives the two assertions, after increasing the constants.

These properties follow directly for both displayed source averages, CMP109 (0.4) and (0.12), from their finite contour support and (0.5)–(0.9). They use only the regular branch. If the original field is sufficiently small on the patch, every intermediate average remains in that branch, so an arbitrary continuation on genuinely large fields is irrelevant to the implication.

Iteration gives

\[
\sup_{p'\subset D}|V_j(\partial p')-1|
\le K_L^j
\sup_{p\subset D^{\leftarrow j}}|U_0(\partial p)-1|,
\tag{H9.9}
\]

provided the right side is below the fixed chart radius. The backward support \(D^{\leftarrow j}\) has diameter at most \(CL^j\) times that of a unit current determining patch. This follows by summing the one-step support enlargements geometrically. On an unchanged causal patch the actual current field is this deterministic block average, up to gauge transformations, which leave the plaquette norm unchanged.

#### 4.2 The source local minimizing field

The ordinary P test is on the local background \(U_{j,\square}(V_j)\), rather than directly on \(V_j\). CMP119 (2.16), p.257, defines it by

\[
U_{j,\square}(V_j)
=U\!\left(\mathbf B_j(\square^{\sim4}),
 M^\bullet(Q_j^{s*}V_j)\right).
\tag{H9.10}
\]

The map \(Q_j^{s*}\), given in (1.3) and generalized immediately after (2.16), puts the identity on bonds inside a \(j\)-block and copies the corresponding \(V_j\) link across adjacent \(j\)-blocks. It is gauge covariant under the constant extension of a coarse gauge transformation to its blocks.

The copied map also gives a direct check on the mixed determining data. On nested source blocks, \(M(Q_\ell^{s*}V)=Q_{\ell-1}^{s*}V\): every contour in one averaging operation either stays inside one \(\ell\)-block and has transport one, or crosses its one relevant interface and has the identical transport \(V(c)\). The source mean returns that identical transport. Thus \(M^iQ_j^{s*}V=Q_{j-i}^{s*}V\). Plaquettes of these copied fields are identities or transported copies of coarse plaquettes; the prescribed mixed-level extension gives the same values at an interface. This verifies that there is no unexamined nonregular boundary datum in (H9.10). The coarser exponential estimate below is retained to avoid using any optimal constant from this identity.

Suppose the original plaquette bound on the backward patch is \(t\). First use (H9.9), then choose a coordinate-tree gauge on the enlarged current cube, of side \(O(R_j)\). Its \(V_j\) links obey

\[
\sup |V_j(b)-1|\le C(1+R_j)^2K_L^j t.
\tag{H9.11}
\]

The power two is a harmless upper bound for the number of plaquettes in the coordinate surfaces. The copied fine configuration has the same link bound. Every level-\(i\) average appearing in the mixed determining data in (H9.10), \(i\le j\), has link bound at most \(A_L^i\) times it. This also bounds the mixed plaquettes at a change of scale: their constituent variables are these same averages or their prescribed coarse extensions. Hence the regularity parameter for the determining data is bounded by

\[
e_{\rm data}\le C A_L^jK_L^j(1+R_j)^2t.
\tag{H9.12}
\]

CMP102, Theorem 1, printed pp.278–279, applies when this number is below its fixed admissibility radius. It gives

\[
|U_{j,\square}(\partial p)-1|
\le B_3e_{\rm data}L^{-2j}
\quad\text{on the central test region}.
\tag{H9.13}
\]

The region in (H9.13) is indeed in the depth-\(j\) part of the minimal determining set. CMP119 pp.256–257 constructs \(\mathbf B_j(\Omega)\) with the final domain containing the interior of \(\Omega\) after removal of two fixed \(M_1\) layers. The test region \(\square^\sim\) is separated from the boundary of \(\square^{\sim4}\) by several \(M_2R_j\) layers. Thus the requisite depth and margin hold uniformly.

No arbitrary-boundary minimizer has been introduced: this is exactly the local P-test background with the explicit copied determining data.

#### 4.3 Canonical approximate fluctuation

Set \(k=j-1\), and let \(V_{\square}^{(k)}=M^k(U_{j,\square})\), as in CMP119 (3.4). Use the block axial convention already present in the source Q test. This is a source identification, not a new gauge change of the comparison field: the first equality in CMP119 (3.9), p.266, explicitly uses \(V_{\square}^{(k)}(y,x)=1\) for the same averaged contour variable appearing in the gauge-fixing identity. The next display (3.10) imposes that same condition on the global comparison minimum. The actual source comparison can therefore be expressed as

\[
V_k^u(b)=r_{b_-}^{-1}V_k^{\,0}(b)r_{b_+},
\qquad r_y=1\text{ at block centers},
\tag{H9.14}
\]

where \(V_k^{\,0}\) is the canonical field with its averaged axial contour variables equal to one. The comparison field is independent of the current gauge innovations: its argument \(V_j\) is unchanged by the block gauge transformations fixing the coarse centers.

We use the elementary block-axial comparison behind CMP119 (3.13). Two regular fields on two neighboring blocks, with the same block average and the same axial condition, differ on their bonds by at most \(C_L\) times the sum of their plaquette bounds. One proof uses a tree gauge on each block: comparisons of different paths introduce at most \(C_L\) elementary plaquettes; the fixed coarse average identifies the remaining cross-block transport. The mean-contour axial gauge differs from the tree gauge by the same \(C_L\) plaquette bound. The estimate is gauge covariant and does not require the common coarse average to be the identity.

The fields \(V_k^{\,0}\) and \(V_{\square}^{(k)}\) have the same next average \(V_j\). Apply this comparison, (H9.9), and (H9.13); applying the first bound of §4.1 to the \(k\) averages of the latter only costs \(K_L^k\). Increasing one fixed \(D\ge2\) gives

\[
\sup_{b\text{ in the Q/R test region}}
|V_k^{\,0}(b)(V_{\square}^{(k)}(b))^{-1}-1|
\le C D^j(1+R_j)^2t.
\tag{H9.15}
\]

All intervening regularity parameters are small if the right side is made a fixed small multiple of \(\delta_k\). The enlarged test cube supplies the support margin for the averaged comparison fields. This is why a fixed exponential loss \(D^j\), rather than an unproved uniform-in-depth Lipschitz constant, is retained.

For unitary matrices (H9.14) gives the exact elementary estimate

\[
|V_k^u(b)(V_{\square}^{(k)}(b))^{-1}-1|
\le |V_k^{\,0}(b)(V_{\square}^{(k)}(b))^{-1}-1|
+|r_{b_-}-1|+|r_{b_+}-1|.
\tag{H9.16}
\]

### 5. Actual ordinary birth witnesses

Let \(a_j=\min(\varepsilon_j,\delta_{j-1})\) for \(j\ge1\). Choose the fixed small constant \(c_*\) below once, and define

\[
t_j=c_*a_jD^{-j}(1+R_j)^{-2},\qquad
\Gamma_j=\beta t_j^2 .
\tag{H9.17}
\]

#### Lemma H9-C: P/Q/R dichotomy

For each ordinary birth cube at depth \(j\) whose determining patch is unchanged, its bad flag implies at least one of:

1. some original fine plaquette in a patch of physical diameter \(Cs_j\) has defect at least \(t_j\);
2. some actual gauge innovation in the current test neighborhood satisfies
   \(|r_x-1|\ge c_*\delta_{j-1}\).

The number of possible fine witnesses is at most \(CL^{4j}(1+R_j)^4\), and the number of possible current gauge witnesses is at most \(C(1+R_j)^4\).

**P test.** If every fine plaquette is smaller than \(t_j\), (H9.12)–(H9.13), with \(c_*\) small enough, put the local background strictly below \(\varepsilon_jL^{-2j}\) on the source test region. Thus the P flag is good.

**Q test.** CMP119 (1.8) and (3.3) define the approximate-fluctuation bad flag by a bond defect at least \(2\delta_{j-1}\). Equations (H9.15)–(H9.16) exclude this when the original fine plaquettes are smaller than \(t_j\) and all the displayed innovations are smaller than \(c_*\delta_{j-1}\).

**R test.** The source R test is on the independent starred bond coordinates. The linearization of the averaging constraint changes only the distinguished \(b_0(c)\) bonds; on the independent bonds the physical logarithmic fluctuation is \(g_{j-1}A_{j-1}\). This is stated at the first step immediately after CMP119 (1.14), and the later step repeats the same construction. The ordinary bad cutoff therefore forces a physical fluctuation of size at least a fixed multiple of \(\delta_{j-1}\), including the first-step \(M_0\) offset.

The comparison background here is initially the global constrained minimum \(V^{(k)}\). CMP119 (3.17)–(3.19), pp.268–269, gives

\[
\sup_{b\in(\square^{\sim2})^{(k)*}}
|V^{(k)}(b)(V_{\square}^{(k)}(b))^{-1}-1|
\le C\varepsilon_k e^{-R_k}.
\tag{H9.18}
\]

The derivation uses the P/Q regular domain and the inner-cube margin, which are present before the R classification. It does not use the R-small condition. It therefore also applies to an R-bad cube. At the fixed weak endpoint its right side is less than any selected fixed fraction of \(\delta_k\). A large physical fluctuation relative to \(V^{(k)}\) consequently forces a comparable approximate fluctuation relative to \(V_{\square}^{(k)}\). Apply (H9.15)–(H9.16) again.

The subsequent localized changes of fluctuation variables retain the R characteristic functions; CMP119 explains this after (1.22), and repeats the construction after (3.21). Equivalently the argument labels the birth at the moment its cutoff is inserted and carries that label through the exact change of variables. It does not replace the actual R event by a new numerator cutoff. \(\square\)

The large innovation in this lemma is a normalized gauge draw, not an R-reset draw. The canonical physical approximate fluctuation can itself be large; no unconditional statement that every Q/R birth is a gauge artifact is made.

#### 5.1 A normalized Q/R sector at arbitrary depth

There is an additional consequence that does not require an unchanged past. Let \(\mathscr F_{k,\rm pre}\) contain the physical input, its next block average, the P-admitted gauge-fixing domain, and all history before the fresh ordinary gauge draw. For specified cubes \(\mathcal S\), let \(H_{\mathcal S}\) be the event that these cubes are P-admitted and their actual canonical approximate fluctuation
\(\sup|V_k^{\,0}(V_{\square}^{(k)})^{-1}-1|\)
is less than \(c_*\delta_k\). This is an explicit \(\mathscr F_{k,\rm pre}\)-measurable event, even when earlier resets occurred.

The Q argument in H9-C uses only this margin and (H9.16). For an actual R cube, the source P/Q domain supplies (H9.18) independently of how the earlier physical input was generated. Thus either bad flag on this carrier forces a large fresh gauge innovation. Conditional independence of the draw coordinates, a fixed cube extraction, and the \(O(R_{k+1}^4)\) witness count give

\[
\mathbb E_\Pi\!\left[
1_{H_{\mathcal S}}\prod_{C\in\mathcal S}
1_{\{Q_{k+1}\text{ or }R_{k+1}^{\rm bad}\text{ at }C\}}
\mid\mathscr F_{k,\rm pre}\right]
\le
1_{H_{\mathcal S}}e^{-c p_0(g_k)^2|\mathcal S|}.
\tag{H9.37}
\]

The weak threshold is independent of depth. For any nonnegative pre-draw old marked mass \(H_0\), the same right side multiplies \(\mathbb E[H_0 1_{H_{\mathcal S}}]\) after averaging. This is an actual normalized sector estimate. It leaves the complementary event of large canonical physical fluctuation untouched and does not by itself convert a microscopic old marked norm into a current-scale norm.

#### Theorem H9-D: normalized same-scale ordinary birth families

Let \(\mathcal S\) be any specified family of current ordinary birth cubes. Let \(E_{j,C}^{\rm ord}\) require an actual P, Q, or R birth at \(C\), together with the unchanged causal-patch condition. If
\(\Gamma_j\ge C(1+\log\beta+j+\log(1+R_j))\) and
\(\Gamma_j\le C_0p_0(g_{j-1})^2\) for a fixed \(C_0\), then

\[
\boxed{\quad
\Pi\!\left(\bigcap_{C\in\mathcal S}E_{j,C}^{\rm ord}\right)
\le e^{-c\Gamma_j|\mathcal S|}.
\quad}
\tag{H9.19}
\]

**Proof.** A fixed geometric coloring selects a fixed fraction of the current cubes whose enlarged witness patches are disjoint. The coloring constant is independent of \(j,R_j\): each enlargement is only a fixed multiple of a cube of that same scale.

For every selected cube use the dichotomy H9-C. First choose which cubes use original-field witnesses and which use gauge witnesses. Choose one witness in each. Fine witnesses from different selected cubes are distinct, and so are the chosen current gauge coordinates. The specified original-field events are measurable before all the gauge draws. Apply (H9.3) to them and (H9.8) to the gauge witnesses. At weak coupling the latter cost
\(\exp[-c p_0(g_{j-1})^2]\), which is at least as strong as \(\exp[-c\Gamma_j]\) in the early range below. The choices of types and witnesses cost at most
\(\exp[C(j+\log(1+R_j))|\mathcal S|]\).
Absorb that entropy and the coloring loss. The unchosen exterior histories have total conditional mass at most one. \(\square\)

Both numerical hypotheses hold throughout the prefix of §6 at a sufficiently weak endpoint. Outside that range one may instead retain the minimum of the original-field and gauge costs, provided that minimum pays the entropy. Nothing in this proof conditions the original Wilson law on an effective field, a gauge flag, or a history.

### 6. A growing prefix with one uniform normalization budget

Choose a fixed \(\kappa>0\) small enough that

\[
\alpha:=2P-4r-2\kappa\log D>4r+1,
\qquad
J=\left\lfloor\kappa\log\log\beta\right\rfloor .
\tag{H9.20}
\]

Such a choice exists since \(P\ge5r\) and \(r\ge2\). For the frozen AF trajectory, the ordinary source coupling/radius comparisons in CMP119 (2.6)–(2.9) give, throughout \(0\le i\le J\),
\(g_i\asymp g_0\), \(p_0(g_i)\asymp p_0(g_0)\), and \(R_i\asymp R_0\). In particular all the deterministic comparison charts used above remain admitted.

Let

\[
t_*^{(J)}
=cD^{-J}(1+R_0)^{-2}
\min\{\varepsilon_0,a_1,\ldots,a_J\},
\qquad
\Gamma_*=\beta(t_*^{(J)})^2.
\tag{H9.21}
\]

After decreasing the fixed \(c\), this threshold is no larger than every one used in H9-C, including the initial P0 threshold. Its size is

\[
\Gamma_*\asymp
Q\,D^{-2J}(1+R_0)^{-4}
\ge c(\log\beta)^\alpha,
\qquad
\frac{\Gamma_*}{R_0^4+J+\log\beta}\longrightarrow\infty .
\tag{H9.22}
\]

For later all-order use there is also the useful exact growth consequence

\[
\Gamma_*\ge c e^{\gamma J},
\qquad
\gamma=\frac{2P-4r}{\kappa}-2\log D>0.
\tag{H9.23}
\]

The floor in \(J\) changes only constants. Making \(\kappa\) smaller increases \(\gamma\).

#### 6.1 Hybrid witnesses at several prefix depths

A specified family of original fine plaquette witnesses at threshold \(t_*^{(J)}\), together with distinct gauge innovations at any depths at most \(J\), has probability at most

\[
\exp[-c\Gamma_*(N_{\rm fine}+N_{\rm gauge})].
\tag{H9.24}
\]

For the fine part use (H9.3). For the gauge part use (H9.8) in chronological order, with the original fine event as the initial multiplier. The gauge costs are uniformly \(\exp[-cQ]\), hence stronger than the displayed cost. Distinct gauge coordinates can have different depths and need no spatial independence beyond their actual conditional product/tower property.

It is not legitimate to infer (H9.24) from a same-scale birth bound alone. The witnesses and their distinctness are retained explicitly.

### 7. Restart after arbitrary early ordinary births and failed preparations

Define \(\mathscr A_J^{\rm pre}\) as the union of current source active cells belonging to unresolved components with the following prefix properties:

* every ordinary creation in their ancestry is an initial P0 creation or one of the ordinary P/Q/R creations at depths at most \(J\);
* every such later birth has the unchanged causal patch specified in §1;
* no successful reset has occurred in their selected unresolved ancestry.

All preparation failures during the prefix are allowed. They need not be interpreted as fresh innovations and are not assigned separate independent probabilities. The corresponding attempted active component is retained geometrically. A failure occurring after (1.76) can already involve a replacement of some current physical variables; this is permitted inside the prefix ancestry, but a later ordinary birth whose backward stencil uses those variables fails the separate unchanged-patch condition. Other histories elsewhere are unrestricted.

The unchanged-birth-patch condition is stronger than merely saying that the newly born component has not yet completed a reset: either a previous accepted reset or a failed post-(1.76) replacement can lie in a backward determining patch. Such a birth patch is excluded here.

#### Lemma H9-E: normalized restart occupancy

For every specified family \(\mathcal S\) of current \(MR_J\)-cells,

\[
\boxed{\quad
\Pi(\mathcal S\subset\mathscr A_J^{\rm pre})
\le e^{-c\Gamma_*|\mathcal S|}.
\quad}
\tag{H9.25}
\]

**Proof.** Trace a selected occupied cell backward through the actual covers, fixed layers, and bounded rectangular fills until an ordinary creation is reached. Before a successful reset these operations have finite propagation, as in H8. A failed preparation retains a component and does not insert a new distant active region. Thus an ordinary ancestor birth occurs within physical distance \(Cs_J\) of the selected cell. Its original fine or gauge witness from H9-C is within the same enlarged neighborhood, after increasing \(C\). The source radius comparisons and \(\sum_{i\le J}s_i\le Cs_J\) are used here.

A fixed coloring selects a fixed fraction of the current cells with disjoint enlarged physical neighborhoods. Their selected witnesses are therefore distinct fine plaquettes or distinct space-time gauge coordinates. This is true even if their ancestor births occurred at different depths.

Within one enlarged neighborhood, the number of original fine plaquettes is at most \(CL^{4J}(1+R_0)^4\). The number of potential gauge coordinates at all prefix depths is bounded by the same expression times a harmless fixed or polynomial-in-\(J\) factor, since the counts form a geometric sum. Hence witness choices cost at most \(\exp[C(J+\log(1+R_0))]\) per selected cell. Apply (H9.24) and absorb this entropy using (H9.22). There is no count of the full histories or of the preparation failures. \(\square\)

The initial cells in this restart theorem are actual active cells at depth \(J\). They are not required to be initial P0 cubes and can have arisen from the later ordinary births or from an expanding component during the prefix.

#### Theorem H9-F: normalized clean evolution after the prefix

For \(j\ge J\), let \(\mathscr A_j^{\rm pre,cl}\) be the unresolved descendants of the restart class, allowing arbitrary mergers within that class, but with no later ordinary birth, no failed preparation after \(J\), and no successful reset in the selected ancestry. Choose the clean-window length

\[
w_J=\lceil C_RR_J\rceil+u_0(D_{\rm geom})+C_w .
\tag{H9.26}
\]

Then

\[
\boxed{\quad
\Pi(\mathcal S\subset\mathscr A_j^{\rm pre,cl})
\le
\exp[-c\Gamma_*2^{\lfloor(j-J)/w_J\rfloor}|\mathcal S|].
\quad}
\tag{H9.27}
\]

**Proof.** The deterministic two-witness proof H8-A does not depend on what caused the active cells at its base time. After \(J\) the selected evolution has exactly its finite propagation, small-envelope, successful-preparation, and merger properties. A component confined to a bounded collection becomes small and resets after the same source clean window. Every unresolved cell therefore produces the H8 binary witness tree rooted now at time \(J\), with distinct current-\(J\) leaves. Use (H9.25) for the leaf family. The embedding entropy is \(\exp[Cw_JN]\), and \(\Gamma_*/w_J\to\infty\) by (H9.22). The source geometry and initial-time indexing only change fixed constants in the exponent. \(\square\)

### 8. Ordinary size, selected old means, and the sharp two-root sum

Let \(Y\) be a connected active component of the class in H9-F, let \(m_j(Y)\) count its \(MR_j\)-cells, and let \(\ell_j(Y)\) count an ordinary localization size in fixed \(M\)-blocks. Thus
\(\ell_j(Y)\le C R_j^4m_j(Y)\).
The ordinary lattice-animal count and (H9.27), with
\(\Gamma_*\gg R_0^4\), give, for each fixed \(\lambda\),

\[
\mathbb E_\Pi\sum_{Y\ni x}
e^{\lambda\ell_j(Y)}
\le
C_\lambda
e^{-c\Gamma_*2^{\lfloor(j-J)/w_J\rfloor}}.
\tag{H9.28}
\]

The notation selects active components, rather than arbitrary additional supports created by a signed polymer expansion.

Let a deterministically centered old microscopic seed obey

\[
|F_0(x)|\le A_xa^{-4}T(a)^s,\qquad T(h)=1+\log(1/h).
\tag{H9.29}
\]

The prefix and post-prefix engineering losses satisfy

\[
L^{8j}\left[\frac{T(a)}{T(h_j)}\right]^{2s}
\le \exp[C_s(J+(j-J))]
\le \exp[C_sJ+C_sw_J2^{\lfloor(j-J)/w_J\rfloor}].
\tag{H9.30}
\]

Equation (H9.22) pays both terms with a fixed fraction of the rare reserve. Consequently

\[
\boxed{\quad
\mathbb E_\Pi\sum_{Y\ni x}|F_0(x)|^2e^{\lambda\ell_j(Y)}
\le
C_{\lambda,s}A_x^2h_j^{-8}T(h_j)^{2s}
e^{-c\Gamma_*2^{\lfloor(j-J)/w_J\rfloor}} .
\quad}
\tag{H9.31}
\]

For any retained sigma algebra \(\mathscr G_j\), conditional Jensen therefore gives the actual selected old-mean estimate

\[
\left\|
\mathbb E_\Pi[1_{\{x\in\mathscr A_j^{\rm pre,cl}\}}F_0(x)
\mid\mathscr G_j]\right\|_2^2
\le
C_sA_x^2h_j^{-8}T(h_j)^{2s}
e^{-c\Gamma_*2^{\lfloor(j-J)/w_J\rfloor}} .
\tag{H9.32}
\]

This includes roots first swallowed during the prefix. It does not divide by the probability of that event, nor replace the old seed by a freshly sampled field. At terminal scale, restore the factor \(\ell_0^{-8}\) in the squared norm, exactly as in H8.

For two roots at periodic separation \(r>0\), write \(C_j(x,y)\) for the event that one component of this class contains both support collars. The same animal argument gives

\[
\Pi(C_j(x,y))
\le
C\exp\!\left[
-c\Gamma_*2^{\lfloor(j-J)/w_J\rfloor}
\left(1+\frac{r}{h_jR_j}\right)\right].
\tag{H9.33}
\]

Use part of the first exponent to pay (H9.30), retain the spatial exponent, and use \(R_j\le CR_0\). The geometric scale sum of
\(h_j^{-8}T(h_j)^{2s}e^{-cr/(h_jR_0)}\)
is bounded by
\(C_sr^{-8}T(r)^{2s}R_0^8(1+\log R_0)^{2s}\).
The remaining \(\Gamma_*\) reserve absorbs the displayed radius factors. Therefore, in terminal units \(0<r\le1\),

\[
\boxed{\quad
\sum_{j\ge J}
\mathbb E_\Pi[1_{C_j(x,y)}|F_0(x)F_0(y)|]
\le
C_sA_xA_y\,r^{-8}T(r)^{2s}e^{-c\Gamma_*}.
\quad}
\tag{H9.34}
\]

The corresponding selected conditional covariance follows by using the deterministic seed envelopes inside the selected conditional law and retaining its posterior probability, as in H8. The proof does not use an invalid inequality between a product of posterior means and a conditional product.

### 9. A direct normalized strict-extension-failure estimate

The preceding restart theorem does not need to attach an independent probability to every early preparation failure. There is nevertheless a separate concrete consequence for the strict extension selector.

LFR I, printed p.193 after (1.75), proves pointwise that failure of \(\chi_{j,\Lambda}\) forces

\[
|V_j(\partial p')-1|\ge c(B_3,M)\varepsilon_j
\quad\text{for some }p'\subset Z\cap\Lambda^c.
\tag{H9.35}
\]

The offending plaquette is retained outside the resampling domain. If its full backward determining patch is unchanged, (H9.9) traces it to an original fine plaquette with threshold
\(c\varepsilon_jK_L^{-j}\), which is stronger than the conservative threshold (H9.17).

For a family of eligible components at specified distinct canonical anchor cells, each contained in its source \(100MR_j\) cube, one can extract a fixed fraction with disjoint enlarged witness patches. If all potential offending retained plaquette patches are unchanged, (H9.3) and the witness count give

\[
\Pi(\text{all selected strict extension failures})
\le e^{-c\Gamma_jN}
\qquad (j\le J).
\tag{H9.36}
\]

The count \(N\) is the number of selected components before the fixed extraction loss. Other preparation or gauge/derivative failures do not inherit (H9.35). A terminal old-mean estimate at these prefix scales follows directly from the deterministic seed envelope, the age cost \(e^{C_sj}\), and Jensen, with \(\Gamma_j\) paying the age.

This is an annealed normalized failure theorem. Given the offending retained exterior itself, the source failure may still have conditional probability one. There is no contradiction.

### 10. What remains in boundary surgery and at deeper scales

The arguments above make three parts of a broader strategy concrete:

1. A strict failed extension has an actual retained coarse-plaquette witness, (H9.35).
2. On an unchanged causal patch that witness, and the canonical ordinary birth fields, have a quantitative original-field pullback, with the explicit loss \(D^j\).
3. Ordinary gauge contributions have their own exact normalized causal tails, (H9.6)–(H9.8).

At depths comparable to the full UV hierarchy, the threshold \(t_j\) becomes too small for \(\beta t_j^2\) to dominate even the fine-tile entropy \(C\log\beta\). The present deterministic supremum pullback therefore cannot prove normalized birth rarity there.

Enlarging a failed reset patch to include its offending retained plaquette is a plausible next comparison, but it changes what is conditioned on. H8's finite-patch excess-energy theorem then requires an actual local conditional density, a lower bound near a constrained minimum with the same new exterior, and an excess-energy gap for the bad set relative to that minimum. The source fresh-reset denominator only supplies this information after its good-selector restrictions have been met. It does not supply it for an arbitrary failed exterior.

The all-depth unmarked stability statement also does not by itself give the needed constrained numerator with the same ultraviolet normalization as a useful lower bound. A coarse chessboard strategy would require that relative constrained estimate, as well as reflection factorization of the actual frozen coarse law. The R-reset normalizer and its geometry need not factor across a reflection plane; positivity alone is insufficient.

For causal patches containing earlier successful resets, the inherited minimizing background can itself carry a coarse defect. The Gaussian tails for the fresh fluctuation do not bound that background without a boundary response or excess-energy estimate. Its old marked conditional mean also survives the reset as a function of the retained boundary, as proved in H8's screening identity.

Thus the present additional closure consists of the explicit prefix sector H9-F, the actual gauge innovation theorem, and the strict-extension-failure consequence. Later births at arbitrary depth, persistent failed preparations after the prefix, mixed boundary response, and the covariance of different history-sector means remain necessary for full Gate 3 and full S2.

### 11. Sources and relation to the companion notes

The new elementary estimates in §§2–8 are derived here. Their source identifications use:

* **CMP109 (1987), pp.252–254:** finite contour support, gauge covariance, analytic group means, and the displayed block averages (0.4) and (0.12).
* **CMP102 (1985), pp.278–279, Theorem 1:** regular mixed determining data and the depth-dependent curvature bound for its unique regular minimal orbit.
* **CMP119 (1988), pp.246–250, 256–257, 265–269:** P/Q/R definitions; the copied local background (2.16); the actual normalized soft gauge identity (1.5); canonical block axial comparisons; independent starred coordinates; and the global/local background estimate (3.17)–(3.19).
* **LFR I (1989), pp.178, 183, 187:** the final ordinary rescaled cutoff convention and its inherited family; **pp.192–194:** the actual strict extension selector, its retained plaquette witness, and the subsequent minimization.
* **LFR II (1989), pp.384–387:** the covers, bounded fills, clean windows, and component processing underlying H8's geometric restart.
* **Brydges–Fröhlich–Seiler, On the Construction of Quantized Gauge Fields I, original 1978 preprint, Theorems 2.8 and 2.10:** Wilson reflection positivity and chessboard on compatible periodic lattices, as already used in H7.

The separate root module R9 proves all-order bounds for clean components with roots retained from its base time. Its §7, Theorem R9-D and (R9.16)–(R9.20), now applies H9-E's restart law at time \(J\). Equation (H9.23), with \(\kappa\) chosen so that \(\gamma\ge D_s\), pays every microscopic age before \(J\) with at most one additional factorial. The resulting normalized products have bounds with factorial powers five for bare dimension-four seeds and six for seeds with a fixed logarithmic envelope; posterior-weighted selected cumulants have powers six and seven, respectively. These all-order bounds retain a factor \(e^{-c\Gamma_*}\) and a weak-coupling threshold independent of the order. They are proved by the separate joint witness argument, not inferred from the second-moment theorem (H9.31). Their unchanged-causal-patch restriction includes the exclusion of current-field integration (1.76) on every ordinary-birth stencil, even on a branch whose later preparation fails.

---
