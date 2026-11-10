# The actual flat Maxwell lift gives a two-power quadratic gain

This note proves a smoothing estimate for the flat minimizing lift of
the literal Balaban averaging operation. Combined with WQ's quadratic
Ward projector and exact Gaussian vacuum subtraction, it gives an
\(L^{-2}\) bound on arbitrary coarse fields. The coarse fields need not
be band limited.

The theorem is about the actual linearized averaging constraint and
the untruncated Maxwell Gaussian, including the source's averaged
gauge fixing. It does not replace a nonlinear interacting step by a
Gaussian, and it does not identify moving hard Q domains with a
centered Gaussian domain. The final section also gives the exact
iterated flat statement, using the inherited Schur action rather than
resetting the coarse action to bare Wilson.

## 1. Source convention and energy normalization

Work first with fine spacing one in dimension four and odd integer
\(L\ge3\). The coarse spacing is \(L\). Each independent Lie-algebra
colour has the same calculation, so suppress colour and use its fixed
positive invariant inner product.

A fine one-cochain \(A_\mu(x)\) is the dimensionless angle on
\((x,x+e_\mu)\). Its curl is \(F=d_fA\), with one component for each
\(\mu<\nu\). Write

\[
 Q_W(A)=\frac12\sum_{x,\mu<\nu}|F_{\mu\nu}(x)|^2,\qquad
 \|\nabla_fF\|_2^2
   =\sum_{\lambda,x,\mu<\nu}
      |F_{\mu\nu}(x+e_\lambda)-F_{\mu\nu}(x)|^2 .
 \tag{FH.1}
\]

This is the same unit Maxwell normalization as WQ.11. Fixed trace or
colour constants can be restored on both sides without changing the
scale gain.

The averaging operation used here is the symmetric one in CMP109,
printed pp.252--254, (0.4)--(0.12). The source explicitly replaces its
earlier nonsymmetric contour convention. The linearization of the
full nonlinear contour mean is the mean of the contour integrals,
by (0.8). Consequently the literal derivative of (0.12) is

\[
 (Q_1A)_\mu(y)
  =L^{-4}\sum_{x\in B(y)}
       \sum_{r=0}^{L-1}A_\mu(x+r e_\mu)
       +\phi_y(A)-\phi_{y+Le_\mu}(A).
 \tag{FH.2}
\]

Here \(B(y)\) is the centered \(L^4\)-site block and \(\phi_y\) is the
average of its actual center-to-site contour integrals. Indeed, the
two endpoint terms in the derivative of (0.12) give these two
averages. The reference straight coarse transport in that equation
cancels from its linearization. Symmetrizing the contour family
changes \(\phi\), but not the first term of FH.2.

The last two terms in FH.2 are a coarse gradient. Taking the coarse
curl therefore gives the exact cochain identity

\[
 d_cQ_1=Q_2d_f,
 \tag{FH.3}
\]

where

\[
 (Q_2F)_{\mu\nu}(y)
  =L^{-4}\sum_{x\in B(y)}
        \sum_{r,s=0}^{L-1}
       F_{\mu\nu}(x+r e_\mu+s e_\nu).
 \tag{FH.4}
\]

The signs follow the chosen positive orientation. This is a block
average of the actual \(L\)-by-\(L\) plaquette sheet. In particular
constant fine curvature is sent to \(L^2F\), not to \(F\).

One can work on a fine periodic lattice with side \(LJ\), its coarse
quotient with side \(J\), and unitary discrete Fourier transforms.
All constants below are independent of \(J\). The infinite-lattice
statement follows by the same Fourier calculation and Plancherel.
The only zero-curvature harmonic modes are treated explicitly below.

## 2. Centered aliases and the exact-form projection

Locate a fine edge at \(x+e_\mu/2\), a fine plaquette at
\(x+(e_\mu+e_\nu)/2\), and the corresponding coarse objects at their
coarse geometric centers. Put

\[
 \widehat k_\lambda=2\sin(k_\lambda/2),\qquad
 S_L(t)=\sum_{r=-(L-1)/2}^{(L-1)/2}e^{irt}
       =\frac{\sin(Lt/2)}{\sin(t/2)},\qquad
 B_L(k)=L^{-4}\prod_{\lambda=1}^4S_L(k_\lambda).
 \tag{FH.5}
\]

The values at removable singularities are understood by continuity.
For a coarse momentum \(p\in[-\pi,\pi]^4\), its fine aliases are

\[
 k_n=\frac{p+2\pi n}{L},\qquad
 n_\lambda=-(L-1)/2,\ldots,(L-1)/2.
 \tag{FH.6}
\]

The sheet filter, before the centering signs, is diagonal:

\[
 q_{\mu\nu}(k)=B_L(k)S_L(k_\mu)S_L(k_\nu).
 \tag{FH.7}
\]

Let \(D_2(n)\) be diagonal on two-forms, with entry
\((-1)^{n_\mu+n_\nu}\) on \(\mu\nu\). Centering the coarse plaquette
introduces exactly this sign. In unitary finite-volume Fourier
coordinates, FH.4 becomes

\[
 \widehat f(p)=
   \sum_n L^{-2}D_2(n)\operatorname{diag}(q(k_n))
                              \widehat F(k_n).
 \tag{FH.8}
\]

The factor \(L^{-2}\) is the square root of the four-dimensional
volume ratio in the two unitary transforms. With nonunitary
infinite-volume transforms the alias factor is \(L^{-4}\);
setting \(u_n=L^{-2}\widehat F(k_n)\) gives the identical Hilbert-space
formula and energy below.

The signs cannot be omitted in the cochain identity, although they
drop out of the trace estimates. For example

\[
 \widehat p_\lambda
    =(-1)^{n_\lambda}S_L(k_{n,\lambda})\widehat k_{n,\lambda}.
 \tag{FH.9}
\]

For \(k\ne0\), let \(\mathcal E(k)\) be the space of exact two-forms
\(\widehat k\wedge a\), and let \(P_2(k)\) be its orthogonal projection.
It has rank three and

\[
 P_2(k)=|\widehat k|^{-2}
       (\widehat k\wedge)(\widehat k\mathbin{\lrcorner}),\qquad
 [P_2(k)]_{\mu\nu,\mu\nu}
       =\frac{\widehat k_\mu^2+\widehat k_\nu^2}
                    {|\widehat k|^2}.
 \tag{FH.10}
\]

At \(k=0\) the curvature of a periodic one-cochain is zero; set
\(\mathcal E(0)=\{0\}\). Let \(\mathcal G(p)=\mathcal E(p)\) on the
coarse lattice. Equations FH.3 and FH.9 show that every alias map
in FH.8 sends \(\mathcal E(k_n)\) into \(\mathcal G(p)\).

Define a map from the \(n\)-th exact-form space by

\[
 M_n(p)=L^{-2}D_2(n)\operatorname{diag}(q(k_n))
                      \big|_{\mathcal E(k_n)}.
 \tag{FH.11}
\]

Its two positive Gram sums on \(\mathcal G(p)\) are

\[
 \mathcal A(p)=\sum_nM_nM_n^*,\qquad
 \mathcal B(p)=\sum_n|\widehat k_n|^2M_nM_n^*.
 \tag{FH.12}
\]

The exact-form projection in \(M_nM_n^*\) is essential. Replacing it
by the identity would discard the Bianchi constraint and would not
give the sharp estimate below.

## 3. Uniform Gram bounds

### Lemma FH.1

For every \(p\ne0\), with \(c_0=(2/\pi)^6\),

\[
 c_0^2I_{\mathcal G(p)}
       \le\mathcal A(p)\le I_{\mathcal G(p)},\qquad
 0\le\mathcal B(p)
       \le 3L^{-2}|\widehat p|^2I_{\mathcal G(p)}
       \le 3c_0^{-2}L^{-2}|\widehat p|^2\mathcal A(p).
 \tag{FH.13}
\]

The constants are independent of \(L\), the volume and \(p\).

**Proof.** The one-dimensional alias identity is

\[
 \sum_{n=-(L-1)/2}^{(L-1)/2}
      |S_L((p+2\pi n)/L)|^2=L^2,\qquad
 \sum_n|S_L((p+2\pi n)/L)|^4\le L^4 .
 \tag{FH.14}
\]

For the first equality expand the two block sums. Summing the alias
phase annihilates every difference of block indices except zero.
There are \(L\) such diagonal terms and the alias sum contributes
\(L\). The second inequality follows from
\(\sum a_n^2\le(\sum a_n)^2\) for \(a_n\ge0\).

Since \(P_2\le I\), the full positive matrix \(\mathcal A\) is at most
the diagonal matrix with \(\mu\nu\) entry

\[
 L^{-4}\sum_n B_L(k_n)^2
                    S_L(k_{n,\mu})^2S_L(k_{n,\nu})^2
 \le L^{-12}L^4L^4L^2L^2=1.
 \tag{FH.15}
\]

This gives the upper bound. For the main alias \(n=0\),
\[
 2/\pi\le L^{-1}S_L(p_\lambda/L)\le1,\qquad
 (2/\pi)^4\le B_L(p/L)\le1.
 \tag{FH.16}
\]
Thus the diagonal map \(L^{-2}\operatorname{diag}(q(p/L))\)
has every singular value between \(c_0\) and one. Its restriction
to \(\mathcal E(p/L)\) maps into \(\mathcal G(p)\) and is injective.
Both spaces have dimension three, so it is onto and its restricted
singular values have the same lower bound. The main-alias Gram
alone is at least \(c_0^2I_{\mathcal G(p)}\).

For the weighted estimate use the diagonal in FH.10 before summing:

\[
 \operatorname{Tr}\mathcal B
 =L^{-4}\sum_nB_L(k_n)^2
   \sum_{\mu<\nu}S_\mu^2S_\nu^2
                     (\widehat k_{n,\mu}^2+\widehat k_{n,\nu}^2).
 \tag{FH.17}
\]

Here \(S_\lambda=S_L(k_{n,\lambda})\). Equation FH.9 gives
\(S_\mu^2\widehat k_{n,\mu}^2=\widehat p_\mu^2\).
After this cancellation, the \(\mu\)-term for a fixed pair is at most

\[
 L^{-12}\widehat p_\mu^2
   \left(\sum S_\mu^2\right)
   \left(\sum S_\nu^4\right)
   \prod_{\lambda\ne\mu,\nu}\left(\sum S_\lambda^2\right)
 \le L^{-2}\widehat p_\mu^2 .
 \tag{FH.18}
\]

Each coordinate occurs in three pairs. Therefore
\(\operatorname{Tr}\mathcal B\le3L^{-2}|\widehat p|^2\).
The matrix is positive and supported on \(\mathcal G(p)\), so its
operator bound follows from its trace. The lower bound for
\(\mathcal A\) proves the final inequality. \(\square\)

## 4. The literal constrained Maxwell minimum

Let \(H_La\) be the minimizing fine one-cochain for the Maxwell action
under the actual condition \(Q_1A=a\), in the source averaged gauge.
Only its curvature is needed here.

First this is exactly the curvature minimization described by FH.8.
Any fine curvature satisfying \(Q_2F=d_ca\) comes from a fine
one-cochain in the exact-form spaces above. The mismatch
\(Q_1A-a\) is coarse closed. On a finite torus it is a coarse gradient
plus a constant harmonic one-cochain. A fine gauge with the desired
values at the coarse centers corrects the gradient, by the endpoint
covariance of the literal average. A constant fine one-cochain
corrects the harmonic part: \(Q_1\) sends a constant angle \(h\) to
\(Lh\). Both corrections have zero curl.

The source soft gauge does not alter this curvature minimization.
At the identity, its full averaged contour has linear sampler
\(\tau\), and
\(\tau(A+d\omega)(y,x)=\tau A(y,x)+\omega(x)-\omega(y)\),
up to the common orientation convention. A center-fixed gauge
\(\omega(y)=0\) can set every sampler entry to zero, without changing
the coarse constraint or curvature. Thus the minimum of the
Maxwell form plus the positive averaged soft quadratic has precisely
the same curvature as the physical Maxwell minimum. This uses the
actual full sampler in CMP109 (0.11), (0.14), (2.2)--(2.5), not an
unrelated gauge term. The exceptional-coordinate embedding is just
a parametrization of the same constraint.

For \(f=\widehat{d_ca}(p)\), the minimizing exact-form array is

\[
 u_{H,n}=M_n^*\mathcal A^{-1}f,\qquad
 E_H(p):=\sum_n|u_{H,n}|^2
                 =f^*\mathcal A^{-1}f.
 \tag{FH.19}
\]

The harmonic component at \(p=0\) has a zero-curvature lift and
contributes no energy. Lemma FH.1 gives

\[
 |f|^2\le E_H(p)\le c_0^{-2}|f|^2,
 \tag{FH.20}
\]

and

\[
 \begin{split}
 E_{\nabla H}(p)
  &:=\sum_n|\widehat k_n|^2|u_{H,n}|^2\\
  &=f^*\mathcal A^{-1}\mathcal B\mathcal A^{-1}f\\
  &\le3c_0^{-2}L^{-2}|\widehat p|^2E_H(p).
 \end{split}
 \tag{FH.21}
\]

Consequently, with numerical constants depending only on dimension,

\[
 Q_{W,c}(a)\le Q_W(H_La)\le c_0^{-2}Q_{W,c}(a),\qquad
 \boxed{\ \|\nabla_fd_fH_La\|_2^2
             \le C L^{-2}\|d_fH_La\|_2^2.\ }
 \tag{FH.22}
\]

There is the stronger momentumwise factor
\(|\widehat p|^2\) in FH.21. The second inequality in FH.22 used only
\(|\widehat p|^2\le16\); it therefore applies to every coarse field,
including coarse lattice-scale oscillations.

This is a proof of the smoothing estimate for the actual minimizing
lift. Numerical attenuation of coarse plaquettes alone would not
have proved it.

## 5. The Ward remainder on arbitrary fine fields

Let \(K\) satisfy the infinite-lattice hypotheses of WQ: exponential
locality, self-adjointness, exact gauge invariance, colour invariance,
translation invariance and full hypercubic symmetry in centered-edge
coordinates. Let
\[
 R=K-c_KK_W
 \tag{FH.23}
\]
be its actual quadratic Ward remainder.

The WQ fourth-order Taylor estimate can be taken on the whole real
Brillouin zone. All derivatives up to degree three at zero vanish
after the subtraction. Integrating the bounded fourth derivative
along the segment from zero to \(k\) gives
\(\|\mathscr R(k)\|\le C_\rho\|K\|_\rho|k|^4\).
For \(k\in[-\pi,\pi]^4\),
\(|k|\le(\pi/2)|\widehat k|\). The exact Ward identity makes
\(\mathscr R\) act only on the subspace perpendicular to
\(\widehat k\). Hence, for every fine vector \(v\),

\[
 |v^*\mathscr R(k)v|
  \le C_\rho\|K\|_\rho|\widehat k|^2
                    |\widehat k\wedge v|^2 .
 \tag{FH.24}
\]

Unlike WQ's band-limited corollary, this statement has no support
restriction on \(v(k)\). Its right side is an extra-derivative energy.
Integrating FH.24 and using FH.21 gives

\[
 \boxed{\quad
 |Q_R(H_La)|
     \le C_\rho\|K\|_\rho L^{-2}Q_W(H_La)
     \le C_\rho'\|K\|_\rho L^{-2}Q_{W,c}(a).
 \quad}
 \tag{FH.25}
\]

No positivity of \(R\) is assumed. More precisely, let
\(K_{\mathrm{eff}}(p)=d_c(p)^*\mathcal A(p)^{-1}d_c(p)\), and let
\(R_{\mathrm{out}}\) be the coarse quadratic form obtained by
substitution of the minimizing lift. Then

\[
 |v^*R_{\mathrm{out}}(p)v|
 \le C_\rho\|K\|_\rho L^{-2}|\widehat p|^2
                        v^*K_{\mathrm{eff}}(p)v
 \le C_\rho'\|K\|_\rho L^{-2}|\widehat p|^2
                        v^*K_W(p)v.
 \tag{FH.25a}
\]

It therefore has no newly generated quadratic marginal term at
\(p=0\). This is an energy/Taylor statement; no additional
exponential spatial kernel theorem for the minimizing lift is
inferred just from FH.25a.

For a finite torus, take the compatible periodization of this
infinite-lattice \(R\) when applying FH.24. The separate finite-volume
winding difference in SW is not silently included in the Ward
remainder. In particular a Wilson-relative estimate for an arbitrary
torus holonomy contribution is not asserted.

## 6. Exact Gaussian integration and vacuum extraction

For this section work on a finite compatible periodic lattice, so
that every determinant, rank and trace in the displayed identities is
finite. Consider the actual flat source Gaussian, with the constraint
\(Q_1A=a\), the complete averaged soft-gauge quadratic, and the
source independent-coordinate embedding \(C\). Its conditional
normal form is

\[
 A=H_La+Cz,\qquad
 \mu(dz)=
    \frac{\det(K_{\mathrm f})^{1/2}}{(2\pi)^{D/2}}
       e^{-\frac12 z^TK_{\mathrm f}z}\,dz .
 \tag{FH.26}
\]

Here \(K_{\mathrm f}=C^*(d_f^*d_f+c_{\mathrm{gf}}\tau^*\tau)C\)
on the actual free list. Its positive gap at fixed \(L\) follows
from the source flat constraint/gauge estimate, or the fixed-block
Poincare decomposition used in AP/IG. The linear coarea and the
normalized gauge insertion have constants independent of \(a\);
they are retained in the unnormalized coarse density and cancel
in this exact conditional probability. The determinant in FH.26
is that of the same precision as its inverse.

The covariance in the full fine one-cochain space is
\(\Gamma_{\mathrm f}=CK_{\mathrm f}^{-1}C^*\). Centering and the
quadratic identity give, without any estimate,

\[
 \mathbb E_{\mu_a}Q_R(A)
     =Q_R(H_La)+\frac12\operatorname{Tr}(R\Gamma_{\mathrm f}).
 \tag{FH.27}
\]

The trace is the exact vacuum contribution. Define the
vacuum-subtracted linearized Gaussian RG insertion by

\[
 (\mathcal R_L^{\rm quad}Q_R)(a)
  :=\mathbb E_{\mu_a}Q_R(A)-\mathbb E_{\mu_0}Q_R(A).
 \tag{FH.28}
\]

Then

\[
 (\mathcal R_L^{\rm quad}Q_R)(a)=Q_R(H_La),\qquad
 |(\mathcal R_L^{\rm quad}Q_R)(a)|
  \le C_\rho'\|K\|_\rho L^{-2}Q_{W,c}(a).
 \tag{FH.29}
\]

Equivalently, FH.28 is the field-dependent derivative at zero of
the Gaussian effective action after adding the quadratic insertion
to the fine action. The trace subtraction is not replaced by a
finite-pulse identity coefficient.

An infinite-lattice or density statement is taken only after this
finite-volume subtraction. Its field-dependent limit is the
curvature-energy expression \(Q_R(H_La)\), with the uniform bound
FH.29. There is no subtraction of two independently infinite total
vacuum traces.

Restoring fine spacing \(h\) and coarse spacing \(H=Lh\) changes the
scale factor to \((h/H)^2\). If fine normalized fluctuations have
physical angle \(g_{\rm f}z\) and the coarse normalized angle is
\(g_{\rm c}a\), the fine conditional mean in those normalized units
is \((g_{\rm c}/g_{\rm f})H_La\). Thus FH.29 has the explicit factor
\((g_{\rm c}/g_{\rm f})^2\) when the insertion is measured in the
fine normalized coordinates. In the common convention
\(\beta_i=(Ng_i^2)^{-1}\), this is
\(\beta_{\rm f}/\beta_{\rm c}\). No coupling-flow identity or equality
of these couplings is assumed.

## 7. Exact iteration inside the flat Gaussian model

The gain can be iterated without multiplying the estimate's constant
at each stage, provided one keeps the original Gaussian and its exact
inherited Schur action.

For \(q\) literal averaging steps put \(M=L^q\). The curvature filters
compose exactly because

\[
 \prod_{r=0}^{q-1}S_L(L^rt)=S_M(t),\qquad
 \prod_{r=0}^{q-1}B_L(L^rk)=B_M(k).
 \tag{FH.30}
\]

These are identities of finite trigonometric sums, including their
removable zeros. Cochain identity FH.3 at each stage then shows that
the curvature of the total readout has precisely the filter FH.7
with \(L\) replaced by \(M\). Differences in the intermediate
contour-gradient terms do not change the curvature constraint.
The same final gradient/harmonic repair proves equivalence with
the actual iterated one-cochain constraint.

Applying the alias calculation once at scale \(M\) therefore gives

\[
 \|\nabla_fd_fH_{Q^{q}}a\|_2^2
       \le C L^{-2q}\|d_fH_{Q^{q}}a\|_2^2,\qquad
 Q_W(H_{Q^{q}}a)\le c_0^{-2}Q_{W,\mathrm{final}}(a).
 \tag{FH.31}
\]

On each finite compatible lattice, successive Gaussian integrations
are exact Schur elimination of the same joint quadratic form. Their
total conditional mean is \(H_{Q^{q}}a\); their conditional covariance
contributes one finite total vacuum trace to a quadratic insertion.
Subtract this trace before passing to any anchored, density or
infinite-volume limit. The intermediate normalized
averaged-gauge samplers may be retained: a center-fixed gauge at
one level sets that sampler to zero, and its block-constant lifts
preserve the already fixed finer sampler. Equivalently, their
normalized gauge integrations do not change the physical Gaussian
quotient. They select representatives and normalization constants,
not a different curvature minimizer.

After subtracting that total vacuum trace, the bound is

\[
 |\mathcal R_{Q^{q}}^{\rm quad}Q_R(a)|
   \le C_\rho'\|K\|_\rho L^{-2q}
                         Q_{W,\mathrm{final}}(a).
 \tag{FH.32}
\]

In normalized physical-angle variables retain the additional
\((g_{\rm final}/g_{\rm initial})^2\) from Section 6.
There is one constant in FH.32, not \(C^q\).

This is a uniform-depth fact about the exact flat untruncated
Gaussian model. It does not use the false operation of replacing
each inherited precision by a bare Wilson precision, and it does
not assert a uniform nonlinear or hard-cutoff induction.

## 8. An insertion already on an inherited Gaussian lattice

There is an additional distinction when the insertion is itself on
a lattice reached after \(b\) earlier Gaussian integrations. Its
incoming classical Gaussian action is the inherited Maxwell Schur
action. It is not bare nearest-neighbor Maxwell.

Factor out the single original Wilson coefficient, and let
\(C_b(k)\) denote the resulting curvature covariance shape on the
level-\(b\) lattice. On \(\mathcal E(k)\) the inherited action is
\(\frac12\langle f,C_b(k)^{-1}f\rangle\).
For \(b=0\), \(C_0=P_2\). For \(b>0\), exact elimination and FH.30
identify \(C_b\) with the Gram matrix FH.12 for total block size
\(L^b\). Thus FH.13 gives, uniformly in \(b\),

\[
 c_0^2P_2(k)\le C_b(k)\le P_2(k).
 \tag{FH.33}
\]

At zero momentum the exact curvature space is zero and harmonic
one-cochains are handled as before. A common positive scalar
coefficient in the physical inherited action multiplies its
precision and divides its covariance; it cancels from the
conditional mean. FH.33 concerns this covariance shape, not a
covariance from which a running coupling was silently omitted.

Make \(q\) further actual blockings, with \(M=L^q\), and let \(M_n\)
now be the alias maps FH.11 with block size \(M\) in the
level-\(b\) units. Define

\[
 A_{b,M}(p)=\sum_nM_nC_b(k_n)M_n^*,\qquad
 D_{b,M}(p)=\sum_n|\widehat k_n|^2
                       M_nC_b(k_n)^2M_n^* .
 \tag{FH.34}
\]

The exact inherited Gaussian mean curvature and its incoming
inherited energy are

\[
 u_{H,n}=C_b(k_n)M_n^*A_{b,M}^{-1}f,\qquad
 E_{b,M}(p)
   =\sum_n u_{H,n}^*C_b(k_n)^{-1}u_{H,n}
   =f^*A_{b,M}^{-1}f .
 \tag{FH.35}
\]

All inverses in these formulas are on the exact-form spaces.
Equations FH.13 and FH.33 give

\[
 c_0^4I_{\mathcal G}\le A_{b,M}\le I_{\mathcal G},\qquad
 D_{b,M}\le\mathcal B_{\mathrm{bare},M}
               \le3M^{-2}|\widehat p|^2I_{\mathcal G}.
 \tag{FH.36}
\]

The second inequality follows from \(C_b^2\le P_2\). It would not
follow from an unproved replacement of \(C_b\) by an identity
matrix in the actual incoming action. Consequently

\[
 \begin{split}
 \sum_n|\widehat k_n|^2|u_{H,n}|^2
   &\le3c_0^{-4}M^{-2}|\widehat p|^2E_{b,M}(p),\\
 E_{b,M}(p)&\le c_0^{-4}|f|^2.
 \end{split}
 \tag{FH.37}
\]

Apply FH.24 to a WQ remainder on the level-\(b\) lattice, and use
the finite-volume Gaussian identity FH.27 with this actual
inherited conditional. After its exact vacuum subtraction,

\[
 |v^*R_{\mathrm{out}}(p)v|
  \le C_\rho\|K\|_\rho M^{-2}|\widehat p|^2
                          v^*K_W(p)v .
 \tag{FH.38}
\]

The constant is independent of both \(b\) and \(q\). In normalized
angle variables FH.38 has the explicit multiplier
\((g_{b+q}/g_b)^2\). The same zero quadratic marginal conclusion
holds. Exact successive Schur elimination also identifies
\(A_{b,M}\) with the total inherited covariance shape
\(C_{b+q}\); the weaker direct lower bound in FH.36 was already
enough for this proof.

This establishes the gain for an insertion already sitting on an
inherited flat Gaussian background. It includes neither radiative
analytic interactions nor cutoff corrections in the incoming
precision. They belong to the nonlinear comparison problem.

## 9. Application and remaining boundary of the result

The quadratic kernel constructed in SW is one actual infinite-lattice
smooth, spatially summed marked Hessian to which WQ and hence the
present flat transfer apply. For that kernel's level-three
application, use the inherited-input construction in Section 8:
its classical Gaussian backbone is the inherited Schur action.
The correct order is: construct the kernel; remove its Ward
marginal coefficient; transport its quadratic remainder through
that flat classical Gaussian conditional; and remove the exact
finite-volume Gaussian vacuum trace. This is not an identification
of the full smooth interacting law with that Gaussian backbone.

The new estimate fills the minimizing-lift/smoothing gap in applying
the quadratic low-momentum gain to arbitrary coarse fields at the
Gaussian level. It leaves the following distinct tasks open:

* comparison of the nonlinear constrained reconstruction and
  interacting conditional law with this quadratic transfer, in the
  required marked energy/current norm;
* local-source-position moments and the corresponding nonlinear Ward
  matching, as opposed to the integrated zero-source-momentum kernel;
* the full physical-carrier and separated-origin current bookkeeping
  for that nonlinear remainder;
* preservation of the old real cutoff-core certificates and all
  relevant/vacuum budgets at arbitrary depth.

No hard P/Q cutoff claim, moving-domain claim, or Yang--Mills existence
claim is made by FH.29, FH.32 or FH.38.

Primary source input: Balaban, CMP109 (1987), printed pp.252--255,
(0.4)--(0.16), for the actual symmetric average and normalized averaged
gauge insertion; printed pp.265--269, (2.2)--(2.18), for its
constraint/free-coordinate Gaussian normal form and covariance.
The literal averaging formula is (0.12) on CMP 109, p. 254.
The Ward projector and its exponential-kernel assumptions are in
[M04 Quadratic Ward Projector and Low Momentum Gain](../D_native_nonlinear/M04_Quadratic_Ward_Projector_and_Low_Momentum_Gain.md).
FH.3--FH.38 are derived here from that source map and elementary
finite-dimensional/Fourier identities.
