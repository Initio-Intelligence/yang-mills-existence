# M-04: an exact local Wilson source and adaptive zero-free domains

Sections 1–7 prove an adaptive source estimate for the actual positive regular conditional law and a conversion for complex localized kernels. Sections 8–10 use the first-step raw lift, exact scalar Taylor rows and the original Gaussian reserve to prove a supported first-clean scalar theorem with separate continuous direct and kernel records on the buffered native graph. The complete ambient and arbitrary-history M-04 theorem is not asserted.

## 1. Freeze the operation, vary only the physical plaquette source

At one fixed regular step write the actual normalized conditional law in its source-free coordinates as

\[
 q_v(dz)=Z_v^{-1}{\bf1}_D(z)e^{L(z;v)}dz.                     \tag{LC.1}
\]

The reconstruction \(U(z,v)\), constrained background, independent-coordinate elimination, current cutoffs, history selectors, coarea density, all old E/B/R factors and every reference normalizer are fixed at zero source. The exponent \(L\) is the complete exponent; no factor is replaced by a Gaussian law.

For the incoming native scalar with fixed stencil \(S\), write its dimensionless value as

\[
 W(z,v):=h^4F(U(z,v))
   =\alpha\beta\sum_{p\in S}a_p s(U_p(z,v))-h^4c,
 \qquad s(P)=N-\operatorname{ReTr}P.                         \tag{LC.2}
\]

The finite stencil and its fixed coefficients are those of F-01/SR20.1. The incoming normalization \(\alpha\) and identity \(c\) are specified external numbers. The exact source family is

\[
 \mathscr Z_v(\tau)
 =\frac{\int_D e^{L(z;v)+\tau W(z,v)}dz}
        {\int_D e^{L(z;v)}dz}.                              \tag{LC.3}
\]

For an original Wilson scalar this is exactly a local inhomogeneous change of the physical plaquette coefficient,
\(\beta_p\mapsto\beta_p-\tau\alpha\beta a_p\), with every auxiliary construction specified. In particular it is **not** differentiation of the adaptive source-free recursion in its running coupling. The latter would also differentiate its minimizing maps, cutoffs, reference densities and scale choices.

At finite cutoff the integrals are analytic in \(\tau\) near zero, and

\[
 \partial_\tau\log\mathscr Z_v(0)=q_vW=h^4QF(v).             \tag{LC.4}
\]

Let

\[
 W_0(v)=W(0,v),\qquad \Delta W=W-W_0,
 \qquad \Xi_v(\tau)=q_v e^{\tau\Delta W}.
\]

Then exactly

\[
 \mathscr Z_v(\tau)=e^{\tau W_0(v)}\Xi_v(\tau),\qquad
 h^4QF=W_0+\partial_\tau\log\Xi_v(0).                       \tag{LC.5}
\]

The deterministic background factor is never discarded. It is separated because it has no zeros and because its retained-variable response is direct, not a normalized-kernel current.

## 2. Actual scalar fluctuations have a square-root background budget

### The verified real class used here

Use the real clean regular slice of the [M07 Regulator Repair](../F_analytic_families/M07_Regulator_Repair.md), Section 3: all preceding/current blocks regular, whole periodic free-bond region, no inherited large-field component or exterior force, and real admitted homogeneous determining data. The complete interacting conditional density is retained. That section establishes, uniformly in the depth and volume of this specified class,

\[
 \|z_i\|_{L^p(q_v)}\le C_z\sqrt p,\qquad p\ge1,             \tag{LC.6}
\]

and the actual reconstruction row estimate

\[
 \|\theta_e(z)\|\le Cg\sum_i e^{-\gamma d(e,i)}|z_i|,
 \qquad U_e(z,v)=e^{i\theta_e(z)}U_e(0,v),
 \qquad \beta g^2\le C.                                   \tag{LC.7}
\]

The complete quadratic/coarea/interaction law behind these facts is CMP119 (3.15), (3.25), with the native coordinate construction already examined in C-01 and C-07. The nonlinear background derivative and analytic chart are in CMP102 pp.305–309, Proposition 9 and (190). The proof below uses the actual real conditional law and (LC.6)–(LC.7), not a Gaussian substitution.

Let

\[
 E_0(v)=\beta\sum_{p\in S}|a_p|s(U_p(0,v)),\qquad R(v)=1+E_0(v).
\]

Choose a fixed nonnegative summable row \(w_i\), supported with exponential tails about the stencil, that bounds the sums of the four link rows in (LC.7), and put
\(Z_S(z)=\sum_i w_i|z_i|\). Its row sum is uniform, hence Minkowski and (LC.6) give

\[
 \|Z_S\|_p\le C\sqrt p.                                    \tag{LC.8}
\]

### Proposition LC.1 — centered real Wilson fluctuation estimate

For the exact scalar (LC.2),

\[
 |\Delta W(z,v)|
 \le C|\alpha|\bigl[\sqrt{E_0(v)}Z_S(z)+Z_S(z)^2\bigr],       \tag{LC.9}
\]

and therefore

\[
 \|\Delta W\|_{L^p(q_v)}
 \le C|\alpha|\left[\sqrt{E_0(v)}\sqrt p+p\right]
 \le C A(v)p,
 \quad A(v):=|\alpha|\bigl(1+\sqrt{E_0(v)}\bigr).            \tag{LC.10}
\]

The constants depend on the fixed stencil, group and admitted chart constants; they are independent of volume, cutoff, the real background energy and the scale on the stated clean class.

#### Proof

For real unitary plaquettes,
\(s(P)=\frac12\|I-P\|_{\rm HS}^2\). Consequently

\[
 |s(P)-s(P_0)|
 \le\sqrt{2s(P_0)}\|P-P_0\|_{\rm HS}
       +\tfrac12\|P-P_0\|_{\rm HS}^2.                       \tag{LC.11}
\]

Telescoping the four unitary link factors and using (LC.7) yields
\(\|P-P_0\|_{\rm HS}\le CgZ_S\). Multiply (LC.11) by \(\beta|a_p|\), use \(\beta g^2\le C\), and sum the fixed stencil. Cauchy–Schwarz in that finite sum gives (LC.9). Its moment estimate follows from (LC.8) at orders \(p\) and \(2p\). The identity coefficient cancels exactly from \(\Delta W\). ∎

This is sharper than an uncentered bound by \(R+Z_S^2\): the background appears only through \(\sqrt{E_0}\) in the fluctuating part.

### Extension when the regular conditional mean is not bounded

If only the centered coordinate estimate
\(\|z_i-m_i\|_p\le C\sqrt p\) is available, take the deterministic center \(m=q_vz\) in the convex product domain and use the same Lipschitz reconstruction along the segment from \(m\) to \(z\). The proof holds with \(W_0=W(m,v)\) and background energy evaluated at \(U(m,v)\). Alternatively the displayed center at zero gives (LC.10) with

\[
 R(v)=1+E_0(v)+\left(\sum_iw_i|m_i(v)|\right)^2.             \tag{LC.12}
\]

This proves a conditional source window on an arbitrary uniformly convex regular fiber. It does not prove that the mean term in (LC.12) is bounded by the specified output-native M-03 regulator. That is a genuine retained-background estimate.

## 3. A zero-free disk for the actual normalized source

### Theorem LC.2 — adaptive source analyticity

For \(\alpha\ne0\), there are fixed \(K,c,C>0\) such that

\[
 q_v\exp\left(\frac{|\Delta W|}{K A(v)}\right)\le2,          \tag{LC.13}
\]

and throughout

\[
 |\tau|\le\rho(v):=\frac{c}{A(v)}                           \tag{LC.14}
\]

one has

\[
 |\Xi_v(\tau)-1|<\tfrac12,\qquad
 |\log\Xi_v(\tau)|\le C A(v)|\tau|.                         \tag{LC.15}
\]

The logarithm is the analytic branch equal to zero at \(\tau=0\). Thus the exact source ratio \(\mathscr Z_v\) is zero-free on this disk. In particular,

\[
 |h^4QF(v)-W_0(v)|\le C A(v),                               \tag{LC.16}
\]

and for every \(m\ge2\),

\[
 |\kappa_m^{q_v}(W)|
 =|\partial_\tau^m\log\Xi_v(0)|
 \le m!\,[C A(v)]^m.                                      \tag{LC.17}
\]

For \(\alpha=0\) the insertion is constant and the source family is an entire nonvanishing exponential.

#### Proof

By (LC.10),
\(q_v|\Delta W|^n\le(C A)^n n^n\). Since \(n^n/n!\le e^n\), the exponential series proves (LC.13) for a sufficiently large fixed \(K\).

Put \(Y=|\Delta W|/(K A)\), so \(q_ve^Y\le2\). For \(u=K A|\tau|\le1/8\),

\[
 |\Xi_v(\tau)-1|
 \le q_v|e^{\tau\Delta W}-1|
 \le u\,q_v(Ye^{uY})
 \le\frac{2u}{1-u}<\tfrac12.                               \tag{LC.18}
\]

The penultimate inequality uses \(Ye^{uY}\le e^Y/(1-u)\). The logarithmic series therefore converges absolutely and gives
\(|\log\Xi_v|\le 2u/(1-3u)\le4u\). This proves (LC.14)–(LC.15). Cauchy's formula on a fixed smaller circle proves (LC.16)–(LC.17). The equality in (LC.17) follows from the exact normalized source definition. ∎

Several details are essential:

* The complex variable is the physical scalar source. The integration links remain real compact links. No coercivity of a complex Wilson trace is assumed.
* The disk shrinks only like \(R^{-1/2}\), after subtraction of the background value. Its reciprocal is within the allowed scalar energy budget. The identity centering does not shrink the disk.
* The center \(v\) is fixed when Cauchy is applied. Neither \(A(v)\) nor its square root is differentiated or declared holomorphic in retained data.
* These are all-order **same-root** conditional cumulant bounds. They do not establish a spatial carrier expansion or all-order multi-root contacts.

## 4. The normalized-kernel current remains separate

Let \(d\) be a smooth normalized retained-coordinate direction whose path stays inside the same fixed geometry and buffered chart. Its complete centered score is

\[
 S_d(z;v)=\partial_dL(z;v)-q_v\partial_dL,
 \qquad B_d(v)=\|S_d\|_{L^2(q_v)}.                          \tag{LC.19}
\]

Every constrained precision, coarea, old activity and boundary response belongs to \(\partial_dL\). Retained-only additive terms cancel from this centered score but remain in the outer history weight. The direct variation of the mark is a different record.

For the source with its mark specified in taking the kernel variation, define

\[
 K_d(\tau;v)=
 \frac{q_v[e^{\tau\Delta W}S_d]}{\Xi_v(\tau)}.              \tag{LC.20}
\]

### Proposition LC.3 — source estimate for the separate kernel current

On a fixed smaller disk than (LC.14),

\[
 |K_d(\tau;v)|\le C|\tau|A(v)B_d(v),                        \tag{LC.21}
\]

and

\[
 \partial_\tau K_d(0;v)
 =\operatorname{Cov}_{q_v}(W,\partial_dL)
 =h^4J_d(v),\qquad
 |h^4J_d(v)|\le C A(v)B_d(v).                              \tag{LC.22}
\]

This is a bound for the normalized-kernel response itself, not only for the total derivative of \(QF\).

#### Proof

The score has zero mean, so its numerator in (LC.20) is
\(q_v[(e^{\tau\Delta W}-1)S_d]\). The exponential-moment estimate (LC.13) implies, after reducing the source radius by a fixed factor,

\[
 \|e^{\tau\Delta W}-1\|_2\le C|\tau|A(v).
\]

Indeed \(|e^z-1|\le |z|e^{|z|}\), and the squared integrand is bounded by the same exponential reserve in (LC.13). Cauchy–Schwarz and \(|\Xi_v|\ge1/2\) give (LC.21). Differentiate at zero; the centered deterministic term \(W_0\) drops out against \(S_d\). Cauchy also gives the stated bound. ∎

The full smooth response is exactly

\[
 h^4\partial_dQF=q_v(\partial_dW)+h^4J_d.                  \tag{LC.23}
\]

Thus the direct and kernel records remain distinct. In particular the source method does not erase an interface current when a selector changes.

### A concrete score-gradient criterion

A Poincaré bound with gap \(\lambda\) gives

\[
 B_d\le\lambda^{-1/2}\|\nabla_z\partial_dL\|_2.             \tag{LC.24}
\]

For the actual decomposition
\(L=-z^TK(v)z/2+b(v)^Tz+W_{\rm int}(z;v)\), the gradient on the right is exactly

\[
 -K_dz+b_d+\nabla_z\partial_dW_{\rm int}.                    \tag{LC.25}
\]

For example, a verified coefficient row bound

\[
 \|(K_d)_{ij}\|\le a_d e^{-\gamma[d(i,d)+d(j,d)]},\quad
 |b_{d,i}|+\|\partial_i\partial_dW_{\rm int}\|_2
       \le a_d'e^{-\gamma d(i,d)}                           \tag{LC.26}
\]

and (LC.6) imply \(B_d\le C(a_d+a_d')\), with no volume factor. The proof is direct: Minkowski bounds the \(L^2\) norm of each row of \(K_dz\); its square sum over \(i\) converges by exponential decay. The other rows are treated in the same way, then use (LC.24).

For an anchored current, the available weighted covariance inequality yields the stronger spatial form

\[
 |h^4J_d|
 \le C\sum_{i,j}e^{-\gamma d(i,j)}
   \|\partial_iW\|_2\,
   \|\partial_j\partial_dL\|_2.                            \tag{LC.27}
\]

The scalar chart estimate supplies the rooted derivative row
\(\|\partial_iW\|_2\le C A(v)e^{-\gamma d(S,i)}\) wherever the corresponding differential chart row is verified. Combining this with (LC.26) gives

\[
 |h^4J_d|\le C A(v)(a_d+a_d')e^{-\gamma' d(S,d)}.             \tag{LC.28}
\]

These formulas identify exactly the mixed retained-score estimate needed. The native background derivative row (CMP102 (190)) controls the first reconstruction factor, but it does not by itself prove every mixed coefficient in (LC.26), especially inherited boundary/Schur terms. This note does **not** mark (LC.26) verified for arbitrary histories. Even (LC.28) alone is a pointwise spatial response bound, not the stronger exponential full-volume carrier decomposition of M-03.

## 5. What happens for complex localized kernels

The preceding positive-law argument does not automatically survive substitution of complex Gaussian decoupling parameters. There is, however, a useful quantitative conversion that shows how much reserve would suffice.

### Lemma LC.4 — complex-measure source window

Let \(\nu\) be a finite complex measure with \(\nu1=1\), and suppose a centered root \(\Delta W\) obeys

\[
 \int|\Delta W|^p\,d|\nu|
 \le T\,p!\,[K A]^p,\qquad p\ge1,\quad T\ge1.              \tag{LC.29}
\]

Then \(\Xi(\tau)=\nu e^{\tau\Delta W}\) is analytic and nonzero for

\[
 |\tau|\le\frac{c}{K A T},                                \tag{LC.30}
\]

and \(|\partial_\tau\log\Xi(0)|\le C KAT\).

#### Proof

The moment series gives, with \(u=K A|\tau|<1\),
\(|\Xi-1|\le T u/(1-u)\). Choose \(u\le1/(4T+2)\), so the right side is less than one half. The logarithmic series and Cauchy formula give the conclusion. ∎

Suppose on each connected physical carrier \(Y\) the actual normalized complex kernel, uniformly on its full decoupling polydisc, satisfies (LC.29) with

\[
 T_Y\le e^{\eta|Y|}.                                      \tag{LC.31}
\]

Then the source derivative costs only an extra exponential \(e^{\eta|Y|}\). This can be paid by a spatial reserve. For instance, if root decoupling coefficients have the factor \((R_s-1)^{-|Y|}\), there are at most \(C A_{\rm geom}^{|Y|}\) rooted carriers, and the specified connected M-03 weight is bounded by \(e^{2\kappa|Y|}\), a sufficient strict inequality is

\[
 \log(R_s-1)>
 \log A_{\rm geom}+2\kappa+\eta.                            \tag{LC.32}
\]

An additional fixed polynomial in \(|Y|\) is absorbed by any strict slack in (LC.32). This is a genuine conversion estimate: it does not demand one complex source radius uniform over every carrier. The circle for the source derivative is allowed to shrink by an explicitly paid exponential carrier factor.

In CMP116, the absolute Gaussian comparison (2.15)–(2.26) introduces precisely exponentials proportional to localized volume. A local quadratic root consumes a fixed part of the positive Gaussian reserve and has factorial moments under the remaining Gaussian majorant. Thus a bound of the *type* (LC.29) is compatible with that proof. But the exact normalized complex measure, its denominator, its raw-current supports and its moment factor \(T_Y\) must all be identified before applying this lemma to a physical output carrier. A bound on a single numerator term, or a theorem for a different localization coordinate, is not that identification.

## 6. Analysis of the proposed use of unmarked CMP116/CMP119

The source method is promising for a precise reason: the scalar is an exact action insertion, and the real root source window in Theorem LC.2 is now proved from the verified clean conditional chart. It supplies more than a formal derivative identity. It gives a nonzero analytic radius, a logarithm branch, factorial same-root bounds and a separate normalized-kernel response estimate.

It does not make the following source gaps disappear.

### 6.1 The printed unmarked expansion is not a theorem for arbitrary local coupling arrays

CMP116 Section 1 localizes its specified fluctuation effective action using the nonlinear minimizing equations and generalized random walks. Section 2 then proves the Gaussian majorants and polymer estimates for those localized potentials. The source \(\tau\beta s(U_p)\) has a quadratic part of order \(\tau\), rather than the small \(O(g)\) bulk interaction. For a single distinguished root, smallness of the root is not needed for the rooted quotient, but its quadratic form must be charged to an explicit Gaussian reserve. Simply replacing the homogeneous coupling by a spatial array in a theorem statement does not verify that reserve or preserve the source's counterterm construction.

CMP119 pp.277–278, (3.44)–(3.47), explicitly constructs the numerator/denominator cancellation for the stated action-response insertion. Its claim that its root factor satisfies the needed bound concerns that insertion. The full physical scalar, complete current records and raw retained-coordinate support still have to be connected to that root estimate.

### 6.2 Positivity only proves the real-center source window

Theorem LC.2 permits complex \(\tau\) but keeps the underlying links and conditional probability real. It is not an assertion of positivity or zero-freeness after all complex propagator decouplings. Lemma LC.4 gives a sufficient quantitative replacement and shows that an exponential-in-carrier normalization loss is potentially affordable. That actual loss has not been proved on every required family.

### 6.3 The fixed residual component remains in the same baseline

If the conditional integral contains normalized fixed-component operations and the full boundary exponential, they remain in both integrals in (LC.3). Differentiating the actual source family differentiates its marked numerator with those factors present. No independent Gaussian baseline or deletion of a history scalar is allowed.

The LFR II relative norm excludes the interiors of certain fixed residual components from its tree cost. The specified M-03 norm includes every raw retained dependency inside them. The derivative in (LC.4) changes neither fact. Thus (LC.31) must be proved for the actual physical carrier, including those interiors, or replaced by a sharper supported cancellation. An outer rare-component probability does not pay an ambient pointwise source estimate.

### 6.4 Selector interfaces and the ambient version are separate

The source family uses the chosen source-independent kernel. Its derivative in \(\tau\) cannot repair a jump of that kernel as a function of retained data. The default-version obstruction in [support analysis](support_analysis.md) therefore still applies. A buffered extension must be recorded and its own current estimated. The source estimates in this note hold on the specified active real chart and on any extension for which their displayed moment/score hypotheses have actually been verified.

### 6.5 A previous transported scalar is not automatically a native plaquette source

Equations (LC.2) and (LC.9) are verified for the actual native incoming scalar. For an already transported \(F_k\), its exact specified source is \(e^{\tau h^4F_k}\); replacing it by a new native plaquette source would change the left side of M-04. An induction can use this method if its incoming source vertices have an explicit fluctuation estimate of the form (LC.9), or a stated more general analytic source budget. Proving that budget propagates is part of M-07, not a consequence of (LC.4).

## 7. Precise advance and remaining task

The new proved result is the adaptive zero-free source disk

\[
 |\tau|\le
 \frac{c}{|\alpha|(1+\sqrt{E_0(v)})}
\]

for the **same actual positive clean regular conditional integral**, with exact scalar derivative, factorial connected same-root coefficients and separate kernel-current bounds. This sharpens the earlier real moment statement into a normalized complex-source theorem. The radius is sufficient for the energy grading: its inverse grows only as the square root of the retained background energy.

To complete M-04 through this route, the remaining central step is an actual supported complex-decoupling estimate such as (LC.29)–(LC.31), together with the corresponding complete retained-score/current bounds, on the entire full-history density and full native ambient versions. Once those are proved with the spatial slack (LC.32), the rooted quotient and scalar extraction can be applied to the same transported mark. The present note proves the source analytic window and its quantitative conversions; it does not assert the missing physical localization.

## 8. A stronger first-clean route: put the localized defect into the original unmarked expansion

The complex-measure criterion in Section 5 is sufficient, but need not be established as a separate normalized-measure theorem. At the first clean step, the root can instead be inserted into the very action class used in CMP116. This section gives that argument in detail. It uses the new raw-coarse root localization in [local extension kernel](local_extension_kernel.md), Sections 1–3. The resulting statement concerns a fixed first-clean geometry on its buffered native graph. Ambient inactive extensions and changes to an active history are separate obligations.

### 8.1 The actual source and the exact Taylor rows

Write \(n(Y)\) for the number of fixed source blocks in a connected localization carrier \(Y\), and \(\operatorname{foot}Y\) for its complete raw retained-coordinate footprint. All fixed corridors, constraint readouts and plaquette stencils are included. The first-step lift is \(U_0=Q^fV\), not the nonlocal minimizing field considered as an independent coordinate.

On complex link charts the Wilson polynomial is continued as \(\mathsf s(P)=N-\tfrac12\operatorname{Tr}(P+P^{-1})\). It agrees with \(s(P)\) on the compact real group. The symbol \(\operatorname{ReTr}\) is never differentiated as if it were holomorphic.

The force estimate and component decoupling in [local extension kernel](local_extension_kernel.md) give

\[
 h^4F(U(z,V))=\sum_{Y\ni x} f_Y(z,V),
 \qquad a_Y\le Cb e^{-\nu n(Y)},                     \tag{LC.33}
\]

where the sum is the source's real fundamental-theorem-of-calculus localization. Every \(f_Y\) depends only on variables in \(\operatorname{foot}Y\). On the enlarged decoupling polydiscs it has the bounds

\[
\begin{split}
 |f_Y(0,V)|&\le a_Y E_Y(V),\\
 |f_Y(z,V)-f_Y(0,V)|
 &\le a_Y\{\sqrt{E_Y(V)}\,\|z_Y\|+\|z_Y\|^2\},\qquad
 E_Y(V)=1+\sum_{p\subset\operatorname{foot}Y}\beta s(V_p).
\end{split}                                                    \tag{LC.34}
\]

A fixed polynomial in \(n(Y)\) may be moved into \(a_Y\) by consuming any fixed spare part of \(\nu\). The same estimate holds on a fixed, smaller one-coordinate complex disc in a normalized retained direction, with the real-center energy on the right multiplied by a fixed constant. This follows by Taylor expansion around the real compact retained configuration: a normalized retained increment has physical size \(O(g)\), and \(\beta g^2\) is fixed. The radius is chosen inside the variational and current buffer, not across a selector discontinuity.

Here is a coefficient version of (LC.34), which is what the unmarked action proof needs. Put \(c_Y(V)=f_Y(0,V)\), and use Taylor's formula in the actual independent fluctuation coordinates:

\[
 f_Y(z,V)-c_Y(V)
 =\sum_i\ell_{Y,i}(V)z_i+
   \sum_{i,j}z_i v_{Y,ij}(gz,V)z_j.                    \tag{LC.35}
\]

This is an exact identity, not a quadratic approximation. The coefficients are

\[
 \ell_{Y,i}=\partial_{z_i}f_Y(0,V),\qquad
 v_{Y,ij}(gz,V)=\int_0^1(1-t)\partial_{z_i}\partial_{z_j}f_Y(tz,V)\,dt.
                                                               \tag{LC.36}
\]

Let \(d_Y\le C_{\rm coord}(1+n(Y))\) be the number of actual independent real coordinates in the enlarged root carrier. On the smaller fixed physical fluctuation tube,

\[
 \sum_i|\ell_{Y,i}|
 \le Ca_Yd_Y\sqrt{E_Y(V)},\qquad
 \sum_{i,j}\sup|v_{Y,ij}|\le Ca_Yd_Y^2.                \tag{LC.37}
\]

**Justification of the uniform second row.** Before taking a localization derivative, the microscopic reconstruction has the form \(U_e=\exp(i\Theta_e(gz,V))U_{0,e}\), with all derivatives of \(\Theta_e\) with respect to its physical argument bounded on the fixed tube. A normalized fluctuation derivative supplies a factor \(g\). Two such derivatives of \(\beta\mathsf s(U_p)\) therefore have coefficient \(\beta g^2=O(1)\). The chain-rule term with a second derivative of the reconstruction has the same factor, multiplied by a bounded Wilson first derivative. It is not omitted. The first derivative at \(z=0\) is bounded by \(\beta g\) times the background plaquette defect. The force-resolved comparison of the background with \(Q^fV\) bounds this by \(C\sqrt{E_Y}\). A component Cauchy derivative supplies the factor \(e^{-\nu n(Y)}\) in both rows. Summing the finitely many coordinate indices in a component costs a polynomial in its block count. These observations prove (LC.37). In particular, a bound \(O(g^{-1})\) on the first row is unnecessary.

The coefficient argument is needed: an upper bound on the numerical value of a function on the real contour, without its analytic tube and its exact reconstruction, would not prove (LC.37).

### 8.2 A root source can use an adaptive radius without changing the kernel

For one fixed \(Y\), insert the exact factor

\[
 \exp\{\tau[f_Y(z,V)-c_Y(V)]\}                        \tag{LC.38}
\]

in the original source-free conditional integral. Its Gaussian, current slots, nonlinear coordinates, independent-variable cutoffs, coarea terms and normalization factors are unchanged. The native unmarked normal form is the already critical-cancelled one. At a decoupled value of the parameters it is not replaced by the Wilson action evaluated at a new purported stationary point.

Fix a source decay parameter \(\lambda>0\), measured per source block and large enough to fit the localized-action class, and define at the real retained center

\[
 A_Y=Ca_Y(1+d_Y)^2(1+\sqrt{E_Y(V)}),\qquad
 \rho_Y=\frac{r_*e^{-\lambda n(Y)}}{A_Y}.              \tag{LC.39}
\]

When \(a_Y=0\), the source is absent. On \(|\tau|\le2\rho_Y\), both the linear row and quadratic row in (LC.35), including their supported matrix-element sums, are bounded by \(2r_*e^{-\lambda n(Y)}\). These are the quantities entering the Gaussian reserve. The possibly large deterministic constant \(c_Y\) has been extracted exactly and is restored as \(\tau c_Y\) in the logarithm.

The elementary linear-growth extension of the source proof can be made explicit. Normalize a linear row as \(L_Y(z)=\epsilon_Y\widehat L_Y(z)\), \(\sum_i|\widehat\ell_i|\le1\). For an auxiliary complex amplitude \(|\zeta|\le\delta\),

\[
 |\zeta\widehat L_Y(z)|
 \le a\sum_{i\in Y}|z_i|^2+\frac{\delta^2}{4a}.        \tag{LC.40}
\]

Choose \(a\) to be a fixed part of the available positive quadratic reserve. Choose \(\delta\) so that its scalar cost fits the original scalar slack. Since \(e^{\zeta\widehat L_Y}-1\) vanishes at \(\zeta=0\), Cauchy's formula yields the actual small Mayer factor \(2|\epsilon_Y|/\delta\) for \(|\epsilon_Y|\le\delta/2\), multiplied by the boundary Gaussian majorant. The same argument for a quadratic row uses

\[
 |\zeta z^{\mathsf T}\widehat v(gz)z|
 \le\delta\sum_{i\in Y}|z_i|^2
\]

after normalizing its absolute coefficient sum. Thus the source contributes a small localized Mayer vertex; it is not bounded by the supremum of \(|z|\) on the cutoff support. Independent auxiliary amplitudes handle products of source vertices, and their summed Gaussian costs are finite because of their exponentially weighted coefficient bound. For a single distinguished root there is only one such carrier species.

There is a useful trace refinement of these reserve bounds. If \(\sum_i|\widehat\ell_i|\le1\), put \(P_\ell=\operatorname{diag}(|\widehat\ell_i|)\). Weighted Cauchy–Schwarz gives \(|\widehat L_Y(z)|\le(z^{\mathsf T}P_\ell z)^{1/2}\), so (LC.40) holds with \(\sum_i|z_i|^2\) replaced by \(z^{\mathsf T}P_\ell z\), and \(\operatorname{Tr}P_\ell\le1\). Similarly, put \(q_{ij}=\sup|\widehat v_{ij}|\) and \(P_q(i,i)=\tfrac12\sum_j(q_{ij}+q_{ji})\). Then

\[
 |z^{\mathsf T}\widehat v(gz)z|\le z^{\mathsf T}P_qz,
 \qquad \|P_q\|\le\operatorname{Tr}P_q=\sum_{i,j}q_{ij}\le1.
\]

The Gaussian exponential price of either normalized root is therefore a bounded trace cost, independent of the ambient rank. The explicit coordinate factor \((1+d_Y)^2\) was already paid in (LC.39). The source does not introduce an additional hidden exponential in \(E_Y\) or in the total lattice volume. The existing conditioning determinant's exponential in the localization volume is still paid by the declared rate allowances.

This is precisely the extra estimate needed in CMP116 (2.18)–(2.26). The source consumes a fixed additional fraction of \(\alpha_4\), while leaving a fixed positive precision in (2.23). Its bounded scalar allowance is paid before (2.28). Choose \(r_*\) below the finitely many strict reserve and extracted-activity inequalities. These choices are independent of \(g\), total volume and \(E_Y\); all energy dependence has entered the radius (LC.39).

The physical cutoff and the interaction budget must be kept distinct here. At the CMP119 first step the actual free cutoff is \(P(g)=\delta_0(g)/g\), with \(P(g)\to\infty\). Adding a fixed small source coefficient does not replace this cutoff by a different one. The failed-cutoff estimate remains \(\exp[-cP(g)^2]\), with a smaller fixed \(c>0\) after the source reserve is used. This still tends to zero and meets the source's finite smallness inequalities for sufficiently small \(g\). The proof does not require pretending that the added coefficient is \(O(\delta_0(g))\).

The relevant rates have different units and must be compared explicitly. Suppose

\[
 |\operatorname{foot}Y|+t(\operatorname{foot}Y)
 \le C_{\rm geo}n(Y)+C_0,
 \qquad \#\{Y\ni x:n(Y)=n\}\le C_0A_{\rm an}^n.
                                                               \tag{LC.39a}
\]

If the source-species norm is specified with a physical-footprint rate \(\lambda_{\rm phys}\), choose the block rate \(\lambda\) at least \(C_{\rm geo}\lambda_{\rm phys}\), plus the fixed native conversion and incidence allowances. A sufficient margin for the later raw M-03 weight is

\[
 \nu-\lambda>
 \log A_{\rm an}+\kappa C_{\rm geo}+\delta,\qquad \delta>0.
                                                               \tag{LC.39b}
\]

Fixed polynomial trace and direction counts use part of \(\delta\). The native parameters are selected in this order: leave a strict source localization margin, choose the decoupling exponent large enough for (LC.39b), choose its block buffer sufficiently large for the source random-walk inequalities, and then choose a positive raw \(\kappa\) below the resulting geometric ceiling. This is not a claim for arbitrary \(\kappa\) at a fixed source block size. Any factor \(e^{c n(Y)}\) from incidence or the determinant comparison is included in \(\lambda\); none is silently treated as a polynomial.

### Lemma LC.5 — stability of the actual native cluster proof under one localized Wilson defect

On the first-clean buffered native graph, suppose the source-free coefficient and propagator localizations are those of CMP116, with their complete raw pullbacks through \(Q^fV\) as described in [local extension kernel](local_extension_kernel.md), Sections 1–3. Let \(f_Y\) be the actual coefficient in (LC.33). Then the integral with the added factor (LC.38) has the same convergent connected expansion on \(|\tau|<2\rho_Y\). It is nonzero there. Its logarithmic difference from \(\tau=0\) is represented by connected terms whose carriers contain \(\operatorname{foot}Y\), and differentiating this expansion at zero gives the exact conditional mean of \(f_Y-c_Y\).

The assertion is about an **already proved unmarked expansion with one newly checked input species**, not an assumption that its marked numerator has a finite norm.

**Proof.** Equations (LC.35)–(LC.40) check the localized-action bounds for the added species on the same fluctuation analyticity domains. The added constants, linear coefficients and quadratic coefficients satisfy the source's separate scalar, Gaussian-reserve and small Mayer-factor bounds. Apply the unchanged Mayer expansion, conditioning on the full union of supports, failed-cutoff expansion and covariance-square-root localization in CMP116 (2.1)–(2.9). The added carrier is present in the initial conditioning region. The absolute Gaussian comparison (2.15)–(2.26) therefore applies with the reserve slightly reduced. The summations (2.27)–(2.38) and the connected logarithm (2.12)–(2.13) converge with the same strict decay margin. Their exponential equals the original integral with (LC.38), so nonvanishing is a conclusion.

In the difference from zero source, every connected diagram contains a source vertex. Its carrier contains \(Y\) because the entire declared dependency footprint of that vertex was included before conditioning. The marked Mayer estimate above supplies its small factor, so the source difference estimate is uniform even when the source-free interaction tends to zero. In particular no division by the unmarked smallness parameter is used. Uniform convergence on a spare source circle permits termwise differentiation. Differentiating the original integral and subtracting its source-free logarithm gives the normalized conditional mean. \(\square\)

### 8.3 The absolute one-root estimate and its precise source-free premise

Here is how Lemma LC.5 pays the absolute root sum, rather than merely its final conditional value. Give the source-free connected expansion a decay margin larger than the desired output rate. The convergent marked-Mayer majorant at the source circle gives, for a fixed \(Y\),

\[
 \sum_{Z\supset Y} e^{\kappa_0 n(Z)}
       \sum_{\gamma\in\Gamma(Z;Y)}
       |\Phi_{\gamma;Y}(\tau,V)|
 \le C r_* e^{-\lambda' n(Y)},\qquad |\tau|\le\rho_Y,\tag{LC.41}
\]

with a fixed \(\lambda'>0\) after paying the root's incidence and carrier weights. Here \(\gamma\) records the individual Mayer, failed-cutoff, conditioning and connected-cluster choices. The summands have at least one source factor, so each vanishes at zero source. One can avoid optimizing \(\lambda'\): dropping the factor on the right still suffices when \(\nu\) has the extra \(\lambda\) reserve. The majorant is uniform on the source circle and is summed **before** the complex tagged summands are combined into a carrier coefficient.

More precisely, the proof produces nonnegative tagged majorants \(M_{\gamma;Y}\), independent of the retained center, with

\[
 \sup_{V\in\mathcal D_Z}\sup_{|\tau|\le\rho_Y(V)}
 |\Phi_{\gamma;Y}(\tau,V)|\le M_{\gamma;Y},\qquad
 \sum_{Z\supset Y}e^{\kappa_0n(Z)}
       \sum_{\gamma\in\Gamma(Z;Y)}M_{\gamma;Y}
 \le Cr_*e^{-\lambda'n(Y)}.                          \tag{LC.41a}
\]

This follows because each source row is bounded by the same \(2r_*e^{-\lambda n(Y)}\), and every other bound used for a tagged term is the source-free uniform coefficient bound. It is stronger than a bound for the sum at a single retained point and justifies the sums of local suprema below. Termwise Cauchy now yields

\[
 \sum_{Z\supset Y}e^{\kappa_0 n(Z)}
 \sum_{\gamma\in\Gamma(Z;Y)}
 |\partial_\tau\Phi_{\gamma;Y}(0,V)|
 \le C a_Y(1+d_Y)^2(1+\sqrt{E_Y(V)})
                e^{\lambda n(Y)}.                   \tag{LC.42}
\]

Restore the exact scalar term \(c_Y\), whose carrier is already \(Y\). Since \(Y\subset Z\), \(E_Y\le E_Z\), and \(1+\sqrt{E_Z}\le2E_Z\). If \(\nu-\lambda\) exceeds the connected-carrier entropy and the desired raw-footprint weight, summation over \(Y\ni x\) gives

\[
 \sum_{Z\ni x}e^{\kappa_0 n(Z)}
 \sup_{V\in\mathcal D_Z}
 \frac{|h^4 A_Z(V)|}{E_Z(V)}\le Cb.                  \tag{LC.43}
\]

Here \(\mathcal D_Z\) is the actual buffered native domain of that coefficient. The norm contains a supremum over the local domain; it does not use the average probability of the clean sector. Rooted diagrams may be organized before quotienting as the marked \(H'_Z\) of CMP119 (3.44), and then resummed by exactly its (3.45)–(3.47), or organized as source derivatives of the connected logarithm. They give the same conditional mark, because (LC.38) perturbs the numerator and denominator through the same original conditional integral. The connected logarithm automatically cancels every component disjoint from the root.

There is also a direct Gaussian check on the cost in (LC.42). For each individual tag, (LC.34) multiplies the exact joint Gaussian majorant of CMP116 (2.23). The finite-rank insertion inequality in [actual kernel](actual_kernel.md), G1–G3, costs only \(C(E_Y+|Y|)\) times that tag's existing Gaussian mass. The determinant comparison is not paid twice. This proves that the source proof has not hidden an \(e^{CE_Y}\), a factor \(P(g)^2\), or an ambient-rank loss.

**What the premise means.** The source-free premise in Lemma LC.5 is substantive but strictly upstream of M-04's marked root. It is the full native localization of the actual precision, complete non-Gaussian action and covariance-square-root conditioning, as functions of the raw retained data. The primitive first-step lift and variational equations identify these objects, whereas arbitrary inherited E/B/R operations do not follow from that identification. If the full source-free raw pullback has not yet been verified for a proposed kernel extension, (LC.43) is available only on the native graph where the original construction supplies it. It must not be promoted to an ambient assertion by calling the premise a marked norm budget.

## 9. Separate direct and kernel currents by using two retained copies

The source method gives separate records without a cancellation between them. Fix the first-clean geometry and its independent fluctuation space. Introduce independent retained arguments \(v_{\rm ins}\) and \(v_{\rm ker}\), and define

\[
 \mathcal L_Y(\tau;v_{\rm ins},v_{\rm ker})
 =\log\int q_{v_{\rm ker}}(dz)
       e^{\tau[f_Y(z,v_{\rm ins})-c_Y(v_{\rm ins})]}.
                                                               \tag{LC.44}
\]

All source-free normalizers are in \(q_{v_{\rm ker}}\). The mark reconstruction alone uses \(v_{\rm ins}\). At the diagonal, the derivative in \(\tau\), plus \(c_Y\), is the transported localized scalar. A derivative in the first retained argument gives

\[
 B_{Y,d}=q_v\partial_d f_Y,                            \tag{LC.45}
\]

and a derivative in the second gives

\[
 J_{Y,d}=\operatorname{Cov}_{q_v}(f_Y,\partial_dL_v).   \tag{LC.46}
\]

Thus the exact normalizer response is retained in \(J\). The constant row has zero kernel current.

The native action proof and the defect estimate hold uniformly when either retained copy varies in a fixed smaller normalized one-coordinate complex disc. The physical size of that disc is \(O(g)\), inside the fixed geometric variational buffer. On the mark disc the real-center energy changes by only a fixed additive constant per affected local stencil. On the kernel disc the complete already critical-cancelled action, covariance and coarea factors use their native analytic continuations. The radius (LC.39) is fixed using the real center and is not differentiated.

Apply independent Cauchy formulas to the source circle and either retained circle **before** summing their absolute majorants. This gives the same estimate as (LC.42) for each separate record, up to a fixed factor. A derivative vanishes unless its raw coordinate is in the complete output carrier. On the first-clean graph there are at most \(C n(Z)\) continuous raw-coordinate directions on that carrier, including the fixed Lie-algebra multiplicity. Summing them costs only a polynomial, paid by another strictly positive piece of the localization margin. Consequently (LC.43) holds with

\[
 |A_Z|\quad\hbox{replaced by}\quad
 |A_Z|+\sum_d\bigl(|B_{Z,d}|+|J_{Z,d}|\bigr),          \tag{LC.47}
\]

using the appropriate direct and kernel coefficients of the connected expansion. No estimate of the derivative of their sum is substituted for (LC.47).

For a finite normalized link displacement, use the **specified endpoint decomposition** required by M.30, rather than integrating both infinitesimal records along the diagonal. Write \(v_t=\tau_{d,t}v\) and

\[
 H(v_{\rm ins},v_{\rm ker})=q_{v_{\rm ker}}f_Y(\cdot,v_{\rm ins}).
\]

With no incoming old current, the actual records are

\[
 B_{Y,d,t}=\frac{H(v_t,v_t)-H(v,v_t)}{t},\qquad
 J_{Y,d,t}=\frac{H(v,v_t)-H(v,v)}{t}.                 \tag{LC.47a}
\]

Their sum is exactly \([H(v_t,v_t)-H(v,v)]/t\). Bound the first difference by a path in the insertion copy with the kernel fixed at \(v_t\), and the second by a path in the kernel copy with the insertion fixed at \(v\). The independent-copy majorants prove each bound separately. Apply this decomposition to each represented carrier coefficient; it retains the exact incoming-current convention and its support. On these paths the energy is bounded by a fixed multiple of the M-03 shifted regulator, since

\[
 \beta s(e^{tT/\sqrt{1+\beta}}P)
 \le 2\beta s(P)+C t^2,\qquad |t|\le1.               \tag{LC.48}
\]

There are a fixed number of affected plaquettes for one elementary direction. Thus the continuous finite-difference records obey the M-03 value grade \(1\) and current grade \(3/2\), with room to spare: the displayed bound grows only like one local energy. This argument does not assign a derivative to a jump at a history or selector interface.

### Theorem LC.6 — the first-clean scalar on the buffered native graph

Fix the original first globally regular Wilson step on a periodic lattice, with no previously created effective activities, no fixed residual components and no exterior boundary force. Fix the native blocking and localization parameters with the strict margins used above. Keep the exact source-free independent variables, constraint map, soft gauge factor, Haar/coarea terms and the CMP119 free cutoff. Let

\[
 F_h=\alpha\beta_0h^{-4}\sum_{p\in S}a_p s(U_p)-c,
 \qquad b=|\alpha|+h^4|c|,
\]

where \(S\) is the prescribed fixed microscopic scalar stencil and the fixed \(a_p\) and trace convention are included in the constants. Suppose the first-step coupling ratio \(\beta_0/\beta_1\) lies in a stated fixed compact interval of positive numbers. Choose a positive target raw-carrier rate \(\kappa\) for which (LC.39b) holds.

Then the **actual** conditional value \(QF_h\), restricted to the buffered native first-clean graph, has a representation by raw-supported connected carriers and separate direct and normalized-kernel current records. For every sufficiently small admitted coupling,

\[
 (Lh)^4\sum_{Z\ni x}e^{\kappa(|Z|+t(Z))}
 \left[
  \sup_{\mathcal D_Z}\frac{|A_Z|}{\widehat R_Z}
  +\sup_{\mathcal D_Z}\sum_d
    \frac{|B_{Z,d}|+|J_{Z,d}|}{\widehat R_Z^{3/2}}
 \right]
 \le C L^4 b.                                       \tag{LC.50}
\]

The direction records in this formula are infinitesimal native continuous directions at active data, or finite normalized displacements with **both endpoints active** and with complete paths lying in the stated analytic buffer. Take the corresponding supremum over allowed displacement sizes in each direction. \(Z\) includes every raw dependency of its coefficient and direction. The regulator is the actual first-step output regulator; the coupling-ratio assumption compares its \(\beta_1s(V_p)\) to the \(\beta_0s(V_p)\) used in (LC.34). The constant is independent of the coupling and total volume.

The regular normalized integral has a native continuation on the analytic buffer after its common retained coarse selector has canceled. That continuation is used to estimate derivatives and paths. It agrees with the original conditional kernel at the active endpoints. It is not asserted to equal the M.1 point-mass convention at an inactive endpoint. Thus (LC.50) does not contradict the default-version jump proved in [support analysis](support_analysis.md).

If, in addition, the original outer blocked Wilson law has the first-scale energy-moment reserve (LC.49), the same representation satisfies the averaged value/current estimates with grades \(1\) and \(3/2\), using the unnormalized restriction to the clean event. This additional conclusion does not condition the outer law on an event whose probability may vanish with volume.

**Verification of the source-free inputs at this first step.** The map \(Q^fV\) is the local raw lift printed in CMP119 (1.3), and is the first-step reference specified in CMP102, p.280, after (11)/(14). CMP119 p.249, (1.14)–(1.17), eliminates the distinguished coordinate \(b_0(c)\) using the two adjacent blocks. Thus its linear embedding and exact nonlinear constraint solve are local at fixed background. The Wilson, soft gauge, Haar and coarea vertices are local analytic functions of these maps, the actual background and its actual current. They contain no inherited E/B/R vertices at this step.

The constrained reference precision, including the current-dependent constraint Hessian, has a uniform positive gap by [first step precision gap](first_step_precision_gap.md), PG.1–PG.5. Its true raw-supported resolvent and covariance square root are supplied by [physical carrier resolvent](physical_carrier_resolvent.md), PR.1 and PR.13. The nonlinear correction from the lift to the minimum is the force-resolved fixed point localized in [local extension kernel](local_extension_kernel.md), Sections 1–3. The component decoupling applies to each of the preceding local analytic vertices. On the source's enlarged domains it gives the required coefficient smallness for the precision correction and the full nonlinear action, and genuine raw retained support when all decouplers outside a component vanish. At the first step the nonlinear Wilson and Jacobian budgets tend to zero with \(gP(g)^3\) and \(g^2P(g)^2\), up to the fixed source constants; \(P(g)\) is polylogarithmic. A normalized one-coordinate retained disc of fixed radius has physical radius \(O(g)\), so it fits the common native buffer for \(P(g)\gg1\). These are unmarked source facts and the explicit positive-gap/resolvent calculations, rather than the marked conclusion (LC.50).

**Proof.** The verified source-free inputs permit Lemma LC.5. Equations (LC.33)–(LC.37) verify its new input for this exact microscopic scalar. Use the uniform tagged majorants (LC.41a), source Cauchy (LC.42), and the separate retained-copy Cauchy formulas (LC.44)–(LC.47). Their coefficients are supported in the physical carriers because every input is localized before conditioning and because multiplication only unions overlapping carriers. The rate inequality (LC.39b) sums the root choices, physical weights and polynomial coordinate counts. Equations (LC.47a)–(LC.48) pass from native derivatives to the exact specified-endpoint finite-difference records of M.30. The two separate records sum to the exact finite difference of the represented value by the displayed two-copy telescoping identity. This proves (LC.50), with the displayed scale conversion. For the averaged assertion, apply (LC.49) to the same nonnegative regulator majorants and spend a further fixed piece of the remaining decay on \(|Z|\); \(p\le p^{3/2}\) pays the current grade for \(p\ge1\). \(\square\)

The theorem is a first-step, fixed-geometry continuous-carrier theorem. It is not the full augmented-state M-03 theorem. In particular, its \(\mathcal D_Z\) supremum is not the ambient product supremum of the M-03 statement, and its set of directions does not include changing an active retained history to another active geometry.

If a smooth local cutoff \(\eta_X\) is used in a positive kernel extension, it destroys holomorphy in raw retained variables. The extended derivative must therefore be taken termwise as

\[
 D(\eta_X a_X)=\eta_XDa_X+(D\eta_X)a_X.
\]

Only \(Da_X\) is bounded by native Cauchy. The explicit collar bound must control \(D\eta_X\), with its actual carrier. The same rule applies to the extended precision and Gaussian normalizer, and to the reconstructed old state. Extending (LC.50) by applying an unmodified raw-variable Cauchy formula to \(\eta_Xa_X\) would be invalid.

## 10. What this adds to the first-clean proof, and what remains outside it

Sections 8–9 provide the missing **marked-input calculation** for the first-clean native expansion. The scalar defect is an actual new linear/quadratic species admitted by the source's Gaussian proof. Its adaptive source radius is explicit. The source-free unmarked construction is kept fixed. The entire connected scalar and its separate continuous direct/kernel records follow from the same expansion, and the sole cost beyond the unmarked summation is paid by the already available root decay. This avoids assuming a uniform complex source disk on a normalized, globally decoupled probability law.

Theorem LC.6 combines the first-step raw pullback, precision gap, absolute resolvent and scalar source calculation into a theorem on the buffered native graph. Its verification paragraph identifies all unmarked first-step ingredients. This native result requires neither an all-history marked estimate as an assumption nor a new source-dependent saddle or cutoff. The extension of the same source-free budget to an ambient kernel, and then to general histories, is separate.

For an **ambient** M-03 theorem, one must additionally use a recorded source-independent positive kernel and reconstruction extension and verify the same source-free carrier estimates for it. The local Gram extension in that companion note is designed for this purpose. A coefficientwise extension of the already integrated scalar would not meet the recursive kernel convention. Neither the present native result nor a continuous extension on one fixed geometry controls replacements of an active history by a different geometry.

For the averaged part of M-03, the exact first-step raw averaging inequality in [M07 Regulator Repair](../F_analytic_families/M07_Regulator_Repair.md) supplies

\[
 \left\|1_{\rm clean}\sum_{p\subset X}\beta_1 s(V_p)\right\|_{L^p}
 \le C_L |X|p                                         \tag{LC.49}
\]

under the original blocked Wilson law, provided the exposed first-step coupling ratio is bounded. The indicator is essential: the exact raw readout used in this estimate is verified on the first globally regular branch. The formula does not assert the same readout on other retained geometries. It is an unnormalized-sector estimate and does not divide by the probability that the whole torus is clean. Together with the absolute carrier estimates it pays the restricted averaged value and continuous-current grades. The scale conversion contributes \((Lh)^4/h^4=L^4\); no claim of a depth-independent iteration is made.

Finally, a bounded scalar/identity projector can be applied to these same supported outputs, as proved in [scalar extraction](scalar_extraction.md). The M-04 statement fixes the incoming F-01 basis but does not prescribe a unique projector for a general transported output. The finite-pulse projector below therefore meets its algebraic extraction requirement on any domain where the needed operator bound has been proved. F-01's separated measurements fix the normalization of the basis; they are not an additional definition of this projector. Identification with any more specific downstream coefficient prescription is a separate matter. The source calculation does not permit substituting a fresh coarse plaquette for an already transported scalar at a later step. The full M-04 statement, with arbitrary histories, fixed residual components and all ambient currents, remains outside the proved native first-clean calculation.

### Corollary LC.7 — an explicit bounded projection of this same first-clean output

Let \(h'=Lh\), let \(\varphi_{h'}=\beta_1\sigma_{h'}\) be the exact F-01 scalar energy representative, and let \(v_0,v_1\) be the identity and one-link pulse of [scalar extraction](scalar_extraction.md), (SE.2), on the current coarse lattice. For any fixed \(0<t\le1/4\), both belong to the first-clean active domain for all sufficiently small admitted coupling: the normalized pulse is \(O(g)\), whereas the native coarse test allows \(g\) times a diverging polylogarithm. Their energy difference is the explicitly nonzero number

\[
 d(\beta_1,t)=h'^4\varphi_{h'}(v_1)
 \ge\sqrt{3/2}\,t^2/8.                               \tag{LC.51}
\]

Let \(\mathcal H_x\) be the finite group of signed coordinate permutations fixing the insertion anchor. Translate this group and the pulse together with that anchor and the original block convention. If a color-invariant evaluation functional is desired, also average the pulse over compact global color conjugations; its scalar denominator is unchanged. For each output coefficient supplied by LC.6, set

\[
 c_Z=A_Z(v_0),\qquad
 a_Z=\frac{h'^4\left[|\mathcal H_x|^{-1}
        \sum_{r\in\mathcal H_x}A_Z(rv_1)-A_Z(v_0)\right]}
          {d(\beta_1,t)},
 \qquad \mathcal R_Z=A_Z-c_Z-a_Z\varphi_{h'}.          \tag{LC.52}
\]

Subtract \(a_Z\delta\varphi_{h'}\) from its direct record, and leave its kernel current unchanged. Enlarge the carrier by the fixed scalar stencil. The two probe regulators are uniformly bounded because only a fixed number of raw coarse plaquettes is excited, even after one further elementary shift. The primitive scalar and its direct differences have the same local energy budget. Therefore the proof of (SE.11), now with \(r=0\), gives

\[
 QF_h=a\varphi_{h'}+c_{\rm out}+\mathcal R,\qquad
 |a|+h'^4|c_{\rm out}|+
 \|\mathcal R\|_{\rm native,\kappa}
 \le C L^4 b.                                       \tag{LC.53}
\]

The norm here is precisely the restricted value/continuous-record norm of LC.6; its averaged part uses the same additional first-scale moment reserve. The equalities use the transported output \(QF_h\), not a newly inserted coarse field. The remainder vanishes at the identity probe and has zero averaged pulse readout. All its old and new current bookkeeping is retained. Averaging does not enlarge the scalar's fixed stencil and does not increase the norm bound. This projection intertwines the signed-permutation action. Translating the full input/step geometry and insertion anchor gives the same coefficient, so a translation-covariant clean operator has a spacetime-constant scalar coefficient. No additional fine-translation symmetry of a fixed blocking offset is assumed.

If the fixed incoming F-01 scalar normalization is \(z_S^{\rm in}\ne0\), rewrite the scalar term as

\[
 a\varphi_{h'}
 =\left(a\frac{\beta_1}{z_S^{\rm in}}\right)
       z_S^{\rm in}\sigma_{h'}.                      \tag{LC.54}
\]

This exposes the exact conversion to the fixed incoming basis and uses no final running normalization. When the incoming physical centering and energy reserve give \(b\le C|z_S^{\rm in}|/\beta_0\), its coefficient is bounded by \(CL^4\beta_1/\beta_0\). Without that incoming reserve the displayed \(b\beta_1/|z_S^{\rm in}|\) is retained explicitly.

This is a bounded **choice of projection** onto the already fixed scalar and identity directions. It completes the algebraic extraction requested by M-04 on the domain of LC.6. The M-04 statement imposes no further Taylor or separated-measurement projector. If a downstream F-03/Gamma calculation imposes such an additional coefficient prescription, its relation to this choice must be checked there; that is not an additional M-04 requirement.

## 11. An explicit flat first-clean identity coefficient

The Gaussian part also gives a finite coefficient that can be calculated without a formal continuum limit. In this section \(\mathbb E_G\) denotes the **untruncated** normalized flat Gaussian on the actual independent free-coordinate space. The original truncated conditional law is compared to it only in (LC.58). Let \(n_f\) and \(n_c=n_f/L^4\) be the numbers of fine and coarse sites on the periodic first-step lattice, and put \(d_G=N^2-1\). At the flat retained configuration, let \(Q\) be the actual linearized coarse averaging operation. Its exact local right inverse implies that it has rank \(4n_cd_G\). Hence

\[
 \dim\ker Q=4(n_f-n_c)d_G.                            \tag{LC.55}
\]

The center-fixed infinitesimal gauge transformations \(d\phi\), with \(\phi=0\) at coarse centers, form a subspace of dimension \((n_f-n_c)d_G\). They are in \(\ker Q\) and in the kernel of the Wilson quadratic form. There are no additional Wilson zero modes in the constrained quotient: PG.1 in [first step precision gap](first_step_precision_gap.md) eliminates them after the actual soft gauge coordinate is fixed.

The symmetrized source gauge coordinate obeys \(\tau_{\rm av}d\phi=\phi\) for such center-fixed \(\phi\). Every \(a\in\ker Q\) therefore decomposes uniquely as

\[
 a=a_\perp+d\phi,\qquad \tau_{\rm av}a_\perp=0,
 \qquad \phi=\tau_{\rm av}a.
\]

The flat Wilson quadratic form depends only on \(a_\perp\), and the soft gauge quadratic form depends only on \(\phi\). Their Jacobian is a fixed nonzero constant and cancels on normalization. Thus the untruncated flat Gaussian law factorizes in these coordinates, and the physical quadratic action has rank

\[
 d_{\rm phys}=3(n_f-n_c)d_G.
\]

### Proposition LC.8 — the flat constrained Gaussian coefficient

With the exact source convention for \(\beta\), so that its Wilson density is \(e^{-\beta S}\),

\[
 \mathbb E_G[\beta S^{(2)}]
 =\tfrac12d_{\rm phys}
 =\tfrac32(n_f-n_c)(N^2-1).                          \tag{LC.56}
\]

**Proof.** In the physical quotient write the exponent as \(\tfrac12x^{\mathsf T}K_Wx\), with \(K_W>0\). Its normalized Gaussian covariance is \(K_W^{-1}\), so the expectation is \(\tfrac12\operatorname{Tr}(K_WK_W^{-1})\). The gauge integral cancels and contributes no Wilson action. The dimension computed above proves the formula. \(\square\)

Because the coarse constraint is tied to its block centers, this does not imply the same coefficient at every fine site. Average over one complete \(L\)-block instead:

\[
 \overline\sigma_h(B)=L^{-4}\sum_{x\in B}\sigma_h(x).
\]

Translation by a coarse block preserves the flat conditional Gaussian. The exact F-01 scalar sum then gives

\[
 h^4\mathbb E_G[\beta\overline\sigma_h(B)]
 =\sqrt{\frac32}\,(1-L^{-4})(N^2-1).                \tag{LC.57}
\]

This coefficient is strictly positive for \(L>1\). It is an identity contribution generated by actual fluctuating physical directions, not a scalar renormalization coefficient.

The same native rooted expansion used in LC.5 gives the corresponding first-clean asymptotic with a volume-independent error. At \(V=I\), the minimizing field is exactly identity, the leading precision is the flat one, and the constraint map is \(gC_0z+O(g^2z^2)\). Split the comparison into three exact differences: the expectation of the exact root minus its quadratic root under the actual conditional law; the interaction change for that quadratic root at the fixed original cutoff; and removal of that cutoff from the Gaussian expectation.

For the first difference, the root Taylor remainder has a quadratic-growth coefficient \(O(gP(g))\). For the second, the complete interaction coefficient bounds tend to zero, with the sufficient bound \(C[gP(g)^3+g^2P(g)^2]\). For the third, the local failed-cutoff expansion gives a species of size \(Ce^{-cP(g)^2}\). The quadratic root can supply an additional fixed polynomial, such as \(P(g)^2\), to a failed-cutoff moment; it is absorbed by decreasing the fixed positive tail exponent \(c\). The product cutoff is not required to factor in the physical/gauge direct sum used for (LC.56).

In each normalized marked difference every surviving connected diagram has at least one corresponding root, interaction or cutoff difference vertex; disconnected vacuum components cancel. The same tagged summation therefore yields

\[
 \left|h^4Q_I[\beta\overline\sigma_h(B)]
    -\sqrt{\frac32}(1-L^{-4})(N^2-1)\right|
 \le C\{gP(g)^3+g^2P(g)^2+e^{-cP(g)^2}\}=o(1).       \tag{LC.58}
\]

The constants are independent of total volume. This uses the complete first-clean normalized integral and its original cutoff, not a global comparison of that integral with an untruncated Gaussian partition function. For \(F_h=\alpha\beta\sigma_h-c\), the block-averaged flat identity readout is consequently \(\alpha\) times (LC.57), minus \(h^4c\), with the error in (LC.58) multiplied by \(|\alpha|\). In output units \(h'=Lh\),

\[
 h'^4 Q_I\overline F_h(B)
 =\alpha\sqrt{\frac32}(L^4-1)(N^2-1)-h'^4c
   +O\!\left(L^4|\alpha|
      [gP^3+g^2P^2+e^{-c_0P^2}]\right).             \tag{LC.59}
\]

Here \(c_0>0\) is the Gaussian tail constant, distinct from the original identity coefficient \(c\). No claim about the separated physical normalization system, full running normalization or a later history follows from this coefficient.
