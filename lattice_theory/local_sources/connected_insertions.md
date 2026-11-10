# Hard cutoffs, connected insertions and marginal normalization

## Part I. Weighted covariance and entropy with the actual regular cutoff

### Result and scope

The hard characteristic function in the regular fluctuation integral can be retained exactly. A spatially weighted covariance estimate follows from contraction of normally reflected Langevin dynamics on the product cutoff domain. The estimate is uniform in the cutoff radii, the number of independent bonds, the normalization constant, and a fixed exterior linear source.

Two consequences are established here.

1. The actual constrained, hard-truncated Gaussian carrier has exponential covariance decay for arbitrary observables with localized gradients. Applying the estimate to the full nonlinear minimizing-field Wilson/clover insertion includes all its nonlinear Taylor terms.
2. The same theorem applies to a non-Gaussian regular effective law as soon as the full effective potential has a small exponentially weighted Hessian on the actual cutoff domain. No extension of that potential beyond its analytic domain, no removal of the cutoff, and no tail union over the whole volume are needed.

The independent-coordinate cutoff and the coercive local precision are checked against the printed Balaban papers below. The companion note on the regular effective potential supplies a sufficient Hessian estimate for the admitted full-torus small-field carrier. The corresponding claim for every multiscale history, including all boundary and R terms, still requires the additional analytic-domain estimates stated in Section 7. This note does not replace an old transported insertion by a minimizing-field insertion.

### 1. A weighted covariance theorem on product convex sets

Let \(I\) be a finite set of coordinate blocks. Write

\[
{\cal X}=\bigoplus_{i\in I}{\mathbb R}^{n_i},
\qquad
D=\prod_{i\in I}D_i ,
\tag{HC1}
\]

where each \(D_i\) is a bounded convex body with nonempty interior. Neither smoothness nor strict convexity of its boundary is required. In particular, a ball for a matrix norm on a real Lie algebra is allowed.

Let \(H\) be real and \(C^2\) on a neighborhood of \(\overline D\), and let

\[
\mu(dA)=Z^{-1}{\bf1}_{D}(A)e^{-H(A)}\,dA.
\tag{HC2}
\]

Take a positive block-scalar matrix

\[
W=\operatorname{diag}_{i\in I}(w_i I_{n_i}).
\tag{HC3}
\]

Assume that, throughout \(D\),

\[
\operatorname{Sym}\!\left(W H''(A)W^{-1}\right)
\ \ge\ \lambda_W I,
\qquad \lambda_W>0.
\tag{HC4}
\]

Here \(\operatorname{Sym}K=(K+K^*)/2\), with the real Euclidean adjoint.

#### Theorem HC-W

For \(f,g\in C^1(\overline D)\), and hence by approximation for functions in the corresponding weighted Sobolev space,

\[
\boxed{
|\operatorname{Cov}_{\mu}(f,g)|
\le
\lambda_W^{-1}
\|W\nabla f\|_{L^2(\mu)}
\|W^{-1}\nabla g\|_{L^2(\mu)} .
}
\tag{HC5}
\]

The theorem includes the normalization of the truncated law. Its constant does not contain \(Z^{-1}\), a boundary-to-volume ratio, or a lower bound on the probability of the cutoff event.

#### Proof

Use the normally reflected diffusion on \(\overline D\),

\[
dX_t=\sqrt2\,dB_t-\nabla H(X_t)\,dt-n_t\,dL_t ,
\qquad n_t\in N_D(X_t).
\tag{HC6}
\]

The boundary measure is supported on times when \(X_t\in\partial D\); \(N_D(x)\) is the outward normal cone. Existence and pathwise uniqueness for a convex body with Lipschitz drift, and the identification of its reversible measure as (HC2), are the standard finite-dimensional reflected-diffusion facts imported here. They are stated explicitly in Bubeck–Eldan–Lehec, Section 3.1, using Tanaka's construction. A Lipschitz extension of the drift may be used to construct the process; only its values on \(D\) enter the argument. No convexity or Hessian estimate outside \(D\) is assumed.

**Weighted contraction, including the boundary.** Couple solutions starting at \(a,b\) with the same Brownian motion, and put \(Z_t=X_t^a-X_t^b\). For a product convex set,

\[
N_D(x)=\prod_iN_{D_i}(x_i).
\tag{HC7}
\]

Consequently, whenever \(n\in N_D(x)\) and \(y\in D\),

\[
\langle W^{-2}(x-y),n\rangle
=\sum_iw_i^{-2}\langle x_i-y_i,n_i\rangle\ge0.
\tag{HC8}
\]

Thus both normal-reflection terms in the differential of
\(\|W^{-1}Z_t\|^2\) have the favorable sign. This is where the product domain and the block-scalar weights are used.

The line segment between the two solutions lies in \(D\). Since \(H''\) is symmetric,

\[
\operatorname{Sym}(W^{-1}H''W)
=\operatorname{Sym}(WH''W^{-1}).
\tag{HC9}
\]

The mean-value formula and (HC4) therefore give

\[
\begin{aligned}
\langle W^{-2}(x-y),\nabla H(x)-\nabla H(y)\rangle
&=
\int_0^1
\left\langle
W^{-1}(x-y),
W^{-1}H''(y+s(x-y))W\,W^{-1}(x-y)
\right\rangle ds\\
&\ge\lambda_W\|W^{-1}(x-y)\|^2.
\end{aligned}
\tag{HC10}
\]

The Brownian noises cancel in the difference process, so the ordinary finite-variation chain rule, (HC8), and Grönwall give the pathwise bound

\[
\|W^{-1}(X_t^a-X_t^b)\|
\le e^{-\lambda_Wt}\|W^{-1}(a-b)\|.
\tag{HC11}
\]

The use of normal cones covers corners and nonsmooth norm balls directly.

**Gradient contraction without differentiating the reflection map.** Let \(P_t\) be the transition semigroup. For \(f\in C^1(\overline D)\), apply the fundamental theorem of calculus to \(f\) along the segment joining \(X_t^{a+\epsilon v}\) and \(X_t^a\), and then use (HC11). After division by \(|\epsilon|\) and passage to the limit,

\[
|\partial_v P_tf(a)|
\le
e^{-\lambda_Wt}\|W^{-1}v\|\,
P_t\bigl(\|W\nabla f\|\bigr)(a)
\tag{HC12}
\]

at points where the derivative exists. The semigroup function is Lipschitz by (HC11), so Rademacher's theorem supplies these derivatives almost everywhere. Continuity and boundedness of \(\nabla f\) justify the limit in expectation. Taking the dual norm gives

\[
\|W\nabla P_tf(a)\|
\le
e^{-\lambda_Wt}P_t\bigl(\|W\nabla f\|\bigr)(a).
\tag{HC13}
\]

Jensen's inequality and invariance of \(\mu\) imply

\[
\|W\nabla P_tf\|_{L^2(\mu)}
\le e^{-\lambda_Wt}\|W\nabla f\|_{L^2(\mu)}.
\tag{HC14}
\]

**Covariance identity.** The symmetric Dirichlet form of (HC6) is

\[
{\cal E}(u,v)=\int_D\nabla u\cdot\nabla v\,d\mu.
\tag{HC15}
\]

For the present smooth functions, reversibility yields

\[
-\frac{d}{dt}\int_D(P_tf)g\,d\mu
={\cal E}(P_tf,g).
\tag{HC16}
\]

Contraction on the compact set \(D\) implies \(P_tf\to\mu f\). Integrating (HC16),

\[
\operatorname{Cov}_{\mu}(f,g)
=\int_0^\infty
\int_D
\langle W\nabla P_tf,W^{-1}\nabla g\rangle\,d\mu\,dt.
\tag{HC17}
\]

Use Cauchy–Schwarz and (HC14), and integrate \(e^{-\lambda_Wt}\). This proves (HC5). Smooth-function approximation in the Neumann form domain gives the Sobolev extension. \(\square\)

This argument is also a direct explanation of why an integration-by-parts calculation for an untruncated Gaussian is unnecessary. The boundary is already represented in the dynamics, and its contribution is nonpositive in the correct weighted metric.

### 2. Coercive local precision plus a small interaction

Equip \(I\) with a metric \(d\) having the uniform polynomial growth of the current-unit bond lattice. Let

\[
H(A)=\tfrac12\langle A,MA\rangle+\langle\ell,A\rangle+V(A),
\qquad M=M^*\ge mI.
\tag{HC18}
\]

Assume the blocks of \(M\) have uniform exponential decay. Define

\[
\kappa_M(\alpha)
=\sup_i\sum_j
\bigl(e^{\alpha d(i,j)}-1\bigr)\|M_{ij}\|.
\tag{HC19}
\]

Exponential decay and lattice volume growth imply
\(\kappa_M(\alpha)\to0\) as \(\alpha\downarrow0\), uniformly in the finite volume. For example, if
\(\|M_{ij}\|\le C_Me^{-\nu d(i,j)}\), then
\(\kappa_M(\alpha)\le C\alpha\) for \(0\le\alpha\le\nu/2\).

Suppose

\[
\varepsilon_\alpha:=
\sup_{A\in D}\sup_i\sum_j
e^{\alpha d(i,j)}
\|\nabla_i\nabla_jV(A)\|<\infty.
\tag{HC20}
\]

Choose \(w_i=e^{\alpha\psi(i)}\), where
\(|\psi(i)-\psi(j)|\le d(i,j)\). By the row/column Schur estimate and symmetry of the block Hessians,

\[
\|WMW^{-1}-M\|\le\kappa_M(\alpha),
\qquad
\|WV''(A)W^{-1}\|\le\varepsilon_\alpha.
\tag{HC21}
\]

Therefore (HC4) holds with

\[
\boxed{\lambda_W=m-\kappa_M(\alpha)-\varepsilon_\alpha.}
\tag{HC22}
\]

In particular, \(\kappa_M(\alpha)\le m/4\) and
\(\varepsilon_\alpha\le m/4\) give \(\lambda_W\ge m/2\).

No diagonal-dominance or sign condition on \(M_{ij}\) is required. The linear term \(\ell\), including a term induced by fixing exterior fluctuation variables, has no effect on (HC22).

#### Exponential covariance from localized gradients

Suppose, for two observables centered at current-unit points \(x,y\),

\[
\|\nabla_i f_x\|_{L^2(\mu)}
\le A_xe^{-\gamma d(i,x)},\qquad
\|\nabla_i g_y\|_{L^2(\mu)}
\le A_ye^{-\gamma d(i,y)}.
\tag{HC23}
\]

Take \(\psi(i)=d(i,x)\) and \(0<\alpha<\gamma\). Uniform summability of lattice exponentials and the triangle inequality give

\[
\|W\nabla f_x\|_2\le C_{\gamma-\alpha}A_x,
\quad
\|W^{-1}\nabla g_y\|_2
\le C_{\gamma-\alpha}A_ye^{-\alpha d(x,y)}.
\tag{HC24}
\]

Combining (HC5) and (HC24),

\[
\boxed{
|\operatorname{Cov}_{\mu}(f_x,g_y)|
\le
C_{\gamma-\alpha}^2\lambda_W^{-1}
A_xA_y e^{-\alpha d(x,y)}.
}
\tag{HC25}
\]

Pointwise localized gradient bounds imply (HC23). In particular, no comparison of the truncated and untruncated normalization constants is needed.

### 3. Exact source check: the regular cutoff is on independent bonds

The following statements are taken from CMP119, printed pp.247–249 and 268–270.

* On p.247, equation (1.9) defines the starred set by
  \[
  X^*=X\setminus\{b_0(c):c\in X^{(1)}\}.
  \tag{HC26}
  \]
  Thus the star removes the special dependent bonds used to solve the averaging constraints.
* On p.249, immediately after (1.14), the paper states that the constraint-linearizing transformation changes only the special \(b_0(c)\) bonds; the characteristic function is unchanged. The constraints then express those variables in terms of the remaining variables, written \(A\), through \(A'=CA\).
* The new decomposition (3.16), p.268, uses the supremum of the fluctuation coordinate over the starred bond set \((\square'^{\sim2})^{(k)*}\). Each small-field factor is therefore a product of single-independent-bond norm-ball indicators.
* Page 269 states that on \(\Lambda_{k+1}\), and its enlarged region, only these new small-field characteristic factors remain. Their product is denoted \(\chi^{(k)}(\Lambda_{k+1})\).
* Page 270, (3.23)–(3.25), takes the conditional integral in the fluctuation coordinates on \(\Lambda_{k+1}\), with the remaining coordinates incorporated into the exterior operation.

Overlapping cubes only repeat some of the single-bond inequalities. They do not couple the inequalities. After fixing an admissible exterior and the geometry, the internal domain is

\[
D_Y=\prod_{b\in I_Y}\{A_b\in\mathfrak g:\ |A_b|<r_{k,b}^{\chi}\}.
\tag{HC27}
\]

An exterior factor is either zero or one; conditioning on a nonzero carrier removes it from the internal domain. The radii in (HC27) mean the radii after the source's scaling convention has been applied. Their numerical value is unnecessary for (HC5). In particular, this argument does not confuse a restriction on independent \(A_b\) with a restriction on all \(CA\) bonds or on the nonlinear field \(gCA-hD(gCA)\).

The unnormalized regular part of the conditional density is the one displayed in CMP119 (3.28):

\[
\mathbf1_{D_Y}(A)
\exp\!\left\{
-\tfrac12\langle A,C^*\Delta^{(k)}CA\rangle
+P^{(k)}(g_k,A)
+E_k\!\left(U_k(e^{i[g_kCA-hD(g_kCA)]}V^{(k)})\right)
-E_k(U_{k+1})
\right\}.
\tag{HC28}
\]

Exterior conditioning can also contribute the linear term seen in (3.25). Other boundary/history contributions in the complete decomposition must be included in the potential before applying (HC20) to that complete law.

### 4. Exact source check: the precision itself is local and coercive

Balaban, CMP99, printed p.428, defines

\[
C^{(k)}(\Lambda)
=C(C^*\Delta_k C)^{-1}C^*
\tag{HC29}
\]

in (3.158). Immediately before and after that formula, the paper describes the independent-coordinate embedding \(C\), states a uniform positive lower bound \(\gamma_0\) for \(C^*\Delta_kC\), and uses exponential decay of this precision to obtain exponential decay of its inverse.

This is stronger than knowing only that the covariance decays. It is exactly what (HC19) needs. The source assumptions, including the admitted regular background and its smallness conditions, remain in force. The embedding \(C\) fills a dependent bond using variables in a fixed number of adjacent current-unit blocks, so its finite-range bounds depend on the fixed blocking geometry, not on ultraviolet depth.

For a fixed-exterior conditional Gaussian, the internal precision is a principal compression of the same form. It retains the lower bound \(\gamma_0\) and the exponential kernel bound. Its conditional mean changes through a linear term, which is harmless in (HC18).

Consequently, for sufficiently small fixed \(\alpha>0\),

\[
\kappa_M(\alpha)\le\gamma_0/4,
\qquad
M=C^*\Delta^{(k)}C,
\tag{HC30}
\]

uniformly on this source-admitted family. Theorem HC-W with \(V=0\) proves the hard-truncated Gaussian result on the actual domain (HC27).

### 5. The nonlinear constraint coordinates preserve the response scale

Avoid the notational collision between the physical current scale \(h\) and the source's operator \(h\). In this section denote the latter by \(h_{\rm c}\).

The actual argument of the minimizing field is

\[
B'(A)=g_kCA-h_{\rm c}D(g_kCA).
\tag{HC31}
\]

CMP109, printed pp.267–268, derives this map by solving

\[
D(B)={\cal C}\bigl(B-h_{\rm c}D(B)\bigr),
\tag{HC32}
\]

where \({\cal C}\) is the nonlinear remainder of the local current-scale averaging operation. It starts at degree two. The sparse operator \(h_{\rm c}\) satisfies \(LQh_{\rm c}=I\) and is supported on the special constraint bonds. CMP116 (1.19) repeats (HC31); its preceding localization argument explicitly uses that \(B'\) is a local function of \(B\).

Here is a direct weighted estimate, which also applies if one keeps only exponential locality. For a block kernel \(K\), use the maximum of its exponentially weighted row and column sums, denoted \(\|K\|_\beta\). Fixed-range operators obey an algebra estimate in this norm. On a sufficiently small current-unit sup-norm ball,

\[
\|{\cal C}'(B-h_{\rm c}D(B))\|_\beta
\le C_{\rm geom}\delta,
\qquad
\|h_{\rm c}\|_\beta+\|C\|_\beta\le C_{\rm geom},
\tag{HC33}
\]

where \(\delta\) bounds the argument. The first estimate follows from the quadratic vanishing, the analytic local averaging function, and its bounded number of current-unit inputs.

Differentiating (HC32) gives

\[
D'(B)=
\left(I+{\cal C}'(B-h_{\rm c}D(B))h_{\rm c}\right)^{-1}
{\cal C}'(B-h_{\rm c}D(B)).
\tag{HC34}
\]

For \(C_{\rm geom}^2\delta<1/2\), a Neumann series in the weighted kernel norm yields

\[
\|D'(B)\|_\beta\le C\delta.
\tag{HC35}
\]

Therefore

\[
\begin{aligned}
D_AB'(A)&=g_k\bigl(I-h_{\rm c}D'(g_kCA)\bigr)C,\\
\|D_AB'(A)\|_\beta&\le Cg_k,\\
\|\partial_{A_c}B'_b(A)\|&\le Cg_ke^{-\beta d(b,c)}.
\end{aligned}
\tag{HC36}
\]

The constants are uniform as long as the true cutoff support remains in the source's small analytic domain. This calculation treats only differentiation in the internal fluctuation \(A\). Derivatives of \(C,h_{\rm c},D\), or the minimizing background with respect to retained external fields are a different estimate.

Now use the established nonlinear minimizing-field derivative LR-B from [Minimizing-field response and the two-insertion cluster formula](two_insertion_clusters.md), Part I. For a matrix component of the Wilson/clover insertion,

\[
\left\|
D_{B'}Q^W\!\left(U_k(e^{iB'}V^{(k)});x\right)[b]
\right\|
\le
C\epsilon_{\rm reg}h^{-4}e^{-c d(z_x,b)}.
\tag{HC37}
\]

Here \(h\) is the physical current scale and \(z_x\) the corresponding current-unit position. The bound holds throughout the admitted real domain, including the allowed fluctuation fields. The parameter \(\epsilon_{\rm reg}\) must bound the whole admitted minimizing-field family, not just its zero-fluctuation background.

Define the exact nonlinear function of the independent fluctuation coordinates,

\[
F_x(A)=Q^W\!\left(
U_k(e^{i[g_kCA-h_{\rm c}D(g_kCA)]}V^{(k)});x
\right).
\tag{HC38}
\]

Chain differentiation, (HC36), (HC37), and convolution of lattice exponentials give

\[
\boxed{
\|\nabla_{A_c}F_x(A)\|
\le
Cg_k\epsilon_{\rm reg}h^{-4}e^{-c' d(z_x,c)}.
}
\tag{HC39}
\]

No Taylor truncation of the observable appears in (HC38) or (HC39).

#### Corollary HC-NL: nonlinear covariance with the hard cutoff retained

On the hard-truncated constrained Gaussian carrier just verified,

\[
\boxed{
|\operatorname{Cov}(F_x,F_y)|
\le
Cg_k^2\epsilon_{\rm reg}^2 h^{-8}
e^{-c|x-y|/h}.
}
\tag{HC40}
\]

The covariance is that of the normalized law with the actual indicator. The proof is simply (HC25) with the pointwise amplitudes in (HC39). The same conclusion holds for the regular interacting law if its full effective potential satisfies (HC20) with \(\varepsilon_\alpha\le\gamma_0/4\).

If the admitted background and the actual cutoff imply

\[
\epsilon_{\rm reg}
\le Cg_k\left(P_k+r_k^\chi\right),
\tag{HC41}
\]

then (HC40) improves to

\[
|\operatorname{Cov}(F_x,F_y)|
\le
Cg_k^4(P_k+r_k^\chi)^2h^{-8}e^{-c|x-y|/h}.
\tag{HC42}
\]

Equation (HC42) requires the running-smallness hypothesis (HC41). A fixed coarse regularity bound \(\alpha_0\) only gives the corresponding bound with \(\epsilon_{\rm reg}\) retained.

### 6. A usable interface for the full regular interaction

The regular fluctuation action includes the Haar density and coordinate Jacobian terms in \(P^{(k)}\), as well as the complete effective-action difference in (HC28). Checking only the classical cubic term would not verify (HC20).

The companion regular-potential analysis uses CMP116 Lemmas 1–2, (1.33)–(1.43), to represent the complete regular exponent as

\[
{\cal V}_{\rm reg}(A)=\sum_YV_Y(A).
\tag{HC43}
\]

A sufficient quantitative input is the following. On a complex coordinate polydisc of radius \(\rho\ge1\) strictly containing the real cutoff,

\[
4r_k^\chi\le\rho,\qquad
|V_Y|\le a_Y\bigl(g_k\rho^3+E_*\bigr),
\tag{HC44}
\]

with the source-localized summability bound

\[
\mathfrak A_\alpha:=
\sup_b\sum_{Y\ni b}
a_Y|I_Y|e^{\alpha\operatorname{diam}Y}<\infty.
\tag{HC45}
\]

Here \(I_Y\) is the set of independent coordinates in the support of \(V_Y\). The bounded amplitude \(E_*=E_0+C_{\rm an}\) includes the localized effective-action remainder and any remaining bounded analytic Haar/Jacobian pieces; it is not a claim that every term of \(P^{(k)}\) starts cubically. One sacrifices part of the localization exponent to absorb the polynomial support factors. A two-coordinate Cauchy estimate on the remaining polydisc margin gives

\[
\sup_{A\in D_Y}\sup_b\sum_c
e^{\alpha d(b,c)}
\|\nabla_b\nabla_c{\cal V}_{\rm reg}(A)\|
\le
C_{\mathfrak g}\mathfrak A_\alpha
\left(g_k\rho+E_*\rho^{-2}\right).
\tag{HC46}
\]

The sign of the exponent does not matter: \(V=-{\cal V}_{\rm reg}\) in (HC18) has the same Hessian norm.

For the fixed-domain full-torus small-field construction of CMP109/116, the available analytic radius can be written \(\rho=\epsilon_{\rm ana}/g_k\). The right side of (HC46) is then

\[
C_{\mathfrak g}\mathfrak A_\alpha
\left(\epsilon_{\rm ana}+E_*g_k^2/\epsilon_{\rm ana}^2\right).
\tag{HC47}
\]

Choose the available analytic smallness first, and then \(g_k\), so this is below \(\gamma_0/4\), while retaining the explicit cutoff margin \(4r_k^\chi\le\rho\). The cutoff radius and the analytic smallness parameter must not be silently identified. A cutoff defined at the edge of an analytic domain does not provide the Cauchy margin used above.

The reflected-diffusion proof works directly on the true real cutoff support. Thus a polylogarithmic analytic radius would also suffice whenever the complete potential admits it and
\[
g_k\rho\longrightarrow0,\qquad E_*\rho^{-2}\longrightarrow0.
\tag{HC48}
\]
There is no mathematical need to extend the potential to all of fluctuation space.

The source verification for (HC44)–(HC45), and the distinction between the full-torus regular carrier and the additional multiscale terms, are recorded in the companion note. Theorem HC-W resolves the probability-law step once those analytic estimates are available.

### 7. What the result does and does not close

The following are now established on the stated carrier:

| Item | Result |
|---|---|
| Actual regular cutoff geometry | Product of convex balls in independent starred bond variables |
| Precision needed by a weighted covariance argument | Uniform gap and exponential locality of \(C^*\Delta^{(k)}C\), not only decay of its inverse |
| Cutoff boundary | Included exactly through convex normal reflection; corners and arbitrary norm balls allowed |
| Normalization | Exact normalized covariance, with no lower estimate for the global cutoff probability |
| Nonlinear coordinate map | Its internal derivative has a uniform \(O(g_k)\) exponentially local bound |
| Nonlinear minimizing observable | Covariance (HC40), with no observable Taylor truncation |
| Non-Gaussian extension | Theorem HC-W plus the explicit full-potential Hessian criterion (HC46) |

For full S2 the remaining interfaces are substantive:

1. The exact old transported mark must satisfy the requisite gradient or marked-numerator bound. The function in (HC38) is the actual nonlinear observable on a minimizer; it is not automatically the conditional expectation of an old fine observable after preceding integrations.
2. The analytic radius and Hessian estimate for every term in a general history must be checked. CMP119 has additional boundary and R contributions, and its analytic radii shrink near some multiscale boundaries. Full-torus CMP116 estimates cannot simply be asserted for those terms.
3. Conditional means must be controlled when histories or exteriors are marginalized. Conditional covariance decay alone does not bound covariance of those means.
4. The terminal covariance and the sum of all admitted histories must still be supplied in the common physical normalization.

The first and third interfaces can use the following exact derivative formula, rather than treating the normalization as an uncontrolled quotient.

### 8. Conditional-mean sensitivity: an immediate tool for positive transport

Let \(y\) be a retained parameter, and suppose the geometry and cutoff radii are fixed while \(H_y,f_y\) vary smoothly. Write \(T_yf_y=\mu_y(f_y)\), where \(\mu_y\) has the same product domain as (HC2). Direct differentiation of the normalized integral gives

\[
\partial_{y_j}T_yf_y
=T_y(\partial_{y_j}f_y)
-\operatorname{Cov}_{\mu_y}
\left(f_y,\partial_{y_j}H_y\right).
\tag{HC49}
\]

Applying HC-W,

\[
\begin{aligned}
|\partial_{y_j}T_yf_y|
\le{}&T_y|\partial_{y_j}f_y|\\
&+\lambda_W^{-1}
\|W\nabla_Af_y\|_{L^2(\mu_y)}
\|W^{-1}\nabla_A\partial_{y_j}H_y\|_{L^2(\mu_y)}.
\end{aligned}
\tag{HC50}
\]

If the first gradient is exponentially localized at \(x\), and the mixed score gradient is exponentially localized at \(j\), their covariance contribution is exponentially small in \(d(x,j)\), by exactly the calculation (HC24). This gives a precise local norm in which a normalized positive transport step can be estimated.

Equation (HC50) is not a claim that the needed background derivatives are already known. For the YM carrier they include derivatives of the source-dependent constraint embedding, precision, effective potentials, and minimizer. Those source-background estimates must be supplied or obtained by the marked expansion. What is now closed is the normalized covariance mechanism with the actual hard cutoff.

#### A closed special case: arbitrary partial integration in one regular carrier

There is a useful case where the mixed score estimate in (HC50) is already supplied by the hypotheses. Fix one admitted regular source background and a law on all independent coordinates \(A\in D\), with

\[
H(A)=\tfrac12\langle A,MA\rangle+\langle\ell,A\rangle+V(A)
\tag{HC51}
\]

satisfying (HC18)–(HC22), and with a pointwise exponentially local full Hessian

\[
\|H''_{ij}(A)\|\le C_He^{-\nu d(i,j)}.
\tag{HC52}
\]

Split the coordinates into \(I=I_{\rm int}\sqcup I_{\rm ext}\). For an admitted retained configuration \(y=A_{\rm ext}\), integrate \(A_{\rm int}\) against its exact conditional law and write the resulting mean as \(T_{\rm int}f_x(y)\).

The conditional precision is the principal compression \(M_{\rm int,int}\). Its gap and the weighted perturbation bounds are no worse than those of the original precision. The internal cutoff is still a product. Moreover, for \(j\in I_{\rm ext}\),

\[
\nabla_{A_i}\partial_{y_j}H(A_{\rm int},y)=H''_{ij}(A_{\rm int},y).
\tag{HC53}
\]

Suppose the original mark has a pointwise profile

\[
\|\nabla_i f_x(A)\|\le A_f e^{-\gamma d(i,x)}
\quad\hbox{for every }i\in I.
\tag{HC54}
\]

Apply (HC50) with a weight centered at \(x\). Equations (HC52)–(HC54) and the exponential-sum estimate (HC24) give, for some fixed
\(0<\alpha<\min(\gamma,\nu)\),

\[
\boxed{
\|\partial_{y_j}T_{\rm int}f_x(y)\|
\le
C\left(1+\frac{C_H}{\lambda_W}\right)
A_f e^{-\alpha d(x,j)}.
}
\tag{HC55}
\]

This is uniform in the subset being integrated, its volume, and the admitted retained configuration. It is a statement about the normalized conditional mean of the actual mark \(f_x\), not about a ratio whose denominator is bounded separately.

Several successive integrations within this same carrier can be replaced by integration over their union, by the tower property. Thus the constant in (HC55) need not be multiplied once for every such subdivision. Changing the source background or passing to a new RG scale is outside this fixed-carrier assertion.

### 9. Centered moments on the actual regular cutoff carrier

The unweighted version of the same dynamics supplies all finite centered moments for marks whose gradient is bounded. Let

\[
H''\ge m_0I\quad\hbox{on }D,\qquad m_0>0.
\tag{HC56}
\]

For (HC18) one can take \(m_0=m-\varepsilon_0\). Theorem HC-W's proof with \(W=I\) gives

\[
|\nabla P_tq|\le e^{-m_0t}P_t|\nabla q|.
\tag{HC57}
\]

For a positive smooth function \(q\), the reversible entropy identity and the chain rule for the Neumann form are

\[
\operatorname{Ent}_{\mu}(q)
=\int_0^\infty
\mu\!\left(\frac{|\nabla P_tq|^2}{P_tq}\right)\,dt.
\tag{HC58}
\]

Cauchy–Schwarz under the Markov kernel gives

\[
\frac{(P_t|\nabla q|)^2}{P_tq}
\le P_t\!\left(\frac{|\nabla q|^2}{q}\right).
\tag{HC59}
\]

Use (HC57), invariance, and
\(\int_0^\infty e^{-2m_0t}dt=(2m_0)^{-1}\). Setting \(q=u^2\), with a positive approximation if necessary, proves the cutoff-uniform logarithmic Sobolev inequality

\[
\boxed{
\operatorname{Ent}_{\mu}(u^2)
\le \frac{2}{m_0}\mu|\nabla u|^2.
}
\tag{HC60}
\]

For a real mark \(f\) with \(\sup_D|\nabla f|\le L_f\), apply (HC60) to \(u=e^{tf/2}\). If
\(\psi(t)=\log\mu e^{tf}\), the result is
\[
t\psi'(t)-\psi(t)\le \frac{t^2L_f^2}{2m_0}.
\tag{HC61}
\]
Integration from \(0\), where \(\psi'(0)=\mu f\), gives

\[
\boxed{
\mu e^{t(f-\mu f)}
\le \exp\!\left(\frac{t^2L_f^2}{2m_0}\right)
\quad (t\in\mathbb R).
}
\tag{HC62}
\]

Consequently,

\[
\mu\{|f-\mu f|\ge s\}
\le 2e^{-m_0s^2/(2L_f^2)},
\qquad
\|f-\mu f\|_{L^p(\mu)}
\le C L_f\sqrt{p/m_0},\quad p\ge2.
\tag{HC63}
\]

For the nonlinear minimizing-field mark (HC38), summing (HC39) in \(\ell^2\) gives \(L_f\le Cg_k\epsilon_{\rm reg}h^{-4}\), hence

\[
\boxed{
\|F_x-\mu F_x\|_{L^p(\mu)}
\le
Cg_k\epsilon_{\rm reg}h^{-4}\sqrt{p/m_0}.
}
\tag{HC64}
\]

These estimates retain the same characteristic function and complete regular density whenever (HC56) has been verified for that density. They are potentially useful for posterior-weighted marked estimates in an R component. Their centering is conditional on the carrier; they do not bound variation of the carrier means, or identify a fine observable transported through older RG scales with (HC38).

### Sources and verification record

* Balaban, CMP99 (1985), 389–434, printed p.428, (3.156)–(3.158): independent constraint coordinates, uniformly positive and exponentially local precision.
* Balaban, CMP119 (1988), 243–285, printed pp.247–249, (1.8)–(1.15), and pp.268–272, (3.16)–(3.28): actual starred cutoff, conditional interior carrier, nonlinear coordinates and regular effective density.
* Balaban, CMP109 (1987), 249–301, printed pp.267–268: local constraint-linearizing equation and scaling to independent coordinates.
* Balaban, CMP116 (1988), 1–22, pp.3 and 6, (1.19)–(1.20), and pp.9–11, Lemmas 1–2: locality of \(B'\), analytic regular fluctuation action and localized bounds.
* Bubeck, Eldan, Lehec, *Sampling from a log-concave distribution with Projected Langevin Monte Carlo*, Section 3.1, printed p.14: existence of normal reflection in a convex body with Lipschitz drift, and the exact truncated Gibbs reversible measure. [Primary author manuscript](https://arxiv.org/abs/1507.02564). Only these standard process facts are imported; (HC8)–(HC25) are the weighted argument given here.
* [Minimizing-field response and the two-insertion cluster formula](two_insertion_clusters.md), Part I, Theorem LR-B: nonlinear minimizing-field leaf and Wilson/clover derivative, itself using the variational estimates of CMP102 Proposition 9.

The proof above never assumes that a cutoff on nonlinear dependent variables is convex.

---

## Part II.A. Complete regular potential and normalized rooted clusters

### Results and exact scope

This note proves two estimates needed by the observable route.

1. A localized analytic bound for the **actual regular fluctuation potential** implies a small exponentially weighted Hessian on the actual hard-cutoff domain. The required analytic bound is supplied by the full-torus small-field construction in Balaban, CMP **116** (1988), pp. 8–11, without needing to reconstruct the poorly extracted display (1.43). Combined with the companion reflected-diffusion theorem, this gives covariance decay for the full nonlinear minimizing-field insertion under the interacting regular hard-cutoff law.
2. Individual one-root and two-root activity norms, together with a strict unmarked Kotecký–Preiss bound, imply a normalized connected two-root estimate. This removes the earlier requirement to assume a bound for the entire marked cluster sum. Applied to the companion large-field age-budget estimates, it proves a conditional covariance bound for marked components retained in the reset core.

Neither result identifies an arbitrary old transported scalar insertion with a fresh minimizing-field insertion. The source-dependent regular induction, the remaining exterior covariance after an R reset, and the analytic-domain verification for every mixed multiscale history remain separate obligations. The distinction is essential to the scope of the conclusions below.

### 1. An analytic localization lemma for the full Hessian

Let \(I\) denote independent current-scale bond coordinates. Each coordinate belongs to a fixed finite-dimensional real Lie algebra, complexified for analyticity. Use current-unit bond distance \(d\), and write

\[
 V(B)=\sum_Y V_Y(B),\qquad \|B\|_\infty<\rho .
 \tag{H1}
\]

Each \(V_Y\) depends only on the coordinate set \(I_Y\). Suppose it is analytic on the displayed ball and

\[
 \sup_{\|B\|_\infty<\rho}|V_Y(B)|
 \le A_Y\,[g\rho^3+E_*],
 \tag{H2}
\]

where \(E_*\) is a fixed bounded analytic amplitude. It may include the previous-action amplitude \(E_0\) and a fixed constant for Jacobian or determinant terms. The localization weights satisfy

\[
 \mathfrak A_\alpha
 :=\sup_b\sum_{Y:b\in I_Y}
 A_Y\,|I_Y|\,e^{\alpha\operatorname{diam}I_Y}<\infty.
 \tag{H3}
\]

This assumption is on individual localized terms. In the application, \(A_Y\) is an exponentially decaying polymer weight and (H3) follows by sacrificing part of its decay exponent. It is uniform in lattice volume, ultraviolet depth, and the position of \(b\), with fixed blocking and localization constants.

Let the actual domain be

\[
 D=\prod_{b\in I}\{B_b:|B_b|\le r_b\},
 \qquad r_\chi:=\sup_b r_b\le\rho/4.
 \tag{H4}
\]

#### Proposition H

There is a constant depending only on the coordinate norm and Lie algebra such that

\[
 \boxed{
 \sup_{B\in D}\sup_b\sum_c e^{\alpha d(b,c)}
 \|\nabla_b\nabla_c V(B)\|
 \le C_G\mathfrak A_\alpha
 \left(g\rho+E_*\rho^{-2}\right).
 }
 \tag{H5}
\]

**Proof.** Choose a fixed basis of the Lie algebra. Norm equivalence supplies a constant \(c_G>0\) such that varying any two complex components by at most \(c_G\rho\) around a point of \(D\) stays inside \(\|B\|_\infty<\rho\). The two-variable Cauchy estimate, with the usual factor of two when a component is differentiated twice, gives

\[
 \|\nabla_b\nabla_c V_Y(B)\|
 \le C_G A_Y\left(g\rho+E_*\rho^{-2}\right).
 \tag{H6}
\]

The derivative is zero unless both \(b,c\in I_Y\). Therefore

\[
 \begin{aligned}
 \sum_c e^{\alpha d(b,c)}\|\nabla_b\nabla_cV(B)\|
 &\le C_G(g\rho+E_*\rho^{-2})
 \sum_{Y:b\in I_Y} A_Y
 \sum_{c\in I_Y}e^{\alpha d(b,c)}\\
 &\le C_G\mathfrak A_\alpha(g\rho+E_*\rho^{-2}).
 \end{aligned}
\]

The same summable majorant justifies twice differentiating the series. This proves the proposition. \(\square\)

#### Two useful choices of radius

For a fixed small analytic parameter \(\epsilon_{\rm ana}\), take

\[
 \rho=\epsilon_{\rm ana}/g.
\]

Then (H5) is

\[
 \varepsilon_{\rm Hess}
 \le C_G\mathfrak A_\alpha
 \left(\epsilon_{\rm ana}
       +E_*g^2\epsilon_{\rm ana}^{-2}\right).
 \tag{H7}
\]

Choose \(\epsilon_{\rm ana}\) small first and then the maximal running coupling small. This makes the Hessian perturbation smaller than any fixed fraction of the Gaussian precision gap. The hard cutoff requires the separate margin \(4g r_\chi\le\epsilon_{\rm ana}\). Using the same symbol for a cutoff parameter and an analytic radius does not prove that margin.

The same conclusion holds for a growing radius satisfying

\[
 4r_\chi(g)\le\rho(g),\qquad
 \rho(g)\longrightarrow\infty,\qquad
 g\rho(g)\longrightarrow0.
 \tag{H8}
\]

For example, a sufficiently large fixed multiple of a positive power of \(\log g^{-2}\) works whenever it lies inside the source analytic domain. The resulting bound is

\[
 C_G\mathfrak A_\alpha
 \left(g\,\operatorname{polylog}(g^{-1})
      +E_*\operatorname{polylog}(g^{-1})^{-2}\right).
 \tag{H9}
\]

No extension of \(V\) outside its original analytic domain is used.

### 2. What the small-field source supplies

The primary source is Balaban, *Renormalization group approach to lattice gauge field theories. II. Cluster expansions*, CMP **116** (1988), 1–22. The relevant clauses are:

- (1.19)–(1.21): the independent field enters through \(B'=gCB-\mathfrak hD(gCB)\), analytic for small \(g\|B\|\), with \(\|B'\|\le Cg\|B\|\).
- Lemma 1, (1.33)–(1.36): the complete old-action difference is localized in \(Y\), analytic for \(\|B\|<\epsilon_1/g\), with a depth-uniform exponentially decaying bound. The sums over earlier scales are already performed in (1.26)–(1.32).
- (1.37)–(1.40): the localized classical remainder has cubic size in \(B'\). Multiplication by \(g^{-2}\) gives the \(g\rho^3\) term in (H2).
- The paragraph before Lemma 2 extends the localization analysis to all remaining fluctuation-action terms. Their bounded analytic pieces can be included in \(E_*\).

This source information supplies (H1)–(H3) for the full-torus regular fluctuation action, with fixed localization parameters. Polynomial factors from summing local plaquettes and differentiating can be absorbed into the localization exponent, as in the source summations. Thus (H7) is an additional estimate **derived from** that construction; it is not a restatement of a missing marked source bound.

The associated fixed-cutoff construction is Balaban, CMP **109** (1987), 249–301, (2.9) and the subsequent elimination of constrained bonds. Its small cutoff constant must be chosen sufficiently below the allowed analytic constant. Since both constants are auxiliary smallness choices, one can impose \(\epsilon_{\rm ana}\ge4\epsilon_{\rm cut}\) while retaining the source absolute smallness requirements.

#### Threshold robustness of the source-free regular induction

The preceding assertion first concerns the CMP **109**/**116** small-field model. Its old effective action must not be identified with a differently cut off history merely because both models use small fields. The following extension removes one specific difficulty in comparing them.

**Proposition H-cut.** In the full-torus source-free regular construction, replace the independent-coordinate cutoff at step \(k\) by

\[
 \chi_{r_k}(B)=\prod_{b\in I_k}{\bf1}_{|B_b|\le r_k},
 \qquad
 r_0\le r_k\le\epsilon_{\rm cut}/g_k,
 \tag{Hc1}
\]

where \(r_k\) is independent of the background field. For \(r_0\) sufficiently large, depending only on the fixed localization parameters and the desired activity slack, the source-free localized analytic induction has the same background domain and uniform bounds. It therefore supplies (H2)–(H3) for the resulting sequence of effective actions. The constants do not depend on the particular sequence \((r_k)\).

**Proof.** The interaction estimates before the final Gaussian integration remain valid, because the cutoff has only been reduced inside the admitted analytic field ball. On the union \(Y_0\) of active interaction supports the cutoff is kept. Outside \(Y_0\), use the exact identity

\[
 \prod_{b\notin Y_0}{\bf1}_{|B_b|\le r_k}
 =\sum_{P\subset I_k\setminus Y_0}(-1)^{|P|}
   \prod_{b\in P}{\bf1}_{|B_b|>r_k}.
 \tag{Hc2}
\]

For a fixed sufficiently small \(u>0\),

\[
 \prod_{b\in P}{\bf1}_{|B_b|>r_k}
 \le e^{-u r_k^2|P|}
       \exp\left(u\sum_{b\in P}|B_b|^2\right).
 \tag{Hc3}
\]

This is the complete radius dependence of the defect estimate. The positive quadratic exponential is absorbed into the localized Gaussian precision, leaving a uniform positive gap. For a real centered Gaussian with covariance norm at most \(\sigma^2\), the finite-coordinate moment is explicitly

\[
 \mathbb E\exp\left(u\sum_{b\in P}|B_b|^2\right)
 =\det(I-2uC_P)^{-1/2}
 \le e^{C|P|},\qquad 2u\sigma^2<1/2.
 \tag{Hc4}
\]

The source performs the corresponding localized complex-background estimates in (2.15)–(2.26). Their determinant and localization factors depend on \(Y_0,P\), and the enclosing localization domain, but not on \(r_k\). The replacement in that calculation is exactly (Hc3) in place of the original Gaussian cutoff-tail bound.

The remaining sums spend finitely many portions of the factor \(e^{-u r_k^2|P|}\): one bounds the choices of defect bonds, and the others pay the size of the additional localization blocks and their connecting lengths. The source executes these sums in (2.31)–(2.34). With fixed block sizes and localization exponents, their requirements are finite inequalities of the form

\[
 c_1r_k^2\ge C_{L,M,\kappa}
          +\log(1/\varepsilon_{\rm tail}).
 \tag{Hc5}
\]

Choose \(r_0\) to meet them. The contributions containing interaction potentials retain the same analytic bounds; pure-cutoff contributions are at most the chosen \(\varepsilon_{\rm tail}\) in that norm. Taking this smaller than the unused induction margin closes the same source-free action induction. The cutoffs are independent of the background, so holomorphy in the background is preserved by the dominated localized Gaussian integrals. Gauge invariance and the background-field subtraction identities are unchanged. Induction from the same initial Wilson action proves the assertion. \(\square\)

For \(r_k=C(\log g_k^{-2})^p\), \(p>0\), (Hc1) holds uniformly when the maximal coupling is sufficiently small. If smoothness at \(g=0\) of the resulting coupling correction is additionally needed, \(p>1/2\) makes the tail \(e^{-c(\log g^{-2})^{2p}}\) smaller than every power of \(g\). Its fixed-order derivatives, including the polynomial factors from differentiating the moving cutoff surface, also tend to zero. This last observation concerns fixed derivative orders; it is not a uniform all-order source budget.

The fixed \(r_0\) statement preserves a fixed small activity amplitude. If a particular inductive clause requires a coupling-dependent amplitude, one must retain that amplitude in (Hc5). The sufficient condition is
\(e^{-c r_k^2}\le\varepsilon_{\rm tail}(g_k)\) after the fixed geometric losses. For any prescribed finite power \(\varepsilon_{\rm tail}(g)=g^N\), the polylogarithmic choice with \(p>1/2\) satisfies the condition uniformly at small coupling. Thus the robustness argument does not replace a required \(g\)-dependent induction bound by a merely fixed small constant.

Proposition H-cut proves robustness of the regular analytic construction under running independent-coordinate thresholds. The following source comparison matches that construction to the full-torus sector of the final CMP **119**/LFR construction. It does not remove the additional boundary terms or old-stratum conditions of a mixed history.

#### Analysis of the full-torus specialization of CMP 119

Set \(\Omega_j=\Lambda_j=T\) at every preceding scale. Then the old exterior strata, boundary field, and large-field operations are absent; the position-dependent coupling is constant. The history-determined constrained operators reduce to their ordinary full-torus counterparts. CMP **119**, immediately after (3.28), identifies its regular logarithm with the formula in the small-field construction except for domain restriction and history-determined operators. Both exceptions disappear in this specialization. Its paragraph leading to (3.43) likewise states that interior localized terms obey the original regular localization lemmas.

The point-root counterterm does not create a new scalar renormalization scheme in this specialization. Equations (3.61)–(3.64) explicitly identify its scalar coefficient with the earlier coefficient; the partition of unity (3.40) then sums the local Wilson counterterm to the full Wilson action. Vacuum constants have no effect on the conditional covariance.

There is, however, a displayed scaling ambiguity that must not be silently repaired. The first-step formula (1.18), on printed p. 250, uses the rescaled independent-field threshold \(g_0^{-1}\delta_0\). The later text on p. 267 performs the fluctuation rescaling, and (3.15) has Gaussian precision without a factor \(g_k^{-2}\); the printed (3.16), p. 268, nevertheless displays the threshold \(\delta_k\) on the variable named \(A_k\). Formula (3.25) does not make an additional argument rescaling explicit. These displayed formulas do not by themselves determine an unambiguous common variable convention. We therefore do **not** assert that the exact printed later cutoff is already the threshold \(\delta_k/g_k\).

The later LFR I paper resolves the convention for the final construction. On its printed p. 178, (1.8) uses \(\exp(ig_jA_j)\), while (1.9) explicitly gives \(|A_j|<g_j^{-1}\delta_j\). The paragraph above identifies the operations under discussion as the existing one-step operations (2.21) of CMP **119**, not newly chosen reset cutoffs. Thus the final construction specifies the regular rescaled threshold

\[
 r_j=g_j^{-1}\delta_j=\frac{A_1}{A_0}p_0(g_j).
 \tag{Hc6}
\]

This is independent of the background, diverges polylogarithmically at small coupling, and has \(g_jr_j\to0\). It satisfies the hypotheses of Proposition H-cut, including any fixed finite-power tail requirement. The all-regular action, scalar counterterm, independent variables, and cutoff now match the threshold-robust small-field construction. Therefore (H7) and the nonlinear regular covariance consequence apply to that **full-torus regular carrier of the final construction**. This conclusion uses the explicit later formula; it does not assert that the displayed CMP **119** equation is an established erratum. Mixed-history old-stratum and boundary estimates remain outside this matching argument.

#### A concrete regular-law consequence

Let the full-torus regular conditional law in independent coordinates be

\[
 \mu(dB)=Z^{-1}{\bf1}_{D}(B)
 \exp\{-\tfrac12\langle B,MB\rangle+V(B)+\langle\ell,B\rangle\}\,dB.
 \tag{H10}
\]

The precision is the actual constrained precision \(M=C^*\Delta_kC\), whose uniform gap and exponential locality are recorded in CMP **99** (1985), p. 428. Assume the cutoff and analytic parameters are chosen as above. The perturbation (H7), followed by a sufficiently small spatial weight exponent, gives the weighted coercivity required by Theorem HC-W in **Part I**.

Consequently, every pair of observables with localized gradients satisfies the normalized weighted covariance estimate from that theorem. In particular, use the previously proved nonlinear minimizing-field derivative bound in actual fluctuation coordinates:

\[
 |\nabla_b Q_x|
 \le Cg\epsilon_{\rm reg}h^{-4}
 e^{-c d(b,z_x)}.
 \tag{H11}
\]

Then

\[
 \boxed{
 |\operatorname{Cov}_\mu(Q_x,Q_y)|
 \le Cg^2\epsilon_{\rm reg}^2h^{-8}
 e^{-c'|x-y|/h}.
 }
 \tag{H12}
\]

If the background and actual fluctuation cutoff imply
\(\epsilon_{\rm reg}\le Cg(P+r_\chi)\), this becomes

\[
 |\operatorname{Cov}_\mu(Q_x,Q_y)|
 \le Cg^4(P+r_\chi)^2h^{-8}e^{-c'|x-y|/h}.
 \tag{H13}
\]

This statement retains the hard characteristic function, normalization, nonlinear observable, and nonlinear regular interaction. Its observable remains the minimizing-field insertion at this step. It is not yet the old insertion obtained by an arbitrary sequence of previous transport kernels.

#### Shrinking domains in the full multiscale construction

The CMP **119** (1988) construction uses scale-dependent background radii in (2.28), of the form

\[
 \alpha_{0,j}=g_jC_0(\log g_j^{-2})^{q_0},\qquad
 \alpha_{1,j}=g_jC_1(\log g_j^{-2})^{q_1}.
 \tag{H14}
\]

A fixed radius \(\epsilon/g_k\) cannot simply be imported into every old stratum. The flexible form (H8) is useful precisely here.

Here is a sufficient route to verifying the radius in a current regular stratum. Put \(m=k-j\). Suppose the nested minimizing-field bounds carry a current perturbation \(g_kB\) to a \(j\)-scale potential of size \(CL^{-m}g_k\|B\|\), with the expected stronger \(L^{-2m}\) gain for curvature. A sufficient common ball is then

\[
 \rho_k\le c\min_{j\le k}
 L^{k-j}\frac{\min(\alpha_{0,j},\alpha_{1,j})}{g_k}.
 \tag{H15}
\]

The coupling comparison (2.6), \(g_k/g_j\le C\sqrt{1+k-j}\), and the monotonicity of the older logarithms give a lower bound by a positive multiple of
\((\log g_k^{-2})^{\min(q_0,q_1)}\), since
\(\inf_{m\ge0}L^m/\sqrt{1+m}>0\). This removes the apparent loss caused solely by the coupling ratio. To use (H15), one must still check the actual norm definitions, nonlinear domain reserve, and the margin over the cutoff (3.16).

A second issue is summing the old potentials without paying a factor equal to the RG depth. Vacuum and scalar marginal subtraction is needed before using the fifth-order irrelevant gain. If a localized \(j\)-term has the source's \(5-\varepsilon\) power gain, its rescaled contribution per current block is bounded by a summable sequence of the form

\[
 C E_*\,(1+m)^p L^{-(1-\varepsilon)m},\qquad 0<\varepsilon<1,
 \tag{H16}
\]

after the \(L^{4m}\) old-block count. The polynomial accounts for coupling and analytic-radius ratios. Hence a verified (H16) would give a uniform constant in (H2). The point-root subtraction and Ward expansion in CMP **119**, (3.48)–(3.67), are the appropriate source mechanism. Applying that mechanism to every inherited mark, as opposed to the source-free action, remains the regular marked-induction question.

For outer old strata, boundary terms, and R-generated activities, the actual domain inclusion and weighted sum must be checked separately. Source statements that propagator decay compensates shrinking domains indicate a strategy; they do not by themselves prove all the marked estimates. Accordingly (H15)–(H16) are a precise proposed verification route, while the full-torus conclusion (H12) uses the already established CMP **109**/**116** regular action.

### 3. A rooted KP theorem from individual marked norms

Consider a finite hard-core polymer gas, with incompatibility denoted \(X\nsim Y\). A polymer is incompatible with itself. Let \(\ell(X)\ge1\) be a localization length; for example, one plus a minimal connecting-tree length in blocks. Let \(a(X)\ge a_{\min}>0\). Suppose that, for some \(\lambda>0\) and \(0<\theta<1\),

\[
 \sum_{Y:Y\nsim X}|H(Y)|
 e^{\lambda\ell(Y)+a(Y)}
 \le (1-\theta)a(X).
 \tag{K1}
\]

The slack in (K1) is substantive. A source-free estimate merely at the boundary of convergence is not sufficient for the particular proof below.

Introduce two local sources with activity jet

\[
 K_{s,t}(X)=H(X)+sJ_1(X)+tJ_2(X)+stJ_{12}(X)
 +O(s^2)+O(t^2).
 \tag{K2}
\]

The coefficients are the actual derivatives of the source-deformed activities. Define the **individual activity norms**

\[
 A_i=\sum_X |J_i(X)|e^{\lambda\ell(X)+a(X)},
 \qquad
 A_{12}=\sum_X |J_{12}(X)|e^{\lambda\ell(X)+a(X)}.
 \tag{K3}
\]

For spatial decay, assume each \(J_i\) is anchored at \(x_i\), and \(J_{12}\) at both points. One may either require its support to contain the anchors, or include the lengths of connecting paths from anchors to support in \(\ell\) for marked activities. Suppose a connected cluster carrying both marks satisfies

\[
 \sum_{X\text{ in cluster}}\ell(X)
 \ge c_0\frac{|x_1-x_2|}{hR}.
 \tag{K4}
\]

The source block geometry gives such an inequality because an incompatibility-connected cluster joins the anchors. It also holds for a single mixed polymer.

#### Theorem K2

Let \(Z(s,t)\) be the partition function with activities (K2), and let
\(\Gamma_{12}=\partial_s\partial_t\log Z(s,t)|_{s=t=0}\). Then

\[
 \boxed{
 |\Gamma_{12}|
 \le \left(A_{12}+\frac{A_1A_2}{\theta a_{\min}}\right)
 \exp\left[-c_0\lambda\frac{|x_1-x_2|}{hR}\right].
 }
 \tag{K5}
\]

If an explicit scalar factor \(\exp(c(s,t))\) was removed before defining the gas, its mixed coefficient \(\partial_s\partial_t c(0,0)\) must be included separately. A product of two separate linear scalar factors has no mixed logarithmic coefficient.

#### Proof

Write \(\varphi^T(X_0,\ldots,X_n)\) for the usual connected Ursell coefficient of the hard-core incompatibility graph. The connected graph sum satisfies the tree bound

\[
 |\varphi^T(X_0,\ldots,X_n)|
 \le \sum_{\tau\text{ spanning tree}}
 \prod_{\{i,j\}\in\tau}{\bf1}_{X_i\nsim X_j}.
 \tag{K6}
\]

For completeness, fix an ordering of the labeled vertices and extract a rooted breadth-first spanning tree from each connected graph. The graphs giving a fixed tree form an interval between the tree and its allowed closure. The alternating edge sum over this interval is zero unless the extra-edge set is empty, in which case its absolute value is one. Summing over trees gives (K6).

For any nonnegative activity \(z\) satisfying

\[
 \sum_{Y:Y\nsim X}z(Y)e^{a(Y)}\le a(X),
 \tag{K7}
\]

the rooted absolute cluster sum obeys

\[
 \mathcal T_z(X):=
 \sum_{n\ge0}\frac1{n!}
 \sum_{X_1,\ldots,X_n}
 |\varphi^T(X,X_1,\ldots,X_n)|
 \prod_{j=1}^n z(X_j)
 \le e^{a(X)}.
 \tag{K8}
\]

Indeed, the tree majorant has the rooted-tree recursion

\[
 T_{q+1}(X)
 =\exp\left(\sum_{Y:Y\nsim X}z(Y)T_q(Y)\right),
 \qquad T_0(X)=1.
 \tag{K9}
\]

Inductively \(T_q(X)\le e^{a(X)}\) by (K7). Monotone convergence, followed by (K6), proves (K8). This also gives absolute convergence of the cluster series used below.

Put \(z(Y)=e^{\lambda\ell(Y)}|H(Y)|\). The terms containing one mixed root \(J_{12}\) are bounded by \(A_{12}\), by (K8).

For the terms with two distinct marked polymer occurrences, assume \(A_2>0\) and define

\[
 z_\sigma(Y)=e^{\lambda\ell(Y)}
 \left(|H(Y)|+\sigma\frac{|J_2(Y)|}{A_2}\right),
 \qquad \sigma_*:=\theta a_{\min}.
 \tag{K10}
\]

For \(0\le\sigma\le\sigma_*\), the marked contribution to the left side of (K7) is at most \(\sigma\). Together with (K1), this is at most \(a(X)\). Hence (K8) applies to \(z_{\sigma_*}\).

Root the series at \(J_1\) and set

\[
 \mathcal R(\sigma)
 =\sum_X e^{\lambda\ell(X)}|J_1(X)|\mathcal T_{z_\sigma}(X).
 \tag{K11}
\]

Every Taylor coefficient of this series is nonnegative and
\(\mathcal R(\sigma_*)\le A_1\). Its coefficient of \(\sigma\), multiplied by \(A_2\), is exactly the absolute two-root cluster sum in which the two derivatives land on different polymer occurrences. The factorials agree: choosing the second marked occurrence among \(n\) nonroot occurrences changes \(1/n!\) into \(1/(n-1)!\). Therefore this contribution is at most

\[
 A_2[\sigma]\mathcal R(\sigma)
 \le A_1A_2/\sigma_*.
 \tag{K12}
\]

If \(A_2=0\), the contribution vanishes. Finally, each connected marked term has the geometrical property (K4). Remove the exponential factor in (K5) from its weight and apply the weighted bounds just proved. Adding the one-mixed-root contribution proves (K5). \(\square\)

#### Why this is a new usable estimate

The hypotheses involve the source-free activity norm and the individual marked coefficients \(J_i,J_{12}\). They do not assume the desired bound for a sum over all two-root clusters. The partition denominator is accounted for by the logarithm and the connected expansion. No uniform bound on a normalized ratio \(N_\gamma^F/N_\gamma\) is required.

When the original source partition function is

\[
 Z(s,t)=Z(0,0)\,
 \mathbb E[(1+sF_{x_1})(1+tF_{x_2})],
 \tag{K13}
\]

its mixed logarithmic coefficient is exactly
\(\operatorname{Cov}(F_{x_1},F_{x_2})\). Exponential sources have the same degree-\((1,1)\) coefficient. Thus Theorem K2 directly estimates normalized covariances once the actual activity jet has been constructed.

### 4. Consequence for marked R cores

The companion R analysis uses the actual future-budget induction in LFR II, (1.80)–(1.88), to pay the engineering scaling cost of a bounded degree-two marked ancestry. It preserves a small factor \(\eta_k=e^{-c p_0(g_k)}\) after increasing a fixed budget constant. For the restricted component gas whose roots remain in the reset core, it supplies activity norms of the form

\[
 A_1\le C\mathcal F_1 h_k^{-4}\eta_k,
 \qquad A_2\le C\mathcal F_2 h_k^{-4}\eta_k,
 \qquad A_{12}\le C\mathcal F_1\mathcal F_2h_k^{-8}\eta_k.
 \tag{R1}
\]

Here \(\mathcal F_i\) are the bounded seed norms at their own birth scales. Root-localization and analytic norm overheads must already be included in (R1); any fixed factors can be paid by the same large-field penalty as described in that analysis. The unmarked component gas must retain the strict KP slack (K1), obtained by using a sufficiently small running coupling and sacrificing part of its exponential decay.

Then Theorem K2 gives the explicit normalized conditional estimate

\[
 \boxed{
 |\operatorname{Cov}_{\rm core}(F_{x_1},F_{x_2}\mid\text{exterior})|
 \le C\mathcal F_1\mathcal F_2h_k^{-8}
 (\eta_k+\eta_k^2)
 e^{-c|x_1-x_2|/(h_kR_k)}.
 }
 \tag{R2}
\]

This includes clusters with two marks in one component and in distinct components. It supplies the missing normalization-and-connection step for that restricted gas. It is not a proof that all marks at all scales remain in the core. The covariance of the conditional exterior means, and roots that have left the core, require the regular marked norm and remain visible.

### 5. The precise remaining regular marked induction

The remaining issue is to prove that **the actual old source coefficient** obtained by integrating the previous scale belongs to an anchored analytic class with its physical current-scale normalization. A sufficient structure is

\[
 F_{k,x}=c_{k,x}+z_{k,x}\,q_k+R_{k,x},
 \tag{M1}
\]

where \(q_k\) is the scalar marginal density, the first term is an identity coefficient, and the remainder has an irrelevant and spatially localized norm. The new work above supplies interaction covariance estimates and the convergent cluster operation once the input marked norm exists. It does not yet supply the marginal recurrence for \(z_{k,x}\).

The source-free point-root Ward analysis suggests applying the scalar projection to each actual generated jet. The block-constant scalar part should be compared with the derivative of the running coupling map, while source gradients are assigned to the contracting remainder. For a frozen observable transport kernel, differentiating the coupling also differentiates the kernel and its cutoff; those score and boundary terms must be identified and controlled. Omitting them would change the observable being transported.

An estimate of the form

\[
 |z_{k+1}|\le(1+\epsilon_k)|z_k|+C\|R_k\|,
 \qquad \sum_k\epsilon_k<\infty,
 \tag{M2}
\]

together with an actual contracting recurrence for \(R_k\), would provide one sufficient scale-uniform input to (K3). It is stronger than necessary if a common running source normalization is allowed. The later cocycle notes prove that \(I+O(g_k^2)\), combined with a contracting irrelevant block and normalization by a single deterministic terminal-scale cocycle, gives a physical-logarithm bound depending only on the remaining scales. No summability of the bare \(g_k^2\) multipliers is then needed. The finite-jet and one-root analytic notes develop the corresponding actual regular operator estimates. Root-position/source-profile dependence, common normalization across carriers, and mixed-history interfaces still have to be settled. Uniform differentiability of a source-free scalar coupling correction alone does not prove these facts or the frozen-kernel identity.

#### Status summary

| Item | Status after this note |
|---|---|
| Analytic localization \(\Rightarrow\) weighted Hessian, including cutoff margin | Proved in Proposition H |
| Full-torus CMP 109/116 regular fluctuation action satisfies sufficient analytic bounds | Supplied by CMP 116 clauses identified above; yields (H7) |
| Source-free regular analytic induction with running independent-coordinate cutoff thresholds | Proved in Proposition H-cut for (Hc1); final all-regular carrier matched using LFR I (1.8)–(1.9) |
| Nonlinear minimizing-field covariance under interacting hard-cutoff regular law | Proved by Proposition H plus companion HC-W, in the stated regular carrier |
| Normalized connected two-root bound from individual marked activity norms | Proved in Theorem K2 |
| Restricted marked R core, including distinct component connection | Proved by Theorem K2 given companion source-specific activity estimates (R1) |
| Analytic-domain reserve for every mixed multiscale history | Verification route (H15)–(H16); not completed here |
| Affine current-scale norm for arbitrary old scalar source through regular T steps | Not completed; requires actual marginal/irrelevant source recurrence |
| Exterior covariance after an R reset | Requires that regular marked recurrence |
| S2 for every actual old insertion, hence the full YM existence proof | Not established by these results |

---

## Part II.B. Analysis of the actual rescaled cutoff radius

This section checks the rescaled cutoff radius used in the regular-carrier covariance and Hessian estimates.

### Finding

The later final-construction paper, Balaban's **Large Field Renormalization I**, explicitly gives the ordinary rescaled fluctuation cutoff as

\[
\chi_{\square'}^{(j)}(A_j)
=\mathbf 1\!\left\{
\sup_{b\in(\square'^{\sim2})^{(k)*}}|A_j(b)|
<g_j^{-1}\delta_j
\right\}.
\tag{RA1}
\]

This is the displayed equation **(1.9), printed p.178**. The notation for the enlarged cube and the starred bond set is retained from the source. The same page's preceding equation **(1.8)** uses \(\exp(i g_j A_j)\), so \(A_j\) in (RA1) is the rescaled variable. This is an explicit later definition, not a cutoff radius inferred from a desired Gaussian tail estimate.

The literal mismatch in **CMP119 (3.16)** remains recorded: after the stated scaling \(A'_k=g_kA_k\), that earlier display prints the radius \(\delta_k\). No published erratum is known or asserted here. The later definition (RA1) specifies the convention used in the final construction.

### Why (1.9) is not a separate boundary-only convention

The displayed instance on p.178 is initially indexed by cubes in

\[
(\widetilde\Lambda_{j+1}\setminus\Lambda_{j+1})\cap Z.
\]

Consequently, p.178 alone should not be described as an entire full-torus fluctuation integral. The identification with the inherited ordinary cutoff family has the following explicit source chain.

1. **CMP119, p.269, following (3.20):** the source says that the product of small-field functions from decomposition **(3.16)** on the regular interior is \(\chi^{(k)}(\Lambda_{k+1})\). In **(3.21)** it uses the same \(\chi^{(k)}\) factors on the remaining part of \(\Omega_{k+1}\cap\Lambda_{k+1}^{c}\). Thus the interior and exterior pieces come from one decomposition and one cutoff family.

2. **CMP119, p.270, (3.23)–(3.25):** the integration over the remaining fluctuation variables on \(\Omega_{k+1}\cap\Lambda_{k+1}^{c}\), including the factors from (3.21), enters the inherited one-step operation. The conditional interior integral in **(3.25)** retains \(\chi^{(k)}(\Lambda_{k+1})\). These are the two pieces of the same original cutoff, split by the conditioning operation. The notation \(\mathbb T^{(k+1)}\) in this construction and the general \(\mathbb T^{(j)}\) convention in (2.21) have the source's step indexing; no inference about the radius depends on that offset.

3. **LFR I, p.178, paragraph preceding (1.3):** the author explicitly identifies the one-step operations being written as those in **(2.21) [III]**. Reference **[III]**, as confirmed in the bibliography on p.202, is CMP119, 243–285. The seven groups (1.3)–(1.9) are a restatement of these inherited characteristic factors on an admitted component with no new large-field factors in the preceding \(N\) operations. Equation (1.9) is therefore a specification of this inherited ordinary fluctuation cutoff family.

4. **LFR I, p.183, paragraph and equation (1.28):** the source explicitly recalls the functions \(\chi_{\square'}^{(j)}\) “given by (1.9),” then completes **those same functions** to the whole domain

   \[
   Z_{j+1}\cap\Omega_{j+1}
   \]

   by a new decomposition of unity. This directly extends the displayed radius \(g_j^{-1}\delta_j\) beyond the original boundary strip to the whole regular fluctuation subdomain of the component being integrated.

5. **LFR I, p.187, paragraph before (1.53):** after the removal of redundant restrictions, the source explicitly says that the remaining characteristic functions in the integral **(1.25)** are **(1.9)** and **(1.27)**, restricting the fluctuation field on \(\Omega_{j+1}\cap Z_{j+1}\) and its corresponding exterior subdomain, respectively. Thus (1.9) actually remains in the integration law on the completed regular domain; it is not merely an auxiliary boundary estimate.

This chain establishes that the later rescaled convention belongs to the ordinary cutoff family shared by the regular interior and the inherited exterior operation. It does not supply a separate literal all-torus integral display in LFR I, and it does not retrospectively change the typography of CMP119 (3.16).

### Size of the radius and consequences

**CMP119, printed p.265, immediately after (3.4),** defines

\[
\delta_k=g_k\frac{A_1}{A_0}p_0(g_k).
\tag{RA2}
\]

Together with the source definition \(p_0(g)=A_0(\log g^{-2})^{p_0}\), the later ordinary rescaled radius is

\[
r_k^\chi=g_k^{-1}\delta_k
=\frac{A_1}{A_0}p_0(g_k)
=A_1(\log g_k^{-2})^{p_0}.
\tag{RA3}
\]

In particular, for fixed positive source constants and sufficiently small \(g_k\),

\[
r_0\le r_k^\chi\le\frac{\epsilon_{\rm cut}}{g_k},
\qquad
4r_k^\chi\le\rho_{\rm ana}
\quad\text{when }\rho_{\rm ana}=\epsilon_{\rm ana}/g_k.
\tag{RA4}
\]

These are elementary consequences of \(g(\log g^{-2})^{p_0}\to0\). They give exactly the radius and analytic-margin regime needed by the threshold-robust regular CMP109/116 analysis, whenever the corresponding regular action and source chart have otherwise been identified. The present analysis removes the rescaled-cutoff convention ambiguity for that use of the later construction; it does not verify all mixed-history analytic domains or boundary interactions.

The cutoff in (RA1) is a supremum of individual independent-bond norms. Products over overlapping cubes impose intersections of these same single-variable norm constraints. They therefore preserve the product-convex nature of the independent-coordinate cutoff used in HC-W; overlap of cubes does not couple distinct variables in the cutoff domain.

### Corroboration, not a substitute for the definition

**LFR II, printed p.380**, states that the failed ordinary fluctuation cutoff \(\chi^{(j-1)c}(R_j)\) produces the factor

\[
\exp\!\left[
-\gamma_0 g_j^{-2}\delta_j^2
(LM_2R_j)^{-d}|R_j|
\right].
\tag{RA5}
\]

This agrees with the explicit rescaled radius in (RA1). The argument for (RA1) above uses the actual definition and its source identifications; it does not reason backwards from (RA5).

The newly introduced **R-component** fluctuation restriction is a different family, with \(\delta'_j\) in place of \(\delta_j\). It must not be used interchangeably with the ordinary cutoff. For example, LFR II p.361 explicitly describes \(V=\exp(i g_kB)\) and \(|B|<g_k^{-1}\delta'_k\), referring to (1.82) [IV]. That is a separate source convention, not the reason for (RA1).

### Sources

- Balaban, CMP119 (1988), 243–285: printed pp.265, 269–270; including pp.267–268 and (3.15)–(3.16).
- Balaban, Large Field Renormalization I, CMP122 (1989), 175–202: printed pp.178, 183, 187; bibliography p.202.
- Balaban, Large Field Renormalization II, CMP122 (1989), 355–392: printed pp.361 and 380.

The cited printed pages fix the cutoff conventions used below.

**Conclusion:** use the later explicit ordinary cutoff \(r_k^\chi=g_k^{-1}\delta_k\), accompanied by the above source chain and the recorded earlier display discrepancy. Do not claim an erratum, an all-history convexity theorem, or a full Yang–Mills existence proof from this clarification.

---

## Part III. Second derivatives, raw moments, and nonlinear covariance

### Results and scope

This part continues the hard-cutoff covariance analysis of Part I. It proves the exact second-derivative transport identity, a spatial tree estimate for its third-cumulant term, and bounds for Hessians of normalized conditional marks. It also proves a weighted raw-moment estimate that is uniform in volume and cutoff radius.

There are two different conclusions.

* A pointwise Hessian estimate holds with an explicit first-gradient term. A uniform pointwise estimate using only the original Hessian is false, even for an even quadratic mark under a truncated Gaussian; Section 7 gives a counterexample.
* An estimate in the actual marginal \(L^p\) law of the retained variables has constants independent of the cutoff radius. It is a Hessian seminorm modulo constants in the scalar invariant sector. This is the norm appropriate for combining the estimate with posterior-weighted marked transport.

The starting minimizing-field insertion acquires a localized Hessian bound \(Cg_k^2h^{-4}\) from the source's complex analytic response estimates. Weighted raw moments then improve its nonlinear covariance to

\[
C\left(g_k^2\epsilon_{\rm bg}^2+g_k^4\right)
h^{-8}e^{-c|x-y|/h},
\tag{HT0}
\]

with the actual regular hard cutoff retained. Under
\(\epsilon_{\rm bg}\le Cg_kP_k\), this is
\(Cg_k^4(1+P_k^2)h^{-8}e^{-c|x-y|/h}\).

The full-torus regular CMP109/116 carrier is the source-verified application. The exact old mark is treated as the actual function being integrated, with its stated derivative norm as input; it is not replaced by a minimizing-field observable. General coarse-background derivatives and multiscale R/boundary histories remain separate source interfaces, detailed in Section 10.

### 1. Setting and analysis of the preceding cutoff proof

Let

\[
\mu(dA)=Z^{-1}\mathbf1_D(A)e^{-H(A)}\,dA,\qquad
D=\prod_{i\in I}D_i,
\tag{HT1}
\]

where \(D_i\) are bounded convex bodies containing \(0\) in their interiors. The matrix-norm balls of the actual independent starred fluctuation coordinates satisfy this condition. Assume the coercive local precision and small weighted Hessian hypotheses of the preceding note, so that

\[
H''\ge m_0I,\qquad
\operatorname{Sym}(W H''W^{-1})\ge\lambda I
\tag{HT2}
\]

for the spatial weights used below, with positive constants independent of volume and cutoff radius.

The preceding proof gives

\[
|\operatorname{Cov}_{\mu}(f,g)|
\le\lambda^{-1}
\|W\nabla f\|_2\|W^{-1}\nabla g\|_2,
\tag{HT3}
\]

and

\[
\operatorname{Ent}_{\mu}(u^2)
\le \frac2{m_0}\mu|\nabla u|^2.
\tag{HT4}
\]

The following points are used.

1. Because \(H''\) is symmetric,
   \(\operatorname{Sym}(W^{-1}H''W)=\operatorname{Sym}(WH''W^{-1})\). Thus the accretivity assumption is exactly the one needed by contraction in the \(W^{-1}\) distance.
2. The normal cone of a product is the product of the factor normal cones. Positive scalar weights on each factor preserve its normal cone. This covers nonsmooth norm balls and corners; a smooth-boundary approximation is not being assumed.
3. The semigroup gradient estimate follows from difference quotients and the fundamental theorem of calculus along a segment inside \(D\). It does not require differentiation of a reflected stochastic flow.
4. The covariance and entropy identities use the Neumann Dirichlet form. The boundary term is already represented by reflection, and no untruncated Gaussian integration-by-parts identity is substituted.
5. A finite-dimensional Lipschitz extension of the drift can be used for existence of the reflected process. Its convexity or locality outside \(D\) is irrelevant because the process remains in \(D\).

The only process-theoretic import is the standard existence and Gibbs reversibility of normally reflected diffusion in a convex body, as explicitly stated in Bubeck–Eldan–Lehec, Section 3.1. No gap in the weighted argument or its logarithmic Sobolev consequence was found under the stated product-domain and block-scalar-weight hypotheses. A nonproduct nonlinear cutoff would require a different argument.

### 2. Exact second derivative of a normalized conditional mark

Split the coordinates into internal variables \(u\) and retained variables \(y\). For fixed \(y\),

\[
\mu_y(du)
=Z(y)^{-1}\mathbf1_{D_{\rm int}}(u)e^{-H(u,y)}\,du,
\qquad
Tf(y)=\mu_y f(u,y).
\tag{HT5}
\]

The domain and its coordinate measure are independent of \(y\). Derivatives below are ordinary coordinate derivatives, or derivatives in fixed unit directions in the relevant Lie-algebra blocks. Write

\[
f_j=\partial_{y_j}f,\quad
H_j=\partial_{y_j}H,\quad
f_{jk}=\partial_{y_j}\partial_{y_k}f,\quad
H_{jk}=\partial_{y_j}\partial_{y_k}H.
\]

The first derivative is

\[
\partial_jTf
=\mu_y f_j-\operatorname{Cov}_{\mu_y}(f,H_j).
\tag{HT6}
\]

Differentiating once more gives the exact formula

\[
\boxed{
\begin{aligned}
\partial_j\partial_kTf
={}&\mu_y f_{jk}
-\operatorname{Cov}_{\mu_y}(f_j,H_k)
-\operatorname{Cov}_{\mu_y}(f_k,H_j)\\
&-\operatorname{Cov}_{\mu_y}(f,H_{jk})
+\kappa_{3,\mu_y}(f,H_j,H_k).
\end{aligned}}
\tag{HT7}
\]

Here
\(\kappa_3(f,g,h)=\mu_y[(f-\mu_yf)(g-\mu_yg)(h-\mu_yh)]\).

For verification, direct differentiation of a covariance gives

\[
\partial_k\operatorname{Cov}_{\mu_y}(f,g)
=
\operatorname{Cov}_{\mu_y}(f_k,g)
+\operatorname{Cov}_{\mu_y}(f,g_k)
-\kappa_{3,\mu_y}(f,g,H_k).
\tag{HT8}
\]

Applying (HT8) to (HT6) proves (HT7), including its signs and all normalization terms. At finite volume the smoothness and compact cutoff domain justify differentiation under the integral. Appropriate Sobolev versions follow by approximation.

No estimate for \(Z(y)^{-1}\) occurs. Additive \(y\)-dependent constants in \(H\) drop out of the centered terms. Additive constants in \(f\) also drop out of its Hessian transport.

### 3. A three-point tree bound from weighted covariance

For three positions define their metric minimum-spanning-tree length

\[
\tau(x_1,x_2,x_3)
=\min\{
d_{12}+d_{13},\ d_{12}+d_{23},\ d_{13}+d_{23}
\}.
\tag{HT9}
\]

Suppose \(F_a\), \(a=1,2,3\), satisfy localized pointwise gradients

\[
|\nabla_iF_a|\le A_a e^{-\gamma d(i,x_a)}.
\tag{HT10}
\]

Center \(F_a\) under the relevant conditional law. The identity

\[
\kappa_3(F_1,F_2,F_3)
=\operatorname{Cov}(F_1,\overline F_2\,\overline F_3)
\tag{HT11}
\]

and the product rule give

\[
\nabla_i(\overline F_2\,\overline F_3)
=(\nabla_iF_2)\overline F_3
+\overline F_2(\nabla_iF_3).
\tag{HT12}
\]

The ordinary Poincaré inequality implies
\(\|\overline F_a\|_2\le C A_a/\sqrt{m_0}\).
Use (HT3), a weight centered at \(x_1\), and summability of lattice exponentials. For some fixed \(0<\alpha<\gamma\),

\[
|\kappa_3(F_1,F_2,F_3)|
\le
\frac{C A_1A_2A_3}{\lambda\sqrt{m_0}}
\left(e^{-\alpha d_{12}}+e^{-\alpha d_{13}}\right).
\tag{HT13}
\]

Repeat with each of the three functions as the covariance's first argument. If the pair distances in increasing order are \(r_1\le r_2\le r_3\), the largest of the three nearest-neighbor distances is \(r_2\), while
\(\tau=r_1+r_2\le2r_2\). Taking the best of the three bounds proves

\[
\boxed{
|\kappa_3(F_1,F_2,F_3)|
\le
\frac{C A_1A_2A_3}{\lambda\sqrt{m_0}}
e^{-\alpha\tau(x_1,x_2,x_3)/2}.
}
\tag{HT14}
\]

This proof uses no derivative of a Poisson solution and no third derivative of the mark. The fixed loss in spatial exponent is explicit.

#### A version with a mark gradient in \(L^4\)

If \(F_1=f\) has only
\[
\|\nabla_if\|_{L^4(\mu_y)}
\le G_x(y)e^{-\beta d(i,x)},
\tag{HT15}
\]
while \(F_2,F_3\) have the pointwise profiles (HT10), the same conclusion holds with \(A_1=G_x(y)\) and a smaller fixed exponent.

For the representation rooted at \(F_1\), \(L^2\) gradients suffice. In the two other representations, Hölder bounds
\(\|\overline F_a\nabla_if\|_2\) by
\(\|\overline F_a\|_4\|\nabla_if\|_4\).
The scores' centered \(L^4\) moments are bounded by \(CA_a/\sqrt{m_0}\). This follows either from (HT4), or by applying Poincaré to \(\overline F_a^2\) and solving the resulting quadratic inequality. The term
\(\overline f\nabla_iF_a\) needs only
\(\|\overline f\|_2\le m_0^{-1/2}\|\nabla f\|_2\).
Thus all three symmetric bounds retain the same factor \(G_x(y)\).

More generally, all three functions may have localized gradients in \(L^4\), with amplitudes \(A_1,A_2,A_3\). Apply Hölder to both factors in (HT12), and use the \(L^4\) Poincaré estimate for the centered functions. The three symmetric bounds, and therefore (HT14), are unchanged up to an absolute constant. This version is useful when a score gradient is linear in the fluctuation field.

### 4. Pointwise Hessian transport, with the necessary first-gradient term

Assume the full carrier has

\[
|H''_{ij}(A)|\le B_2e^{-\nu d(i,j)},\qquad
|H'''_{ijk}(A)|\le B_3e^{-\nu\tau(i,j,k)}.
\tag{HT16}
\]

For a mark rooted at \(x\), assume

\[
|\nabla_if_x|\le A_1e^{-\gamma d(i,x)},\qquad
|\nabla_i\nabla_jf_x|
\le A_2e^{-\gamma\tau(x,i,j)}.
\tag{HT17}
\]

Every conditional law obtained by fixing any subset of the coordinates retains the internal coercivity and weighted covariance constants. Apply (HT7).

* Its direct Hessian term is bounded by \(A_2e^{-\gamma\tau(x,j,k)}\).
* For \(\operatorname{Cov}(f_j,H_k)\), use
  \[
  |\nabla_if_j|
  \le
  A_2e^{-\gamma d(x,j)/2}e^{-\gamma d(x,i)/2},
  \tag{HT18}
  \]
  and the \(k\)-localized column \(H''_{ik}\).
* For \(\operatorname{Cov}(f,H_{jk})\), the relevant score gradient is
  \(H'''_{ijk}\). Split its tree exponent in the same way.
* For the last term, apply (HT14) to \(f,H_j,H_k\), whose gradient amplitudes are \(A_1,B_2,B_2\).

For a fixed \(c>0\) depending only on the input exponents and geometric summability constants, this proves

\[
\boxed{
|\partial_j\partial_kTf_x(y)|
\le
C\left[
A_2\left(1+\frac{B_2}{\lambda}\right)
+A_1\left(
\frac{B_3}{\lambda}
+\frac{B_2^2}{\lambda\sqrt{m_0}}
\right)
\right]e^{-c\tau(x,j,k)}.
}
\tag{HT19}
\]

No third derivative of \(f\) is needed. The third derivative of \(H\) enters only in the mixed second-score term of (HT7). The cumulant is controlled using the second derivative of \(H\) and the ordinary centered score moments.

The constant is independent of the subset integrated and its number of connected components. Successive integrations inside the same original carrier equal integration over their union. Applying (HT19) directly to the union avoids an artificial multiplication of constants for each subdivision.

### 5. Weighted raw moments without a zero-mean assumption

Here is the additional estimate needed to replace cutoff-radius factors by actual moments. It does not assume that the carrier is even or centered.

Let \(b=\nabla H(0)\). For a fixed current-unit point \(x\), put

\[
W_x=\operatorname{diag}_i(e^{-\alpha d(x,i)}I_{n_i}),\qquad
T_x=\operatorname{tr}W_x^2,\qquad
B_x=\|W_xb\|.
\tag{HT20}
\]

Assume weighted coercivity with this \(W_x\), and denote its lower bound by \(\lambda\). Since \(0\in D_i\), the normal reflection satisfies

\[
\langle W_x^2A,n\rangle\ge0
\quad\hbox{for }n\in N_D(A).
\tag{HT21}
\]

The mean-value formula gives

\[
\langle W_x^2A,\nabla H(A)\rangle
\ge\lambda|W_xA|^2-B_x|W_xA|.
\tag{HT22}
\]

Run the reflected diffusion in stationarity. For
\(q(A)=|W_xA|^2\), the Itô formula for \(q^{p/2}\), \(p\ge2\), has a nonpositive reflection term. Its bulk terms, using
\(|W_x^2A|^2\le\|W_x\|^2q\), imply

\[
\lambda\,\mu q^{p/2}
\le
\bigl(T_x+(p-2)\|W_x\|^2\bigr)\mu q^{p/2-1}
+B_x\mu q^{p/2-1/2}.
\tag{HT23}
\]

One may first use \(q+\epsilon\) and pass to the limit at \(q=0\). Let
\(R_p=\||W_xA|\|_{L^p(\mu)}\). Hölder's inequality yields

\[
\lambda R_p^2
\le T_x+(p-2)\|W_x\|^2+B_xR_p.
\tag{HT24}
\]

Solving this scalar quadratic gives

\[
\boxed{
\||W_xA|\|_p
\le
\frac{B_x}{\lambda}
+\sqrt{\frac{T_x+(p-2)\|W_x\|^2}{\lambda}}.
}
\tag{HT25}
\]

On a current-unit lattice, \(T_x\le C_\alpha\) uniformly in volume, and \(\|W_x\|\le1\). If \(\sup_i|b_i|\le b_0\), then \(B_x\le C_\alpha b_0\). In particular,

\[
\boxed{
\|A_x\|_p\le C_\alpha
\left(\frac{b_0}{\lambda}+\sqrt{\frac{p}{\lambda}}\right),
\qquad p\ge2.
}
\tag{HT26}
\]

This is a raw moment bound, not a bound about an assumed zero mean. Its constants do not involve the cutoff radii.

The estimate is applied to the original joint regular carrier. A conditional law at an arbitrary retained configuration can have a large linear source and need not satisfy a uniform bound on \(\nabla_uH(0,y)\). Posterior integration and conditional Jensen, rather than a false uniform conditional centering assertion, are used next.

### 6. Hessian transport in the actual marginal \(L^p\) law

Let \(\nu\) be the retained-variable marginal of \(\mu\). For \(p\ge4\), define the rooted Hessian seminorm

\[
\mathcal H_{\gamma,p}(f_x;\mu)
:=
\sup_{i,j}
e^{\gamma\tau(x,i,j)}
\|\nabla_i\nabla_jf_x\|_{L^p(\mu)}
=A_{2,p}.
\tag{HT27}
\]

Let \(0<\beta<\gamma/2\) be small enough for the weighted covariance estimates, and define

\[
K_{1,p}
:=
\left(
\sum_i e^{2\beta d(x,i)}
\|\nabla_if_x\|_{L^p(\mu)}^2
\right)^{1/2}.
\tag{HT28}
\]

An internal conditional envelope is

\[
G_x(y)
:=
\left(
\sum_{i\in I_{\rm int}}
e^{2\beta d(x,i)}
\|\nabla_if_x\|_{L^4(\mu_y)}^2
\right)^{1/2}.
\tag{HT29}
\]

Conditional Jensen and Minkowski give

\[
\|G_x\|_{L^p(\nu)}\le K_{1,p},\qquad p\ge4.
\tag{HT30}
\]

Apply (HT7), using (HT15) for the cumulant. For the terms involving \(f_{ij}\), use their conditional \(L^2\) norms and then posterior Jensen. The same exponential-sum estimates as in Section 4 prove

\[
\boxed{
\mathcal H_{c,p}(Tf_x;\nu)
\le
C\left[
A_{2,p}\left(1+\frac{B_2}{\lambda}\right)
+K_{1,p}\left(
\frac{B_3}{\lambda}
+\frac{B_2^2}{\lambda\sqrt{m_0}}
\right)
\right].
}
\tag{HT31}
\]

This is an estimate for the exact normalized old mark. In particular, the norm on the left is taken in its actual marginal probability law, not in an auxiliary reference law.

#### 6.1 A Hessian-only norm in the invariant sector

The logarithmic Sobolev inequality implies the useful \(L^p\) Poincaré estimate

\[
\boxed{
\|u-\mu u\|_p
\le\sqrt{\frac{p-1}{m_0}}\,
\||\nabla u|\|_p,\qquad p\ge2.
}
\tag{HT32}
\]

For completeness, apply (HT4) to \(|u-\mu u|^{q/2}\). The identity

\[
\frac{d}{dq}\|u-\mu u\|_q^2
=\frac2{q^2}
\|u-\mu u\|_q^{2-q}
\operatorname{Ent}_{\mu}(|u-\mu u|^q)
\tag{HT33}
\]

and Hölder give
\[
\frac{d}{dq}\|u-\mu u\|_q^2
\le m_0^{-1}\||\nabla u|\|_q^2.
\]
Integrating from \(2\) to \(p\), with the ordinary Poincaré bound at \(2\), proves (HT32). Positive regularization handles zeros.

Apply this to each component of \(\nabla_if_x\). If

\[
\mu\nabla_if_x=0\quad\hbox{for every }i,
\tag{HT34}
\]

then the localized Hessian norm gives

\[
K_{1,p}\le C\sqrt{p/m_0}\,A_{2,p}.
\tag{HT35}
\]

Therefore

\[
\boxed{
\mathcal H_{c,p}(Tf_x;\nu)
\le
C A_{2,p}
\left[
1+\frac{B_2}{\lambda}
+\frac{\sqrt p\,B_3}{\lambda\sqrt{m_0}}
+\frac{\sqrt p\,B_2^2}{\lambda m_0}
\right].
}
\tag{HT36}
\]

This closes a same-\(p\) Hessian estimate. There is no growth of a required moment exponent from one subdivision to the next.

One actual source of (HT34) is a scalar mark and a joint carrier invariant under simultaneous global adjoint transformations, with a semisimple gauge Lie algebra. The vector \(\mu\nabla_if\) would have to be fixed by every adjoint transformation; the semisimple adjoint representation has no nonzero invariant vector. Both the retained marginal and the transported mark retain this invariance.

In this invariant function space, the Hessian seminorm is a norm modulo constants: an affine invariant scalar function has zero linear part. This explains precisely where gauge symmetry makes a Hessian-only norm appropriate.

A fixed nontrivial background need not leave the internal conditional law invariant under adjoint transformations of \(A\) alone. The background transforms too. Thus one must not impose (HT34) at a generic fixed background merely by saying that the original observable is gauge invariant.

#### 6.2 Zero first jet plus raw moments, without invariant centering

Another route uses a pointwise Hessian profile \(A_{2,\infty}\), the raw moments (HT26), and a first jet

\[
|\nabla_if_x(0)|\le A_1^{(0)}e^{-\gamma d(x,i)}.
\tag{HT37}
\]

Because \(D\) is convex and contains \(0\),

\[
\nabla_if_x(A)
=\nabla_if_x(0)
+\int_0^1\sum_j
\nabla_j\nabla_if_x(tA)\,A_j\,dt.
\tag{HT38}
\]

The tree profile and (HT26) give

\[
K_{1,p}
\le C\left[
A_1^{(0)}
+A_{2,\infty}
\left(\frac{b_0}{\lambda}+\sqrt{\frac p\lambda}\right)
\right].
\tag{HT39}
\]

Use this in (HT31). When gauge symmetry at the actual expansion point kills the first jet, \(A_1^{(0)}=0\). This version requires no assumption that the law is centered or invariant. It also shows explicitly how a nonzero background first jet enters.

Both versions are uniform in the chosen subset of coordinates. For successive integrations within one fixed carrier, the tower property again permits a single application to the union.

### 7. Why pointwise Hessian-only transport cannot be uniform

The distinction between (HT19) and (HT36) is necessary.

For \(R>1\), consider

\[
D_R=[-R,R]^2,\qquad
H(a,y)=\tfrac12a^2-2ay+\tfrac52y^2,\qquad f(a,y)=a^2.
\tag{HT40}
\]

The precision has eigenvalues \(3\pm2\sqrt2\), independent of \(R\). The carrier is invariant under \((a,y)\mapsto(-a,-y)\), and \(f\) has zero first jet at \(0\) and constant Hessian \(f_{aa}=2\).

Conditional on \(y\), \(a\) is \(N(2y,1)\) truncated to \([-R,R]\). Let
\(s=2y-R\) and \(u=a-R\). Write \(m_R(s)=E_su\) and
\(q_R(s)=E_su^2\), for \(u\in[-2R,0]\). Then

\[
Tf(y)=R^2+2Rm_R(s)+q_R(s),\qquad
(Tf)''(R/2)=8R\,m_R''(0)+4q_R''(0).
\tag{HT41}
\]

As \(R\to\infty\), the first two derivatives of these moments converge to those of a normal variable of mean \(s\), truncated above at \(0\). This follows by differentiating its Gaussian integrals; the removed tail has Gaussian decay with polynomial derivative factors.

For this limiting law,

\[
m_\infty(s)=s-\frac{\phi(s)}{\Phi(-s)},\qquad
m_\infty''(0)=\sqrt{\frac2\pi}\left(1-\frac4\pi\right)\ne0,
\tag{HT42}
\]

while \(q_R''(0)\) remains bounded. Therefore
\[
|(Tf)''(R/2)|\asymp R.
\tag{HT43}
\]

The original Hessian remains equal to \(2\). Thus zero first jet, convexity, locality and the hard cutoff do not imply a pointwise Hessian-only bound independent of \(R\).

The joint drift at \(0\) is zero, so the joint raw moments are uniformly bounded by Section 5. The exceptional retained fields \(y\approx R/2\) are rare in that joint law. Posterior \(L^p\) estimates use this fact without discarding the cutoff or asserting a false uniform bound.

### 8. Source verification for \(H'''\) and the drift at zero

Fix the admitted full-torus regular CMP109/116 carrier, its background, and a complex independent-coordinate radius \(\rho\ge1\) with an explicit margin
\[
4r_k^\chi\le\rho.
\tag{HT44}
\]

The companion potential analysis supplies localized activities for the complete regular exponent,
\[
{\cal V}_{\rm reg}(A)=\sum_YV_Y(A),\qquad
|V_Y|\le a_Y(g_k\rho^3+E_*),
\tag{HT45}
\]
with summability after polynomial support factors and a fixed fraction of the localization exponent are paid. Here \(E_*\) includes the bounded analytic effective-action and Haar/Jacobian pieces.

Three-coordinate Cauchy estimates give

\[
|\partial_i\partial_j\partial_kV_Y|
\le C a_Y(g_k+E_*\rho^{-3}).
\tag{HT46}
\]

The derivative vanishes unless all differentiated coordinates belong to the activity support. Since
\(\tau(i,j,k)\le2\operatorname{diam}Y\), summing the activities after sacrificing an exponential factor gives (HT16) with

\[
B_3\le C(g_k+E_*\rho^{-3}).
\tag{HT47}
\]

The full second-derivative coefficient \(B_2\) is bounded by the local precision and the small interaction Hessian already established.

For the drift at zero, CMP116 Lemma 2, (1.42), writes an activity as a quadratic form in \(A\), with an analytic coefficient, plus a bounded analytic term \(V_Y'\). The quadratic piece has zero first jet. Cauchy on \(V_Y'\), followed by localized summation, gives

\[
\sup_i|\partial_i{\cal V}_{\rm reg}(0)|
\le C E_*/\rho.
\tag{HT48}
\]

The classical linear term has been removed by the constrained stationary equation; this cancellation is stated in CMP109 printed p.267 immediately before (2.11). Thus the full-torus law has no exterior linear source, and

\[
b_0=\sup_i|\partial_iH(0)|\le C E_*/\rho.
\tag{HT49}
\]

This discharges the raw-moment hypothesis for that complete regular law. With
\(\rho\asymp\epsilon_{\rm ana}/g_k\), \(b_0\) is bounded uniformly and
\(B_3=O(g_k)\), with fixed source constants.

For an arbitrary fixed-exterior conditional law there is an additional linear source. Equations (HT48)–(HT49) do not say that this conditional source is uniformly bounded. The use of the original joint carrier and posterior Jensen is deliberate.

The extension from the full-torus regular action to every CMP119 multiscale boundary/R contribution requires its own analytic-domain and support verification. It is not a consequence of (HT45) alone.

### 9. Actual nonlinear insertion: Hessian, sharp moments and covariance

Let

\[
F_x(A)=Q^W\!\left(
U_k(e^{i[g_kCA-h_{\rm c}D(g_kCA)]}V^{(k)});x
\right).
\tag{HT50}
\]

The same statements apply componentwise to the clover and leaf quadratic insertions. This is the full nonlinear observable on the admitted minimizer.

#### 9.1 Complex response and Cauchy give the Hessian

CMP102 Proposition 9, printed pp.307–309, places the minimizing field in a complex analytic domain and includes the derivative estimate (190) there. The text of that proposition explicitly extends the preceding properties to the analytic external-background setting. CMP116 (1.19)–(1.21) supplies the analytic independent-coordinate map and its current-unit bounds.

Take a complex independent-coordinate polydisc of radius
\[
\rho_F\asymp\epsilon_{\rm ana}/g_k
\tag{HT51}
\]
which contains the actual real cutoff with a fixed margin and remains inside these source domains. The background must also have the corresponding regularity margin.

The proof of LR-B extends to this complex domain. Unitary conjugation is replaced by uniformly bounded conjugation in the small complex neighborhood. For the scalar Wilson term the holomorphic continuation is
\[
1-\tfrac12\operatorname{tr}(P+P^{-1}).
\]
Its derivative is bounded by \(C|P-I||\dot P|\), so the same fine-plaquette cancellation applies. Clover leaves use \(P-P^{-1}\) and have the same analytic continuation. Thus the internal derivative satisfies

\[
|\partial_{A_i}F_x|
\le Cg_k\epsilon_{\rm ana}h^{-4}e^{-\gamma d(x,i)}
\tag{HT52}
\]

throughout the smaller complex polydisc.

Cauchy in coordinate \(j\), using the fixed margin of (HT51), gives
\[
|\partial_{A_j}\partial_{A_i}F_x|
\le Cg_k^2h^{-4}e^{-\gamma d(x,i)}.
\tag{HT53}
\]
Exchange \(i,j\) and use symmetry of the second derivative. Since
\(\tau(x,i,j)\le d(x,i)+d(x,j)\le2\max(d(x,i),d(x,j))\),

\[
\boxed{
|\partial_{A_i}\partial_{A_j}F_x|
\le Cg_k^2h^{-4}e^{-\gamma\tau(x,i,j)/2}.
}
\tag{HT54}
\]

This is a new second-derivative bound for the actual minimizing observable. It does not establish the corresponding norm for an old transported mark; (HT31) and (HT36) are the tools for transporting such a norm once its incoming value is known.

#### 9.2 Raw moments remove the cutoff radius from the gradient amplitude

At \(A=0\), the actual background first derivative obeys

\[
|\partial_{A_i}F_x(0)|
\le Cg_k\epsilon_{\rm bg}h^{-4}e^{-c d(x,i)}.
\tag{HT55}
\]

Use the line-segment formula (HT38), the Hessian bound (HT54), and the raw moments (HT26), with the source bound (HT49). For every \(p\ge2\),

\[
\boxed{
\|\partial_{A_i}F_x\|_{L^p(\mu)}
\le
Ch^{-4}
\left(g_k\epsilon_{\rm bg}+g_k^2\sqrt p\right)
e^{-c' d(x,i)}.
}
\tag{HT56}
\]

Constants absorb the uniformly bounded drift and coercivity parameters. Unlike the pointwise gradient bound, (HT56) has no factor of the cutoff radius.

Applying the \(L^p\) Poincaré estimate (HT32),

\[
\boxed{
\|F_x-\mu F_x\|_{L^p(\mu)}
\le
Ch^{-4}
\left(\sqrt p\,g_k\epsilon_{\rm bg}+p\,g_k^2\right),
\qquad p\ge2.
}
\tag{HT57}
\]

In particular, with
\[
\mathcal B_x=h^{-4}(g_k\epsilon_{\rm bg}+g_k^2),
\tag{HT58}
\]
one has localized gradient moments at most \(C\sqrt p\,\mathcal B_x\) and centered mark moments at most \(Cp\,\mathcal B_x\). These are the inputs for the companion all-order connected calculation.

Finally apply weighted covariance to (HT56) at \(p=2\):

\[
\boxed{
|\operatorname{Cov}_{\mu}(F_x,F_y)|
\le
C(g_k^2\epsilon_{\rm bg}^2+g_k^4)
h^{-8}e^{-c|x-y|/h}.
}
\tag{HT59}
\]

The density is the complete regular interacting density and the actual hard cutoff. The precision, interaction, raw-drift and complex-response margins must all be the ones checked above on this same carrier. No observable Taylor terms have been dropped.

### 10. Genuine coarse-background parameters: the formula survives, the hypotheses change

The fixed cutoff is useful beyond partial integration in coordinates of one joint carrier. After fixing the history geometry, use a local chart \(y\) for the retained coarse background. The regular interior indicator acts on the independent fluctuation \(A\), not on its nonlinear dependent-coordinate image. Its radii and coordinate measure are independent of the background chart. All coordinate Jacobians belong in \(H_y(A)\).

Consequently (HT7) remains an exact formula for
\[
T_yf_y=\frac{\int_{D}f_y(A)e^{-H_y(A)}\,dA}
{\int_De^{-H_y(A)}\,dA}.
\tag{HT60}
\]

However, the mixed score derivatives now required are

\[
\nabla_A\partial_{y_j}H_y,\qquad
\nabla_A\partial_{y_j}\partial_{y_k}H_y.
\tag{HT61}
\]

They are not merely columns of the internal \(A\)-Hessian and \(A\)-third derivative. For example, if
\[
H_y(A)=\tfrac12\langle A,M_yA\rangle+\langle\ell_y,A\rangle+V_y(A),
\]
then
\[
\begin{aligned}
\partial_{A_i}\partial_{y_j}H_y
&=\sum_l(\partial_{y_j}M_y)_{il}A_l
+\partial_{y_j}(\ell_y)_i
+\partial_{A_i}\partial_{y_j}V_y,\\
\partial_{A_i}\partial_{y_j}\partial_{y_k}H_y
&=\sum_l(\partial_{y_j}\partial_{y_k}M_y)_{il}A_l
+\partial_{y_j}\partial_{y_k}(\ell_y)_i
+\partial_{A_i}\partial_{y_j}\partial_{y_k}V_y.
\end{aligned}
\tag{HT62}
\]

The mark also needs its direct \(\partial_y^2 f_y\) and mixed
\(\nabla_A\partial_y f_y\) bounds.

Thus a sufficient background-transport theorem has exactly four inputs: a localized internal mark gradient; a localized mixed mark Hessian and direct background Hessian; a localized first mixed score; and a localized second mixed score. Formula (HT7), weighted covariance, and the three-point lemma then give the same tree structure.

More explicitly, the following moment assumptions suffice, uniformly over the admitted background chart:

\[
\begin{aligned}
\|\nabla_{A_i}f_y\|_{L^4(\mu_y)}
&\le A_{10}e^{-\gamma d(i,x)},\\
\|\nabla_{A_i}\partial_{y_j}f_y\|_{L^2(\mu_y)}
&\le A_{11}e^{-\gamma\tau(x,i,j)},\\
\mu_y|\partial_{y_j}\partial_{y_k}f_y|
&\le A_{02}e^{-\gamma\tau(x,j,k)},\\
\|\nabla_{A_i}\partial_{y_j}H_y\|_{L^4(\mu_y)}
&\le B_{11}e^{-\nu d(i,j)},\\
\|\nabla_{A_i}\partial_{y_j}\partial_{y_k}H_y\|_{L^2(\mu_y)}
&\le B_{12}e^{-\nu\tau(i,j,k)}.
\end{aligned}
\tag{HT63}
\]

The internal and background labels are placed in the same current-unit geometry. Their spacings may differ by the fixed block factor. The all-\(L^4\) version of Section 3 and (HT7) prove

\[
\boxed{
|\partial_{y_j}\partial_{y_k}T_yf_y|
\le
C\left[
A_{02}+\frac{A_{11}B_{11}}{\lambda}
+\frac{A_{10}B_{12}}{\lambda}
+\frac{A_{10}B_{11}^2}{\lambda\sqrt{m_0}}
\right]e^{-c\tau(x,j,k)}.
}
\tag{HT64}
\]

Thus no pointwise bound proportional to the cutoff radius is required for the fluctuation factors in (HT62). For example, localized kernels \(\partial_yM_y\) with a connected tree through the two precision endpoints and the background derivative label, together with (HT26), give the first score estimate in (HT63). A corresponding four-label tree for \(\partial_y^2M_y\) gives the second score estimate after the unused endpoint is summed. Summability costs a fixed fraction of the exponential decay, not a volume factor.

The source's localized analytic propagator expansions suggest a concrete way to obtain (HT61): mark the external background derivative in the random-walk localization domains and use the available complex margin. Differentiating once and twice costs the inverse margin and its square. One must additionally differentiate the source-dependent constraint embedding and minimizing-background map. The analytic-map response from CMP102 and the localized operator expansions are relevant inputs, but their composition with the actual coarse chart and all multiscale analytic radii must be proved.

Raw moments from Section 5 can control the factors \(A_l\) in (HT62), provided the whole family has a uniform drift-at-zero bound. They do not supply localization or smallness of \(\partial_yM_y\), \(\partial_y^2M_y\), or the mixed effective-potential derivatives.

Finally, a history change can change the integration domain or its dimension. The fixed-carrier identity (HT7) cannot be differentiated across such a change without summing or reorganizing the corresponding histories. This is precisely why posterior-weighted marked expansions are still needed for the full route.

### 11. What is now available for the route

| Item | Status supplied by this part |
|---|---|
| Second derivative of normalized old mark | Exact score/covariance/cumulant formula (HT7) |
| Three-point spatial connection | Tree decay (HT14), including an \(L^4\)-gradient version |
| Hessian transport within one carrier | Pointwise estimate (HT19); posterior \(L^p\) estimate (HT31) |
| Hessian norm modulo constants | Closed in the invariant sector by (HT36); no new moment order needed |
| Raw local moments | (HT25)–(HT26), with no zero-mean assumption |
| Source drift at zero | Bound (HT49) for the full-torus complete regular action |
| Actual nonlinear minimizing mark | Hessian (HT54), moments (HT57), sharper covariance (HT59) |
| Subdivision accumulation | Avoided by the tower property within the same original carrier |
| Coarse-background transport | Exact fixed-cutoff formula; mixed source derivatives explicitly identified |
| Every multiscale history / full S2 | Still requires the marked/background/R interface and terminal estimates |

### Source record

* Previous module: **Part I**.
* Balaban, CMP102 (1985), printed pp.307–309, Proposition 9 and (190): complex analytic minimizing-field response.
* Balaban, CMP109 (1987), printed pp.267–268: stationary cancellation of the classical linear term and the independent-coordinate transformation.
* Balaban, CMP116 (1988), (1.19)–(1.21), Lemmas 1–2, (1.33)–(1.43): analytic regular action, local coordinate map, quadratic-plus-bounded activity decomposition.
* Balaban, CMP119 (1988), pp.247–249, 268–272: background-independent starred-bond cutoff on a fixed regular carrier.
* Bubeck–Eldan–Lehec, Section 3.1: reflected diffusion and the truncated Gibbs reversible law. [Primary manuscript](https://arxiv.org/abs/1507.02564).

All derivative identities, moment estimates, tree bounds and Hessian-transport estimates above are derived in this part. The source assumptions determine the carrier on which they apply.

---

## Part IV. Every connected order on one admitted regular carrier

### Result

The hard-cutoff covariance and logarithmic Sobolev estimates also yield a fixed factorial budget for **every connected order on the same regular carrier**. The small-coupling condition used to establish that carrier does not depend on the number of marks.

The spatial decay rate in the estimate below loses a factor \(m-1\) at order \(m\). This is acceptable for the stated integrated estimate: its cost is absorbed into a single factorial exponent. It is explicitly retained, rather than described as an order-independent tree decay rate.

This result applies to actual nonlinear minimizing-field observables under the admitted full-torus regular interacting law. It does not supply the all-history marked induction, contact extensions, or the all-order large-field budget required for the full OS theorem.

### 1. Assumptions and norms

Let \(\mu\) be the actual normalized product-cutoff carrier of Theorem HC-W, with a uniform unweighted gap \(m_0>0\) and weighted gap \(\lambda>0\). Assume its independent coordinate blocks have uniform \(d\)-dimensional volume growth. In the four-dimensional application \(d=4\).

The available exponential Hessian bounds imply that HC-W holds, with this same \(\lambda\), for every weight

\[
W=\operatorname{diag}_b(e^{\alpha\varphi(b)}I_b),
\qquad |\varphi(b)-\varphi(c)|\le d(b,c),
\tag{A1}
\]

where \(\alpha>0\) is a fixed sufficiently small number. The commutator proof uses only the Lipschitz condition in (A1), so distance to a set is allowed as well as distance to one point.

Let real observables \(F_1,\ldots,F_m\), anchored at \(x_1,\ldots,x_m\), satisfy

\[
|\nabla_b F_i|\le A_i e^{-\nu d(b,x_i)},\qquad
0<2\alpha<\nu.
\tag{A2}
\]

Center them by their means under this **single carrier**, writing \(X_i=F_i-\mu F_i\). For \(m\ge2\), this does not change their joint cumulant. HC-LSI and the uniform spatial sum of the squared gradient give

\[
\|X_i\|_{L^p(\mu)}\le C_0 A_i\sqrt p,
\qquad p\ge2.
\tag{A3}
\]

The constants below depend on \(\lambda,m_0,\alpha,\nu\), the growth constants and the fixed coordinate dimension, but not on volume, cutoff radius, or \(m\).

### 2. A separated-product covariance bound

Split the labels into nonempty sets \(I,J\), put \(n=|I|\), \(s=|J|\), \(m=n+s\), and let

\[
R=\min_{i\in I,j\in J}d(x_i,x_j),\quad
P_I=\prod_{i\in I}X_i,\quad P_J=\prod_{j\in J}X_j.
\tag{A4}
\]

Choose \(\varphi(b)=\operatorname{dist}(b,\{x_i:i\in I\})\) in (A1). For each \(i\in I\),

\[
\left(\sum_b e^{2\alpha\varphi(b)}|\nabla_bF_i|^2\right)^{1/2}
\le C A_i.
\tag{A5}
\]

For \(j\in J\), the triangle inequality gives
\(\varphi(b)\ge R-d(b,x_j)\), and hence

\[
\left(\sum_b e^{-2\alpha\varphi(b)}|\nabla_bF_j|^2\right)^{1/2}
\le C A_j e^{-\alpha R}.
\tag{A6}
\]

The product rule, Minkowski, and Hölder with at most \(m-1\) factors now imply

\[
\|W\nabla P_I\|_2
\le Cn(C_1\sqrt m)^{n-1}\prod_{i\in I}A_i,
\]

\[
\|W^{-1}\nabla P_J\|_2
\le Cs(C_1\sqrt m)^{s-1}\prod_{j\in J}A_j\,e^{-\alpha R}.
\tag{A7}
\]

An empty product has value one, so these bounds cover singleton groups. Applying HC-W proves

\[
\boxed{
|\operatorname{Cov}_\mu(P_I,P_J)|
\le C_2^{m}ns\,m^{(m-2)/2}
 \left(\prod_{i=1}^m A_i\right)e^{-\alpha R}.
}
\tag{A8}
\]

This is a spatial estimate for products, not just for individual observables.

### 3. A connected cumulant estimate with one factorial exponent

Let \(\nu_{I,J}\) denote the probability law on the vector \((X_1,\ldots,X_m)\) obtained by taking its \(I\)- and \(J\)-marginal laws independently. The order-\(m\) cumulant under this law is zero, because it involves labels from two independent nonempty groups. For a label block \(B\),

\[
\mu\!\prod_{i\in B}X_i-
\nu_{I,J}\!\prod_{i\in B}X_i
=\operatorname{Cov}_\mu
 \left(\prod_{i\in B\cap I}X_i,
       \prod_{i\in B\cap J}X_i\right).
\tag{A9}
\]

The right side vanishes if either intersection is empty. Otherwise (A8), with the total label count \(m\) as an upper bound on all moment orders, supplies an \(e^{-\alpha R}\) factor. Every other block moment has the bound

\[
\left|\mu\prod_{i\in B}X_i\right|,
\left|\nu_{I,J}\prod_{i\in B}X_i\right|
\le (C_3\sqrt m)^{|B|}\prod_{i\in B}A_i.
\tag{A10}
\]

Use the finite moment-cumulant identity

\[
\kappa_m(X_1,\ldots,X_m)
=\sum_{\pi\in\Pi_m}
(-1)^{|\pi|-1}(|\pi|-1)!
\prod_{B\in\pi}\mu\prod_{i\in B}X_i.
\tag{A11}
\]

Subtract the same expression for \(\nu_{I,J}\), which is zero. Telescope each product over the blocks of \(\pi\). There are at most \(|\pi|\) resulting differences. Equations (A8)–(A10) give

\[
|\kappa_m|
\le C_4^m m^2m^{(m-2)/2}
 \left(\prod_i A_i\right)e^{-\alpha R}
 \sum_{\pi\in\Pi_m}|\pi|!.
\tag{A12}
\]

For completeness, the number of partitions into \(q\) ordered blocks is at most
\(m!\binom{m-1}{q-1}\): order the labels, choose the \(q-1\) cut positions, and then forget the order within each block. This representation may overcount, which is harmless. Summing over \(q\),

\[
\sum_{\pi\in\Pi_m}|\pi|!\le m!\,2^{m-1}.
\tag{A13}
\]

Finally, \(m^{m/2}\le e^{m/2}(m!)^{1/2}\), by \(m!\ge(m/e)^m\); polynomial factors in \(m\) can be included in another constant to the power \(m\). Consequently,

\[
\boxed{
|\kappa_m(F_1,\ldots,F_m)|
\le C_5^m(m!)^{3/2}
 \left(\prod_i A_i\right)e^{-\alpha R},\qquad m\ge2.
}
\tag{A14}
\]

This holds for every nontrivial split \(I,J\).

Let \(\tau(x_1,\ldots,x_m)\) be the length of a minimal spanning tree on the anchor points. Delete a longest edge of such a tree. Its two components define a split with cross distance at least the length of the deleted edge: a shorter cross edge would produce a shorter spanning tree. The deleted length is at least \(\tau/(m-1)\). Equation (A14) therefore yields

\[
\boxed{
|\kappa_m(F_1,\ldots,F_m)|
\le C_5^m(m!)^{3/2}
 \left(\prod_i A_i\right)
 \exp\!\left[-\frac{\alpha}{m-1}\tau(x_1,\ldots,x_m)\right].
}
\tag{A15}
\]

Coincident anchors cause no problem; the corresponding distances are zero. Complex observables can be decomposed into real and imaginary parts, at the cost of another factor \(2^m\).

### 4. Spatial summation has a fixed factorial cost

Suppose the anchors range over the current-unit lattice and \(A_i\le A\). Fix \(x_1\). With \(\beta=\alpha/(m-1)\),

\[
e^{-\beta\tau(x_1,\ldots,x_m)}
\le\sum_{T\text{ labeled tree}}
 \prod_{\{i,j\}\in T}e^{-\beta d(x_i,x_j)}.
\tag{A16}
\]

For each tree, successively sum leaf positions. Uniform polynomial volume growth gives
\(\sup_x\sum_y e^{-\beta d(x,y)}\le C\beta^{-d}\) for the relevant small \(\beta\). There are \(m^{m-2}\) labeled trees. Thus

\[
\sum_{x_2,\ldots,x_m}e^{-\alpha\tau/(m-1)}
\le m^{m-2}[C(m-1)^d]^{m-1}
\le C_6^m(m!)^{d+1}.
\tag{A17}
\]

The same estimate holds on finite periodic lattices with uniform growth constants. Combining (A15)–(A17),

\[
\boxed{
\sum_{x_2,\ldots,x_m}
 |\kappa_m(F_{x_1},\ldots,F_{x_m})|
\le C_7^m A^m(m!)^{d+5/2}.
}
\tag{A18}
\]

For \(d=4\), one may use the simpler integer exponent \(7\), uniformly for all \(m\). No claim of sharpness is made.

### 5. Application and the remaining scope

For the actual nonlinear minimizing-field Wilson/clover family on the admitted regular carrier, the earlier derivative bound gives

\[
A_i\le Cg_k\epsilon_{\rm reg}h_k^{-4}.
\tag{A19}
\]

Consequently, at physical anchor points,

\[
|\kappa_m(Q_{x_1},\ldots,Q_{x_m})|
\le C^m(m!)^{3/2}(g_k\epsilon_{\rm reg})^m h_k^{-4m}
\exp\!\left[-\frac{c}{m-1}
 \frac{\tau(x_1,\ldots,x_m)}{h_k}\right].
\tag{A20}
\]

The uniformly bounded offset between a point and its current block center only changes the constant to the power \(m\). The same statement applies componentwise to all 21 tensor marks.

This is a genuine all-order result for that law, including its hard cutoff and normalization. It uses one fixed carrier smallness condition and one fixed factorial exponent. The all-history theorem still needs transported old marks with the required current-scale norm, the large-field estimates at all degrees with one common admissible trajectory, the composition of connected jets across scales, and the required contact extensions. In particular, (A18) is not by itself the continuum OS regularity bound: the physical shell factors and the collision subtractions must be handled in that separate assembly.

**Sources:** The probability-law inputs are HC-W and HC-LSI, proved in Part I from the actual independent-coordinate cutoff and source precision bounds. The combinatorial, interpolation-of-laws, and tree-summation steps (A4)–(A18) are proved explicitly above. No published all-order Yang–Mills theorem is being imported.

### 6. Sharper nonlinear amplitude from raw local moments

The second-derivative transport analysis of Part III gives a useful refinement of the same proof. Suppose, instead of using a pointwise gradient amplitude containing the cutoff radius, one has for every \(p\ge2\)

\[
\|F_i-\mu F_i\|_p\le C p B_i,
\qquad
\|\nabla_bF_i\|_p\le C\sqrt p\, B_i e^{-\nu d(b,x_i)}.
\tag{A21}
\]

The stronger moment dependence is explicit. These bounds follow from a localized Hessian, the first jet at zero, and the new raw-coordinate moment lemma on a joint product-cutoff carrier containing zero. They require a uniform local bound on \(\nabla H(0)\); a conditional exterior linear source cannot be ignored.

Repeat the product proof with Hölder exponents \(2m\). One gradient factor costs \(\sqrt m\), and each of the other mark factors costs \(m\). Therefore the analog of (A8) is

\[
|\operatorname{Cov}(P_I,P_J)|
\le C^m |I||J|\,m^{m-1}
 \left(\prod_iB_i\right)e^{-\alpha R}.
\tag{A22}
\]

The passage from coordinatewise gradient norms to the \(L^{2m}\) norm of the weighted gradient vector uses Minkowski in \(L^m\), followed by the same exponential spatial sum as (A5)–(A6). Thus it is uniform in the number of coordinates.

Other block moments in the cumulant difference now cost \((Cm)^{|B|}\). The partition argument is unchanged, and \(m^m\le e^m m!\). It gives

\[
\boxed{
|\kappa_m(F_1,\ldots,F_m)|
\le C^m(m!)^2\left(\prod_i B_i\right)
 \exp\!\left[-\frac{\alpha}{m-1}\tau(x_1,\ldots,x_m)\right].
}
\tag{A23}
\]

The spatial sum then has factorial exponent \(d+3\), exactly \(7\) in dimension four.

For the nonlinear minimizing-field insertion, the source-admitted complex-domain Hessian estimate and the raw-coordinate moment bound yield

\[
B_i\le C\bigl(g_k\epsilon_{\rm bg}+g_k^2\bigr)h_k^{-4},
\tag{A24}
\]

where \(\epsilon_{\rm bg}\) is the fixed background's curvature-smallness parameter. On the running-small background \(\epsilon_{\rm bg}\le Cg_kP_k\), this is
\(B_i\le Cg_k^2(1+P_k)h_k^{-4}\). Thus (A23) gives the sharper all-order estimate

\[
|\kappa_m(Q_{x_1},\ldots,Q_{x_m})|
\le C^m(m!)^2
 [g_k^2(1+P_k)]^m h_k^{-4m}
 \exp\!\left[-\frac{c}{m-1}
 \frac{\tau(x_1,\ldots,x_m)}{h_k}\right].
\tag{A25}
\]

This statement retains all the complex-domain, actual-law and background hypotheses of Part III. Its current-scale amplitude contains no extra power of the hard-cutoff radius. It still concerns the nonlinear minimizing observable on that carrier, not an arbitrary old insertion from earlier RG/R steps.

---

## Part V. Actual old R numerators, means, and forced composition

**Status:** A new finite-degree module for the actual R operation. This closes the inverse-carrier-denominator issue and the engineering-dimension cost of an insertion while it remains in an unresolved large-field ancestry. It also gives a normalized marked component-gas estimate for bounded marks wholly contained in the old integrated cores. It does not yet control an arbitrary old insertion after it has entered the regular sector, or its covariance under the full outer-field law.

### 1. The marked R ratio

The old insertion on a retained R carrier is

\[
f_\gamma^F(b)=\frac{N_\gamma^F(b)}{N_\gamma(b)}.
\tag{MR1}
\]

It would be unnecessarily strong to require every such ratio to have a uniform physical-scale pointwise bound. The actual law weights that ratio by the same old numerator. Two facts allow a more effective estimate:

1. Conditional Jensen bounds the posterior-weighted ratio without dividing a small carrier mass.
2. LFR II has a cumulative budget for the entire time a large-field component remains unresolved. That budget, rather than only the suppression at its birth, pays a fixed engineering-dimension charge per RG step.

For one or two dimension-four marks, the extra charge is at most \(8\log L\) per occupied component per step. It can be absorbed by increasing the constant in the already present source cost \(C_0M^dR_j^{d+1}d'_j(Z)\). The source proof survives this change after tightening its small-coupling threshold. This gives an actual bound on the marked old integral operation, not a comparison with an observable of the freshly sampled minimizer.

The distinction between a *component operation* and the *full normalized measure* remains essential. Component bounds enter the localized polymer gas and are normalized through connected rooted clusters. A global extensive numerator estimate is never divided crudely by the full partition function.

### 2. Exact posterior estimates for the actual reset

Use the positive reset representation of LFR I, pp.192–194 and 201, (1.73)–(1.76), (1.100)–(1.102). Within one fixed-geometry sector,

\[
N_\gamma(b)=\int \rho_\gamma(u,b)\,du,
\qquad
N_\gamma^F(b)=\int \rho_\gamma(u,b)F(u,b)\,du,
\]

\[
\rho'(v,b)=\sum_\gamma N_\gamma(b)r_\gamma(v\mid b),
\qquad \int r_\gamma(v\mid b)\,dv=1.
\tag{MR2}
\]

All densities and kernels in this paragraph are positive; this is before the signed cluster expansion. Define

\[
w_\gamma(v,b)=\frac{N_\gamma(b)r_\gamma(v\mid b)}{\rho'(v,b)}.
\]

For every deterministic common subtraction \(c\), every \(p\ge1\), and every nonzero carrier,

\[
\boxed{N_\gamma|f_\gamma^F-c|^p
\le N_\gamma^{|F-c|^p}.}
\tag{MR3}
\]

This is Jensen under \(\rho_\gamma/N_\gamma\). Consequently, for any measurable set \(\mathcal B\) of carriers,

\[
\int\mu'(dV)\sum_{\gamma\in\mathcal B}w_\gamma(V)
 |f_\gamma^F-c|^p
\le \frac1Z\sum_{\gamma\in\mathcal B}
 \int \rho_\gamma|F-c|^p.
\tag{MR4}
\]

The right side is an exact restricted marked mass, not a product of an unconditional moment and an unrelated bad-event estimate. No inverse \(N_\gamma\) occurs. No square root of the rare-event penalty is needed when a deterministic seed bound is used directly.

For two marks and arbitrary deterministic \(c_F,c_G\), Cauchy–Schwarz also gives

\[
N_\gamma|f_\gamma^F-c_F||f_\gamma^G-c_G|
\le
\sqrt{N_\gamma^{|F-c_F|^2}N_\gamma^{|G-c_G|^2}},
\tag{MR5}
\]

\[
N_\gamma\left|\operatorname{Cov}_{\rho_\gamma/N_\gamma}(F,G)\right|
\le
\sqrt{N_\gamma^{|F-c_F|^2}N_\gamma^{|G-c_G|^2}}.
\tag{MR6}
\]

The mixture contribution remains the exact expression

\[
\operatorname{Cov}_w(f^F,f^G)
=\frac12\sum_{\gamma,\delta}w_\gamma w_\delta
(f_\gamma^F-f_\delta^F)(f_\gamma^G-f_\delta^G).
\tag{MR7}
\]

Equations (MR3)–(MR6) control magnitude, but do not supply spatial connectivity. The connected cluster estimate in §6 supplies that additional ingredient. A different conditional subtraction on each carrier would change (MR7), and is not permitted.

When geometries differ, use the disjoint union of the carrier-specific exterior spaces and write \(b_\gamma(V)\) in each term. The weights are Radon–Nikodym derivatives of the component output measures with respect to their positive sum. The same proof applies; it does not assume a common exterior coordinate system for inequivalent reset domains.

### 3. The source controls total unresolved age, not just a clean lookback window

LFR I p.177 permits the reset when a component fits in a cube of side \(100MR_k\), and no new large fields have occurred in a preceding clean window of \(N\) steps. This \(N\) is not the component's total age. An old component may be large, merge with another component, or have a failed reset. Replacing its total age by \(N\) would be incorrect.

LFR II pp.383–387, (1.79)–(1.89), deals with precisely this difficulty. After the elementary positive-integral bounds and history summations, each active component carries a factor of the form

\[
\exp\{-\kappa_j(Z)-2p_0(g_{j(Z)})\}.
\tag{MR8}
\]

Here \(j(Z)\) is the first birth scale in the component's ancestry. Let \(S\) be the source cover-and-thicken operation and \(K_j(Z)\) the number of further clean steps needed to make the component eligible for reset. With

\[
q_j(Z)=M^dR_j^{d+1}d'_j(Z),
\tag{MR9}
\]

the source invariant is

\[
\kappa_j(Z)\ge
\sum_{n=j+1}^{j+K_j(Z)}C_0q_n(S^{n-j}Z).
\tag{MR10}
\]

The geometric estimate (1.81) bounds that future sum by

\[
C_{\rm geom} C_0 M^dL^{d+1}R_j^{d+2}
\bigl(d'_j(Z)+1\bigr).
\tag{MR11}
\]

The source obtains this from shrinking the unthickened component until it is small, then allowing the clean window. Its proof gives a bound of the form

\[
K_j(Z)\le C+\left\lceil\log_2(d'_j(Z)+1)\right\rceil+R_j.
\tag{MR12}
\]

Thus a very long clean lifetime requires a large initial region. The birth penalty is proportional to \(p_0(g_j)^2(d'_j(Z)+1)\), which pays for that lifetime. Failed resets provide new \(p_0(g_j)\) reserves. Mergers retain the sum of old reserves and have an additional positive remainder from their birth factors. None of these controls is visible in a bound that keeps only one bare factor \(e^{-p_0(g_j)}\).

### 4. Finite-dimensional age absorption

#### Theorem MR-A: stability of the source large-field budget under a fixed age charge

Fix a finite \(D_*\ge0\). In each history, attach a collection of marks to unresolved large-field ancestors. The total dimension carried by any component is at most \(D_*\). A mark of dimension \(\Delta_i\), inserted at scale \(b_i\), is charged \(\Delta_i\log L\) for each step during which it remains in that unresolved ancestry. Marks can merge; the sum of their dimensions remains at most \(D_*\).

Here \(b_i\) is the scale of the **bounded incoming seed**, not automatically the first birth scale of the component containing it. With the convention that transition \(j-1\to j\) is paid by the active output component at \(j\), the charged transitions are exactly \(j=b_i+1,\ldots,k\). A seed present before the first source step is charged at every step \(1,\ldots,k\). A harmless one-step change of indexing costs at most \(L^{D_*}\).

Then the proof of LFR II (1.79)–(1.89) remains valid after multiplying each history by

\[
\exp\!\left\{\sum_i\Delta_i(k-b_i)\log L\right\},
\tag{MR13}
\]

provided each mark is carried continuously by the unresolved component until the operation at scale \(k\), and the source small-coupling conditions are tightened by a constant depending on \(D_*\). A positive fraction of the source \(p_0\) and spatial-decay reserves can be retained.

More explicitly, take

\[
C_{D_*}=C_0+D_*\log L,
\qquad
H_{D_*}=C_*(1+\beta_0)C_{D_*}M^dL^{d+1},
\tag{MR14}
\]

where \(C_*\) is a fixed geometric constant chosen to dominate the constants in (1.81), the failed-reset comparison and (1.88), with additional fixed slack for the desired spatial-decay rate. Sufficient uniform conditions are

\[
p_0(g_j)\ge H_{D_*}R_j^{d+2},
\qquad
c_{\rm birth}A_1^2p_0(g_j)^2\ge H_{D_*}R_j^{d+2},
\tag{MR15}
\]

where one may take the source birth constant
\(c_{\rm birth}=\frac14\gamma_0 14^{-d}\), reducing it by a fixed factor if part of the birth budget is reserved separately. The quantities denoted \(O(1)\) in the source are not numerically evaluated here; (MR14)–(MR15) state the threshold explicitly in terms of those fixed source constants. They do not introduce a depth-dependent constant.

**Proof.** The active thickened components have linear size greater than \(20MR_j\); see LFR I p.177. Thus, for these components, \(d'_j(Z)\ge1\) in the source block units. In particular,

\[
D_*\log L\le D_*\log L\,q_j(Z).
\tag{MR16}
\]

For a single newborn block before thickening, use \(d'+1\) in the birth estimate. Charging begins in its subsequent active component. This avoids an artificial problem caused by a tree-size convention that assigns size zero to one block.

For any fixed history the number of occupied marked component-steps is bounded by the total number of active component-steps. Multiplying its integrand by (MR13) therefore enlarges the source positive overhead at each step from \(C_0q_j\) to at most \(C_{D_*}q_j\). The positive integration and history summation that lead to (1.79) are otherwise unchanged: the additional factor is bounded history by history before those operations.

It remains to check that the induction tolerates the enlarged constant, which is the useful content of the source budget.

* At birth, (1.82) supplies \(c_{\rm birth}A_1^2p_0^2(d'+1)\). Equations (MR11) and (MR15) pay the current cost and all future clean-step costs with \(C_{D_*}\) in place of \(C_0\).
* At a clean step, the exact update (1.83) subtracts that step's cost. Subtracting the marked age charge gives the same update with the enlarged cost. The future-cost invariant then shifts by one step.
* At a failed reset, the source resets a pessimistic lower budget to \(p_0(g_j)-C_0q_{j+1}(Z)\). Replacing \(C_0\) by \(C_{D_*}\) is valid under (MR15), since this is a small component whose further clean window is bounded as in the source.
* At a merger, old costs and marked ages add. The exact merger identity (1.85) and its tree induction (1.86)–(1.88) are unchanged except for \(C_{D_*}\). The positive surplus \(2(1+\beta_0)^{-1}p_0(g_{j+1})\) pays the fixed geometric merger overhead and the new marked-step charge. Condition (MR15) is chosen to dominate precisely that overhead.

Equivalently, rerun the entire source induction with \(C_{D_*}\) as its overhead constant. This pessimistically charges all components, including unmarked ones, and therefore dominates the marked majorant. At a completed reset the future horizon is zero, leaving a nonnegative budget and the reserved \(2p_0(g_{j(Z)})\) factor. A fixed part of the original geometric penalty can be kept throughout by using extra slack in (MR15). This proves the assertion. \(\square\)

For the scalar two-point problem, \(D_*=8\). In a single clean window with \(N\le R_j\), the elementary special case is

\[
L^{8N}e^{-c p_0(g_j)}
\le e^{-c p_0(g_j)/2}
\quad\text{if}\quad
p_0(g_j)\ge16c^{-1}N\log L.
\tag{MR17}
\]

Theorem MR-A is stronger because it handles arbitrary total age, large birth regions, failed resets and mergers. In the source parameter regime \(R(g)\asymp(\log g^{-2})^{r_0}\), it is enough to choose the exponent in \(p_0(g)\) strictly larger than \((d+2)r_0\), then reduce the coupling threshold. More generally, only \(p_0(g)/R(g)^{d+2}\to\infty\) is needed for this fixed-degree enlargement.

**Important entry-scale limitation.** Suppose the original mark is inserted at scale \(s\), but first enters an unresolved large-field ancestry at a later scale \(b>s\). The theorem pays \(L^{\Delta(k-b)}\). It does not pay the earlier factor \(L^{\Delta(b-s)}\), because there were no corresponding occupied component-steps. If only the original bound \(A h_s^{-\Delta}\) is known at entry, the correct incoming amplitude is \(A_b=A L^{\Delta(b-s)}\), and this factor remains in (MR19). A separate regular marked estimate is needed to replace it by a controlled amplitude at \(h_b\). This is why the microscopic example below is restricted to marks in protected old cores, rather than all marks that ever meet a later large-field region.

This theorem is deliberately finite-degree. Repeating it separately for every \(m\) with \(D_*=4m\) would allow a threshold depending on \(m\). It would not prove the single uniform factorial budget required by the all-order marked theorem.

### 5. Consequence for actual old marked component operations

Let \(\mathcal T'_k(X)\) be the source operation defined by LFR II (1.71). It is formed **after** the matched reset normalizer and Wilson/vacuum terms have been reorganized in (1.70). It is not a raw numerator integrated against an unrelated reference measure. The source states at p.379 that every expression in this operation is localized in \(X\).

Consider at most two bounded gauge-invariant old seeds \(F_i\), with the following precise property: each seed depends only on old variables integrated by the selected component operation, and its support remains in the unresolved ancestry from its insertion scale \(b_i\) to \(k\). Assume

\[
|F_i|\le A_i h_{b_i}^{-\Delta_i},
\qquad h_j=L^j a,
\qquad \sum_i\Delta_i\le D_*.
\tag{MR18}
\]

Apply the operation to the product of the old seeds, without replacing them by a fresh-field observable. Positivity, (MR18) and Theorem MR-A give

\[
\boxed{
\left|\mathcal T'_k(X)\prod_iF_i\right|
\le C\Bigl(\prod_iA_i\Bigr)h_k^{-\sum_i\Delta_i}
e^{-c p_0(g_k)}e^{-\kappa_*d_k(X)}.
}
\tag{MR19}
\]

Here the source's localization conventions for \(d_k\) are retained, and the last exponential is used where the source gives the ordinary tree-size bound. The proof simply rewrites
\(\prod_i h_{b_i}^{-\Delta_i}=h_k^{-\sum_i\Delta_i}\prod_iL^{\Delta_i(k-b_i)}\), then absorbs the second product into the actual history budget. For general still-unprocessed large regions, use the corresponding source operation and its stated geometric/boundary convention rather than silently converting its collapsed metric into physical distance.

There is also a useful analytic statement. LFR II p.380 proves, for the actual analytically continued component operation,

\[
|\mathcal T'_k(X,(U,J))F|
\le \mathcal T'_k(X,(U,0))\!\left(e^{|\sigma|}|F|\right),
\tag{MR20}
\]

and

\[
\left|\frac{\mathcal T'_k(X,(U,J))F}
 {\mathcal T'_k(X,(U,J))1}\right|
\le e^{3\sup|\sigma|}\sup|F|.
\tag{MR21}
\]

These are (1.73) and (1.75). The source explains that only its quadratic form and the term \(V(X^-)\) depend on the complex background, while \(F\) is a function of the integration variables. Therefore a fixed bounded seed of those variables can be integrated against the analytic kernel, and remains analytic in the same background domain by dominated integration. Equation (MR20), with \(\sup|\sigma|\le1\) on the source domain used in (1.92), extends (MR19) there with a fixed factor. No all-orders source-differentiability assertion is needed for these finite coefficients.

If a seed itself depends on the complex background after a change of variables, its uniform analytic norm must also be supplied; the preceding conclusion does not eliminate that requirement. Gauge invariance is needed when the source uses the reversed Faddeev–Popov equivalence in (1.70)–(1.72).

#### An actual microscopic example

The already proved pointwise bounds are

\[
0\le q_W(x)\le24N_c a^{-4},\qquad
|\Phi_{AB}(x)|\le28N_c a^{-4}.
\tag{MR22}
\]

For one or two such old marks whose entire based-loop support lies in retained old integration variables of an unresolved component, (MR18) holds at the initial scale. Equation (MR19) gives the current \(h_k^{-4}\) or \(h_k^{-8}\) power with the large-field penalty. This is a genuinely transported old-mark statement, although its support/ancestry condition is restrictive. A common deterministic subtraction is allowed, with its magnitude included in \(A_i\).

A running normalization or mixing matrix is not automatically harmless. Its known norm must multiply \(A_i\), or a proved per-step growth bound must be added to the age charge. A fixed polynomial in \(g_{b_i}^{-1}\) can be paid from additional birth reserve when \(p_0(g)\) dominates \(\log g^{-1}\); an unspecified mixing growth cannot be paid merely by invoking positivity.

### 6. Normalization and the two spatial cases

The quotient bound (MR21) explains why there is no uncontrolled analytic inverse of a component denominator. It does **not** itself improve the microscopic seed power: dividing (MR19) by a tiny \(\mathcal T'_k1\) would discard the useful rare-component factor. Retain the marked component operation in the activity.

LFR II (1.90)–(1.100) turns the expression in braces in (1.72) into a localized polymer gas and then its logarithm. In the activity estimate (1.92), the source inserts the unmarked bound (1.89). For a marked component, insert (MR19) at exactly that step. All unchanged Mayer links, connected supports and unmarked combinatorial bounds remain available. Fixed extra anchor/localization costs of order \(\exp(CR_k^d)\) are paid by the slack in \(p_0(g_k)\gg R_k^{d+2}\).

For clarity, use nilpotent labels \(t_1,t_2\) and keep only the four coefficients

\[
\zeta_t(X)=\zeta(X)+t_1J_1(X)+t_2J_2(X)+t_1t_2J_{12}(X).
\tag{MR23}
\]

Freeze the unmarked forward reset kernel, its normalizers and its cutoff choices while inserting these labels in the old integrand. Thus no derivative of the reset kernel is included. For the full positive coupling one has exactly
\(\rho'_t(V)=\rho'(V)[1+t_1Q_RF(V)+t_2Q_RG(V)+t_1t_2Q_R(FG)(V)]\), with the appropriate component/history selectors when the marks are restricted to the core class. Its logarithm gives the actual conditional covariance given the physical output \(V\).

For the particular component gas \(\Xi\) in source (1.72), the conditioning is finer: all variables on which the still-unperformed outer operations act are held fixed as well. At that conditioning level the outer factors cancel and the marked density ratio is \(\Xi(t)/\Xi(0)\). Its logarithm gives the conditional covariance at this finer level. Outer integral operations generally act on \(\Xi\); they cannot be treated as a scalar factor after integration. Passing to the physical output or the full measure therefore requires the outer covariance of conditional means analyzed below. This distinction is also why one must not identify \([t_1t_2]\log\Xi\) with full S2. Freezing the kernels throughout avoids the kernel-score term that appears if a source-dependent family of transformations is differentiated instead.

The mixed activity includes the old product when both marks belong to one component. Products of separate root activities give the different-component terms. This finite algebra transports the old insertions exactly; it is not a claim of a uniform nonzero complex source radius.

In the regular R part, whose clusters are disjoint from the remaining large-field regions \(Y_i\), source (1.100) supplies ordinary geometric decay. Provided the seeds satisfy the conditions of §5, the same source expansion gives anchored norms of the form

\[
\mathcal A_i\le C A_i h_k^{-4}\eta_k,
\qquad
\mathcal A_{12}\le C A_1A_2h_k^{-8}\eta_k,
\qquad \eta_k=e^{-c p_0(g_k)}.
\tag{MR24}
\]

The norms include the chosen connectivity and KP weights, with fixed slack below the source's available decay exponent. This assertion is restricted to those localized finite coefficients; it does not assert that every transported insertion already has such a representation.

The rooted KP estimate proved in the companion marked-cluster note states that if the unmarked gas has weighted KP slack \(\theta\), and \(a(X)\ge a_{\min}>0\), then

\[
\left|[t_1t_2]\log\Xi(t)\right|
\le
\left[\mathcal A_{12}+
\frac{\mathcal A_1\mathcal A_2}{\theta a_{\min}}\right]
e^{-c_\lambda\operatorname{dist}(x,y)/(h_kR_k)}.
\tag{MR25}
\]

Concretely one can take \(a(X)=a_0\) times its number of blocks, with fixed \(a_0>0\). The norms in (MR24) are \(\sum_X|J_i(X)|e^{\lambda\ell(X)+a(X)}\), and similarly for the mixed root; root-to-support connecting lengths are included in \(\ell\). Their decay exponents use fixed slack inside the source activity decay. Two coincident roots are treated as two labels in the same component, with total dimension eight. A single label is assigned to its unique component; components are disjoint, and boundary-straddling seeds are outside the restricted theorem until they have an anchored decomposition.

This formula makes the normalization exact: \([t_1t_2]\log\Xi\) is the normalized connected coefficient. Disconnected vacuum components cancel algebraically in the logarithm; the rooted bounds are uniform in total volume. There is no step of the form \(e^{C|\Lambda|}/Z\le C\).

Combining (MR24)–(MR25) yields the conditional component-gas bound

\[
\boxed{
\left|[t_1t_2]\log\Xi(t)\right|
\le C A_1A_2h_k^{-8}(\eta_k+\eta_k^2)
e^{-c\operatorname{dist}(x,y)/(h_kR_k)}.
}
\tag{MR26}
\]

The two terms have different geometric origins:

* **Same reset component.** The mixed activity \(J_{12}\) itself contains both roots and carries its component tree decay. A small completed-reset component has diameter at most \(C h_kR_k\), so the displayed distance factor costs at most a fixed constant there. For a larger connected localization domain, its ordinary tree-size bound supplies the connection.
* **Different reset components.** The connected cluster joining the two root activities carries a chain between their supports. Disconnected root components cancel in \(\log\Xi\). This is the source of the distance factor multiplying \(\mathcal A_1\mathcal A_2\).

The remaining large-field regions \(Y_i\) require separate treatment. Source (1.97) gives \(\alpha^{1/3}\), rather than \(e^{-p_0}\), for terms intersecting them, and (1.99) uses the corresponding collapsed geometry. Those terms are assigned to boundary terms in (1.100)–(1.104). They stay in the unresolved-component bookkeeping until it is legitimate to discharge them. They cannot be counted as ordinary physical-distance regular R activities prematurely.

Finally, (MR26) is a statement at fixed admitted outer/background data for the component gas in (1.72), or for the corresponding localized source coefficient. Averaging over outer fields adds the covariance of the conditional means. Controlling that additional term requires the regular marked induction. Thus (MR26) is a normalized actual old-core result, not the full-law S2 estimate.

### 7. The R losses are summable once their marked interface is available

Under the admitted asymptotically free trajectory, suppose

\[
g_k^{-2}\ge x_*+c_*(K-k),
\qquad
p_0(g)\ge c_0(\log g^{-2})^P,
\qquad P>1.
\tag{MR27}
\]

For any fixed logarithmic or polynomial prefactor, losses of the form

\[
\eta_k\le C(1+g_k^{-2})^q
\exp\{-c(\log g_k^{-2})^P\}
\tag{MR28}
\]

satisfy

\[
\sup_K\sum_{k=0}^K\eta_k<\infty,
\qquad
\sup_K\sum_{k=0}^K\eta_k\longrightarrow0
\quad\text{as }x_*\longrightarrow\infty.
\tag{MR29}
\]

Indeed, for every fixed \(s>q+1\), \(c(\log x)^P\ge s\log x\) for sufficiently large \(x\), and the tail is bounded by a convergent power series. This is an elementary consequence of the assumed trajectory, not an independent proof of that trajectory.

If a regular marked construction supplies dimensionless incoming seed norms \(B_{i,k},B_{12,k}\), the proved core module gives the sufficient R interface

\[
\delta_R B_{i,k}\le C\eta_k B_{i,k},
\qquad
\delta_R B_{12,k}\le C\eta_k
\bigl(B_{12,k}+B_{1,k}B_{2,k}\bigr).
\tag{MR30}
\]

Equation (MR30) is conditional on the local seed decomposition specified in §§5–6. It is not asserted for an arbitrary incoming function solely from its global \(L^2\) norm. Once it applies, its multiplicative loss is bounded by \(\exp(C\sum_k\eta_k)\), uniformly in depth. Regular marginal mixing, which can have a nonsummable \(O(g_k^2)\) part before renormalization, remains a separate issue.

### 8. Accomplished and remaining

**Completed finite-degree statements:**

1. Posterior-weighted Jensen and second-moment estimates for the actual old R numerator, including variable reset geometries. No pointwise smallness of an individual ratio is required.
2. Stability of the actual LFR II lifetime/merger/failed-reset budget under any fixed engineering-age charge, in particular \(D_*=8\), with a scale-independent small-coupling threshold stated in source constants.
3. Physical-scale bounds for genuinely old bounded gauge-invariant core insertions while their support remains inside unresolved integration variables; the source analytic component bound extends them to the same background domain when the seed is background-independent.
4. A normalized connected component-gas estimate for those restricted insertions, using the source localization and the companion rooted KP theorem. The normalization removes vacuum volume factors exactly.
5. Summability of the resulting finite-degree R losses under the admitted trajectory.

**Still needed for full S2:**

* Construct and propagate a localized regular norm for the actual old insertion after it leaves a core, including its scalar running normalization, identity subtraction and finite source coefficients.
* Prove the matching of that regular insertion to a controlled local operator plus remainder, instead of identifying it with a fresh minimizer.
* Compose the resulting norm with the actual regular conditional covariance bound and keep the boundary/remaining-large-field bookkeeping on the same normalized history law.
* Bound the outer-field covariance of generated conditional means and the final terminal covariance.

The fixed two-mark argument also does not prove the uniform all-order factorial budget, tensor mixing, Euclidean restoration, nontriviality or the other construction gates. Its contribution is to remove a specific artificial obstruction: a rare carrier's old numerator ratio need not be bounded by itself, and its entire unresolved age is already represented in a source budget that can pay a fixed insertion dimension.

### 9. Further development: control of posterior means from concentration and analytic roots

The preceding component estimate can be extended in two complementary ways. The first is an exact probability theorem requiring only a sub-Gaussian marginal. The second supplies a spatial bound when the generated old conditional mean is an analytic local function of a regular outer field. Both sum or average carriers before estimating; neither needs a pointwise lower bound on an individual carrier probability.

#### 9.1 Posterior–Herbst rarity theorem

Let \((\omega,\Gamma,V)\) have any positive joint probability law, with old marginal \(\mu(d\omega)\). Set

\[
c_F=\mu F,\qquad
\mathbb E_\mu e^{t(F-c_F)}\le e^{\sigma_F^2t^2/2}
\quad(t\in\mathbb R).
\tag{MR31}
\]

Write \(\mathcal G=\sigma(\Gamma,V)\), \(f=\mathbb E[F\mid\mathcal G]\), and let \(B\in\mathcal G\) be an arbitrary carrier event of probability \(p\). It may contain arbitrarily many histories or varying reset geometries. Then

\[
\boxed{
\mathbb E[1_B|f-c_F|^2]
\le 2\sigma_F^2p\left(1+\log\frac2p\right).
}
\tag{MR32}
\]

For \(p=0\), interpret the right side as zero. If \(G\) satisfies the analogous sub-Gaussian bound, then

\[
\mathbb E[1_B|f-c_F||g-c_G|]
\le2\sigma_F\sigma_Gp\left(1+\log\frac2p\right),
\tag{MR33}
\]

\[
\mathbb E\!\left[1_B\left|\operatorname{Cov}(F,G\mid\mathcal G)\right|\right]
\le2\sigma_F\sigma_Gp\left(1+\log\frac2p\right).
\tag{MR34}
\]

**Proof.** Conditional Jensen gives
\(\mathbb E1_B|f-c_F|^2\le\mathbb E1_B|F-c_F|^2\).
The sub-Gaussian tail satisfies
\(\mathbb P(|F-c_F|^2>u)\le2e^{-u/(2\sigma_F^2)}\). Therefore

\[
\begin{aligned}
\mathbb E1_B|F-c_F|^2
&\le\int_0^\infty\min\{p,2e^{-u/(2\sigma_F^2)}\}\,du\\
&=2\sigma_F^2p\left(\log\frac2p+1\right).
\end{aligned}
\tag{MR35}
\]

The last equality splits the integral at \(2\sigma_F^2\log(2/p)\). Cauchy–Schwarz proves (MR33). For (MR34), bound each conditional variance by its conditional second moment about the common constant and apply Cauchy–Schwarz again. \(\square\)

This proof depends on the total rare probability \(p\), not on the Shannon entropy of the individual history labels. In particular, one does not lose a factor counting the number of tiny carriers.

There is also a version for the history-mean covariance (MR7). At each \(V\), take two conditionally independent carrier labels \(\Gamma_1,\Gamma_2\), and retain the terms for which at least one label belongs to \(B\). Denote the resulting half-pair covariance by \(H_B(V)\). Then

\[
\boxed{
\mathbb E|H_B(V)|
\le8\sigma_F\sigma_Gp\left(1+\log\frac2p\right).
}
\tag{MR36}
\]

To prove it, conditional Jensen first shows that each copy of the posterior mean has the sub-Gaussian parameter \(\sigma_F\). Cauchy–Schwarz in the moment generating function shows that their difference has parameter \(2\sigma_F\), even though the two copies are not independent without conditioning on \(V\). The pair event has probability \(q\le\min(1,2p)\). Applying (MR35) to both differences and then Cauchy–Schwarz yields
\(4\sigma_F\sigma_Gq(1+\log(2/q))\), which is at most the right side of (MR36).

On a regular hard-cutoff carrier satisfying the companion log-Sobolev inequality

\[
\operatorname{Ent}_\mu(u^2)\le\frac2{m_0}\mu|\nabla u|^2,
\]

Herbst's argument gives (MR31) with

\[
\sigma_F^2\le\frac{\sup|\nabla F|^2}{m_0}.
\tag{MR37}
\]

Thus a *compatible* bound \(p\le C\eta_k\) and a physical Lipschitz scale for the actual mark give rare-carrier losses of order
\(\sigma_F\sigma_G(1+p_0(g_k))e^{-c p_0(g_k)}\), with the full rare exponential up to a logarithm. These losses are summable by §7.

There are two essential qualifications. First, the probability bound and the sub-Gaussian estimate must hold under the **same normalized joint law**. A concentration estimate for a fresh minimizing-field observable under a regular reference measure cannot be substituted for (MR31) for an arbitrary old insertion in the full history law. Second, a mean \(c_F\) computed after conditioning on an outer sector is constant only within that conditional problem. Its variation between sectors must be retained as an additional covariance; it is not an allowed global history-dependent subtraction.

The theorem is therefore a new tool for controlling genuine component-dependent means when the regular marked norm is available. By itself it gives no separation factor in \(|x-y|\).

#### 9.2 A spatial outer-mean theorem for generated old-core roots

There is a more direct route for the core contributions already estimated here. Define the **summed** conditional mean

\[
M_x(A)=[t_x]\log\Xi(t,A).
\tag{MR38}
\]

It is the mean of the actual selected old mark at the component-gas conditioning level, as explained in §6. It is not a fresh minimizing-field insertion. The root cluster expansion gives it as a sum of analytic localized coefficients, so one can differentiate this sum instead of the individual ratios \(N_\gamma^F/N_\gamma\).

Here is a precise sufficient theorem. Let the remaining independent regular coordinates be \(A=(A_b)\), with real domain a product of convex balls, and normalized law \(\mu(dA)\propto1_D e^{-V(A)}dA\). Assume the weighted hard-cutoff covariance theorem holds with gap \(m_s>0\) for weights

\[
W_x(b)=e^{s\,d(x,b)},
\qquad d(x,y)=\frac{|x-y|}{h_kR_k}.
\tag{MR39}
\]

Suppose

\[
M_x(A)=\sum_{X\ni x}m_x(X,A),
\tag{MR40}
\]

with each coefficient depending only on the coordinates in its support (or with the equivalent exponentially localized expansion after composing the coordinate map). Suppose each coefficient is holomorphic on a coordinatewise complex tube of radius \(\delta_k\) around the real domain. If \(n(X)\) is the number of scalar coordinates in its support and \(\ell_x(X)\ge\max_{b\in X}d(x,b)\), assume

\[
\sum_{X\ni x}n(X)^{1/2}e^{s\ell_x(X)}
 \sup_{D_{\delta_k}}|m_x(X,A)|\le B_{x,k}.
\tag{MR41}
\]

Then

\[
\|W_x\nabla M_x\|_{L^2(\mu;\ell^2)}
\le\delta_k^{-1}B_{x,k},
\tag{MR42}
\]

and

\[
\boxed{
|\operatorname{Cov}_\mu(M_x,M_y)|
\le\frac{B_{x,k}B_{y,k}}{m_s\delta_k^2}
e^{-s d(x,y)}.
}
\tag{MR43}
\]

**Proof.** Cauchy's formula bounds each scalar derivative of \(m_x(X)\) by \(\delta_k^{-1}\sup|m_x(X)|\). The weighted Euclidean norm of its gradient is at most \(\delta_k^{-1}n(X)^{1/2}e^{s\ell_x(X)}\sup|m_x(X)|\). Sum these norms to obtain (MR42). The metric triangle inequality implies
\(W_x^{-1}(b)\le e^{-s d(x,y)}W_y(b)\). Apply the weighted covariance bound with \(W_x\) to obtain (MR43). \(\square\)

The factor \(n(X)^{1/2}\) in (MR41) can be paid from fixed slack in the exponential support/KP weights, with explicit finite block-size factors if the coordinates are finer than the polymer blocks. Thus a pulled-back analytic root estimate corresponding to (MR24) gives

\[
B_{x,k}\le C A_x h_k^{-4}\eta_k
\]

and hence

\[
|\operatorname{Cov}_\mu(M_x,M_y)|
\le C A_xA_yh_k^{-8}
\frac{\eta_k^2}{m_s\delta_k^2}
e^{-s|x-y|/(h_kR_k)}.
\tag{MR44}
\]

The log-Sobolev inequality additionally gives

\[
\|M_x-\mu M_x\|_p
\le C\sqrt{\frac p{m_0}}\,\delta_k^{-1}B_{x,k}
\quad(p\ge2),
\tag{MR45}
\]

which can be combined with (MR32)–(MR36) for further compatible carrier selections. These are ordinary conditional covariance and moment statements for the old-core means after summing histories; no ratio lower bound or per-history recentering is used.

#### 9.3 Exact source interface still to verify for (MR44)

The source verifies analyticity of \(\mathcal T'_k\), its activities and the rooted sums in its admitted **background** variables. The companion regular-coordinate analysis verifies an analytic chart

\[
B'(A)=g_k C A-\mathfrak h D(g_k C A),
\]

with exponentially localized derivative of size \(O(g_k)\) on its inner regular domain. If the background R coefficient has a uniform margin \(\delta_{R,k}\) in the corresponding source regularity norm, a sufficient pulled-back radius is

\[
\delta_k\le c\,\frac{\min(\delta_{R,k},\delta_0)}{g_k}.
\tag{MR46}
\]

Equivalently, one can combine Cauchy derivatives in the background variables with the weighted Jacobian bound for this chart. Either route must preserve the root-to-support decay.

The exact remaining check is therefore concrete: exhibit a uniform inner-domain margin \(\delta_{R,k}\) for the **marked R coefficients** on the real outer regular carrier, and show that their pullback has the weighted localization needed in (MR41). The source's shrinking background domains must be used as stated. If this margin loses only fixed powers of \(g_k\) and logarithms, its inverse is absorbed by the super-logarithmic \(\eta_k^2\) loss, so (MR44) remains summable.

There is a source-based way to verify that margin on a current regular domain. CMP119 p.259, (2.28), gives
\(\alpha_{i,k}=g_k C_i(\log g_k^{-2})^{q_i}\), \(i=0,1\), and its R activities inherit those analytic spaces. CMP109 pp.262–263, (1.11)–(1.16), defines the background domain and proves an inner-domain inclusion: smaller regularity constants in its first three conditions imply the fourth, hierarchical condition, using a fixed factor \(2B_3\). Consequently it suffices to verify the actual real field and its chart perturbation with a fixed reserve below those constants. Algebraically, if the actual regular size is \(g_kA_0(\log g_k^{-2})^{p_0}\), taking admitted parameters with \(q_i\ge p_0\) and sufficiently large \(C_i/A_0\) would provide such a reserve. Compatibility of that parameter choice with all source restrictions, and the exact running hard-cutoff radius, have not been certified here. This is a verifiable criterion for (MR46), not a replacement for that check. CMP109, pp.262–263.

There is a second, separate law requirement: \(\mu\) in (MR43) must be the actual normalized outer regular law, including its interactions and hard cutoff, with the stated weighted Hessian gap. The companion HC theorem supplies the implication from that gap; it must not be applied to a signed polymer gas as if the gas were a probability measure. If some outer variables still describe unresolved large-field components or discrete geometries, condition on them, use (MR43) on the regular factor, and retain the covariance between those conditional means. A complete proof must discharge that remaining covariance through the boundary/regular marked induction. Equations (MR31)–(MR46) identify sufficient quantitative estimates for doing so, without demanding pointwise small carrier ratios.

### 10. Conditional composition with a common bulk marginal normalization

The large-field estimates can be composed with an almost marginal bulk recursion without introducing a normalization that depends on the history. The following theorem makes the exact additional one-step hypothesis explicit.

#### 10.1 Weighted super-logarithmic tails

Let \(x_j\) denote the inverse-coupling scale, with fine-to-coarse index increasing in \(j\). Assume

\[
x_j\ge x_*,\qquad
c_-\le x_j-x_{j+1}\le c_+,
\tag{MR47}
\]

for fixed positive \(c_-,c_+\). The corresponding bounded-comparability variant gives the same conclusions if it also controls the number of indices per interval in \(x\). Write

\[
\eta(x)=C_\eta x^q(1+\log x)^r
e^{-c(\log x)^P},
\quad P>1,\quad q,r\ge0.
\tag{MR48}
\]

Any fixed polynomial loss from running normalizations, analytic radii or finite block factors may be included in \(q,r\). For fixed \(p\ge0\), once \(x_*\) is sufficiently large depending on \(p,q,r,c,P\),

\[
\boxed{
\sum_{j\le k}\eta(x_j)\left(\frac{x_j}{x_k}\right)^p
\le \Theta_p(x_k),
}
\tag{MR49}
\]

where one may take

\[
\Theta_p(x)=C\eta(x)
\left(1+\frac{x}{(\log x)^{P-1}}\right).
\tag{MR50}
\]

Here the threshold and the fixed constant depend on \(p\), but not on the total number of scales. In particular \(\Theta_p(x)\to0\) faster than any fixed inverse power of \(x\).

**Proof.** The function \(f(t)=t^p\eta(t)\) is decreasing above a fixed threshold. The lower spacing bound in (MR47) gives

\[
\sum_{j\le k}f(x_j)
\le f(x_k)+c_-^{-1}\int_{x_k}^{\infty}f(t)\,dt.
\]

Set \(u=\log t\). The integral has exponent
\(-\Phi(u)\), where
\(\Phi(u)=cu^P-(p+q+1)u-r\log(1+u)\).
For example, it is enough to require

\[
\log x_*\ge
\max\left\{1,
\left[\frac{2(p+q+1+r)}{cP}\right]^{1/(P-1)}\right\}.
\]

Then \(\Phi'(u)\ge(cP/2)u^{P-1}>0\), and \(\Phi''(u)>0\). Convexity bounds the tail integral by
\(e^{-\Phi(\log x_k)}/\Phi'(\log x_k)\).
Divide by \(x_k^p\) to obtain (MR49)–(MR50). \(\square\)

The direction of the weight matters. For \(j\ge k\),

\[
\sum_{j=k}^K\eta(x_j)\left(\frac{x_j}{x_k}\right)^p
\le\Theta_0(x_K),
\tag{MR51}
\]

whereas the inverse-weighted version satisfies

\[
\sum_{j=k}^K\eta(x_j)\left(\frac{x_k}{x_j}\right)^p
\le\left(\frac{x_k}{x_K}\right)^p\Theta_0(x_K).
\tag{MR52}
\]

The permitted bulk factor in (MR52) cannot be discarded. The single final term is already \(\eta(x_K)(x_k/x_K)^p\), which need not be uniformly bounded as the UV depth increases. Equation (MR52) is uniform **relative to that bulk growth**, exactly the weight handled by a common normalization fixed at the physical matching scale.

For a strictly contracting block, one also has

\[
\sum_{j<k}\vartheta^{k-1-j}
\left(\frac{x_j}{x_k}\right)^p\eta(x_j)
\le C_{p,\vartheta}\eta(x_k),
\qquad 0<\vartheta<1.
\tag{MR53}
\]

Indeed, \(\eta(x_j)\le\eta(x_k)\) above the monotonicity threshold and
\(x_j/x_k\le1+c_+(k-j)/x_*\); the remaining geometrically weighted polynomial series converges. This is sharper than the merely summable marginal estimate.

#### 10.2 Forced marked-block theorem

At scale \(j\), let \(\mathcal B_j\) be a Banach space of anchored marked coefficients. Its norm is **dimensionless in physical units**: for \(m\) dimension-four marks the factor \(h_j^{4m}\) has already been included. Assume its support weights preserve a fixed positive tree-decay rate. Choose a single deterministic bulk normalization \(N_j\), fixed by the bulk cocycle and the physical matching scale \(\ell_0\); it is the same on every carrier.

The hypotheses are:

1. **Bulk block theorem.** The actual normalized regular operation, with its insertion counterterms and common subtraction included, has a propagator \(U_{k,j}:\mathcal B_j\to\mathcal B_k\) satisfying
   \[
   \|U_{k,j}\|\le C_B\left(\frac{x_j}{x_k}\right)^p,
   \qquad j\le k,
   \tag{MR54}
   \]
   and the prescribed irrelevant block has the additional factor \(\vartheta^{k-j}\). This is an assumption about the **actual old marked operation**, not about the unmarked density or a fresh minimizer.
2. **Compatible normalized R/boundary forcing.** After summing histories and performing anchored normalization, the discharged R and boundary roots give remainders \(r_j\) satisfying
   \[
   \|r_j\|_{\mathcal B_{j+1}}
   \le\eta(x_j)\bigl(\|v_j\|_{\mathcal B_j}+d_j\bigr).
   \tag{MR55}
   \]
   This bound uses the same \(N_j\), the same physical units and the same normalized law as (MR54). A still-unprocessed boundary term with only the source's collapsed metric does not satisfy this hypothesis merely because it has an unmarked small factor.
3. **Exact recurrence.** The marked coefficients satisfy
   \[
   v_{j+1}=U_{j+1,j}v_j+r_j,
   \tag{MR56}
   \]
   or the corresponding inhomogeneous version. All carrier-dependent scalar remnants are retained in \(r_j\) or in a separately controlled boundary block; they have not been removed by changing the subtraction on individual histories.

Then Duhamel's formula and discrete Gronwall give

\[
\boxed{
\|v_k\|
\le C_B e^{C_B\sum_{j<k}\eta(x_j)}
\left[
\left(\frac{x_0}{x_k}\right)^p\|v_0\|
+\sum_{j<k}\left(\frac{x_j}{x_k}\right)^p\eta(x_j)d_j
\right].
}
\tag{MR57}
\]

**Proof.** In the exact Duhamel formula the propagator after a forcing at step \(j\) is \(U_{k,j+1}\). Since \(x_{j+1}\le x_j\), (MR54) is bounded by the displayed weight. Multiply the norm inequality by \(x_k^p\); the propagator weights telescope to \(x_j^p\). Discrete Gronwall then bounds the feedback factors by
\(\prod_j(1+C_B\eta(x_j))\le e^{C_B\sum_j\eta(x_j)}\), proving (MR57). \(\square\)

A particularly useful formulation compares the result with the already chosen bulk solution. Let \(v_k^{\rm bulk}\) use the same initial data and normalization, and suppose

\[
\|v_k^{\rm bulk}\|+d_k
\le A\left(\frac{x_k}{x_K}\right)^s
\tag{MR58}
\]

for a fixed finite \(s\ge0\). Suppose the R remainder satisfies the corresponding feedback inequality in \(v_k^{\rm bulk}+e_k\), where \(e_k=v_k-v_k^{\rm bulk}\). Then

\[
\boxed{
\|e_k\|
\le C A\left(\frac{x_k}{x_K}\right)^s
e^{C\Theta_0(x_K)}\Theta_{p+s}(x_k).
}
\tag{MR59}
\]

To see this, apply the same Gronwall argument to the zero-initial-data error. In each source term,

\[
\left(\frac{x_j}{x_k}\right)^p
\eta(x_j)\left(\frac{x_j}{x_K}\right)^s
=\left(\frac{x_k}{x_K}\right)^s
\eta(x_j)\left(\frac{x_j}{x_k}\right)^{p+s}.
\]

Equation (MR49) gives (MR59), while (MR51) bounds the accumulated feedback. Thus the R correction is uniformly small relative to the permitted bulk polynomial growth, and it is super-logarithmically smaller toward the UV. No replacement of the deterministic bulk cocycle by a carrier-dependent normalization is involved.

For two marks, first apply the theorem to the one-root coefficients. The mixed remainder has the natural form

\[
\|r_j^{12}\|\le C\eta(x_j)
\bigl(\|v_j^{12}\|+\|v_j^1\|\,\|v_j^2\|\bigr).
\tag{MR60}
\]

The already bounded product of one-root norms is a forcing of the form (MR58), with exponent \(s_1+s_2\). Applying (MR59) again controls the mixed coefficient. Its norm includes the connected support weight, so the propagation preserves the spatial decay provided by the one-step marked-block theorem. This is a finite-degree composition statement; it does not assert uniform control as the number of marks tends to infinity.

#### 10.3 What this composition does, and what it does not assume away

The theorem connects the current-scale old-core estimate (MR19)/(MR24) to later regular propagation: once a discharged root has an actual \(h_j^{-4}\) or \(h_j^{-8}\) normalized anchored norm, its super-logarithmic source factor survives any fixed polynomial almost-marginal bulk amplification. Repeated R events give a uniformly finite feedback factor. The original microscopic-to-entry scale deficit identified after (MR17) is not hidden in this argument; it must be absent because the incoming marked-block norm has genuinely been proved.

There is supporting source structure for the required linearized operation. CMP119 p.262 states that RT maps the whole admissible density class at scale \(k\) into the class at \(k+1\). Its (3.26) represents the R contribution through a normalized expectation, and p.276 treats R terms by the same analytic localization as E terms, without the coupling-counterterm extraction. Moreover, the proof of (2.44), printed p.283, explicitly bounds each vacuum-subtracted regular R activity by a factor proportional to \((L^jL^{-n})^4\) on a smoother scale-\(n\) background before summing its possible locations. This identifies the engineering gain that an anchored proof must retain.

Those source statements do not automatically establish (MR54)–(MR55). In particular, an unanchored volume estimate may sum over \(L^4\) fine positions and lose the fixed-root gain; a source-free action stability theorem does not by itself transport the marked old numerator. The remaining constructive step is to prove the finite marked block map with the root held fixed, the exact normalized numerator retained, and boundary scalar terms carried explicitly. Once that step is done, (MR49)–(MR60) show that the R tail is a controlled perturbation of the common bulk cocycle.

### 11. Potential failure modes

The source comparison and the KP proof of Part II.A are checked against the following potential failure modes:

| Potential failure | Outcome and required restriction |
|---|---|
| Microscopic insertion scale confused with a later component birth | Treated explicitly after MR17. Only occupied ancestry steps are paid. Earlier regular evolution must provide the incoming physical-scale norm. |
| Both seeds merge into one component | The global label count is fixed. Their dimensions add to at most eight; charging every active component by eight overestimates rather than underestimates the required cost. A repeated physical location still has two labels. |
| A one-block region has \(d'=0\) | Source active components are thickened and have \(d'\ge1\). Thin newborn sets use the source \(d'+1\) birth penalty. No age charge is assigned to a nonexistent active component. |
| Missed or duplicated occupancy steps | Transition \(j-1\to j\) is charged to the active component at \(j\). The source overhead in (1.79) runs through these steps. A mark outside active ancestry violates the theorem's assumption; it is not charged retroactively. |
| A tiny analytic reset denominator | Source (1.75) controls the normalized analytic operation, while the physical-scale estimate retains its unnormalized marked activity. KP/logarithmic normalization cancels disconnected vacuum factors. |
| Root/carrier domain does not contain the mark | The restricted theorem requires the full old loop support in the component's retained variables. Cover-and-thicken ancestry preserves containment; boundary-straddling marks need a separate anchored decomposition. |
| Two roots coincide or lie in one activity | The mixed coefficient \(J_{12}\) is retained. It is not replaced by a product of one-root coefficients. Part II.A verifies MR24–MR26 with explicit \(a_{\min}\) and root-connection lengths. |
| Component-gas normalization mistaken for full output conditioning | Addressed in §6: outer operations may act on \(\Xi\). The conditional covariance of their means is a real additional term; §9 provides a sufficient spatial theorem for its regular continuous part. |
| Source-free analyticity silently supplies regular marked transport | It does not. It supplies fixed old-core coefficients; the later regular marked induction and the pulled-back analytic margin in (MR46) must still be established. |

### Sources

* **LFR I:** Balaban, Large Field Renormalization I, CMP122 (1989), 175–202, p.177 for component thickness and reset eligibility; pp.192–194 and 201 for exact old-field integration, normalized replacement and integral preservation.
* **LFR II:** Balaban, Large Field Renormalization II, CMP122 (1989), 355–392, pp.377–380, (1.70)–(1.75), for localized matched component operations and analytic positivity bounds; pp.383–387, (1.79)–(1.89), for the history budget; pp.388–391, (1.90)–(1.104), for polymer normalization and the distinction between regular R and remaining-boundary terms.
* **CMP119:** Balaban, Convergent Renormalization Expansions for Lattice Gauge Theories, CMP119 (1988), 243–285, p.255, (2.3)–(2.7), for large-field and scale conventions, and Corollary 3/(2.50) for the general large-field operation bound to which LFR II refers.
* **CMP109:** Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories I*, CMP **109** (1987), pp.262–263, (1.11)–(1.16). Used only for the background-domain inner inclusion identified in §9.3. The current CMP119 radii are those of CMP119, p.259.
* **Microscopic seed:** the exact Wilson/clover insertion and its deterministic bounds, as constructed in [Minimizing-field response and the two-insertion cluster formula](two_insertion_clusters.md).
* **Marked-cluster estimate:** **Part II.A**, for the rooted KP proof and the precise norm and slack hypotheses used in (MR25), including the embedding used in MR24–MR26, with root-to-support lengths and \(a(X)\ge a_{\min}>0\) explicit.
* **Companion cutoff/covariance note:** **Part I**, for the weighted covariance and log-Sobolev theorems on the actual convex hard-cutoff regular domain, and the nonlinear regular-coordinate chart. Equations (MR43)–(MR46) keep its actual-law and analytic-margin assumptions explicit.

---

## Part VI.A. Frozen-cutoff source jets and classical curvature projection

### Purpose and scope

This note derives a uniform \(O(g^2)\) correction for the **finite marginal jets** of the actual normalized regular source map, under localized analytic input and the full-torus regular-action estimates described below. The argument keeps the actual cutoff fixed during an auxiliary fluctuation-amplitude interpolation. It avoids a derivative of the family of physical coupling-dependent kernels.

The main new point is that strong spatial covariance plus local moments controls the two extensive score insertions appearing in the second derivative. No global partition-function estimate and no independently assumed three-root cluster norm are needed. The result is a real finite-jet estimate. It does not by itself prove stability or contraction of the entire complex analytic remainder norm through every RG step.

### 1. Finite cumulants from the weighted covariance theorem

Let \(\mu\) be a measure on a symmetric product convex cutoff domain. Assume the weighted covariance estimate HC-W, uniformly for block-scalar weights whose logarithms have Lipschitz constant at most \(\alpha\). Suppose local observables and their coordinate gradients have the finite moments used below.

For a local observable \(F_i\), let \(X_i\) contain its coordinate support. Put

\[
 L_i(p)=\|F_i\|_{L^p(\mu)}
       +\|\nabla F_i\|_{L^p(\mu;\ell^2)}.
 \tag{J1}
\]

#### Lemma J-C

For each fixed \(n\ge2\), there is a constant \(C_n\) such that

\[
 |\kappa_n(F_1,\ldots,F_n)|
 \le C_n\prod_iL_i(2n)
       e^{-\alpha d(U_A,U_B)}
 \tag{J2}
\]

for every nontrivial partition \(A\cup B=\{1,\ldots,n\}\), where
\(U_A=\bigcup_{i\in A}X_i\) and \(U_B=\bigcup_{i\in B}X_i\). The constant can depend on the uniform coercivity gap and \(n\), but not on the cutoff radii, volume, or separation.

**Proof.** Let \(\nu\) be the product of the \(\mu\)-marginal joint laws of the groups \(A\) and \(B\). Its mixed cumulant of all \(n\) observables is zero. For any subset \(S\),

\[
 \mu\prod_{i\in S}F_i-\nu\prod_{i\in S}F_i
 =\operatorname{Cov}_\mu
   \left(\prod_{i\in S\cap A}F_i,
         \prod_{i\in S\cap B}F_i\right).
 \tag{J3}
\]

This difference is zero if either product is empty. Otherwise choose
\(W_b=e^{\alpha d(b,U_A)}\) in HC-W. The gradient of the first product is supported in \(U_A\), where \(W=1\); the inverse weight on the second support is at most \(e^{-\alpha d(U_A,U_B)}\). The product rule and Hölder's inequality bound the covariance by a fixed multiple of
\(e^{-\alpha d(U_A,U_B)}\prod_{i\in S}L_i(2n)\).

Expand the cumulant by its finite moment-partition formula. Replace each moment under \(\mu\) by the corresponding moment under \(\nu\), using a telescoping difference for products of moments. All unchanged moments are bounded by Hölder. The cumulant under \(\nu\) is zero, so (J2) follows. \(\square\)

If the supports have representative points \(z_i\), take a minimum spanning tree on the points and remove one of its longest edges. Every edge crossing the resulting partition has length at least that removed edge; otherwise the original tree was not minimal. That edge is at least
\(\operatorname{diam}\{z_i\}/(n-1)\). Consequently (J2) implies

\[
 |\kappa_n(F_1,\ldots,F_n)|
 \le C_n\prod_iL_i(2n)
 \exp\left[-\frac{\alpha}{n-1}
       \operatorname{diam}\{z_i\}
       +2\alpha\sum_i\operatorname{diam}X_i\right].
 \tag{J4}
\]

The support-size factors can be paid by the available activity localization. For fixed \(n\), the remaining exponential is summable over the \(n-1\) unfixed root positions on a lattice of polynomial volume growth.

For \(n=3\), one can see the mechanism directly from

\[
 \kappa_3(F,G,H)
 =\operatorname{Cov}(F,(G-\mu G)(H-\mu H))
 \tag{J5}
\]

and its other two versions. One of the three points is at distance at least half the total diameter from the other two. This supplies exponential decay in the complete three-point diameter and makes both score-location sums finite.

The lemma concerns each fixed cumulant order. It is not the uniform all-order factorial estimate required by the later all-order construction gates.

### 2. The actual auxiliary amplitude interpolation

Fix an admitted real background \(U\), the old couplings entering its effective action, and the actual independent-coordinate cutoff
\(D=D_{r(g)}\). Keep all of these fixed while varying a real parameter \(\tau\in[-g,g]\). In independent fluctuation coordinates define

\[
 \mu_\tau(dA)=Z_\tau^{-1}{\bf1}_D(A)e^{-H_\tau(U,A)}\,dA,
 \qquad
 \mathcal T_\tau f(U)=\mu_\tau F_\tau,
 \tag{J6}
\]

where

\[
 F_\tau(U,A)=f(\mathcal U(U,\tau A)).
 \tag{J7}
\]

The regular action is interpolated consistently with the source's expansion:

\[
 H_\tau
 =\tfrac12\langle A,M(U)A\rangle
  +\tau^{-2}W(U,\tau A)
  +E_{\rm old}(\mathcal U(U,\tau A))
       -E_{\rm old}(\mathcal U(U,0))
  +J(U,\tau A).
 \tag{J8}
\]

Signs of the last terms can be incorporated in \(W,E,J\). The classical remainder \(W\) vanishes to order three, so \(\tau^{-2}W(U,\tau A)\) extends smoothly to \(\tau=0\), with value zero. The analytic Jacobian term is normalized so \(J(U,0)=0\). Thus \(\mu_0\) is a centered Gaussian restricted to the symmetric product domain \(D\).

It is essential that the classical interpolation uses \(\tau^{-2}W(U,\tau A)\). Keeping a fixed factor \(g^{-2}\) while replacing only its argument by \(\tau A\) defines a different path and introduces unnecessary inverse-coupling derivative losses.

All old couplings are frozen. The value at \(\tau=g\) is the actual regular source map at this step. The auxiliary family is used only to compare that map with its classical value at \(\tau=0\).

### 3. Exact first- and second-derivative identities

The first derivative is

\[
 \frac{d}{d\tau}\mu_\tau F_\tau
 =\mu_\tau F'_\tau
  -\operatorname{Cov}_{\mu_\tau}(F_\tau,H'_\tau).
 \tag{J9}
\]

At zero amplitude, \(F_0=f(\mathcal U(U,0))\) is constant in \(A\). Also \(F'_0\) is linear in \(A\), since the derivative of the minimizing-field map at zero is the linear response. Hence

\[
 \left.\frac{d}{d\tau}\mathcal T_\tau f(U)\right|_{\tau=0}=0.
 \tag{J10}
\]

The covariance in (J9) vanishes because its first argument is constant. The remaining Gaussian expectation vanishes by parity. The cutoff need not be removed for either cancellation.

Differentiating (J9) once more gives the exact identity

\[
 \boxed{
 \frac{d^2}{d\tau^2}\mu_\tau F_\tau
 =\mu_\tau F''_\tau
  -2\operatorname{Cov}_{\mu_\tau}(F'_\tau,H'_\tau)
  -\operatorname{Cov}_{\mu_\tau}(F_\tau,H''_\tau)
  +\kappa_{3,\mu_\tau}(F_\tau,H'_\tau,H'_\tau).
 }
 \tag{J11}
\]

This formula includes all normalization and score terms. No frozen-kernel score is omitted.

### 4. A uniform local bound for the second derivative

Assume uniformly in \(|\tau|\le g\):

1. The laws \(\mu_\tau\) satisfy HC-W and the raw local moment estimates
   \(\|A_b\|_{L^p}\le C\sqrt p\), for the finitely many orders required below.
2. The input source has an anchored localized analytic decomposition. After composition with \(\mathcal U(U,\tau A)\), its zeroth, first, and second amplitude derivatives and their coordinate gradients have local polynomial bounds with exponentially summable support weights, of total size \(\mathcal N_f\).
3. The scores have localized decompositions
   \(H'_\tau=\sum_Y S_{\tau,Y}\),
   \(H''_\tau=\sum_Y T_{\tau,Y}\). Their local polynomial bounds and coordinate-gradient bounds have a uniformly summable norm per bond.

The summability in conditions 2–3 is **exponentially weighted summability with reserve**, not unweighted summability. More explicitly, after converting polynomial bounds to the moment norms (J1), require for a fixed \(\kappa>2\alpha\)

\[
 \sup_b\sum_{Y\ni b}e^{\kappa d(Y)}
 \left[L_{S_{\tau,Y}}(p_*)+L_{T_{\tau,Y}}(p_*)\right]\le C_H,
 \quad
 \sum_{X\ni x}e^{\kappa d(X)}
 \sum_{r=0}^2L_{\partial_\tau^r F_{\tau,X}}(p_*)\le\mathcal N_f,
 \tag{J11a}
\]

uniformly in \(\tau\), with further fixed slack if \(d(X)\) and the support diameter differ by a fixed geometric factor. Choose \(p_*\) at least as large as the moment orders needed in Lemma J-C. The same requirement is imposed on the finite background derivatives when they are used. This pays the factors \(e^{2\alpha\sum\operatorname{diam}X_i}\) in (J4).

The polynomial bounds mean finite sums of powers of local \(A_b\)'s, with degree bounded independently of scale; support-volume powers are allowed when the localization exponent has slack. Raw local moments convert these bounds into (J11a) without powers of the cutoff radius.

#### Theorem J2

Under these hypotheses,

\[
 \sup_{|\tau|\le g}
 \left|\frac{d^2}{d\tau^2}\mathcal T_\tau f(U)\right|
 \le C\mathcal N_f,
 \tag{J12}
\]

where \(C\) is uniform in volume, cutoff radius, microscopic depth, and \(g\) within the admitted small-coupling range. Therefore

\[
 \boxed{
 |\mathcal T_gf(U)-f(\mathcal U(U,0))|
 \le\tfrac12C g^2\mathcal N_f.
 }
 \tag{J13}
\]

**Proof.** Expand each term of (J11) into its localized supports. The first term is bounded directly by the anchored source norm and local moments. For the two covariances, apply HC-W and sum the exponential separation between the source support and the score support. For the third cumulant, apply (J4) at \(n=3\) and sum over both score supports. The sum is finite because

\[
 \sum_{y,z}e^{-c\operatorname{diam}\{x,y,z\}}<\infty
 \tag{J14}
\]

uniformly in the lattice volume; it is bounded by a convergent sum of an exponential times a fixed polynomial in the diameter. Support-size factors are absorbed into the localization weights. This proves (J12). Integrate twice from zero and use (J10) to obtain (J13). \(\square\)

#### Finite background jets

Suppose the same localized polynomial bounds hold after up to \(m\) background derivatives, with the corresponding localized derivatives of the action. Differentiating a normalized expectation or cumulant adds only finitely many differentiated observables and one additional score insertion per derivative. Applying Lemma J-C at orders at most \(m+3\) therefore gives

\[
 \|\mathcal T_gf-\mathcal T_0f\|_{C^m_{\rm loc}}
 \le C_m g^2\mathcal N_f.
 \tag{J15}
\]

The norm here is the specified finite collection of background derivatives, with its localization weights. Polynomial coordinate factors used to extract a zero-momentum curvature jet can be included, since the rooted exponential decay sums every fixed spatial moment. For a curvature-quadratic marginal projection, the required background Hessian uses \(m=2\); cumulants through order five suffice.

The cancellation (J10) is an identity as a function of the background, so its background derivatives also vanish. No new first-order term appears when taking the marginal projection.

### 5. Which hypotheses the regular source construction supplies

For the full-torus CMP **109**/**116** regular small-field model, and the explicitly specified threshold-robust extension in Proposition H-cut, the analytic localization bounds have a fixed small physical-field radius. This supplies the action-polynomial bounds in condition 3. The relevant estimates are CMP **116**, (1.19)–(1.21), (1.33)–(1.40), and the decomposition before Lemma 2.

For example, write the localized classical remainder as
\(W_Y(Z)=\sum_{n\ge3}W_{Y,n}(Z)\), with an analytic bound on a fixed physical-field ball. On a smaller ball,

\[
 \left|\partial_\tau\{\tau^{-2}W_Y(\tau A)\}\right|
 \le C w_Y\,\|A\|_Y^3,
 \qquad
 \left|\partial_\tau^2\{\tau^{-2}W_Y(\tau A)\}\right|
 \le C w_Y\,\|A\|_Y^4,
 \tag{J16}
\]

where \(w_Y\) is exponentially localized. The cubic term has zero second amplitude derivative; the second bound begins at degree four. The old analytic action difference has first and second amplitude derivatives bounded by localized multiples of \(\|A\|_Y\) and \(\|A\|_Y^2\). Bounded analytic Jacobian terms have the same finite-polynomial structure. Fixed background derivatives change constants and support factors but do not introduce inverse powers of the running coupling on this fixed analytic domain.

The small weighted Hessian estimate of Proposition H is uniform along \(|\tau|\le g\), using \(g\|A\|_\infty\le\epsilon_{\rm cut}\) and the fixed analytic reserve. The gradient at \(A=0\) is locally bounded; it is in fact of order \(|\tau|\) for the action in (J8). Thus the companion reflected-diffusion moment argument applies. It supplies condition 1 without any factor depending on \(r(g)\).

For condition 2, a localized analytic input mark on the admitted enlarged domain gives the required finite derivatives by Cauchy estimates and the minimizing-field response. The source's localizing expansions, or their finite derivatives, retain the anchored support weights. This is an input-class assumption for the operator theorem: one must still prove that repeated transport keeps the old mark in that class with a controlled norm.

The fixed-domain source argument is not silently extended to every multiscale mixed history. The full-torus regular carrier of the final construction is matched using the explicit later LFR I formulas (1.8)–(1.9), which specify \(\exp(ig_jA_j)\) and \(|A_j|<g_j^{-1}\delta_j\); the detailed comparison is in Part II.B. Theorem J2 itself applies to any carrier satisfying its stated hypotheses.

### 6. Consequence for the marginal block

For dimensionless current-unit source functions, write \(\widehat{\mathcal T}_\tau=L^4\mathcal T_\tau\). The factor compares dimension-four densities before and after one block step; it is a fixed constant in the estimates above. Let \(\Pi\) be a finite marginal projection defined by the local curvature jets, and let the irrelevant subspace satisfy \(\Pi f=0\). Suppose the engineering-rescaled classical map preserves this filtration:

\[
 \Pi\widehat{\mathcal T}_0f=0\quad\text{for irrelevant }f,
 \qquad
 \Pi\widehat{\mathcal T}_0q=\Pi q\quad\text{for the chosen marginal basis }q.
 \tag{J17}
\]

Then (J15), with the fixed derivative order defining \(\Pi\), implies

\[
 \|\Pi\widehat{\mathcal T}_g|_{\mathcal R}\|
 \le Cg^2,
 \qquad
 \|\Pi\widehat{\mathcal T}_g|_{\mathcal M}-I\|
 \le Cg^2.
 \tag{J18}
\]

These are the blocks \(B_k=O(g_k^2)\) and \(A_k=I+O(g_k^2)\) required by the bounded-remainder cocycle theorem in **Part VII.B**. A bounded \(C_k\) is allowed there.

This reduces the regular source question further. The marginal estimate can be attacked through actual normalized finite jets, with all score terms included and no cutoff-polynomial loss. What remains is to prove the classical filtration statement for the selected source projection, the contracting irrelevant norm under the full regular map, and its compatibility with R-generated and boundary coefficients. The finite-jet argument does not already prove those Banach-space remainder estimates or the all-history S2 theorem.

### Appendix: classical reproduction of curvature-quadratic jets

For the bulk flat-background minimizing map, the classical filtration statement in (J17) can be proved directly. The finite-volume qualification at the end of this appendix is part of the statement.

#### A. Linearized averaging reproduces physical constant curvature

In fine lattice units, take a Lie-algebra-valued antisymmetric array \(F_{\mu\nu}\) and the affine one-form

\[
 A_{F,\mu}(x)=-\tfrac12\sum_\nu F_{\mu\nu}x_\nu.
 \tag{JA1}
\]

It has constant discrete curl \(dA_F=F\) and satisfies

\[
 d^*A_F=0,\qquad d^*dA_F=0.
 \tag{JA2}
\]

At the trivial field, the averaging operation of CMP **109**, (0.8), (0.11), and (0.12), linearizes to an arithmetic average of path sums joining the endpoints of a coarse bond. The paths are finite and are translated with the coarse bond. For a constant one-form, every path sum is its contraction with the endpoint displacement. Translating an affine one-form by a coarse translation \(Lv\) changes the integrand by a constant one-form. Consequently

\[
 (QA_F)_\mu(y)
 =-\tfrac12\sum_\nu L^2F_{\mu\nu}y_\nu+c_\mu(F)
 \tag{JA3}
\]

in coarse lattice units, where \(c_\mu(F)\) is independent of \(y\). This constant one-form is a linearized gauge gradient. Equation (JA3) is independent of the detailed path areas. Thus the physical constant curvature is reproduced exactly. Iterating the averaging gives the corresponding statement with \(L\) replaced by \(L^j\).

#### B. The constrained minimizer reproduces the affine field modulo gauge

Let \(H_1\) be the actual linear derivative of the constrained minimizing map at the trivial field. The quadratic Wilson action is the curl energy. By (JA2), \(A_F\) is stationary under all compactly supported variations, and in particular under those preserving its blocked field. The constrained minimizer with data \(QA_F\) therefore equals \(A_F\) modulo its gauge representative:

\[
 H_1(QA_F)=A_F+d\lambda.
 \tag{JA4}
\]

This statement on polynomial fields can be justified without treating an unbounded affine field as an allowed small background. First multiply \(A_F\) by a smooth lattice cutoff equal to one in a ball of radius \(R\). The failure of stationarity is supported in its outer annulus and grows only polynomially in \(R\). The inverse of the constrained, gauge-fixed quadratic precision is exponentially local and has a uniform gap. Its response at a fixed interior root to that annular residual tends to zero like a polynomial times \(e^{-cR}\). The same argument applies to the linearized minimizing map. Taking the limit of the local kernels proves (JA4) on the infinite lattice. Equivalently, the exponentially decaying inverse extends its inverse identities to polynomially growing fields by absolute convergence.

The argument concerns uniqueness modulo gauge. A gauge-fixed representative of the affine field may differ from (JA1), but a gauge-invariant observable and its quadratic jet give the same result. The total-depth minimizing maps satisfy the same statement: apply it to \(Q^jA_F\), then use the variational nesting identity. Thus this is not a replacement of the actual accumulated minimizer by a nearest-neighbor guess.

#### C. The nonlinear minimizing map has the same quadratic source jet

Let \(f\) be an analytic gauge-invariant localized mark, and assume the gauge Lie algebra is semisimple. Its first derivative at the trivial field vanishes:

\[
 Df(0)=0.
 \tag{JA5}
\]

Indeed, constant gauge transformations act by the adjoint representation separately on each bond variation. An invariant linear functional on a semisimple Lie algebra is zero. Gauge invariance then also makes the Hessian vanish when one input is a linearized gauge direction.

For the nonlinear minimizing map \(\mathcal U\), the Hessian chain rule therefore reduces to

\[
 D^2(f\circ\mathcal U)(0)[a,b]
 =D^2f(0)[H_1a,H_1b].
 \tag{JA6}
\]

There is no contribution involving \(D^2\mathcal U\), because it is multiplied by \(Df(0)\). Equations (JA3)–(JA6) prove that evaluation on two constant-curvature test directions preserves the curvature-quadratic coefficient in physical units.

For a simple gauge algebra, color invariance reduces its color contraction to the invariant quadratic form. In four dimensions, the six two-form components then have a symmetric \(6\times6\) coefficient matrix, giving the 21 curvature-bilinear jets. For a semisimple algebra with several simple factors, the corresponding multiplicities must be retained. No commutativity assumption on the Lie-algebra values of the test \(F\)'s is needed: their noncommutative effects begin at higher field order and do not alter the bilinear calculation.

If \(\Pi\) denotes this local zero-momentum curvature projection and source densities are compared in their current lattice units, then

\[
 \boxed{\Pi\bigl(L^4\mathcal T_0f\bigr)=\Pi f.}
 \tag{JA7}
\]

The factor \(L^4\) is the engineering rescaling for a dimension-four density. It compensates the two factors \(L^{-2}\) relating fine and coarse curvature components. In physical-density notation the equality has no extra factor. Consequently the normalized classical map has identity marginal block and zero irrelevant-to-marginal block. An order-one marginal-to-irrelevant lattice remainder is still permitted.

#### D. Local tests and periodic volumes

The curvature projection can be defined by applying the Hessian to cutoff affine tests and then taking the cutoff radius to infinity. Exponential localization of the Hessian and of \(H_1\) makes all spatial moments converge. This does not impose a continuous family of nonzero constant fluxes on a periodic torus.

At a fixed finite periodic volume, an unrestricted affine test is not periodic. The rigorous bulk comparison is instead with the infinite-volume local kernels. When their periodization error has the source's exponential bound, (JA7) has an error

\[
 O\left(e^{-cD/h_k}\right)\|f\|_{\rm input},
 \tag{JA8}
\]

up to fixed polynomial factors absorbed into the exponent, where \(D\) is the torus linear size. These errors are summable over the ultraviolet steps at fixed terminal scale:

\[
 \sum_{k<K}e^{-cD/h_k}
 \le\sum_{m\ge1}e^{-c(D/h_K)L^m}<\infty.
 \tag{JA9}
\]

For uniformity in the family of tori, require \(D/h_K\ge d_0>0\); the expanding-torus route satisfies this condition at fixed terminal scale. The sum is then bounded by a constant depending only on \(d_0,c,L\). To control an inverse cocycle as well, summability alone is insufficient: each perturbed marginal map must remain invertible. One can choose \(D/h_K\) sufficiently large along the cofinal expanding-torus sequence that the wrap-error norm is smaller than the remaining near-identity invertibility margin, or separately verify the finitely many infrared maps. Under that additional condition the errors contribute a bounded extra cocycle factor. This finite-volume conclusion uses the explicit periodic-versus-infinite kernel comparison; if that comparison has not been included in a chosen norm, keep (JA7) as the infinite-volume bulk identity and retain (JA8) as the required finite-volume interface. Boundary and mixed-history carriers do not inherit the affine-translation argument automatically.

---

## Part VI.B. Conditional analytic operator strategy

**Status.** The normalized KP and Cauchy implications in this note are proved. Two source-specific input estimates remain hypotheses: the generic-root localization bound (AO3), including the norm of the original insertion after composition with the minimizing map, and the classical contraction (AO11) in the chosen complex analytic norm uniformly in block depth. Source results for specified action insertions and real minimizing backgrounds do not automatically prove these arbitrary-source Banach-space estimates. This is a precise conditional operator theorem and a strategy, not a completed regular marked induction.

### 1. A norm that distinguishes the two estimates needed

For a current-scale rooted insertion, use a decomposition

\[
 f=\sum_{X\ni x}f_X,
 \qquad
 \|f\|_{\alpha,\kappa,x}
 =\inf\sum_{X\ni x}e^{\kappa d(X)}
       \sup_{\mathcal D(X,\alpha)}|f_X|.
 \tag{AO1}
\]

The infimum is over gauge-invariant analytic localized decompositions on the source background domain. The dimension-four physical factor is removed when using this norm. Supports can contain the root through a connecting path, whose length is included in \(d(X)\). Fixed polynomial support factors can be included without changing the discussion, by using localization slack.

The chosen exponent must also retain the reserve required by the finite-jet theorem: its local coefficient and gradient moment norms, including the zeroth source coefficient, satisfy the exponentially weighted per-bond and per-root bounds (J11a), with enough slack to pay the support-diameter factors in its cumulant estimate. Plain unweighted support summability would not suffice.

Let \(\Pi\) be the finite curvature-quadratic projection and remove the identity coefficient. Assume explicitly that coefficient extraction and the embedding of the chosen marginal representatives are bounded in the input and output norms, uniformly in scale and support; thus \(\Pi^2=\Pi\) and \(\sup_k\|\Pi\|_k<\infty\). For the quantum perturbation of the complete analytic norm, a small bound tending to zero is enough. Only its finite marginal projection needs the sharper \(O(g^2)\) bound of the companion source-jet note. Confusing these two needs would force an unnecessarily strong analytic estimate.

### 2. The one-root insertion bound

Consider the actual full-torus regular small-field integral with its explicit running independent-field cutoff. The source construction gives a uniformly convergent unmarked polymer gas, with strict weighted KP slack on the chosen complex background domain.

Take a single localized insertion \(I_X(U,A)\), supported on \(X\) in background and fluctuation coordinates, analytic in the admitted background domain and in the interpolation parameters used for localization. Suppose

\[
 |I_X(U,A)|\le\iota_X
 \quad\text{on the retained cutoff and localization domain}.
 \tag{AO2}
\]

Repeating the source numerator expansion inserts \(I_X\) exactly once. It produces one distinguished activity \(J_X(Z_0)\), with \(Z_0\) connected to \(X\); all other polymer activities are the unchanged unmarked ones. This is the algebra of CMP **119**, (3.44)–(3.47).

The quantitative extension must be proved at the local Gaussian estimate, before any quotient is formed. Use the following **fully weighted individual-root activity norm as the primary hypothesis**. Let \(\bar X\) be a connected coarse cover of the prescribed input root support. Choose the polymer length \(\ell_{\rm out}\) so that the output size of a connected union is at most the sum of its polymer lengths. Require

\[
 \mathcal A_X:=
 \sum_{Z_0}e^{a(Z_0)+\kappa\ell_{\rm out}(Z_0)}
       \sup_{\mathcal D_{\rm out}}|J_X(Z_0)|
 \le C\iota_X
       e^{c_{\rm root}d_{\rm in}(X)+\kappa d_{\rm out}(\bar X)}.
 \tag{AO3}
\]

The supremum uses the complete required complex background domain, including the auxiliary \(J\) variables; any localization-parameter bounds needed to construct the activities must be part of the verification. All interaction, cutoff-defect, and extension-support sums have already been taken in (AO3). Constants are uniform in input support, volume, and coupling. Thus (AO3) pays **both** polymer-animal entropy and the entire KP factor \(e^{a(Z_0)}\), including its contribution on arbitrarily long extensions of the root. Only costs belonging to the prescribed input root may be put into \(c_{\rm root}d_{\rm in}(X)\). This is an assumption on individual root activities, not on the final normalized marked cluster sum.

A pointwise estimate \(|J_X(Z_0)|\le C\iota_Xe^{c|X|}e^{-\kappa_*d(Z_0;X)}\), with merely \(\kappa_*>\kappa\), would not suffice: the remaining exponent must additionally pay extension-animal counting and the extension part of \(a(Z_0)\). Taking the full sum (AO3) as the hypothesis removes that ambiguity.

A concrete candidate derivation retains the local Gaussian comparisons in CMP **116**, (2.15)–(2.34), uses the insertion bound once, and pays a local determinant cost on the prescribed root region. Added blocks should be paid by interaction, cutoff-defect, or interpolation-decay factors. For an insertion already localized and uniformly bounded throughout the interpolation domain, Cauchy estimates control derivatives hitting it. The missing verification is that the original arbitrary analytic source composed with the minimizing map admits such a decomposition with the claimed input norm and per-block costs. Linearity of the source's specified numerator expansion does not establish that verification. No whole-volume complex density ratio may replace it.

Assuming (AO3) and strict weighted KP slack, divide by the unmarked partition function through the rooted connected expansion. The one-root KP estimate proves

\[
 \sum_Ye^{\kappa d_{\rm out}(Y)}
  \sup_{\mathcal D_{\rm out}}|\mathcal E_{I_X}(Y)|
 \le\mathcal A_X
 \le C\iota_X
       e^{c_{\rm root}d_{\rm in}(X)+\kappa d_{\rm out}(\bar X)}.
 \tag{AO4}
\]

The extra root factor \(e^{a(Z_0)}\) in the rooted KP theorem is already present in the left side of (AO3). The length inequality pays the output connected-union weight. Analyticity follows from uniform absolute convergence of analytic localized terms. Normalization has therefore been handled exactly; (AO4) is a bound on the normalized insertion operator.

#### Preserving a fixed localization norm

One must check the input and output weights in (AO4), rather than discard them as unspecified constants. Over a fixed block of \(N\) RG steps, the same physical support satisfies

\[
 d_{\rm out}(\bar X)\le q_N d_{\rm in}(X)+C_N,
 \qquad q_N\longrightarrow0
 \quad(N\longrightarrow\infty).
 \tag{AO5}
\]

Use connected \(M\)-block tree size in (AO1) and (AO5). An elementary covering proof gives \(q_N\le C_dL^{-N}\) and \(C_N\le C_d\): traverse a spanning tree of the input \(M\)-blocks, using each edge at most twice, and divide that traversal into pieces of at most \(L^N\) edges. Each piece has diameter at most one coarse-block scale and meets at most a dimension-dependent number of coarse \(M\)-blocks. Their connected coarse cover has at most \(C_d[1+L^{-N}d_{\rm in}(X)]\) blocks. A fixed extra layer changes only \(C_d\). This proof concerns the **prescribed input support**. Random localization extensions are not silently coarsened away; their weights and counting remain in (AO3).

The number of independent coordinates in the prescribed input support is bounded by \(CM^d(d_{\rm in}(X)+1)\), uniformly in scale. An \(MR_k\)-block count would carry an additional \(R_k^d\) volume factor and cannot be substituted without paying it. The constant \(c_{\rm root}\) in (AO3) must include all prescribed-root costs, including its portion of the KP factor, local Gaussian total variation, determinants, interactions, and interpolation/Cauchy support factors. Require

\[
 c_{\rm root}+q_N\kappa<\kappa.
 \tag{AO6}
\]

with strict slack. Then summing (AO4) against the input decomposition gives a bounded operator in a single localization norm. Its bound \(C_N\) is independent of ultraviolet depth and volume. These parameter inequalities are part of the norm choice; an arbitrary preassigned exponent need not work.

For an \(N\)-step statement, (AO3) must be verified either for the actual joint \(N\)-step marked expansion or uniformly at each of its \(N\) individual steps on a compatible chain of intermediate complex domains and support norms. In the latter case, all finite products of operator and localization constants are included in \(C_N\). A one-step bound on only the initial and final domains does not establish the \(N\)-step hypothesis.

### 3. Analytic reserve and the small quantum perturbation

The insertion estimate needs an actual common analytic domain. The required analytic reserve is a **uniform complex directional tube in a specified local chart and regularity norm**, not merely membership in a set carrying a smaller parameter label. Write \(\Phi_0=(\mathcal U_0,\mathcal J_0)\) for the classical background and auxiliary-current data. For some \(\delta_N>0\), independent of support, volume and ultraviolet depth, require

\[
 B_{\rm chart}\bigl(\Phi_0(U,J),\delta_N\bigr)
 \subset\mathcal D_{\rm in}(X,\alpha)
 \quad\text{for every admitted }(U,J)\in\mathcal D_{\rm out},
 \tag{AO7}
\]

with the same tube for every allowed localization interpolation and, in the successive-step version, on every intermediate domain. The chart norm includes all required \(U\) and auxiliary \(J\) regularity conditions. A construction using a smaller parameter domain \(\mathcal D_{\rm in}(\theta\alpha)\), \(\theta<1\), is sufficient only after proving its chart stability gives this actual tube. Expected old-scale factors \(L^{-N}\) for potential and \(L^{-2N}\) for curvature, together with the hierarchy-domain inclusion in CMP **109**, p. 263, are proposed ingredients. They are not a verification of (AO7) for the chosen source norm and all interpolations. Mixed histories require additional checks.

For a block starting at scale \(k\), retain the exact smallness quantity

\[
 \varepsilon_{k,N}:=
   \max_{k\le j<k+N} g_j r_{\chi,j},
 \qquad g_{k,N}:=\max_{k\le j<k+N}g_j.
 \tag{AO7a}
\]

The corresponding fluctuation-map estimate required on the actual cutoff is

\[
 \|\Phi_{\boldsymbol g}-\Phi_0\|_{\rm chart}
 \le C_N\varepsilon_{k,N},
 \tag{AO8}
\]

This estimate includes the auxiliary \(J\) data and all localization interpolations used in the root expansion. Assume \(C_N\varepsilon_{k,N}\le\delta_N/2\). A directional Cauchy estimate inside the tube then gives

\[
 \sup|f_X(\Phi_{\boldsymbol g})-f_X(\Phi_0)|
 \le C_N\varepsilon_{k,N}
       \sup_{\mathcal D_{
       \rm in}(X,\alpha)}|f_X|.
 \tag{AO9}
\]

The Cauchy estimate can be taken in the direction of the whole perturbation in the supremum norm; it does not require a factor equal to the number of coordinates. To use it in the rooted norm, the localization of the composed difference must satisfy the generic-root bound (AO3) with the norm just obtained. This is included in the stated hypothesis, not inferred from the Cauchy estimate alone.

Under these hypotheses, apply the normalized one-root operator estimate to the difference. The background-dependent quantity \(f_X(\Phi_0)\) is constant in the fluctuation integration, so it exits the normalized integral exactly. Consequently

\[
 \boxed{
 \|\widehat{\mathcal T}^{(N)}_{\boldsymbol g} f
       -\widehat{\mathcal T}^{(N)}_0 f\|_{
       \alpha,\kappa,x}
 \le C_N\varepsilon_{k,N}\|f\|_{\alpha,\kappa,x}.
 }
 \tag{AO10}
\]

The hats include the fixed engineering factor \(L^{4N}\) for the \(N\)-step block. Only after proving fixed-block trajectory comparability may \(\varepsilon_{k,N}\) be replaced by \(C_Ng_{k,N}r_\chi(g_{k,N})\); otherwise the displayed maximum must be retained. The admitted asymptotically free estimates and a specified polylogarithmic radius can supply that comparison for fixed \(N\). A fixed extra finite power of the cutoff radius would still tend to zero when multiplied by the coupling, but would have to be displayed in the input estimates. Equation (AO10) does not assert an \(O(g^2)\) bound for the whole analytic norm.

The detailed domain and support inequalities (AO6)–(AO8) are indispensable. The source-free action bound alone, without an input source decomposition and analytic reserve, would not prove this operator estimate.

### 4. Classical irrelevant contraction and all 21 curvature coefficients

The point-root gauge argument in CMP **119**, (3.48)–(3.72), suggests the appropriate projection. Before the final Euclidean-symmetry reduction, its retained term is a general curvature-bilinear form. Thus an arbitrary point-root insertion requires the full 21-dimensional form for a simple gauge algebra, rather than its scalar subspace alone. The source theorem for its action terms on minimizing backgrounds is not already the operator-norm statement for every analytic source.

The alternative axial-gauge proof suggests the following derivation. On a root neighborhood of size \(R\), the old-scale connection has size \(L^{-2N}\) times current curvature, with polynomial support factors. The first derivative of a semisimple invariant mark is zero. In the quadratic term, replacing curvature and transport by their root value should cost one further scale power; a cubic remainder has at least six. This explains the expected \(L^{-(5-\varepsilon)N}\) gain. To turn this into contraction of (AO1), one must prove the complex-domain inclusion, localize the remainder with controlled weights, and verify that the constant is uniform in \(N\). The source's real-background gain alone does not prove those requirements.

The precise additional **classical analytic contraction hypothesis** is

\[
 \|(1-\Pi)\widehat{\mathcal T}^{(N)}_0
      |_{\ker\Pi}\|
 \le C L^{-(1-\varepsilon)N}.
 \tag{AO11}
\]

If (AO11) holds with a constant independent of \(N\), choose one fixed \(N\) making the right side less than one half. Under the generic-root and analytic-domain hypotheses above, (AO10) then gives strict interacting irrelevant contraction at small coupling. With the hypotheses of the companion finite-jet theorem also verified, the resulting blocks satisfy

\[
 A=I+O(g_{k,N}^2),\quad B=O(g_{k,N}^2),\quad
 C=O(1),\quad \|D\|<1.
 \tag{AO12}
\]

This conditional conclusion combines analytic remainder control with the normalized finite-jet estimate. The projection's classical reproduction, which is weaker than contraction of a whole remainder norm, is proved in the affine-test appendix of **Part VI.A**. Periodic finite-volume errors and every mixed-history analytic-domain interface retain their qualifications.

For (AO12), the finite-jet estimate must likewise hold through the joint block or along all intermediate domains. With \(N\) fixed, its accumulated error is bounded by \(C_N\sum_{j=k}^{k+N-1}g_j^2\le C_NN g_{k,N}^2\), where the finite factor \(N\) is included in the displayed block constants. The boundedness of \(\Pi\) stated after (AO1) is used when passing from (AO10) to the remainder and off-diagonal blocks.

### 5. A remaining issue even after these operator estimates

An arbitrary point mark need not have a marginal coefficient described by a single universal 21-dimensional matrix. Fixed blocking can leave a dependence on the position of the microscopic root within a block and can distribute the output over several nearby coarse roots. Its natural marginal object is then a localized coefficient kernel in the source position.

Translation covariance of the **summed action density** does not prove that the marginal map of every individual point root is the same matrix. Applying a separate inverse matrix depending on the random carrier would also change the observable. Even a deterministic root-phase-dependent normalization must be reconciled with the required continuum translation covariance.

To finish the regular point-source induction, the source-profile space must therefore be specified. One promising decomposition separates the block-constant source component from its zero-average or source-gradient part. The first should use the common deterministic bulk cocycle. The second must be shown to contract, together with the irrelevant field remainder, in a norm controlling the coefficient kernel's spatial moments. Alternatively, a permitted averaging over blocking origins must be built into the transport construction and its normalization explicitly.

The analytic one-root bound and the finite-jet estimate are usable on this enlarged source-profile space, but they do not by themselves establish its spectral decomposition. This profile issue, the mixed-history domain interfaces, and the normalized R/exterior composition remain explicit before claiming a full old-point-insertion theorem.

---

## Part VI.C. Source analysis for the complex contraction requirement

Primary source: Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP119 (1988), 243–285.

### Source conclusion

**CMP119 Theorem 2, p.263, (2.43), and its pointwise conclusion p.283, (3.67), establish the dimension-five gain for the source's prescribed localized action on sufficiently regular minimizing configurations \(U_k=U_k(V)\), including the real configurations admitted by its characteristic functions. They do not state a supremum estimate on the entire complex background domain for an arbitrary rooted input.**

Theorem 2 explicitly makes its constant independent of \(j,k\), the regions, and the torus. Thus its stated source estimate is uniform in scale separation. The unresolved uniformity is the retention of this control after passing to arbitrary marks and the chosen **complex analytic Banach norm**, not uniformity of the theorem itself.

### What the proof supplies

The local Taylor and gauge-identity argument is linear in the analytic input. Before the Euclidean-symmetry reduction, (3.56)–(3.57) retain a general curvature-bilinear tensor. Therefore the full 21-component curvature projection for a simple gauge algebra in four dimensions is compatible with the algebra; an arbitrary point mark should not use the scalar reduction justified for the resummed Euclidean-covariant action.

The alternative proof (3.68)–(3.72), pp.283–284, gives the intended mechanism: the axial-gauge connection has two scale powers, replacing curvature and transport by their root values introduces a third-power remainder, and the cubic Taylor term has at least six powers. The resulting quadratic replacement error has five powers. Exponential localization pays large supports.

The analytic extension is not absent from the source's discussion. On p.280 it discusses replacing backgrounds by complex variables for the fuller renormalization analysis. But the final paragraph on p.284 expressly requires the rooted representation (2.26), (2.27) **and its corresponding properties** to elaborate the proof. Those include the actual localized analytic domains, gauge invariance, and uniform exponential bounds. Merely removing finitely many jets does not supply them.

### Missing interface for AO11

For the complete complex output norm domain, uniformly in ultraviolet depth, volume, and separation \(N\), the arbitrary-root adaptation still needs:

1. A holomorphic rooted gauge/minimizer chart with a verified Cauchy margin in the actual input domain and controlled running-radius ratios.
2. A connection bound \(C P(N,R)L^{-2N}\) and curvature/transport replacement error \(C P(N,R)L^{-3N}\), with a fixed polynomial \(P\), throughout that complex domain and its localization deformations.
3. A rooted output decomposition whose localization reserve absorbs support factors and large-support tails without hidden exponential growth in \(N\).
4. A bounded curvature projection consistent with the chosen root/coefficient-profile convention.

With these estimates, the source Taylor argument yields

\[
\|(1-\Pi)\widehat{\mathcal T}^{(N)}_0f\|_{
\alpha,\kappa,x}
\le C_\epsilon L^{-(1-\epsilon)N}
\|f\|_{\alpha,\kappa,x},
\qquad f\in\ker\Pi,
\]

where \(C_\epsilon\) is independent of \(N\). Polynomial losses can be absorbed in \(L^{\epsilon N}\). The current notes have not verified all four requirements in this form.

Two shortcuts are invalid: holomorphicity alone does not promote a bound on a real slice to a bound on a complex neighborhood; and an estimate with an uncontrolled \(C_N\) does not justify choosing \(N\) large enough for contraction. AO7's domain inclusion, even when proved, is not by itself the required two-power/three-power geometric estimate.

### Status to retain

**AO11, the strict irrelevant-block contraction in AO12, and the resulting analytic old-mark induction remain conditional on this complex-domain interface and the separately stated generic-root localization input to AO3/AO10.** The finite-jet results remain separate completed modules. The source classical estimate remains valid in its stated scope.

The relevant primary text is CMP119, pp.259–263 and 279–284, including the displayed formulas on pp.263, 280, and 284.

---

## Part VII.A. Common marginal normalization with a small generated remainder

### Why this changes the next proof target

A summable bound on every marginal transport correction is sufficient, but it is stronger than S2 requires. The route permits fixed powers of the logarithm of the remaining physical scale ratio. An almost-marginal one-step factor of the form \(I+O(g_k^2)\) can produce exactly that growth after the microscopic field is normalized at a fixed physical scale. It need not be replaced by \(I+O(g_k^{2+\epsilon})\).

There are two qualifications. The normalization must be the inverse of the **actual finite-dimensional marginal cocycle**, with its coupling to the irrelevant remainder included. Also, the required block estimates must be proved for the **frozen positive transport of the actual insertion**. A derivative of a coupling-dependent transformation does not establish those estimates without its kernel-score terms.

This section proves the cocycle statement, including the irrelevant component. It is a new sufficient strategy for the remaining marked induction, not a claim that the Yang–Mills block estimates have already been verified.

### 1. Exact block evolution modulo the identity

Let \(h_k=aL^k\), \(0\le k\le K\), and \(h_K=\ell_0\). Work modulo deterministic constants. At scale \(k\), suppose an actual transported finite family has a decomposition into a marginal coefficient \(m_k\in\mathbb R^d\) and a remainder \(r_k\in\mathcal B_k\). The finite-dimensional marginal space may have \(d=1\) for the scalar or \(d=21\) for the full curvature-bilinear family. The norms on \(\mathcal B_k\) include the current physical scaling and spatial anchoring; they are not microscopic supremum norms.

Assume the exact linear transport has block form

\[
\begin{pmatrix}m_{k+1}\\r_{k+1}\end{pmatrix}
=
\begin{pmatrix}A_k&B_k\\C_k&D_k\end{pmatrix}
\begin{pmatrix}m_k\\r_k\end{pmatrix}.
\tag{Z1}
\]

The maps may depend on the admitted source-free coupling history. No autonomous beta function or commutativity of matrices is assumed. Suppose

Here the coupling history is a **deterministically specified trajectory**, not a random large-field history. The matrix in (Z6) must be one common renormalization for the field. If a geometrical history changes the marginal map, its difference from a common bulk map must be bounded separately; choosing a different inverse cocycle on each carrier would define a different observable and would not prove the route's claim.

For a point insertion, one must also keep its localized coefficient kernel over neighboring coarse sites and its position relative to the blocking cells. An invariant zero-momentum action coefficient does not by itself show that all such point-root coefficients have the same finite-dimensional cocycle. A proof must identify their common bulk part and control the spatially varying/source-gradient part in the remainder norm. This is a substantive hypothesis of a field-level application of the theorem.

\[
\|A_k-I\|\le a_1\varepsilon_k,\quad
\|B_k\|\le b_1,\quad
\|C_k\|\le c_1\varepsilon_k,\quad
\|D_k\|\le q<1,
\tag{Z2}
\]

where \(0\le\varepsilon_k\le\varepsilon_*\) is nondecreasing. The letters \(a_1,b_1,c_1\) are fixed norm constants, unrelated to the lattice spacing \(a\). Consider a family initially lying on a graph

\[
r_0=S_0m_0,\qquad \|S_0\|\le s_*.
\tag{Z3}
\]

It is enough to take \(s_*\) and \(\varepsilon_*\) sufficiently small in terms of \(a_1,b_1,c_1,q\). An initial bounded number of preparatory scales can be included separately if their exact maps and inverses have uniformly bounded norms and put the family in (Z3).

#### Theorem Z: normalized transport with logarithmic growth

Under (Z1)–(Z3), there exist exact graph maps \(S_k\) and invertible marginal matrices \(M_k\) such that

\[
r_k=S_km_k,\qquad m_{k+1}=M_km_k,
\tag{Z4}
\]

and, for fixed constants \(q_1<1,C_Z\),

\[
\|S_k\|\le s_*q_1^k+C_Z\varepsilon_k,
\qquad
\|M_k-I\|\le C_Z\varepsilon_k+b_1s_*q_1^k.
\tag{Z5}
\]

Choose the microscopic matrix normalization so that the terminal marginal coefficient is the identity:

For this displayed formula, first choose the column basis of the initial field family so that its initial marginal coefficient matrix is \(I\). The normalization acts by right multiplication on these columns. If instead its initial coefficient is an invertible matrix \(M_{\rm init}\), replace the right side of (Z6) by \((M_{K-1}\cdots M_0M_{\rm init})^{-1}\). The cancellation (Z15) is then unchanged. Proving that the actual seed family has a uniformly admissible marginal basis is part of an application, not a consequence of the abstract recurrence.

\[
Z_{a,\ell_0}=(M_{K-1}\cdots M_0)^{-1}.
\tag{Z6}
\]

For this normalized family,

\[
\|m_k\|+\|r_k\|
\le C\exp\!\left(C\sum_{j=k}^{K-1}\varepsilon_j\right).
\tag{Z7}
\]

If additionally

\[
\varepsilon_j\le C_\varepsilon g_j^2,
\qquad
g_j^{-2}\ge x_*+c_*(K-j),\quad x_*>0,
\tag{Z8}
\]

then for a fixed exponent \(p_Z\), independent of \(a,K\),

\[
\boxed{
\|m_k\|+\|r_k\|
\le C\left(1+\log\frac{\ell_0}{h_k}\right)^{p_Z}.
}
\tag{Z9}
\]

This is the form of marginal growth permitted in the S2 shell estimate.

#### Proof

Choose \(0<\delta<\min(1/2,1-q)\), and choose \(s_*,\varepsilon_*\) so that

\[
a_1\varepsilon_*+b_1s_*\le\delta,
\qquad
\frac{c_1\varepsilon_*}{1-\delta}
\le(1-q_1)s_* ,
\qquad q_1:=\frac q{1-\delta}<1.
\tag{Z10}
\]

Such positive choices exist: choose \(s_*\) first small enough, then \(\varepsilon_*\) sufficiently small. If \(b_1=0\), the first restriction is even simpler.

Suppose \(\|S_k\|\le s_*\). Define

\[
M_k=A_k+B_kS_k,\qquad
S_{k+1}=(C_k+D_kS_k)M_k^{-1}.
\tag{Z11}
\]

The first inequality in (Z10) gives \(\|M_k-I\|\le\delta<1\), so \(M_k\) is invertible and \(\|M_k^{-1}\|\le(1-\delta)^{-1}\). The other inequalities imply

\[
\|S_{k+1}\|
\le \frac{c_1\varepsilon_k}{1-\delta}+q_1\|S_k\|
\le s_*.
\tag{Z12}
\]

Thus the graph construction continues through every scale, and substitution into (Z1) proves (Z4) exactly. Iterating (Z12) and using monotonicity of \(\varepsilon_k\),

\[
\|S_k\|
\le q_1^k\|S_0\|
 +\frac{c_1}{1-\delta}\sum_{j<k}q_1^{k-1-j}\varepsilon_j
\le s_*q_1^k+\frac{c_1}{(1-\delta)(1-q_1)}\varepsilon_k.
\tag{Z13}
\]

This and \(M_k=A_k+B_kS_k\) establish (Z5). Put
\(u_k=C_Z\varepsilon_k+b_1s_*q_1^k\), increasing \(C_Z\) if necessary. Uniformly \(\|M_k-I\|\le\delta<1/2\), so

\[
\|M_k\|\le e^{u_k},\qquad
\|M_k^{-1}\|\le e^{2u_k}.
\tag{Z14}
\]

Let \(P_k=M_{k-1}\cdots M_0\), with \(P_0=I\). The normalized marginal matrix at scale \(k\) is

\[
m_k=P_kP_K^{-1}
 =(M_{K-1}\cdots M_k)^{-1}.
\tag{Z15}
\]

The order in (Z15) is important; no matrices have been commuted. Equations (Z14)–(Z15), the geometric sum of \(q_1^j\), and \(r_k=S_km_k\) prove (Z7).

Finally, with \(n=K-k\), (Z8) gives

\[
\sum_{j=k}^{K-1}\varepsilon_j
\le C_\varepsilon\sum_{s=1}^{n}\frac1{x_*+c_*s}
\le\frac{C_\varepsilon}{c_*}
 \log\left(1+\frac{c_*n}{x_*}\right).
\tag{Z16}
\]

Since \(n=\log(\ell_0/h_k)/\log L\), exponentiation proves (Z9). \(\square\)

The same proof permits a nonmonotone \(\varepsilon_k\) if a monotone upper envelope satisfying (Z8) is available, or more generally if the exponentially weighted sums in (Z13) have the stated bound. The lower asymptotically free trajectory estimate is an input here, not proved by this lemma.

### 2. Consequence for the proposed marked norm

Suppose the current-scale norm in (Z1) controls the actual normalized regular shell by

\[
\mathbb E|D_k(F_x,F_y)|
\le C h_k^{-8}\,\mathcal N_k(F_x)\mathcal N_k(F_y)
 e^{-c|x-y|/(h_kR_k)},
\tag{Z17}
\]

and controls the terminal covariance by
\(C\ell_0^{-8}\mathcal N_K(F_x)\mathcal N_K(F_y)\).
If \(\mathcal N_k\le C(\|m_k\|+\|r_k\|)\), Theorem Z gives

\[
\mathbb E|D_k(F_x,F_y)|
\le C h_k^{-8}
 \left(1+\log\frac{\ell_0}{h_k}\right)^{2p_Z}
 e^{-c|x-y|/(h_kR_k)}.
\tag{Z18}
\]

The profile-summation argument then applies to the actual \(R_k\), including the iterated-logarithm correction furnished by the source geometry.

This implication identifies the usable normalization. It does not prove (Z1), (Z2), (Z17), or the terminal estimate for Yang–Mills. In particular, defining a finite-cutoff inverse matrix is not enough unless the marginal coefficient exists, has the uniform near-identity bounds, and is coupled to an actual contracting remainder as above.

### 3. Which source structure can supply the blocks

The CMP119 analysis, printed pp.279–283, (3.48)–(3.67), provides the appropriate **source-free** projection mechanism. Gauge identities reduce the quadratic local Taylor jet to curvature bilinears; hypercubic symmetry reduces an invariant scalar to the Wilson-action direction. After the scalar coefficient and the value at the trivial field are subtracted, the source obtains a \(5-\epsilon\) scale gain. The sum over old cells costs four powers of scale, leaving an irrelevant contraction.

That source calculation must now be applied to the actual one-mark coefficient, with its anchored norms and normalization derivatives included. For tensor marks the marginal block must retain all 21 components and their allowed mixing; hypercubic symmetry does not collapse a general tensor insertion to one scalar.

The practical targets are therefore:

1. Construct an anchored analytic norm on a fixed finite source jet after normalized integration, using the hard-cutoff covariance and second-derivative transport results.
2. Verify the local identity/curvature projection on that exact coefficient and prove the contractive remainder estimate.
3. Prove the marginal and marginal-to-remainder errors at the \(O(g_k^2)\) scale, or another scale whose remaining-time sum is logarithmic. An uncontrolled \(O(g_k)\) error would generally produce \(\exp(C\sqrt{\log(\ell_0/h)})\), which is not the stated fixed logarithmic power.
4. Form the exact marginal cocycle including the graph correction \(B_kS_k\), and normalize at the chosen physical reference scale by (Z6).
5. Compose with the marked R-core estimate and carry remaining-boundary terms in the same norm.

The distinction from a bare product estimate matters. Without the normalization, \(P_k\) contains the product from the microscopic scale up to \(h_k\) and can retain a cutoff-dependent power of \(\log(1/a)\). Equation (Z15) converts that product into the remaining physical-scale product. This is an algebraic cancellation proved above, not an assumption that the marginal errors are summable.

### 4. Coupling history and frozen kernels

CMP109, printed p.264 after (1.22), states smoothness and bounded fixed-order derivatives of its coupling correction in the displayed last argument. The same paper, printed p.298, explicitly notes dependence on the preceding effective couplings. A one-variable derivative estimate alone therefore does not prove the marked block estimates in (Z2).

Theorem Z allows coupling memory: it only needs uniform norms of the actual matrices at every scale along each admitted deterministic coupling trajectory, not a memory-free beta function. To obtain those matrices by differentiating a source-free trajectory, one still has to account for the complete coupling-history derivative and the score of every coupling-dependent kernel. Alternatively, constructing the finite marked jet directly with the unmarked kernel frozen avoids that identification problem.

### Sources and status

- Balaban, CMP119 (1988), pp.279–283, (3.48)–(3.67): the source-free Ward projection, matching scalar counterterm, and irrelevant gain.
- Balaban, CMP109 (1987), pp.264 and 298: the scoped coupling differentiability and history dependence.
- The S2 criterion of the observable route: fixed logarithmic growth is allowed in S2. Its admitted trajectory supplies a possible input of the form (Z8).

**Proved here:** (Z4)–(Z16), under the explicitly stated block hypotheses; and the implication (Z17) to (Z18). **Still to verify for Yang–Mills:** the marked block hypotheses and all-history norm estimate. No S2 closure is claimed from the cocycle algebra alone.

---

## Part VII.B. Common marginal normalization with bounded lattice remainders

This part gives the variant in which a canonical marginal operator can generate an order-one irrelevant lattice remainder, while the reverse mixing is of order \(g_k^2\). It supplements the small-lower-block theorem in **Part VII.A**.

The conclusions below are proved for an explicitly stated linear block recurrence. Applying them to the Yang–Mills source requires estimates for the **actual normalized frozen-kernel marked map**. Source-free coupling differentiability alone does not supply those estimates.

### 1. Hypotheses and graph recurrence

Let \(\mathcal M\) be a fixed finite-dimensional marginal space and \(\mathcal R\) a Banach space of localized irrelevant remainders. Vacuum/identity coefficients have been removed, since they do not enter separated connected covariance. At scale \(k\), suppose the source map is

\[
 \begin{pmatrix}m_{k+1}\\r_{k+1}\end{pmatrix}
 =\begin{pmatrix}A_k&B_k\\ C_k&D_k\end{pmatrix}
  \begin{pmatrix}m_k\\r_k\end{pmatrix},
 \tag{CV1}
\]

with norms satisfying

\[
 \|A_k-I\|\le a t_k,\qquad
 \|B_k\|\le b t_k,\qquad
 \|C_k\|\le c,\qquad
 \|D_k\|\le q<1,
 \quad 0<t_k\le t_*.
 \tag{CV2}
\]

Here \(t_k=g_k^2\). No monotonicity of \(t_k\) is needed for the bounded-graph part. The bounds must hold in a single scale-adjusted anchored norm, and their constants must be independent of the microscopic cutoff and history depth.

Let an actual microscopic seed family have the representation

\[
 r_0=S_0m_0,\qquad \|S_0\|\le K_0.
 \tag{CV3}
\]

Thus the family can have a bounded, order-one lattice remainder. It need not already be an exact Gaussian eigenoperator.

Choose

\[
 K_S\ge\max\left(K_0,1,\frac{2c}{1-q}\right),
 \quad C_E=a+bK_S,
 \tag{CV4}
\]

and take \(t_*\) small enough that

\[
 C_Et_*\le\frac{1-q}{4},\qquad
 K_Sbt_*\le\frac{1-q}{4}.
 \tag{CV5}
\]

#### Proposition CV-G

Define successively

\[
 E_k=A_k+B_kS_k,
 \qquad
 S_{k+1}=(C_k+D_kS_k)E_k^{-1}.
 \tag{CV6}
\]

Then the inverses exist, \(\|S_k\|\le K_S\), and

\[
 \|E_k-I\|\le C_Et_k.
 \tag{CV7}
\]

Every seed in (CV3) evolves exactly as

\[
 r_k=S_km_k,\qquad m_{k+1}=E_km_k.
 \tag{CV8}
\]

**Proof.** If \(\|S_k\|\le K_S\), the first inequality in (CV5) gives
\(\|E_k^{-1}\|\le(1-C_Et_*)^{-1}\). Also

\[
 \|C_k+D_kS_k\|
 \le c+qK_S\le K_S(1+q)/2.
\]

Since \(1-C_Et_*\ge(3+q)/4>(1+q)/2\), (CV6) implies \(\|S_{k+1}\|\le K_S\). This starts from (CV3), and (CV7) follows at the same time. Substituting \(r_k=S_km_k\) into (CV1) proves (CV8). \(\square\)

The point is that the small block is \(B_k\), the map from irrelevant terms into the marginal coefficients. An order-one \(C_k\) is compatible with an effective marginal map \(I+O(g_k^2)\).

### 2. Normalization at a fixed terminal physical scale

For \(j<k\), define the ordered product

\[
 P_{j,k}=E_{k-1}\cdots E_j,\qquad P_{k,k}=I.
 \tag{CV9}
\]

Fix a terminal physical scale \(K\) and a desired marginal coefficient \(v\). Normalize the seed by

\[
 m_0=P_{0,K}^{-1}v,
 \qquad r_0=S_0P_{0,K}^{-1}v.
 \tag{CV10}
\]

This is a finite matrix normalization of the actual microscopic seed family. It can depend on the cutoff, as a renormalization matrix normally does. For an observable defined on the full measure, the product \(P_{0,K}\) must be a **single deterministic bulk cocycle**, common to all geometric carriers and field configurations. It may depend on the deterministic past coupling sequence. It cannot be chosen separately for each random large-field history: that would define different observables on different carriers. History-dependent R and boundary changes must instead be treated as controlled perturbations of this common normalization. Under this requirement, at every intermediate scale,

\[
 \boxed{
 m_k=P_{k,K}^{-1}v,\qquad r_k=S_kP_{k,K}^{-1}v.
 }
 \tag{CV11}
\]

Indeed, \(P_{0,K}=P_{k,K}P_{0,k}\), so
\(P_{0,k}P_{0,K}^{-1}=P_{k,K}^{-1}\). This identity does not require the matrices at different scales to commute. Only the remaining scales occur in (CV11); the potentially long ultraviolet part of the product has canceled exactly.

Suppose the admitted asymptotically free trajectory satisfies

\[
 x_k=g_k^{-2},\qquad
 0<c_-\le x_k-x_{k+1}\le c_+,
 \qquad x_K\ge x_*>0.
 \tag{CV12}
\]

For sufficiently large \(x_*\), (CV7) gives

\[
 \|E_k^{-1}\|\le e^{2C_E/x_k},
 \qquad
 \sum_{j=k}^{K-1}\frac1{x_j}
 \le\frac1{c_-}\log\frac{x_k}{x_K}.
 \tag{CV13}
\]

The second inequality follows by applying
\(\log(x_j/x_{j+1})\ge(x_j-x_{j+1})/x_j\) at each step. Therefore

\[
 \boxed{
 \|m_k\|+\|r_k\|
 \le (1+K_S)\left(\frac{x_k}{x_K}\right)^{\nu}\|v\|,
 \qquad \nu=\frac{2C_E}{c_-}.
 }
 \tag{CV14}
\]

After restoring the engineering dimension of a scalar density, the corresponding bound is

\[
 \|F_{k,x}\|_{\rm anchored}
 \le C h_k^{-4}(g_k^{-2})^{\nu}.
 \tag{CV15}
\]

For a fixed terminal scale and an admitted trajectory, \(g_k^{-2}\) is comparable to the remaining logarithmic scale interval. Thus (CV15) is a power of a physical logarithm, independent of the microscopic lattice spacing at fixed \(h_k\). A summable error \(\sum g_k^2<\infty\) is unnecessary for this conclusion. One does need the allowed running source normalization (CV10).

### 3. Arbitrary stable components

The graph formula is also useful when a source contains a stable component outside the chosen seed family. Put

\[
 \zeta_k=r_k-S_km_k.
\]

Then the exact transformed recurrence is

\[
 m_{k+1}=E_km_k+B_k\zeta_k,
 \qquad
 \zeta_{k+1}=F_k\zeta_k,
 \quad F_k=D_k-S_{k+1}B_k.
 \tag{CV16}
\]

By (CV5),

\[
 \|F_k\|\le q_*:=q+(1-q)/4<1.
 \tag{CV17}
\]

For a finite horizon define \(T_K=0\) and recursively

\[
 T_k=E_k^{-1}(B_k+T_{k+1}F_k).
 \tag{CV18}
\]

Taking \(t_*\) smaller if necessary gives
\(\sup_k\|E_k^{-1}\|q_*<1\); the backward recursion then yields a bound
\(\sup_k\|T_k\|\le C t_*\), independent of \(K\). With

\[
 u_k=m_k+T_k\zeta_k,
\]

the recurrence becomes block diagonal:

\[
 u_{k+1}=E_ku_k,\qquad \zeta_{k+1}=F_k\zeta_k.
 \tag{CV19}
\]

The normalization \(u_0=P_{0,K}^{-1}v\) therefore fixes \(m_K=v\), since \(T_K=0\). At intermediate scales,

\[
 u_k=P_{k,K}^{-1}v,
 \qquad \|\zeta_k\|\le q_*^k\|\zeta_0\|.
 \tag{CV20}
\]

If the microscopic stable norm grows at most like a fixed power \(x_0^N\), then (CV12) gives

\[
 q_*^k x_0^N
 \le x_k^N q_*^k
       \left(1+\frac{c_+k}{x_*}\right)^N
 \le C_{N,q_*,x_*}x_k^N.
 \tag{CV21}
\]

Thus polynomial ultraviolet growth of a stable birth component becomes an allowed physical-scale polynomial bound. The terminal normalization of a completely arbitrary seed may require adjusting its marginal component: one must solve
\((I-T_0S_0)m_0+T_0r_0=P_{0,K}^{-1}v\). This is possible when \(t_*\) is small because \(\|T_0S_0\|<1\). It is not automatic if the problem forbids the corresponding mixing or counterterm. For the microscopic family (CV3), no such extra adjustment is needed.

### 4. A concrete route to the small reverse block

There is an exact one-step cancellation in the actual regular integral that is relevant to proving \(B_k=O(g_k^2)\). It uses a frozen cutoff and does not identify a coupling derivative with an observable derivative.

At fixed admitted background \(U\), fixed cutoff radius \(r\), and fixed old analytic insertion \(f\), consider the auxiliary amplitude interpolation

\[
 \mathcal T_\tau f(U)=
 \frac{\int_D d\gamma_{M(U)}(A)\,
       e^{V_\tau(U,A)}f(\mathcal U(U,\tau A))}
      {\int_D d\gamma_{M(U)}(A)\,
       e^{V_\tau(U,A)}}.
 \tag{CV22}
\]

Here \(D\) is the actual symmetric product cutoff, kept fixed while \(\tau\) varies; \(V_0=0\); \(\mathcal U(U,0)=\mathcal U_0(U)\); and
\(\partial_\tau\mathcal U(U,\tau A)|_0\) is linear in \(A\). The actual map is \(\mathcal T_g\). This is the kind of auxiliary fluctuation-amplitude interpolation used in CMP **119**, (3.30), and not a derivative of the family of physical coupling-dependent transport kernels.

At \(\tau=0\), the insertion is independent of \(A\). Differentiating the normalized ratio gives

\[
 \begin{aligned}
 \left.\partial_\tau\mathcal T_\tau f(U)\right|_0
 &=\mathbb E_{\gamma_M(\cdot\mid D)}
   \left[Df(\mathcal U_0(U))\,
       \left.\partial_\tau\mathcal U(U,\tau A)\right|_0\right]\\
 &\quad+\operatorname{Cov}_{\gamma_M(\cdot\mid D)}
    \bigl(f(\mathcal U_0(U)),\partial_\tau V_0(U,A)\bigr)
 =0.
 \end{aligned}
 \tag{CV23}
\]

The covariance term vanishes because its first argument is constant in \(A\). The expectation vanishes because the remaining integrand is odd and the centered truncated Gaussian is even. This identity includes the normalization exactly.

Consequently, if one proves the localized operator estimate

\[
 \sup_{|\tau|\le g}
 \|\partial_\tau^2\mathcal T_\tau f\|_{\rm anchored}
 \le C\|f\|_{\rm input},
 \tag{CV24}
\]

then the fundamental theorem of calculus gives

\[
 \|\mathcal T_gf-\mathcal T_0f\|_{\rm anchored}
 \le\tfrac12Cg^2\|f\|_{\rm input}.
 \tag{CV25}
\]

If the classical map \(\mathcal T_0\) preserves the dimension filtration, so that an irrelevant remainder has no projected marginal jet after that map, (CV25) implies \(\|B_k\|\le Cg_k^2\). On the marginal space, an identity classical jet implies \(A_k=I+O(g_k^2)\). The classical map can still create a bounded irrelevant remainder, which is why \(C_k=O(1)\) is allowed.

The uniformity in (CV24) is a real estimate still to prove for the chosen source class. A cutoff-supremum bound alone produces powers of \(r(g)\) and can change the cocycle growth. The useful route is to retain the finite polynomial powers of \(A\) arising from two amplitude derivatives, integrate them using localized Gaussian moments, and use connected rooted cluster bounds for the score terms. Normalization removes disconnected extensive contributions. This estimate must include analytic localization in the background and all admitted history/boundary interfaces; the source-free scalar beta function does not replace it.

### 5. What this changes in the proof plan

The marked induction need not prove a summable scalar multiplier before renormalizing the observable. For the deterministic bulk map, it suffices to prove (CV2), a bounded microscopic seed graph, and the admitted trajectory. The actual finite source family can then be normalized at a terminal physical scale, with the physical-scale bound (CV15). The two-root KP estimate can use those norms. Applying the same normalization to all carriers additionally requires control of their deviations from the bulk map; the large-field module is designed to add those summable perturbations, rather than to introduce a separate history-dependent normalization.

The remaining substantive targets are now concrete: the localized second amplitude-derivative estimate (CV24), classical preservation of the chosen marginal/irrelevant filtration, a contraction \(\|D_k\|<1\) after the point-root gauge Taylor subtraction, and compatibility of these estimates with the actual R and boundary terms. No claim that these hypotheses are already established is made here.

---
