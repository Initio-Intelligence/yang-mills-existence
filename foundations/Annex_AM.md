# Reference-coordinate current transfer and the local averaging-Hessian estimate

**Annex AM.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

This note proves a local weighted forward averaging row and adjoint-minimizer rows, a weighted regular constrained-covariance estimate, and a physical-minimizer tangent theorem with an explicitly retained matched-lift premise. The last theorem avoids the rough gauge-projection term in the earlier formula (RT.33). It is not a bound for the excluded generic covariant Laplacian of the fully gauge-projected covariance.

The common-gauge lift is constructed in CC.5 for matched source-regularized data. The actual joined geometry, the raw-data matching, and the complete native/carrier application remain necessary to complete C-05. No uniform conclusion is claimed here.

### 1. Actual norms, geometry and source inputs

Let \(\eta\) be the physical fine mesh. An admitted determining geometry has blocks \(\Delta(a)\) of mesh \(h_a=L^{r_a}\eta\) and the source distance \(d(a,b)\). All constants below depend on the fixed group, dimension \(d=4\), block size and admitted geometric constants. They do not depend on the number of determining layers or the total volume.

The fine inner product uses measure \(\eta^4\). The determining-variable inner product uses \(h_b^4\). Adjoint symbols refer to these real inner products; their analytic continuations are bilinear transposes, not conjugate-dependent operations.

A positive profile \(w\) is admissible at rate \(\beta\) if

\[
 w_a/w_b\le A_w e^{\beta d(a,b)}.
 \tag{CC.1}
\]

An endpoint factor \(e^{-\kappa d(a,A_*)}\) can be included in \(w_a\); it increases the comparison rate by at most \(\kappa\). Write

\[
 \|f\|_{F_w}=\sup_a w_a^{-1}\|f\|_{\infty,\Delta(a)},
 \quad
 \|u\|_{E_w}=\sup_a\max\left\{
 \frac{\|u\|_{\infty,\Delta(a)}}{h_a^2w_a},
 \frac{\|\nabla_Uu\|_{\infty,\Delta(a)}}{h_aw_a},
 \frac{\|\Delta_U^{\rm cov}u\|_{\infty,\Delta(a)}}{w_a}
 \right\}.
 \tag{CC.2}
\]

The last operator is the componentwise covariant Laplacian. It is distinguished from the Wilson quadratic Hessian below.

CMP96 (2.2), Lemma 2.1 and (2.60)–(2.61) supply

\[
 d(a,b)\ge RM\max\{|r_a-r_b|-1,0\},
 \quad
 h_a/h_b\le L e^{c_h d(a,b)},\quad
 c_h=\frac{\log L}{RM},
 \tag{CC.3}
\]

and finite exponential row sums \(S(t)=\sup_a\sum_b e^{-td(a,b)}\) at the admitted rates. Choose the fixed geometry so that all rates used below, in particular

\[
 t_*=\delta-\beta-\kappa-4c_h>0,
 \tag{CC.4}
\]

retain the additional reserve required by that source summation lemma. Here \(\delta\) is a common smaller exponential rate of the source kernels. This is a fixed geometric restriction, not a claim for arbitrary \(R,M\).

We use the original regular Wilson propagator

\[
 G_0=(\Delta+DRD^*+Q^*aQ)^{-1},
 \quad
 H_0=G_0Q^*(QG_0Q^*)^{-1},
 \quad
 P_0=I-H_0Q,
 \quad
 C_0=P_0G_0=G_0P_0^*.
 \tag{CC.5}
\]

\(\Delta\) is the Wilson quadratic Hessian at the real background. \(G_0\) is the operator of CMP99 Theorem 3.3, before the gauge-invariant modification used to define \(G_1\). Theorem 3.3 includes the component-Laplacian estimate. CMP102 (129)–(130) supplies that estimate also for \(H_0\).

In (129)–(130), the printed \(H_0B\) takes dimensionless determining data \(B\). In the convention of (CC.5), its argument is \(h^{-1}B\). Thus the source estimate reads

\[
 \left|D_{\rm out}^{(j)}
       (H_0h^{-1})(x,b)\right|
 \le C h_a^{-1-j}h_b^{-4}e^{-\delta d(a,b)},
 \quad j=0,1,2,\quad x\in\Delta(a),
 \tag{CC.6}
\]

where \(j=2\) means the component covariant Laplacian, not all arbitrary second partial derivatives. Formula (CC.6) is not an estimate for the fully gauge-projected covariance \(\mathcal G\).

### 2. A uniform forward row for the actual averaging map

#### Proposition CC.1 — forward averaging without a flat-map identification

On the admitted real background class, and on its fixed smaller analytic relative-field neighborhood, the source reference-regularized averaging derivative has the local weighted bound

\[
 \|Qu\|_{\infty,w}\le C_Q A_w e^{\beta c_Q}\|u\|_{\infty,w}.
 \tag{CC.7}
\]

The norms on the two sides use their respective fine and determining blocks and the same physical profile. The fixed constant \(c_Q\) allows the actual averaging stencil.

**Proof.** Fix a proper-scale local gauge cube of size \(O(Mh)\), with \(h=L^j\eta\). The text immediately following CMP99 (3.78) gives analyticity of the actual relative averages on \(\|A\|_\infty<\alpha_1/h\), and bounds their intermediate logarithms by

\[
 \|B_r\|_\infty\le C\alpha_1L^{r-j},\quad 0\le r<j.
 \tag{CC.8}
\]

The remaining fixed-\(L\) averaging step is analytic and has a fixed derivative bound on the small one-step chart, by (3.79). Consequently the final relative logarithm is bounded by \(C_L\alpha_1\) on that disc. The dimensionful relative averaging map from the defining (3.14),

\[
 \Phi_j(A)=h^{-1}\mathcal Q_j(U,\eta A)
   =\frac{1}{ih}\log\overline{(e^{i\eta A})}^{\,j}_{U,\rm rel},
 \qquad D\Phi_j(0)=Q_j(U).
 \tag{CC.9}
\]

Here \(\mathcal Q_j\) is exactly the source nonlinear function in CMP99 (3.13), and the last symbol denotes its reference-corrected relative average, with the background \(U\) fixed. It is not the quotient of two uncorrected symmetric averages.

therefore satisfies \(\sup\|\Phi_j(A)\|\le C_L\alpha_1/h\). Cauchy on \(A=tu\) gives

\[
 \|Q_j(U)u\|_\infty\le C_L\|u\|_\infty,
 \tag{CC.10}
\]

uniformly in \(j\). The same argument holds about a smaller complex relative-field center by retaining half the source reserve. There is no constant raised to the number of layers.

The physical support radius of the \(j\)-step derivative is at most \(c_Lh\), since its fixed-range one-step radii sum as a geometric series. Choose the admitted collar with \(RM>Lc_L\), allowing the endpoint conventions. A point in a determining layer can then meet stencils from only a fixed number of neighboring layers. This follows from the separation in CMP96 (2.2): a layer two or more steps away is separated by a distance greater than the stencil radius. The proper meshes of the remaining layers differ by fixed powers of \(L\), and their source distances are bounded by a fixed \(c_Q\).

Apply (CC.1) on these supports. Real local gauge changes act unitarily. For complex relative fields the real gauge is fixed and the relative field remains in the source neighborhood. This proves (CC.7). \(\square\)

**Operator-family caution.** The symmetric contour average in CMP109 (0.12), the reference-transport average used to define CMP99 (3.14), and their gauge corrections must not be interchanged. In particular, the bare symmetric contour derivative at the identity need not be the straight-line operator of CMP95. The preceding proof uses the actual bounded relative average identified in CMP99 (3.14), (3.78) and does not make that flat identification. A stand-alone physical transpose row for the symmetric average has not been proved here and is not needed in Proposition CC.3.

Only those estimates of the CMP98 averaging paper that are explicitly reproduced in CMP99 are used.

### 3. Adjoint minimizing rows with the full baseline profile retained

#### Proposition CC.2 — arbitrary slow current profiles

Let \(H\) be the dimensionful minimizing operator of CMP99 (3.126), or \(H_1\) of (3.129), on their admitted background class. Then

\[
 \|H^*f\|_{\infty,w}\le C_HA_w L^4
           S(\delta-\beta-4c_h)\|f\|_{\infty,w}.
 \tag{CC.11}
\]

The same formula holds with \(H_1\), and with an endpoint profile included as in (CC.4).

**Proof.** The value part of source (3.133) is

\[
 |H(x,b)|\le C h_b^{-4}e^{-\delta d(a,b)},
 \qquad x\in\Delta(a).
\]

The physical adjoint therefore gives

\[
 |H^*f(b)|
 \le C\sum_a (h_a/h_b)^4e^{-\delta d(a,b)}
                \|f\|_{\infty,\Delta(a)}.
 \tag{CC.12}
\]

Use (CC.1), then (CC.3), and the admitted exponential row sum. This proves (CC.11). \(\square\)

The familiar current norm \(h_a^{-3}\) reduces the mesh exponent in this argument from four to one; that special case was proved in the argument. Keeping a general profile is useful here because the actual reconstructed baseline has stronger original-layer current restrictions than the generic joined-layer bound.

### 4. Regular constrained covariance without a rough projection

#### Proposition CC.3 — current forcing to a second-order field

With the stated fixed rate reserves,

\[
 \|C_0f\|_{E_w}\le C_0^{\rm bd}\|f\|_{F_w}.
 \tag{CC.13}
\]

**Proof.** The localized value, first-derivative and component-Laplacian estimates of CMP99 Theorem 3.3 map a forcing on \(\Delta(b)\) to

\[
 C e^{-\delta d(a,b)}
       (h_a^2,h_a,1)\|f\|_{\infty,\Delta(b)}.
 \tag{CC.14}
\]

Summation against (CC.1) bounds \(G_0f\) in \(E_w\). Proposition CC.1 and the fixed neighboring-block mesh comparison then give

\[
 |(QG_0f)(b)|\le C h_b^2w_b\|f\|_{F_w}.
 \tag{CC.15}
\]

Set \(B_b=h_b(QG_0f)(b)\). Thus \(|B_b|\le Ch_b^3w_b\|f\|_{F_w}\). Applying the actual source bound (CC.6), with the physical measure \(h_b^4\), gives after normalization by the output factor \(h_a^{2-j}w_a\)

\[
 C\sum_b (h_b/h_a)^3
             e^{-\delta d(a,b)}w_b/w_a\,\|f\|_{F_w}.
 \tag{CC.16}
\]

The reserved rate in (CC.4) bounds this sum. Both pieces of \(C_0=G_0-H_0QG_0\) are now controlled in \(E_w\), proving (CC.13). \(\square\)

In particular the two powers gained by \(G_0\) before the average are retained. Applying an output current row to an unrelated bare determining mark would lose that information and reproduce the fine-collar problem (RT.12).

The source local kernels and averaging rows are analytic on their admitted relative-field domains. Their smaller common domain uses the actual strong field/current restrictions and a uniform inverse reserve for \(QG_0Q^*\). One cannot obtain a claim for independently altered, unmatched kernels by applying this proposition to their names alone.

### 5. Physical stationarity removes the \(K^*D_2\) term

At a physical constrained Wilson minimum \(W\), define

\[
 T=\Delta-D_2,\qquad
 \langle A,D_2A\rangle
       =2\langle H C^{(2)}(A),J_W\rangle .
 \tag{CC.17}
\]

The normalization of \(C^{(2)}\) is matched to the dimensionful \(H\), as specified after CMP99 (3.127). The source multiplier is \(\lambda=H^*J_W\). The exact formula (3.136) retains this multiplier at each determining bond. Its subsequent printed estimate first substitutes \(|\lambda_b|\le CM\alpha h_b^{-3}\), and invokes the unavailable averaging-paper inequality (149). That substituted estimate alone would **not** imply the stronger profile bound needed here.

The needed pointwise derivative information is, however, explicitly displayed in a different published source: CMP102, printed p.289, equation (72). The argument below uses that displayed equation, not the formula (149).

#### Lemma CC.3a — local multiplier estimate from the reproduced pointwise derivative

For the actual reference-regularized averaging and its admitted geometry,

\[
 |D_2u(x)|\le C h_a
       \sup_{b\in N(a)}|\lambda_b|\,
       \sup_{y\in N(a)}|u(y)|,\quad x\in\Delta(a).
 \tag{CC.18}
\]

Here \(N(a)\) is a fixed union of neighboring proper-scale blocks. The constants are independent of the fine spacing, number of layers and total volume.

**Proof.** For a determining bond \(b\) of mesh \(h_b=L^j\eta\), write
\(f_b(A)=C_j(h_bA,b)\) in CMP102's notation (44), and let

\[
 \mathcal F_b(A;x)
   =\frac{\delta f_b}{\delta A}(A;x).
 \tag{CC.18a}
\]

The kernel uses the physical fine measure \(\eta^4\). CMP102 (72) states the pointwise bound

\[
 \mathcal F_b(A'-HD(A');x)
   =h_b\frac{\delta C_j}{\delta A}
       \bigl(h_b[A'-HD(A')],b;x\bigr),
 \qquad
 |\mathcal F_b(A'-HD(A');x)|
 \le 2C_3\epsilon_3 h_b^{1-d},\quad d=4.
 \tag{CC.18b}
\]

The paragraph immediately after that equation explains the factor \(h_b^{-d}\) as the change to the physical fine-lattice measure. The linearizing correction \(D(A')\) is holomorphic, begins at degree two, and is defined on the complex **value** ball \(\|A'\|_{(-1)}<\epsilon_3\), where \(\|A'\|_{(-1)}=\sup h|A'|\). The value-ball assertion is explicit in CMP102 p.287; a first-gradient assumption is additional, not a condition needed to define this map.

Fix a test direction \(V\) and put \(A'=tV\). Since \(D(tV)=O(t^2)\), and the remainder \(C_j\) has no constant or linear term, the coefficient of \(t\) in
\(\mathcal F_b(tV-HD(tV);x)\) is the derivative of the quadratic part \(f_b^{(2)}\) at \(V\). Cauchy on
\(|t|=\epsilon_3/(2\|V\|_{(-1)})\) gives

\[
 \left|
   \frac{\delta f_b^{(2)}}{\delta A}(V;x)
 \right|
 \le 4C_3h_b^{1-d}\|V\|_{(-1)}.
 \tag{CC.18c}
\]

The quadratic homogeneity convention is
\(f_b^{(2)}(A)=h_b^2 C_j^{(2)}(A,b)\), exactly as explained in CMP99 p.421 after (3.127). Therefore

\[
 \left|
   \frac{\delta C_j^{(2)}}{\delta A}(V,b;x)
 \right|
 \le C h_b^{-1-d}\|V\|_{(-1)}.
 \tag{CC.18d}
\]

This derivative depends on \(V\) only in the actual local \(j\)-average footprint. Take \(V=u\) on that footprint and zero elsewhere. Sharp truncation is allowed because only the value-ball norm is used. The stencil and collar comparison proved in CC.1 makes every proper mesh met by the footprint comparable to \(h_b\), with fixed constants. Thus
\(\|V\|_{(-1)}\le C h_b\sup_{\operatorname{foot}(b)}|u|\), and

\[
 \left|
   \frac{\delta C_j^{(2)}}{\delta A}(u,b;x)
 \right|
 \le C h_b^{-d}
      \sup_{\operatorname{foot}(b)}|u|.
 \tag{CC.18e}
\]

The kernel vanishes when \(x\) is outside that footprint. For a fixed fine \(x\), only a fixed number of neighboring determining bonds, at meshes comparable to \(h_a\), have a footprint containing \(x\). Insert (CC.18e) into the exact CMP99 (3.136). Its physical determining factor \(h_b^{d+1}\) leaves the factor \(h_b\). The resulting fixed neighboring sum is (CC.18). \(\square\)

Substituting the generic admitted multiplier bound \(|\lambda|\le CM\alpha h^{-3}\) into (CC.18) recovers the printed CMP99 (3.137), and gives

\[
 \|D_2u\|_{F_w}\le C_D M\alpha\|u\|_{E_w}.
 \tag{CC.19}
\]

The stronger slow-profile bound (CC.11) can instead be used in (CC.18) when \(J_W\) has original-layer current restrictions. The local-majorant step is thus supplied by the reproduced pointwise derivative (72), not inferred from linear dependence on \(\lambda\) or from the already substituted bound (3.137).

#### Theorem CC.4 — normalized physical current of a matched tangent

Suppose \(W(t)\) is an admitted differentiable family of physical constrained Wilson minima with its fixed determining geometry. Work in the relative Landau gauge based at \(W(0)\). Let \(u\) be its physical tangent at zero, and let \(A\) be an actual matched lift satisfying

\[
 QA=Qu,\qquad RD^*A=RD^*u=0.
 \tag{CC.20}
\]

Assume that \(A\), its Wilson quadratic current \(\Delta A\), and the actual baseline multiplier make the following number finite:

\[
 F_A=\|\Delta A\|_{F_w}
      +\left\|
       h_a\sup_{N(a)}|\lambda|\sup_{N(a)}|A|
       \right\|_{\infty,w}.
 \tag{CC.21}
\]

For \(C_0^{\rm bd}C_DM\alpha\le1/2\), the difference \(e=u-A\) satisfies

\[
 \|e\|_{E_w}\le 2C_0^{\rm bd}F_A.
 \tag{CC.22}
\]

It also satisfies a physical Wilson-current bound

\[
 \|\Delta e\|_{F_w}\le C_{\rm cur}F_A.
 \tag{CC.23}
\]

**Proof.** The source's unrestricted constrained variational equation is CMP102 (127), and its derivation in pp.296–297 is essential: admissible variations satisfy \(Qv=0\), without a Landau condition on the variation. Differentiating the constrained stationary equation at a true minimum gives

\[
 \langle v,Tu\rangle=0\quad\text{for every }Qv=0.
 \tag{CC.24}
\]

This is the actual Lagrange-Hessian equation, with the averaging Hessian term in (CC.17) retained. Since \(Qe=0\) and \(RD^*e=0\), the argument of CMP102 (129)–(133) gives the exact identity

\[
 e=C_0(D_2e-TA).
 \tag{CC.25}
\]

There is no \(K^*D_2\) term. The covariance in this identity constrains \(Q\), and physical stationarity supplied the unrestricted variation equation. Replacing an arbitrary fully gauge-projected forcing problem by (CC.25) would not be justified.

Proposition CC.3, (CC.18) and (CC.19) yield

\[
 \|e\|_{E_w}\le C_0^{\rm bd}
          (C_DM\alpha\|e\|_{E_w}+F_A).
\]

Absorb the first term to obtain (CC.22).

To recover the Wilson quadratic current, use \(RD^*e=0\), hence \(DD^*e=DPD^*e\) with \(P=I-R\). CMP99 (3.49) bounds \(DPD^*\) by a regular exponential kernel of order two. Applying its physical-measure kernel to \(|e|\le h^2w\|e\|_{E_w}\), with the same mesh-rate reserve, gives a bound \(Cw\|e\|_{E_w}\). The identity between \(D^*D+DD^*\) and the component Laplacian has only the local curvature term displayed in CMP102 (135). The Wilson Hessian differs from \(D^*D\) by the bounded local term of CMP99 (3.10), (3.69). Their coefficients are \(O(M\alpha h^{-2})\). Combining these facts with (CC.22) proves (CC.23). \(\square\)

#### Why the stronger baseline profile matters

Let \(n\) be the original layer, \(p\) the reconstruction scale, \(h_*=h_{\min(n,p)}\), and let \(h_a\le h_*\) be the joined mesh. The admitted old-B baseline restriction has the form

\[
 |J_W|\le \alpha_n h_*^{-1}h_n^{-2}.
 \tag{CC.26}
\]

If the actual smooth lift has \(|A|\le u_nh_n^{-1}\), Proposition CC.2 and (CC.18), with fixed profile comparison losses, give

\[
 |D_2A|
 \le C\alpha_nu_n\frac{h_a}{h_*}h_n^{-3}
 \le C\alpha_nu_n h_n^{-3}.
 \tag{CC.27}
\]

This is bounded by the required \(u_nh_*^{-1}h_n^{-2}\) profile, since \(h_*\le h_n\). Replacing (CC.26) prematurely by the weaker \(O(\alpha h_a^{-3})\) would discard this gain.

The nonlinear physical current in a left exponential chart has, at its real center, derivative equal to the quadratic Hessian plus a local chart term bounded by \(C\eta|u||J_W|\). This follows by differentiating the local exponential differential, whose first correction is \(\frac12 i\eta\,\mathrm{ad}_u\). The strong baseline bound (CC.26), \(\eta\le h_a\le h_*\), and (CC.22) bound that chart term by the same profile. This controls the chart conversion once the actual lift (CC.20) is available.

### 6. A matched lift for the actual regularized linear constraint

The following strengthens the preceding conditional theorem. It does not identify a raw symmetric-average derivative with the reference-regularized \(Q\). That conversion is kept explicit below.

#### Lemma CC.5 — the Landau correction needs no second-gradient estimate

Use one fixed real physical minimum \(W\), its actual joined operators \(D,Q,Q',R,G'\), and its physical current \(J_W\). Suppose the original-layer profiles satisfy (CC.1) with a sufficient rate reserve. Let \(h_a\le h_*:=h_{\min(n,p)}\le h_n\). Suppose an actual input tangent \(A\) obeys

\[
 |A|\le C_Au_nh_n^{-1},\qquad
 |D^*A|\le C_Au_nh_n^{-2},\qquad
 |\Delta A|\le C_Au_nh_n^{-3},
 \qquad
 |J_W|\le\alpha_nh_*^{-1}h_n^{-2}.
 \tag{CC.28}
\]

Set \(w_2=u_nh_n^{-2}\), \(w_3=u_nh_n^{-3}\), and define

\[
 \chi=G'RD^*A,\qquad \widehat A=A-D\chi.
 \tag{CC.29}
\]

Then

\[
 Q\widehat A=QA,\qquad RD^*\widehat A=0,
 \tag{CC.30}
\]

and, with constants independent of the fine spacing and the joined collar depth,

\[
 |\chi|\le C C_Ah_a^2w_2,\qquad
 |D\chi|\le C C_Ah_aw_2,\qquad
 |\widehat A|\le C C_Au_nh_n^{-1},\qquad
 |\Delta\widehat A|\le C C_A(1+\alpha_n)w_3.
 \tag{CC.31}
\]

**Proof.** The projection \(R\) has range \(\Delta_{\rm sc}\ker Q'\), where \(\Delta_{\rm sc}=D^*D\) is the covariant scalar Laplacian; this is CMP99 (3.21). Thus, if \(f\in\operatorname{ran}R\), there exists \(\chi\in\ker Q'\) with \(\Delta_{\rm sc}\chi=f\). Since \(Q'\chi=0\), the same \(\chi\) is \(G'f\). In particular

\[
 Q'G'R=0,\qquad R\Delta_{\rm sc}G'R=R.
 \tag{CC.32}
\]

CMP99 (3.115) gives \(QD=D^{\rm coarse}Q'\). Applying these identities to (CC.29) proves (CC.30). These are exactly the projection identities used by the source in (3.119); they are not an assumed right inverse for the raw nonlinear constraint.

For the norms, write \(R=I-P\). The physical-measure kernel of \(P\), CMP99 (3.49), is an exponentially decaying operator of order zero. Its row sum against the slow profile \(w_2\) is bounded by the same geometric argument as (CC.10). Thus \(|RD^*A|\le C C_Aw_2\). The scalar \(G'\) value and first-gradient rows in Theorem 3.1, (3.42), then give the first two estimates of (CC.31), with local gains \(h_a^2\) and \(h_a\), respectively. This uses no bound for a general second gradient of \(G'\).

The quadratic Wilson Ward identity is CMP99 (3.117), involving the physical current \(J_W\). Replacing its gauge parameter by \(t\chi\), and comparing the coefficient bilinear in \(t\) and an arbitrary field \(v\), gives the exact weak identity

\[
 2\langle v,\Delta D\chi\rangle
 =\left\langle i[\chi(b_-)+R_b\chi(b_+),v(b)],J_W(b)\right\rangle .
 \tag{CC.33}
\]

Consequently

\[
 |(\Delta D\chi)(b)|
 \le C|J_W(b)|\bigl(|\chi(b_-)|+|\chi(b_+)|\bigr).
 \tag{CC.34}
\]

There is no derivative of \(\chi\) on the right. Its original-layer bound is

\[
 |J_W|\,|\chi|
 \le C C_A\alpha_nu_n
       \frac{h_a^2}{h_*h_n}\,h_n^{-3}
 \le C C_A\alpha_n w_3.
 \tag{CC.35}
\]

The neighboring-point comparisons are fixed profile constants. Together with \(h_a/h_n\le1\), this proves the remaining assertions of (CC.31). \(\square\)

#### Consequence for a physically stationary tangent

Suppose the actual relative-Landau tangent \(u\) of the reconstructed minimum has the **matched regularized datum**

\[
 Qu=QA.
 \tag{CC.36}
\]

Then \(\widehat A\) satisfies the matching condition (CC.20). Apply Theorem CC.4 with \(w=w_3\). Proposition CC.2, (CC.18), and the original value estimate for \(\widehat A\) give

\[
 |D_2\widehat A|
 \le C C_A\alpha_n u_n\frac{h_a}{h_*}h_n^{-3}
 \le C C_A\alpha_n w_3.
 \tag{CC.37}
\]

Thus, for the same fixed smallness reserve as in CC.4,

\[
 e:=u-\widehat A,
 \qquad
 |e|\le CC_Ah_a^2w_3,\quad
 |\nabla e|\le CC_Ah_aw_3,\quad
 |\Delta e|\le CC_Aw_3,
 \tag{CC.38}
\]

and the physical current derivative of \(u\) has the original \(w_3\) bound, including the local exponential-chart correction already described after (CC.27). This is stronger than the reconstructed target \(u_nh_*^{-1}h_n^{-2}\).

A general uniform bound for \(\nabla D\chi\) has **not** been asserted. It is unnecessary for the forcing estimate. When the original tangent also has \(|\nabla A|\le C_Au_nh_n^{-2}\), restore its infinitesimal gauge after solving:

\[
 u+D\chi=A+e.
 \tag{CC.39}
\]

The right-hand side has the original value and first-gradient bounds by (CC.38). Gauge covariance changes the physical current derivative by a local adjoint term bounded by \(|J_W||\chi|\), which is controlled by (CC.35). Curvature has the corresponding local commutator correction. This proves the regularity in that representative without an unsupported scalar second-gradient estimate.

#### The actual data conversion that is still required

Condition (CC.36) is an equality of the source's regularized data. The raw symmetric averaging \(M\) used in the determining constraints, and the reference/gauge-regularized relative average whose differential is \(Q\), are not automatically the same even at a common baseline. In particular, \(\chi\in\ker Q'\) generally does not mean that \(\chi\) vanishes at all determining centers. The projection in (CC.29) therefore preserves \(Q\), but does not by itself prove preservation of the raw \(M\)-datum.

A source one-step conversion is visible in CMP99 (3.113), for the averaging operation underlying that reference construction. Write \(m(A)\) for its raw relative-average derivative, \(q(A)=QA\) for the corrected derivative, and \(\xi_y(A)\) for \(1/i\) times the derivative at zero of \(\overline{R_yU'_t}\), with \(U'_t=\exp(i\eta tA)\). Differentiating the printed endpoint factors gives exactly

\[
 q(A)=m(A)+D^{\rm coarse}\xi(A),\qquad
 |\xi_y(A)|\le C h\sup_{B(y)}|A|.
 \tag{CC.40}
\]

Here \(h=L\eta\) for this step, and \(D^{\rm coarse}\xi=(R_c\xi_{c_+}-\xi_{c_-})/h\). The local bound follows by differentiating the transported path logarithms in (3.113); each path has at most \(C h/\eta\) fine bonds, and each link insertion carries \(\eta\). At a real baseline all transports are isometries. The corresponding smaller complex chart uses its admitted uniform transport bound. Iterating the same reference construction yields levelwise endpoint corrections \(\Xi_j(A)\); the accumulated bound is \(C\sum_{r\le j}h_r\sup|Q_{r-1}A|\le C h_j\sup|A|\), by the forward averaging row and the geometric sum of scales.

The raw average in (CC.40) has **not** been identified with CMP109's later symmetric \(M\). A complete mixed-history application must check that operator-family conversion, and identify the composed endpoint corrections at the actual determining sites. A level-\(j\) bond can meet a site belonging to a finer determining shell, so a collection of levelwise corrections is not automatically one consistent gauge on the mixed determining set. The source's exact relative axialization would provide an alternative verification. For a verified correction, a bounded local gauge parameter is enough for current control by (CC.34); no generic second-gradient projection bound is needed. Neither an operator-family identification nor a mixed-level identification has been replaced by a same-baseline assertion.

### 7. Independent external parameters and the unresolved application

The independent external source-current variable must not replace \(J_W\) in (CC.17) or in the Wilson Ward equation. Here \(J_W\) is the physical current of the reconstructed minimum. External variables may enter its determining data through a prepared input map; the minimizing problem remains the physical Wilson problem.

For a genuine common holomorphic family of those data, (CC.24)–(CC.25) continue as identities in the parameters. The bounds then require the corresponding uniform analytic profile and inverse reserves. This does not prove the admission of an arbitrary prepared family, and it is not an estimate for unrelated separately modified propagator pieces.

The remaining application is concrete:

1. Identify the actual joined determining geometry and exact data.
2. Match the raw mixed-history datum to the source regularized constraint. Lemma CC.5 then constructs the common-gauge lift (CC.20) with its original-layer current bound. A same-baseline statement or pointwise comparison in two separately chosen gauges is insufficient.
3. Admit all actual independent external and preparation parameters on one strictly smaller domain.
4. Retain endpoint and marked-path localization through the nonlinear solution and the complete B carrier sums.

The source bond-support convention requires a separate check. In particular a local average generally produces star support; it does not by itself preserve a two-endpoint interior support. No exact reconstruction consistency is assumed in this note.

### Primary references

- CMP95 (1984), 17–40: (1.11), (1.18), used to distinguish its straight-line averaging from other source averaging conventions; no unidentified transpose norm is imported.
- CMP96 (1984), 223–250: (2.1)–(2.4), Lemma 2.1, (2.60)–(2.61), admitted geometry, physical support and exponential sums.
- CMP99 (1985), 389–434: Theorems 3.3–3.4; (3.49); (3.78)–(3.81), including its explicit transpose extension; (3.126), (3.133), (3.136)–(3.137), physical minimizing kernels and averaging Hessian.
- CMP102 (1985), 277–309: pp.285–289, (44), (51), (55), (63), (72), including the value-ball analytic linearizing map and the explicitly reproduced pointwise averaging derivative; pp.296–300, especially (123)–(143), unrestricted constrained stationarity and the regular alternative; the explicit \(H_0\) component-Laplacian bound (130).

No technical theorem of the CMP98 averaging paper is used beyond what CMP99 reproduces.
