# Wilson tensor witnesses and large-field suppression

## 2. an explicit local Wilson-compatible tensor family

### 2.1 Based clover curvature

For a signed coordinate unit vector \(u\), write \(U_u(z)\) for the link from \(z\) to \(z+au\), with reversed links represented by inverses. For perpendicular signed coordinate vectors \(u,v\), define the based plaquette
\[
P_{u,v}(z)=U_u(z)U_v(z+au)U_{-u}(z+au+av)U_{-v}(z+av).
\tag{2.1}
\]
It follows the loop \(u,v,-u,-v\). Reversal gives \(P_{v,u}(z)=P_{u,v}(z)^{-1}\).

For a unitary matrix \(P\), set
\[
H(P)=\pi_0\frac{P-P^\dagger}{2i},\qquad
\pi_0 X=X-\frac{\operatorname{Tr}X}{N}I_N.
\]
The projection \(\pi_0\) acts on Hermitian matrices. It is orthogonal for the real Hilbert inner product \(\operatorname{Tr}(XY)\). Define
\[
F^C(u,v;z)=\frac1{4a^2}
\sum_{\epsilon,\delta=\pm1}\epsilon\delta\,
H(P_{\epsilon u,\delta v}(z)).
\tag{2.2}
\]
Let \(A=(\mu,\nu)\), \(\mu<\nu\), range over the six independent coordinate planes, and write \(F_A^C=F^C(e_\mu,e_\nu)\). Each \(F_A^C\) is traceless Hermitian. Changing summation signs and reversing loops proves the exact identities
\[
F^C(-u,v)=-F^C(u,v),\qquad F^C(v,u)=-F^C(u,v).
\tag{2.3}
\]

Let \(\bar s_A(z)\) be the average deficit of the four plaquettes in plane \(A\) incident on \(z\):
\[
\bar s_A(z)=\frac14\sum_{\epsilon,\delta=\pm1}
s(P_{\epsilon e_\mu,\delta e_\nu}(z)).
\tag{2.4}
\]
Reversal and cyclic rebasing leave the deficit unchanged, so these are ordinary Wilson plaquette deficits.

### 2.2 Pointwise domination by the Wilson action

If the eigenvalues of \(P\) are \(e^{i\theta_j}\), then
\[
\|H(P)\|_{\rm HS}^2
\le\sum_j\sin^2\theta_j
\le2\sum_j(1-\cos\theta_j)=2s(P).
\tag{2.5}
\]
Convexity of the squared Hilbert norm applied to (2.2) yields
\[
\operatorname{Tr}(F_A^C(z)^2)\le2a^{-4}\bar s_A(z).
\tag{2.6}
\]
Define the real symmetric Gram matrix, its trace, and the symmetrized Wilson scalar by
\[
Q^C_{AB}(z)=\operatorname{Tr}(F_A^C(z)F_B^C(z)),\qquad
q_C(z)=\sum_AQ^C_{AA}(z),\qquad
q_W(z)=2a^{-4}\sum_A\bar s_A(z).
\tag{2.7}
\]
Thus
\[
Q^C(z)\succeq0,\qquad 0\le q_C(z)\le q_W(z)\le24N a^{-4}.
\tag{2.8}
\]
The notation \(\succeq0\) denotes positivity of the ordinary \(6\times6\) matrix of random variables at each configuration. It is distinct from reflection positivity.

### 2.3 The scalar-corrected multiplet

**Theorem 1.** The 21 independent entries of
\[
\boxed{Q^W_{AB}(z)=Q^C_{AB}(z)+\frac{\delta_{AB}}6\,[q_W(z)-q_C(z)]}
\tag{2.9}
\]
form a real, gauge-invariant, local lattice tensor family with the following exact properties:
\[
Q^W(z)\succeq0,\qquad \operatorname{tr}_6Q^W(z)=q_W(z),
\qquad |Q^W_{AB}(z)|\le q_W(z)\le24Na^{-4},
\tag{2.10}
\]
\[
\boxed{a^4\sum_zq_W(z)=2S.}
\tag{2.11}
\]
The family transforms as \(\operatorname{Sym}^2(\Lambda^2\mathbb R^4)\) under every signed coordinate permutation. It has the corresponding tensor reflection action and a stencil of radius at most \(\sqrt2a\).

**Proof.** Equation (2.8) makes the correction in (2.9) a nonnegative multiple of \(I_6\), proving matrix positivity. Its trace is \(q_W\). The operator norm of a positive matrix is at most its trace, proving the entry bounds. Each ordinary plaquette is counted at its four corners in (2.4), with weight \(1/4\) at each; this proves (2.11).

Every based loop transforms by conjugation at its base under a gauge transformation. Both \(H\) and \(\pi_0\) commute with unitary conjugation. Therefore \(F^C\) transforms by conjugation and its traced bilinears are gauge invariant. The deficit is gauge invariant as well.

A signed coordinate permutation \(R\) sends a based geometric loop to its image. Equations (2.2)–(2.3) imply the two-form transformation \(F^C\mapsto(\Lambda^2R)F^C\). Consequently \(Q^C\mapsto(\Lambda^2R)Q^C(\Lambda^2R)^T\). Both \(q_C\) and \(q_W\) are scalars, and \(I_6\) is invariant, proving the claim for \(Q^W\). The correction changes only the scalar representation; all six nonscalar hypercubic channels in [C1, Part III] are retained.

All loop vertices lie in \(z+[-a,a]^4\), at distance at most \(\sqrt2a\) from \(z\). This proves the support claim. Finally, traces of products of two Hermitian matrices are real because conjugation reverses the factors and cyclicity restores their order. This proves reality. \(\square\)

For time reflection \(\theta\), the tensor action is explicitly
\[
Q^W_{\mu\nu,\rho\sigma}(z)\mapsto
(-1)^{\#\{\text{time indices in }\mu,\nu,\rho,\sigma\}}
Q^W_{\mu\nu,\rho\sigma}(\theta z).
\tag{2.12}
\]
The OS involution also conjugates scalar test coefficients. A polynomial in fields whose stencils remain inside a positive-time half is an actual element of the Wilson positive-time algebra. The finite-cutoff reflection positivity proved in Section 3.2 therefore applies to it.

### 2.4 Exact scalar normalization and a local source

The earlier one-corner density \(q_a=a^{-4}\sum_A s_A\) integrates to \(S\). The present \(q_W\) is twice its local four-corner average. Accordingly,
\[
2Nx_0S=Nx_0 a^4\sum_zq_W(z).
\tag{2.13}
\]
For a scalar source \(j\),
\[
a^4\sum_z j(z)q_W(z)=2\sum_p\bar j_p s_p,
\qquad \bar j_p=\frac14\sum_{z\text{ a corner of }p}j(z).
\tag{2.14}
\]
Thus the local coefficient becomes \(\beta_p=\beta-2\bar j_p\), or \(x_{0,p}=x_0-\bar j_p/N\). This is an exact finite-lattice identity with the source normalization fixed; it makes no assertion about a cutoff-uniform finite-source analytic functional.

### 2.5 A symmetry-preserving centered family

Coordinate sign flips give distinct characters to the six coordinate two-forms. Invariance of the full Wilson law under these flips forces \(\mathbb E Q^W_{AB}=0\) for \(A\ne B\). Coordinate permutations equate the six diagonal expectations. Hence
\[
\mathbb E Q^W_{AB}(z)=\frac{\mathbb E q_W(z)}6\delta_{AB}.
\]
The concrete centered fields
\[
\boxed{\Phi_{AB}(z)=Q^W_{AB}(z)-\frac{\mathbb E q_W(z)}6\delta_{AB}}
\tag{2.15}
\]
have zero one-point functions, preserve all stated lattice symmetries, and satisfy
\[
|\Phi_{AB}(z)|\le28Na^{-4}.
\tag{2.16}
\]
The centering number may depend on the chosen cutoff, coupling and torus. It is deterministic, so it does not enlarge the configuration support of the observable. Centered polynomials remain in the same positive-time algebra. This supplies a definite finite-sequence one-point normalization; matching a prescribed continuum renormalization scheme remains a separate task.

The collision-strip theorem of [C1, Part III, L.1] now applies to actual centered fields with \(D=4\). For \(0<\eta<1\), \(m\ge2\), and coincidence-flat Schwartz \(F\), their full-moment contribution from \(r_m\le a^\eta\) obeys
\[
|E_{m,a}(F)|\le C^{m+1}a^\eta\nu_{qm}(F),
\qquad q>\max\{4,4/\eta+2\},
\tag{2.17}
\]
on the same central torus lift used there. This is an unconditional application to the bare centered family. A later mixing matrix \(Z_a\) must still have its cutoff growth controlled before the same statement is applied to the physically renormalized fields.

### 2.6 Smooth classical consistency

Take links to be parallel transports of a fixed smooth Hermitian traceless connection, with curvature convention \(P_{e_\mu,e_\nu}=I+ia^2F_{\mu\nu}+O(a^3)\). To expand a rectangle, choose radial gauge about its base point: the connection vanishes there and is \(O(a)\) on the rectangle. Higher holonomy terms are then \(O(a^4)\), as is the integrated commutator correction between ordinary exterior differentiation and curvature. Ordinary componentwise Stokes and Taylor expansion about the rectangle centroid give the terms through order \(a^3\). Restoring gauge covariance yields
\[
H(P_{\epsilon e_\mu,\delta e_\nu}(z))
=\epsilon\delta a^2\left[F_{\mu\nu}(z)+
\frac a2(\epsilon D_\mu+\delta D_\nu)F_{\mu\nu}(z)\right]+O(a^4).
\]
The signed average cancels the first derivative terms, so \(F_A^C=F_A+O(a^2)\). Similarly,
\[
\bar s_A=\frac{a^4}{2}\operatorname{Tr}F_A^2+O(a^6),
\qquad q_W=\sum_A\operatorname{Tr}F_A^2+O(a^2).
\]
It follows that
\[
Q^W_{AB}=\operatorname{Tr}(F_AF_B)+O(a^2).
\tag{2.18}
\]
For \(\operatorname{Tr}T^aT^b=\delta^{ab}/2\), this scalar is \(\frac14\sum_{a,\mu,\nu}(F^a_{\mu\nu})^2\). These are classical consistency statements for fixed smooth connections. Their remainders depend on smooth connection norms and do not justify discarding the scalar correction on random rough fields.

## 3. full-law moments and microscopic large-field suppression

### 3.1 A volume-uniform partition estimate

Choose \(r_0\in(0,1]\) and \(c_G>0\) so that
\[
\operatorname{Haar}\{U:\|U-I\|_{\rm HS}\le r\}\ge c_Gr^{d_G},
\qquad 0<r\le r_0,\qquad c_Gr_0^{d_G}\le1.
\]
These constants exist in an exponential chart at the identity: the Haar density is continuous and positive there, and \(\|e^X-I\|_{\rm HS}\le\|X\|_{\rm HS}\) for skew-Hermitian \(X\). Set
\[
C_0=48r_0^2-4\log(c_Gr_0^{d_G}),\qquad
K_\beta=1+C_0+2d_G\log\beta\ge1.
\tag{3.1}
\]

Restrict every link to the ball of radius \(r_0\beta^{-1/2}\). Telescoping a product of unitary matrices gives
\[
\|U_p-I\|_{\rm HS}\le4r_0\beta^{-1/2},\qquad
s_p\le8r_0^2/\beta.
\]
There are \(6V\) plaquettes and \(4V\) independent links. Integrating over this set therefore proves
\[
\boxed{e^{-(K_\beta-1)V}\le Z(\beta)\le1.}
\tag{3.2}
\]
This lower-bound integration is only a method of estimating the partition function; the probability measure in every following result remains the complete law (1.1).

Relative entropy with respect to normalized product Haar measure is
\[
0\le D(\mu_\beta\Vert\nu)=-\beta\mathbb E S-\log Z(\beta).
\]
All plaquettes are equidistributed on the isotropic cubic torus. Thus
\[
\mathbb E s_p\le\frac{K_\beta-1}{6\beta},\qquad
\mathbb E q_W(z)\le\frac{2(K_\beta-1)}{\beta a^4}.
\tag{3.3}
\]
The logarithm in \(K_\beta\) is part of the proved estimate; an \(O(1/\beta)\) bound without that logarithm has not been asserted.

### 3.2 Site-plane reflection positivity

Reflect the even torus through the two site planes \(z_i=j\) and \(z_i=j+n/2\), in lattice units. Let \(U_0\) denote tangential links lying in these planes, and \(U_+,U_-\) the remaining links in the respective closed halves. A unit plaquette cannot involve variables from both open halves. Consequently,
\[
S=S_+(U_+,U_0)+S_-(U_-,U_0)+S_0(U_0),\qquad S_-=\theta S_+.
\]
Reflection preserves Haar measure and fixes the boundary tangential links. Conditional on them, the two open-half integrations factor. For any bounded function \(F\) of the positive closed half,
\[
\mathbb E[(\Theta F)F]=Z(\beta)^{-1}
\int e^{-\beta S_0(U_0)}
\left|\int F(U_+,U_0)e^{-\beta S_+(U_+,U_0)}dU_+\right|^2dU_0\ge0,
\tag{3.4}
\]
where \(\Theta F=\overline{F\circ\theta}\). The associated Cauchy–Schwarz inequality follows. Functions of neighboring closed cubes may share boundary links; (3.4) allows precisely this overlap.

### 3.3 Chessboard estimate without a power-of-two assumption

Let \(C_z=z+[0,1]^4\) be the closed unit cubes of the periodic cell complex. Suppose \(F_z\) are bounded nonnegative cube functions mapped into one another by coordinate reflections through cube boundaries. For every set \(A\) of distinct cubes,
\[
\boxed{\mathbb E\prod_{z\in A}F_z
\le\left(\mathbb E\prod_{z\in\Lambda}F_z\right)^{|A|/V}.}
\tag{3.5}
\]

**Proof.** First assume strict positivity. Put
\(m_F=(\mathbb E\prod_zF_z)^{1/V}\) and \(f_z=F_z/m_F\). For each binary pattern \(\varepsilon\), define
\(Z(\varepsilon)=\mathbb E\prod_z f_z^{\varepsilon_z}\).
Both constant patterns have value one. Choose a pattern maximizing \(Z\), and among maximizers choose one minimizing the number of disagreeing nearest-neighbor labels. Let its value be \(M\ge1\).

If it is nonconstant, an adjacent unequal pair exists. Cut through its common face and the opposite face of the torus. Reflect the positive half-pattern onto the negative half to get \(\varepsilon^+\), and conversely get \(\varepsilon^-\). Reflection Cauchy–Schwarz gives
\[
M^2\le Z(\varepsilon^+)Z(\varepsilon^-)\le M^2.
\]
Both reflected patterns are therefore maximizers. If \(D\) counts original disagreements and \(D_{\rm cut}>0\) counts those across the two interfaces, the two reflected disagreement counts satisfy
\[
D(\varepsilon^+)+D(\varepsilon^-)=2(D-D_{\rm cut})<2D.
\]
Internal disagreements are duplicated, while the labels on each reflected interface match. One reflected maximizer has fewer disagreements, a contradiction. The maximizing pattern is constant, hence \(M=1\). Applying this to the indicator of \(A\) gives (3.5). General nonnegative functions follow by adding a positive constant and taking a limit. \(\square\)

Only evenness was used to form the opposite site plane. No repeated halving or dyadic torus assumption is present.

### 3.4 A joint exponential bound on local cube energies

Define
\[
E_z=\sum_{p\subset C_z}s_p.
\tag{3.6}
\]
A four-dimensional cube has 24 square faces; each plaquette belongs to four cubes. Therefore \(\sum_zE_z=4S\).

**Theorem 2.** For every set \(A\) of distinct cubes,
\[
\boxed{\mathbb E\exp\left(\frac\beta8\sum_{z\in A}E_z\right)
\le e^{(K_\beta-1)|A|}\le e^{K_\beta|A|}.}
\tag{3.7}
\]
In particular, for thresholds \(u_z\ge0\),
\[
\mu_\beta\left(\bigcap_{z\in A}\{E_z\ge u_z\}\right)
\le\min\left\{1,\exp\left[K_\beta|A|-\frac\beta8\sum_{z\in A}u_z\right]\right\}.
\tag{3.8}
\]

**Proof.** Use (3.5) with \(F_z=e^{\beta E_z/8}\). Full dissemination gives the exact identity
\[
\mathbb E\prod_zF_z=\mathbb E e^{\beta S/2}
=\frac{Z(\beta/2)}{Z(\beta)}\le e^{(K_\beta-1)V}.
\]
The upper bound \(Z(\beta/2)\le1\) holds even when \(\beta/2<1\). Equation (3.7) follows, and exponential Markov inequality gives (3.8). \(\square\)

The theorem concerns the full positive Wilson law. No independence of neighboring cubes, no regular-background restriction, and no perturbative approximation is used.

### 3.5 All local moments and a uniform exponential envelope

Equation (3.8) gives
\[
\mu_\beta\left(E_z>\frac8\beta(K_\beta+t)\right)\le e^{-t},\qquad t\ge0.
\]
For each integer \(m\ge1\), the positive part of \(\beta E_z/8-K_\beta\) therefore has \(m\)-th moment at most \(m!\). Minkowski's inequality and \((m!)^{1/m}\le m\) give
\[
\|s_p\|_m\le\|E_z\|_m\le\frac8\beta(K_\beta+m),\qquad p\subset C_z.
\tag{3.9}
\]
Since \(q_W(z)=\frac1{2a^4}\sum_{p\ni z}s_p\), with 24 incident plaquettes,
\[
\boxed{\|Q^W_{AB}(z)\|_m\le\|q_W(z)\|_m
\le\frac{96(K_\beta+m)}{\beta a^4}.}
\tag{3.10}
\]
The exact centering (2.15) improves the simple factor-two centered estimate to
\[
\|\Phi_{AB}(z)\|_m\le14a^{-4}\|s_p\|_m
\le\frac{112(K_\beta+m)}{\beta a^4}.
\tag{3.11}
\]
For clover curvature itself, (2.6) and convexity yield
\[
\mathbb E\|F_A^C(z)\|_{\rm HS}^{2m}
\le(2a^{-4})^m\mathbb E s_p^m,
\qquad
\mathbb E\|F_A^C(z)\|_{\rm HS}^{2}
\le\frac{K_\beta-1}{3\beta a^4}.
\tag{3.12}
\]

Concavity of \(t\mapsto t^{1/K_\beta}\), followed by convexity for the average of 24 plaquette deficits, also gives
\[
\boxed{\mathbb E\exp\left(\frac{\beta a^4}{96K_\beta}q_W(z)\right)\le e.}
\tag{3.13}
\]
Set
\[
\sigma_{\beta,a}=\frac{96K_\beta}{\beta a^4}.
\tag{3.14}
\]
Then \(\mathbb E q_W^m\le e\,m!\sigma_{\beta,a}^m\). This is a fixed factorial budget, with its cutoff and coupling dependence explicit.

The centered family also has one common positive envelope. Put
\[
R_a(z)=q_W(z)+\frac{\mathbb E q_W(z)}6,
\qquad \sigma^\circ_{\beta,a}=\frac76\sigma_{\beta,a}
=\frac{112K_\beta}{\beta a^4}.
\]
Then
\[
\boxed{\max_{A,B}|\Phi_{AB}(z)|\le R_a(z),\qquad
\mathbb E e^{R_a(z)/\sigma^\circ_{\beta,a}}\le e.}
\tag{3.14a}
\]
Indeed Jensen gives \(\mathbb E q_W\le\sigma_{\beta,a}\). The deterministic term contributes at most \(e^{1/7}\), while concavity bounds the remaining expectation by \((\mathbb E e^{q_W/\sigma_{\beta,a}})^{6/7}\le e^{6/7}\).

### 3.6 Connected microscopic large-field sets, including inserted marks

Declare a cube bad when \(E_z\ge u\). For a prescribed set \(\Gamma\), let \(B_\Gamma\) mean that all its cubes are bad, and set
\[
\kappa=\frac{\beta u}{8}-K_\beta>0.
\]
Equation (3.8) gives \(\mu_\beta(B_\Gamma)\le e^{-\kappa|\Gamma|}\).

Face adjacency gives a cube graph of degree eight. A connected set of \(k\) cubes containing a fixed root can be encoded by the depth-first traversal of a canonically selected spanning tree. That traversal has \(2(k-1)\) steps and determines the visited set. There are at most \(8^{2(k-1)}=64^{k-1}\) such sets. If the root's bad component \(\mathcal C\) has size at least \(k\), it contains one such set of size exactly \(k\). Consequently,
\[
\mu_\beta(|\mathcal C|\ge k)\le64^{k-1}e^{-\kappa k}.
\]
The choice
\[
\boxed{u=\frac8\beta(K_\beta+\log64+t),\qquad t>0}
\quad\Longrightarrow\quad
\boxed{\mu_\beta(|\mathcal C|\ge k)\le e^{-tk}}
\tag{3.15}
\]
is uniform in the torus. A threshold larger than the maximum cube energy simply makes the bad event empty.

The bound survives insertions. For arbitrary sites, including coincidences, and arbitrary tensor entries,
\[
\boxed{\mathbb E\left[\prod_{i=1}^m|Q^W_{A_iB_i}(z_i)|\,\mathbf1_{B_\Gamma}\right]
\le\left[\frac{96(K_\beta+2m)}{\beta a^4}\right]^m
e^{-\kappa|\Gamma|/2}.}
\tag{3.16}
\]
Indeed, Cauchy–Schwarz separates the indicator, and Hölder bounds the remaining factor by \(\prod_i\|Q_i^W\|_{2m}\). Equation (3.11) gives the same centered bound with 112 in place of 96.

This proves marked suppression for actual microscopic Wilson large-field sets. Identifying the scale-dependent Balaban R carriers with controlled events requires an additional argument; they are not silently identified with \(B_\Gamma\).

## 4. Exact consequences for the observable route

### 4.1 Full-law moment and cumulant growth at every order

Hölder and (3.13) show, for arbitrary \(m\) sites and tensor labels,
\[
\left|\mathbb E\prod_{i=1}^m Q_i^W\right|
\le e\,m!\sigma_{\beta,a}^m.
\tag{4.1}
\]
For a partition \(\pi\) into \(k\) blocks, the cumulant formula has coefficient \((k-1)!\). The exact weighted partition count is
\[
\sum_{\substack{\pi\in\Pi_m\\|\pi|=k}}\prod_{B\in\pi}|B|!
=\frac{m!}{k!}\binom{m-1}{k-1}.
\]
To see this, order the blocks, choose their positive sizes, and assign the \(m\) distinct labels. The product of the block factorials cancels the multinomial denominators; divide by \(k!\) for unordered blocks. Inserting (4.1) gives
\[
\boxed{|\kappa_m(Q_1^W,\ldots,Q_m^W)|
\le(m-1)![(1+e)^m-1]\sigma_{\beta,a}^m.}
\tag{4.2}
\]
Here \(\sum_{k=1}^m e^k\binom{m-1}{k-1}/k=[(1+e)^m-1]/m\).
Deterministic centering does not change connected orders \(m\ge2\). Thus the initial full-law cumulants have factorial exponent one. This conclusion concerns their microscopic size; it supplies no separated-point decay.

### 4.2 The envelope survives every exact positive transport step

Use the route's normalized positive transports \(\mathcal Q_k\), with
\[
\mathcal Q_k1=1,\qquad
\int\mathcal Q_k f\,d\mu_{k+1}=\int f\,d\mu_k,
\]
and their conditional-expectation interpretation [OR, Section 3]. Start at \(\mu_0=\mu_\beta\), and transport matrix entries and their trace:
\[
Q_{k+1}^W(z)=\mathcal Q_k Q_k^W(z),\qquad
q_{k+1}(z)=\mathcal Q_kq_k(z),\qquad q_0=q_W.
\]
Positivity preserves the finite-dimensional matrix cone: \(v^TQ_{k+1}^Wv=\mathcal Q_k(v^TQ_k^Wv)\ge0\), first simultaneously for the countable set of rational vectors and then for every vector by continuity. The trace identity is linear. Therefore
\[
Q_k^W\succeq0,\qquad \operatorname{tr}_6Q_k^W=q_k,
\qquad |Q_{k,AB}^W|\le q_k.
\]
Conditional Jensen and preservation of expectations give
\[
\boxed{\int e^{q_k(z)/\sigma_{\beta,a}}d\mu_k\le e,\qquad
\|Q_{k,AB}^W(z)\|_m\le\frac{96(K_\beta+m)}{\beta a^4}.}
\tag{4.3}
\]
The centered version contracts in \(L^m\) and retains (3.11). Transporting the common positive envelope \(R_a\) also preserves (3.14a). The constants contain no factor depending on \(k\). These arguments use each valid positive joint law separately, so nested sigma-algebras are unnecessary. They apply before replacing positive histories by a signed polymer expansion.

For the large-field indicator, define \(b_0=\mathbf1_{B_\Gamma}\) and \(b_{k+1}=\mathcal Q_kb_k\). Then \(0\le b_k\le1\), \(\int b_k=\mu_\beta(B_\Gamma)\), and \(\|b_k\|_2\le\mu_\beta(B_\Gamma)^{1/2}\). The proof of (3.16) gives
\[
\int\prod_{i=1}^m|Q^W_{k,A_iB_i}(z_i)|\,b_k\,d\mu_k
\le\left[\frac{96(K_\beta+2m)}{\beta a^4}\right]^m
e^{-\kappa|\Gamma|/2}.
\tag{4.4}
\]
Here \(b_k\) is the transported probability of the original event, not an indicator newly defined at a coarser scale.

### 4.3 A depth-independent absolute covariance budget

Let \(F_{k+1}=\mathcal Q_kF_k\) and \(G_{k+1}=\mathcal Q_kG_k\) for real square-integrable marks. Define the actual covariance shell
\[
D_k^{FG}=\mathcal Q_k(F_kG_k)-F_{k+1}G_{k+1}.
\]
Then for every finite terminal depth \(J\),
\[
\boxed{\sum_{k=0}^{J-1}\mathbb E_{\mu_{k+1}}|D_k^{FG}|
+|\operatorname{Cov}_{\mu_J}(F_J,G_J)|
\le\sqrt{\operatorname{Var}_{\mu_0}F_0\operatorname{Var}_{\mu_0}G_0}.}
\tag{4.5}
\]

**Proof.** Conditional Cauchy–Schwarz gives
\(|D_k^{FG}|\le\sqrt{D_k^{FF}D_k^{GG}}\), with both diagonal terms nonnegative. Set \(v_k^F=\mathbb E D_k^{FF}\), and append \(v_J^F=\operatorname{Var}F_J\). The exact variance telescope gives \(\sum_{k=0}^Jv_k^F=\operatorname{Var}F_0\), and similarly for \(G\). Cauchy–Schwarz first in probability and then across the finite list of shells, including the terminal variances, proves (4.5). \(\square\)

For any two centered fields (2.15), the right side is at most
\[
\left[\frac{112(K_\beta+2)}{\beta a^4}\right]^2.
\tag{4.6}
\]
This is an absolute shell budget for the actual positive transports, including their terminal contribution. It neither relies on cancellation of shell signs nor loses a factor of \(J\). Its \(a^{-8}\) size does not yet give the required separated-point continuum estimate.

### 4.4 Integrability of all transported logarithmic jets

This conclusion is about the actual finite jets in the frozen-transport algebra, rather than only products of transported first-degree marks. Let \(T_k=\mathcal Q_{k-1}\cdots\mathcal Q_0\). Take initial bare entries \(F_i=Q^W_{A_iB_i}(z_i)\), or their centered versions. More generally, the same proof applies to the exponential-moment hypothesis stated below. Use distinct formal labels and set
\[
G_k(t)=T_k\exp\left(\sum_{i=1}^m t_iF_i\right),\qquad
\Psi_k(t)=\log G_k(t),
\]
with only the finite Taylor jet retained. Since \(T_k1=1\), the coefficient of \(t_1\cdots t_m\) in \(\Psi_k\) is
\[
\Psi_k^{[m]}=\sum_{\pi\in\Pi_m}(-1)^{|\pi|-1}(|\pi|-1)!
\prod_{B\in\pi}T_k\left(\prod_{i\in B}F_i\right).
\tag{4.7}
\]
Conditional Hölder, including a factor of 1 when a block has fewer than \(m\) labels, implies for every partition
\[
\prod_{B\in\pi}\left|T_k\prod_{i\in B}F_i\right|
\le\prod_{i=1}^m(T_k|F_i|^m)^{1/m}.
\]
Outer Hölder and preservation of expectations bound its integral by \(\prod_i\|F_i\|_m\). Also
\[
\sum_{\pi\in\Pi_m}(|\pi|-1)!
\le\sum_{r=1}^m r!S(m,r)\le2^{m-1}m!.
\]
Here \(S(m,r)\) counts partitions into \(r\) blocks. For each positive ordered composition \(n_1+\cdots+n_r=m\), the number of ordered partitions of those sizes is \(m!/(n_1!\cdots n_r!)\le m!\). There are \(\binom{m-1}{r-1}\) such compositions, whose sum over \(r\) is \(2^{m-1}\). If \(\mathbb E e^{|F_i|/\sigma_i}\le e\), the product of the \(m\)-th moment norms is at most \(e\,m!\prod_i\sigma_i\). Consequently,
\[
\boxed{\|\Psi_k^{[m]}\|_{L^1(\mu_k)}
\le e\,2^{m-1}(m!)^2\prod_{i=1}^m\sigma_i.}
\tag{4.8}
\]
For bare entries take every \(\sigma_i=\sigma_{\beta,a}\); for the centered entries use \(\sigma_i=\sigma^\circ_{\beta,a}\) from (3.14a). This is uniform in transport depth, sites and labels. It requires no uniform complex-source neighborhood or zero-free region. The factorial exponent two bounds absolute conditional coefficients, whereas (4.2) bounds full-law initial cumulants with exponent one.

Equation (4.8) controls each whole assembled finite jet. It does not bound the sum of the absolute values of the terms in a subsequent signed polymer or localization expansion. Additional nonlinear source counterterms, if a later normalization scheme introduces them, must be included and estimated in the initial jet.
