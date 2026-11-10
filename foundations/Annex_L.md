# Phasewise ultraviolet coefficients from vacuum block estimates

**Annex L.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

This note proves a phase-transfer theorem that uses only vacuum norms of local positive-time blocks and their scale derivatives, once a valid field/phase disintegration exists. For two- and three-field ultraviolet coefficients, its inputs are mixed-vacuum four- and six-field distributions. It does not require an operator-norm OPE bound to transfer those coefficients.

The implication is P. Its application to the interacting Wilson limit remains C: neither the required four/six-field ultraviolet block estimates nor the decomposition hypotheses have been established for that limit here. In particular, this result does not prove the requested field energy bound or construct the continuum hierarchy.

The distinction from a two- or three-point calculation is exact. Knowing the mixed-state mean of a candidate coefficient identifies its average. The additional reflected block norm controls its dispersion across components. That second piece is what rules out different ultraviolet coefficients in different phases.

### 1. The actual positive-time block and its vacuum norm

Assume an OS hierarchy has already been constructed and reconstructed. Let \(\mathcal A_+\) be its polynomial positive-time test algebra. The coefficient tests are joint coincidence-flat kernels, with the component reflection/adjoint convention fixed once.

For \(F\in\mathcal A_+\), denote the corresponding reconstructed vacuum vector by
\[
\Psi(F)=[F],\qquad
\langle\Psi(F),\Psi(G)\rangle=S(\Theta F\otimes G).
\tag{1.1}
\]
No operator closure or energy estimate is needed to define these vectors. A degree-\(q\) joint kernel is a single element of the algebra; it need not be a tensor product.

Fix \(q=2\) or \(q=3\), a compact set \(K\) of relative \(q\)-point configurations away from all coincidence diagonals, and a physical center \(x_*\) strictly in positive time. For sufficiently small \(\rho>0\), the configurations \(x_*+\rho K\) remain strictly in positive time. Let \(A_\rho(F)\in\mathcal A_+\), for \(F\in C_c^\infty(K)\), be the specified rescaled \(q\)-field block, including the normalization required by the desired AF coefficient. The source order is \(q\), although lower-order terms can be included if prescribed centering requires them.

Let \(c_q(F)\) be the proposed limiting coefficient, a continuous linear functional of the relative test. Set
\[
B_\rho(F)=A_\rho(F)-c_q(F)1.
\tag{1.2}
\]
The exact norm identity is
\[
\begin{aligned}
\|\Psi(B_\rho(F))\|^2
={}&S(\Theta A_\rho(F)\otimes A_\rho(F))\\
&-2\operatorname{Re}\!\left[
\overline{c_q(F)}S(A_\rho(F))\right]+|c_q(F)|^2.
\end{aligned}
\tag{1.3}
\]

For a homogeneous block of degree \(q\), this uses \(S_q\) and \(S_{2q}\). The reflection keeps the two shrinking clusters a fixed physical distance apart. Internal points within either cluster remain separated by order \(\rho\). All tests in (1.3) remain in the corrected coincidence-flat test space.

Consequently a uniform cutoff estimate for the right side, before the continuum limit and with the same field normalization, passes to the reconstructed norm at each fixed \(\rho\). It must be an estimate for the full hierarchy. A connected \(2q\)-point function alone is not the right-hand side of (1.3).

### 2. A precise phase-disintegration input

Assume a valid decomposition of the reconstructed field system:
\[
\mathcal H=\int^\oplus \mathcal H_\omega\,d\nu(\omega),
\qquad
\Omega=\int^\oplus\Omega_\omega\,d\nu(\omega),
\qquad
\|\Omega_\omega\|=1
\quad\text{a.e.}
\tag{2.1}
\]
Assume the polynomial vacuum vectors disintegrate consistently:
\[
\Psi(F)=\int^\oplus\Psi_\omega(F)\,d\nu(\omega),
\quad
S_\omega(F)=\langle\Omega_\omega,\Psi_\omega(F)\rangle.
\tag{2.2}
\]
The phase fields and their vacuum distributions must have the continuity and common-core properties supplied by the chosen valid decomposition theorem. These are hypotheses, not consequences of merely writing a direct integral.

The elementary estimate is
\[
\boxed{
\int|S_\omega(A_\rho(F))-c_q(F)|^2\,d\nu(\omega)
\le\|\Psi(B_\rho(F))\|^2.
}
\tag{2.3}
\]

**Proof.** In each fiber, apply Cauchy--Schwarz to
\(\langle\Omega_\omega,\Psi_\omega(B_\rho(F))\rangle\), using the normalization in (2.1). Integrate the squared inequality and use the direct-integral norm identity. \(\square\)

This is a variance estimate across phases. It uses the full reflected block norm and retains the one-field identity terms in the definition of the block.

### 3. Phase transfer on a countable ultraviolet sequence

#### Theorem 3.1 — phase coefficient from a summable vacuum error, P

For one fixed block profile \(F\), suppose \(\rho_n\downarrow0\) and
\[
\sum_n\|\Psi(B_{\rho_n}(F))\|^2<\infty.
\tag{3.1}
\]
Then
\[
S_\omega(A_{\rho_n}(F))\longrightarrow c_q(F)
\quad\text{for a.e. }\omega.
\tag{3.2}
\]
The conclusion holds simultaneously for any countable family of profiles, field labels and coefficients for which (3.1) holds.

**Proof.** Sum (2.3) and apply Tonelli:
\[
\int\sum_n|S_\omega(A_{\rho_n}(F))-c_q(F)|^2\,d\nu(\omega)<\infty.
\]
The nonnegative series is therefore finite for almost every \(\omega\), and its terms tend to zero. Intersect the resulting countably many full-measure sets. \(\square\)

An error \(C\rho^\alpha[1+|\log\rho|]^b\), with \(\alpha>0\), is summable on every fixed geometric sequence. This conclusion is stronger than finding one phase with a nonzero coefficient: the prescribed value transfers to almost every phase in the decomposition.

Without quantitative summability, (2.3) gives convergence in \(L^2(d\nu)\), and a subsequence gives almost-everywhere convergence. It does not automatically give pointwise convergence along every prescribed sequence.

### 4. The continuous short-distance limit for all compact profiles

The countable result can be strengthened without assuming a phasewise ultraviolet bound in advance.

Put \(t=-\log\rho\) and \(B_t=B_{e^{-t}}\). Fix one compact relative configuration set \(K\), with an open neighborhood disjoint from the coincidence diagonals. Let \(\|\cdot\|_r\) denote the maximum of derivatives through order \(r\) on a fixed surrounding box. Tensor labels range over a fixed finite set.

Assume \(t\mapsto A_t(F)\) is continuously differentiable in the positive-time test-algebra topology for every profile, and the phase distributions in (2.2) are continuous on that algebra. Suppose, for some fixed \(r\),
\[
\|\Psi(B_t(F))\|\le e_0(t)\|F\|_r,
\qquad
\|\partial_t\Psi(B_t(F))\|\le e_1(t)\|F\|_r,
\tag{4.1}
\]
where
\[
\int_{t_0}^{\infty}\bigl[e_0(t)^2+e_1(t)^2\bigr]dt<\infty.
\tag{4.2}
\]
Scale-dependent AF powers and logarithms are part of \(A_t\), so their derivatives must be retained in the second inequality.

#### Theorem 4.1 — distributional phase transfer for every short-distance scale, P

Under (2.1)--(2.2) and (4.1)--(4.2), there is a Sobolev order \(s\), depending only on \(r\) and the finite profile dimension, such that for almost every phase
\[
\boxed{
\sup_{\substack{F\in C_c^\infty(K)\\\|F\|_{H^s}\le1}}
|S_\omega(A_\rho(F))-c_q(F)|
\longrightarrow0
\quad(\rho\downarrow0).
}
\tag{4.3}
\]
Thus the limiting coefficient holds as a distribution on the off-diagonal relative configuration space. One common full-measure set works for \(q=2,3\), the finite field family and a countable compact exhaustion.

**Proof.** The profile dimension is \(d=4q\). Embed the surrounding box into a fixed flat torus and extend the compact profiles by zero. Sobolev embedding supplies an integer \(\ell>r+d/2\) and a constant \(C_K\) with
\[
\|F\|_r\le C_K\|F\|_{H^\ell}.
\tag{4.4}
\]
Write \(E_v=\overline{C_c^\infty(K)}^{\,H^v}\) inside this torus. For an integer \(u>d/2\), the inclusion
\[
J:E_{\ell+u}\longrightarrow E_\ell
\tag{4.5}
\]
is Hilbert--Schmidt: the ambient torus inclusion has squared Hilbert--Schmidt norm a fixed multiple of
\(\sum_{n\in\mathbb Z^d}(1+|n|^2)^{-u}<\infty\).
Restricting its domain and codomain to these supported-profile closures does not increase this norm. Take \(s=\ell+u\).

Define
\[
(T_tF)(\omega)=S_\omega(A_t(F))-c_q(F).
\]
By (2.3), (4.1) and (4.4), \(T_t\) and its weak \(t\)-derivative extend from the profile space to bounded maps \(E_\ell\to L^2(d\nu)\), with norms at most \(C_Ke_0(t)\) and \(C_Ke_1(t)\). Composing with (4.5) gives Hilbert--Schmidt maps.

Choose an orthonormal basis \((f_j)\) of \(E_s\). Their coefficient functions define a random dual vector \(b_\omega(t)\in E_s^*\), with
\[
\int\|b_\omega(t)\|_{E_s^*}^2\,d\nu(\omega)
\le C_K e_0(t)^2,
\]
\[
\int\|\partial_tb_\omega(t)\|_{E_s^*}^2\,d\nu(\omega)
\le C_K e_1(t)^2.
\tag{4.6}
\]
These statements follow by summing the squared coefficient norms and using the Hilbert--Schmidt bound. They also construct consistent measurable versions. On each bounded time interval, integrating the derivative estimate shows that \(T_tJ\) has an \(H^1\) representative with values in the Hilbert--Schmidt maps \(E_s\to L^2(d\nu)\). Its continuous representative equals the pointwise-defined \(T_tJ\) at every \(t\); this follows first on smooth profiles from test-algebra continuity and then by the common norm bound. Evaluation at a fixed time consequently agrees in \(L^2(d\nu)\) with the Fubini \(H^1\) representative.

To identify the phasewise continuous representatives with the original phase evaluations, first use rational \(t\) and a countable set dense in the \(C_K^\infty\) topology, discarding one null set. The assumed continuity of \(t\mapsto A_t(F)\), the phase distributions and the \(H^1\) representatives gives equality for every \(t\) on this set. Approximation in \(C_K^\infty\), which also implies convergence in \(E_s\), then gives equality for every smooth profile. The construction therefore controls the actual phase distributions, rather than only unrelated almost-everywhere versions at each separate scale.

For a Hilbert-space-valued \(H^1\) function on a unit interval \(I_n=[n,n+1]\),
\[
\sup_{t\in I_n}\|b(t)\|^2
\le C\int_{I_n}\bigl(\|b(t)\|^2+\|b'(t)\|^2\bigr)dt.
\tag{4.7}
\]
For example, choose a point whose norm is no larger than the interval \(L^2\) norm, apply the fundamental theorem of calculus, and then Cauchy--Schwarz. Fubini and (4.6) show that the phase curves have the required \(H^1\) representatives almost surely.

Integrating (4.7), summing over \(n\), and using (4.2) gives
\[
\int\sum_n\sup_{t\in I_n}\|b_\omega(t)\|^2\,d\nu(\omega)<\infty.
\]
The suprema therefore tend to zero for almost every \(\omega\). This is (4.3). Countable intersections over compact sets and the finite labels prove the final assertion. \(\square\)

The test-space step is explicit. It does not identify a bound only on tensor-product tests with a bound on arbitrary joint kernels. The norm premises (4.1) are themselves for all joint profiles.

### 5. Connected two- and three-point coefficients

For a translation-invariant phase, the one-point distribution of a scalar field is a constant. Restrict first to block profiles satisfying \(\int F(u_1,\ldots,u_q)\,du_i=0\) as a function of all remaining variables, for each \(i\). Vanishing of the total integral alone is not this condition. Then every one-point contribution vanishes in every phase.

For \(q=2,3\), the full block expectation on these profiles equals its connected version. Theorems 3.1 and 4.1 therefore transfer the prescribed connected coefficients, including a specified nonzero three-point value, once their vacuum block premises hold. More general profiles can be treated only after the relevant lower-order phase terms and normalization have been controlled.

This avoids the incorrect inference that an averaged nonzero three-point coefficient by itself gives the prescribed coefficient in a selected phase. The reflected four/six-field estimates supply the missing phase dispersion control.

If the decomposition theorem and the energy/covariance argument already provide their required properties on a full-measure set, intersect that set with the one supplied by Theorem 4.1. Every phase in the intersection retains both the prescribed coefficients and those properties. The present theorem does not create that energy/covariance set.

### 6. A Gaussian benchmark with the correct two-block geometry

The vacuum norm premise is natural in the frozen Gaussian test, but it remains an interacting obligation.

Consider a reflection-positive, stationary Gaussian curvature field whose off-diagonal covariance \(C_{\alpha\beta}(x-y)\) is homogeneous of degree \(-4\), with
\[
|C_{\alpha\beta}(x-y)|\le C|x-y|^{-4}.
\tag{6.1}
\]
Take quadratic Wick fields \(O\) of dimension four. Their Schwinger functions on separated supports are defined by Wick contraction, with the stated tensor reflection convention. One need not claim that every Euclidean composite extends as an ordinary random distribution across its self-coincidence diagonals.

For \(q=2\) or \(q=3\), define
\[
A_\rho(F)=\rho^{4q}
\int F(u_1,\ldots,u_q)
O(x_*+\rho u_1)\cdots O(x_*+\rho u_q)\,du.
\tag{6.2}
\]
The profiles are supported in the fixed compact \(K\) away from internal coincidences. Gaussian homogeneity makes the vacuum coefficient \(c_q(F)=S(A_\rho(F))\) independent of \(\rho\).

#### Proposition 6.1 — Gaussian block-norm remainder, P

For sufficiently small \(\rho\),
\[
\|\Psi(A_\rho(F)-c_q(F))\|^2
\le C_{K,q,x_*}\rho^8\|F\|_0^2.
\tag{6.3}
\]
Its logarithmic scale derivative has the same power, with a fixed first-derivative profile norm.

**Proof.** In the reflected \(2q\)-field moment there are \(4q\) Gaussian legs and \(2q\) contraction edges. The two blocks are separated by a fixed physical time gap. The diagrams with no edge between blocks give exactly \(|c_q(F)|^2\), and cancel in (1.3).

Every remaining diagram has an even number \(r\ge2\) of cross-block edges: each block has \(2q\) legs, and internal contractions consume an even number of them. Cross-block kernels are uniformly bounded by the fixed gap. Each of the other \(2q-r\) edges costs at most \(C\rho^{-4}\). The two block normalizations contribute \(\rho^{8q}\), leaving
\[
\rho^{8q}\rho^{-4(2q-r)}
=\rho^{4r}\le C\rho^8
\quad(0<\rho\le1).
\]
There are finitely many diagrams for \(q=2,3\), and the compact profile integrals are bounded by a fixed multiple of \(\|F\|_0^2\).

For the scale derivative, the smeared block in (6.2) is equivalently the degree-\(q\) field evaluated on \(F((x_i-x_*)/\rho)\). With \(t=-\log\rho\), differentiation replaces \(F\) by \(\mathcal DF=\sum_i u_i\cdot\nabla_{u_i}F\). Homogeneity gives \(c_q(\mathcal DF)=0\). The same contraction count, with the fixed derivative profile norm, proves the derivative claim. \(\square\)

Thus \(e_0(t),e_1(t)\) can be taken proportional to \(e^{-4t}\) in this Gaussian benchmark. Fixed logarithmic losses remain integrable in (4.2). The calculation does not determine the interacting scalar three-point coefficient: in channels where the Gaussian coefficient vanishes, the required higher perturbative coefficient still has to be established with its uniform remainder.

### 7. Why this is weaker than an operator-norm OPE estimate

Let a central real Gaussian variable \(A\) act by multiplication on \(L^2\) of its law, with vacuum \(1\). The block \(B_\rho=\rho A\) obeys
\[
\|B_\rho\Omega\|=\rho,
\qquad
\|B_\rho\|=\infty
\quad(\rho>0).
\]
Disintegration over \(A=a\) gives \(B_{\rho,a}=\rho a\to0\) in every finite-\(a\) component.

This example shows that a vacuum block estimate can transfer a coefficient even when a global operator-norm bound is false. It is not a Yang--Mills model. It also explains why the present improvement cannot supply P1's separate field energy requirement.

### 8. Exact remaining Yang--Mills input

The sufficient UV-transfer estimate still to be proved is the following: on the actual normalized cutoff hierarchy and uniformly before taking the cutoff/volume limit, the two-block full-moment bounds corresponding to (4.1), for \(q=2,3\), including the logarithmic scale derivative and the actual field/coupling normalization.

The means alone are J4's usual two/three-point coefficient calculations. The norm remainders add reflected four/six-point information with a fixed macroscopic separation between the shrinking blocks. This is an observable statement; it is not an arbitrary-vector operator theorem.

No complete Wilson estimate of this strength is proved in this note. The Gaussian benchmark verifies the mechanism in its stated model, and the phase theorem shows exactly how the interacting estimate would transfer the coefficients. The independent decomposition, rotation/covariance and energy requirements remain explicit.

### Source scope

The OS positive-time vector and reconstruction setup is the one retained from Osterwalder--Schrader II, CMP 42 (1975), 281--305, with the corrected flat test space. The disintegration is conditional on the hypotheses of the chosen field decomposition theorem, such as Driessler--Summers, Helv. Phys. Acta 59 (1986), 331--348. No extra decomposition theorem is imported from vacuum moments.

The phase \(L^2\) inequality, countable and continuous-profile transfer theorems, Sobolev/Hilbert--Schmidt argument, Gaussian block calculation and central example are proved above. They are not quotations of an interacting Yang--Mills result.


---
