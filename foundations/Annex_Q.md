# Compact magnetic operator bounds for every SU(N)

**Annex Q.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

The full renormalized energy obligation E0 is still open. This note proves a new estimate on the actual compact Wilson transfer operator for every \(SU(N)\), rather than only the SU(2) temporal scalar of Annex M.

The result controls every spatial-slice multiplication observable \(q\) satisfying a pointwise bound
\[
|q|\le B S_\Gamma,
\]
where \(S_\Gamma\) is the sum of the spatial Wilson plaquette actions incident on a fixed finite link set. It gives a volume-uniform heat-sandwich estimate and a one-sided graph estimate of order \((1+\log(1+\beta))/\beta\) for the ground-centered bare field. The proof retains all spatial interactions and all compact configurations, and it does not square a quadratic-form inequality.

All six raw magnetic clover bilinears satisfy the hypothesis. There is a necessary qualification for the exact field architecture chosen: its scalar repair adds a temporal contribution to the diagonal entries. Consequently the theorem directly covers the five trace-free magnetic combinations in that exact architecture; the raw magnetic trace is an additional auxiliary representative. This distinction is kept explicit below.

The physical \(a^{-4}\) normalization remains. The same-cubic periodic-state premise has not been proved, and a choice of a cofinal sequence alone does not establish it. Section 6 gives the exact quantifier obstruction.

The standard compact transfer representation is the pure-gauge specialization of Lüscher, *Construction of a selfadjoint, strictly positive transfer matrix for Euclidean lattice gauge theories*, CMP 54 (1977), 283–292, [preprint](https://bib-pubdb1.desy.de/record/396349/files/7611148.pdf). All local comparisons used below are proved here or are the already-proved local deletion reserve of Annex M; no new complete-history RG estimate is imported.

### 1. The actual local deletion identity

Fix a finite periodic spatial lattice, spacing \(a>0\), gauge group \(SU(N)\), and the physical gauge-invariant subspace of
\[
\mathcal H_0=L^2(SU(N)^{\mathcal L_s},dH).
\]
Use the unchanged convention
\[
s(U)=N-\operatorname{Re}\operatorname{Tr}U,\qquad
0\le s(U)\le2N,\qquad \beta=2Nx_0,\qquad X_B=N\beta.
\tag{1.1}
\]

Let \(K=\bigotimes_l C_\beta\) be the normalized electric convolution, let
\[
V_s=\beta\sum_{p\ \mathrm{spatial}}s(U_p),\qquad
A=e^{-V_s/2},\qquad T_0=AKA,
\tag{1.2}
\]
and let \(\lambda_0=\|T_0\|\). Positivity improvement and gauge invariance put the unique positive top vector in the physical subspace, so the physical transfer operator \(T\) has the same norm. Normalize
\[
P=T/\lambda_0=e^{-aH},\qquad H\ge0.
\tag{1.3}
\]

For a fixed finite spatial link set \(\Gamma\), let \(\mathcal P_\Gamma\) be all spatial plaquettes incident on \(\Gamma\). Set
\[
S_\Gamma=\sum_{p\in\mathcal P_\Gamma}s(U_p),\qquad
A_\Gamma=e^{-\beta S_\Gamma/2},\qquad A=A_\Gamma A_r.
\tag{1.4}
\]
The multiplication operator \(A_r\) is independent of all links in \(\Gamma\). Therefore, on the full link Hilbert space,
\[
T_0=A_\Gamma T_{\rm del}A_\Gamma,\qquad
T_{\rm del}=K_\Gamma\otimes(A_rK_rA_r).
\tag{1.5}
\]
This is an identity, with every undeleted action factor retained. Write
\[
\lambda_{\rm del}=\|T_{\rm del}\|,\qquad
\Delta_\Gamma=\log(\lambda_{\rm del}/\lambda_0)\ge0.
\tag{1.6}
\]
Both operators commute with gauge projection. The strictly positive top-vector argument applies to \(T_{\rm del}\) as well, so its full and physical norms agree.

Since \(0\le T_{\rm del}\le\lambda_{\rm del}I\), (1.5) gives
\[
\boxed{
T\le\lambda_{\rm del}e^{-\beta S_\Gamma},
\qquad
P\le e^{\Delta_\Gamma}e^{-\beta S_\Gamma}.
}
\tag{1.7}
\]
The multiplier \(S_\Gamma\) is bounded at each fixed cutoff, nonnegative, and gauge invariant.

Two previously proved bounds remain available:
\[
0\le\Delta_\Gamma\le2N\beta|\mathcal P_\Gamma|,
\tag{1.8}
\]
and, when the containing fixed \(B\)-site spatial cube fits the compatible even-block geometry,
\[
\boxed{
\Delta_\Gamma
\le B^3\{c_N+2(N^2-1)\log(1+\beta)\}.
}
\tag{1.9}
\]
The latter is the cylinder reserve and fixed-spatial-lattice trace limit. The value of \(B\) depends only on the finite local stencil. It is independent of the total spatial volume. No temporal aspect-ratio extension of the source-free RG is used in that elementary comparison.

### 2. Local spatial energy as a quadratic form

#### Theorem 2.1 — local magnetic form comparison, P

On the physical Hilbert space,
\[
\boxed{
\beta S_\Gamma\le aH+\Delta_\Gamma I
}
\tag{2.1}
\]
as closed quadratic forms.

**Proof.** Apply operator monotonicity of the logarithm to (1.7), with a small positive regularization if necessary. Explicitly, for bounded strictly positive \(X\le Y\),
\[
\log Y-\log X
=\int_0^\infty\bigl[(X+t)^{-1}-(Y+t)^{-1}\bigr]\,dt
\]
is nonnegative in the quadratic-form sense. To cover \(P\), which has no bounded inverse, replace both sides of (1.7) by their sums with \(\epsilon I\), use the resolvent integral, and let \(\epsilon\downarrow0\). The spectral theorem gives the closed form of \(\log P=-aH\). The right comparison operator is boundedly invertible at this fixed cutoff, and its logarithm is \(\Delta_\Gamma-\beta S_\Gamma\). Hence
\[
-aH\le\Delta_\Gamma-\beta S_\Gamma,
\]
which is (2.1). \(\square\)

In contrast to the earlier electric comparison, no polar unitary occurs in (2.1): \(S_\Gamma\) is the actual time-zero multiplication operator.

For any real gauge-invariant multiplication observable \(q\) with
\[
|q(U)|\le B S_\Gamma(U),
\tag{2.2}
\]
one immediately has
\[
\bigl|\langle\psi,q\psi\rangle\bigr|
\le\frac B\beta
\left(a\langle\psi,H\psi\rangle
+\Delta_\Gamma\|\psi\|^2\right).
\tag{2.3}
\]
If \(\Omega\) is the normalized ground vector, then
\[
|\langle\Omega,q\Omega\rangle|
\le B\Delta_\Gamma/\beta.
\tag{2.4}
\]

#### Corollary 2.2 — heat-sandwich bounds, P

For \(t>0\),
\[
\boxed{
\|e^{-tH}qe^{-tH}\|
\le\frac B\beta
\left(\Delta_\Gamma+\frac a{2et}\right).
}
\tag{2.5}
\]
For \(q^\circ=q-\langle\Omega,q\Omega\rangle I\),
\[
\boxed{
\|e^{-tH}q^\circ e^{-tH}\|
\le\frac B\beta
\left(2\Delta_\Gamma+\frac a{2et}\right).
}
\tag{2.6}
\]
When \(q\ge0\), the coefficient \(2\Delta_\Gamma\) in (2.6) can be replaced by \(\Delta_\Gamma\).

**Proof.** Substitute \(e^{-tH}\psi\) in (2.3) and use
\[
\|He^{-2tH}\|=\sup_{x\ge0}xe^{-2tx}=(2et)^{-1}.
\]
The centered bound follows from (2.4) and \(\|e^{-2tH}\|\le1\). In the positive case, both \(e^{-tH}qe^{-tH}\) and \(\langle q\rangle_\Omega e^{-2tH}\) are positive. The norm of their selfadjoint difference is bounded by the larger of their norms, giving the improvement. \(\square\)

These are arbitrary-vector operator bounds for the actual cutoff ground Hamiltonian. They are not merely estimates of vacuum matrix elements.

### 3. One-sided graph bounds without squaring forms

The form bound (2.1) must not be squared to infer a one-sided operator estimate. The stronger exponential comparison (1.7) supplies the missing argument.

#### Lemma 3.1 — local exponential range estimate, P

For \(0<s\le1/2\),
\[
\boxed{
\|e^{s\beta S_\Gamma}e^{-saH}\|
\le e^{s\Delta_\Gamma}.
}
\tag{3.1}
\]

**Proof.** The function \(x\mapsto x^{2s}\) is operator monotone for \(0<2s\le1\). For completeness, if \(0<r<1\), its representation
\[
x^r=\frac{\sin\pi r}{\pi}
\int_0^\infty t^{r-1}x(t+x)^{-1}\,dt
\]
proves this from resolvent monotonicity; the case \(r=1\) is immediate. Applying it to (1.7) gives
\[
P^{2s}\le
e^{2s\Delta_\Gamma}e^{-2s\beta S_\Gamma}.
\tag{3.2}
\]
Conjugation by \(e^{s\beta S_\Gamma}\), which is bounded at fixed cutoff, gives
\[
\|P^s e^{s\beta S_\Gamma}\|^2
\le e^{2s\Delta_\Gamma}.
\]
Taking the adjoint and using \(P^s=e^{-saH}\) proves (3.1). This is the relevant range-factorization step. \(\square\)

Let \(\Pi_E=\mathbf1_{[0,E]}(H)\). From (3.1),
\[
\|e^{s\beta S_\Gamma}\Pi_E\|
\le e^{s(\Delta_\Gamma+aE)}.
\tag{3.3}
\]
For \(q\) satisfying (2.2),
\[
\|q e^{-s\beta S_\Gamma}\|
\le B\sup_{u\ge0}u e^{-s\beta u}
=\frac B{es\beta}.
\tag{3.4}
\]
Choose \(s=(2+\Delta_\Gamma+aE)^{-1}\). This is at most \(1/2\), and \(s(\Delta_\Gamma+aE)\le1\), so
\[
\boxed{
\|q\Pi_E\|
\le\frac B\beta(2+\Delta_\Gamma+aE).
}
\tag{3.5}
\]

#### Theorem 3.2 — local spatial field graph bound, P

For every real multiplication \(q\) satisfying (2.2),
\[
\boxed{
\|q(1+H)^{-2}\|
\le\frac{4B}{\beta}(2+\Delta_\Gamma+a).
}
\tag{3.6}
\]
For its ground-centered version,
\[
\boxed{
\|q^\circ(1+H)^{-2}\|
\le\frac B\beta(8+5\Delta_\Gamma+4a).
}
\tag{3.7}
\]

**Proof.** Decompose the spectrum with
\[
R_j=\mathbf1_{\{2^j\le1+H<2^{j+1}\}},\qquad j\ge0.
\]
Using (3.5) with \(E=2^{j+1}\) and the triangle inequality for the operator-norm convergent sum,
\[
\begin{aligned}
\|q(1+H)^{-2}\|
&\le\frac B\beta\sum_{j\ge0}
(2+\Delta_\Gamma+a2^{j+1})\,2^{-2j}\\
&=\frac B\beta
\left\{\frac43(2+\Delta_\Gamma)+4a\right\}\\
&\le\frac{4B}{\beta}(2+\Delta_\Gamma+a).
\end{aligned}
\]
Adding the identity subtraction bound (2.4) proves (3.7). \(\square\)

At each fixed cutoff \(q\) is a bounded multiplication operator, so its domain is the full physical Hilbert space. The important content of (3.6)–(3.7) is the uniform cutoff and spatial-volume coefficient in the specified normalization. They make no claim that an unconstructed renormalized continuum operator has already been obtained.

A more general polynomial local version follows from the same proof. If \(|q|\le B S_\Gamma^r\), with \(r\ge1\), choose \(s=r/(2r+\Delta_\Gamma+aE)\). Then
\[
\|q\Pi_E\|
\le B\beta^{-r}(2r+\Delta_\Gamma+aE)^r,
\tag{3.8}
\]
and
\[
\boxed{
\|q(1+H)^{-(r+1)}\|
\le 2B\beta^{-r}(2r+\Delta_\Gamma+2a)^r.
}
\tag{3.9}
\]
Indeed, on the \(j\)-th spectral band the numerator in (3.8) is at most
\(2^{jr}(2r+\Delta_\Gamma+2a)^r\), leaving the summable factor \(2^{-j}\). This supplies a controlled finite-product extension on any fixed local stencil.

### 4. Exact application to the magnetic clover tensor

Use the same four-quadrant clover as the architecture. For \(A=(i,j)\), \(1\le i<j\le3\), let
\[
C_A(x)=\frac1{8i}\sum_{\sigma,\tau=\pm1}\sigma\tau\,
\pi_0\bigl(P_{\sigma e_i,\tau e_j}(x)
-P_{\sigma e_i,\tau e_j}(x)^\dagger\bigr),
\tag{4.1}
\]
where all loops are based at \(x\), and \(\pi_0\) removes the scalar matrix part. All links in these stencils lie in the same time slice.

Write \(\mathcal I_B=\{(1,2),(1,3),(2,3)\}\). For a real symmetric \(3\)-by-\(3\) matrix \(M\), define the dimensionless raw magnetic field
\[
\mathsf q_M(x)=
\sum_{A,B\in\mathcal I_B}M_{AB}
\operatorname{Tr}(C_A(x)C_B(x)).
\tag{4.2}
\]
The six independent choices of \(M\) are the six raw spatial curvature-bilinear components.

For a unitary matrix \(U\),
\[
\left\|\frac{U-U^\dagger}{2i}\right\|_{\rm HS}^2
=\sum_j\sin^2\theta_j
\le2\sum_j(1-\cos\theta_j)=2s(U).
\tag{4.3}
\]
Orthogonal projection \(\pi_0\) contracts the Hilbert–Schmidt norm. Convexity of that norm squared therefore gives
\[
\|C_A(x)\|_{\rm HS}^2
\le\frac12\sum_{\sigma,\tau}
s(P_{\sigma e_i,\tau e_j}(x)).
\tag{4.4}
\]
Let \(\Gamma\) contain the finitely many links needed to include these magnetic plaquettes in \(\mathcal P_\Gamma\). The Gram matrix
\[
G_{AB}(x)=\operatorname{Tr}(C_A(x)C_B(x))
\]
is positive semidefinite. Hence
\[
\begin{aligned}
|\mathsf q_M(x)|
&\le\|M\|_{\rm op}\operatorname{Tr}G(x)\\
&\le\frac{\|M\|_{\rm op}}2
\sum_{A\in\mathcal I_B}\sum_{\sigma,\tau}s(P_{\sigma A_1,\tau A_2}(x))\\
&\le\frac{\|M\|_{\rm op}}2 S_\Gamma.
\end{aligned}
\tag{4.5}
\]
Each plaquette on the second line is one of the finitely many geometric plaquettes in the stencil. On the nondegenerate tori used in the construction, different quadrants and magnetic orientations give distinct such plaquettes. A fixed multiplicity factor can be inserted on smaller exceptional geometries; those are excluded by the cofinal minimum-size conditions.

#### Corollary 4.1 — all-\(SU(N)\) magnetic clover bound, P

For every fixed real symmetric \(M\), define
\[
\mathsf q_M^\circ(x)=
\mathsf q_M(x)-\langle\Omega,\mathsf q_M(x)\Omega\rangle I.
\]
Then
\[
\boxed{
\|\mathsf q_M^\circ(x)(1+H)^{-2}\|
\le
\frac{\|M\|_{\rm op}}{2\beta}
(8+5\Delta_\Gamma+4a).
}
\tag{4.6}
\]
The heat estimate is
\[
\boxed{
\|e^{-tH}\mathsf q_M^\circ(x)e^{-tH}\|
\le
\frac{\|M\|_{\rm op}}{2\beta}
\left(2\Delta_\Gamma+\frac a{2et}\right).
}
\tag{4.7}
\]
If \(M\ge0\), the \(2\Delta_\Gamma\) in (4.7) can be replaced by \(\Delta_\Gamma\).

With (1.9), these estimates are
\[
O\!\left(\frac{1+\log(1+\beta)}{\beta}\right)
\]
at fixed \(t>0\), uniformly in compatible spatial volume and \(0<a\le1\). They apply to arbitrary vectors in the physical Hilbert space and retain the entire compact Wilson action.

#### 4.1 The scalar-repair caveat is necessary

The exact hierarchy uses
\[
\widetilde q_{AB,a}
=a^{-4}\operatorname{Tr}(C_A C_B)
+\frac{\delta_{AB}}6(2w_a-t_a),
\tag{4.8}
\]
where \(w_a\) is the full four-dimensional Wilson action density and \(t_a\) is the trace over all six curvature planes. This ensures that the scalar trace is the exact Wilson coupling derivative.

For magnetic \(M\),
\[
\sum_{A,B\in\mathcal I_B}M_{AB}\widetilde q_{AB,a}
=a^{-4}\mathsf q_M
+\frac{\operatorname{Tr}M}{6}(2w_a-t_a).
\tag{4.9}
\]
Thus if \(\operatorname{Tr}M=0\), the correction cancels exactly. The five-dimensional trace-free magnetic subspace consists of three off-diagonal entries and two independent diagonal differences. It is directly covered by (4.6)–(4.7), with the factor \(a^{-4}\) restored.

If \(\operatorname{Tr}M\ne0\), the repaired field contains temporal plaquettes and is not a time-zero multiplication observable. Equations (4.6)–(4.7) control its raw magnetic part only. The raw magnetic trace is a legitimate auxiliary cutoff field, but it is not silently substituted for the repaired scalar channel.

Likewise, changing which coordinate is called time gives a related estimate in a different reflection reconstruction. That does not, by itself, give all 21 fields a bound with respect to one common Hamiltonian.

### 5. Physical smearing and the ultraviolet loss

Let \(g\) be a fixed compact spatial test, and let
\[
\mathsf Q_{M,a}(g)
=a^3\sum_{\mathbf x}g(\mathbf x)\,
\mathsf q_M^\circ(\mathbf x).
\tag{5.1}
\]
Translation invariance and the uniform local deletion constant imply
\[
\|\mathsf Q_{M,a}(g)(1+H)^{-2}\|
\le
\frac{\|M\|_{\rm op}}{2\beta}
(8+5\Delta_*+4a)
\left(a^3\sum_{\mathbf x}|g(\mathbf x)|\right),
\tag{5.2}
\]
with \(\Delta_*\) bounded by the same fixed-stencil version of (1.9). The same argument applies to the heat sandwiches. There is no factor from the total spatial volume.

For a physical dimension-four normalization
\[
Q^R_{M,a}(g)
=z_a a^{-4}\mathsf Q_{M,a}(g)+d_a(g)I,
\tag{5.3}
\]
the theorem yields only
\[
\boxed{
\|Q^R_{M,a}(g)(1+H)^{-2}\|
\le
|z_a|a^{-4}
\frac{\|M\|_{\rm op}}{2\beta}
(8+5\Delta_*+4a)
\|g\|_{\ell^1_a}
+|d_a(g)|.
}
\tag{5.4}
\]
The factor \(a^{-4}\) remains. Along an AF trajectory, a logarithmic gain in \(\beta\) does not cancel it. The theorem therefore supplies a sharper actual cutoff operator estimate, not the renormalized E0 conclusion.

There are two further distinctions. First, the center in this proof is the finite-volume ground-state mean, while the continuum prescription must use the normalization and identity coefficient fixed in F0. Second, the periodic Wilson hierarchy need not be replaced by ground-state matrix elements without the state-control step. The periodic bridge remains conditional.

### 6. Why the same-cubic thermal premise is not a diagonal-choice theorem

For the spatial lattice of side \(T\), denote its normalized transfer Hamiltonian by \(H_{a,T}\). The required the quantity is
\[
\Gamma(a,T)
=\log\frac{\operatorname{Tr}e^{-(T/2)H_{a,T}}}
{\operatorname{Tr}e^{-T H_{a,T}}}.
\tag{6.1}
\]
At every *fixed* \(a,T\), trace class and a unique ground state imply
\[
\lim_{u\to\infty}
\log\frac{\operatorname{Tr}e^{-(u/2)H_{a,T}}}
{\operatorname{Tr}e^{-uH_{a,T}}}=0.
\tag{6.2}
\]
This follows by spectral expansion and dominated convergence at a fixed trace-class reference time. It is a statement about one spatial operator while the temporal length \(u\) grows independently.

The target instead sets \(u=T\) and changes \(H_{a,T}\) when \(T\) changes. Formula (6.2) does not establish
\[
\Gamma(a_n,T_n)/T_n\longrightarrow0
\tag{6.3}
\]
on a cubic sequence.

A genuine diagonal selection would be justified, for example, if one first proved that, for each sufficiently small admitted \(a\),
\[
\liminf_{\substack{T\to\infty\\T\ {\rm admitted}}}
\Gamma(a,T)/T=0.
\tag{6.4}
\]
Then one could select admitted \(T_n\) with \(\Gamma(a_n,T_n)/T_n<1/n\), \(T_n\to\infty\), and \(\log(1/a_n)/T_n\to0\). But (6.4) is an additional spatially uniform spectral assertion. Neither finite-cutoff ground-state uniqueness nor the known local deletion reserve proves it.

The positive-transfer counterexample demonstrates the logical gap even in finite-dimensional transfer families with good ground-state insertion estimates. Locality of the Wilson kernel may provide further information, but that information must enter through a proved estimate. No such thermal estimate is established in this argument.

The new local magnetic bounds also do not imply (6.3). Their Hamiltonian is the ground-normalized one, and their local energy cost \(\Delta_\Gamma\) controls a fixed insertion region. The thermal trace increment sums excitations throughout the whole growing spatial torus. A uniform local form bound is not a bound on that total spectral multiplicity.

### 7. Operator conditions

**Closed in this note:** local spatial action form control; a local exponential range estimate; one-sided polynomial graph bounds for dominated spatial multiplication marks; and their exact all-\(SU(N)\) magnetic clover application, including the five trace-free magnetic combinations in the chosen scalar-repaired field architecture.

**Still open for E0/V0:** renormalized physical cancellation of the \(a^{-4}\) loss; correct running mixing and identity normalization; temporal and mixed tensor representatives on one common reconstructed domain; the same-cubic periodic state estimate or another rigorously verified state passage; and the interacting block/disintegration hypotheses required by the phase-transfer theorem.

The new results concern the complete compact Wilson cutoff theory in their stated channels. They do not close the renormalized continuum operator obligation, and they do not complete four-dimensional Yang–Mills existence.


---
