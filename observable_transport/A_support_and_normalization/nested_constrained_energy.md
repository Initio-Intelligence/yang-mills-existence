# A common constrained Hessian transfers the original test exponent

This note gives the precise linear energy comparison needed by the
finite-restoration route. It explains why a polynomial bound on every
coordinate map need not degrade the original R^9 test bound. The
linear and differential statements below are proved. Identifying
the complete source positive energy with this Hessian remains an
application input, specified in Section 4.

## 1. Nested readouts of one positive quadratic

Let X be a finite-dimensional real physical space after gauge null
directions and the fixed terminal linear constraints have been
removed. Let H be positive definite on X. Let A:X→Z be a surjective
master readout, and suppose the readout of history i is
B_i=L_i A. Define the exact minimum energies

\[
 q_*(z)=\inf_{Au=z}\tfrac12\langle u,Hu\rangle,\qquad
 q_i(y)=\inf_{B_i u=y}\tfrac12\langle u,Hu\rangle.
 \tag{NE.1}
\]

For every z,

\[
 \boxed{\qquad q_i(L_i z)\le q_*(z).\qquad}
 \tag{NE.2}
\]

Indeed the master constraint fiber is a subset of the history-i
fiber. Equivalently,

\[
 q_*(z)=\tfrac12
  \langle z,(AH^{-1}A^*)^{-1}z\rangle,
 \tag{NE.3}
\]

with the analogous formula on the image of B_i. Any redundant
coordinates are removed or restricted to that image. A determinant
on a redundant constraint space is not used.

Suppose a particular original history test satisfies

\[
 \|T_i y\|^2\le C R^9 q_i(y).
 \tag{NE.4}
\]

Then its pullback satisfies exactly

\[
 \|T_i L_i z\|^2\le C R^9 q_*(z).
 \tag{NE.5}
\]

There is no norm of L_i in this estimate. Bounding that norm
separately would lose information about the energy geometry and
can introduce an unnecessary power of the master rank.

Independent padded soft-gauge variables can be included in X with
their own positive quadratic blocks. If a test uses its original
sampler, its corresponding energy block is retained. A compact
gauge direction with zero action cannot instead be called a
positive Gaussian variable.

## 2. Successive Schur eliminations preserve the same energy

For a block decomposition u=(x,y),

\[
 \tfrac12 u^THu=
 \tfrac12(y^TSy)+
 \tfrac12(x+H_{xx}^{-1}H_{xy}y)^T
 H_{xx}(x+H_{xx}^{-1}H_{xy}y),
 \tag{NE.6}
\]

where \(S=H_{yy}-H_{yx}H_{xx}^{-1}H_{xy}\).
Completing squares again in either block gives the minimum over
the union of the eliminated variables. Infima over a Cartesian
fiber commute. Thus any sequence of exact Schur eliminations
gives the same reduced form as one simultaneous elimination.

The statement includes the complete off-diagonal Schur terms.
Deleting a term because its entries were assigned to a source
boundary interaction would change the quadratic. A uniformly
small relative off-diagonal remainder may be absorbed after a
separate estimate, but is not identically zero.

This is why restoration should add conditional quadratic energies
to the retained Schur form, rather than multiply unrelated
conditional-mean inequalities at every scale.

## 3. Nonlinear constraints and the actual background force

There is a corresponding differential theorem. Let M be the
smooth manifold defined by the *exact fixed terminal constraints*
and a valid local gauge quotient. Let S be the physical action
restricted to M, and suppose x_0 is a nondegenerate local minimum.
In local coordinates on M centered at x_0,

\[
 S(u)=S(0)+\tfrac12 u^THu+O(\|u\|^3).
 \tag{NE.7}
\]

Let r:M→Z be a smooth submersion with r(0)=0 and dr(0)=A.
For the local minimizing value
\(\mathcal S_r(z)=\min\{S(u):r(u)=z\}\),

\[
 d\mathcal S_r(0)=0,\qquad
 \tfrac12 d^2\mathcal S_r(0)[z,z]=q_*(z).
 \tag{NE.8}
\]

**Proof.** A constrained minimizer has first variation
u(z)=u_1(z)+O(\|z\|^2), where A u_1=z.
The multiplier for the new readout constraints is zero at z=0,
because S is already critical on all of M. The first nonconstant
term of its value is therefore the minimum of
\(\tfrac12 u_1^THu_1\) subject to A u_1=z. The positive Hessian
on the kernel supplies the local smooth minimizing branch by the
implicit function theorem. This proves NE.8.

If r_i=f_i∘r, then dr_i(0)=df_i(0)A and NE.2 applies to the
Hessians of the two minimizing values.

### Force precision

The restriction to M is essential. In ambient coordinates with
terminal constraint \(\Phi(u)=v\), the correct constrained Hessian is

\[
 H=\left.
   \left(S''-\sum_\alpha\lambda_\alpha\Phi_\alpha''\right)
   \right|_{\ker D\Phi},
 \tag{NE.9}
\]

with the actual terminal Lagrange multipliers. The ambient gradient
of S need not vanish. Omitting the multiplier term would repeat
the incorrect step of treating a constrained Wilson minimum as an
unconstrained critical point.

For every finer readout whose value is chosen from the same x_0,
the same terminal-constrained minimum persists. On M its new
readout multiplier is zero. This is the valid common-background
reason for the Schur nesting. It does not require erasing the
actual exterior Wilson force.

## 4. Conditional source consequence and its outstanding identity

The promoted master construction PM gives literal nonlinear
readout factorization for its admitted finite lists. The common
reference U_0 is the source minimum with the prescribed current
field outside the prepared core. Thus PM and variational uniqueness
provide the structural inputs to Section 3 after a valid terminal
constraint chart and gauge quotient are established.

To apply NE.5 to ER's restored positive energy, one still must show
on the relevant actual support that

\[
 E_*(z)\ge c\,q_*(z)-o(1)
 \tag{NE.10}
\]

and that the linearized original test form in LFR II (1.77)--(1.78)
is the q_i belonging to the same H, up to fixed comparable factors.
The following bookkeeping is necessary:

- The outer and inner energy pieces use their actual partition
  of the common reference action.
- All original and restored ordinary Schur cross terms are kept.
- The genuine terminal multiplier contribution in NE.9 is
  retained, or quantitatively included in the source error.
- Running-coupling weights are compared in the same normalization.
- Gauge samplers used by the alternative test retain their
  original positive cost and exact pullback.
- The nonlinear test error and its reference offset are bounded
  on the actual support by less than a fixed fraction of p_1.

If these statements hold, the already original test exponent 9
survives refinement. Combining NE.5, NE.10 and a small nonlinear
test remainder gives failure energy at least
\(c p_1^2/R^9-o(1)\). The positive-energy exchange theorem AE then
uses the existing parameter hierarchy, without strengthening it
to pay an arbitrary power of D.

NE.10 is not proved by a rank count or a primitive analytic
radius. This note isolates the exact source energy identity that
would finish that part of the argument.

## Related notes

- M04_Raw_Master_Determination.md, PM.1--PM.11.
- M04_Refined_Forest_Density.md, FD.5--FD.10.
- M04_Finite_Restoration_Energy_Reserve.md, ER.3--ER.11.
- energy_exchange_reduction.md, AE.10--AE.12.
- The original constrained-background force analysis and
  first_step_precision_gap.md.
