# Complete conditional-law criteria and exact scalar integration by parts

**Annex AB.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 0. Disposition and new results

**C-08 and M-04 remain open.** The complete current-coordinate activity and background-derivative budgets have not been established for every admitted history. A new calculation of the homogeneous no-R law, or an abstract criterion which assumes those budgets, would not pass their stated mathematical requirements.

This annex gives three concrete results. None of them is a completed statement for the actual model.

1. It gives a local, volume-independent conditional-mean criterion which retains the exact exterior Schur force and the first derivative of the complete interaction. This specifies the mean input which is absent from a coercivity inequality alone.
2. It proves an exact scalar quadratic readout for the **actual incoming mark** under the full regular conditional law. The identity isolates a constrained trace term and retains the exterior mean, all inherited E/R/B and measure gradients, and the incoming Taylor remainder. A compactly supported integration-by-parts field replaces the hard-boundary flux by an explicit ordinary expectation on coordinate collars. No coupling derivative or source-dependent minimizer is used.
3. It gives a local rare-collar bound and the exact first and second retained-parameter response formulas. These formulas expose the additional costs needed for the M-03 current norm and for the scalar marginal coefficient.

The new exact identities apply at finite cutoff whenever their displayed integrals exist. Their quantitative consequences retain explicit hypotheses. They do not turn an unspecified transported mark into a freshly inserted native coarse plaquette, or prove a summable multiscale matching error.

### 1. The actual regular law and the actual incoming mark

#### 1.1 Source support and the change of conditioning

The primary formulas used here are CMP119, printed pp.267-270, (3.15)-(3.25). The source first eliminates the exceptional variables of the linearized averaging constraint; the constrained quadratic form subsequently appears as \(C^*\Delta^{(k)}C\). It then inserts the free-bond partition (3.16). On the regular interior the old approximate-fluctuation selector is exactly one. Formula (3.25) displays only the product good-field cutoff in the inner integral. The boundary relocation is retained in the exponent.

The support calculation in Annex AA checks the complete R return to that inductive form. Its result concerns the **source-normal-form regular marginal**, not a finer conditional law obtained by fixing every archived selector label. Let \(v\) contain the live geometry and all exterior variables retained by that normal form. Write its free variables as \(z=(z_i)_{i\in I}\), with bounded-dimensional real Lie-algebra blocks. The inner domain is

\[
 D=\prod_{i\in I}D_i,\qquad D_i=P_iD_i^0,
 \tag{CM.1}
\]

where each \(D_i^0\) is the fixed symmetric convex bond-norm unit ball. The radii \(P_i\) are the actual source radii in these coordinates. They are fixed while the retained field values vary within one admitted live-geometry chart. No alternative radius convention is substituted.

Let \(F^{\rm aug}\) be the incoming scalar mark on the positive augmented construction, and let \(\omega\) denote the variables already integrated out in obtaining this marginal. The mark to be inserted in the regular integral is

\[
 F(z;v)=\mathbb E[F^{\rm aug}\mid z,v].
 \tag{CM.2}
\]

For a full finite source jet, (CM.2) is applied to every coefficient of the **whole** jet. Its logarithm retains the resulting conditional cumulants. The identity

\[
 \mathbb E[F^{\rm aug}f(z,v)]
 =\mathbb E[F(z;v)f(z,v)]
 \tag{CM.3}
\]

holds for every bounded retained test \(f\). This justifies using the regular marginal, but gives no pointwise or Sobolev identification of \(F\) with a native field. In particular, a smooth marginal density need not make every projected mark smooth. Regularity and localization of (CM.2) remain part of the marked induction.

#### 1.2 Complete potential and exterior force

Split the true constrained quadratic form into interior and retained current coordinates. In the notation of C-01, let \(y\) be the retained exterior current field and put

\[
 K=K_{\Lambda\Lambda},\qquad
 b=-K_{\Lambda\Lambda^c}y,\qquad C=K^{-1}.
 \tag{CM.4}
\]

At fixed retained data, the complete regular conditional law is

\[
 d\nu_v(z)=Z_v^{-1}\mathbf1_D(z)
 \exp\left[-\frac12 z^TKz+b^Tz+W(z;v)\right]dz.
 \tag{CM.5}
\]

Here \(W\), up to a retained-data-only constant, contains precisely

\[
 \begin{split}
 W={}&-\mathscr V+\log J+\Delta\mathbf E
       +\Delta\mathbf R+\Delta\mathbf B\\
     &-\Delta A(w_k-g_k^{-2},\cdot)
       +\mathscr B_{\partial},
 \end{split}
 \tag{CM.6}
\]

evaluated on the actual interior/exterior coordinate map. Any older operation factor which depends on this free variable in the chosen exact representation also belongs in \(W\). The quadratic exterior constant belongs in the outer weight; its linear cross term is \(b^Tz\) and remains in (CM.5). The same convention is used for the fixed Haar/constraint prefactor: it cancels from this conditional ratio but remains in the outer marginal and history law.

The estimates below never assert that \(W\) or its derivatives are small merely because it has been written in the form (CM.6).

### 2. A local mean criterion with the exterior force retained

#### 2.1 Quantitative hypotheses

Let the block metric obey

\[
 S_a:=\sup_i\sum_j e^{-a d(i,j)}<\infty
 \quad(a>0),
 \tag{CM.7}
\]

with the desired volume-independent constants. For \(0\le s\le1\), let

\[
 d\nu_s=Z_s^{-1}\mathbf1_D
 e^{-\frac12z^TKz+b^Tz+sW(z)}dz.
 \tag{CM.8}
\]

Assume the complete potentials on this **same** product domain, including their real linear tilts, have the uniform coercivity and weighted covariance estimate

\[
 |\operatorname{Cov}_{\nu_s}(z_i,f)|
 \le\sum_j G_{ij}\|\nabla_jf\|_{L^2(\nu_s)},
 \qquad G_{ij}=c_*e^{-\gamma d(i,j)}.
 \tag{CM.9}
\]

The norm on the left is the Euclidean norm of the block covariance. For the arbitrary-mark cumulant and retained-current consequences below, retain explicitly the stronger bilinear estimate

\[
 |\operatorname{Cov}_{\nu_s}(f,g)|
 \le\sum_{i,j}G_{ij}
       \|\nabla_i f\|_{L^2(\nu_s)}
       \|\nabla_j g\|_{L^2(\nu_s)}.
 \tag{CM.9a}
\]

It is required for the relevant weighted Sobolev functions and the same real linear tilts. The mean proof uses (CM.9); the coordinate estimate alone is not asserted to imply (CM.9a).

Assume also that every real linear tilt of these measures has Hessian at least \(\lambda I\), with the same convex support. These conclusions follow from the existing weighted Neumann/convex-domain argument when the **actual** constrained precision has its admitted gap and weighted conjugation bound and the complete \(W\) Hessian fits inside the corresponding numerical margin. C-04-C-06 must supply that application; (CM.9)-(CM.9a) are not asserted without it.

Define the nonnegative matrix and local zero-field force

\[
 A_{ij}=\sup_{z\in D}\|\nabla_i\nabla_jW(z)\|,
 \qquad d_i=|\nabla_iW(0)|.
 \tag{CM.10}
\]

Use the weighted positive-kernel row norm

\[
 \|T\|_a=\sup_i\sum_j e^{a d(i,j)}T_{ij}.
 \tag{CM.11}
\]

For one fixed \(0<a<\gamma\), require

\[
 \|GA\|_a<1.
 \tag{CM.12}
\]

This is an explicit additional smallness condition, not a hidden use of an unweighted value bound. A sufficient condition is
\(c_*S_{\gamma-a}\|A\|_a<1\).

#### Theorem CM.1 -- force-resolvent mean and moment bounds

Under (CM.7)-(CM.12), let

\[
 H=(I-GA)^{-1}G,
 \qquad
 \sigma=\sqrt{d_{\max}/\lambda},
 \tag{CM.13}
\]

where \(d_{\max}\) is the largest real block dimension. Then

\[
 \sup_{0\le s\le1}|\nu_s z_i|
 \le\sum_j H_{ij}
 \left(|b_j|+d_j+\sigma\sum_lA_{jl}\right).
 \tag{CM.14}
\]

Moreover, for every \(p\ge1\),

\[
 \|z_i-\nu_s z_i\|_{L^p(\nu_s)}
 \le C\sqrt{p/\lambda},
 \tag{CM.15}
\]

with \(C\) depending only on the bounded block dimension. Finally,

\[
 \|H\|_a\le
 \frac{c_*S_{\gamma-a}}{1-\|GA\|_a}.
 \tag{CM.16}
\]

Thus the local mean is controlled by a spatially decaying convolution of the **actual exterior force and actual interaction gradient**, not by setting the retained Gaussian mean to zero.

**Proof.** A linear tilt leaves the Hessian unchanged. Applying the convex-domain variance bound to that tilted measure gives, for a unit vector \(u\) in one block,

\[
 \frac{d^2}{dt^2}\log\nu_s e^{t u\cdot z_i}
 =\operatorname{Var}_{\nu_{s,t}}(u\cdot z_i)
 \le\lambda^{-1}.
 \tag{CM.17}
\]

Integrate twice and subtract the mean. The usual exponential Markov inequality gives a sub-Gaussian tail for each real block component. Integrating that tail and summing over at most \(d_{\max}\) components proves (CM.15). In particular its \(L^2\) block fluctuation is at most \(\sigma\).

At \(s=0,b=0\), the symmetric product domain and even quadratic density give zero mean. Interpolate the linear force from zero to \(b\), and apply (CM.9), which has the same constants under this linear tilt. The resulting Gaussian reference mean satisfies

\[
 |\nu_0 z_i|\le\sum_jG_{ij}|b_j|.
 \tag{CM.18}
\]

The line segment from zero to \(z\) lies in \(D\). Taylor's integral formula therefore yields

\[
 |\nabla_jW(z)|\le d_j+\sum_lA_{jl}|z_l|.
 \tag{CM.19}
\]

Let \(M_i=\sup_{0\le s\le1}|\nu_s z_i|\). Differentiation in \(s\), the exact normalized covariance identity, (CM.9), (CM.15), and (CM.19) give

\[
 M\le G|b|+Gd+GA(M+\sigma\mathbf1).
 \tag{CM.20}
\]

All objects at finite cutoff have finitely many blocks. By (CM.12) the positive Neumann series for \((I-GA)^{-1}\) converges, proving (CM.14). The weighted row norm is submultiplicative by the triangle inequality for the metric. Since \(\|G\|_a\le c_*S_{\gamma-a}\), the same series gives (CM.16). No determinant ratio or total-volume factor appears. \(\square\)

#### 2.2 Consequence for local quadratic field budgets

Let \(x\) be an insertion anchor. Suppose a native mark, or an actual transported mark for which this has been proved, obeys

\[
 |O_x(z)|\le C h^{-4}
 \left(B_x+\sum_i e^{-\gamma_1d(x,i)}|z_i|\right)^2,
 \tag{CM.21}
\]

\[
 |\nabla_jO_x(z)|\le C h^{-4}e^{-\gamma_1d(x,j)}
 \left(B_x+\sum_i e^{-\gamma_1d(x,i)}|z_i|\right).
 \tag{CM.22}
\]

Write \(M_i\) for the right side of (CM.14), and put

\[
 \mathcal B_x=1+B_x+
       \sum_i e^{-\gamma_1d(x,i)}M_i.
 \tag{CM.23}
\]

Minkowski's inequality and Theorem CM.1 give

\[
 \|O_x\|_p\le Ch^{-4}(\mathcal B_x+\sqrt p)^2,
 \qquad
 \|\nabla_jO_x\|_p\le
 Ch^{-4}e^{-\gamma_1d(x,j)}(\mathcal B_x+\sqrt p).
 \tag{CM.24}
\]

Inserting these bounds into the existing real cut-cumulant theorem gives a fixed factorial bound of the form

\[
 |\kappa_m(O_{x_1},\ldots,O_{x_m})|
 \le C^m(m!)^2h^{-4m}
       \prod_{r=1}^m\mathcal B_{x_r}^{2}
       \exp\left[-\frac{c\tau(x_1,\ldots,x_m)}{m-1}\right],
 \qquad m\ge2,
 \tag{CM.25}
\]

with the same conditional scope. The constants in (CM.24)-(CM.25) depend on the fixed lower bound \(\lambda\), the fixed covariance constants \(c_*,\gamma\), the localization rate \(\gamma_1\), the geometric sums (CM.7), the fixed block dimensions, and the constants in (CM.21)-(CM.22). They are uniform in volume, source order and the cutoff only when those inputs and the force-resolvent margin are uniform; no uniformity as \(\lambda\) tends to zero is claimed.

One can check the factorial growth directly: apply the covariance bound to the two products across a longest-edge cut of a minimal spanning tree; use Holder with moment order at most \(2m\); and sum the cumulant partition coefficients. Each undifferentiated quadratic mark costs at most \(Cm\mathcal B_x^2\), each differentiated mark at most \(C\sqrt m\mathcal B_x\). The fixed polynomial factors in \(m\), the partition sum, and \(m^m\le e^m m!\) fit in \(C^m(m!)^2\). The longest-edge cut provides the displayed order-dependent range. This is the same cumulant mechanism already proved in the collection; the new point is the explicit nonzero-force budget (CM.14).

Neither (CM.24) nor (CM.25) bounds \(\mathcal B_x\) in the outer retained/history law. That is H-05 and the relevant part of H-04. Nor does the native-field bound (CM.21) automatically hold for the projected mark (CM.2).

### 3. Exact scalar readout without a coupling derivative

#### 3.1 A quadratic readout of the actual incoming function

At a fixed retained datum, choose a quadratic readout of the actual function \(F\) in (CM.2):

\[
 F(z)=a+\ell^Tz+\frac12z^TVz+T(z),
 \qquad V=V^T.
 \tag{CM.26}
\]

When a common differentiable chart has been proved, one may use its Taylor coefficients at zero. Otherwise (CM.26) simply defines the exact residual \(T\) for the chosen quadratic readout. Its mere existence proves no smallness. In particular, an arbitrary measurable transported mark is not declared analytic by this notation.

Set

\[
 B=CV,\qquad
 \Psi(z)=\frac12z^TKz-b^Tz-W(z).
 \tag{CM.27}
\]

For each block choose a fixed smooth cutoff \(0\le\chi_i\le1\), equal to one on \(\tfrac12D_i\), with support in \(\tfrac34D_i\), and

\[
 |\nabla\chi_i|\le c_\chi/P_i.
 \tag{CM.28}
\]

Fixed-dimensional norm equivalence and mollification supply these cutoffs for the actual bond-norm balls. They do not change the probability law. Their sole purpose is to make the integration-by-parts vector field vanish at its coordinate boundary.

Define the explicit collar expectation

\[
 \begin{split}
 \mathcal E_\chi(B)
 =\nu_v\sum_i\big[&
 (\chi_i-1)\operatorname{tr}B_{ii}
 +\nabla\chi_i\cdot(Bz)_i\\
 &+(1-\chi_i)(Bz)_i\cdot\nabla_i\Psi(z)\big].
 \end{split}
 \tag{CM.29}
\]

Every summand is supported in the coordinate collar
\(E_i=\{z_i\notin\tfrac12D_i\}\). Unlike a surface trace, (CM.29) is an expectation in the actual normalized law.

#### Theorem CM.2 -- exact selected-law virial readout

Assume the integrals in the following formula are absolutely finite. Then

\[
 \boxed{
 \begin{aligned}
 \nu_vF={}&a+\ell^T\nu_vz
 +\frac12\operatorname{Tr}(CV)\\
 &+\frac12\nu_v[(CVz)\cdot(b+\nabla W)]
 +\frac12\mathcal E_\chi(CV)+\nu_vT.
 \end{aligned}}
 \tag{CM.30}
\]

At every finite source regular fiber this applies to the actual incoming mark and chosen readout whenever the displayed derivative and integrability conditions hold. It uses the full \(W\) in (CM.6), not a Gaussian replacement of the density.

**Proof.** The vector field with block components
\(X_i(z)=\chi_i(z_i)(Bz)_i\) vanishes near the boundary of its own integration block. Integration by parts in that block, followed by Fubini, gives

\[
 0=\nu_v\sum_i
 \left[\chi_i\operatorname{tr}B_{ii}
 +\nabla\chi_i\cdot(Bz)_i
 -\chi_i(Bz)_i\cdot\nabla_i\Psi\right].
 \tag{CM.31}
\]

No assertion that the sharp cutoff has zero derivative is used. Rearrange (CM.31), add the complementary \(1-\chi_i\) terms, and use
\(\nabla\Psi=Kz-b-\nabla W\). Because \(K\) and \(V\) are symmetric,

\[
 (CVz)\cdot Kz=z^TVz.
 \tag{CM.32}
\]

The result is

\[
 \nu_v(z^TVz)=\operatorname{Tr}(CV)
 +\nu_v[(CVz)\cdot(b+\nabla W)]
 +\mathcal E_\chi(CV).
 \tag{CM.33}
\]

Insert (CM.26). This proves (CM.30). \(\square\)

#### 3.2 Checks and interpretation

For an untruncated Gaussian with \(W=0\), the collar term is absent and \(m=Cb\). Formula (CM.30) becomes

\[
 \nu F=a+\ell^Tm+\tfrac12\operatorname{Tr}(CV)
       +\tfrac12m^TVm+\nu T,
 \tag{CM.34}
\]

the exact Gaussian expectation. Thus the retained mean is not hidden in the determinant term.

For a standard one-dimensional Gaussian truncated to \((-P,P)\), \(b=W=0\) and \(V=K=1\), (CM.33) gives

\[
 \mathcal E_\chi(1)
 =\nu(z^2)-1
 =-\frac{2P\varphi(P)}{2\Phi(P)-1},
 \tag{CM.35}
\]

where \(\varphi,\Phi\) are the standard Gaussian density and distribution. In particular the exact collar expression has the nonzero boundary correction with the correct sign, independently of which admissible cutoff \(\chi\) was used.

For the scalar YM mark, (CM.30) isolates the constrained trace term which appears in the Gaussian diagnostic, but its complete correction is now explicit. It contains the inner exterior-force response, the gradients of inherited E/R/B and coarea terms, the heterogeneous action correction, the boundary-relocation contribution, the actual incoming remainder, and a coordinate-collar expectation. No parameter derivative of the running coupling or of an adaptive R reference kernel has been used.

The readout \(a(v)+\tfrac12\operatorname{Tr}(C(v)V(v))\) is still a function of retained data. It has **not** yet been identified with a scalar coarse field plus a scalar constant in the F-01 prescription. That projection, its exact normalization, and its localized error remain part of M-04/F-03.

### 4. Local quantitative control of the collar term

This section proves that the ordinary expectation in (CM.29) can be bounded without a global partition-function comparison or a surface-density estimate.

Suppose, at the fixed retained datum, that for every \(p\ge1\),

\[
 \|z_j\|_p\le M_j+c_z\sqrt p,
 \qquad
 \|\nabla_i\Psi\|_p\le U_i+c_\Psi k_i\sqrt p.
 \tag{CM.36}
\]

Theorem CM.1 and (CM.19) give one sufficient instance:

\[
 \begin{split}
 U_i&=|b_i|+d_i+
       \sum_j(\|K_{ij}\|+A_{ij})M_j,\\
 k_i&=\sum_j(\|K_{ij}\|+A_{ij}),
 \end{split}
 \tag{CM.37}
\]

with fixed \(c_z,c_\Psi\). The following result only needs (CM.36).

#### Proposition CM.3 -- rare-collar estimate with anchored summation

Let \(q_i=\nu_v(E_i)\), and put \(L_i=1+\log(1/q_i)\) when \(q_i>0\). Then

\[
 \begin{split}
 |\mathcal E_\chi(B)|
 \le C\sum_{i:q_i>0}q_i\bigg[&
 |\operatorname{tr}B_{ii}|\\
 &+\sum_j\|B_{ij}\|
 (M_j+c_z\sqrt{L_i})
 \left(P_i^{-1}+U_i+c_\Psi k_i\sqrt{L_i}\right)
 \bigg].
 \end{split}
 \tag{CM.38}
\]

The constant depends only on the fixed cutoff template and bounded block dimension. A term with \(q_i=0\) is zero. No total-volume factor is implicit in (CM.38).

**Proof.** For an event of probability \(q>0\), choose
\(r=\max\{2,\log(1/q)\}\). Holder gives

\[
 \nu(\mathbf1_E|Y|)\le
 q^{1-1/r}\|Y\|_r\le e\,q\|Y\|_r.
 \tag{CM.39}
\]

Here the last inequality also holds when \(r=2\), since then \(q\ge e^{-2}\). The trace term in (CM.29) is bounded directly by \(q_i|\operatorname{tr}B_{ii}|\). For the derivative-cutoff term use (CM.28), (CM.39), and the first estimate in (CM.36). For the last term apply Holder once more to the product of \(z_j\) and \(\nabla_i\Psi\), at moment order \(2r\), and use both estimates in (CM.36). Since \(r\le2L_i\), all factors fit in (CM.38) after a fixed change of constant. Sum the explicit matrix entries. \(\square\)

For an insertion anchor \(x\), a useful input is an actual weighted matrix bound

\[
 \sum_{i,j}e^{\kappa(d(x,i)+d(x,j))}\|B_{ij}\|
 \le V_x.
 \tag{CM.40}
\]

When the other local quantities in (CM.38) have a controlled envelope, (CM.40) makes the collar sum local and volume independent. It is not enough to bound the trace alone: the full matrix entries occur in (CM.38).

If, in addition, \(D_i\) contains a Euclidean ball of radius \(c_DP_i\) and the mean obeys \(|\nu z_i|\le c_DP_i/4\), the concentration proof of (CM.15) gives

\[
 q_i\le C\exp[-c\lambda P_i^2].
 \tag{CM.41}
\]

Indeed, outside \(\tfrac12D_i\), the block is at Euclidean distance at least \(c_DP_i/2\) from zero, hence at least \(c_DP_i/4\) from its mean. A finite union over real components and (CM.17) gives (CM.41). The required mean margin is a numerical condition on the actual right side of (CM.14). The fact that the support is a product does not establish that margin.

For a homogeneous radius \(P\), uniform force envelopes and (CM.40), (CM.38)-(CM.41) yield an exponentially small collar error with an explicit polynomial prefactor in \(P\). To insert a numerical upper bound on \(q_i\) in (CM.38), one can either use the same Holder proof with the numerical rate in place of the optimization or use the monotonicity of \(q(1+\log(1/q))^r\) once \(q\) is sufficiently small. No monotonicity outside that range is assumed.

This is an actual normalized-measure estimate whenever its moment and probability inputs have been verified. It is not yet a proof of those inputs on every interacting RG history.

### 5. Retained-variable derivatives and the scalar marginal coefficient

#### 5.1 Exact current within one fixed regular chart

Let \(v(s)\) be a differentiable retained-data path which stays within one fixed live geometry and coupling chart. The product support (CM.1) is then fixed. Define the unnormalized exponent

\[
 L(z;v)=-\tfrac12z^TK(v)z+b(v)^Tz+W(z;v).
 \tag{CM.42}
\]

Whenever differentiation is justified by the actual local bounds,

\[
 \frac d{ds}\nu_{v(s)}F_{v(s)}
 =\nu_{v(s)}\dot F
  +\operatorname{Cov}_{\nu_{v(s)}}(F,\dot L).
 \tag{CM.43}
\]

In particular,

\[
 \dot L=-\tfrac12z^T\dot Kz+\dot b^Tz+\dot W.
 \tag{CM.44}
\]

Every background, chart, E/R/B, coarea and boundary-relocation derivative is retained in (CM.44). A retained-only additive constant in \(L\) disappears from the covariance, as it must for the same conditional law; its derivative remains in the outer weight. This is a conditional normalization cancellation, not permission to discard relative history weights.

Under the weighted covariance estimate, (CM.43) yields the local current bound

\[
 \left|\frac d{ds}\nu F-\nu\dot F\right|
 \le C\sum_{i,j}e^{-\gamma d(i,j)}
       \|\nabla_iF\|_2\|\nabla_j\dot L\|_2.
 \tag{CM.45}
\]

It is the **gradient** of the complete retained score which must be localized and estimated. A real bound on the conditional partition function does not imply this estimate.

Integrating (CM.43) along an admitted path gives the finite-difference current needed by M-03. If the path crosses a live-selector interface, its interface current must additionally be included. The fixed regular support theorem does not remove those currents, and the formula is not asserted across a change of geometry without them.

#### 5.2 The exact second retained derivative

For retained coordinates \(v_a,v_b\) inside such a chart, put \(S_a=\partial_aL\). Direct differentiation of the normalized integrals gives

\[
 \begin{split}
 \partial_a\partial_b(\nu F)
 ={}&\nu F_{ab}
 +\operatorname{Cov}(F_a,S_b)
 +\operatorname{Cov}(F_b,S_a)\\
 &+\operatorname{Cov}(F,\partial_a\partial_bL)
 +\kappa_3(F,S_a,S_b).
 \end{split}
 \tag{CM.46}
\]

**Proof.** Differentiate (CM.43) in the second coordinate. Differentiating the two factors in the covariance produces the two covariance terms involving derivatives of its arguments. The change of the normalized law produces the third joint cumulant. Expanding those expectations proves (CM.46); retained-only constants in \(S_a,S_b\) cancel from every covariance and cumulant. \(\square\)

This gives a direct formula for the quadratic retained-background coefficient of the exact transported scalar mark, once the appropriate scalar projection and physical normalization have been fixed. It includes the actual first and second retained derivatives of the complete density and of the projected incoming mark. Using only the derivative of the native classical action would omit four classes of terms in (CM.46).

No uniform bound on those derivatives or a numerical evaluation of the interacting scalar coefficient is supplied by this identity. Thus it does not complete F-03 or M-04.

### 6. The precise remaining inequalities

#### C-08

The fixed product support, granted the source estimates of Annex AA, removes the unspecified inner-support premise for the source-normal-form regular marginal. The remaining quantitative theorem must verify, on the actual complete family (CM.5):

- the constrained precision gap and weighted localization on the heterogeneous admitted class;
- the full E/R/B/measure/heterogeneous Hessian bound strong enough for the numerical covariance margin and (CM.12);
- the local zero-field gradient and exterior-force envelopes in (CM.14), including any collar-margin requirement used in (CM.41);
- the actual field and gradient estimates for the projected marks, with the fixed factorial growth needed at every source order;
- the uniformity in scale and volume, with retained-background factors exposed before outer-history averaging.

Neither a small value bound for the action nor the covariance inequality for the earlier homogeneous no-R model establishes these statements. C-08 therefore remains open.

#### M-04

The exact incoming scalar transport now admits the readout (CM.30), and the finite retained coefficient can be expressed by (CM.46). To meet the stated requirements one must still prove, for that same incoming mark and full law:

1. a localized representation and quantitative readout bound for (CM.2), rather than assuming that it is a native field;
2. the scalar projection of \(a(v)+\tfrac12\operatorname{Tr}(C(v)V(v))\) into the prescribed current scalar basis and identity coefficient;
3. a uniform bound in M-03 for the exterior-mean, complete-interaction-gradient, incoming-remainder and collar terms in (CM.30);
4. localized retained-score and direct-mark derivatives for (CM.45), including interfaces encountered by the actual finite-difference norm;
5. the scale gain or coefficient budget that makes the subsequent all-scale induction valid. A one-step \(O(g)\) comparison alone is not summable on the expected asymptotically free trajectory.


### 7. References

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243-285: (3.15)-(3.25), printed pp.267-270. The actual current cutoff and exponent are retained.
-  Annex W: complete current-coordinate law, coarea and Haar normalization, boundary relocation, and Schur-complement bookkeeping.
- Annex AA: source-normal-form product support after complete R, exact projection of marked jets, and the weighted Neumann boundary check.
- The conditional-mean and real cut-cumulant proofs of the earlier annexes: used only for their stated weighted covariance and cumulant mechanism, not as estimates for a different interacting law.

All new elementary identities are proved above. The proposed force and moment criteria retain their unverified actual-model inputs explicitly.


---
