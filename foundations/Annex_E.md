# Explicit Wilson tensor hierarchy, positivity and contact locality

**Annex E.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

This note completes a concrete **cutoff positivity and translation architecture** for the full 21-component curvature-bilinear family. It specifies the lattice fields, including an exact Wilson coupling-derivative scalar; gives a source-jet prescription compatible at every order; proves its partial-diagonal support and reflection positivity; and proves a quantitative removal of microscopic overlapping stencils on coincidence-flat tests.

There are two different conclusions.

1. **P: structural P0 theorem.** The explicitly defined Wilson hierarchy below has permutation symmetry, exact fine-lattice translations, the full signed-permutation tensor action, and the required reflection positivity on every fixed positive-time test algebra once its support margin fits the stencil. These statements hold for arbitrary finite running real equivariant mixing coefficients and real scalar identity subtractions. Higher point-local source contacts are compatible at all orders, preserve positivity, and vanish exactly on the coincidence-flat test space.
2. **P with an explicit normalization budget: microscopic contact theorem.** A coherent finite-stencil exclusion of overlapping insertion centers preserves the same positivity and symmetries. Its difference from the ordinary moments is at most
   \[
   a\,C^{m+1}m!\,\nu_{qm}(F)
   \]
   for fixed \(q,C\), if the one-field normalization has a fixed polynomial cutoff bound. The theorem applies unconditionally to the specified energy-normalized, vacuum-centered cutoff family. It also applies to any eventual logarithmically running normalization for which that bound is established.

These results do **not** prove that the ultraviolet matching coefficients required by F0 exist in this architecture, that the prescribed normalization at \(\mu\) is achieved, or that its off-diagonal correlations satisfy S0. Neither full \(O(4)\) restoration nor phase/operator control is claimed. In particular, the renormalization/matching obligation is not renamed as a positivity result.

The proofs use the actual compact Wilson measure. They do not use a reflection-positive law for auxiliary RG histories and do not require source-dependent integration maps.

### 1. The actual finite field family

#### 1.1 Links and the four-quadrant clover

Let
\[
\Lambda_{a,T}=a\mathbb Z^4/T\mathbb Z^4,\qquad T=na,
\]
with even \(n\ge4\). Time is coordinate \(0\). The gauge group is \(SU(N)\), \(N\ge2\), with normalized Haar measure and one variable on each positively oriented link. For the reverse link set \(U_{yx}=U_{xy}^{-1}\). The probability law is
\[
d\mu_{a,T,\beta}(U)=Z^{-1}
\exp\left[-\beta\sum_p\bigl(N-\operatorname{Re}\operatorname{Tr}U_p\bigr)\right]
\prod_\ell dU_\ell,\qquad \beta\ge0.
\tag{1.1}
\]

The normalization dictionary remains \(\beta=2Nx_0\), and the coefficient of Balaban's normalized-trace action is \(X_B=N\beta=2N^2x_0\). Thus the total scalar in (1.6) is the \(\beta\)-derivative of the specified P2 action, while its \(x_0\)-derivative is \(2N\) times that scalar. No convention change is hidden in the tensor definition.

For two orthogonal signed unit vectors \(u,v\), define the plaquette based at \(x\) by
\[
P_{u,v}(x)=
U_{x,x+au}\,
U_{x+au,x+a(u+v)}\,
U_{x+a(u+v),x+av}\,
U_{x+av,x}.
\tag{1.2}
\]
In particular \(P_{v,u}(x)=P_{u,v}(x)^{-1}\).

Let \(\pi_0 H=H-\operatorname{Tr}(H)I/N\). For \(0\le\mu<\nu\le3\), put
\[
C_{\mu\nu,a}(x)=
\frac{1}{8i}
\sum_{\sigma,\tau=\pm1}\sigma\tau\,
\pi_0\!\left(P_{\sigma e_\mu,\tau e_\nu}(x)
             -P_{\sigma e_\mu,\tau e_\nu}(x)^\dagger\right),
\qquad C_{\nu\mu,a}=-C_{\mu\nu,a}.
\tag{1.3}
\]

Each \(C_{\mu\nu,a}\) is traceless Hermitian. All plaquette loops are based at the same vertex; no comparison of Lie algebra variables in different gauge frames is implicit.

Let \(\mathcal I=\{(\mu,\nu):0\le\mu<\nu\le3\}\), so \(|\mathcal I|=6\). The real symmetric matrix
\[
q_{AB,a}(x)=a^{-4}\operatorname{Tr}\bigl(C_{A,a}(x)C_{B,a}(x)\bigr),
\qquad A,B\in\mathcal I,
\tag{1.4}
\]
has 21 independent components. Its trace will be denoted
\[
t_a(x)=\sum_{A\in\mathcal I}q_{AA,a}(x).
\]

The matrix entries are real: for Hermitian \(C_A,C_B\),
\(\overline{\operatorname{Tr}(C_AC_B)}
=\operatorname{Tr}(C_BC_A)=\operatorname{Tr}(C_AC_B)\).
The matrix \(q(x)\) is positive semidefinite as a Gram matrix, although positivity of individual field values is not needed for OS positivity.

#### 1.2 Retain the exact Wilson scalar channel

Define the vertex action density
\[
w_a(x)=\frac{1}{4a^4}
\sum_{\mu<\nu}\sum_{\sigma,\tau=\pm1}
\left[N-\operatorname{Re}\operatorname{Tr}
P_{\sigma e_\mu,\tau e_\nu}(x)\right].
\tag{1.5}
\]

Every unoriented elementary plaquette occurs once at each of its four vertices. Its trace action is unchanged by orientation reversal and by moving the root around the plaquette. Hence, exactly,
\[
\boxed{a^4\sum_{x\in\Lambda_{a,T}}w_a(x)=\sum_p s(U_p).}
\tag{1.6}
\]

More generally, for any vertex profile \(f\),
\[
\boxed{
a^4\sum_x f(x)w_a(x)
=\sum_p s(U_p)\,\frac14\sum_{v\in\operatorname{Vert}(p)}f(v).
}
\tag{1.7}
\]

Thus the scalar source has the explicit four-corner plaquette coefficient. For \(f=1\), it is the exact total coupling insertion \(\partial_\beta(\beta S)\). A source factor \(e^{\lambda a^4\sum f w_a}\) changes the Wilson plaquette coefficient to
\(\beta-\lambda\frac14\sum_{v\in p}f(v)\); this fixes the sign convention.

To keep this scalar together with the other twenty tensor directions, set
\[
\boxed{
\widetilde q_{AB,a}(x)
=q_{AB,a}(x)+\frac{\delta_{AB}}6\,[\,2w_a(x)-t_a(x)\,].
}
\tag{1.8}
\]
Then
\[
\frac12\sum_A\widetilde q_{AA,a}(x)=w_a(x).
\tag{1.9}
\]

Only the scalar component is changed. The traceless Ricci/stress, pseudoscalar and Weyl components remain those of the clover bilinear.

For a fixed smooth classical connection, plaquette expansion gives
\[
C_{\mu\nu,a}(x)=a^2F_{\mu\nu}(x)+O(a^3),
\]
\[
w_a(x)=\frac12\sum_{\mu<\nu}
\operatorname{Tr}\bigl(F_{\mu\nu}(x)^2\bigr)+O(a),
\qquad
\widetilde q_{AB,a}(x)=\operatorname{Tr}(F_AF_B)(x)+O(a).
\tag{1.10}
\]
The conservative errors shown here suffice to identify the engineering tensor type; the symmetric stencil allows sharper classical errors. This is a classical consistency calculation, not a theorem of quantum universality.

There is also a useful exact bound. For a unitary matrix \(P\), let
\(H(P)=(P-P^\dagger)/(2i)\). Spectral calculus gives
\[
\|H(P)\|_{\mathrm{HS}}^2
=\sum_j\sin^2\theta_j
\le2\sum_j(1-\cos\theta_j)=2s(P).
\]
Since (1.3) is the average of four signed \(\pi_0H(P)\)'s,
\[
\|C_{A,a}(x)\|_{\mathrm{HS}}^2
\le\frac12\sum_{\sigma,\tau}s(P_{\sigma A_1,\tau A_2}(x)).
\]
Summing over \(A\) proves
\[
0\le t_a(x)\le2w_a(x).
\tag{1.11}
\]
Consequently \(\widetilde q(x)\) is also positive semidefinite and has trace \(2w_a(x)\). In particular,
\[
|\widetilde q_{AB,a}(x)|\le2w_a(x).
\tag{1.12}
\]

#### 1.3 Exact gauge, translation and hypercubic transformations

A gauge transformation sends every plaquette in (1.2) to
\(\Omega_xP_{u,v}(x)\Omega_x^{-1}\). Therefore \(C_A(x)\) transforms by conjugation at \(x\), and every component of \(\widetilde q(x)\) is gauge invariant.

Let \(g\in H_4=(\mathbb Z_2)^4\rtimes S_4\), and write
\[
ge_\mu=\varepsilon_\mu e_{\pi(\mu)}.
\]
Use the pullback convention \((gU)_{xy}=U_{gx,gy}\). Relabeling the four quadrants in (1.3) gives exactly
\[
C_{\mu\nu,a}(x;gU)=
\varepsilon_\mu\varepsilon_\nu
C_{\pi(\mu)\pi(\nu),a}(gx;U),
\tag{1.13}
\]
with the displayed antisymmetry used to reorder a pair. The action density obeys \(w_a(x;gU)=w_a(gx;U)\). Thus (1.8) transforms in the canonical representation
\[
E=\operatorname{Sym}^2(\Lambda^2\mathbb R^4).
\]
Denote its matrix by \(D(g)\). In an orthonormal component basis,
\[
\widetilde q_a(x;gU)=D(g)\widetilde q_a(gx;U).
\tag{1.14}
\]

Translations by \(b\in a\mathbb Z^4\) obey the analogous identity with no tensor matrix. All these identities are exact on the torus. The Wilson measure is invariant under the corresponding change of link variables, since it preserves Haar measure and permutes unoriented plaquettes.

Each field depends only on plaquettes incident on \(x\), hence on links with endpoints in \(x+[-a,a]^4\). The same support statement holds after (1.8). This is the actual support margin used below.

#### 1.4 Running one-field mixing

Choose, at each cutoff, a finite real matrix \(Z_a\) commuting with every \(D(g)\), and a finite real vector \(c_a\in E^{H_4}\). Define
\[
\Phi_{\alpha,a}(x)
=\sum_\beta (Z_a)_{\alpha\beta}
\widetilde q_{\beta,a}(x)-(c_a)_\alpha.
\tag{1.15}
\]

No uniform bound on \(Z_a\), \(Z_a^{-1}\) or \(c_a\) is assumed for the positivity theorem. An inverse is not needed. The seven real hypercubic channel coefficients from the classification give an explicit parametrization of \(Z_a\). The invariant vector \(c_a\) is the scalar identity-mixing direction.

The coefficients are independent of \(x\). Their normalization at \(\mu\), cutoff dependence and permitted volume dependence are questions for F0; the positivity theorem does not select their values. Its conclusions hold in particular for any prescribed \(Z(a,\mu)\) and \(c(a,\mu)\) that meet the displayed reality and symmetry conditions.

Equations (1.14) and the exact lattice translation identity continue to hold for \(\Phi\).

### 2. Reflection positivity proved directly on the Wilson integral

#### 2.1 Site-reflection factorization

Let \(\theta(x_0,\mathbf x)=(-x_0,\mathbf x)\) modulo \(T\). The two fixed planes are \(x_0=0\) and \(x_0=T/2\). Decompose the link variables into:

- \(B\): spatial links lying in the two fixed planes;
- \(U_+\): all other links in the closed positive half-torus;
- \(U_-\): their reflected partners in the negative half.

Every elementary plaquette lies entirely in one closed half or entirely in a fixed plane. The action therefore splits as
\[
S(U)=S_+(U_+,B)+S_-(U_-,B)+S_0(B),
\]
and reflection identifies the two first terms. Haar measure has the corresponding product decomposition. For every bounded complex function \(A(U_+,B)\),
\[
\begin{aligned}
\mathbb E_\mu[\overline{A(\theta U)}A(U)]
&=Z^{-1}\int dB\,e^{-\beta S_0(B)}
\\
&\quad\times
\left|\int dU_+\,e^{-\beta S_+(U_+,B)}A(U_+,B)\right|^2
\ge0.
\end{aligned}
\tag{2.1}
\]

This proof uses the original unconstrained compact link integral. It introduces no gauge fixing or signed activity law. It is the site-reflection property needed here; no assertion about an independently defined auxiliary-history reflection is made.

#### 2.2 Tensor reflection and Wick phases

Let \(r=\operatorname{diag}(-1,1,1,1)\). In the real tensor-component basis,
\[
D(r)_{\alpha\alpha}=(-1)^{n_0(\alpha)},
\]
where \(n_0(\alpha)\in\{0,1,2\}\) counts the occurrences of the time index in the two antisymmetric index pairs. Thus
\[
\overline{\Phi_\alpha(x;\theta U)}
=\sum_\beta D(r)_{\alpha\beta}\Phi_\beta(\theta x;U).
\tag{2.2}
\]

For a component test kernel \(F_m\), define \(\Theta F_m\) by reflecting all arguments, complex conjugating its coefficients, applying \(D(r)\) to each component index, and reversing their order. The reversal makes it the usual Borchers involution; the cutoff random variables themselves commute.

If a Hermitian Wick component convention is desired, put
\[
\widehat\Phi_\alpha=i^{n_0(\alpha)}\Phi_\alpha.
\tag{2.3}
\]
The antilinearity in (2.2) cancels the reflection sign:
\[
\overline{i^{n_0(\alpha)}}(-1)^{n_0(\alpha)}
=i^{n_0(\alpha)}.
\]
In that basis the antilinear reflection has no remaining component sign. General Euclidean tensor transformations are conjugated by this fixed Wick matrix. One must use a single convention throughout the hierarchy; a real Euclidean tensor component with an odd number of time indices is not assigned the wrong scalar reflection rule.

#### 2.3 The full cutoff hierarchy

For a finite joint test vector \(F=(F_0,F_1,\ldots,F_M)\), let
\[
\mathcal A_a(F;U)=
\sum_{m=0}^M a^{4m}
\sum_{x_1,\ldots,x_m}
\sum_{\alpha_1,\ldots,\alpha_m}
F_{m;\boldsymbol\alpha}(x_1,\ldots,x_m)
\prod_{j=1}^m\Phi_{\alpha_j,a}(x_j).
\tag{2.4}
\]
At finite cutoff the sum is finite. For continuum tests use their interior torus embedding, specified in Section 6.

Suppose the center supports of all nonzero \(F_m\) lie in
\[
\delta<x_{j,0}<T/2-\delta
\]
for a fixed \(\delta>0\), and \(a<\delta\). The actual link support of every term in (2.4) then lies in the positive half. Equation (2.1) proves
\[
\boxed{
\sum_{r,s}S_{r+s,a,T}(\Theta F_r\otimes F_s)
=\mathbb E_\mu[\overline{\mathcal A_a(F;\theta U)}
\mathcal A_a(F;U)]
\ge0.
}
\tag{2.5}
\]

This is a statement about the full moments, for arbitrary polynomial degree and arbitrary joint test kernels. It is not an estimate only on connected derivatives or on factorized tests. Permutation symmetry, exact lattice translations and hypercubic covariance follow directly from their proved field/measure identities.

### 3. A concrete all-order point-contact prescription

#### 3.1 Formal source maps

Use smooth compactly supported sources \(j:\mathbb R^4\to E\), sampled together with their derivatives at lattice vertices. This is a permitted cutoff source prescription: source jets are evaluated at a point even though the marked field has a neighboring plaquette support.

Put
\[
\mathcal L_a(j;U)=a^4\sum_x\langle j(x),\Phi_a(x;U)\rangle.
\]
Choose formal coefficient sequences, compatible under truncation in source degree,
\[
R_a[j](x)=j(x)
+\sum_{r\ge2}\frac1{r!}T_{a,r}\bigl(j(x),\ldots,j(x)\bigr),
\tag{3.1}
\]
and
\[
C_a[j]=a^4\sum_x\sum_{r\ge2}\frac1{r!}
\sum_{\sum_i|\gamma_i|\le4}
c^{\gamma_1,\ldots,\gamma_r}_{a,r}
\bigl(\partial^{\gamma_1}j(x),\ldots,
\partial^{\gamma_r}j(x)\bigr).
\tag{3.2}
\]

Here \(T_{a,r}:\operatorname{Sym}^r E\to E\) is real and \(H_4\)-equivariant. The real coefficients of \(C_a\) are invariant for the simultaneous tensor and source-derivative action, and are symmetrized in the pairs of source labels and derivative indices. All coefficients are independent of \(x\).

The derivative order four in (3.2) is the vacuum contact degree in the dimension-four power-counting class. Dimension-four operator-valued outputs in (3.1) carry no source derivatives. The formulas do not assert that these are the only outputs of the interacting induction: irrelevant vertices remain in that induction. They specify the local relevant/contact prescription used for the external hierarchy.

Define, as a formal source jet,
\[
G_a[j;U]=
\exp\{\mathcal L_a(R_a[j];U)-C_a[j]\},
\qquad
\mathcal M_a^{R,C}[j]=\mathbb E_\mu G_a[j;U].
\tag{3.3}
\]

At any finite source order \(M\), truncate all series above \(M\). Only finitely many coefficients and finite cutoff moments occur. The logarithm/exponential composition is algebraic; no cutoff-independent complex source disc or convergence of the infinite source series is assumed. The constant coefficient is one.

The one-field coefficient is exactly the field (1.15), since \(R_a[j]=j+O(j^2)\) and \(C_a[j]=O(j^2)\). Its identity subtraction is not confused with a higher-source contact subtraction.

#### 3.2 Explicit positivity and triangularity

For two sources supported in disjoint time half-spaces,
\[
R_a[j_-+j_+]=R_a[j_-]+R_a[j_+],\qquad
C_a[j_-+j_+]=C_a[j_-]+C_a[j_+].
\tag{3.4}
\]
All derivatives of the absent source vanish at every root in the other support. Consequently
\[
G_a[j_-+j_+;U]=G_a[j_-;U]G_a[j_+;U]
\tag{3.5}
\]
coefficient by coefficient. Reality and equivariance give
\[
G_a[\Theta j;U]=\overline{G_a[j;\theta U]}.
\tag{3.6}
\]

For a positive-time polynomial test vector \(F\), extract its finite coefficients from \(G_a\) to obtain a bounded positive-half-link function \(\mathcal T_aF\). This is a triangular map: the degree-\(m\) coefficient has leading term the ordinary product of \(m\) fields (1.15), while every nonlinear \(R\) or \(C\) vertex lowers the number of field factors. The finite source degree ensures that the map is defined even if the full source series diverges.

Equations (3.5)–(3.6) and the Wilson square formula (2.1) prove
\[
\boxed{
\sum_{r,s}S^{R,C}_{r+s,a,T}(\Theta F_r\otimes F_s)
=\mathbb E_\mu[\overline{(\mathcal T_aF)(\theta U)}
(\mathcal T_aF)(U)]\ge0.
}
\tag{3.7}
\]

The same proof works for joint test kernels. At finite cutoff, coefficient extraction produces finite sums of values and derivatives of those kernels on partial diagonals. Thus the polynomial map extends directly; an unproved nuclearity passage is not being used for this finite-cutoff statement.

#### 3.3 Composition closes in the same class

Let \(\mathfrak T_{R,C}\) act on a normalized formal functional by
\[
(\mathfrak T_{R,C}\mathcal M)[j]=e^{-C[j]}\mathcal M[R[j]].
\]
Then
\[
\boxed{
\mathfrak T_{R_2,C_2}\mathfrak T_{R_1,C_1}
=\mathfrak T_{\,R_1\circ R_2,\ C_2+C_1\circ R_2}.
}
\tag{3.8}
\]

Since \(R_2\) has no source derivatives, differentiating \(R_2[j]\) in a monomial of total derivative order at most four leaves the total derivative order at most four. Thus \(C_1\circ R_2\) is again of the form (3.2). The composed \(R\) is again point-local, equivariant and real, with identity linear term. The formal inverse also exists:
\[
(R,C)^{-1}=(R^{-1},-C\circ R^{-1}).
\]
No estimate for a uniformly bounded inverse mixing matrix is involved.

This proves all-order compatibility for repeated local renormalization at the same external source point. It does not identify a finite-size carrier or a coarse source stencil with that point without a remainder estimate; such an identification remains part of F0/M0.

#### 3.4 Symmetry can be imposed at the coefficient level

The finite-group Reynolds map gives an explicit projection onto the permitted source coefficients:
\[
T_{a,r}^{\mathrm{sym}}(v_1,\ldots,v_r)
=\frac1{|H_4|}\sum_{g\in H_4}D(g)^{-1}
\widetilde T_{a,r}(D(g)v_1,\ldots,D(g)v_r).
\tag{3.9}
\]
Apply the analogous invariant projection to the order-four source-jet tensors of \(C_a\), and take real coefficients. The group acts isometrically on the finite component/derivative spaces, so these projections do not increase the corresponding multilinear operator norm. They commute with truncation in source degree.

This is a coefficient-level construction. Averaging an arbitrary nonsymmetric renormalized hierarchy is not claimed to preserve its ultraviolet normalization. The one-field coefficients in (1.15) are chosen translation independent and equivariant from the outset.

### 4. Exact contact support on the required test space

Let
\[
\Delta_m=\bigcup_{i<j}\{x_i=x_j\},
\qquad
\mathcal S_0(\mathbb R^{4m})
=\{F\in\mathcal S:\partial^\alpha F|_{\Delta_m}=0
\text{ for every }\alpha\}.
\tag{4.1}
\]

#### Theorem 4.1 — exact partial-diagonal support

At fixed cutoff and fixed source order \(m\), the difference between the hierarchy (3.3) and the ordinary full moments of (1.15) is a finite-order distribution supported on partial coincidence diagonals. Its spatial derivative order is at most \(2m\). For compact tests embedded without torus seam identifications,
\[
\boxed{S^{R,C}_{m,a,T}(F)=S^\Phi_{m,a,T}(F)
\quad\text{for every }F\in\mathcal S_0.}
\tag{4.2}
\]

**Proof.** In a term containing a higher \(R\) vertex of source degree \(r\ge2\), all \(r\) differentiated source slots are evaluated at one lattice root \(x\). Hence their external source coordinates coincide. The same is true for a higher \(C\) vertex, possibly with source derivatives. The remaining field/source factors can be at arbitrary other roots.

Thus every non-baseline term contains a block \(B\) with \(|B|\ge2\), supported on \(\{x_i=x_j:i,j\in B\}\). Different contact vertices use disjoint source-label blocks in the coefficient extraction. A \(C\) vertex differentiates its sources to total order at most four, and there are at most \(\lfloor m/2\rfloor\) such vertices. Higher \(R\) vertices add no spatial derivative. The total distribution order is therefore at most \(4\lfloor m/2\rfloor\le2m\).

All these derivatives annihilate \(F\in\mathcal S_0\) on the indicated partial diagonal. Finite cutoff sums and finite source order justify this termwise, without any coefficient bound. ∎

The statement is exact even if the contact coefficients diverge with the cutoff or grow rapidly with source order: on the required flat test space their contribution is identically zero at each order. Such growth could matter for an extension to non-flat Euclidean product tests, but no such extension is silently included in this theorem.

The one-field identity term \(c_a\), and the one-field matrix \(Z_a\), are excluded from this cancellation: they affect separated moments and remain inside the ultraviolet/operator estimates.

Point-local source derivatives and field support are different notions here. The field at root \(x\) uses neighboring links, but all external source slots of a higher local vertex are evaluated at \(x\). Its source contact is therefore exact, despite its larger gauge-variable carrier.

### 5. A coherent microscopic exclusion with a quantitative contact error

This section deals with a shrinking finite stencil, rather than an exact point contact. It supplies an additional way to remove microscopic overlapping insertions while retaining positivity.

#### 5.1 The finite source polynomial

Fix \(R>0\). Put an edge between distinct vertices \(x,y\) when their periodic Euclidean distance satisfies \(d_T(x,y)\le Ra\). Let \(\mathfrak I_{a,T,R}\) be the independent subsets of this finite graph. Define
\[
\mathcal G_{a,R}[j;U]=
\sum_{I\in\mathfrak I_{a,T,R}}
\prod_{x\in I}
\left[a^4\langle j(x),\Phi_a(x;U)\rangle\right].
\tag{5.1}
\]

This is one finite polynomial, with constant coefficient one, so all its source orders are compatible. Its \(m\)-th full source coefficient is
\[
S^{\mathrm{sep}}_{m,a,T}(F)
=a^{4m}\sum_X
\mathbf1_{\{d_T(x_i,x_j)>Ra\ \forall i<j\}}
\mathbb E_\mu\!\left[\prod_i\Phi_{\alpha_i,a}(x_i)\right]
F_{\boldsymbol\alpha}(X),
\tag{5.2}
\]
summed over component labels as usual. Repeated vertices are excluded. For example, any \(R>2\sqrt2\) excludes overlapping clover link supports.

For positive/negative source supports with a fixed time margin \(\delta\), their periodic separation is at least \(2\delta\), including the second reflection plane. Once \(Ra<2\delta\), no graph edge joins these supports. Every independent set therefore splits uniquely into its positive and negative parts:
\[
\mathcal G_{a,R}[j_-+j_+;U]
=\mathcal G_{a,R}[j_-;U]\mathcal G_{a,R}[j_+;U].
\tag{5.3}
\]
The graph is reflection and translation invariant, and the coefficients obey the tensor reflection rule. Equations (2.1) and (5.3) prove reflection positivity of the entire full hierarchy (5.2), on every fixed positive-time polynomial algebra for all sufficiently fine cutoffs. This is not an assertion that (5.1) is a probability Laplace transform.

For joint kernels the same statement is especially transparent: the mask for the combined reflected and positive test factors into the separate internal masks, because every cross-half pair has distance greater than \(Ra\). The OS form is the Wilson Gram form of the masked polynomial test vector.

Permutation symmetry, fine-lattice translations and the full hypercubic tensor covariance are exact. One can also apply the point-contact transformation (3.3) to this source polynomial; the same splitting proof and exact flat-test identity remain valid.

#### 5.2 The actual raw moment budget

Here \(\beta>0\), as on the admitted AF sequence.

Let \(X_x\) be the fixed set of plaquettes incident on \(x\), and let
\[
E_{X_x}=\beta\sum_{p\in X_x}s(U_p).
\]
The Wilson reserve gives
\[
\|E_{X_x}\|_{L^p(\mu)}\le C p,\qquad p\ge1,
\tag{5.4}
\]
uniformly along the admitted cofinal sequence. The number of covering cubes for \(X_x\) is a fixed geometric constant.

Equation (1.12) now gives
\[
\|\widetilde q_{\alpha,a}(x)\|_p
\le C a^{-4}\beta^{-1}p.
\tag{5.5}
\]

Suppose the prescribed one-field coefficients satisfy, for some fixed \(A,\zeta\ge0\),
\[
\boxed{
\beta^{-1}\max_\alpha\sum_\gamma|(Z_a)_{\alpha\gamma}|
+a^4\max_\alpha|(c_a)_\alpha|
\le A a^{-\zeta}.}
\tag{5.6}
\]
Then, with \(b=4+\zeta\),
\[
\|\Phi_{\alpha,a}(x)\|_p\le C A\,p\,a^{-b}.
\tag{5.7}
\]

The hypothesis includes fixed powers of logarithmic running after choosing any fixed positive \(\zeta\) and enlarging the constant. It is not inferred for an as-yet-unconstructed F0 normalization.

A completely specified unconditional instance is \(Z_a=\beta I\) and
\(c_a=\mathbb E_\mu[\beta\widetilde q_a(x)]\). Translation and hypercubic invariance make this vector independent of \(x\) and scalar. Equations (5.4)–(5.5) prove (5.6) with \(\zeta=0\) for that finite-cutoff family. This choice is not declared to be the final \(\mu\)-normalization or to have the prescribed Yang–Mills short-distance coefficients.

#### Theorem 5.1 — all-order vanishing of the microscopic collision strip

Assume (5.7), with fixed \(b,A\). Choose an integer
\[
q\ge\max\{6,\lceil b\rceil+2\}.
\]
Use the interior torus embedding in Section 6. There is a constant \(C\), independent of \(m,a,T\) along the sequence, such that for every coincidence-flat Schwartz test,
\[
\boxed{
\left|S^\Phi_{m,a,T}(F)-S^{\mathrm{sep}}_{m,a,T}(F)\right|
\le a\,C^{m+1}m!\,\nu_{qm}(F).
}
\tag{5.8}
\]
For \(m=0,1\) the difference is zero. The statement holds for every fixed \(R\), with \(C\) depending on \(R\). Point-contact transformations of Section 3 can be applied on either side without changing (5.8) on the flat test space.

**Proof.** Hölder with exponent \(m\) and (5.7) give
\[
\left|\mathbb E\prod_{i=1}^m\Phi_{\alpha_i,a}(x_i)\right|
\le (CA)^m m^m a^{-bm}
\le (eCA)^m m!a^{-bm}.
\tag{5.9}
\]
The difference in (5.8) is supported where at least one pair has periodic separation at most \(Ra\). Within the central embedding this is an ordinary Euclidean separation. Choose such a nearest pair, and let \(Y\) be the point obtained by replacing that pair by its midpoint. Then \(Y\in\Delta_m\), and \(V=X-Y\) satisfies
\[
\|V\|_1\le2Ra,\qquad |V|^2\le R^2a^2/2,\qquad Y\perp V.
\]
Take \(r_m=\lceil bm\rceil+1\). Since \(m\ge2\), the chosen \(q\) gives \(r_m\le qm\). Flatness and the directional Taylor remainder give
\[
|F(X)|\le
\frac{(2Ra)^{r_m}}{r_m!}
C_R^{qm/2}\nu_{qm}(F)
(1+|X|^2)^{-qm/2}.
\tag{5.10}
\]
Here the weight comparison along \(Y+tV\) follows from orthogonality:
\[
\frac{1+|X|^2}{1+|Y+tV|^2}
\le1+R^2a^2/2\le1+R^2/2
\]
for \(a\le1\). The power \(a^{-bm}\) in (5.9) leaves at least one power of \(a\) after multiplication by (5.10).

Finally,
\[
(1+\textstyle\sum_i|x_i|^2)^{-qm/2}
\le\prod_i(1+|x_i|^2)^{-q/2},
\]
and for \(q>4\),
\[
a^4\sum_{x\in a\mathbb Z^4}(1+|x|^2)^{-q/2}\le C_q.
\]
Thus the full lattice sum contributes at most \(C_q^m\). The \(21^m\) component sum is exponential and is absorbed into \(C^{m+1}\). The powers of \(R\) and the weight-comparison constant are likewise exponential in \(m\); the Taylor factorial need not even be used to improve the result.

The interior cutoff factors are kept bounded by one throughout this estimate; Taylor expansion is applied to \(F\), not to those factors. No derivative of the torus-embedding cutoff is taken. This proves (5.8). ∎

The theorem removes the entire microscopic collision strip with one fixed linear test order and one fixed factorial exponent. It is stronger than proving vanishing separately at each source order with arbitrary constants. It still says nothing about the separated correlation kernel outside that strip; the full observable/matching estimate remains necessary there.

### 6. Torus embeddings and continuum inheritance

#### 6.1 Avoiding the seam

Choose smooth cutoffs \(0\le\chi_T\le1\), invariant under \(H_4\), equal to one on a growing central box and supported in
\[
(-T/4,T/4)^4.
\]
For a joint test \(F_m\), use
\[
F_{m,T}(X)=\prod_{i=1}^m\chi_T(x_i)\,F_m(X)
\tag{6.1}
\]
in the lattice sums, with the ordinary central representatives of the torus sites. Every fixed compact test is unchanged for sufficiently large \(T\). On this support, each coordinate difference has absolute value less than \(T/2\), so periodic distance and ordinary Euclidean distance agree.

Consequently a periodic-near pair in Theorem 5.1 is genuinely near a Euclidean coincidence diagonal. Without this embedding, two points near opposite torus seams would not be controlled by coincidence-flat Taylor expansion alone. No extra relation between \(T\) and \(a^{-1}\) is used.

The products in (6.1) preserve flatness. Exact point contacts therefore vanish as in Theorem 4.1, including those with source derivatives. For (5.8), the proof uses only \(0\le\chi_T\le1\), so it incurs no derivative-order or factorial cost from the embedding.

#### 6.2 Translation covariance of any controlled limit

Let a subsequence of one of these hierarchies converge on \(\mathcal S_0\), with the common Schwartz seminorm bounds required by S0. For a compact test \(F\) and a fixed translation \(b\in\mathbb R^4\), choose \(b_a\in a\mathbb Z^4\) with \(b_a\to b\). Once the original and translated supports lie where \(\chi_T=1\), exact lattice translation covariance gives
\[
S_{m,a,T}(\tau_{b_a}F)=S_{m,a,T}(F).
\tag{6.2}
\]
Continuity of translations in the common Schwartz seminorm gives
\[
S_{m,a,T}(\tau_bF-\tau_{b_a}F)\longrightarrow0.
\]
Pass to the limit and then approximate a general flat Schwartz test by compact flat tests. The limit is translation covariant. Thus no separate physical-cell-grid translation defect remains in this specified hierarchy.

The common seminorm bound is part of the still-open S0 estimate. This section proves the symmetry implication once that estimate is available; it does not derive S0 from positivity.

#### 6.3 Positivity and the finite symmetry group in the limit

First take a finite OS vector of compact coincidence-flat kernels supported strictly inside positive time. There is then a common positive support margin. Its combined reflected test kernels are still coincidence-flat: internal collisions are killed by flatness, and cross-half collisions are excluded by that margin. For all sufficiently fine lattices and large tori, the stencil and, if used, the exclusion graph fit the margin. Equations (2.5), (3.7) or (5.3) give nonnegative cutoff OS forms. Their finite sums of convergent Schwinger evaluations have a nonnegative limit.

A general positive-time Schwartz kernel need not have a strictly positive support margin. Approximate it by multiplying by a compact cutoff and by smooth cutoffs that vanish near every time boundary. A smooth function supported in the closed positive-time region is flat at those boundaries; its weighted derivatives therefore make this approximation converge in each required Schwartz seminorm. Multiplication by these cutoffs also preserves coincidence-flatness. The assumed common S0 bound makes the finite OS quadratic form continuous in this approximation. Its nonnegativity extends to the full positive-time Schwartz algebra. This step uses the separately required S0 estimate; it does not assert uniform cutoff positivity for tests whose stencils cross the reflection plane.

Permutation symmetry and the full signed-permutation tensor covariance pass directly. The correct Wick phases are fixed once, before taking the limit. Full continuous rotations remain a separate defect theorem; no rotation average is performed.

The exact source-free positive transports may be used to calculate these cutoff moments. Since they preserve every marked integral, their fixed cell grids and selectors do not change the symmetry identities of the original hierarchy. They need not themselves form a reflection-positive random process.

### 7. Completion conditions for P0 and F0

| Statement | Status |
|---|---|
| Explicit actual 21-component Wilson fields | P: vertex clovers with the scalar trace replaced by the exact Wilson action density |
| Exact one-field gauge covariance, translations and hypercubic tensor transformations | P |
| Reflection positivity of the full finite-cutoff moment hierarchy | P on every fixed positive-time test algebra once its support margin fits the stencil |
| Running equivariant one-field mixing and scalar identity subtraction preserve these properties | P for arbitrary finite coefficients at each cutoff |
| Compatible local source jets at every order | P: one formal functional and its composition law |
| Exact partial-diagonal support and vanishing on the corrected OS test space | P; no contact-coefficient norm is needed for exact point contacts |
| Microscopic finite-stencil collision removal with fixed factorial/linear-order bounds | P under (5.6), and instantiated unconditionally for the stated energy-normalized vacuum-centered cutoff family |
| Positivity, translations and the finite tensor symmetry group of a controlled continuum limit | P implication using the separately required convergence/OS seminorm bound |
| The ultraviolet renormalization coefficients of the actual RG induction belong to this architecture and meet the prescribed \(\mu\)-conditions | O: this is F0/M0, not proved by the algebra |
| Current-scale transported-field bounds, full history control and the off-diagonal hierarchy | O |
| Full \(O(4)\) restoration, quantitative AF identification and phase/operator control | O |

P0 is realized by one concrete definition on the actual Wilson measure. It is unnecessary to leave reflection positivity as an unspecified property of a future global source normal form. The remaining F0 problem is to prove that the normalization and local extractions required by the observable induction can be implemented in this explicit class, with their errors controlled. Point-contact positivity itself then requires no additional estimate.

### Source and proof dependencies

The compact Wilson action and the reduced finite tensor target are those of the main paper. The exact source-free transport interpretation and the coincidence-flat OS test space are proved or scoped in the other annexes. The uniform raw energy reserve used only in Section 5.2 is the theorem of Annex A, with its cofinal geometric condition retained.

The site-reflection square formula, explicit field covariance, Wilson scalar identity, formal source composition, partial-diagonal statement and finite-stencil positivity/error theorem are proved in this note. No unproved observable theorem, phase decomposition or unpublished Yang–Mills construction is imported.


---
