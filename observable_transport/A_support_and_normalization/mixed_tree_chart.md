# A finite mixed physical chart with the exact gauge weights retained

This note proves a polynomial coordinate bound on a finite, admitted mixed determining region, and an exact change of the source's normalized axial gauge variables. It uses the single graded connection GR.1. It does not identify the complete two-history restored density with a Gaussian, and does not discard gauge-dependent selectors. The distinction matters: a small physical curvature does not make an arbitrary gauge representative a small link field.

The intended source application is the first-birth, globally P/Q-regular R-only family, with the first microscopic birth variables already factored as in LE.4. The two later annular lists have the common mixed refinement of [M04 Two List Common Refinement](M04_Two_List_Common_Refinement.md). Its full raw/free rank is `D≤C R^5`. The source waiting depth remains `N=R`.

## 1. The finite region and the counted cover

Let B be a convex current-scale box containing the two refined lists and their fixed source collars. The geometric assumptions needed here are explicit:

1. B lies in an admitted regular determining neighborhood. No arbitrary strong specified field is crossed by the surfaces used below.
2. The aligned mixed decomposition of B has a cover by at most `C D` convex cells Q. For each Q, its diameter is at most `C h_Q`, where `h_Q` is its native mesh, and neighboring mesh sizes differ by at most the fixed source factor. The fixed halos needed for GR are included.
3. The retained boundary vertices are connected by fixed retained edges in B, or in an included fixed boundary collar, using at most `C D` edges. The two fields being compared agree on those edges.

These assumptions have a direct verification for the two-hole, first-birth geometry whenever its containing box is in the stated all-regular neighborhood. Decompose each source shell into its own native blocks, intersect the two aligned decompositions, and retain the fixed incidence collar. Intersections choose the finer of two nested grids; the shell and ordinary-free counts are bounded by the union counts in CR.3–CR.5 of the common-refinement note. Fill the remaining portion of the containing box with current-scale cells. Its current volume is `O(R^4)`. Balancing the finite interfaces and adding their fixed halos multiplies the count only by a fixed L-dependent constant. Thus this construction uses `O(R^5)` graded cells, not all microscopic cells in the box. A boundary collar of current cells gives a connected retained boundary graph when the actual retained exterior is connected there.

The regularity of a field on this refinement is a separate admission condition. The rank statement alone does not prove that arbitrary variables restored from a different history are regular. In particular, applying this chart to the whole common probability measure requires a source cutoff enclosure or a controlled complement. That probabilistic step is not inferred below.

Write the graph constructed in GR Sections 2–3 as `G=(V,E)`. Its edges are the subdivided determining edges and their exact connectors. It has at most `C D` vertices and edges. On Q, the actual graded connection associated with regular data U satisfies

\[
 \|F_U(x)\|\le C\varepsilon h_Q^{-2}.
 \tag{MT.1}
\]

For a reference field U_* satisfying the same admission, use the corresponding connection and the same geometric graph and cover. Both connections reproduce every determining-edge product exactly. In the first quiet window one can take a common ceiling `ε=C g_k P(g_k)` with fixed constants, using the source coupling comparison over `N=R` steps. More generally all bounds below use the maximum of the native ceilings on this finite list.

## 2. A polynomial holonomy estimate without a microscopic filling

### Lemma MT.1

For a closed graph walk γ with q edges in B,

\[
 \|U(\gamma)-I\|\le C qD\varepsilon.
 \tag{MT.2}
\]

The same statement holds for U_*.

**Proof.** Choose a point o in B and cone each geometric edge of γ to o. There are q Euclidean triangles, with multiplicities retained. Every triangle lies in B by convexity. A triangle intersects each convex cell Q in a convex planar set of area at most `C h_Q^2`. Therefore

\[
 \int_{\text{one triangle}}\|F_U\|\,dA
 \le\sum_Q C\varepsilon h_Q^{-2}h_Q^2
 \le C D\varepsilon.
 \tag{MT.3}
\]

Bounded overlap of the cover changes only the constant. Cells are counted at their native scales; no factor involving the ratio of largest to smallest mesh occurs.

The holonomy variation formula on a parametrized disk gives
`||Hol(∂Σ)−I||≤∫_Σ ||F||`: differentiate parallel transport along the radial family, insert its curvature, and use the fact that all intervening real transports are unitary. It applies to the pullback bundle on each triangle even if the ambient connection was described in several local frames. Multiplying the triangular boundary holonomies cancels the internal cone paths. The norm of a product of unitary matrices minus I is at most the sum of their individual defects. Summing (MT.3) proves (MT.2). Degenerate triangles follow by a limit. ∎

This argument supplies the needed filling estimate from the proved continuous graded connection. It does not postulate a polynomial combinatorial filling area in the mixed graph.

## 3. A gauge fixing every retained boundary vertex

Choose a spanning tree T_B in the fixed retained boundary graph. Extend it to a spanning tree T of G. Equivalently, the remaining edges of T form a forest F, with every interior vertex connected to one retained boundary root. This can be done without placing a second retained root in the same component of F. Let o be the root of T_B. For x in V denote by

\[
 t_x(U)=U(T:o\to x),\qquad t_x(U_*)=U_*(T:o\to x)
\]

the ordered products on the chosen tree path. Set

\[
 g_x=t_x(U_*)^{-1}t_x(U).
 \tag{MT.4}
\]

Use the convention `U^g_{xy}=g_x U_{xy}g_y^{-1}`. Then

\[
 U^g_e=U_{*,e}\quad(e\in T),\qquad
 g_x=I\quad(x\text{ retained on the boundary}).
 \tag{MT.5}
\]

The second assertion uses the agreement of U and U_* on T_B. It preserves every retained boundary edge, including those not in T_B.

For a non-tree edge e=(x,y), write

\[
 L_e(U)=t_x(U)U_e t_y(U)^{-1}.
\]

This is the holonomy of a loop with at most `2|V|+1≤C D` graph edges. Direct multiplication gives

\[
 U^g_e U_{*,e}^{-1}
 =t_x(U_*)^{-1}L_e(U)L_e(U_*)^{-1}t_x(U_*).
\]

Lemma MT.1 therefore yields

\[
 \boxed{\quad
 \|U^g_e U_{*,e}^{-1}-I\|\le C\varepsilon D^2
 \quad\text{for every graph edge }e.
 \quad}
 \tag{MT.6}
\]

For `C εD²<c_G`, where c_G is a fixed injectivity radius, the unique small Lie logarithm exists:

\[
 U^g_e=\exp(i g_k a_e)U_{*,e},\qquad
 \|a_e\|\le C\frac{\varepsilon}{g_k}D^2
             \le C P(g_k)D^2.
 \tag{MT.7}
\]

The coordinates on F are zero. The remaining physical coordinates are on the free nonforest edges. This is polynomial in R and P when `D≤C R^5`; `g_k P(g_k)D²→0`. There is no `L^N` or `C^N` chart-radius loss.

The boundary-connectivity assumption is necessary for this conclusion in its stated form. A flat connection on an interval can have arbitrary endpoint-to-endpoint transport when both endpoints are fixed but no path of fixed edges connects them. Such a transport cannot be gauged away by fixing both endpoints. Likewise, noncontractible torus cycles require their actual holonomy coordinates; they are not controlled by a cone lying in a convex box. This note neither removes those modes nor counts them as small curvature effects.

## 4. Polynomial derivatives of this coordinate change

The forest products (MT.4) involve at most `C D` original graph matrices and inverses. Each connector of GR.3 involves at most a fixed number depending on L of original determining matrices. Hold the reference fixed, or regard its graph matrices as a second independent raw copy. On real unitary data, differentiating a product places the derivative in one factor and leaves all other factors with norm one. Thus, for m specified raw left-invariant directions, the mth derivative of any forest product is bounded by

\[
 m!(C D)^m\prod_{j=1}^m\|\delta_j U\|_\infty.
 \tag{MT.8}
\]

The same bound, with a new constant, holds for the logarithms of the relative chord matrices as long as (MT.6) is in a fixed smaller logarithm ball. One direct justification is to complexify each raw matrix by a left perturbation of size `c/D`. All products remain uniformly bounded, the relative chord matrices remain in the fixed logarithm domain, and Cauchy gives (MT.8).

If the directions use the native normalized increments `exp(i g_j δa_j)`, and `g_j/g_k` is bounded on this source window, the derivatives of the normalized logarithms have the bound

\[
 \|d^m a\|\le m!(C D)^m g_k^{m-1}
                  \prod_{j=1}^m\|\delta a_j\|_\infty.
 \tag{MT.9}
\]

This is a bound for the explicit forest/connector/logarithm map. It does not yet bound the composition with every historical variational reconstruction, a reference depending on the retained data, a constraint correction or a test map. Those maps must be included in a common-chart analysis; a bound on (MT.9) is not a substitute for that analysis.

## 5. Exact Haar pushforward, with no gauge-invariance assumption

Let E_B be the fixed boundary edges. Regard the remaining graph matrices as independent Haar variables for this statement. Let `G_int=G^{V\setminus B}` be the interior gauge group, with normalized Haar measure. Given g in this group and free matrices h_e on `E\setminus(E_B∪F)`, set h_e=U_{*,e} on F, retain the fixed boundary h, and define

\[
 U_{xy}=g_x^{-1}h_{xy}g_y,
 \qquad g=I\text{ on }B.
 \tag{MT.10}
\]

Then the exact measure identity is

\[
 \prod_{e\notin E_B}dU_e
 =\left(\prod_{x\notin B}dg_x\right)
   \left(\prod_{e\notin E_B\cup F}dh_e\right).
 \tag{MT.11}
\]

To prove it, solve outward from the roots of F. For a new child vertex, its forest edge identifies its gauge matrix by a left/right translate and possibly inversion. Haar invariance gives Jacobian one. After these substitutions, each remaining edge changes by left and right multiplication at fixed g, again preserving Haar. The procedure is triangular.

The graph connector change is also triangular Haar: the new connector is the original higher edge multiplied by a known lower path inverse. Order the native levels from lower to higher. Each such substitution has Jacobian one conditional on the lower entries. Thus (MT.11) applies after the actual mixed graph subdivision, not merely to an unrelated abstract graph.

For **every** integrable function Ψ of the fields and additional variables ξ,

\[
 \int\Psi(U,\xi)\,dU\,d\xi
 =\int\Psi(g^{-1}hg,\xi)\,dh\,dg\,d\xi.
 \tag{MT.12}
\]

No gauge invariance of Ψ was used. In particular its complete action, coarea factors, normalized soft-gauge weights, primitive Q/R selectors, preparation selectors and all gauge auxiliaries must remain in the pullback. Declaring the scalar gauge invariant does not justify deleting the g-dependence of those other factors.

If the source measure has already imposed a hard axial gauge or integrated a gauge sampler, first restore its exact normalized Faddeev–Popov identity, or retain its delta and Jacobian in Ψ. Formula (MT.11) is not permission to count an already removed gauge direction twice. The full common-refinement disintegration must decide this bookkeeping before using these coordinates.

On the small physical chart, `h_e=exp(i g_k a_e)U_{*,e}` has its ordinary Haar Jacobian `c_G g_k^{dim G}j(g_k a_e) da_e`. These factors and the corresponding source normalization constants are retained. The compact gauge coordinates in (MT.11) have not been assumed small.

## 6. The actual source soft axial coordinates are small independent variables

The compact gauge coordinates have a more useful parametrization when the literal source gauge sampler is present. This is an exact statement for the Euclidean invariant axial mean used in the source, not a replacement by one chosen tree path.

For x in a block B(y), let

\[
 C_{yx}(U)=M\{U(\Gamma):\Gamma\in\mathcal G(y,x)\}
\]

be the averaged contour matrix of CMP109 printed p.253, (0.11). Property (0.6) of that average implies exact endpoint covariance:

\[
 C_{yx}(U^u)=u_y C_{yx}(U)u_x^{-1}.
 \tag{MT.13}
\]

At fixed U and fixed center gauge u_y define, independently for every x≠y,

\[
 w_x=u_y C_{yx}(U)u_x^{-1},\qquad
 u_x=w_x^{-1}u_y C_{yx}(U).
 \tag{MT.14}
\]

Since left/right translations and inversion preserve Haar,

\[
 \prod_{x\ne y}du_x=\prod_{x\ne y}dw_x.
 \tag{MT.15}
\]

The source sampler CMP119 printed p.247, (1.5), becomes exactly

\[
 \prod_{x\ne y} d\gamma_j(w_x),\qquad
 d\gamma_j(w)=Z_j^{-1}\mathbf1_{\{\|w-I\|<\varepsilon_j\}}
          \exp[-g_j^{-2}s(w)]\,dw,
 \quad s(w)=1-\operatorname{Re}\operatorname{tr}w.
 \tag{MT.16}
\]

This law is independent of the physical U and is normalized by the original Z_j. The original contour average is defined because the native physical field is in the regular block domain. It need not itself be close to I in an arbitrary representative; endpoint covariance suffices for the change of variables.

For any remaining integrand F, including gauge-dependent tests, the exact identity is

\[
 \int\prod_{x\ne y}du_x\,
       \prod_{x\ne y}Z_j^{-1}\chi(C_{yx}(U^u))
                   e^{-s(C_{yx}(U^u))/g_j^2}\,F(U^u)
 =\int\prod_{x\ne y}d\gamma_j(w_x)\,
                   F\bigl(U^{u(U,w)}\bigr).
 \tag{MT.17}
\]

One may pad an absent sampler with the same independent normalized γ_j law. Integration of that unused variable is exactly one. This does not replace either history's gauge law by free Haar or by an unnormalized Gaussian. In the common refinement both histories' required auxiliary samplers can be retained with their own labels; each actual test is evaluated using the corresponding reconstructed `u(U,w)`.

LFR I printed p.182 states that the gauge terms (1.5), (1.6) are included in ζ in the annular operation (1.25), and introduces them on the remaining center-fixed region by the Faddeev–Popov procedure. Thus (MT.17) applies to those exact normalized factors. Hard axial gauges are the corresponding fixed-w case when that authorized source variant is actually being used; they are not silently substituted for the soft convention.

There is also a local analytic Gaussian description of each γ_j. On its small support put `w=exp(i g_j ξ)`. With the fixed invariant quadratic form κ of the Lie algebra,

\[
 g_j^{-2}s(e^{i g_j\xi})
       =\tfrac12\kappa(\xi,\xi)+O(g_j^2\|\xi\|^4),
 \qquad
 \log j(g_j\xi)=O(g_j^2\|\xi\|^2).
 \tag{MT.18}
\]

The norm of ξ is `O(ε_j/g_j)=O(P_j)`. On any fixed-factor enlarged Lie ball, the Hessian of the remainder is `O(g_j²P_j²)` and the force at zero vanishes. Constants depend on the compact group and the specified fixed norm, not on the number of samplers. Across `O(D)` samplers their total log-density remainder is `O(Dg_k²P^4)` when the couplings and cutoffs are comparable on the window.

The actual cutoff remains `||exp(i g_j ξ)−I||<ε_j`. For an operator norm it is a fixed symmetric spectral norm ball with the exact arcsine radius in the small tube. For a different stipulated source norm one must retain the nonlinear cutoff or prove its convex/sandwich replacement; (MT.18) alone does not make it a product box. A safe norm-independent statement is the sandwich supplied by

\[
 \|e^{i g_j\xi}-I-i g_j\xi\|
       \le Cg_j^2\|\xi\|^2.
 \tag{MT.19}
\]

Every occurrence of a gauge transformation in a Q/R or preparation test must use (MT.14). If several source samplers are nested, solve their center-fixed identities in their actual order; each is an exact normalized change. Polynomial derivative bounds for the whole resulting composition require the polynomial bounds for the intervening physical reconstruction maps. The elementary endpoint identity does not supply those missing maps automatically.

## 7. What has and has not been closed

The geometric logarithm problem is closed on the stated admitted finite region: the explicit boundary-preserving forest gauge yields a chart of radius `P·poly(D)` and explicit polynomial derivatives, with no dependence exponential in the number of RG steps. The actual soft axial samplers also have an exact field-independent normalized representation (MT.16), with their original small cutoff and positive quadratic cost. These are constructive input lemmas for a common-refinement proof.

The remaining analytic problem is narrower than the original global gauge concern, but substantive. One must express the **same complete restored measure** in these coordinates (or a source-compatible bounded variant), identify its joint positive quadratic and reference shift, bound the full nonlinear/constraint/Haar/E/B/R correction, and prove an enclosure and Taylor sandwich for each original quiet test. The composition with the original variational maps must be included. The current statement does not assert that either separate self-operation ledger is the density of this common measure.

In particular, a first R-only history can have a regular physical representative and still contain gauge-dependent rare tests. They remain exactly in (MT.12) or (MT.17). Similarly, a test involving `(1,V_h)` is covariant under a proposed inner gauge only if every artificially filled identity bond is preserved by that gauge. Merely fixing some vertices is insufficient; the literal incident-bond footprint must be checked, or the test must simply be kept as its full pullback.

When the common density and selectors have been verified, CE.1 requires only `osc W=o(H_R)`, and CE.2 offers the alternative complete Hessian/force bound. Neither follows just from the existence of the chart proved here.

## Source and construction record

- CMP109 (1987), printed pp.252–254, (0.5)–(0.12): contour average, endpoint covariance and its actual Euclidean invariant axial definition.
- CMP119 (1988), printed p.247, (1.5)–(1.7): the normalized soft axial sampler and its gauge action; printed pp.255–257, (2.2), (2.6)–(2.15): determining data, coupling comparison and joined domains.
- LFR I (1989), printed p.182, (1.25) and the paragraph following it: the gauge factors inside ζ and the exact center-fixed annular Faddeev–Popov step.
- [graded bundle reference](graded_bundle_reference.md), GR.1–GR.13: the one graded connection, exact graph transports and scale-weighted curvature bound.
- [M04 Two List Common Refinement](M04_Two_List_Common_Refinement.md), CR.1–CR.5: the two-history intersection geometry, native rank count and complete list of variables that must be restored.
- [common reference exchange](common_reference_exchange.md), CE.1–CE.3 and CE.19–CE.22: the precise later density and selector bounds to which this chart may be applied after they are proved.
