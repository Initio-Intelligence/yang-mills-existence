# The sign of the first placement term of the Wilson scalar

Use the original periodic \(SU(N)\) Wilson measure with \(\beta\sum_p s_p\), \(s_p=N-\Re\operatorname{Tr}U_p\), and the specified four-vertex scalar \(V_x=a^4w_a(x)\). Write \(X_x=\beta(V_x-\langle V_x\rangle)\), \(d_A=N^2-1\). On the compatible weak tori of Annex O §22, fix \(\epsilon=10^{-6}\), \(l=L^{\lfloor\epsilon\log_L\beta\rfloor}\mid n\), even \(n\ge3l\), and its uniform local moment reserve. For every integer \(R\to\infty\) with \(R\le\beta^{\epsilon/100}\),
\[
 R^{14}\kappa_3(X_0,X_{Re_0},X_{3Re_0})
 =-\frac{49d_A}{1944\pi^6}
 +O_{N,L}\!\left(R^{-2}+R^{14}[\beta^{-\epsilon/6}+R/l]\right). \tag{1}
\]
The error tends to zero throughout that window. The corresponding closed-cube scalar has the opposite leading coefficient. Section 3 below proves a strictly negative result also on the explicit disjoint zero-mean scalar profiles used for the perturbative target. These are single-copy cumulants with the ordinary unconditioned exterior. Their engineering-scaled size is \(R^{-2}\). Finite-cutoff six-plaquette comparison, (1) · Placement identity, (12) · Target, §23 (298)–(304)

## 1. Isolating the order \(R^{-2}\) term by duality

Use the infinite discrete Gaussian curl comparator in the orthonormal color-contraction convention of Annex O. Write \(K(x)=\pi^{-2}|x|^{-4}\Lambda^2(I-2xx^\top/|x|^2)\). For plaquettes with their actual oriented midpoints a displacement \(r\) apart, the scalar color covariance has entries
\[
 P_{\alpha\delta}(r)=K_{\alpha\delta}(r)+D_{\alpha\delta}(r)+O(|r|^{-8}),
 \qquad |\partial^jD(r)|\le C_j|r|^{-6-j}.                       \tag{2}
\]
Here \(D\) is a smooth, degree \(-6\) kernel off the origin. To verify its existence, in midpoint coordinates the symbol of \(P\) is the two-form projection onto \(\hat k\wedge\mathbb R^4\), where \(\hat k_j=2\sin(k_j/2)\). Expand this rational angular symbol at zero as its homogeneous terms of degrees zero and two plus a remainder whose order-\(j\) derivatives are \(O_j(|k|^{4-j})\). The increment two follows from the odd sine and the even squared denominator. Fourier transforming the cut-off homogeneous terms gives \(K,D\) off the origin up to rapidly decreasing errors. Indeed away from zero in position the inverse transforms are smooth, by integration by parts, and homogeneous by distributional scaling of the original locally integrable symbols. After \(B>8\) integrations by parts the dyadic remainder at frequency \(h\) is bounded by \(C_Bh^8(1+h|r|)^{-B}\). For the periodic smooth complement use the anchored symbol with its phases intact before integrating by parts; only the near-zero part has been converted to midpoint displacements. Equation (2) holds on the actual allowed midpoint sublattices. It does not extend the periodic multiplier past the Brillouin zone by dropping half-link phases. No explicit evaluation of \(D\) is required.

Take three lattice sites \(x_i=Ru_i\) in a compact separated region of the rescaled variables. For \(V_{x_i}\), conditional on its orientation \(\alpha=\{\mu,\nu\}\), the plaquette-square midpoint has four equally weighted displacements \((\pm e_\mu\pm e_\nu)/2\) from \(x_i\). For the closed-cube placement \(C_{x_i}\) the analogous displacements from \(x_i+h,\ h=(1/2,1/2,1/2,1/2)\), use the two complementary axes. Only *relative* midpoints enter the triangle; the common \(h\) drops out. In either placement the two Wick legs at each insertion share the same displacement, and the three displacement averages are independent. Write \(H_b=\Lambda^2(I-2e_be_b^\top)\) for \(b=0,1,2,3\), and define
\[
 T_{i,b}(u)=\operatorname{tr}\!\left[
 H_b K(u_i-u_j)K(u_j-u_k)K(u_k-u_i)\right],                    \tag{3}
\]
where \(i,j,k\) are cyclic. The reversed cycle gives the same trace after transposition since each continuum covariance is symmetric.

In the difference of the two Gaussian triples, the order-\(R^{-14}\) contributions obtained by replacing just one \(K\) by \(D\) are identical before displacements. The remaining displacement error on these contributions is \(O(R^{-16})\), since the first moments vanish and (2) controls two derivatives. Two \(D\)'s or one covariance remainder also contribute only at \(O(R^{-16})\). For the three \(K\)'s the second Taylor term at site \(i\) in the vertex-minus-cube difference is
\[
 \tfrac18\left(\sum_{b\in\alpha}\partial_{i,b}^2
                      -\sum_{b\notin\alpha}\partial_{i,b}^2\right)
\]
in lattice units. All odd total terms vanish by simultaneous inversion of the centered offsets; the fourth-order remainder is \(O(R^{-16})\). Orientation summation of the coefficient at each \(b\) inserts the diagonal matrix \(-H_b\), whose entries are \(+1\) on planes containing \(b\) and \(-1\) otherwise. The trace factor of the half-quadratic scalar is \(d_A\), including both oriented Wick cycles. the corresponding estimate (12) proves the *entire* cube triple equals minus the vertex triple at these separated vertices. Dividing the difference by two gives
\[
 \kappa_3^G(X_{x_1},X_{x_2},X_{x_3})
   =R^{-14}\mathcal D(u)+O(R^{-16}),\qquad
 \mathcal D(u)=-\frac{d_A}{16}\sum_{i=1}^3\sum_{b=0}^3
                           \partial_{i,b}^2T_{i,b}(u).            \tag{4}
\]
The centered zeroth-order scalar triangle is identically zero by Hodge parity. Equation (4) identifies the leading term surviving that cancellation; its derivation uses the second midpoint moments of the actual plaquette squares.

## 2. Evaluation on the time axis

Let \(u_i=t_i e_0\), and set \(k=\prod_{i<j}|t_i-t_j|^{-4}\). At a fixed site \(i\) write \(A=(t_i-t_j)^{-1}, B=(t_i-t_k)^{-1}\). Temporal displacement keeps \(T_{i,0}=6\pi^{-6} k\), so its second temporal derivative is \(\pi^{-6} k[96(A+B)^2+24(A^2+B^2)]\).

For any spatial \(b\), move site \(i\) by \(v e_b\). The three reflection normals lie in the \(0b\) plane, and the product of their three reflections is a single reflection with normal \(n(v)\) there. Its normal angle is the first edge angle minus the second plus the third, modulo \(\pi\) (composition of three plane reflections). The middle edge stays temporal. Thus \(n_b(v)^2=v^2(A+B)^2+O(v^4)\). The exterior-square trace of the product with the \(b\)-normal reflection is \(8n_b(v)^2-2\): their product in the vector representation is a plane rotation and two fixed directions, with exterior-square trace \(2+4\cos(2\angle(e_b,n))\). The common scalar distance factor changes by \(k[1-2(A^2+B^2)v^2+O(v^4)]\). This gives \(\partial_{i,b}^2 T_{i,b}=\pi^{-6} k[16(A+B)^2+8(A^2+B^2)]\). Adding the three spatial directions and the temporal one, (4) yields
\[
 \frac{\pi^6}{d_A}\mathcal D(t_1e_0,t_2e_0,t_3e_0)
   =-24\,k\sum_{i<j}(t_i-t_j)^{-2}.                              \tag{5}
\]
Here \(\sum_i[(t_i-t_j)(t_i-t_k)]^{-1}=0\) for three distinct numbers. At \(t=(0,1,3)\), \(k=1/1296\) and the inverse-square sum is \(49/36\). The compact Wilson six-leg estimate of the corresponding estimate gives an absolute error \(O(\beta^{-\epsilon/6}+R/l)\) per lattice triple on the fixed rescaled compact. This proves (1), including the absence of any change in exterior measure. At \(R=\lfloor\beta^{\epsilon/100}\rfloor\) its total rescaled error is \(O(\beta^{-\epsilon/50})\).

## 3. The prescribed separated signed profiles

Let \(v_1=0,v_2=e_0,v_3=3e_0\), and \(f_i=-\partial_0\eta_\sigma(\cdot-v_i)\), where \(\eta\ge0\) is smooth of unit integral supported on the unit ball and \(\sigma=10^{-24}\), as in the corresponding estimate §3. Then
\[
 R^2\kappa_3\left(\sum_x f_i(x/R)X_x:\,1\le i\le3\right)
 = \int\mathcal D(u)\prod_i f_i(u_i)\,du+
 O_f\!\left(R^{-2}+R^{14}[\beta^{-\epsilon/6}+R/l]\right).        \tag{6}
\]
The number of tuples costs \(O_f(R^{12})\). Their empirical average of the smooth, compactly supported \(\mathcal D\prod f_i\) differs from its integral by \(O_f(R^{-2})\) using centered unit-cell quadrature in the rescaled variables. The lattice centering in \(X\) is exact. One may additionally impose \(aR\to0\) if a shrinking physical length is desired.

The coefficient of (6) has the opposite sign to the perturbative benchmark on these same profiles:
\[
 \left|\frac{\pi^6}{d_A}\int\mathcal D\prod_i f_i
                     +\frac{1715}{729}\right|<10^{-3}.            \tag{7}
\]
For a short verification of its number, (5) is \(-24\sum_{e}\prod_{a<b}|t_a-t_b|^{-p_{ab}}\), where for each distinguished pair \(e\) its exponent is 6 and the other two exponents are 4. For one such product \(g\) set \(l_i=-\sum_{j\ne i}p_{ij}/(t_i-t_j)\), \(l_{ij}=-p_{ij}/(t_i-t_j)^2\). Its mixed derivative is \(g(l_1l_2l_3+l_{12}l_3+l_{13}l_2+l_{23}l_1)\). At \((0,1,3)\) summing the three products and multiplying by \(-24\) gives \(-1715/729\).

For the explicit width in (7), use the same complex coordinate radii \(1/64\) as in the corresponding estimate §3 about any points on the three lobes. The normalized traces \(\pi^6T_{i,b}\) have modulus at most \(10^6\) there: \(|v\cdot v|\ge0.8\,|t_{ij}|^2\) for each complex separation, and each normalized reflection kernel has norm below 40. Formula (4) and Cauchy's estimate bound the fourth derivative of \(\pi^6\mathcal D/d_A\) by \((12/16)\,6!\,64^6\,10^6\). Three integrations by parts replace \(\prod f_i\) by \(\prod\eta_\sigma\) against the mixed third time derivative. Displacing the twelve real coordinates by at most \(\sigma\) changes that derivative by less than \(10^{-3}\). This proves (7). For comparison, the same mixed derivative of the physical benchmark shape \(k\) is \(+25/729\) by §23 (303). No coincidence or contact terms occur on these lobes.

**Scope of the obstruction.** The ordinary cube and vertex Gaussian placement difference is twice the term in (4), including its sign. On the stated Wilson window their difference has the same nonzero leading term up to the displayed absolute six-leg error. Consequently replacing the vertex by the parity average of the two triples costs a *sharp* order \(R^{-2}\) in engineering-scaled units even on the stipulated separated test. With the tree-level comparison \(g_{\rm bare}^2=2N/\beta\), this greatly exceeds \(g_{\rm bare}^2\) throughout the controlled window. More generally suppressing this particular placement term below a proposed canonical first interacting coefficient of size \(g_\rho^2\) requires \(R^{-2}=o(g_\rho^2)\) when comparing these coefficients without an explicit subtraction. Subtracting \(\mathcal D/R^2\) from the engineering-scaled vertex measurement improves its Gaussian placement remainder to \(O(R^{-4})\); the compact thermal comparison term still costs \(O_f(R^{12}[\beta^{-\epsilon/6}+R/l])\). These estimates do not identify \(g_\rho\) on the target trajectory or compare the remaining signal to \(o(g_\rho^2)\). They give a signed cutoff effect in the unmodified observable, consistent with a different sign after taking the continuum limit first. U-01 and U-02 remain open.

## 4. The corresponding two-point term in the same scalar

The two-point function on the same window has a nonzero *common* vertex and cube mesh correction. In lattice units, for integer \(R\to\infty\),
\[
 R^{10}\left\{\kappa_2(X_0,X_{Re_0})
                   -\frac{3d_A}{\pi^4 R^8}\right\}
 =\frac{48d_A}{\pi^4}
   +O_{N,L}\!\left(R^{-2}+R^{10}\beta^{-\epsilon/6}\right).       \tag{8}
\]
Here Annex O (O.33) gives the absolute compact error for the individual Wilson plaquette pairs in the finite stencil sum. In particular (8) does not use the three-stencil bad-offset cost.

To compute the intrinsic projection correction, let \(G\) denote the scalar Green function of the infinite lattice with symbol \(1/\sum\hat k_i^2\), and set \(\delta_0^2G(r)=G((r+1)e_0)-2G(re_0)+G((r-1)e_0)\). At integer temporal separation \(r>0\), symmetry of the three spatial directions and \(\sum_\mu\delta_\mu^2G=0\) give
\[
 P_{12,12}(re_0)=\tfrac23\delta_0^2G(r).
\]
Indeed the magnetic numerator is \(\hat k_1^2+\hat k_2^2\). The complementary electric entry is its negative at nonzero separation since the two diagonal Fourier numerators add to \(\sum\hat k_i^2\). Near zero the Green symbol begins with \(|k|^{-2}+\sum k_i^4/(12|k|^4)\). In four dimensions these terms transform off the origin to \(1/(4\pi^2|x|^2)\) and \(-\sum_i\partial_i^4\log |x|/(96\pi^2)\), since the inverse transform of the finite part of \(|k|^{-4}\) is \(-\log |x|/(8\pi^2)\) up to a constant. On the time axis each of the four fourth derivatives is \(-6/r^4\). Keeping one more homogeneous term of degree two in the symbol, the same shell proof as (2) gives \(G(re_0)=(r^{-2}+r^{-4})/(4\pi^2)+c\,r^{-6}+O(r^{-8})\). Its second difference is controlled to the required order. Thus the magnetic diagonal curl entry is \((r^{-4}+5r^{-6})/\pi^2+O(r^{-8})\). At coalesced offsets \(K\) is diagonal on the time axis, so in \(\tfrac{d_A}2\sum_{\alpha,\delta}P_{\alpha\delta}^2\) the \(K D\) interference contributes \(30d_A/(\pi^4 r^{10})\).

For the midpoint displacement of the pair at one site, use \(\sum_\delta K_{\alpha\delta}(x)^2=1/(\pi^4|x|^8)\) for every \(\alpha\), by orthogonality. Its vertex average contributes \(\tfrac{d_A}{2\pi^4}\tfrac38\Delta |x|^{-8}\) per site because exactly three orientations contain each coordinate direction. The same count holds for the cube complementary directions. Both sites together give \(18d_A/(\pi^4r^{10})\), using \(\Delta |x|^{-8}=48|x|^{-10}\) off zero in four dimensions. Odd displacement terms vanish and the next two-point remainder has order \(r^{-12}\). The coefficients \(30+18=48\) yield (8). This positive correction to the canonical two-point comparison does not supply the logarithmic normalization or physical field matching of U-01.

For example, use (1) and (8) for the three pair separations \(R,2R,3R\) (fixed multiples do not affect the window estimates). Their covariances are eventually positive. Writing \(X_i=X_{t_iRe_0}\) with \(t=(0,1,3)\), the **ordinary one-sector field** has
\[
 R^2\,\frac{\kappa_3(X_1,X_2,X_3)}
 {\sqrt{\kappa_2(X_1,X_2)\kappa_2(X_2,X_3)\kappa_2(X_3,X_1)}}
 \longrightarrow -\frac{98}{9\sqrt{3d_A}}.                       \tag{9}
\]
Indeed the pair products restore the common factor \(\pi^{-6}k\) and supply \((3d_A)^{3/2}\). Every common positive scalar multiplier cancels at each finite cutoff, including the measured scalar-channel factor when it is defined. This supplies a sign and rate for the *same* scalar diagnostic as the corresponding estimate (5) on the controlled weak window, independently of the unknown scalar multiplicative normalization. The running coupling and the order of the two limiting operations remain essential for the physical test.
