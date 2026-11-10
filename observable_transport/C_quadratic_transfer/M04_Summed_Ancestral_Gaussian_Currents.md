# Summed terminal responses of an actual birth Gaussian event

This note strengthens the single-direction real Gaussian consequence AP.33. It proves a sum over all terminal bond/Lie directions, with the actual birth marginal rank and the factor \(g_NL^{-(N-b)}\). The proof uses the source's one analytic map of the entire terminal array. It does not sum separate operator-norm estimates and does not assume locality of a field-dependent gauge transformation.

The scope is the centered, untruncated Gaussian coefficient of the homogeneous admitted source problem. Its precision includes the constraint-force terms and the actual averaged soft gauge. Fixed product balls or annuli in full Lie fibers are allowed as insertions. Moving Q centers, interacting densities, noninvariant marks, conditional exterior means, physical-carrier current norms and the canonical finite-rectangle interface remain outside this theorem.

## 1. Source setting and one common tangent map

Thus \(h_j=L^j\eta\), \(N\ge b+1\), the birth free list \(\mathcal F_b\) is fixed, and the actual terminal minimum is \(F=U_N(V_N)\). All geometry is homogeneous. The source native tube has a fixed buffer.

The matrix
\[
 K=K_b^{\rm rel}(F)
 \tag{SG.1}
\]
is the complete precision AP.8 in dimensionless birth coordinates: physical birth angle \(g_bz\), action normalization \(g_b^{-2}\). In particular it retains both the earlier force correction in CMP99 (3.127)--(3.138) and the next-constraint force term in (3.156). Its soft coefficient is the derivative of the full nonlinear averaged variable, as in AP.5--11 and CMP109 (0.11), (2.5). It is not an absolute soft Hessian evaluated at a noncanonical field. AP proves
\[
 mI\le K\le MI
\]
and the uniform holomorphic bound in the two-sided exponentially weighted matrix norm
\[
 \|H\|_\rho=
 \max\left\{\sup_e\sum_f e^{\rho d_b(e,f)}\|H_{ef}\|,
             \sup_f\sum_e e^{\rho d_b(e,f)}\|H_{ef}\|\right\}.
 \tag{SG.2}
\]
All constants below may depend on the fixed group, dimension, \(L\), the source fixed block parameters and the fixed weak-coupling ceiling, but not on the volume, \(b,N\), or \(\eta/h_b\).

Choose an orthonormal real Lie basis. Let \(v=(v_d)\) be an arbitrary real terminal bond/Lie array and put
\[
 V_N(tv)(c)=
  \exp\!\left(ig_Nt\sum_\alpha v_{c,\alpha}T_\alpha\right)V_N(c).
 \tag{SG.3}
\]
The finite-dimensional coordinate sup norm of \(v\) and the supremum of its per-bond Lie norms differ only by a fixed group constant.

CMP102, printed pp.305--309, (172)--(180) and Proposition 9, constructs one analytic relative Landau solution for the entire small array, not independent gauge choices for individual bonds:
\[
 U_N(V_N(tv))^{u(tv)}
       =\exp[i\eta A(tv)]F,\qquad A(0)=0.
 \tag{SG.4}
\]
The derivative \(v\mapsto \dot A[v]\) is therefore a single real linear map. Applying the functional-derivative estimate (190), printed p.308, to an arbitrary bounded array gives
\[
 \|\dot A[v]\|_\infty\le Cg_Nh_N^{-1}\|v\|_\infty,\qquad
 \|\nabla_F\dot A[v]\|_\infty
       \le Cg_Nh_N^{-2}\|v\|_\infty,
\]
\[
 \|D_F^*D_F\dot A[v]\|_\infty
       \le Cg_Nh_N^{-3}\|v\|_\infty.
 \tag{SG.5}
\]
Here the functional kernel includes \(h_N^{-4}\); the coarse cell measure in its action cancels this factor, and the exponential kernel has a uniformly bounded row integral on the homogeneous terminal lattice. The same statement also follows by differentiating the full sup-norm array tube in (172)--(177), with its source regularity norms. Arbitrary bounded sign arrays are admissible infinitesimal directions in this buffered tube. No spatial smoothness of the terminal array is being imposed.

In the birth regularity norm AP.12 this yields
\[
 \|\dot A[v]\|_{\mathcal R_b(F)}
       \le Cg_NL^{-(N-b)}\|v\|_\infty.
 \tag{SG.6}
\]
The gradient and second-order entries have the stronger factors \(L^{-2(N-b)}\) and \(L^{-3(N-b)}\). Combining this with the Banach-valued derivative bound of AP.1 gives, for
\[
 K^{\rm cov}(tv)=K_b^{\rm rel}(\exp[i\eta A(tv)]F),\qquad
 {\cal L}v=\left.\frac{d}{dt}K^{\rm cov}(tv)\right|_{t=0},
\]
\[
 \|{\cal L}v\|_\rho
       \le C\delta_N\|v\|_\infty,\qquad
 \delta_N=g_NL^{-(N-b)}.
 \tag{SG.7}
\]
This is an operator estimate from the whole terminal \(\ell^\infty\) array space. It is stronger than the list of single-bond bounds AP.31.

The analytic precision input in this step is already source-specific: CMP99 Theorem 3.4, the force-corrected series (3.130), (3.138), and the unit-lattice estimate (3.132), together with the fixed-\(L\) constraint and averaged-gauge maps in AP.1. Thus (SG.7) does not identify small plaquette curvature with a precision estimate without controlling the latter.

## 2. Entrywise duality and positive envelopes

For the unit terminal coordinate \(e_d\), put \(E_d={\cal L}e_d\). Each \(E_d\) is real self-adjoint. Fix two birth bonds \(e,f\) and two Lie components \(\alpha,\beta\). The coordinate functional
\[
 v\longmapsto ({\cal L}v)_{e\alpha,f\beta}
\]
is real linear. Choosing each \(v_d\) to be the sign of the corresponding coefficient, and using (SG.7), gives the exact finite-dimensional duality estimate
\[
 \sum_d |(E_d)_{e\alpha,f\beta}|
       \le C\delta_N e^{-\rho d_b(e,f)}.
 \tag{SG.8}
\]
The sign array may be chosen separately for each matrix entry; that is sufficient because the array estimate is uniform over all such choices. Summing the fixed number of Lie components gives
\[
 \sum_d\|(E_d)_{ef}\|
       \le C\delta_N e^{-\rho d_b(e,f)}.
 \tag{SG.9}
\]
In particular, for every \(0<\rho'<\rho\), the matrix with entries
\(\sum_d\|(E_d)_{ef}\|\) has two-sided weighted Schur norm at rate \(\rho'\) at most \(C_{\rho-\rho'}\delta_N\). The loss of rate pays the birth-lattice sum. There is no sum of the separate norms \(\|E_d\|_\rho\).

For a useful positive formulation set
\[
 r_d(e)=\sum_f\|(E_d)_{ef}\|,\qquad
 D_d=\operatorname{diag}_{e\in\mathcal F_b}
                        [r_d(e)I_{\mathfrak g}].
 \tag{SG.10}
\]
Self-adjointness makes the block norm envelope symmetric. The inequality
\(2ab\le a^2+b^2\) then gives, as quadratic forms,
\[
 -D_d\le E_d\le D_d,\qquad
 D_d\ge0,\qquad
 \sum_dD_d\le C\delta_N I.
 \tag{SG.11}
\]
This is the positive domination needed below. It does not require simultaneous diagonalization of the \(E_d\).

## 3. One fixed birth marginal

Let \(I\subset\mathcal F_b\) be any fixed set of birth bonds, retaining every Lie component at each chosen bond. Let \(P_I\) be restriction, \(r_I=|I|\dim\mathfrak g\), and
\[
 \Sigma=P_IK^{-1}P_I^*.
 \tag{SG.12}
\]
The same covariance supplies the marginal's inverse and determinant. For each terminal direction in the common frame,
\[
 \dot\Sigma_d=-P_IK^{-1}E_dK^{-1}P_I^*.
\]
Define
\[
 R=K^{-1}P_I^*\Sigma^{-1/2},\qquad
 T_d=\Sigma^{-1/2}\dot\Sigma_d\Sigma^{-1/2}=-R^*E_dR.
 \tag{SG.13}
\]
Since \(R^*KR=I\), the gap implies \(R^*R\le m^{-1}I\). Therefore
\[
 -A_d\le T_d\le A_d,\qquad
 A_d=R^*D_dR\ge0,\qquad
 \sum_dA_d\le C\delta_N I.
 \tag{SG.14}
\]
It follows that
\[
 \sum_d\|T_d\|_1\le C r_I\delta_N,\qquad
 \sum_d|w^*T_dw|\le C\delta_N|w|^2
 \quad\hbox{for every }w\in\mathbb R^{r_I}.
 \tag{SG.15}
\]
For the trace-norm assertion, if \(-A\le T\le A\) and \(A\ge0\), the positive and negative spectral projections of \(T\) give \(\operatorname{Tr}|T|\le\operatorname{Tr}A\). Summing (SG.14) proves the first inequality. The second follows directly from the quadratic form domination. In particular, no decay estimate for \(\Sigma^{-1}\), and no rank bound for the whole birth lattice, was assumed.

## 4. Actual invariant-domain current

Let \(D_I\) be a fixed measurable product of adjoint-invariant norm balls or annuli in these full Lie fibers. Its centered Gaussian probability is unchanged by every pointwise adjoint transport on the birth free list. AP.9--11 transports the exact constraint subspace, its exceptional solve and the full relative averaged sampler. Thus for every sufficiently small real terminal array, the Gaussian event computed from the actual canonical source precision equals the event computed in (SG.4)'s relative Landau frame.

This equality is the reason its actual derivative may be computed from \(T_d\). There is no assertion that the field-dependent gauge has local raw dependence, nor that its derivative has already been bounded. Its contribution cancels for this particular invariant event.

Write \(p=p_\Sigma\) and \(w=\Sigma^{-1/2}x\). The normalized marginal score is
\[
 \partial_d p(x)
 =\frac12\left[w^*T_dw-\operatorname{Tr}T_d\right]p(x).
 \tag{SG.16}
\]
The Gaussian gap and upper bound justify differentiation on any fixed measurable \(D_I\), including hard annuli, by dominated convergence. Equations (SG.15)--(SG.16) prove the following theorem.

### Theorem SG.1

At every real homogeneous admitted terminal datum in the buffered tube,
\[
 \boxed{\quad
 \sum_d\left|\partial_d\Pr_{\rm actual}(D_I)\right|
 \le Cg_NL^{-(N-b)}
       \int_{D_I}\left(r_I+|\Sigma^{-1/2}x|^2\right)
                         p_\Sigma(x)\,dx .
 \quad}
 \tag{SG.17}
\]
The sum includes all normalized terminal bond/Lie directions. The constants are independent of terminal volume and birth age. The right side retains a positive Gaussian tail integral; no rare probability is divided out. Any subsequent Gaussian tail estimate spends the reserve in this same integral once.

The statement is pointwise in the retained datum, with its sum over directions taken there. It is not a claim about a sum of independent retained-data suprema, a carrier representation, or finite endpoint rectangles. Those stronger interfaces require their own common envelopes.

## 5. Summability over available ancestor endpoints

For any actually available finite admitted chain, the coupling bound CMP119 printed p.255, (2.6), gives
\[
 \frac{g_N}{g_b}\le C\sqrt{1+N-b}.
\]
Consequently
\[
 \sum_{N=b+1}^{N_{\max}}\delta_N
 \le C_L g_b\sum_{a\ge1}\sqrt{1+a}L^{-a}
 \le C_Lg_b .
 \tag{SG.18}
\]
This estimate does not assert existence of an infinite admitted chain or a lower beta-function speed.

There is also a useful formulation with one born reference measure. Use AP.19's composed birth transports, \(K_*=\widehat K_{b+1}\), \(\Sigma_*=P_IK_*^{-1}P_I^*\), and \(E_*(x)=|\Sigma_*^{-1/2}x|^2\). AP.26--27 gives, on the same weak ceiling,
\[
 p_{\Sigma_N}(x)\le
       e^{Cr_I\epsilon_b+C\epsilon_bE_*(x)}p_{\Sigma_*}(x),
 \qquad
 |\Sigma_N^{-1/2}x|^2\le C E_*(x).
\]
The invariant domains allow these composed transports without changing their probabilities or these energy integrals. Applying (SG.17) and then (SG.18) gives
\[
 \sum_{N=b+1}^{N_{\max}}\sum_{d\ {\rm at}\ N}
       |\partial_d\Pr_N(D_I)|
 \le C_L g_b\,e^{Cr_I\epsilon_b}
       \int_{D_I}(r_I+E_*(x))e^{C\epsilon_bE_*(x)}
                                     p_{\Sigma_*}(x)\,dx .
 \tag{SG.19}
\]
These are the separate terminal responses of the indicated primitive Gaussian events at the available ancestor endpoints. Equation (SG.19) is not a derivative formula for a product of RG transitions. It spends the one real AP Gaussian comparison reserve, rather than a fresh rank/energy tilt at every age.

## 6. Remaining boundary

The new result resolves a summed real response for the actual untruncated primitive precision and invariant fixed birth domains. It does not localize the co-moving gauges as raw cylinder functions. It does not construct the common restriction-consistent complex carrier family required by UD.19/AP Section 7. It does not differentiate moving Q reference centers or prove an interacting conditional-score estimate. A noninvariant mark or a canonical raw-coordinate current would retain the gauge-transport derivative that cancels in (SG.17).

The argument also does not bound forced Gaussian means, assert an all-depth admitted density induction, or extract relevant/vacuum terms. Those tasks remain distinct from the source-specific array estimate and normalized Gaussian matrix calculation proved here.

## Primary references

The whole-array source map and its scale-normalized derivative are in CMP102, printed pp.305--309, (172)--(190) and Proposition 9. AP.1 supplies the complete actual precision tube, citing CMP99 Theorem 3.4 and (3.130)--(3.138), (3.156)--(3.158), with the actual averaged-gauge comparison from CMP109 (0.11), (2.5). CMP99's coefficientwise walk support in Theorem 3.10 and its force-tree discussion on printed pp.416 and 427 would also permit a localized-bump proof; it is not necessary for the simpler whole-array duality argument above. The age estimate uses only CMP119 (2.6), not an additional asymptotic-freedom hypothesis.
