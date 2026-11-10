# Pointwise majorants before integration

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

These are proved analytic lemmas. Their actual mixed-history input remains a separate source estimate; this note does not close C05.

## 1. The required form of the target

The current estimate in AB17.4, and its C04 comparator DS.10, is a weighted Hessian row bounded uniformly at every point of the admitted chart. They do not require the stronger quantity obtained by putting an independent supremum over the chart inside every endpoint summand. Imposing that stronger quantity is sufficient but unnecessary; it is not used here.

The required order is
\[
 \sup_{(z,\xi)\in D}\sup_i\sum_j
 e^{\gamma\rho(i,j)}\|D_iD_j B(z,\xi)\|_{\rm op}.
\tag{P1}
\]
Likewise DS.16 requires a uniform pointwise sum of local directional jets. This distinction permits a pointwise positive norm and Banach-valued Cauchy. It does not permit interchanging a supremum and a sum without proof.

## 2. Native directional Cauchy in a pointwise weighted l1 norm

Let a finite family of scalar holomorphic functions F_Gamma share a common joint chart. Let S_Gamma be their actual slot dependency supports, including stencils and kernel dependence. Fix nonnegative weights w_Gamma, independent of the analytic parameters. Suppose that for every local slot set S,
\[
 \sup_{\xi\in D_+}\sum_{\Gamma:S_\Gamma\cap S\ne\varnothing}
 w_\Gamma |F_\Gamma(\xi)|\le J N(S).
\tag{P2}
\]
Let h_1,...,h_m be common directions supported in S_1,...,S_m, respectively. Their norms divided by the available slot margins are q_1,...,q_m. Assume the triangle-inequality joint chart: for every xi in the inner domain D_-, the polydisc
\[
 \xi+\sum_{l=1}^m t_lh_l,\qquad |t_l|<(m q_l)^{-1},
\]
lies in D_+. A zero q_l makes the derivative zero.

**Theorem P1.** Under these hypotheses,
\[
 \sup_{\xi\in D_-}\sum_\Gamma w_\Gamma
 |D_{h_1}\cdots D_{h_m}F_\Gamma(\xi)|
 \le e^m m! J N(S_1)\prod_{l=1}^m q_l.
\tag{P3}
\]

**Proof.** The first derivative kills every function whose actual support misses S_1. Apply multivariate Cauchy to the remaining family along the same finite-parameter map. Triangle inequality and Tonelli put the sum inside the common contour integral. Its integrand is bounded by (P2). The product of inverse contour radii is m^m product q_l, and m^m<=e^m m!. No term is evaluated at a function-dependent point of the contour. The finite-family estimate passes to a normally convergent infinite family by Fatou and the same uniform majorant. QED.

Thus an estimate of sum_Gamma sup_D |F_Gamma| is unnecessary for the native target. A purely native first direction is covered, so long as (P2) includes the unsubtracted persistent scalar terms.

## 3. Current Hessian rows without an interchange of supremum and sum

Work first in scalar current coordinates on a finite metric lattice. Let G_Gamma(z,xi) be holomorphic on the common polydisc |z_j|<2P and exactly supported in I_Gamma as a function of z. Set d_Gamma=diam I_Gamma. Suppose
\[
 \sup_{z,\xi}\sup_i
 \sum_{\Gamma:i\in I_\Gamma}
 e^{\lambda d_\Gamma}|G_\Gamma(z,\xi)|\le J,
 \qquad \lambda>\gamma\ge0.
\tag{P4}
\]
Here the supremum is outside the positive sum.

**Theorem P2.** On the inner polydisc |z_j|<P,
\[
 \sup_{z,\xi}\sup_i\sum_j e^{\gamma\rho(i,j)}
 |\partial_i\partial_j\sum_\Gamma G_\Gamma(z,\xi)|
 \le \frac{4J e^\gamma}{P^2[1-e^{-(\lambda-\gamma)}]}.
\tag{P5}
\]
A fixed current block dimension contributes its usual finite coordinate factor.

**Proof.** For a fixed i, only terms containing i can survive differentiation. Group them by n<=d_Gamma<n+1 and write their scalar sum as F_{i,n}. The group depends only on current coordinates in the ball rho(i,j)<n+1, and (P4) gives
\[
 \sup |F_{i,n}|\le J e^{-\lambda n}.
\]
At the point under consideration choose phases u_j aligning the entries partial_i partial_j F_{i,n}, and let
\[
 v_j=e^{\gamma[\rho(i,j)-(n+1)]}u_j
\]
on that ball, with v_j=0 outside it. Then ||v||_infinity<=1. Two-variable Cauchy on z+t e_i+s v, with |t|,|s|<P/2, yields
\[
 \sum_j e^{\gamma\rho(i,j)}
 |\partial_i\partial_jF_{i,n}|
 \le 4P^{-2} e^{\gamma(n+1)}J e^{-\lambda n}.
\]
Sum over n and use the triangle inequality for the full Hessian. This proves (P5). QED.

The fixed reserve lambda-gamma pays a sum of shell suprema. It is not an exchange of the supremum with the original infinite family. Exact current support is a hypothesis. For quasilocal pullbacks one still needs a common-map shell localization or an independent endpoint argument; (P5) does not make native support into current support.

## 4. Positive lifting of a linear source resummation

At fixed geometry let the full linear contribution of incoming block eta to an output coefficient be v_{Y,eta}(xi,omega). The index eta may be the original pair (b,X), with all internal localization histories already summed. Introduce independent complex multipliers zeta_eta before the linear localization and regrouping. Then
\[
 V_Y(\boldsymbol\zeta;\xi,\omega)
 =\sum_\eta\zeta_\eta v_{Y,\eta}(\xi,\omega).
\tag{P6}
\]
For each fixed xi,omega,
\[
 \sup_{|\zeta_\eta|\le1}|V_Y(\boldsymbol\zeta;\xi,\omega)|
 =\sum_\eta|v_{Y,\eta}(\xi,\omega)|.
\tag{P7}
\]
The upper bound is the triangle inequality; the reverse bound chooses each multiplier to cancel the phase of its coefficient. No cardinality factor occurs.

If the scalar source bound is uniform for this marked input class, (P7) gives a final spatial bound for the same positive blocks |v_{Y,eta}| on which a pre-completion age bound can be retained by the triangle inequality. The two-majorant Holder step can then apply to these same blocks. This avoids resolving every internal localization label.

The map from incoming activities to the nonself coefficients through LFR II (1.59)-(1.68), including the fixed-history addback, is linear. Its determining maps are fixed by the source geometry and background construction, not by these auxiliary multipliers. The actual completed self kernel must subsequently be restored to its unmarked physical value; only the nonself blocks are marked in the Mayer analysis. At all marks equal to one the original density is recovered exactly.

The uniform marked source bound is established on the literal ordinary full-tree input class by the absolute estimates in that linear construction; see the companion marked-activity note for its source check. The mixed-history application must still prove its geometric input norm, including old bounded completed cores and their true dependency footprints. Marking cannot strengthen an available spatial norm or turn an ordinary unbounded large-field region into a free component.

## 5. Application boundary

The stronger sum-of-suprema target is not needed. The positive lifting repairs the signed-versus-positive inference on its actual phase-stable source class. The remaining work is source-specific: prove the mixed-history decorated or quotient input norm and a local positive native-root estimate for the full unsubtracted action. These analytic lemmas are designed to consume those estimates without imposing another stronger norm afterward.
