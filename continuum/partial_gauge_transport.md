# Gauge covariance of partial integrals and exterior scores

## Conclusion and source comparison

**Proved identity.** A change of variables in a stopped integral may transport the variables actually integrated. A simultaneous gauge transformation of the earlier fixed tuple instead relates two different conditional fibers. The resulting partial integral is covariant along that exterior orbit; it need not be constant at one fixed earlier tuple.

**Useful repair criterion.** The exterior response need not vanish. For the original C05 projective density argument, its part that varies with the still-integrated tuple must satisfy a bound, while a scalar common to the whole tuple can remain in the mass decomposition. This is weaker than requiring the entire exterior derivative to be small, but stronger than a completed-integral Ward identity.

This appendix does not embed the homogeneous MB.12 example into a literal C05 stopped history. The actual graded preparation and the same Wilson-subtracted source object still have to be identified. It therefore supplies an exact comparison and a sufficient criterion, not a counterexample to C05.

The objects being compared are:

- [Stopped densities and projective comparison](../boundary/stopped_densities.md), SD.1 and SD.5: the actual conditional density at fixed earlier raw tuple \(x\).
- SD.6d–SD.6e: the actual pullbacks \(\Phi_j\), their complete factors \(J_j\), and the final mass. Unrolling cancels only identical intermediate masses.
- [Wilson-subtracted primitive response and interpolation](../boundary/ward_response.md), ST.2–ST.3: the same rootwise bank
  \[
  \mathcal R_{b,z}^{H}(U)=E^{(b)}(\Lambda_b,U,z)
    -E^{(b)}(\Lambda_b,1,z)-\beta_b A(h_z\phi_b,U).
  \tag{PG.1}
  \]
  Its birth coefficient, cutoff, root and localization sum stay fixed.
- [Moving ancestor bases, fixed innovations, and exact latent-gauge current transport](../observable_transport/D_native_nonlinear/M04_Moving_Base_Response_and_Latent_Gauge_Current.md), MB.9–MB.11 and MB.18–MB.25: exact fixed-target covariance and normalized latent transport.

## 1. Exact finite partial-integral identity

Write \(a\) for all variables actually integrated at the stop and \(x\) for every earlier raw coordinate that is fixed. Include all smooth positive multipliers, Jacobians and archived masses in a full coordinate density \(\rho_t(x,a)\). Moving a native-independent multiplier out of SD.1's reference measure and back into \(\rho_t\) is only notation; it is not dropped.

Suppose an actual real gauge path has a fiber-preserving coordinate map
\[
G_t(x,a)=(E_t x,T_t(x,a)),
\qquad
J_t^x(x)=|\det DE_t(x)|,\quad
J_t^a(x,a)=|\det D_aT_t(x,a)|.
\tag{PG.2}
\]
Here the new exterior tuple \(E_t x\) is independent of \(a\). Require the complete source covariance identities
\[
\begin{split}
\rho_t(E_t x,T_t(x,a))J_t^x(x)J_t^a(x,a)&=\rho_0(x,a),\\
S_t(E_t x)&=T_t(x,S_0(x)),\\
f_t(E_t x,T_t(x,a))&=f_0(x,a).
\end{split}
\tag{PG.3}
\]
Every saved target, Q reference, selected factor and normalizer occurring in the source must participate. If covariance is established only after summing branches, PG.3 cannot be asserted separately on each fixed branch.

Define the actual partial mass and normalized expectation
\[
Z_t(x)=\int_{S_t(x)}\rho_t(x,a)\,da,\qquad
H_t(x)=Z_t(x)^{-1}\int_{S_t(x)}\rho_t(x,a)f_t(x,a)\,da.
\tag{PG.4}
\]
Then
\[
\boxed{
 Z_t(E_t x)J_t^x(x)=Z_0(x),\qquad
 H_t(E_t x)=H_0(x).
}
\tag{PG.5}
\]
For the conditional coordinate density \(p_t=\rho_t/Z_t\),
\[
p_t(T_t(x,a)\mid E_t x)J_t^a(x,a)=p_0(a\mid x).
\tag{PG.6}
\]

**Proof.** Substitute \(a'=T_t(x,a)\) in both integrals. The same factor \(J_t^x(x)^{-1}\) multiplies numerator and denominator, and cancels only in their ratio. This proves every identity without differentiating a sharp cutoff. \(\square\)

Real blockwise adjoint maps have determinant one. This removes the displayed Jacobian factors in that case, but does not remove \(E_t x\). At a prescribed fixed exterior point \(x\), PG.5 instead says
\[
H_t(x)=H_0(E_t^{-1}x).
\tag{PG.7}
\]
Thus transporting the integrated tuple is a legitimate integration change of variables; replacing \(x\) by \(E_t^{-1}x\) changes the conditional fiber being evaluated.

Let \(v_t=\dot E_t\circ E_t^{-1}\). At differentiability points,
\[
(\partial_t+v_t\cdot D_x)H_t=0,\qquad
\partial_t Z_t+\operatorname{div}_x(v_t Z_t)=0.
\tag{PG.8}
\]
The same formulas hold weakly when the finite transport identities are the available formulation. A scalar normalized density ratio relative to another source-covariant reference transforms like \(H_t\), because their common exterior Jacobian cancels.

## 2. What remains after the integrated gauge currents cancel

Let \(w_t(x,a)\) be the integrated-coordinate velocity induced by \(G_t\). On an active smooth stratum the complete density has
\[
\partial_t\rho_t+
\operatorname{div}_x(v_t\rho_t)+
\operatorname{div}_a(w_t\rho_t)=0.
\tag{PG.9}
\]
The corresponding equation for the conditional density, extended with its actual support, is
\[
\partial_t p_t+v_t\cdot D_xp_t+
\operatorname{div}_a(w_t p_t)=0.
\tag{PG.10}
\]
This is an equation for a density, not a pointwise assertion that its gauge derivative vanishes.

At fixed \(x\), the original normalized derivative contains insertion, score covariance, and boundary terms, exactly as in SD.15 and MB.19. Apply MB.22 only to the integrated tuple \(a\). Its insertion transport, density divergence and Q-boundary terms combine, leaving precisely
\[
\partial_t H_t(x)=-D_xH_t(x)[v_t(x)].
\tag{PG.11}
\]
This equality is the differentiated finite identity PG.7, so it retains the same numerator, final mass and normalizer. An integration by parts in \(a\) cannot eliminate its \(x\)-derivative.

There are genuine restricted cancellation cases. If the gauge belongs to the stabilizer of the entire fixed tuple, \(v_t(x)=0\), then PG.11 vanishes. It also vanishes for a particular insertion if the resulting \(H_t\) is independently proved constant along that exterior orbit. A general admitted nonzero earlier innovation need satisfy neither condition.

If the proposed gauge sends the exterior tuple to a value depending on \(a\), it does not preserve the conditioning fibers in PG.2. One then gets a continuity equation with exterior flux \(\int \rho_t w_t^x\,da\), rather than PG.8 with a deterministic exterior velocity. Its normalized insertion equation includes the corresponding conditional covariance flux. Such a transformation supplies no simpler argument for dropping the exterior response.

## 3. A criterion that really gives the original projective density bound

The preceding real covariance does not by itself imply SD.10's domination at the same fixed \((x,a)\). In particular, PG.6 compares a density with its pullback at a different exterior point and a different integrated coordinate.

Here is a direct sufficient criterion that preserves the original statement. On the fixed support \(S_x\), let \(W_t(x,a)\) be the same nonvanishing analytic interpolation of the complete SD.1 weight, with \(W_0>0\), and set
\[
q_t(x,a)=\partial_t\log W_t(x,a).
\]
Choose one actual-support anchor \(a_*(x)\). Suppose
\[
\int_0^1\sup_{a\in S_x}
 |q_t(x,a)-q_t(x,a_*)|\,dt\le\delta<\pi/2.
\tag{PG.12}
\]
This must hold uniformly on the required native complex family when used for C05's analytic bound. Then
\[
W_1(x,a)=W_0(x,a)e^{c(x)+\sigma(x,a)},\qquad
|\sigma(x,a)|\le\delta,
\tag{PG.13}
\]
where \(c(x)=\int_0^1q_t(x,a_*)\,dt\). Consequently the exact SD.1 conditional density obeys
\[
|p_1(a\mid x)|\le e^{2\delta}\sec\delta\,p_0(a\mid x).
\tag{PG.14}
\]
The mass retains \(c(x)\).

**Proof.** Integrate the difference of the two logarithmic derivatives. This gives PG.13 on the same fixed fiber, and SD.8–SD.10's sector argument gives PG.14. \(\square\)

For a genuine pure gauge path, on smooth positive strata the complete score from PG.9 is
\[
q_t=-D_x\log\rho_t[v_t]-D_a\log\rho_t[w_t]
     -\operatorname{div}_xv_t-\operatorname{div}_aw_t.
\tag{PG.15}
\]
The exterior divergence is independent of \(a\) and disappears from the anchored difference. For the literal adjoint action the diagonal divergences vanish. The two derivative terms still need their anchored estimates. In a completed owned integral the integrated-coordinate term may cancel by the full transport identity. In the pointwise density criterion PG.12, it is not zero and must not be deleted.

Thus one useful sufficient repair is to bound the exterior anchored score
\[
\sup_{a\in S_x}
\left|
D_x\log\rho_t(x,a)[v_t(x)]
-D_x\log\rho_t(x,a_*)[v_t(x)]
\right|,
\tag{PG.16}
\]
together with the actual integrated-coordinate and transverse contributions needed in PG.12. No bound is needed on the component of the exterior score common to every \(a\); it is exactly an allowed mass scalar. This is a sharper target than controlling the entire exterior derivative.

If an argument uses only complete coefficient integrals, it can instead use MB.22 before taking absolute values, retaining the exterior derivative PG.11 and all original labels. To recover C05's particular positive catalog estimate SD.14 that way, it must prove the resulting common domination or equivalent estimate with the same analytic supremum, weights and origin assignments. A cancellation between separately prescribed absolute labels is insufficient.

## 4. Applying the criterion to the same Wilson-subtracted bank

Set
\[
F_t(x,a)=\mathcal R_{b,z}^{H}(U_t(x,a))
\tag{PG.17}
\]
with exactly PG.1's bank. A simultaneous gauge change of all its native arguments leaves this scalar unchanged when the source covariance hypotheses hold. This licenses expressing both values in a common output gauge; it does not license omitting the motion of the earlier raw parameters used to describe those values.

For example, after pulling back the integrated tuple,
\[
\widehat F_t(x,a):=
F_t\!\left(x,T_t(E_t^{-1}x,a)\right)
 =F_0(E_t^{-1}x,a).
\tag{PG.18}
\]
Writing \(x_t=E_t^{-1}x\), the paired difference has exact derivative
\[
\frac d{dt}
\{\widehat F_t(x,a)-\widehat F_t(x,a_*)\}
=
\{D_xF_0(x_t,a)-D_xF_0(x_t,a_*)\}[\dot x_t].
\tag{PG.19}
\]
The old tuple is identical at the two entries of this difference, so the same Wilson subtraction is retained. But that tuple varies along the estimating path. PG.19 is the term a claimed response estimate must bound.

A constructive sufficient exterior criterion for the disputed \(b\le n<j\) range is therefore an estimate of the form
\[
\left|
\{D_xF_0(x_t,a)-D_xF_0(x_t,a_*)\}[\dot x_t]
\right|
\le B^x_{b,z;j,s}(t),
\tag{PG.20}
\]
where, after integration in \(t\), the positive majorant has the age and physical spatial row required of the crude response in ST.13–ST.14. It may then be combined with the endpoint Ward estimate for this same bank. Contributions from integrated-coordinate pullbacks must also be restored when the original target keeps those coordinates fixed: PG.18 is not an identity identifying their fixed-coordinate derivatives. All current, background and cutoff pieces of the same primitive remain included.

PG.20 is potentially weaker than a pointwise age bound on the entire reconstruction: it only asks for the anchored scalar response after the actual Wilson subtraction. Its feasibility is a substantive model-specific question. Neither MB.11 nor gauge invariance proves it. Conversely, MB.12's coarse plaquette detector alone does not disprove it, because that detector has not been identified with PG.1 on the literal stopped preparation geometry, and the subtraction could remove its leading response.

Finally, MB.9–MB.25 concern a real covariant path. C05's contour supremum additionally needs a common admitted native analytic family and its quantitative majorant. A real gauge identity, or a parameter-dependent choice of real gauges, does not establish that complex-family statement.

**Status.** The partial-integral identities and the anchored-score implication PG.12–PG.14 are proved. The all-history bound PG.20, the other anchored score pieces required by PG.12, and their application on the actual C05 graded preparation remain to be verified. No original all-history C05 closure is inferred here.
