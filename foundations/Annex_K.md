# Gaussian product-cutoff removal and low-order Wick comparison

**Annex K.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Main result and its scope

The Gaussian cutoff-removal lemma below is **proved**. It compares a centered, uniformly massive finite-dimensional Gaussian with its conditioning on a product of symmetric Euclidean balls. The error for every fixed polynomial moment and cumulant is bounded by a polynomial in the cutoff radius times \(\exp(-cP^2)\), uniformly in the number of blocks.

The proof uses the explicit full Gaussian Ornstein–Uhlenbeck semigroup and a divergence identity on the product domain. It does not assume existence, stationarity or regularity of a reflected stochastic process. No estimate of the probability that *all* Gaussian coordinates satisfy the cutoff is used.

The result also covers polynomials whose coefficient kernels have a uniform absolute-sum norm, including exponentially localized polynomial observables with noncompact spatial support. A separate, precisely stated tree-bound input permits summation over a fixed number of extensive anchors. The pointwise error by itself is not summed over the whole volume.

This theorem removes a cutoff from a **Gaussian reference law**. It does not remove the regular-window cutoff from the interacting native law or prove the complete-history C0 estimate.

### 2. Assumptions and notation

Let \(I\) be any finite block set and

\[
\mathcal X_I=\bigoplus_{i\in I}\mathbb R^{d_i},
\qquad 1\leq d_i\leq d_*.
\tag{2.1}
\]

Let \(H\) be a real symmetric matrix on this space. Assume

\[
H\geq\lambda I,\qquad H_{ii}\leq\Lambda I_{d_i},
\qquad \lambda>0,\quad \Lambda<\infty,
\tag{2.2}
\]

with constants independent of the volume. Write

\[
A_H:=
\sup_{i\in I}\sum_{j\in I}
\int_0^\infty\|(e^{-tH})_{ij}\|_{\mathrm{op}}\,dt
\leq A<\infty.
\tag{2.3}
\]

Condition (2.3) is the exact semigroup locality assumption needed below. A sufficient stronger condition is

\[
\sup_i\sum_j e^{\mu d(i,j)}
\|(e^{-tH})_{ij}\|_{\mathrm{op}}
\leq C e^{-\lambda_1t},
\tag{2.4}
\]

which gives \(A\leq C/\lambda_1\). The spectral gap and the diagonal-block bound alone are not silently substituted for (2.3).

Define

\[
\nu_\infty(dz)=Z_\infty^{-1}
e^{-\frac12z^THz}\,dz,
\qquad
K_P=\prod_{i\in I}\overline B_{d_i}(0,P),
\qquad
\nu_P=\nu_\infty(\,\cdot\mid K_P),
\quad P\geq1.
\tag{2.5}
\]

Thus \(Z_P=\int_{K_P}\exp(-z^THz/2)\,dz\) is the unnormalized constrained integral. Matrix inequalities in (2.2) use the quadratic-form order.

The boundary of each factor is a sphere, including the two endpoints when \(d_i=1\). The products of two or more factor boundaries have zero surface measure in the full boundary of \(K_P\). The usual divergence theorem applies face by face, or directly to this bounded convex Lipschitz domain.

For a bounded Lipschitz function \(f\), set

\[
\operatorname{Lip}_i(f)
=\mathop{\mathrm{ess\,sup}}_z|\nabla_i f(z)|.
\tag{2.6}
\]

All constants below depend only on the displayed structural parameters and the indicated fixed polynomial degrees or cumulant orders.

### 3. A one-block marginal has a uniform boundary density

#### Lemma 3.1 — effective-potential sandwich

Fix \(i\), write \(z=(x,w)\) with \(x=z_i\), and integrate over the other constrained blocks:

\[
e^{-v_i(x)}
:=
\int_{\prod_{j\ne i} B_{d_j}(0,P)}
\exp\left[-\frac12(x,w)^TH(x,w)\right]dw.
\tag{3.1}
\]

Then \(v_i\) is a smooth even function on \(\mathbb R^{d_i}\), and

\[
\lambda I\leq v_i''(x)\leq H_{ii}\leq\Lambda I.
\tag{3.2}
\]

Consequently,

\[
\frac{\lambda}{2}|x|^2
\leq v_i(x)-v_i(0)
\leq\frac{\Lambda}{2}|x|^2.
\tag{3.3}
\]

**Proof.** The integration domain in (3.1) is compact and independent of \(x\), so differentiation is justified to every finite order. Evenness follows by replacing \(w\) by \(-w\). Differentiating twice gives

\[
v_i''(x)
=H_{ii}-H_{i,-i}
\operatorname{Cov}_{x,P}(w)
H_{-i,i}
\leq H_{ii}.
\tag{3.4}
\]

For the lower bound, the function

\[
\frac12(x,w)^TH(x,w)-\frac{\lambda}{2}|x|^2
\tag{3.5}
\]

is convex: its Hessian is
\(H-\lambda\operatorname{diag}(I_{d_i},0)\geq0\).
Its exponential with negative sign is log-concave. Integrating over the convex set of the other blocks preserves log-concavity by Prékopa's marginal theorem. Therefore \(v_i(x)-\lambda|x|^2/2\) is convex, proving the lower bound in (3.2). Evenness gives \(v_i'(0)=0\), and integration along the segment from \(0\) to \(x\) gives (3.3). \(\square\)

The sole non-elementary convexity import here is Prékopa's marginal theorem: Theorem 6, printed p.342, in *On logarithmic concave measures and functions*, Acta Sci. Math. 34 (1973), 335–343. A copy of the paper is available at
<https://rutcor.rutgers.edu/Prekopa/pdf/SCIENT2.pdf>.

#### Corollary 3.2 — boundary flux and block moments

The \(i\)-block marginal density of \(\nu_P\), with its continuous boundary value, satisfies

\[
p_{i,P}(x)\leq C_{\lambda,\Lambda,d_*}
e^{-\lambda|x|^2/2}
\quad (|x|\leq P).
\tag{3.6}
\]

In particular the normalized boundary flux of face \(i\) obeys

\[
b_i(P):=
\frac1{Z_P}\int_{\substack{|z_i|=P\\z_{-i}\in K_{P,-i}}}
e^{-\frac12z^THz}\,d\sigma_i(z_i)\,dz_{-i}
\leq C P^{d_*-1}e^{-\lambda P^2/2}.
\tag{3.7}
\]

Every fixed block moment under \(\nu_P\) is bounded uniformly in the volume and \(P\geq1\).

**Proof.** The denominator of the marginal is at least

\[
e^{-v_i(0)}
\int_{|x|\leq1}e^{-\Lambda|x|^2/2}\,dx.
\tag{3.8}
\]

The minimum of the last positive integral over \(1\leq d_i\leq d_*\) depends only on \(\Lambda,d_*\). Apply the lower bound in (3.3) to the numerator. Integrating (3.6) on the sphere gives (3.7), and integrating it against \(|x|^r\) gives the moment assertion. \(\square\)

This is where the potentially tiny global normalization \(Z_P/Z_\infty\) is handled. It is absorbed in the single-block marginal; it never becomes a volume-dependent inverse probability in the final bound.

### 4. Local Lipschitz comparison through the full Gaussian semigroup

#### Theorem 4.1 — volume-uniform Lipschitz estimate

Under (2.1)–(2.3), for every bounded Lipschitz \(f\),

\[
|\nu_P(f)-\nu_\infty(f)|
\leq C A
P^{d_*-1}e^{-\lambda P^2/2}
\sum_{i\in I}\operatorname{Lip}_i(f).
\tag{4.1}
\]

The estimate is useful when the sum of block Lipschitz constants is bounded independently of the volume, as it is for fixed local observables and the clipped polynomials considered below.

**Proof.** First take smooth \(f\) with bounded derivatives. The full Gaussian generator and semigroup are

\[
\mathcal L=\Delta-(Hz)\cdot\nabla,
\qquad
\mathsf P_t f(z)
=\mathbb E f(e^{-tH}z+\xi_t),
\tag{4.2}
\]

where \(\xi_t\) is centered Gaussian with covariance
\(H^{-1}(I-e^{-2tH})\). For \(T>0\), let

\[
u_T(z)=\int_0^T
[\mathsf P_t f(z)-\nu_\infty(f)]\,dt.
\tag{4.3}
\]

Then

\[
\mathcal L u_T=\mathsf P_Tf-f.
\tag{4.4}
\]

Writing \(V(z)=z^THz/2\), the divergence identity
\[
e^{-V}\mathcal L u_T
=\operatorname{div}(e^{-V}\nabla u_T)
\]
and the divergence theorem on \(K_P\) give

\[
\nu_P(\mathsf P_Tf-f)
=\frac1{Z_P}
\sum_j\int_{\partial_jK_P}
\partial_{n_j}u_T\,e^{-V}\,d\sigma.
\tag{4.5}
\]

No boundary condition for \(u_T\) is imposed. This is an identity for the **full-space** OU solution restricted to the product domain.

Differentiating the explicit semigroup yields

\[
|\nabla_j\mathsf P_t f(z)|
\leq\sum_i
\|(e^{-tH})_{ij}\|_{\mathrm{op}}
\operatorname{Lip}_i(f).
\tag{4.6}
\]

Hence the absolute value of the right side of (4.5) is at most

\[
\sum_i\operatorname{Lip}_i(f)
\sum_j b_j(P)
\int_0^T\|(e^{-tH})_{ij}\|_{\mathrm{op}}dt
\leq CA P^{d_*-1}e^{-\lambda P^2/2}
\sum_i\operatorname{Lip}_i(f).
\tag{4.7}
\]

For each fixed finite volume, the gap implies
\(\mathsf P_Tf\to\nu_\infty(f)\) uniformly on the compact set \(K_P\). Let \(T\to\infty\) in (4.5). The bound in (4.7) is already independent of the volume and \(T\), giving (4.1).

For bounded Lipschitz \(f\), convolve with smooth approximate identities. The block Lipschitz bounds do not increase, and the functions converge uniformly. Pass to the limit in (4.1). \(\square\)

The proof justifies all boundary contributions directly. Intersections of faces contribute no surface term; no boundary local-time law or invariant coupling is being assumed.

### 5. Polynomial moments, including absolutely summable kernels

Fix an orthonormal basis in every block and let \(a=(i,\alpha)\) denote a scalar coordinate. Write a polynomial of degree at most \(D\) as

\[
Q(z)=\sum_{d=0}^{D}
\sum_{a_1,\ldots,a_d}
c^{(d)}_{a_1\cdots a_d}
z_{a_1}\cdots z_{a_d},
\qquad
\|Q\|_1:=\sum_{d=0}^{D}
\sum_{a_1,\ldots,a_d}|c^{(d)}_{a_1\cdots a_d}|.
\tag{5.1}
\]

The given coefficient representation is used; no minimization over representations is required. Products satisfy
\(\|Q_1Q_2\|_1\leq\|Q_1\|_1\|Q_2\|_1\).
An exponentially localized coefficient kernel with a uniform absolute-sum bound is admissible even when its support grows with the volume.

#### Theorem 5.1 — polynomial cutoff removal

For each fixed \(D\), there is \(C_D\), independent of the volume and \(P\geq1\), such that

\[
|\nu_P(Q)-\nu_\infty(Q)|
\leq C_D\|Q\|_1
(1+P)^{D+d_*}e^{-\lambda P^2/8}.
\tag{5.2}
\]

**Proof.** Let \(\pi_P\) be blockwise radial projection onto the radius-\(P\) ball and put \(Q_P=Q\circ\pi_P\). Projection is 1-Lipschitz on each block, \(Q_P\) is bounded Lipschitz, and \(Q_P=Q\) on \(K_P\). At differentiability points,

\[
\sum_i\operatorname{Lip}_i(Q_P)
\leq D\|Q\|_1(1+P)^{D-1}.
\tag{5.3}
\]

To verify (5.3), differentiate a monomial. Each occurrence of a coordinate contributes at most \((1+P)^{d-1}\), and summing its multiplicities over the blocks gives \(d\leq D\). Apply Theorem 4.1:

\[
|\nu_P(Q)-\nu_\infty(Q_P)|
\leq C A D\|Q\|_1
(1+P)^{D+d_*-2}e^{-\lambda P^2/2}.
\tag{5.4}
\]

It remains to compare \(Q\) and \(Q_P\) under the full Gaussian. For a monomial of degree \(d\), telescope its product after projection. Each term is bounded by

\[
\prod_{\ell=1}^{d}|z_{a_\ell}|\,
\mathbf1_{\{|z_{i_r}|>P\}}
\tag{5.5}
\]

for one of its \(d\) coordinate occurrences, since radial projection decreases the absolute value of each scalar coordinate.

The covariance of every Gaussian block is bounded by \(\lambda^{-1}I\), so

\[
\mathbb P_{\nu_\infty}(|z_i|>P)
\leq 2^{d_*/2}e^{-\lambda P^2/4}.
\tag{5.6}
\]

This follows by applying Markov's inequality to
\(\exp(\lambda|z_i|^2/4)\).
By Hölder, the \(L^2\) norm of the product in (5.5) is bounded by a constant depending only on \(d,\lambda\), including when indices coincide. Cauchy–Schwarz and (5.6) therefore give

\[
\nu_\infty|Q-Q_P|
\leq C_D\|Q\|_1e^{-\lambda P^2/8}.
\tag{5.7}
\]

Combine (5.4) and (5.7), enlarging the harmless polynomial prefactor to obtain (5.2). The constant polynomial case is exact. \(\square\)

The estimate retains the actual coefficient norm. For an observable carrying a physical factor \(h^{-4}\), that factor is not discarded; it must be included in \(\|Q\|_1\) or removed by the chosen physical normalization.

#### 5.1 Other fixed symmetric norm balls

The same proof applies to products \(K_P=\prod_i P C_i\) of centrally symmetric convex block bodies when, uniformly in the block index,

\[
r_-B_{d_i}\subset C_i\subset r_+B_{d_i},
\qquad
\mathcal H^{d_i-1}(\partial C_i)\leq S_*,
\quad r_->0.
\tag{5.8}
\]

These are explicit fixed-template assumptions; no nonsymmetric or shifting cutoff is included. The effective potential remains even. Its denominator is bounded using the ball of radius \(r_-\), every boundary point has norm at least \(r_-P\), and the boundary area scales as \(P^{d_i-1}\). Use Euclidean nearest-point projection onto \(PC_i\), which is 1-Lipschitz and satisfies \(|\pi_{PC_i}z_i|\leq|z_i|\). In the polynomial tail estimate, replace scalar-coordinate products by the corresponding block-norm products, and use \(z_i\notin PC_i\Rightarrow |z_i|>r_-P\). All conclusions remain valid with changed constants and \(c=\lambda r_-^2/8\) in place of \(\lambda/8\).

This version covers a specified finite family of symmetric convex norm balls, provided the template constants in (5.8) are included in the application. It is not necessary to change the cutoff during the coupling interpolation.

### 6. Joint moments and cumulants of fixed order

#### Corollary 6.1

Let \(Q_1,\ldots,Q_m\) have degrees at most \(d_0\), and let
\(A_i=\|Q_i\|_1\). For every fixed \(m\), in particular \(m\leq6\),

\[
\left|
\nu_P\!\left(\prod_{i=1}^m Q_i\right)
-\nu_\infty\!\left(\prod_{i=1}^m Q_i\right)
\right|
\leq C_{m,d_0}
\left(\prod_iA_i\right)
(1+P)^{md_0+d_*}e^{-\lambda P^2/8},
\tag{6.1}
\]

and

\[
\left|
\kappa_{\nu_P}(Q_1,\ldots,Q_m)
-\kappa_{\nu_\infty}(Q_1,\ldots,Q_m)
\right|
\leq C_{m,d_0}
\left(\prod_iA_i\right)
(1+P)^{md_0+d_*}e^{-\lambda P^2/8}.
\tag{6.2}
\]

**Proof.** Apply Theorem 5.1 to the product polynomial. For cumulants use

\[
\kappa(Q_1,\ldots,Q_m)
=\sum_{\pi\in\Pi_m}
(|\pi|-1)!(-1)^{|\pi|-1}
\prod_{B\in\pi}
\nu\!\left(\prod_{i\in B}Q_i\right).
\tag{6.3}
\]

Every fixed joint moment under both laws is bounded by a constant times the product of the coefficient norms. Under \(\nu_P\), this follows from the block moment bound after (3.7) and Hölder; under \(\nu_\infty\), it follows from its covariance bound. Telescope the product over blocks of each partition in (6.3), apply (6.1) to the changed factor, and sum the finitely many partitions. \(\square\)

The constants are controlled at every fixed order. This corollary is not an all-orders OS-growth theorem. Both measures are even, so moments of odd total polynomial parity vanish exactly; no error bound is needed for those expressions.

### 7. Extensive anchors: interpolation with tree decay

The small bound in (6.2) is pointwise in the anchor positions. Summing it directly over all possible positions would introduce powers of the volume. The following separate implication is the correct way to use it.

#### Proposition 7.1 — anchored summation, with a tree-bound premise

Let \(Q_u^{(a)}\) be polynomial marks anchored at sites \(u\), with degrees and coefficient norms bounded uniformly in \(u\) and the volume. Let \(m\) be fixed. Suppose the cumulants of **both** laws obey

\[
\begin{split}
&|\kappa_{\nu_P}(Q_{u_1}^{(1)},\ldots,Q_{u_m}^{(m)})|
+|\kappa_{\nu_\infty}(Q_{u_1}^{(1)},\ldots,Q_{u_m}^{(m)})|\\
&\qquad\leq
B_m(1+P)^{b_m}
\sum_{T\in\mathcal T_m}
\prod_{\{a,b\}\in T}e^{-\mu d(u_a,u_b)},
\end{split}
\tag{7.1}
\]

with volume-uniform constants. Also suppose the anchor geometry satisfies

\[
S_\gamma:=\sup_u\sum_v e^{-\gamma d(u,v)}<\infty
\tag{7.2}
\]

uniformly in volume at the positive exponents used below.

Then, for any \(r\leq m-1\), summing the cutoff error over \(r\) anchor positions while retaining at least one fixed anchor gives

\[
\sum_{u_{m-r+1},\ldots,u_m}
|\Delta\kappa_m(u_1,\ldots,u_m)|
\leq
C_m(1+P)^{c_m}e^{-\lambda P^2/16}.
\tag{7.3}
\]

If the unsummed anchors are \(u_1,\ldots,u_{m-r}\), the bound can retain

\[
C_m(1+P)^{c_m}e^{-\lambda P^2/16}
e^{-\mu\tau(u_1,\ldots,u_{m-r})/8},
\tag{7.4}
\]

where \(\tau\) is minimum spanning-tree length in the metric \(d\).

**Proof.** Equation (6.2) gives
\[
|\Delta\kappa_m|\leq\varepsilon_m(P),
\qquad
\varepsilon_m(P)\leq
C_m(1+P)^{md_0+d_*}e^{-\lambda P^2/8}.
\]
There are at most \(m^{m-2}\) labeled trees for \(m\geq2\), and every tree has length at least \(\tau(u_1,\ldots,u_m)\). Thus (7.1) also gives
\[
|\Delta\kappa_m|
\leq C_m(1+P)^{b_m}e^{-\mu\tau(u_1,\ldots,u_m)}.
\]
Use \(\min(a,b)\leq\sqrt{ab}\) to obtain
\[
|\Delta\kappa_m|
\leq C_m(1+P)^{c_m}e^{-\lambda P^2/16}
e^{-\mu\tau(u_1,\ldots,u_m)/2}.
\tag{7.5}
\]

For any positive \(\gamma\),
\[
e^{-\gamma\tau(u_1,\ldots,u_m)}
\leq\sum_{T\in\mathcal T_m}
\prod_{\{a,b\}\in T}e^{-\gamma d(u_a,u_b)}.
\]
Root a tree at a fixed anchor and sum leaves successively. Summing all its other vertices costs at most \(S_\gamma^{m-1}\); summing fewer is bounded by the same full sum. This proves (7.3).

For (7.4), a doubled traversal of a tree on all anchors, followed by metric shortcuts, connects the unsummed anchors with length at most twice the original tree length. Hence
\[
\tau(u_1,\ldots,u_m)
\geq\tfrac12\tau(u_1,\ldots,u_{m-r}).
\]
Split the last exponential in (7.5) into two equal factors. Use the preceding inequality on one factor and the leaf summation at exponent \(\mu/4\) on the other. \(\square\)

The proposition applies at every fixed total order, whenever the corresponding two tree bounds are available. In the native second-coefficient application with at most six external fields, there are at most two extensive anchors and at most eight cumulant arguments. Four extensive anchors are also allowed at any fixed total order with at least one unsummed anchor. Bounded coefficients multiplying the anchor sums merely change \(C_m\).

**Scope of the premise.** Theorem 4.1 and Corollary 6.1 prove the cutoff error under (2.1)–(2.3). This note does not derive all higher truncated-Gaussian tree bounds merely from the full Gaussian semigroup estimate. To use (7.3) for extensive anchors, apply the separately established tree theorem for the specified product-cutoff Gaussian law and check that it supplies (7.1), with the same normalization. If it does not, (7.1) remains an explicit additional input.

### 8. Logarithmic cutoffs and small coupling

Let

\[
P(g)=a[\log(g^{-1})]^p,\qquad a>0,\quad p>\tfrac12.
\tag{8.1}
\]

For every fixed \(B,c,R>0\),

\[
P(g)^B e^{-cP(g)^2}=o(g^R)
\quad(g\downarrow0).
\tag{8.2}
\]

**Proof.** Put \(t=\log(g^{-1})\). The logarithm of the ratio to \(g^R\) is
\[
B\log a+Bp\log t-ca^2t^{2p}+Rt.
\]
Since \(2p>1\), this tends to \(-\infty\). \(\square\)

Thus the fixed-degree Gaussian moments, cumulants, and the anchor sums admitted by Section 7 can be replaced by their untruncated Gaussian counterparts with an error smaller than every fixed power of \(g\). If additional explicit fixed powers of \(g^{-1}\) occur in an observable's normalization, they can be included in this comparison. Uniformity is not claimed for an unbounded number of factors or for degrees growing with the cutoff.

### 9. Application conditions

| Question | Result |
|---|---|
| Is the small probability of the full product-cutoff event divided out naively? | No. Lemma 3.1 controls normalized one-block boundary densities directly. |
| Is reflection at intersecting ball boundaries assumed to be well behaved? | No reflected process is used; the proof applies a finite-dimensional divergence theorem on a convex Lipschitz product domain. |
| Is a stationary synchronous coupling required? | No. The explicit full Gaussian semigroup supplies the comparison identity. |
| Are noncompact but exponentially localized polynomial marks covered? | Yes, when their displayed coefficient absolute-sum norms are uniform. |
| Can a pointwise cumulant error be summed over four extensive anchors? | Only after applying Section 7 with the two volume-uniform tree bounds; direct summation is not valid. |
| Does this replace an identity-background truncated Gaussian coefficient by the ordinary Gaussian coefficient? | Yes, for a fixed finite combination of the covered polynomial cumulants, with the anchor proviso above. |
| Does it remove the cutoff from the interacting YM conditional law? | No; the comparison here is precisely \(\nu_P\) versus its own full Gaussian reference \(\nu_\infty\). |

**Final status.** The volume-uniform Gaussian product-cutoff removal theorem for fixed-order polynomial moments and cumulants is proved. Extensive-anchor removal is a proved implication with the explicit tree-bound premise (7.1), rather than an unqualified consequence of pointwise cutoff errors.


### Supplement to Annex K: low-order native Wick comparison


### Result and scope

The parity theorem and the Gaussian product-cutoff lemma combine into a volume-uniform expansion whose leading and second coefficients can be evaluated by ordinary finite-dimensional Gaussian Wick contraction. The result is proved for each source order \(1\le m\le6\), including all extra extensive vertices in the second coefficient.

The inherited action \(E_*\) remains frozen at its actual shell value. The Gaussian precision is the actual finite-volume constrained precision \(H\). This note makes no infinite-volume, continuum, universal-coefficient, or AF-identification claim. It removes the cutoff from the two Gaussian coefficients; the interacting native integral still has its specified regular-window cutoff.

The underlying results are Annex J and Annex K, Gaussian cutoff-removal theorem. The latter's boundary-flux proof has been independently checked: its effective-potential sandwich, full-space OU divergence identity, clipping estimate and fixed-order moment/cumulant telescoping are valid under its displayed hypotheses. Sections 1--3 below verify those hypotheses and the required anchored tree bounds for the present native Gaussian.

### 1. Gaussian semigroup locality follows from the actual precision bounds

Keep the identity-background homogeneous fixed-domain setup of the parity theorem. For this corollary, take the common cutoff to be the product of Euclidean coordinate-block balls

\[
\mathcal D_P=\prod_{i\in\mathcal I}\overline B_{d_i}(0,P),
\qquad P\ge1,\quad d_i\le d_*.
\tag{W.1}
\]

Scalar coordinate cubes are included by treating their scalar coordinates as one-dimensional blocks. The displayed constants below use these Euclidean factors. The fixed centrally symmetric convex block templates covered by Section 5.1 of the Gaussian cutoff theorem give the same conclusions, with constants depending on their stated inradius, outradius and surface-area bounds and with \(\lambda P^2/16\) replaced by \(\lambda r_-^2P^2/16\) in the Gaussian error. This extension keeps the actual chosen cutoff unchanged throughout the interpolation.

The two Gaussian laws are

\[
d\nu_P=Z_P^{-1}\mathbf1_{\mathcal D_P}
e^{-zHz/2}\,dz,\qquad
d\nu_\infty=Z_\infty^{-1}e^{-zHz/2}\,dz.
\tag{W.2}
\]

The actual precision has a volume-uniform gap and physical locality:

\[
H\ge\lambda I,\qquad
\|H_{ij}\|_{\mathrm{op}}\le C e^{-\mu_0d(i,j)}.
\tag{W.3}
\]

The gap is the retained constrained Gaussian input. The second estimate follows from the homogeneous physical second-derivative estimate for \(\mathcal A\), evaluated at zero. In particular \(H_{ii}\le\Lambda I\) for a fixed \(\Lambda\).

To verify the additional semigroup hypothesis in the cutoff lemma, define the block-diagonal weight

\[
(W_xv)_i=e^{a d(i,x)}v_i.
\]

Metric triangle inequalities and the exponential row/column sums in (W.3) imply

\[
\sup_x\|W_xHW_x^{-1}-H\|_{2\to2}
\le\rho(a),\qquad \rho(a)\longrightarrow0
\quad(a\downarrow0),
\tag{W.4}
\]

uniformly in volume. For example, the Schur estimate is bounded by a fixed multiple of
\(\sup_i\sum_j(e^{a d(i,j)}-1)e^{-\mu_0d(i,j)}\).
The four-dimensional current-lattice volume bound makes this expression tend to zero uniformly.

Choose \(a>0\) with \(\rho(a)\le\lambda/2\). The real part of
\(W_xHW_x^{-1}\) is then at least \(\lambda/2\), so its matrix semigroup obeys

\[
\|W_xe^{-tH}W_x^{-1}\|_{2\to2}
\le e^{-\lambda t/2}.
\tag{W.5}
\]

Taking \(x=i\), bounding the block from \(i\) to \(j\), and using symmetry of \(e^{-tH}\) gives

\[
\|(e^{-tH})_{ij}\|_{\mathrm{op}}
\le e^{-a d(i,j)}e^{-\lambda t/2}.
\tag{W.6}
\]

Consequently

\[
\sup_i\sum_j\int_0^\infty
\|(e^{-tH})_{ij}\|_{\mathrm{op}}\,dt
\le\frac2\lambda\sup_i\sum_j e^{-a d(i,j)}
<\infty,
\tag{W.7}
\]

uniformly in volume. Thus the cutoff lemma's semigroup assumption is supplied by the existing homogeneous precision estimate; it is not inferred from the gap alone.

### 2. A weighted polynomial coefficient norm

Fix orthonormal coordinates in every block, and write a scalar coordinate as \(b=(j,\alpha)\), with spatial block \(j(b)=j\). For a polynomial anchored at \(x\), choose a coefficient representation

\[
Q_x(z)=\sum_{d=0}^{D}
\sum_{b_1,\ldots,b_d}
c^{(d)}_{b_1\cdots b_d}
z_{b_1}\cdots z_{b_d}.
\tag{W.8}
\]

Define its weighted absolute-sum norm by

\[
\|Q_x\|_{\theta,1}
=\sum_{d=0}^{D}\sum_{b_1,\ldots,b_d}
|c^{(d)}_{b_1\cdots b_d}|
e^{\theta\tau(x,j(b_1),\ldots,j(b_d))}.
\tag{W.9}
\]

The degree-zero term has weight one. This is a norm on the chosen coefficient representation; no minimization over representations is needed. In particular it dominates the coefficient norm used in the Gaussian cutoff lemma.

Let

\[
O_{i,r}=\partial_g^rO_i(g,z)|_{g=0},
\quad r=0,1,2,
\]

and let
\[
W_r=\partial_g^rW_g(z)|_{g=0},
\quad r=1,2.
\tag{W.10}
\]

These are exactly the polynomials in the parity theorem. Its finite physical derivative bounds give, for one fixed \(\theta>0\),

\[
\deg O_{i,r}\le r+2,\qquad
\|O_{i,r}\|_{\theta,1}\le C h^{-4}.
\tag{W.11}
\]

The constants are uniform over the finite native field family, volume, and admitted shell data. To verify the absolute summation, the physical derivative tensor is bounded by \(C_re^{-c_r\tau}\). Choose \(\theta<c_r\) with a fixed margin. The sum of the remaining exponential over its at most four coordinate positions is finite uniformly in volume: bound it by a sum over finitely many trees rooted at the anchor and sum successive leaves.

#### 2.1 The extensive responses retain their own anchors

Use the exact radial decomposition, evaluated at zero computational coupling:

\[
W_r=\sum_y R_{r,y},\qquad
R_{r,y}(z)=\int_0^1
\langle z_y,D_yW_r(sz)\rangle\,ds.
\tag{W.12}
\]

It gives

\[
\deg R_{1,y}\le3,\qquad
\deg R_{2,y}\le4,\qquad
\|R_{r,y}\|_{\theta,1}\le C.
\tag{W.13}
\]

Indeed \(W_r\) is the sum of its classical homogeneous term of degree \(r+2\) and its E/coarea homogeneous term of degree \(r\). Radial decomposition assigns one coordinate slot to \(y\); the remaining physical derivative tensor has the same tree majorant anchored there. The fixed derivative locality therefore proves (W.13) directly. No volume-sized norm is assigned to the entire \(W_r\).

Only derivatives through order four are needed for the coefficient polynomials in this note. The parity remainder uses its separately established physical derivatives through order six.

### 3. Both Gaussian laws have the required cut-tree bounds

The same weighted conjugation budget (W.4) gives the real covariance estimate for \(\nu_\infty\) and for the Gaussian restricted to the convex product (W.1). For the restricted law, the product-boundary contribution is nonnegative and the weight is scalar on each coordinate block, as required by the previous homogeneous covariance proof.

Both laws are even under \(z\mapsto-z\), so all coordinate means vanish. Linear tilting leaves their potential Hessian equal to \(H\). The established concentration estimate consequently gives

\[
\sup_{i,P}\|z_i\|_{L^p(\nu_P)}
+\sup_i\|z_i\|_{L^p(\nu_\infty)}
\le C\sqrt p.
\tag{W.14}
\]

Here \(P\ge1\), and constants are independent of volume. For a polynomial of fixed degree \(D\), (W.9), Hölder, and the fact that
\(d(x,j)\le\tau(x,j(b_1),\ldots,j(b_d))\) for every participating coordinate imply

\[
\|Q_x\|_p\le C_D\|Q_x\|_{\theta,1}p^{D/2},
\]
\[
\left\|\|\nabla Q_x\|_{\gamma,x}\right\|_p
\le C_D\|Q_x\|_{\theta,1}p^{(D-1)/2},
\quad 0<\gamma<\theta.
\tag{W.15}
\]

These estimates hold under either Gaussian law. Centering costs at most a factor two. Thus the real cut theorem supplies, for every fixed \(N\ge2\),

\[
\begin{aligned}
&|\kappa_{\nu_P}(Q_{u_1}^{(1)},\ldots,Q_{u_N}^{(N)})|
+|\kappa_{\nu_\infty}(Q_{u_1}^{(1)},\ldots,Q_{u_N}^{(N)})|
\\
&\qquad\le
C_{N,D}\prod_{j=1}^N\|Q_{u_j}^{(j)}\|_{\theta,1}
\exp\!\left[
-\frac{\gamma\tau(u_1,\ldots,u_N)}{N-1}
\right].
\end{aligned}
\tag{W.16}
\]

The constants are independent of \(P\). This verifies the two-law spatial premise of the Gaussian cutoff lemma for the present polynomials. A sum over labeled trees is an equivalent sufficient majorant here, since the exponential of the minimum tree length is one term bounded by that tree sum.

#### 3.1 Cutoff error with spatial decay

For fixed polynomial degrees \(d_1,\ldots,d_N\), the cutoff lemma and its moment-partition proof give

\[
|\Delta\kappa_N|
\le C\left(\prod_j\|Q_{u_j}^{(j)}\|_{\theta,1}\right)
(1+P)^{d_1+\cdots+d_N+d_*}
e^{-\lambda P^2/8}.
\tag{W.17}
\]

Combining this bound with (W.16), using
\(\min(A,B)\le\sqrt{AB}\), gives

\[
|\Delta\kappa_N|
\le C\left(\prod_j\|Q_{u_j}^{(j)}\|_{\theta,1}\right)
(1+P)^{D}
e^{-\lambda P^2/16}
e^{-\gamma\tau(u_1,\ldots,u_N)/(2(N-1))},
\tag{W.18}
\]

where one can take the harmless enlarged power
\(D=d_1+\cdots+d_N+d_*\).
The one-argument case uses (W.17) directly and has no spatial factor.

For \(N\le8\), use the common rate \(\mu=\gamma/7\). If any \(n\le N-1\) anchors are summed and at least one remains fixed, split the tree exponential in (W.18) into two factors. A doubled traversal gives the lower bound of one half of the unsummed minimum tree length; the second factor is summed using exponential kernels. This yields

\[
\sum_{\text{summed anchors}}|\Delta\kappa_N|
\le C
\left(\prod_j A_j\right)
(1+P)^D e^{-\lambda P^2/16}
e^{-\gamma\tau(\text{unsummed anchors})/56},
\tag{W.19}
\]

when \(\|Q_{u_j}^{(j)}\|_{\theta,1}\le A_j\) uniformly in any summed position. Constants depend on the fixed \(N,D\), not on volume. This is the required use of the cutoff estimate for extensive vertices; direct summation of (W.17) would not suffice.

### 4. Replacement of both Gaussian coefficients

For \(1\le m\le6\), write

\[
L_m^P=\kappa_{\nu_P}(O_{1,0},\ldots,O_{m,0}),
\qquad
L_m^\infty=\kappa_{\nu_\infty}(O_{1,0},\ldots,O_{m,0}).
\tag{W.20}
\]

Let \(C_{2,m}^P\) be the second coefficient in Annex J (5.7), the parity theorem, and define \(C_{2,m}^\infty\) by the identical formula with every \(\kappa_{\nu_P}\) replaced by \(\kappa_{\nu_\infty}\). Explicitly,

\[
\begin{aligned}
C_{2,m}^\infty
={}&
\sum_i\kappa_\infty(O_{1,0},\ldots,O_{i,2},\ldots,O_{m,0})
\\
&+2\sum_{i<j}\kappa_\infty
(O_{1,0},\ldots,O_{i,1},\ldots,O_{j,1},\ldots,O_{m,0})
\\
&+2\sum_i\kappa_\infty
(O_{1,0},\ldots,O_{i,1},\ldots,O_{m,0},W_1)
\\
&+\kappa_\infty(O_{1,0},\ldots,O_{m,0},W_2)
\\
&+\kappa_\infty(O_{1,0},\ldots,O_{m,0},W_1,W_1).
\end{aligned}
\tag{W.21}
\]

Here \(\kappa_\infty=\kappa_{\nu_\infty}\). The two \(W_1\) factors in the last line remain two cumulant arguments.

#### Corollary 4.1 — uniform Gaussian coefficient replacement, P

For \(1\le m\le6\),

\[
\boxed{
|L_m^P-L_m^\infty|
+|C_{2,m}^P-C_{2,m}^\infty|
\le C_m h^{-4m}(1+P)^{D_m}
e^{-\lambda P^2/16}
e^{-\gamma\tau(x_1,\ldots,x_m)/56},
}
\tag{W.22}
\]

where one may take \(D_m=2m+6+d_*\). All constants are uniform in the finite volume and admissible frozen-shell data.

**Proof.** The largest number of Gaussian cumulant arguments in (W.21) is \(N=m+2\le8\). There are at most two additional anchors, from the last line. The maximum total polynomial degree is \(2m+6\): each native \(O_{i,0}\) contributes two, and each \(R_{1,y}\) contributes at most three. The remaining lines have total degrees at most \(2m+2\) or \(2m+4\).

Use (W.12) in every occurrence of \(W_1,W_2\). At fixed added anchors, (W.11) and (W.13) bound the coefficient-norm product by \(C_mh^{-4m}\). Apply (W.19) to sum the zero, one or two extra anchors in the cutoff difference. For \(L_m\) there are no extra anchors. The finitely many sums over external derivative placements in (W.21) change only \(C_m\). This proves (W.22). \(\square\)

All sums of the extensive Gaussian coefficient insertions are absolutely controlled by the same tree argument. Their volume-uniform meaning is therefore established before comparing their cutoff and untruncated values.

### 5. The combined native expansion

Let \(K_m^P(g)\) be the interacting native cumulant from the parity theorem, with the common cutoff fixed at \(P\) during the signed interpolation. Combining that theorem with (W.22) gives, for \(1\le m\le6\),

\[
\boxed{
\begin{aligned}
K_m^P(g)
={}&L_m^\infty+\frac{g^2}{2}C_{2,m}^\infty
+\mathcal E_m(g,P),\\
|\mathcal E_m(g,P)|
\le{}& C_m h^{-4m}
\left[
|g|^4+(1+P)^{D_m}e^{-\lambda P^2/16}
\right]
e^{-\gamma\tau(x_1,\ldots,x_m)/56}.
\end{aligned}
}
\tag{W.23}
\]

The working decay rate can be decreased once to be common to the parity and Gaussian cut estimates. The parity remainder has the stronger range \(4(m+4)\le40\) at these orders, so the displayed denominator 56 is a valid common weakening. The small coupling ceiling is fixed; the harmless factor \(1+g^2\) multiplying (W.22) has been absorbed into \(C_m\).

Equation (W.23) has ordinary untruncated **finite-volume** Gaussian coefficients. Wick's rule now applies directly to the displayed polynomials with covariance \(H^{-1}\). It does not identify that covariance with a continuum propagator, or compute a universal Yang--Mills ultraviolet coefficient.

#### 5.1 Logarithmic windows at the physical endpoint

If the family of admitted endpoints uses

\[
P(g_*)=a[\log(g_*^{-1})]^p,\qquad p>\tfrac12,
\tag{W.24}
\]

then the cutoff term in (W.23) is smaller than every fixed power of \(g_*\). Hence, at the physical endpoint \(g=g_*\), it can be absorbed into the \(O(g_*^4)\) remainder. For each member of this family, \(P(g_*)\) is held constant throughout the computation of the signed \(g\)-derivatives. No derivative of a moving cutoff has been suppressed.

The fixed-order constants are uniform within the admitted shell bounds, while \(H\), \(E_*\), and the coefficient \(C_{2,m}^\infty\) may still vary from shell to shell. In particular, the result is not a derivative estimate for that variation.

### What remains

This corollary settles the Gaussian-cutoff issue for the second native coefficient at the low source orders used here, including its extensive insertion sums. The parity theorem separately retains its all-source-order factorial bound with the cutoff present.

The step from these native regular integrals to the actual transported Wilson hierarchy, the complete-history domain and geometry estimates, the identification of the running operator normalization, rotation restoration, the interacting phasewise UV estimate, and the operator/phase hypotheses remain separate obligations. No part of (W.23) supplies them by itself.


---
