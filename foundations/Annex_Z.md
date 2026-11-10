# Current-coordinate contours, nonlinear marginal factors and order-uniform scale budgets

**Annex Z.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 0. Results and hypotheses

The contour criteria below apply to regular and heterogeneous histories when the requisite joint domains and carrier bounds hold. Annexes AD–AH treat the regular and boundary contributions separately.

The new work has three concrete uses.

1. It gives an anisotropic contour-to-Hessian test that retains the radius of each differentiated coordinate and each carrier. This avoids imposing the minimum radius of an unrelated distant part of the history on every term.
2. It proves a marginal derivative theorem using complex tubes centered along a **real** radial segment. A complex disc centered at the identity need not reach the real background. The theorem retains the nonlinear second-coordinate-map contribution, and extends to every derivative order with a fixed factorial bound.
3. It proves an all-order old-age summation theorem and a sharp limitation of a different proposed majorant. Exponential decay in old age can pay order-dependent polynomial age losses within one factorial power. Suppression of the form `exp[-c(log(2+age))^r]`, by itself, cannot do so for every source order with one fixed factorial power.

The last distinction is especially relevant to the full Schwinger hierarchy. Summability at every fixed order is weaker than the fixed growth condition required in J2.

All new mathematical results below are direct finite-dimensional proofs or elementary series estimates. Their actual-model premises are listed explicitly in Section 7.

### 1. Source conditions: what is available and what the proposed derivative must preserve

The hypotheses below use CMP119, pp. 244, 255, 259–263, 267–270, 276–277 and 283.

- The inherited regular action is already renormalized. CMP119 (2.25) contains its old vacuum and coupling subtractions; differentiating it must retain their field dependence.
- Each primitive E carrier has a complex extension with its stated decay norm, on the regular primitive space with radii `alpha_{0,j}=g_j C_0(log g_j^{-2})^{q_0}` and `alpha_{1,j}=g_j C_1(log g_j^{-2})^{q_1}`. The source introduces fixed integers `q_0,q_1>1`; this note does not infer an additional inequality between them and the real cutoff exponent.
- **Source scope:** CMP119 (2.34)-(2.39) defines the multiscale boundary domain, including independently extended currents, reconstructed fields and currents, a real-reference representative, local gauge bounds, and a complex relative field. It is not the definition of every primitive E domain. The appropriate domain at each actual preparation stage must be preserved by its contour; Annex AD makes this distinction explicit.
- CMP119 p.276 transfers the small-field localization construction to the complete geometry. Its boundary extension is (3.43). On p.277 the source explains the consumption of the dyadic analytic reserve and the extra fluctuation factor. These statements must be used together with their radii and preparation losses.
- CMP119 Theorem 2, p.263, is a regular-configuration estimate. Its proof obtains a four-power marginal factor for R and an irrelevant gain after coupling subtraction for E. An inequality proved on the real regular configurations is not, merely by analytic continuation, a modulus estimate on a proposed complex contour.

The source uses an independent current precisely because an individual localized field no longer satisfies the full unlocalized Landau-gauge identity. CMP109 (3.10)-(3.17), pp.272-273, makes this distinction. Its insertion norm controls the field, its first derivative, the appropriate projection and covariant Laplacian. The unlocalized minimizing-field derivative in CMP102 Proposition 9 and (190), pp.308-309, also controls the covariant second-order outputs. These are useful map inputs; they do not identify every localized independent-current pullback with the physical current of that localized field.

The exact conditional density is the one derived in Annex W. The results below do not discard its R terms, B terms, heterogeneous coefficient, coordinate factors, retained mean, or selected support. The support theorem of this argument is a separate result.

### 2. An anisotropic contour-to-Hessian certificate

Let `I` be the finite free-coordinate index set at a cutoff, with a metric `d(i,j)`. A coordinate can mean one real component of a Lie-algebra block; alternatively one may work with block operator norms throughout. Let `Y` run over a finite family of localized carriers, and let `I_Y` be the coordinates on which its pulled-back activity `W_Y` depends.

For each real configuration `z` in the actual support, suppose a product contour centered at `z` is admitted for the relevant coordinates, with radii

\[
 r_{Y,i}(z)>0,\qquad i\in I_Y,
 \tag{EC.1}
\]

and with

\[
 |W_Y(z+\zeta)|\le M_Y(z)
 \quad\hbox{on that contour}.
 \tag{EC.2}
\]

For a Hessian bound it is enough to have the corresponding one- and two-coordinate product contours with the same bounds. A collection of pair contours alone does not prove the arbitrary-order estimate stated below.

Let `omega_i>0` be the weights of the intended physical quadratic norm, and put

\[
 \mathcal E_\gamma
 =2\sup_z\sup_i
 \sum_{Y:i\in I_Y}
 \frac{M_Y(z)}{\omega_i r_{Y,i}(z)}
 \sum_{j\in I_Y}
 \frac{e^{\gamma d(i,j)}}{\omega_j r_{Y,j}(z)}.
 \tag{EC.3}
\]

#### Proposition EC.1 -- local radii give the exact weighted budget

Under (EC.1)-(EC.2),

\[
 \sup_z\sup_i\sum_j
 \frac{e^{\gamma d(i,j)}}{\omega_i\omega_j}
 \left|\partial_i\partial_j\sum_Y W_Y(z)\right|
 \le\mathcal E_\gamma.
 \tag{EC.4}
\]

For any multi-index `alpha` supported in a verified full product contour,

\[
 |\partial^\alpha W_Y(z)|
 \le \alpha! M_Y(z)
       \prod_{i\in I_Y}r_{Y,i}(z)^{-\alpha_i}.
 \tag{EC.5}
\]

**Proof.** Cauchy's formula gives `M_Y/(r_{Y,i}r_{Y,j})` for distinct coordinate indices and `2M_Y/r_{Y,i}^2` for a repeated index. Derivatives outside `I_Y` vanish. Sum those estimates, take absolute values before summation, and use the common factor two to get (EC.4). Applying the multi-variable Cauchy formula gives (EC.5). The proof does not differentiate the integration-domain indicator. \(\square\)

The same proposition applies to joint current and retained-background variables: include both types in `I` and use their actual radii and coordinate weights. It is invalid to hold a background constant in a derivative for which that background is an output of the differentiated map.

The activity in (EC.2) must already be the complete pullback used by the construction. If instead `W_Y=f_Y circ Psi_Y`, the nonlinear map derivatives remain to be estimated; Proposition EC.3 below gives one way to do so.

#### Corollary EC.2 -- heterogeneous matrix coercivity and inverse bounds

Let `D_omega=diag(omega_i)`. Assume each `W_Y` is real-valued on the real support, so the perturbation Hessian is real symmetric. Suppose, on that support,

\[
 V(z)=\tfrac12\langle z,H_0z\rangle-\sum_YW_Y(z),
 \qquad H_0\ge\lambda D_\omega^2,
 \quad\mathcal E_0<\lambda.
 \tag{EC.6}
\]

Then

\[
 \nabla^2V(z)\ge(\lambda-\mathcal E_0)D_\omega^2.
 \tag{EC.7}
\]

Define the weighted matrix norm

\[
 \|A\|_\gamma=\sup_i\sum_j e^{\gamma d(i,j)}|A_{ij}|.
 \tag{EC.8}
\]

If `C_0=H_0^{-1}` and

\[
 \|D_\omega C_0D_\omega\|_\gamma\le K_\gamma,
 \qquad K_\gamma\mathcal E_\gamma<1,
 \tag{EC.9}
\]

then the inverse of the actual Hessian obeys

\[
 \left\|D_\omega(\nabla^2V(z))^{-1}D_\omega\right\|_\gamma
 \le\frac{K_\gamma}{1-K_\gamma\mathcal E_\gamma}.
 \tag{EC.10}
\]

**Proof.** The balanced perturbation `P=D_omega^{-1}(sum_Y Hess W_Y)D_omega^{-1}` is real symmetric and has row-sum norm at most `mathcal E_0`. The symmetric Schur estimate bounds its Euclidean operator norm by the same number, proving (EC.7). The triangle inequality for `d` makes (EC.8) submultiplicative. Apply its convergent Neumann series to

\[
 [D_\omega^{-1}H_0D_\omega^{-1}-P]^{-1}
 =\sum_{n\ge0}[(D_\omega C_0D_\omega)P]^n
       D_\omega C_0D_\omega.
\]

This proves (EC.10). \(\square\)

Equation (EC.10) is a matrix inverse estimate, not by itself a covariance theorem on a selected integration domain. The latter also uses the support and integration-by-parts theorem and the relevant field domains.

These formulas expose a concrete sufficient target for C-06. They do not infer (EC.3) from primitive activity norms. In particular, the physically relevant radius is the dimensionless product `omega_i r_{Y,i}`, and it can vary with layer, carrier and retained data.

### 3. Recentered tubes along real backgrounds preserve marginal derivatives

A previous sufficient radial estimate required a complex disc centered at the identity whose radius reached the background. That condition can be stronger than necessary. The following theorem uses a chain of complex neighborhoods centered along a real segment instead.

Let `E` be a finite-dimensional complex normed space, let `b` belong to its real form, and suppose `f` is holomorphic and bounded by `M` on

\[
 \mathcal T(b,\rho)
 =\bigcup_{0\le t\le1}\{tb+w:\|w\|<\rho\},
 \qquad 0<\rho\le1.
 \tag{EC.11}
\]

The norm can be the joint norm of link logarithms and independent-current variables. Its precise definition must be fixed in an application.

#### Lemma EC.3 -- the first derivative at a real background

If `Df(0)=0`, then

\[
 \|D^r f(tb)\|
 \le r!e^r M\rho^{-r}\quad(r\ge1),
 \tag{EC.12}
\]

\[
 \|Df(b)\|\le4M\rho^{-2}\|b\|,
 \qquad
 |f(b)-f(0)|\le2M\rho^{-2}\|b\|^2.
 \tag{EC.13}
\]

The right side of the value bound can also be replaced by its minimum with `2M`.

**Proof.** For unit directions `v_1,...,v_r`, apply Cauchy's formula to `f(tb+sum_l t_l v_l)` on the polydisc of radius `rho/r` in each scalar parameter. This gives `r^r M rho^{-r}`, and `r^r<=e^r r!`. For the Hessian one can use two radii `rho/2`, giving the sharper bound `4M rho^{-2}`. Now integrate

\[
 Df(b)-Df(0)=\int_0^1 D^2f(tb)[b,\cdot]\,dt
\]

and then integrate once more for the value difference, using `Df(0)=0`. \(\square\)

The condition `Df(0)=0` is an exact consequence of semisimple global gauge invariance for the original activity expressed jointly in its Lie-algebra and current variables. Indeed, write a linear functional at the origin as a sum over its variables. Invariance under simultaneous adjoint action, tested with all other variables zero, makes each summand annihilate every commutator. Since the complexified Lie algebra of `SU(N)` equals its commutator algebra, every summand is zero.

This conclusion must not be applied to an arbitrary already-centered function with a nontrivial frozen background: its origin need not be the gauge-fixed flat configuration. The flat origin in this lemma belongs to the **original activity variables**, before the nonlinear current-coordinate pullback.

#### Proposition EC.4 -- all-order composite marginal bound

Let `Psi` be a holomorphic map from the current coordinates to `E`, with `Psi(z_0)=b`. Let `0<theta<=1`, `Q>=0`, `K>=1`, and `g>0`. Suppose

\[
 \|b\|\le Q\theta,
 \qquad
 \|D^s\Psi(z_0)\|
 \le s!K^s g^s\theta\quad(s\ge1).
 \tag{EC.14}
\]

Suppose the tube (EC.11) is admitted for `f`, with the same `rho` along its whole real segment, and `Df(0)=0`. For every integer `m>=2`,

\[
 \boxed{
 \|D^m(f\circ\Psi)(z_0)\|
 \le M(1+4Q)m!
       \left[\frac{(1+e)Kg}{\rho}\right]^m\theta^2.
 }
 \tag{EC.15}
\]

For the first derivative,

\[
 \|D(f\circ\Psi)(z_0)\|
 \le4MQK g\rho^{-2}\theta^2.
 \tag{EC.16}
\]

The bounds use the derivatives of the actual map `Psi`; no linearization of it is substituted for the exact pullback.

**Proof.** Faà di Bruno's partition formula gives

\[
 D^m(f\circ\Psi)[v_1,\ldots,v_m]
 =\sum_{\pi\in\Pi_m}
 D^{|\pi|}f(b)
       [D^{|B|}\Psi[v_i:i\in B]:B\in\pi].
 \tag{EC.17}
\]

The one-block term is bounded, by (EC.13)-(EC.14), by

\[
 4MQ\,m!(Kg)^m\rho^{-2}\theta^2.
 \tag{EC.18}
\]

For `r>=2` blocks, (EC.12) bounds the sum by

\[
 M m!(Kg)^m e^r\binom{m-1}{r-1}
       (\theta/\rho)^r.
 \tag{EC.19}
\]

To obtain its combinatorial coefficient, order the `r` blocks. For prescribed positive sizes summing to `m`, the number of ordered labeled partitions is `m!/(d_1!...d_r!)`. Multiplication by the native derivative factors `prod d_i!`, division by `r!`, and multiplication by the `r!` in (EC.12) leave `m!` times the number of ordered compositions, namely `binom(m-1,r-1)`.

Because `theta<=1`, `rho<=1`, and `2<=r<=m`,

\[
 (\theta/\rho)^r\le\theta^2\rho^{-m}.
\]

The sum of \(e^r\binom{m-1}{r-1}\) is at most \((1+e)^m\). The one-block term also has \(\rho^{-2}\le\rho^{-m}\). Combining these estimates gives (EC.15). Equation (EC.16) follows from the ordinary chain rule and (EC.13). \(\square\)

#### 3.1 Why the nonlinear term matters

At second order the identity is

\[
 D^2(f\circ\Psi)
 =D^2f(\Psi)[D\Psi,D\Psi]+Df(\Psi)D^2\Psi.
 \tag{EC.20}
\]

The second term in (EC.20) is generally nonzero. Lemma EC.3 gives its extra small factor from the background `b`, so both terms retain `theta^2`. A bound on `D^2 f` alone would not have justified this conclusion.

In the intended four-dimensional application, `theta=L^{-2a}` for an old age `a=k-j`. Then `theta^2=L^{-4a}` compensates the four-dimensional old-cell count. The coordinate map includes the local gauge, the constrained minimizing field and the correct independent-current extension. Establishing (EC.11) and (EC.14) for **every** such map is still an actual-source obligation.

There is no need for `||b||<rho` in this theorem. The real background may be larger than the imaginary width of its analytic tube. What is required is a uniformly admitted tube along the real segment, and that is a quantitative condition stronger than knowing the endpoint lies in an open analytic domain.

#### 3.2 A native analytic map can supply all its derivative orders at once

Suppose, in its own native variables, `Psi` is holomorphic on the norm ball of radius `R/g` about `z_0`, with

\[
 \sup_{\|\zeta\|<R/g}\|\Psi(z_0+\zeta)\|
 \le B\theta.
 \tag{EC.21}
\]

The same mixed Cauchy argument gives

\[
 \|D^s\Psi(z_0)\|
 \le s!\left[\frac{e\max(1,B)}{R}\right]^s
        g^s\theta.
 \tag{EC.22}
\]

Thus (EC.14) follows without separately estimating every derivative. The large native ball in (EC.21) is used only to estimate derivatives of `Psi`; the activity `f` is not assumed to be admissible on its entire image. The chain rule uses the separate tube (EC.11). Confusing these two domains would recreate the missing contour step.

### 4. Carrier polynomial losses have a fixed factorial price

#### Lemma EC.5 -- exponential carrier entropy absorbs polynomial derivative losses

Let `b,c>=0` and `delta>0` be fixed. There is a constant `C`, independent of `m`, such that

\[
 \sum_{n\ge1}n^{bm+c}e^{-\delta n}
 \le C^{m+1}(m!)^b,
 \qquad m\ge1.
 \tag{EC.23}
\]

**Proof.** Put `t=bm+c`. Split `exp(-delta n)` into two equal factors. The first factor times `n^t` is at most `(2t/(e delta))^t` for `t>0`; the other factor is summable. For fixed `b,c`, this upper bound is at most `C^{m+1}m^{bm}m^c`. The polynomial `m^c` is absorbed by another fixed exponential, and `m^{bm}<=(e^m m!)^b`. The case `t=0` is immediate. \(\square\)

Suppose the number of carriers of size `n` containing a prescribed current block is at most `mu^n`, their activity decay is `exp(-kappa n)`, and the geometric weight costs at most `exp(gamma D_0 n)`. If

\[
 \delta=\kappa-\log\mu-\gamma D_0>0,
 \tag{EC.24}
\]

then (EC.23) pays any fixed polynomial carrier factor raised to source order `m`. The factorial exponent increases by the degree of that polynomial. This is compatible with J2 when that degree is fixed; it is not compatible if the degree itself grows uncontrollably during the induction.

The actual source's carrier geometry and decay reserve must be checked before identifying its parameters with (EC.24). A unit-lattice animal count cannot silently replace the current-block carrier count.

### 5. An all-order near/far old-age summation theorem

The fixed-order near/far calculation of Annex H can be strengthened to permit polynomial age losses whose exponent grows linearly with the derivative order.

#### Theorem EC.6 -- one fixed factorial budget for all derivative orders

Fix `A>=1`, `p>=0`, `q>0`, `lambda>0`, and `b,sigma,D,tau>=0`. Suppose nonnegative numbers `H_{a,m}(ell)` satisfy, for integers `a>=0`, `m>=2`, and `ell>=e`,

\[
 H_{a,m}(\ell)
 \le A^{m+1}(m!)^p(1+a)^{b+\sigma m}
 \min\{\ell^{-qm},e^{-\lambda a}\ell^{D+\tau m}\}.
 \tag{EC.25}
\]

For every `0<q'<q`, there is a constant `C`, depending only on the displayed fixed parameters and on `q'`, such that

\[
 \boxed{
 \sum_{a\ge0}H_{a,m}(\ell)
 \le C^{m+1}(m!)^{p+\sigma}\ell^{-q'm}.
 }
 \tag{EC.26}
\]

In particular the order-two sum tends to zero as `ell` tends to infinity, while all orders share the same factorial exponent `p+sigma`.

**Proof.** Write `beta_m=b+sigma m` and choose

\[
 n=\left\lceil
 \frac{D+(\tau+q)m}{\lambda}\log\ell
 +\frac{2\beta_m}{\lambda}+1
 \right\rceil.
 \tag{EC.27}
\]

This choice has both

\[
 \ell^{D+\tau m}e^{-\lambda n}\le\ell^{-qm},
 \qquad
 \frac{\beta_m}{1+n}\le\lambda/2,
 \tag{EC.28}
\]

and `n+1<=C_0(m+1)(1+log ell)`.

For `a<=n`, use the first branch of (EC.25) and sum at most `n+1` terms. For `a=n+t>n`,

\[
 \frac{(1+n+t)^{\beta_m}}{(1+n)^{\beta_m}}
 \le\exp\!\left(\frac{\beta_m t}{1+n}\right)
 \le e^{\lambda t/2}.
\]

Use the second branch, (EC.28), and the remaining geometric series. The two portions are therefore bounded by

\[
 C_1 A^{m+1}(m!)^p\ell^{-qm}
      [C_0(m+1)(1+\log\ell)]^{b+\sigma m+1}.
 \tag{EC.29}
\]

The factor `(m+1)^{sigma m+b+1}` is at most `C_2^{m+1}(m!)^sigma`. Since `m>=2`,

\[
 (1+\log\ell)^{b+\sigma m+1}\ell^{-(q-q')m}
 \le
 \left[(1+\log\ell)^{\sigma+(b+1)/2}
             \ell^{-(q-q')}\right]^m.
\]

The quantity in square brackets has a finite supremum for `ell>=e`. Combining the bounds proves (EC.26). \(\square\)

The term `2 beta_m/lambda` in (EC.27) matters. Without it, a tail estimate with a constant depending on `beta_m` could hide a new order-dependent growth loss.

#### 5.1 How the source coupling comparison enters

For an admitted source coupling array, CMP119 (2.6)-(2.7) gives a polynomial comparison between `g_k` and `g_j` and a fixed comparison of the logarithms. If an old analytic radius has a **proved** lower bound

\[
 \rho_{j,k}\ge c\,g_j\ell_j^q(1+k-j)^{-s_0},
 \qquad \ell_j=\log g_j^{-2},
 \tag{EC.30}
\]

then, with `a=k-j`,

\[
 g_k/\rho_{j,k}
 \le C(1+a)^{s_0+1/2}\ell_k^{-q}.
 \tag{EC.31}
\]

The case `a=0` is included by `1+a`. This is arithmetic using an admitted coupling comparison; it is not a derivation of the actual trajectory.

Combining (EC.15), a native polynomial age loss, (EC.31), the old-cell count and a carrier sum of the form (EC.23) yields the first branch of (EC.25), **provided the displayed radius and native-map estimates have actually been established**. An independently proved irrelevant branch on the same objects then invokes Theorem EC.6.

Thus a finite polynomial loss in age per derivative is not automatically fatal. Its factorial price is explicit. What cannot be done is to assume (EC.30), or to use the marginal and irrelevant branches on different unverified contours.

### 6. A sharp failure of a weaker all-order majorant

The previous theorem uses decay exponential in the old age `a`. A large-field small factor expressed in the logarithm of that age can be much weaker for purposes of uniform source-order growth.

#### Proposition EC.7 -- logarithmic age suppression alone is not a factorial budget

Fix `c>0`, `sigma>0`, and `r>1`, and define

\[
 S_m=\sum_{a=0}^\infty
 (1+a)^{\sigma m}
 \exp[-c(\log(2+a))^r],\qquad m\ge1.
 \tag{EC.32}
\]

Every `S_m` is finite. Nevertheless there are positive constants `c_1,c_2` and `m_0`, depending only on the fixed parameters, such that

\[
 c_1m^{r/(r-1)}\le\log S_m
       \le c_2(m+1)^{r/(r-1)},\qquad m\ge m_0.
 \tag{EC.33}
\]

Consequently there are no fixed constants `B,P<infinity` for which

\[
 S_m\le B^{m+1}(m!)^P
 \quad\hbox{for every }m.
 \tag{EC.34}
\]

**Proof.** For the upper bound, divide the integers `a` into exponential bins `e^n<=a<e^{n+1}`. Each bin contains at most `e^{n+1}` integers. Up to a factor exponential in `m`, its contribution is bounded by

\[
 \exp[(\sigma m+1)n-cn^r].
\]

Young's elementary maximization inequality gives

\[
 bn-cn^r
 \le C_{c,r}b^{r/(r-1)}-(c/2)n^r,
 \qquad b\ge0.
\]

The remaining sum over `n` is finite. This proves finiteness and the upper bound in (EC.33).

For the lower bound, let

\[
 t_m=\left(\frac{\sigma m}{cr}\right)^{1/(r-1)}
\]

and take an integer `a_m` within one of `exp(t_m)`. For large `m`,

\[
 \log(1+a_m)\ge t_m-1,
 \qquad \log(2+a_m)\le t_m+1.
\]

A single summand then has logarithm at least

\[
 \sigma m(t_m-1)-c(t_m+1)^r
 =\frac{r-1}{r}\sigma m t_m-O(m)-O(1).
\]

The positive leading term has order `m^{r/(r-1)}`, proving the lower bound. Finally `log(m!)<=m log m`, while `m^{r/(r-1)}/(m log m)` tends to infinity. This excludes (EC.34). \(\square\)

#### 6.1 What this diagnosis says about the Yang-Mills route

Under a reciprocal-linear ultraviolet coupling comparison, an old-scale small factor `exp[-c(log g_j^{-2})^r]` can behave like `exp[-c'(log(2+a))^r]` as a function of the number of older shells. If a proposed absolute majorant simultaneously pays an age factor `(1+a)^{sigma m}` at derivative order `m`, the model sum (EC.32) shows that fixed-order convergence of that majorant is not enough for a fixed OS factorial exponent.

This does **not** prove that actual Yang-Mills correlations have this growth. It proves that this particular class of upper-bound arguments is too weak without another input. Extra exponential spatial/age decay, a better derivative map estimate, resummation before absolute values, or another norm can avoid the example. A bound by a large majorant is not a lower bound on the quantity being estimated.

The argument also does not contradict the completed logarithmic-running budget F-02. There the variable is the absolute ultraviolet logarithm and there is a genuine positive power of the lattice spacing. A factor `exp(-delta t)` pays powers `t^{gamma m}` at a factorial cost. In (EC.32), after setting `t=log(2+a)`, the dangerous derivative factor is `exp(sigma m t)`, and the available damping is `exp(-c t^r)`. These are different optimization problems.

For E, the explicit irrelevant branch in Theorem EC.6 is a way to avoid this loss. For R, a fixed polynomial small-coupling bound, or even the stronger displayed logarithmic large-field factor, cannot alone be declared sufficient at every order without checking the age dependence of the derivative and carrier costs.

### 7. Analytic conditions and the exact remaining certificates

#### C-02 — hypotheses for simultaneous E contours (Annex AD)

Proposition EC.1 identifies the quantitative output required of a contour theorem, and Proposition EC.4 shows how one can use recentered real-segment tubes instead of an unnecessarily large identity-centered disc.

The following actual estimates are still missing:

1. For every active real current configuration, every contributing E carrier and every localization/preparation parameter, an admitted joint tube for all the original variables entering that carrier.
2. Verification of every reconstructed-field and independently extended-current condition, not just the physical plaquette inequality.
3. Quantitative lower bounds on the coordinate radii after composition with the actual constrained, local-gauge and preparation maps, uniform enough to feed (EC.3) and (EC.30).
4. A complex activity majorant on those same tubes, with all carrier and preparation prefactors retained.

A point lying in the source's open analytic set has some positive radius at that finite cutoff. That observation does not prove any of these uniform statements. No missing map estimate is replaced by a choice of names for its radius.

#### C-04 — hypotheses for the regular E/R derivative-carrier sum (Annex AH)

The new composite theorem proves the marginal four-power mechanism, including the nonlinear map contribution, **if** its tube and map estimates are available. The all-order summation theorem gives a fixed factorial budget for an explicit pair of majorants. The logarithmic-age example shows why order-by-order summability is insufficient.

To finish the application one must prove those majorants for the actual E and R pullbacks and sum them with the actual radii, coupling sequence, carrier geometry and preparation losses. In particular the small weighted-Hessian number in (EC.3) has not been obtained for the complete potential. The primitive source norms are not substituted for that sum.

#### C-06 -- heterogeneous retained backgrounds: OPEN

Corollary EC.2 supplies an exact weighted matrix formulation suited to different physical coordinate weights. It prevents a homogeneous estimate from being extended simply by renaming the metric.

The actual source geometry must still supply the weighted principal lower bound and covariance norm in that same coordinate system, together with the complete E/R/B perturbation budget and quantitative domain margins. The unlocalized background theorem is a relevant source input, but it does not by itself verify every localized current and nonlinear preparation output. The complete boundary estimates remain in C-05.

No claim is made that the C-07 support result or an arbitrary-vector moment comparison fills these missing analytic certificates.

### 8. References

Primary references

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, Communications in Mathematical Physics **119** (1988), 243-285. The relevant equations are listed in Section 1.
- T. Balaban, *Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*, Communications in Mathematical Physics **102** (1985), 277-309, Proposition 9 and (190), pp.308-309.

Additional reference:

- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. I*, Communications in Mathematical Physics **109** (1987), 249-301, especially (3.10)-(3.17), pp.272-273. [DOI](https://doi.org/10.1007/BF01215223).


---
