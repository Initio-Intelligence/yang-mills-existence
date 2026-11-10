# A support-preserving non-Abelian completion of the full local Hessian

This note constructs an explicit linear projector from an invariant local analytic coefficient to a globally defined gauge-invariant function with the same quadratic Taylor coefficient. It uses only loops made from the coefficient's own input edges. It neither fills those loops with new input plaquettes nor assigns an enclosing box as their support. Its nonlinear complement has a small native weak-curvature value and composite first-current norm for the actual fixed-depth smooth source, using the bounded-source envelopes in PJ and the scalar equivariantization in EC.

There are three distinct qualifications. The finite-torus estimate has a separate winding term. The current estimate is for the derivative of the completed scalar function, not a separate estimate of every microscopic and kernel origin. The actual application concerns the smooth three-layer comparison family. It does not establish the specified M04 claim or an induction through arbitrary sharp-Q histories.

## 1. Supported input and conventions

Work with SU(N), N at least 2. Positive oriented bonds are the independent variables; negative orientations mean inverse matrices. Write physical link coordinates as

\[
 U_e=\exp(iB_e),\qquad B_e=B_e^*,\quad \operatorname{Tr}B_e=0.
 \tag{GC.1}
\]

The complexification permits complex traceless B. PJ uses an anti-Hermitian convention; multiplication by i identifies the two physical charts without changing a bound. A normalized field is B=ga, where g is the retained-scale coupling. Fix a real orthonormal basis of traceless Hermitian matrices for the trace inner product. All constants can depend on N and on the fixed block and localization choices.

Let f_X be a scalar coefficient with actual finite raw edge-input graph G_X. No graph edges outside this determining input list are needed below. G_X may be disconnected; a forest will handle that case. Set m_X=1+|E(G_X)|. The complete connected carrier X also records the source anchor, normalization connectors, and any needed determining stencils. The native size n(X) satisfies

\[
 m_X\le C n(X),\qquad
 \operatorname{diam}G_X\le C n(X),\qquad n(X)\ge1.
 \tag{GC.2}
\]

The input f_X is invariant under all real gauge transformations at the endpoints of its input edges. It is holomorphic on a fixed physical polydisc about the identity. EC.1 supplies such termwise invariance for a complete scalar coefficient family, provided its already proved real-orbit tube is used in the Haar projection. Projection of arbitrary overlapping uncontracted factors is not allowed.

For the quantitative result, let M_X be deterministic nonnegative envelopes. On a physical polydisc of radius 2r_0 about the flat field, assume

\[
 |f_X(e^{iB})|\le g^{-2}M_X.
 \tag{GC.3}
\]

At every admitted native real center V, assume the same envelope bounds the coefficient on a relative physical polydisc of a fixed radius r_0:

\[
 |f_X(e^{iB}V)|\le C g^{-2}M_X,
 \qquad \|B\|_\infty<r_0.
 \tag{GC.4}
\]

These are coefficientwise hypotheses, stronger than a bound on the total normalized expectation. All complete raw input slots are varied in these charts. The bounds are uniform on real gauge orbits. Constants can be absorbed into M_X. Suppose, for some positive rate nu,

\[
 \sup_n\sum_{X\ni n} e^{\nu n(X)}M_{n,X}\le A.
 \tag{GC.5}
\]

An unanchored coefficient family is treated with the corresponding fixed-point incidence norm. When more than one envelope is available, their sum gives a common envelope at the smaller rate.

For the actual smooth three-layer mark, PJ.1 and PJ.1b give (GC.3)--(GC.5), after the support-preserving operation EC.1, with

\[
 g=g_3,\qquad
 A\le C_L B_3,\qquad
 B_3=L^{12}|\alpha|(g_3/g_0)^2.
 \tag{GC.6}
\]

The identity insertion is removed exactly as in PJ.2 before applying the construction. It is restored separately. The three original conditional normalizers, source normalization, force correction, Haar/coarea terms and inherited action remain in the coefficients furnishing these envelopes.

## 2. The exact completion

Choose a spanning tree in each connected component of G_X and one root in each tree. These choices are fixed combinatorial data, independent of U and g. For each nontree edge e, take the based fundamental loop gamma_e: the tree path from its root to e_-, then e, then the reverse tree path from e_+ to the root. Its length is at most 2|E(G_X)|+1. Its holonomy is denoted Omega_e(U).

Tree gauge makes the original coefficient a function of these holonomies. More precisely, put the tree edges equal to I and the nontree edges equal to W_e, and define

\[
 \varphi_X((W_e)_{e\notin T})
      =f_X(U_{T}=I,U_e=W_e\ (e\notin T)).
 \tag{GC.7}
\]

For real U, a gauge at vertex x equal to the ordered product along its root-to-x tree path sends every tree edge to I and every nontree edge to Omega_e(U). Hence, wherever both expressions belong to the admitted family,

\[
 f_X(U)=\varphi_X((\Omega_e(U))_{e\notin T}).
 \tag{GC.8}
\]

The remaining gauge at a tree root conjugates all its based holonomies simultaneously. Distinct connected components have independent remaining conjugations. Since the adjoint representation of su(N) has no invariant vector,

\[
 D\varphi_X(0)=0.
 \tag{GC.9}
\]

Here and below derivatives of varphi are in W_e=exp(iC_e) at C=0. Uniqueness of an invariant bilinear form on the complexified simple Lie algebra gives

\[
 D^2\varphi_X(0)[C,C]
      =\sum_{e,f\notin T}h_{ef}\operatorname{Tr}(C_e C_f),
 \qquad h_{ef}=h_{fe}.
 \tag{GC.10}
\]

Mixed coefficients between different connected components vanish, by their independent conjugations. This also covers a forest without any nontree edges: its invariant scalar coefficient is constant near the flat field.

Introduce the globally defined matrix function

\[
 \Xi(W)=\frac{W-W^{-1}}{2i}
       -\frac{\operatorname{Tr}(W-W^{-1})}{2iN}I.
 \tag{GC.11}
\]

It is holomorphic on SL(N,C), equivariant under conjugation, real Hermitian and traceless on SU(N), and uniformly bounded there. For traceless Hermitian C,

\[
 \Xi(e^{iC})=C+O(\|C\|^3).
 \tag{GC.12}
\]

Define the completion and the nonlinear complement by

\[
 (\mathcal C_X f_X)(U)
   =\frac12\sum_{e,f\notin T}h_{ef}
       \operatorname{Tr}\!\left[
         \Xi(\Omega_e(U))\Xi(\Omega_f(U))\right],
 \tag{GC.13}
\]

\[
 \mathcal N_X(U)=f_X(U)-f_X(I)-(\mathcal C_X f_X)(U).
 \tag{GC.14}
\]

### Theorem GC.1 -- exact support-preserving quadratic projector

The map f_X to C_X f_X is linear and depends only on the Hessian of f_X at the identity. Its output is a globally defined real gauge-invariant function of the original edge inputs. If f_X is real on real fields, its completion is real there. It has zero constant and linear Taylor coefficients and exactly the same Hessian as f_X. In particular,

\[
 D^j\mathcal N_X(I)=0\quad (j=0,1,2),\qquad
 \mathcal C_X^2=\mathcal C_X.
 \tag{GC.15}
\]

No logarithm or branch choice is used in the globally defined output (GC.13). No filled surface, bounding box, or additional raw edge becomes part of its support.

**Proof.** Each based holonomy in a connected component transforms by conjugation at that component's root. Its trace pairing in (GC.13) is invariant. Cross-component pairings are zero. Every loop uses only original input edges, which proves the support assertion. Unitarity proves boundedness and reality on real fields; inverses are holomorphic on SL(N,C).

For a raw tangent B, write the first-order expansion of a fundamental holonomy as

\[
 \Omega_e(e^{itB})=I+it\,L_e(B)+O(t^2),
 \tag{GC.16}
\]

where L_e is the oriented tree-cycle sum of the raw angles. Equations (GC.8)--(GC.10) show that the quadratic coefficient of f_X along this tangent is one half of the sum h_ef Tr(L_e(B)L_f(B)). Equations (GC.11)--(GC.13) give exactly the same coefficient for C_X f_X. Polarization proves equality of the full Hessians, not only of their diagonal evaluations. Both linear coefficients vanish by (GC.9).

If the tree edges are set to I, the based fundamental holonomies in (GC.13) are exactly the nontree variables. Thus applying (GC.10) to the completion recovers exactly h_ef. Its second application in (GC.13) is unchanged. This proves idempotence. All operations are linear in the original Hessian. \(\square\)

The operator is a completion of the whole quadratic kernel. It is not the scalar Wilson projector of WQ or NW. Those projectors first select the marginal quadratic part. The same construction can be applied to an already transverse remainder kernel, using its supported invariant coefficient representation. A fixed finite lattice-symmetry average can be imposed on a correspondingly closed carrier, with the explicit finite carrier/rate cost recorded in NW; it is not a free preservation of every spatial rate.

### Lemma GC.2 -- bounded completion and local derivatives

For fixed q, on real raw-link fields the completion satisfies

\[
 |\mathcal C_X f_X|\le C g^{-2}m_X^2M_X,
 \qquad
 \|D_B^q(\mathcal C_X f_X)\|_{\infty,\ldots,\infty}
      \le C_q g^{-2}m_X^{q+2}M_X.
 \tag{GC.17}
\]

The derivative formula is valid at real points in physical angle charts of fixed bounded size around any real field. A sum over raw first-coordinate derivatives adds at most one further factor C m_X. Multiplication by g converts such a derivative to its normalized raw-link derivative.

For any strict rate kappa below nu, there is a smaller fixed positive physical radius r_1 for which the completed family has a holomorphic carrier norm at most C A/g^2 on that radius, at rate kappa.

**Proof.** The restriction (GC.7) lies in the same raw physical polydisc as (GC.3). Cauchy estimates give |h_ef| at most C r_0^{-2}M_X/g^2; the fixed colour dimension is absorbed in C. There are at most m_X^2 pairs. A based loop has at most C m_X factors, all unitary at a real field. Differentiating its product q times in physical angle directions costs at most C_q m_X^q times the product of their sup norms. Derivatives of the matrix exponential at Hermitian arguments are bounded by its unitary integral formula. The inverse loop satisfies the same estimates. Product differentiation of the two Xi factors proves (GC.17).

On a complex physical chart of radius r_1 about a real field, a loop product or its inverse has norm at most exp(C m_X r_1). The same coefficient bound therefore gives at most C g^{-2}m_X^2 M_X exp(C m_X r_1) for the completion. Choose r_1 so that the last exponent fits a fixed part of nu-kappa; the remaining margin pays m_X^2. This gives the holomorphic family bound. No claim that complex long-loop norms are uniformly unitary was used. \(\square\)

## 3. A real estimating gauge without changing support

Assume the native real field obeys

\[
 \|I-U(p)\|\le\varepsilon=C_0 gP
 \quad\hbox{for every plaquette in the required native region},
 \qquad P\ge1.
 \tag{GC.18}
\]

On the infinite lattice, place a carrier in a coordinate box of side at most C n(X). For a torus, first restrict this construction to carriers with a coordinate box that lifts injectively to the lattice. Fix a box root and coordinate-ordered paths from it to every vertex. Use their parallel transports as the estimating gauge.

### Lemma GC.3 -- short-carrier small links

In this gauge the edges read by f_X satisfy

\[
 \|I-U_e^{\rm est}\|\le C n(X)^2\varepsilon.
 \tag{GC.19}
\]

Whenever the right side is sufficiently small, the Hermitian logarithms of these edges satisfy

\[
 \|B^{\rm est}\|_\infty\le C n(X)^2 gP.
 \tag{GC.20}
\]

**Proof.** Compare the coordinate-ordered path to the far endpoint of an edge with the coordinate-ordered path to its near endpoint followed by the edge. Adjacent interchanges of coordinate steps, and cancellations of inverse steps, reduce the resulting loop to at most C n(X)^2 elementary plaquettes. This is an exact non-Abelian product identity, with conjugated plaquette holonomies. All conjugations are unitary at a real field. For unitary A_j, the telescoping inequality |I-product A_j| at most sum |I-A_j| proves (GC.19). The ordinary local logarithm estimate near I proves (GC.20). \(\square\)

This gauge may read links elsewhere in the estimating box. Equality of the original gauge-invariant function with its value in this gauge is pointwise. By EC.2 and GC.1, those extra reads do not become arguments of f_X or of its completion. The box is used only to prove a bound on their values. Differentiation below holds the chosen real gauge fixed at the base field; it never differentiates this estimating rule.

## 4. The native cubic remainder

The following explicit small-coupling condition is sufficient:

\[
 0<g<g_*,\qquad P\ge1,\qquad gP^2\le1.
 \tag{GC.21}
\]

To conclude that the value bound tends to zero also require gP^3 to tend to zero. The actual logarithmic radii satisfy both conditions. The weaker condition gP to zero alone would not justify the logarithmic carrier split used here.

For a normalized raw coordinate derivative write

\[
 D_{e,a}^{(g)}F(U)
  =\left.\frac d{dt}F(\ldots,e^{itgT_a}U_e,\ldots)\right|_{t=0}.
 \tag{GC.22}
\]

### Theorem GC.4 -- infinite-lattice or injectively localized estimate

Fix 0<kappa<nu. Under (GC.2)--(GC.5) and (GC.18)--(GC.21), for sufficiently small g,

\[
 \sup_n\sum_{X\ni n}e^{\kappa n(X)}
       \sup_{U\ {\rm native}}|\mathcal N_{n,X}(U)|
       \le C A gP^3,
 \tag{GC.23}
\]

\[
 \sup_n\sum_{X\ni n}e^{\kappa n(X)}
       \sup_{U\ {\rm native}}
          \sum_{e,a}|D_{e,a}^{(g)}\mathcal N_{n,X}(U)|
       \le C A gP^2.
 \tag{GC.24}
\]

These formulas hold on the infinite lattice, or for an explicitly restricted family all of whose small carriers have the injective boxes in Lemma GC.3. The finite-torus statement without that restriction is GC.5 below. Fixed spatial moments may be inserted after reserving another strict rate margin. A coefficientwise common deterministic envelope gives the same bound for admitted normalized coordinate path increments of length at most one, with P replaced by P+C.

**Proof.** Set delta=nu-kappa. Choose D so large that delta D/4 exceeds 4, and split the carrier family at

\[
 n_*(g)=D\log(1/g).
 \tag{GC.25}
\]

By (GC.21), gP is at most sqrt(g). Therefore n_*^2 gP tends to zero. Every carrier with n(X) at most n_* admits the fixed flat chart after applying Lemma GC.3, for sufficiently small g. Its gauged logarithm B has norm at most C n(X)^2 gP.

By GC.15 the remainder in these raw logarithm coordinates has zero jets through order two at 0. On the real segment from 0 to B, the third derivative of f_X is bounded by C M_X/g^2 in the multilinear sup-direction norm, by polarized Cauchy estimates on the fixed physical polydisc in (GC.3). This directional estimate does not sum coordinate indices; polarization uses only a fixed number of scalar complex directions and has no factor depending on the number of edges. The third derivative of its completion is bounded by C m_X^5 M_X/g^2, by (GC.17). Taylor's integral formula, (GC.2), and (GC.20) imply

\[
 |\mathcal N_X(U)|
       \le C (1+n(X))^{12}M_X gP^3.
 \tag{GC.26}
\]

The power 12 is a harmless common upper bound; it is not claimed optimal.

For a raw derivative at U, hold the estimating real gauge fixed. The normalized left link variation then becomes a normalized left variation conjugated by a fixed unitary matrix. On the small logarithm chart its angle velocity has norm at most Cg. Differentiating the Taylor remainder, and using its zero first and second jets, bounds one derivative by C g^{-2}M_X times a polynomial in n(X) times |B|^2 g. Summing all raw edge/colour directions adds at most C m_X. Thus

\[
 \sum_{e,a}|D_{e,a}^{(g)}\mathcal N_X(U)|
       \le C (1+n(X))^{12}M_X gP^2.
 \tag{GC.27}
\]

A fixed gauge at the start of a coordinate path works throughout that path: its additional physical link angle is at most Cg. Alternatively the same uniform coefficientwise envelopes can be integrated along the path. No derivative of a field-dependent gauge is hidden in (GC.27).

For n(X)>n_*, no small-link gauge is required. Equations (GC.3)--(GC.4) and (GC.17) give

\[
 |\mathcal N_X(U)|\le C(1+n(X))^2M_X g^{-2},
 \tag{GC.28}
\]

\[
 \sum_{e,a}|D_{e,a}^{(g)}\mathcal N_X(U)|
       \le C(1+n(X))^4M_X g^{-1}.
 \tag{GC.29}
\]

In (GC.29), the coefficient f_X uses Cauchy on the native-center physical tube (GC.4), rather than an unjustified flat chart. The derivatives of f_X(I) are zero. Spare exponential rate pays all displayed polynomials. The remaining tail factor is at most exp(-delta n_*/2), up to adjustment of a fixed constant. The choice of D makes its product with g^-2 at most Cg and its product with g^-1 at most Cg. Since P is at least 1, these are bounded by the right sides of (GC.23)--(GC.24). Summation of (GC.26)--(GC.27) uses the same spare rate and (GC.5). This proves both bounds. \(\square\)

The supremum of the sum in (GC.24) is obtained here from a common deterministic coefficientwise envelope. It is not an interchange of different coordinate-path suprema. Dividing a coefficientwise bound by a native energy regulator at least one can only decrease it. This observation does not supply any missing support or origin-composition property of the specified M03 interface.

### Theorem GC.5 -- explicit finite-torus winding term

Let ell be the shortest compatible torus period in retained lattice units. Suppose a carrier of size less than c_0 ell has an injective estimating box, as follows from (GC.2) after fixing c_0 sufficiently small. For the complete finite-torus family,

\[
 \|\mathcal N\|_{\kappa,0}
      \le C A\left(gP^3+g^{-2}e^{-c\ell}\right),
 \tag{GC.30}
\]

\[
 \|D^{(g)}\mathcal N\|_{\kappa,1}
      \le C A\left(gP^2+g^{-1}e^{-c\ell}\right).
 \tag{GC.31}
\]

The notation denotes exactly the value and summed-first-derivative norms in (GC.23)--(GC.24). The constants are independent of ell and g within the stated fixed-depth family. The exponential terms include all carriers for which an injective small box is unavailable; they need not be assigned a topologically winding loop individually.

**Proof.** Apply the preceding small-carrier argument only when both n(X) is at most n_*(g) and n(X)<c_0 ell. The tail n(X)>n_* is treated as before. The additional tail n(X) at least c_0 ell is estimated using (GC.28)--(GC.29) and its retained exponential carrier weight. This gives (GC.30)--(GC.31). \(\square\)

If ell is at least a sufficiently large constant times log(1/g), these extra terms fit the respective small remainders. Without such a relation they must stay in the theorem. A flat real field on a short torus can have nontrivial winding holonomy even when every plaquette is I; weak curvature alone does not make all its links small in a periodic gauge. GC.30 therefore does not assert a volume-uniform cubic bound without a winding remainder. This agrees with the distinction already made in SW and FH.

## 5. Actual smooth-source consequence and remaining interfaces

Apply EC.1 to the complete supported coefficient family of the actual local smooth mark Phi_n in PJ. The same full determining carriers and common component restrictions are retained. PJ.1 gives the flat physical tube, PJ.1b gives the native-center bounded-source envelope needed in the long-carrier estimate, and EC.3 retains the normalized coupling powers and common derivative envelopes. Thus GC.1--GC.5 apply to that actual family, with (GC.6).

The resulting identity is coefficientwise and exact:

\[
 \Phi_{n,X}(U)
   =\Phi_{n,X}(I)+(\mathcal C_X\Phi_{n,X})(U)
      +\mathcal N_{n,X}(U).
 \tag{GC.32}
\]

Every term is fully gauge invariant. The completion has the exact raw Hessian, including the full nonlinear loop completion selected by (GC.13). On nonwinding native fields the nonlinear complement has actual bounds

\[
 \|\mathcal N\|_{\kappa,0}\le C_L B_3g_3P^3,
 \qquad
 \|D^{(g_3)}\mathcal N\|_{\kappa,1}\le C_L B_3g_3P^2,
 \tag{GC.33}
\]

with the terms in GC.30--GC.31 on a general finite torus. The chosen P must bound the actual retained native plaquette radius and satisfy GC.21; the source logarithmic choices do so for sufficiently weak coupling. The microscopic identity source is transported exactly and is not part of this nonlinear estimate.

This is stronger than a raw Taylor subtraction on a global small-link slice: both pieces in GC.32 are genuine gauge-invariant functions on their real domains, and the estimate uses local estimating gauges for the original supported coefficients. The statement remains limited in the following concrete ways.

1. A coefficient estimate on the admitted native weak-curvature class is not, by itself, a compact-extension theorem for every raw field in a specified global interface.
2. Completion of a quadratic kernel does not prove that its nonlinear conditional transfer has the Gaussian contraction in FH. The full interacting comparison must be supplied separately, with its exact inherited precision and normalized density.
3. A bound on the derivative of GC.32 does not split that derivative into microscopic insertion and each fixed-test kernel origin. Existing physical current labels and their moving-reference velocities remain part of the induction state.
4. No hard-Q indicator has been analytically continued or differentiated beyond its established real first-current representation. The real boundary/core problem persists.
5. All constants inherited from PJ and EC concern the specified finite three-layer smooth family. No depth-uniform native orbit tube, old-core registry, or repeated contraction constant is inferred here.

These qualifications prevent using a valid finite-depth non-Abelian completion as an unproved claim of M04 closure or Yang--Mills existence.

## 6. Dependencies and checks

The algebraic theorem GC.1 and geometric estimate GC.3 are proved in this note. The analytic and large-carrier estimates explicitly use both kinds of coefficient envelope in GC.3--GC.4. Their model-specific discharge is PJ.1/PJ.1b, not a probabilistic bound on an extensive whole-volume expectation. EC supplies support-preserving scalar invariance, uniform real-orbit control, and the first-jet change-of-basis estimate. WQ and NW identify the marginal Wilson part separately. FH concerns the actual inherited classical Gaussian lift, with its stated scope.

Primary source facts used by PJ/EC are CMP109 (1.7)--(1.19), (2.6)--(2.18), CMP116 (1.13)--(1.21), Lemma 2 and (2.5)--(2.26), and the final gauge-orbit paragraph on CMP116 printed pp.21--22. The full force/gap and raw pullback estimates are those of BA, BR/FC and TC. None of these citations is a claim that the original papers state GC.13 or the present nonlinear-complement estimate; those constructions and deductions are given above.
