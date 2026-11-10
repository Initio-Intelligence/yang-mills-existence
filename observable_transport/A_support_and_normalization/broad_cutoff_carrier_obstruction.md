# A genuine carrier obstruction for broad hard cutoffs

## Outcome and exact scope

Uniform convexity, a fixed finite interaction range, a volume-uniform mass gap, and the exact one-coordinate response estimates of HC do **not**, by themselves, imply a uniform exponential physical-carrier expansion for a broad hard-cutoff conditional quadratic observable.

The counterexample below is a positive, normalized scalar Gaussian conditional with the actual product cutoff \([-P,P]\) on every integrated coordinate. Its precision is a fixed nearest-neighbor massive weighted Laplacian. All retained values have magnitude less than \(2P\). Only one fixed edge weight is exceptional; no parameter of the precision grows with \(P\) or volume. The observable is the nonnegative square of one integrated coordinate.

For every fixed positive carrier-volume rate, the energy-weighted carrier norm diverges along an explicit sequence of domains and cutoffs. The proof uses one fixed mask and mixed differences of retained values. It obstructs **every** absolutely summable supported decomposition with that norm, not merely one reset or inclusion-exclusion prescription.

This is a **surrogate precision**, not a realization of the actual Yang–Mills first-step precision or its Wilson scalar. In the initial Laplacian construction the adjacent baseline pin exceeds \(P\); Section 8 removes even that feature by one fixed diagonal congruence and places all retained data strictly below \(P/2\). Section 9 gives the same obstruction for a local gradient energy. Neither corollary identifies the actual source precision. HC, the untruncated GMK theorem, the narrow-cutoff MP theorem, and the earlier specified-interface GO obstruction remain unchanged. The result identifies a missing structural input for extending HC to full carriers.

## 1. A necessary mixed-difference consequence of the carrier norm

Fix the mask. Suppose a scalar conditional observable has an absolutely convergent supported decomposition
\[
 F(r)=\sum_X F_X(r),\qquad
 |F_X(r)|\le b_X\left(1+\sum_{j\in X}|r_j|^2\right),\qquad
 \mathcal B_\kappa=\sum_X e^{\kappa|X|}b_X<\infty.       \tag{BC.1}
\]
Each \(F_X\) depends only on retained coordinates whose genuine physical slots lie in \(X\). Multiple tags with the same carrier are allowed. The same argument applies to the shifted native regulator: a single bounded shift changes the displayed bound by at most a fixed factor on the configurations below. A tree factor strengthens the assumed norm and is unnecessary for the lower bound.

At \(N\) distinct retained sites \(S=\{b_1,\ldots,b_N\}\), put
\[
 r_{b_j}(\sigma)=Pa_j\sigma_j,\quad |a_j|\le a_*<1,\qquad
 r_{b_0}=cP,\quad |c|<2,                              \tag{BC.2}
\]
where the \(\sigma_j\) are independent signs. All other retained coordinates are zero. Define
\[
 \widehat F(S)=2^{-N}\sum_{\sigma\in\{-1,1\}^N}
        \left(\prod_{j=1}^N\sigma_j\right)F(r(\sigma)). \tag{BC.3}
\]
A tagged term missing any site of \(S\) has zero coefficient. Every remaining term has \(|X|\ge N\); its regulator is at most \(1+P^2(4+Na_*^2)\). Consequently, for \(P\ge1\),
\[
 \boxed{\quad
 P^{-2}|\widehat F(S)|
 \le C(N+1)e^{-\kappa N}\mathcal B_\kappa.
 \quad}                                             \tag{BC.4}
\]
This is representation independent. If a physical cell contains at most a fixed \(J_*\) of these sites, replace \(N\) in the exponential by \(N/J_*\), with no change to the conclusion.

## 2. One fixed massive finite-range precision

Let \(d\ge3\), including \(d=4\). On the integer lattice, or a periodic box much larger than the domains below, take
\[
 K=\mu I+\mathcal L_w,\qquad \mu>0,                   \tag{BC.5}
\]
where \(\mathcal L_w\) is the nearest-neighbor graph Laplacian. Every edge weight is one except the fixed edge
\[
 b_0=(0,0,\ldots,0)\longleftrightarrow
 o=(1,0,\ldots,0),
\]
whose weight is a fixed number
\[
 w_0>2d-1+\mu.                                       \tag{BC.6}
\]
For example \(\mu=1,w_0=4d+2\) works. The same edge and precision rule are used for every domain and cutoff. In particular,
\[
 \mu I\le K\le[\mu+2(w_0+2d-1)]I.                    \tag{BC.7}
\]
Range, absolute row bounds, block dimension and principal-matrix mass gaps are fixed. Thus this is within the real Gaussian assumptions of HC, with \(W=0\).

For \(R\ge2\) integrate
\[
 I_R=\{1,\ldots,R\}\times\{-R,\ldots,R\}^{d-1},\qquad
 n_R=R(2R+1)^{d-1}.                                  \tag{BC.8}
\]
Every other site is retained. Write \(G_R=(K_{I_RI_R})^{-1}\). Its entries are positive. Choose all sites on the opposite face
\(\{R+1\}\times\{-R,\ldots,R\}^{d-1}\) except one as \(S_R\). Then
\[
 N_R=(2R+1)^{d-1}-1                                  \tag{BC.9}
\]
is even and at least four. The unique integrated neighbor of \(b_j=(R+1,y_j)\) is \(v_j=(R,y_j)\). Its root influence is
\[
 \omega_j=(G_R)_{ov_j}>0.                            \tag{BC.10}
\]
Put \(D_*=\mu+w_0+2d-1\). The positive diagonal-Neumann expansion contains a nearest-neighbor path from \(o\) to \(v_j\) of length at most \(dR\), whence
\[
 \omega_j\ge D_*^{-(dR+1)}.                           \tag{BC.11}
\]
The upper bound
\[
 \sum_{j=1}^{N_R}\omega_j\le1                         \tag{BC.12}
\]
follows from the maximum principle: the sum is the value at \(o\) of the massive harmonic extension with boundary value one on \(S_R\) and zero on the remaining retained sites.

## 3. A wall-centered baseline with all other means buffered

Set
\[
 c_R=(w_0(G_R)_{oo})^{-1}.                            \tag{BC.13}
\]
With retained value \(c_R\) at \(b_0\) and zero elsewhere, the unrestricted conditional mean is
\[
 u_i=(G_R)_{io}/(G_R)_{oo},\qquad u_o=1.              \tag{BC.14}
\]
Treating \(o\) as prescribed value one, the maximum principle gives \(0\le u_i\le1\). At every \(i\ne o\) the full weighted degree is \(2d\), so its equation gives
\[
 0\le u_i\le\frac{2d}{2d+\mu}=1-\delta,\qquad
 \delta=\frac{\mu}{2d+\mu}>0.                         \tag{BC.15}
\]
The equation at \(o\) is
\[
 w_0c_R=w_0+\mu+\sum_{i\sim o,\ i\ne b_0}(1-u_i).
\]
Therefore
\[
 1<c_R\le1+\frac{2d-1+\mu}{w_0}<2.                   \tag{BC.16}
\]
A retained value below \(2P\) thus places the root mean exactly at its cutoff \(P\), while all other integrated means remain a fixed fraction below that wall.

Choose \(0<a_*\le\delta/8\) and put
\[
 \epsilon_R=a_*\min_j\omega_j,\qquad
 a_j=\epsilon_R/\omega_j\in(0,a_*].                  \tag{BC.17}
\]
Equation (BC.12) implies
\[
 N_R\epsilon_R\le a_*.                               \tag{BC.18}
\]
Now use the retained values (BC.2), with \(c=c_R\) and these \(a_j\). The unrestricted mean of \(y=z/P\) is
\[
 m_i(\sigma)=u_i+\sum_j(G_R)_{iv_j}a_j\sigma_j,\qquad
 m_o(\sigma)=1+\epsilon_R\sum_j\sigma_j.              \tag{BC.19}
\]
The maximum principle bounds the perturbation by \(a_*\) at every site. All nonroot means are consequently in \([-a_*,1-\delta+a_*]\).

### Lemma BC.1 — the exact constrained minimizer

Let \(y^\sigma\) minimize the conditional quadratic potential over the complete product cube \([-1,1]^{I_R}\). Then
\[
 y_o^\sigma=\min\left(1+\epsilon_R\sum_j\sigma_j,1\right).
                                                               \tag{BC.20}
\]
Every other coordinate stays strictly between the two walls with a gap bounded below independently of \(R,\sigma\).

**Proof.** If \(m_o\le1\), the unrestricted mean already belongs to the cube; its root coordinate is at least \(1-a_*>0\). If \(m_o>1\), impose \(y_o=1\). Exact quadratic conditioning gives
\[
 y_i=m_i-u_i(m_o-1),\qquad i\ne o.                   \tag{BC.21}
\]
The subtracted amount lies between zero and \(a_*\), so
\(-2a_*\le y_i\le1-\delta+a_*\). All these coordinates remain interior. The gradient is zero there, and at \(o\) it is
\(-(m_o-1)/(G_R)_{oo}<0\), the correct sign for an active upper constraint. These are the convex optimality conditions. Strict convexity gives uniqueness, with equality \(m_o=1\) included. ∎

## 4. The complete hard-cutoff conditional and its finite-P error

There is no replacement of the cutoff completion by an unrestricted Schur law. Define the actual conditional
\[
 q_{R,P}^\sigma(dz)=
 \frac{\mathbf1_{[-P,P]^{I_R}}(z)
 e^{-\frac12z^TK_{I_RI_R}z-z^TK_{I_RO}r(\sigma)}\,dz}
 {\int_{[-P,P]^{I_R}}
 e^{-\frac12z^TK_{I_RI_R}z-z^TK_{I_RO}r(\sigma)}\,dz}. \tag{BC.22}
\]
Every denominator is strictly positive; every cutoff volume and retained-force factor is kept. The local mark is
\[
 F_{R,P}(r(\sigma))=q_{R,P}^\sigma(z_o^2).            \tag{BC.23}
\]

After \(z=Py\), the density is proportional to \(e^{-P^2\Psi_\sigma(y)}\) on the fixed cube, with Hessian \(K_{I_RI_R}\). The following estimate includes the exact normalizer:
\[
 \mathbb E_{q_{R,P}^\sigma}|z/P-y^\sigma|^2
 \le\frac{n_R}{\mu P^2}.                             \tag{BC.24}
\]
Indeed, integrate the divergence of
\((y-y^\sigma)e^{-P^2\Psi_\sigma(y)}\). The outward flux is nonnegative on every face, because the minimizer belongs to the cube. Hence
\[
 P^2\mathbb E[(y-y^\sigma)\cdot\nabla\Psi_\sigma(y)]\le n_R.
\]
The variational inequality at the constrained minimizer and the mass bound give
\((y-y^\sigma)\cdot\nabla\Psi_\sigma(y)\ge\mu|y-y^\sigma|^2\).
This proves (BC.24), including a minimizer on the wall, without any cutoff-probability denominator.

Both root values belong to \([-1,1]\). Thus, uniformly over all \(2^{N_R}\) sign configurations,
\[
 \left|P^{-2}F_{R,P}(r(\sigma))-(y_o^\sigma)^2\right|
 \le\frac{2\sqrt{n_R/\mu}}{P}.                        \tag{BC.25}
\]
Averaging to form a Walsh coefficient does not multiply this error by \(2^{N_R}\).

## 5. The exact high mixed coefficient

Let \(N=N_R\) be even, \(N\ge4\). Write \(T_N=\sum_j\sigma_j\) and \(\chi_N=\prod_j\sigma_j\). Then
\[
 (y_o^\sigma)^2
 =1+2\epsilon_R\min(T_N,0)
       +\epsilon_R^2\min(T_N,0)^2.                   \tag{BC.26}
\]
The full Walsh coefficients of constants, \(T_N\) and \(T_N^2\) vanish. Also \(T_N|T_N|\) is odd under simultaneous sign reversal while \(\chi_N\) is even. Since
\(\min(T,0)=(T-|T|)/2\) and
\(\min(T,0)^2=(T^2-T|T|)/2\), one gets exactly
\[
 \mathbb E_\sigma[\chi_N(y_o^\sigma)^2]
 =-\epsilon_R\mathbb E_\sigma[\chi_N|T_N|].          \tag{BC.27}
\]
The elementary binomial identity is
\[
 \mathbb E_\sigma[\chi_N|T_N|]
 =(-1)^{N/2-1}\frac{N}{N-1}\,2^{-N}\binom N{N/2}.   \tag{BC.28}
\]
One proof pairs the \(k\)-negative-sign term with the \(N-k\) term in
\(2^{-N}\sum_k(-1)^k\binom Nk|N-2k|\), then uses the partial alternating binomial sum. The absolute value also equals
\(2^{2-N}\binom{N-2}{N/2-1}\). Consequently, for universal constants,
\[
 cN^{-1/2}\le
 c_N:=|\mathbb E_\sigma[\chi_N|T_N|]|
 \le CN^{-1/2}.                                     \tag{BC.29}
\]

Combining (BC.25),(BC.27), whenever
\[
 P\ge\frac{4\sqrt{n_R/\mu}}{\epsilon_R c_{N_R}},       \tag{BC.30}
\]
the actual finite-cutoff conditional satisfies
\[
 \boxed{\quad
 P^{-2}|\widehat F_{R,P}(S_R)|
 \ge\tfrac12\epsilon_R c_{N_R}
 \ge c\epsilon_R/\sqrt{N_R}.
 \quad}                                            \tag{BC.31}
\]
By (BC.11),(BC.29), the required \(P\) grows at most exponentially in \(R\) times a fixed polynomial. The influential shell radius is therefore of order \(\log P\).

## 6. No uniform exponential carrier-volume bound

Applying (BC.4) to (BC.31) gives, for **every** supported decomposition,
\[
 \boxed{\quad
 \mathcal B_\kappa(F_{R,P})
 \ge c\,\frac{\epsilon_R e^{\kappa N_R}}{N_R^{3/2}}
 \ge c\,\frac{\exp[\kappa N_R-CR]}{N_R^{3/2}}.
 \quad}                                            \tag{BC.32}
\]
All constants depend only on fixed \(d,\mu,w_0,a_*\). For every \(\kappa>0\) and \(d\ge3\), \(N_R\asymp R^{d-1}\), and this lower bound diverges as \(R\) increases along cutoffs satisfying (BC.30). Already the pointwise value norm diverges; current and outer-moment terms cannot fix it.

The incoming mark \(z_o^2\) is supported at one site with unit incoming energy coefficient. The lower bound is not an inflated input budget. Its \(P^2\) amplitude is paid exactly once by native retained energy in (BC.4); the remaining exponential loss cannot be absorbed in a polynomial regulator.

### Theorem BC.2 — broad-cutoff real assumptions are insufficient

There is a family of finite-volume normalized product-cutoff Gaussian conditionals, all obtained from the same massive finite-range precision rule with fixed uniform constants, and a fixed local nonnegative quadratic mark, for which every positive exponential physical-volume carrier norm of the form (BC.1) is unbounded uniformly in the broad cutoff \(P\) and volume. All retained data in the lower bound lie in \((-2P,2P)\). The mask is fixed throughout each mixed-difference experiment. ∎

## 7. Interpretation and exact M04 boundary

1. HC's distance and summed-first-current estimates are consistent with the example. The amplitude \(\epsilon_R\) is exponentially small in distance, but not exponentially small in the number of independent sites on the remote shell.

2. Finite-difference cancellation is evaluated exactly in (BC.28). It leaves \(N^{-1/2}\), rather than an exponential in \(N\). Because (BC.4) is representation independent, choosing different reset coefficients cannot evade this obstruction.

3. The finite-\(P\) density and its conditional mean are smooth in all retained values. There is no finite-cutoff discontinuity in this proof. The explicit concentration estimate (BC.25) justifies the wall limit. Bounded unit continuous currents do not imply the needed uniform higher mixed dependence.

4. The untruncated conditional quadratic is quadratic in the retained data, so its full Walsh coefficient vanishes for \(N>2\). The hard-wall completion creates (BC.31). The matrix inverse expansion in GMK therefore does not provide a completion expansion.

5. This construction does not identify the actual YM exceptional precision with (BC.5), replace a Wilson plaquette by \(z_o^2\), or prove source attainability of this wall configuration. In the initial Laplacian version the baseline pin exceeds \(P\), whereas an actual R-good padded collar can impose a stricter bound. Section 8 shows that a generic retained-size restriction alone is insufficient for a general fixed positive precision: its congruent model has all retained data below \(P/2\). A source-specific conditional-mean margin would be a different assertion and still requires proof.

6. A different positive extension on inconsistent masks could differ from the common primitive density used here. Its exact agreement on the actual law, local support, and all currents would need a new proof. The result is not a no-go theorem for every amended interface.

7. Any actual broad completion theorem now needs genuinely additional structure: for example a verified source-specific margin for the relevant conditional means, a physical-scalar cancellation in the wall direction, or a different exact ambient extension with its own carrier bounds. None is assumed or proved in this note.

The established conclusion is a precise limitation of the generic broad-cutoff strategy, not an additional Yang–Mills no-go claim.

## 8. Actual joint law, genuine input budget, and pins below P/2

The example is compatible with genuine input and outgoing moment reserves; it does not rely on replacing an averaged input budget by a pointwise one.

First take the centered joint Gaussian with precision \(K\), restricted to \([-P,P]\) at the slots of \(I_R\) and to \([-2P,2P]\) at retained slots. Its conditional given the retained values (BC.2) is exactly (BC.22). Every displayed retained configuration lies in the interior of a positive-density marginal. The joint law is even and uniformly log-concave.

There is also a variant with the *same cutoff P on every joint coordinate* and every displayed retained value below \(P/2\). Let \(T\) be the diagonal map which is four at \(b_0\) and one elsewhere, and set
\[
 \widetilde K=T^TKT,\qquad
 \widetilde r_{b_0}=c_RP/4,\qquad
 \widetilde r_{b_j}=Pa_j\sigma_j.                    \tag{BC.33}
\]
All other retained coordinates stay zero. Since \(b_0\) is retained, the integrated principal matrix is unchanged and
\[
 \widetilde K_{I_RI_R}=K_{I_RI_R},\qquad
 \widetilde K_{I_RO}\widetilde r=K_{I_RO}r.           \tag{BC.34}
\]
The normalized conditional is therefore exactly (BC.22), including every cutoff and denominator. Yet
\[
 |\widetilde r_{b_0}|<P/2,\qquad
 |\widetilde r_{b_j}|\le a_*P<P/2.
\]
The precision is still fixed, finite range and uniformly positive:
\[
 \mu I\le\widetilde K\le
 16[\mu+2(w_0+2d-1)]I.                              \tag{BC.35}
\]
The upper constant is merely changed by a fixed factor. This congruent precision need not be a diagonally dominant Laplacian; no such property is part of the generic HC assumptions.

Take the **actual full joint law**
\[
 \widetilde\mu_{R,P}(dx)
 \propto\mathbf1_{[-P,P]^{G_R^{\rm amb}}}(x)
          e^{-\frac12x^T\widetilde Kx}\,dx,          \tag{BC.36}
\]
on a finite ambient torus containing the whole construction, with the indicated fixed mask. Its actual conditional on \(I_R\) is the one already analyzed. All sign-cube values are interior positive-density retained fibers.

Convex-barrier approximation, followed by the strongly convex covariance bound, gives
\(\operatorname{Var}_{\widetilde\mu^t}(x_i)\le\mu^{-1}\) for every real one-coordinate exponential tilt. Evenness gives mean zero at tilt zero. Integrating the second derivative of the log moment generating function proves
\[
 \widetilde\mu_{R,P}e^{t x_i}\le e^{t^2/(2\mu)},
 \qquad \|x_i\|_{L^{2p}(\widetilde\mu_{R,P})}
          \le C\mu^{-1/2}\sqrt p.                   \tag{BC.37}
\]
The same coordinate moment reserve holds in the actual retained marginal.

Thus \(F_h=h^{-4}x_o^2\) has a fixed local incoming pointwise, continuous-current and actual averaged budget, uniformly in \(P,R\). Its unit divided difference is \(h^{-4}(2x_o+t)\). Subtracting its actual joint expectation changes only a fixed-size identity coefficient, by (BC.37), and leaves all high Walsh coefficients unchanged. Input and output engineering factors differ by only the fixed one-step factor \(L^4\), if the two scales are \(h,Lh\).

The conditional is smooth in retained variables at every finite cutoff. A version with finite summed continuous-current norm is locally Lipschitz: on a compact set the regulator is bounded, and summing its current envelopes gives the required finite coordinate Lipschitz bound. Agreement almost everywhere with the actual conditional on a positive-density neighborhood then forces agreement throughout that neighborhood. The finite set of sign-cube points cannot be changed by a null-set version while retaining the asserted current norm. Therefore the lower bound applies to every such version of this exact joint-law conditional.

This proves that neither a genuine incoming/outer moment reserve nor a generic retained bound \(|r_i|<P/2\) is sufficient to upgrade HC to uniform carrier volume for arbitrary fixed positive precisions.

## 9. The same obstruction for a local gradient energy

Choose the fixed neighboring integrated site \(i=(2,0,\ldots,0)\), present for every \(R\ge2\), and let
\[
 F^{\nabla}_{R,P}(r)=q_{R,P}^r[(z_o-z_i)^2].
                                                               \tag{BC.38}
\]
This is a nonnegative local gradient-energy root, with a fixed two-site input budget. Put
\[
 A_R=1-u_i\ge\delta,\qquad
 L_\sigma=\sum_j a_j[(G_R)_{ov_j}-(G_R)_{iv_j}]\sigma_j.
\]
The exact constrained minimizer in Lemma BC.1 satisfies
\[
 y_o^\sigma-y_i^\sigma
   =A_R+L_\sigma-A_R\epsilon_R(T_N)_+.              \tag{BC.39}
\]
Take the full even Walsh coefficient of its square. Constant, linear and quadratic polynomials in the signs vanish for \(N\ge4\). The term \((T_N)_+L_\sigma\) also vanishes: its part \(T_NL_\sigma/2\) has degree two, while \(|T_N|L_\sigma/2\) is odd under simultaneous reversal. The square \((T_N)_+^2=(T_N^2+T_N|T_N|)/2\) vanishes for the same two reasons. The remaining term gives exactly
\[
 \mathbb E_\sigma\!\left[
  \chi_N(y_o^\sigma-y_i^\sigma)^2\right]
 =-A_R^2\epsilon_R\,
        \mathbb E_\sigma[\chi_N|T_N|].              \tag{BC.40}
\]
Its magnitude is at least \(\delta^2\epsilon_R c_N\).

The product cutoff bounds each gradient by two in rescaled units. Equation (BC.24) therefore yields
\[
 \left|P^{-2}F^\nabla_{R,P}(r(\sigma))
       -(y_o^\sigma-y_i^\sigma)^2\right|
 \le \frac{4\sqrt{2n_R/\mu}}{P}.                    \tag{BC.41}
\]
Increasing the lower cutoff threshold in (BC.30) by a fixed factor depending only on \(\delta\) gives the same lower bound (BC.32), with changed fixed constants. The diagonal congruence of Section 8 leaves both integrated sites unchanged, so this corollary also holds in its genuine joint law with all retained values below \(P/2\).

A local gradient square is closer in form to a curvature quadratic, but it is still not an identification with the YM scalar. The proved statement remains an obstruction in the explicitly constructed scalar Gaussian comparison model.
