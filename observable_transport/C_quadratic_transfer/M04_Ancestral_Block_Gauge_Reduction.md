# Reducing an ancestral gauge comparison to a block-constant gauge

This note gives a constructive refinement of AP's real ancestral comparison. After putting both birth readouts in their actual averaged-block gauge, the transporting gauge splits exactly into a block-constant gauge and a small center-fixed residual. The residual, its birth-native finite differences and its derivatives in one ancestor relative-target array have the variational age factor. Exact covariance then gives a canonical birth-precision comparison using only the block-constant large gauge.

The local residual maps have explicit finite birth-stencil support. A single common raw-carrier family for all ancestor transports and saved real Q cores is not inferred. In particular the target-array derivative below keeps the coarser reference fixed; it is not the derivative of an entire terminally varying chronological chain.

## 1. Conventions and the actual real pair

Use the source convention

\[
 V^u(x,x')=u(x)V(x,x')u(x')^{-1},\qquad
 (V^u)^v=V^{vu}.
 \tag{BG.1}
\]

Fix a birth b and a later comparison index `j>=b+1`. Let `h_i=L^i eta`. Consider the admitted real critical fields

\[
 F_-=U_j(V_j),\qquad F_+=U_{j+1}(V_{j+1}),
 \qquad V_j=e^{iB}M^jF_+,
 \quad \|B\|_\infty\le C\epsilon_j.
 \tag{BG.2}
\]

The exact nesting/criticality argument of VN/AP identifies both as actual birth backgrounds. Proposition 9 supplies a relative Landau gauge u and potential A such that

\[
 F_-^u=e^{i\eta A}F_+,
 \qquad \|A\|_{\mathcal R_b(F_+)}
       \le C\epsilon_jL^{-(j-b)}.
 \tag{BG.3}
\]

All free birth coordinates have their fixed birth normalization. The complete source precision includes the constraint-force term and the full nonlinear averaged sampler, as in AP. No later coupling is substituted for the birth coupling.

Write `V_-=M^bF_-`, `V_+=M^bF_+`. Let

\[
 w_x(V)=V(y,x),\qquad x\in B_b(y),
 \tag{BG.4}
\]

be the source's full nonlinear average of all its prescribed intrablock contour transports. Its endpoint covariance is

\[
 w_x(V^g)=g(y)w_x(V)g(x)^{-1}.
 \tag{BG.5}
\]

This is the entire nonlinear mean of CMP109 (0.11), not a chosen path or an average of separate relative derivatives.

Define the birth canonicalizers

\[
 r_\pm(x)=w_x(V_\pm),\qquad r_\pm(y)=I,
 \qquad \bar V_\pm=V_\pm^{r_\pm}.
 \tag{BG.6}
\]

Equation (BG.5) gives `w_x(bar V_\pm)=I` exactly. These real gauges may be large; their unitarity, rather than smallness, is used below. Their microscopic lifts are used only through exact gauge covariance.

## 2. Exact factorization and its order

Let `u_b` be the restriction of u to birth vertices. Endpoint covariance of the literal iterated average gives

\[
 V_-^{u_b}=M^b(e^{i\eta A}F_+).
 \tag{BG.7}
\]

Set

\[
 w=r_+u_b r_-^{-1},\qquad
 X=\bar V_-^w=
       \left[M^b(e^{i\eta A}F_+)\right]^{r_+}
       =e^{ia}\bar V_+.
 \tag{BG.8}
\]

The last equation defines the small relative birth-link angle a on positive bonds. The relative-readout estimate in AP.1, including its uniform averaging bootstrap, gives

\[
 \|a\|_\infty\le C\epsilon_jL^{-(j-b)}=:\delta_{bj}.
 \tag{BG.9}
\]

The real conjugation by `r_+` does not change this bound.

Apply (BG.5) to the canonical field `bar V_-`:

\[
 C_x:=w_x(X)=w(y)w(x)^{-1}.
 \tag{BG.10}
\]

Define

\[
 s(x)=C_x^{-1},\qquad
 v(x)=w(y)\quad(x\in B_b(y)).
 \tag{BG.11}
\]

Then

\[
 s(y)=I,\qquad v\hbox{ is block constant},\qquad
 \boxed{\quad w=s v.\quad}
 \tag{BG.12}
\]

The product order is material: (BG.10) says `s(x)=w(x)w(y)^{-1}`, hence `s(x)v(x)=w(x)`. Moreover `r_\pm(y)=I`, so `v(y)=u_b(y)`. The large remaining gauge is exactly the block-constant lift of the AP transport on the next birth centers.

It follows that

\[
 \bar V_-^v=X^{s^{-1}}=e^{i\tilde a}\bar V_+,
 \tag{BG.13}
\]

where, for `e=(x,x')`,

\[
 \tilde a_e={1\over i}\Log\!\left[
       s(x)^{-1}e^{ia_e}
            \bar V_{+,e}s(x')\bar V_{+,e}^{-1}\right].
 \tag{BG.14}
\]

Both `bar V_-^v` and `bar V_+` are in the actual averaged-block gauge: a block-constant gauge preserves `w_x=I`, and (BG.10)--(BG.13) restores it exactly on the other side. No linearized sampler has replaced the nonlinear one.

## 3. Residual regularity, finite support and derivatives

### Lemma BG.1 — a supported local normal form

On a fixed sufficiently small physical-angle neighborhood of `a=0`, with the reference restricted to a canonical family satisfying `w_x(bar V_+)=I`, the maps

\[
 s_x=\{w_x(e^{ia}\bar V_+)\}^{-1},\qquad
 \tilde a_e\hbox{ given by (BG.14)}
 \tag{BG.15}
\]

are analytic in their displayed native inputs. They have fixed-L birth stencils and vanish relative to their identity values at `a=0`. Uniformly on the admitted real backgrounds,

\[
 \|s-I\|_\infty+\|\tilde a\|_\infty
       \le C_L\|a\|_\infty\le C_L\delta_{bj}.
 \tag{BG.16}
\]

For any fixed number q of birth-lattice covariant finite differences,

\[
 \max_{0\le q\le3}
 h_b^q\left(
    \|\nabla_{\bar V_+}^{q}(s-I)\|_\infty
       +\|\nabla_{\bar V_+}^{q}\tilde a\|_\infty\right)
       \le C_L\delta_{bj}.
 \tag{BG.17}
\]

The difference stencils are enlarged by only a fixed number of birth bonds. These are native birth differences, not microscopic differences across the discontinuities of a piecewise gauge lift.

**Proof.** Every contour in (BG.4) is inside one fixed L-block. The nonlinear group mean is analytic on the source's small-diameter contour tube. At `a=0` its value is identity because `bar V_+` is canonical. Products, inverse and the small logarithm in (BG.14) are therefore analytic on a fixed smaller tube, with bounded first derivatives. This proves (BG.16), its zero-subtraction and its finite support. The stencil of s is one full sampler block; that of `tilde a_e` contains the two endpoint sampler blocks and e.

Each covariant birth difference is a fixed finite sum of unitary translates of its input, divided by `h_b`. Repeating it q times gives at most a fixed number of such terms. Thus (BG.16) gives (BG.17), with constants independent of the ratio `eta/h_b` and the age. No estimate of a long microscopic path is used. The same local analytic bounds give the corresponding coefficient/parameter derivatives within a canonical reference family. ∎

For clarity, zero-subtraction in the reference input is not automatic on an unconstrained product polydisc: the first formula in (BG.15) equals identity at `a=0` only when the reference is canonical. If an unconstrained local reference continuation is needed, use instead the explicitly relative extension

\[
 s_x^{\rm rel}(a,V)
   =\bigl[w_x(e^{ia}V)w_x(V)^{-1}\bigr]^{-1},
 \qquad
 \tilde a_e^{\rm rel}
   ={1\over i}\Log\!\left[
       s_x^{\rm rel\,-1}e^{ia_e}
       V_e s_{x'}^{\rm rel}V_e^{-1}\right].
 \tag{BG.17a}
\]

This extension agrees with (BG.15) on the canonical family, has the same finite stencils, and has `s^rel(0,V)=I`, `tilde a^rel(0,V)=0` throughout a fixed smaller local tube. Consequently its reference derivative is bounded by `C_L|a|`. Its off-canonical values are only a chosen analytic extension; the exact gauge restoration and precision identities in Sections 2 and 4 are asserted on the actual canonical real family. No unconstrained all-depth reference registry is supplied by (BG.17a).

In particular (BG.15) is an actually supported local analytic postprocessing map. If a full raw-carrier series for a and the reference inputs is supplied, this map adds only the stated birth stencils. This sentence does not supply the missing simultaneous ancestor raw registry.

### Lemma BG.2 — the fixed-base ancestor target derivative

Hold `F_+` and hence `bar V_+` fixed. Vary the actual j-level relative-target array B in the source Proposition 9 neighborhood. On a fixed smaller array tube and for a whole array direction H,

\[
 \|D_B a[H]\|_\infty
       +\|D_B s[H]\|_\infty
       +\|D_B\tilde a[H]\|_\infty
       \le C_L L^{-(j-b)}\|H\|_\infty.
 \tag{BG.18}
\]

The native finite differences in (BG.17) satisfy the same derivative estimate. If a terminal-j direction has the actual physical normalization `H=g_j H^{\rm norm}`, the right side is `C_L g_j L^{-(j-b)}||H^norm||_infty`.

**Proof.** In the source (190), integration over the j-data row measure cancels the `h_j^{-d}` kernel factor. The relative potential derivative has the bounds `C||H||/h_j`, `C||H||/h_j^2` and `C||H||/h_j^3`. Its birth readout has the extra factor `h_b`, giving `h_b/h_j=L^{-(j-b)}`. The actual nonlinear averaging from microscopic spacing to h_b has the uniform bootstrap used in AP.1: after factoring the angle scale, the error factors have summable powers of the intermediate-to-j scale ratios. It does not contribute a constant to the power b.

The source analytic neighborhood may be taken about this fixed real regular base with a fixed sufficiently small physical array radius; the real input B in (BG.2) lies in its interior. The same derivative bounds hold on a smaller complex tube by the analytic equations (172)--(180) and (190). Apply the local chain rule to (BG.15), then the fixed finite differences of Lemma BG.1. The reference is held fixed throughout. ∎

At a specified birth output site or bond, the output matrix dimension is fixed. Whole-array sign duality, as in SG, consequently yields

\[
 \sum_d\|D_d s(x)\|
       +\sum_d\|D_d\tilde a(e)\|
       \le C_Lg_jL^{-(j-b)}
 \tag{BG.19}
\]

for the normalized j-array directions. This is a summed-direction bound for a fixed output. It is not a sum over all birth sites and does not discard the rank of an old marginal.

For a varying coarser base the local map has instead the explicit chain-rule structure

\[
 \|\dot s\|+\|\dot{\tilde a}\|
 \le C_L\bigl(\|\dot a\|
              +\|a\|\,\|\dot{\bar V}_+\|_{\rm local}\bigr).
 \tag{BG.20}
\]

The second term uses zero-subtraction at `a=0` along a canonical reference family, or the explicitly relative extension (BG.17a) if a local unconstrained continuation is chosen. It is not a derivative estimate for the unmodified first formula in (BG.15) on arbitrary reference inputs. Bounds for both terms on one common base continuation are necessary for a terminal-N current of an entire chronological chain. No such bound is inferred here merely from (BG.9).

## 4. Canonical precision comparison without a microscopic lift estimate

Let `bar K_-`, `bar K_+` be the actual canonical birth precisions at the two fields in (BG.6), with the complete force and sampler terms. AP's comparison, conjugated by the real gauge `r_+`, gives

\[
 K_w:=T_b(w)\bar K_-T_b(w)^*,\qquad
 \|K_w-\bar K_+\|_\rho\le C\delta_{bj}.
 \tag{BG.21}
\]

Because `w=s v`, exact gauge covariance of the complete relative coefficient and exact exceptional embedding gives

\[
 K_w=T_b(s)K_vT_b(s)^*,\qquad
 K_v=T_b(v)\bar K_-T_b(v)^*.
 \tag{BG.22}
\]

Here `K_v` is an actual canonical coefficient, since v is block constant. `K_w` need only be the relative coefficient at its noncanonical representative. The latter is exactly the object in AP.7--AP.11; it is not the absolute soft Hessian at a noncanonical field.

The pointwise adjoint map of s satisfies

\[
 \|T_b(s)-I\|_{\infty\to\infty}\le C_L\delta_{bj}.
 \tag{BG.23}
\]

Multiplying a weighted matrix row or column by a pointwise bounded map preserves the same weighted norm. Using (BG.21)--(BG.23), the uniform upper bound for `bar K_+`, and real unitarity therefore proves

\[
 \boxed{\quad
 \|T_b(v)\bar K_-T_b(v)^*-\bar K_+\|_\rho
       \le C_L\epsilon_jL^{-(j-b)} .
 \quad}
 \tag{BG.24}
\]

The intertwining of the free embedding follows by differentiating endpoint covariance of the exact next-average equation and using uniqueness of the same exceptional solve. Thus the transformed independent coordinate list is precisely the source list, not a chosen new transverse slice.

No claim about microscopic `R_b` regularity of a piecewise lift of s is needed or made. AP already controls the physical microscopic correction A. The residual s is handled by exact covariance and its small pointwise action on the actual birth coordinates. Its native spatial and target derivatives are the bounds in Section 3.

For a real homogeneous ancestor chain, all the resulting v_j are block constant on the **same birth partition**. Their products remain block constant and orthogonal. Transport all canonical birth matrices to one such frame and telescope (BG.24). The actual source coupling inequality gives

\[
 \sum_{j>b}\epsilon_j L^{-(j-b)}\le C_L\epsilon_b.
 \tag{BG.25}
\]

Hence AP's age-uniform real precision comparison can be achieved with block-constant large transports, with the small center-fixed residual paid by (BG.24). This is stronger information about the allowed gauge class than a generic pointwise orthogonal alignment.

## 5. What block-constant covariance does for the actual real cutoff

The large transport class in (BG.12) is the precise coarse-gauge class singled out in CMP119 p.250 after (1.17). That paragraph distinguishes general gauge covariance of the smooth action from the more restrictive covariance of the Q characteristic functions. For a new coarse gauge v(y), its lift is constant on each current block; the source Q reference transforms by that same lift, and the independent fluctuation transforms by its adjoint.

The identity can also be checked directly. Under this simultaneous real transformation, every factor in a literal Q test becomes

\[
 e^{ig_b z_e}H_{b,*,e}H_{b,\square,e}^{-1}
 \ \longmapsto\
 v(e_-)\,[e^{ig_b z_e}H_{b,*,e}H_{b,\square,e}^{-1}]\,v(e_-)^{-1}.
 \tag{BG.26}
\]

The operator-norm inequality, every overlapping test, and the fixed full-Lie-fiber P ball are unchanged for real v. The reference transformation uses its complete determining data and the source's exact block lift; it is not deduced from a Gaussian symmetry. Endpoint covariance preserves the target constraint, the averaged soft term is conjugated inside each block, and Haar/coarea factors transform by the same actual change of variables. The normalizer therefore transforms with the numerator. This is exact covariance of the real homogeneous birth conditional.

Equation (BG.26) does not assert that two different physical target fields have the same Q domain, nor that a complex nonunitary v preserves a literal operator-norm indicator. It does not allow a general AP gauge to be inserted into the Q test. The reduction to block-constant v is what permits the real covariance identity.

Nor may a cancellation of the total gauge response erase separately recorded microscopic and kernel origins. Their own pre-pullback derivatives and normalization terms still have to be retained, as DP/NC require. The real full-kernel covariance is an exact identity available to that future common registry, not an estimate for all its separate origin currents.

## 6. The remaining common-complex-core step

The constructive result here is the actual factorization (BG.12), the local supported analytic residual map (BG.15), its fixed-base ancestor derivatives, and the canonical precision estimate (BG.24). The flat example AF is the limiting case `s=I`, `tilde a=0`, with all change contained in the block-constant v.

At a single pair the residual construction is holomorphic on its explicit finite native stencils. Proposition 9 provides the source relative input map. This does not yet produce one raw-carrier representation for v_j, the reference canonicalizers, all independently decoupled old coefficients, and every saved real core at arbitrarily many levels. Component restriction and full core/target compatibility are identities that must be verified for such a common construction.

An all-depth use must also distinguish the fixed-base derivative (BG.18) from the terminal derivative of a chain in which both comparison bases and gauges move. Equation (BG.20) displays the missing terms. The numerical real matrix estimate alone does not give the supported zero-subtracted derivative of that moving family, its Jacobian, or the separate physical-origin boundary responses.

The possible stronger comparison of actual global/local Q-center errors, with an additional `e^{-cR_{b+1}}`, is deliberately not claimed here. It would require the uniform local-reference gauges and the same complete component family. Neither the present local residual normal form nor CC's geometric contraction supplies that additional identification.

Primary inputs: exact covariance of the nonlinear average in CMP98/CMP109; CMP102 (172)--(181), Proposition 9 and (190); CMP109 (0.11), (2.5), (2.16); CMP119 p.250 after (1.17); AP.1 and AP.7--AP.22; SG's whole-array duality.
