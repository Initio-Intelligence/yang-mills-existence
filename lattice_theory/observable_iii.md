# Bounded finite parts and the actual regular mean metric

**Status:** The regular-bulk mean metric and the original-source phase-moment subgate are closed under the standing A7/A8/N7 and asymptotic-freedom premises. This is not a full-history S2 or Yang–Mills existence theorem. Equations in this module use the prefix **N9**.

The purpose is to control the actual phase-averaged critical transport, and then the moments of the original translated microscopic source. The positive kernel is not replaced by a random global translation. The exact digit representation is N8.6–N8.11; phase averaging is an average of original observables under the original law.

### 1. What has already been removed from the coefficient

The complete first-amplitude coefficient is the one in N8.14, including the source-dependent minimizer, constraint, gauge fixing, Jacobian, old-action score, and normalization. T9-A proves that the old **covariant current-link action** makes no contribution to its curvature jet. This is a full-density identity, not an identity for each individual polymer. T9-B replaces its truncated Gaussian moments by the untruncated moments with an arbitrarily rare error. Noncovariant and historical forcing remains in the A8 estimates.

For the uniform tensor source, T9.31–T9.34 give a further reduction. The actual Wilson/clover action mark is stationary on every constant commuting Cartan-flux background. Consequently its first fluctuation derivative vanishes there, and the complete mean coefficient, including its classical stable descendants, is the curvature coefficient of the actual constrained Gaussian trace. A convenient gauge may be used only after identifying the same physical quotient.

The seven orthogonal lattice-symmetry sectors in T9-C remove a nonnormal-matrix problem from the mean map. Scalar mean transport is bounded by N8.28–N8.38; pseudoscalar mean transport is bounded by T9-D. The proof below supplies the missing cumulative bound for all five tensor sectors by an exact Gaussian endpoint difference. It uses the gauge-coherent regulator comparison T9-F and the direct universal calculation U9, rather than requiring pointwise negativity of every finite-lattice coefficient.

### 2. An exact local source identity, including the tadpole

Work in any fixed independent coordinates on the actual constrained fluctuation fiber. At its physical stationary point, write

\[
\begin{aligned}
S(q)&=S(0)+\tfrac12 q^T Mq+\tfrac16 S_3[q,q,q]+O(q^4),\\
\log J(q)&=\log J(0)+j^Tq+O(q^2),\\
h(q)&=h(0)+l^Tq+\tfrac12q^THq+O(q^3),\qquad C=M^{-1}.
\end{aligned}
\tag{N9.1}
\]

Here \(J\) is the complete coordinate and coarea density. The action \(S\) includes the chosen gauge fixing on the same physical fiber. In an actual application the Hessian and cubic tensor are the constrained derivatives, not unrestricted Wilson derivatives with the constraint correction omitted.

Put \(q=\tau A\), and use the centered Gaussian of precision \(M\). Expanding the **normalized** expectation of \(h\), all terms multiplying \(h(0)\) cancel between numerator and denominator. Odd Gaussian moments vanish. Its coefficient at order \(\tau^2\) is

\[
\boxed{
b(h)=\frac12\operatorname{Tr}(CH)
-l^TC\left[\frac12(S_3:C)-j\right].
}
\tag{N9.2}
\]

The notation \(S_3:C\) contracts two indices of the cubic tensor. Wick's rule gives
\(\mathbb E[(l^TA)S_3[A,A,A]/6]=l^TC(S_3:C)/2\), which proves the second term with its coefficient and sign. This identity retains the tadpole and the Jacobian score; either may be nonzero for a point source.

Let \(q_\lambda\) be the constrained stationary point of \(S+\lambda h\), in the same coordinates, and let \(M_\lambda\) be its Hessian there. Differentiating the stationary equation gives

\[
q'_0=-Cl,\qquad M'_0=H-S_3[Cl].
\tag{N9.3}
\]

Therefore

\[
\boxed{
b(h)=-\left.\partial_\lambda
\log\left(\frac{J(q_\lambda)}{\sqrt{\det M_\lambda}}\right)
\right|_{\lambda=0}.
}
\tag{N9.4}
\]

Indeed the derivative of \(\log J(q_\lambda)\) is \(-j^TCl\), while the derivative of the determinant is
\(\operatorname{Tr}(CH)/2-l^TC(S_3:C)/2\). Thus (N9.4) is exactly (N9.2), rather than a determinant-only approximation to it. For the actual cutoff the additional difference is the controlled boundary contribution from T9-B; moving a cutoff with the stationary point without retaining its boundary score would not preserve (N9.4).

For the uniform source on the Cartan tests, T9.32 gives \(l=0\). The minimizing background then does not move, and every coordinate/coarea factor chosen from that background is source independent. In that case (N9.4) reduces to the constrained Hessian trace in T9.33. This simplification is specific to the uniform action mark; it is not imposed on an individual point insertion.

### 3. What exact Gaussian nesting does, and does not, establish

In fixed finite-dimensional coordinates split the fluctuation variable as \((a,b)\), with \(a\) in the next constrained fiber. For every source parameter for which the quadratic forms are invertible,

\[
M_\lambda=
\begin{pmatrix}A_\lambda&B_\lambda\\B_\lambda^T&D_\lambda\end{pmatrix},
\qquad
M^{\mathrm{ret}}_\lambda
=D_\lambda-B_\lambda^TA_\lambda^{-1}B_\lambda,
\qquad
\det M_\lambda=\det A_\lambda\det M^{\mathrm{ret}}_\lambda.
\tag{N9.5}
\]

Changing the chosen linear splitting multiplies the determinant identity by a coordinate factor. In the actual constrained operation the coarea factors must obey the corresponding change-of-variables identity. For a uniform stationary source these factors are source independent, so their source derivatives vanish exactly. For a local source they need not be source independent, and their derivatives belong to the \(J\) term of (N9.4).

The source derivative of (N9.5) is an exact telescoping identity. It does **not** by itself bound the retained endpoint as the original fine mesh tends to zero or as the infrared volume grows. Those bounds are separate estimates. Nor does it permit an independently gauge-fixed coarse Hessian to be substituted for the actual retained Schur complement without a quotient/coarea comparison.

### 4. The exact flat curvature filter of the source average

This section supplies an actual free-field limit, rather than an assumption about a generic block average. Let the current coarse lattice spacing be one, let the original spacing be \(\xi=L^{-k}\), and use centered link and plaquette Fourier coordinates. The linearization of CMP109 (0.4), (0.11)–(0.12) has a direct line-average term and a path term. The latter is a coarse gradient: the initial and terminal averaged paths differ only by their endpoints. A coarse curl annihilates that entire term.

Define

\[
s_\xi(q)=\frac{\xi\sin(q/2)}{\sin(\xi q/2)},\qquad
s_0(q)=\frac{\sin(q/2)}{q/2},
\tag{N9.6}
\]

with their continuous values at zero. A centered line average contributes \(s_\xi(q_\mu)\), the centered cell average contributes \(\prod_\rho s_\xi(q_\rho)\), and the gradient identity is
\(d_{1,\mu}=s_\xi(q_\mu)d_{\xi,\mu}\), where \(d_{\xi,\mu}=2i\xi^{-1}\sin(\xi q_\mu/2)\). Thus the exact curvature filter is

\[
\boxed{
K^\xi_{\mu\nu}(q)
=s_\xi(q_\mu)s_\xi(q_\nu)
\prod_{\rho=1}^4s_\xi(q_\rho).
}
\tag{N9.7}
\]

One may also derive (N9.7) one blocking step at a time. The trigonometric ratios telescope, so it is the iterated source filter, not a replacement averaging convention. Centered Fourier phases account for the positions of bonds and faces. They do not affect the estimates below.

Let \(p\in[-\pi,\pi]^4\), \(q=p+2\pi n\), and retain the aliases in the fine Brillouin zone. For each coordinate,

\[
|s_\xi(p_\rho+2\pi n_\rho)|+|s_0(p_\rho+2\pi n_\rho)|
\le\frac{C}{1+|n_\rho|},
\qquad
|s_\xi-s_0|
\le\frac{C\min(\xi^2|q_\rho|^2,1)}{1+|n_\rho|}.
\tag{N9.8}
\]

For the first bound use \(|\sin(\xi q/2)|\ge c\xi|q|\) inside the fine zone. For the second use
\(y/\sin y-1=O(y^2)\) for \(|y|\le\pi/2\). The aliases outside the fine zone are included in the comparison by setting the fine filter to zero there; their limiting-filter tail obeys the same summed estimate.

The free Maxwell curvature covariance \(\mathcal C_\xi(q)\) is uniformly bounded. It is the curl of the covariance \(1/|d_\xi(q)|^2\) with the gradient part cancelled. With the same value assigned to the removed zero mode,

\[
\|\mathcal C_\xi(q)-\mathcal C_0(q)\|
\le C\min(\xi^2|q|^2,1).
\tag{N9.9}
\]

The covariance of the blocked curvature is the alias sum

\[
\mathcal A_\xi(p)
=\sum_{n:\,p+2\pi n\in\mathrm{BZ}_\xi}
K^\xi(p+2\pi n)\,
\mathcal C_\xi(p+2\pi n)\,
K^\xi(p+2\pi n)^*.
\tag{N9.10}
\]

All matrix components have the summable bound
\(C\prod_\rho(1+|n_\rho|)^{-2}\). Furthermore

\[
\sum_{n\in\mathbb Z^4}
\min(\xi^2|p+2\pi n|^2,1)
\prod_\rho(1+|n_\rho|)^{-2}
\le C\xi.
\tag{N9.11}
\]

To verify (N9.11), bound the minimum by the sum of four one-coordinate minima and factor the other three summations. In one dimension split at \(|n|=\xi^{-1}\): the lower part contributes \(C\xi^2\sum_{|n|\le\xi^{-1}}1\le C\xi\), and the upper tail contributes \(C\sum_{|n|>\xi^{-1}}n^{-2}\le C\xi\). Equations (N9.8)–(N9.11) give the uniform limit

\[
\boxed{\sup_{p\in\mathrm{BZ}_1}
\|\mathcal A_\xi(p)-\mathcal A_0(p)\|\le C\xi.}
\tag{N9.12}
\]

This closes the free flat covariance-refinement subproblem for the actual source filter. It is not yet a background-curvature derivative estimate for the source determinant. Such a derivative contains the magnetic composition terms, which the next section retains.

#### 4.1 Uniform ellipticity of the actual retained action

Let \(G_k(p)\) be the covariance of the retained physical connection and \(M_k(p)=G_k(p)^{-1}\). The flat constrained variational problem identifies \(G_k\) with the covariance obtained by the actual tangent block average. On the current transverse space, inversion of the current curl has norm \(|d_1(p)|^{-1}\). The absolutely summable curvature alias bound above consequently gives

\[
G_k(p)\le C|d_1(p)|^{-2}I.
\tag{N9.12a}
\]

For the reverse inequality use only the zero alias \(q=p\). Write \(D_\xi(p)=\operatorname{diag}(s_\xi(p_\mu))\) and \(B_\xi(p)=\prod_\rho s_\xi(p_\rho)\). Every factor is bounded above and below by positive constants on the current Brillouin zone, independently of \(\xi\). Modulo the coarse gradient the zero-alias connection map is \(B_\xi D_\xi\). Since \(d_1=D_\xi d_\xi\), a current-transverse vector \(v\) satisfies \(D_\xi v\perp d_\xi\). Its zero-alias covariance is therefore

\[
\frac{|B_\xi D_\xi v|^2}{|d_\xi(p)|^2}
\ge c|d_1(p)|^{-2}|v|^2.
\]

All other aliases add nonnegative forms. Inverting the two inequalities proves

\[
\boxed{c|d_1(p)|^2I\le M_k(p)\le C|d_1(p)|^2I}
\quad\text{on the physical current space.}
\tag{N9.12b}
\]

The removed zero mode is handled by the infrared mass below. In particular, every nonzero one-step alias near zero coarse momentum has a uniform positive gap for fixed \(L\), independently of the original fine depth. This gap follows from the actual covariance; a bounded irrelevant remainder alone would not imply it.

### 5. Magnetic inverse jets and an integrable remainder

Use the midpoint symbol from T9.37. In one charged Cartan component fix the magnetic phase convention so that the product of two symbols is

\[
a\star_F b
=ab+\mathcal P_1^F(a,b)+\mathcal P_2^F(a,b)+O(F^3),
\quad
\mathcal P_1^F(a,b)=-\frac{i}{2}F_{\mu\nu}\partial_\mu a\,\partial_\nu b,
\quad
\mathcal P_2^F(a,b)=-\frac18F_{\mu\nu}F_{\rho\sigma}
\partial_\mu\partial_\rho a\,\partial_\nu\partial_\sigma b.
\tag{N9.13}
\]

The convention is \([\pi_\mu,\pi_\nu]=-iF_{\mu\nu}\), as in U9. Changing the charged-momentum convention changes the corresponding signs consistently. Formula (N9.13) follows directly by multiplying the two midpoint kernels: the additional phase is the flux through their triangle, and its first two derivatives are the displayed momentum-derivative contractions. Only these finite jets are used. No global holomorphic constant-field Fourier diagonalization is assumed.

Write \(M_F=M_0+M_1+M_2+O(F^3)\), where the subscripts are homogeneous curvature degrees, and let \(C_F=C_0+C_1+C_2+O(F^3)\) be its magnetic inverse. Then

\[
\begin{aligned}
C_0&=M_0^{-1},\\
C_1&=-C_0\bigl(M_1C_0+\mathcal P_1(M_0,C_0)\bigr),\\
C_2&=-C_0\bigl(M_2C_0+M_1C_1
+\mathcal P_1(M_1,C_0)+\mathcal P_1(M_0,C_1)
+\mathcal P_2(M_0,C_0)\bigr).
\end{aligned}
\tag{N9.14}
\]

These are obtained by equating the homogeneous terms in \(M\star_F C=I\). In particular, replacing magnetic composition by ordinary multiplication would omit two terms in \(C_2\).

Consider the actual current precision with the background gauge realization specified below. Its dimension-four leading symbol agrees with the continuum reference. Its difference and its first uniform-source derivative obey the weights in T9.40, including the required finite momentum derivatives:

\[
R_0=O(p^4),\quad R_1=O(Fp^2),\quad R_2=O(F^2),
\qquad
(R_J)_0=O(\|J\|p^4),\quad
(R_J)_1=O(\|J\|Fp^2),\quad
(R_J)_2=O(\|J\|F^2).
\tag{N9.15}
\]

Here is the required actual gauge realization. Add the current background gauge form \(DD^*\), held independent of the uniform tensor source. In midpoint bond coordinates the gradient has symbol \(d_\mu(p)=2i\sin(p_\mu/2)\), with its background parallel transport retained by magnetic composition. Its continuum gradient is \(ip_\mu\), and their difference has weighted order three. Consequently the difference between the lattice form \(DD^*\) and its continuum counterpart has precisely the weights \(p^4,Fp^2,F^2\) in (N9.15). The physical action part has those weights by T9-E, after summing the full covariant density family. Thus the full precision has (N9.15), with no source derivative of the gauge term. At zero curvature (N9.12b) and the gauge form give a uniform full-vector ellipticity bound.

On the stationary Cartan backgrounds both the action and source Hessians annihilate the infinitesimal gauge tangent. The determinant of this gauge-fixed operator with identity mass is the physical-quotient determinant with that mass times a gauge determinant. The latter is independent of the tensor source. Its source derivative vanishes before curvature differentiation, so this gauge realization computes the desired marked determinant. This is a quotient argument, not a claim that a vacuum determinant is gauge independent.

For \(\rho=(|p|^2+\mu^2)^{1/2}\), with a positive mass \(\mu^2I\), the resolvent and its finite magnetic jets have orders
\(C_0=O(\rho^{-2})\), \(C_1=O(F\rho^{-4})\), \(C_2=O(F^2\rho^{-6})\). The difference from the continuum reference gains two powers:

\[
\delta C_0=O(1),\qquad
\delta C_1=O(F\rho^{-2}),\qquad
\delta C_2=O(F^2\rho^{-4}).
\tag{N9.16}
\]

To check (N9.16), start with the resolvent identity for \(C_0\), then substitute it in the second and third lines of (N9.14). Each occurrence of \(R_0,R_1,R_2\) has respectively four, two, or zero powers of momentum, which gains two powers relative to the corresponding leading precision term. Momentum differentiation in \(\mathcal P_1,\mathcal P_2\) removes the same number of powers on both sides. The inequalities \(|p|\le\rho\) give the uniform massive bounds.

For the trace per unit volume, magnetic products integrate to ordinary products. This can be verified from the coincident kernel, or by integrating the antisymmetric momentum derivatives in (N9.13) on the full periodic Brillouin zone. The curvature-quadratic uniform-source trace is therefore

\[
I_J^{(2)}(p)=\operatorname{tr}
\bigl(C_0(M_J)_2+C_1(M_J)_1+C_2(M_J)_0\bigr),
\tag{N9.17}
\]

with polarization for mixed curvature directions. The dimension-four source has orders \(p^2,F,F^2\cdot0\) in its first three homogeneous terms. Equations (N9.15)–(N9.17) yield

\[
|I_{J,k}^{(2)}(p,\mu)-I_{J,\mathrm{cont}}^{(2)}(p,\mu)|
\le C\|J\|\rho^{-2},\qquad |p|\le p_0.
\tag{N9.18}
\]

This is integrable in four dimensions uniformly as \(\mu\downarrow0\). For \(p_0\le|p|\le\pi\), (N9.12b) and the finite symbol jets give a bounded integral. Thus the actual curvature/source determinant has a uniformly bounded finite part after subtraction of its universal continuum logarithm. A bounded finite part is enough; convergence of that finite part as \(k\to\infty\) is unnecessary.

### 6. The actual regulator and physical quotient

At a constant Cartan stationary background, let \(\overline Q\) be the original tangent block map induced on the physical gauge quotients, with source-independent quotient metrics. The background itself, the gauge tangent, and this quotient map are independent of the uniform source by T9.32. Adding a mass of the form \(m^2\overline Q^*\overline Q\) leaves the constrained high fiber unchanged. The exact Schur determinant identity T9.46 is

\[
\det(M_k+m^2\overline Q^*\overline Q)
=c_k(F)\det A_k\det(M_{k+1}+m^2I).
\tag{N9.19a}
\]

The factor \(c_k(F)\) is the determinant of the change to the fiber/right-inverse coordinates. It may depend on the background and volume, but its tensor-source derivative is identically zero. Taking that derivative before extracting the curvature coefficient removes it exactly. The same argument removes the gauge determinants introduced to compute each quotient determinant. No equality of independently chosen gauge matrices is asserted.

The raw source link-angle convention fixes the mass scale. A constant fine connection \(a\) has orthonormal \(L^4\)-cell soft coordinate \(L^2a\), while its coarse link angle is \(La\). Hence

\[
Q_{\mathrm{soft}}(0)=L^{-1}I,\qquad
\widetilde Q=LQ,\qquad m=L\mu.
\tag{N9.19b}
\]

Thus the fine mass in (N9.19a) is
\(\mu^2\overline{\widetilde Q}^{\,*}\overline{\widetilde Q}\), and the retained mass is \((L\mu)^2I\). Forgetting this factor would remove the continuum logarithm that must be present.

T9-F supplies the exact comparison of this block regulator with \(\mu^2I\). It uses the actual finite alias Bloch matrix, since the block regulator is not translation invariant on the fine lattice. At zero momentum its normalized soft component is the identity, all high-alias components vanish, the centered soft defect begins at \(p^2\), and the low-to-high component begins at \(p\). The high gap is (N9.12b).

On physical quotients the transverse projectors have singular curvature derivatives. Their explicit formula is \(P=I-D(D^*D)^{-1}D^*\), with magnetic products. Fine and coarse centered gradients differ from the common continuum gradient by weighted order three; their projector difference therefore has order two. After the gapped aliases are eliminated, the difference of the two soft mass perturbations obeys

\[
\delta M_0=\mu^2O(p^2),\qquad
\delta M_1=\mu^2O(F),\qquad
\delta M_2=\mu^2O(F^2|p|^{-2}),
\tag{N9.20}
\]

including the finite momentum derivatives and one tensor-source derivative. The possible \(p^{-2}\) in the last bound is retained, not replaced by a false bounded-projector assertion.

For clarity, the determinant estimate can be checked directly with (N9.13)–(N9.14). Put \(X=C_\mu\star\delta M\). Its zero-curvature part is \(O(\mu^2)\), its first curvature coefficient is \(O(\mu^2\rho^{-2})\), and its second is
\(O(\mu^2|p|^{-2}\rho^{-2})\). The two-first-derivative terms in \(\log_\star(I+X)\) are bounded by \(C\mu^4\rho^{-4}\), which is no larger than the second-order bound for \(0<|p|,\mu<1\). A source derivative has the same weights. Consequently

\[
|\delta I_J^{(2)}(p,\mu)|
\le C\|J\|\mu^2\left[
\frac1{(|p|^2+\mu^2)^2}
+\frac1{|p|^2(|p|^2+\mu^2)}\right],
\qquad
\int |\delta I_J^{(2)}|\,d^4p
\le C\|J\|\mu^2\bigl(1+|\log\mu|\bigr).
\tag{N9.21}
\]

The gapped aliases and the momentum region away from zero contribute \(O(\mu^2)\). This proves that the regulator discrepancy vanishes. It is stronger than a bounded error per blocking step.

The order of limits matters. Keep \(\mu>0\), remove global gauge stabilizers from the gauge parameter space, and form the bulk local coefficient by a large compatible torus limit or by the localized magnetic jets. Physical harmonic modes are regulated at this stage. Only then send \(\mu\downarrow0\). There is no claim that the physical projector is smooth at the zero momentum mode. The bound (N9.21) is locally integrable there; at fixed \(\mu\), a smallest nonzero momentum contribution has density size \(O(R^{-2})\) on a torus of side \(R\). Curvature differentiation is at zero curvature within the mass-dependent regular neighborhood. Positivity of an unregulated constant magnetic background is not required.

### 7. Bounded finite parts give the actual mean coboundary

Define the retained trace operator, in the same source and density normalization as T9.33, by

\[
\mathcal T_k(\mu)J
=\Pi_{\mathrm{bulk}}\frac1{2\,\operatorname{Vol}_k}
\operatorname{Tr}\bigl[(M_k(F)+\mu^2I)^{-1}M_{J,k}(F)\bigr].
\tag{N9.22}
\]

The gauge quotient is understood as in §§5–6; the source-independent gauge determinant has zero source derivative. The physical source is the full classical descendant of the original uniform microscopic Wilson/clover source. Thus its Hessian is \(M_{J,k}\), including the stable classical part, rather than the Hessian of an arbitrarily replaced current plaquette mark.

By (N9.18), subtracting the continuum principal integrand leaves an integrable function dominated by \(C\|J\||p|^{-2}\). For fixed \(k\) it converges as \(\mu\downarrow0\). The continuum principal integral itself is its logarithmic coefficient times \(\log(1/\mu)\), plus a finite constant depending on the fixed radial cutoff. Hence the limit

\[
\mathcal F_k
=\lim_{\mu\downarrow0}
\left[\mathcal T_k(\mu)-\Gamma_{\mathrm{cont}}\log(1/\mu)\right],
\qquad
\sup_k\|\mathcal F_k\|\le C_L
\tag{N9.23}
\]

exists in the finite-dimensional curvature coefficient space. The bound is uniform in the original fine depth. It may depend on the one fixed admitted block parameter \(L\). No limit of \(\mathcal F_k\) as \(k\to\infty\), and no uniformity as \(L\to\infty\), is needed.

Take the source derivative of (N9.19a), insert the raw mass pair \(\mu,L\mu\), and then apply (N9.21). The constrained high trace equals
\(\lim_{\mu\downarrow0}[\mathcal T_k(\mu)-\mathcal T_{k+1}(L\mu)]\).
Four-dimensional volume rescaling cancels the two curvature factors exactly: \(\operatorname{Vol}_k=L^4\operatorname{Vol}_{k+1}\) and \(F_{k+1}=L^2F_k\). Thus there is no extra density factor in the critical operator. Equation (N9.23) proves

\[
\boxed{
G_k^{\mathrm f}
=(\log L)\Gamma_{\mathrm{cont}}+\mathcal F_k-\mathcal F_{k+1}
+\mathcal E_k,\qquad
\sup_k\|\mathcal F_k\|<\infty.
}
\tag{N9.19}
\]

For the uncut whole-lattice Gaussian coefficient, \(\mathcal E_k=0\). Reinstating the actual cutoff gives \(\|\mathcal E_k\|\le C_Qx_k^{-Q}\) by T9-B. Local finite-volume tails are treated in §9. The old covariant additional action contributes zero to this coefficient by T9-A. Thus (N9.19) is an identity for the complete first-order mean coefficient \(A_k^1+B_k^1S_k^0\), with all its classical stable feedback.

The universal coefficient in (N9.23) is computed directly in U9 from the same marked Gaussian trace. In canonical units, with \(b=11C_A/(24\pi^2)\), it is

\[
\boxed{
\Gamma_{\mathrm{cont}}
=-bP_{\mathrm{stress}}
-\frac{18}{11}bP_{\mathrm{Weyl}}\le0.
}
\tag{N9.24}
\]

The scalar and pseudoscalar eigenvalues are zero. The source's fixed trace/coupling convention rescales \(b\) by the corresponding positive factor; it does not change the signs or their ratio. U9 derives the coefficient through the magnetic inverse, ordered source Hessian, angular contractions, and finite-group color trace. No unverified matching to a quoted continuum coefficient is used in (N9.19).

**Theorem N9-A — actual finite-part coboundary.** Under the established regular atlas and classical transport bounds, the original uniform Wilson/clover source has (N9.19), with bounded endpoint operators (N9.23) and the nonpositive principal operator (N9.24). The proof keeps the constrained quotient, the source-dependent classical source shape, the raw mass rescaling, and the gauge/coarea normalization. The regulator error tends to zero and does not produce an accumulated unknown finite coefficient.

### 8. The mean metric and all original-source phase moments

Let \(t_k=g_k^2=x_k^{-1}\), with the standing two-sided asymptotic-freedom increments
\(0<c_-\le x_k-x_{k+1}\le c_+\).
Then

\[
0\le t_{k+1}-t_k\le Ct_k^2,\qquad
\sum_{k<K}t_k^2\le Cx_K^{-1}.
\tag{N9.25}
\]

There is a particularly direct way to close the mean bound. T9-C shows that the exact mean map and both its graph coordinates are diagonal in the seven fixed orthogonal lattice sectors. N8.20a gives
\(G_k^{\mathrm f}-G_k^{\mathrm b}=R_k-R_{k+1}\), with \(\sup_k\|R_k\|<\infty\). Thus the actual backward-adjoint mean coefficient has (N9.19) with the bounded finite part replaced by
\(\widehat{\mathcal F}_k=\mathcal F_k-R_k\).

Let \(e_{\lambda,k}\) be its exact mean factor in one sector, and \(f_{\lambda,k}\) the corresponding eigenvalue of \(\widehat{\mathcal F}_k\). At a sufficiently weak fixed endpoint the factors are positive and

\[
\log e_{\lambda,k}
\le t_k\bigl[(\log L)\Gamma_\lambda
+f_{\lambda,k}-f_{\lambda,k+1}\bigr]
+C\bigl(t_k^2+t_k\epsilon_k+t_kx_k^{-Q}\bigr),
\quad
|f_{\lambda,k}|\le C,\quad
\epsilon_k=Cg_kr_{\chi,k}.
\tag{N9.26}
\]

This is N8's finite-jet and graph error, not an additional assumption about the mean spectrum. The first error is summable by (N9.25), and
\(t_k\epsilon_k\le Cx_k^{-3/2}(\log x_k)^c\) is summable as well.

For every interval \([a,b)\), Abel summation gives the exact identity

\[
\sum_{k=a}^{b-1}t_k(f_{\lambda,k}-f_{\lambda,k+1})
=t_af_{\lambda,a}-t_{b-1}f_{\lambda,b}
+\sum_{k=a+1}^{b-1}(t_k-t_{k-1})f_{\lambda,k}.
\tag{N9.27}
\]

Its absolute value is bounded by \(2Ct_{b-1}\), independently of the interval length. Since every \(\Gamma_\lambda\le0\), (N9.26) therefore bounds every interval product of the actual mean factors. This proves T9.29 in all five formerly unresolved tensor sectors. T9.30 supplies an exact positive metric:

\[
cI\le H_k\le CI,\qquad
E_k^*H_{k+1}E_k\le H_k,
\tag{N9.28}
\]

with constants independent of the original fine depth and of the finite horizon. This is the actual mean-metric hypothesis of S8-C, not a positivity inference from the Markov kernel. For the two neutral sectors the same argument with both signs bounds the mean product and its inverse.

The exact iid digit representation N8.6–N8.11 now applies to the original regular-bulk kernels. Its noise is \(O(t_k)\); the stable part has its fixed contraction. S8-C gives a uniform second moment, and P9, using the same metric and the deterministic N7 polynomial propagator, gives for the engineered rooted source

\[
\mathbb E_{\mathrm{uniform\ root\ phase}}\|f_k\|^m
\le C^{m+1}(m!)^{d_{\mathrm{ph}}}\|f_0\|^m,
\qquad m\ge1,
\qquad d_{\mathrm{ph}}=\lceil p_{\mathrm b}\rceil.
\tag{N9.29}
\]

The weak-endpoint threshold is independent of \(m\). These norms use exactly the deterministic vacuum convention and engineering rescaling of N8 and P9. No carrier-dependent exterior function is discarded as a scalar. Joint root estimates use Hölder as in P9 and do not require independent phases for different roots.

**Theorem N9-B — original regular phase transport.** The covariant regular-bulk transport of the actual microscopic Wilson/clover family has a bounded common mean metric and the all-order translation-phase moment estimate (N9.29). For the scalar Wilson field, the common scalar mean normalizer and its inverse remain bounded. The result controls the original family averaged over its deterministic translation phases; it neither replaces the frozen kernel by a global phase mixture nor asserts a uniform worst-phase point norm.

The all-21-component moment statement is for uniformly bounded deterministic initial seeds with the stated engineering and vacuum convention. The scalar and pseudoscalar renormalized seeds have bounded initial inverse mean factors. Stress and Weyl renormalization can instead multiply the initial seed by inverse mean factors with powers \(1\) and \(18/11\) of the inverse-coupling ratio. Such seeds are not uniformly bounded in (N9.29). This theorem therefore does not prove the fully renormalized stress/Weyl point moments or the full-matrix endpoint statement SP37.

Born or reset forcing can depend on later digits. It must enter through the deterministic propagator and the already established maturity/rare-forcing estimates, not by treating those digits as independent of the forcing. This is exactly the distinction in N8 and P9.

### 9. Finite volume and the remaining historical scope

The finite parts in (N9.23) are defined through bulk coefficients after keeping the mass positive. One does not need a volume-uniform massless unconstrained determinant. The constrained high trace appearing in the difference is local with a fixed current-scale gap. The actual covariance, minimizing response, and localized source kernels therefore compare on a protected patch with their compatible whole-lattice coefficient by the existing exponential wrapping and cutoff-affine tails.

For a plateau at current physical distance \(D\) from the finite-volume boundary, these tails have the form \(C\exp(-cD/h_k)\). Their contribution to the mean step is multiplied by \(t_k\). Because \(h_k\) grows geometrically,

\[
\sum_{k<K}t_k\,e^{-cD/h_k}
\le C t_K e^{-c'D/h_K}
\tag{N9.30}
\]

whenever \(D/h_K\) is bounded below by the fixed protected-patch margin. This estimate preserves a common finite-volume metric after changing its bounded constants. It does not declare a cutoff-affine torus projection exactly translation-annihilating.

The all-orders phase result removes the regular-bulk tensor-growth bottleneck from the averaged S2 route. It does not prove normalized estimates for every large-field or mixed-boundary history. Those estimates are the independent H9/R9 obligations. A reset may also change the observable argument, so conservation or stationarity of a uniform microscopic action cannot be imposed across such a reset without its actual transport identity.

### 10. Status summary

| Item | Status |
|---|---|
| Local source tadpole, constraint, and Jacobian accounting | Exact identities (N9.1)–(N9.4) |
| Actual iterated flat curvature averaging | Exact filter (N9.7) |
| Free blocked curvature refinement limit | Uniform \(O(\xi)\) estimate (N9.12) |
| Actual retained ellipticity and high-alias gap | Two-sided bound (N9.12b) |
| Magnetic inverse and integrable irrelevant correction | (N9.13)–(N9.18), with actual gauge realization |
| Gauge/coarea and infrared mass comparison | Exact T9-F identity and vanishing bound (N9.21) |
| Complete mean tensor coefficient | Bounded finite-part coboundary, Theorem N9-A |
| Five tensor interval-growth bounds | Proved by (N9.24)–(N9.28) |
| Original regular-bulk translation-phase moments | All orders, one threshold, Theorem N9-B |
| Fully renormalized stress/Weyl point family and SP37 | Remain open; unbounded initial inverse mean factors are not covered |
| Full historical S2 and Yang–Mills existence | Remain separate; no claim of completion |

#### Companion and primary sources

- [Appendix B](observable_appendix_b.md), point normalization: N8.6–N8.14, N8.20a, and N8.28–N8.38.
- [observable_i.md](observable_i.md), tensor generator: T9-A/B for the actual score and cutoff reductions; T9-C/D for the symmetry and neutral sectors; T9-E for the physical magnetic remainder; T9-F for the source-independent quotient, raw mass scale, and regulator comparison.
- [observable_ii.md](observable_ii.md), universal tensor trace: U9.1–U9.18, the direct angular/color calculation of the same source trace, including its gauge and coupling conventions.
- [observable_vii.md](observable_vii.md), phase moments of all orders: the all-orders implication, whose mean metric is now supplied by (N9.28).
- Balaban, CMP109, (0.4), (0.11)–(0.12): the actual averaged contour and block-link maps; (2.6)–(2.12): the constrained fluctuation Hessian and independent coordinates.
- Balaban, CMP99, (3.126)–(3.153): the actual minimizing response and constrained propagator identities. Their constants may depend on the fixed block parameter \(L\).

---
