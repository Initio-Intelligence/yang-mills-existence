# Finite tensor mixing and rotation constraints

**Annex D.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


**Status: (P), finite-dimensional algebra.** This classifies the one-field, dimension-four curvature-bilinear mixing problem. It does not prove rotation restoration of any Schwinger function, determine an RG coefficient, or control contact/derivative remainders.

Let \(V=\mathbb R^4\), \(E=\operatorname{Sym}^2(\Lambda^2 V)\), and \(H_4=(\mathbb Z_2)^4\rtimes S_4\), the full signed-permutation group including reflections. Use formal bilinears \(Q_{ij,kl}=\operatorname{Tr}(F_{ij}F_{kl})\); they are antisymmetric within each pair and symmetric between the pairs. The invariant color quadratic form is fixed. There are 21 independent tensor labels.

### 1. Decomposition under coordinate sign changes

For \(d=\operatorname{diag}(\epsilon_1,\ldots,\epsilon_4)\),

\[
dQ_{ij,kl}=\epsilon_i\epsilon_j\epsilon_k\epsilon_lQ_{ij,kl}.
\]

The sign characters split \(E\) into three invariant types:

1. The six squares \(Q_{ij,ij}\), with trivial sign character.
2. The twelve shared-index bilinears. For each unordered pair \(\{i,j\}\), there are two terms \(Q_{ik,jk}\), where \(k\notin\{i,j\}\), both with character \(\epsilon_i\epsilon_j\).
3. The three disjoint-index terms, all with character \(\epsilon_1\epsilon_2\epsilon_3\epsilon_4\).

Normality of the sign subgroup forces any equivariant endomorphism to preserve these isotypic pieces.

### 2. The seven irreducible summands

#### The six square terms: dimensions 1, 3 and 2

Their permutation representation is the action of \(S_4\) on the edges of a tetrahedron. It decomposes as follows:

- Scalar: \(S=\sum_{i<j}Q_{ij,ij}\), dimension one.
- Diagonal traceless Ricci: coefficients \(q_{ij}=r_i+r_j\), with \(\sum_i r_i=0\), dimension three.
- Diagonal Weyl: \(\sum_{j\ne i}q_{ij}=0\) for every \(i\), dimension two.

The last space consists of

\[
q_{12}=q_{34}=x,\quad q_{13}=q_{24}=y,\quad
q_{14}=q_{23}=z,\quad x+y+z=0.
\]

It is the standard two-dimensional representation obtained by permuting the three perfect matchings. The three-dimensional piece is the standard zero-sum permutation representation of \(S_4\). Both are absolutely irreducible: subtracting a permutation of any nonconstant vector produces coordinate differences, whose permutation orbit spans the respective zero-sum space. The scalar is inequivalent to either.

#### The shared-index terms: dimensions 6 and 6

For each \(\{i,j\}\), let \(k,l\) be the two complementary indices. The two lines in that sign-character space are

\[
T_{ij}=Q_{ik,jk}+Q_{il,jl},\qquad
W_{ij}=Q_{ik,jk}-Q_{il,jl}.
\]

The sums form the six off-diagonal Ricci components. The differences span a six-dimensional Weyl subspace. Their sign-character lines are permuted transitively by \(S_4\). Any invariant subspace is a sum of its sign-character projections, so a nonzero invariant subspace in either six-dimensional piece contains every line. This proves irreducibility over \(\mathbb C\) as well as \(\mathbb R\).

The two representations are inequivalent: in the sign-character space indexed by \(\{i,j\}\), the stabilizer transposition \(k\leftrightarrow l\) acts by \(+1\) on \(T_{ij}\) and by \(-1\) on \(W_{ij}\). An intertwiner must preserve this stabilizer action.

#### The disjoint-index terms: dimensions 1 and 2

Set

\[
p_1=Q_{12,34},\qquad p_2=-Q_{13,24},\qquad p_3=Q_{14,23}.
\]

A signed permutation acts on these three variables by its determinant times the permutation of the three perfect matchings. Hence the line \(p_1+p_2+p_3\) is the pseudoscalar representation. The plane of zero-sum coefficients is a second two-dimensional Weyl representation. It is inequivalent to the earlier two-dimensional representation because their sign-subgroup characters differ.

Thus the seven mutually inequivalent absolutely irreducible summands have dimensions

\[
1,\;3,\;2,\;6,\;6,\;1,\;2.
\]

By Schur's lemma, every \(H_4\)-equivariant real linear mixing map on \(E\) is a scalar on each summand. Its commutant has dimension seven.

### 3. Full rotations impose exactly three additional equalities

Group the summands as follows:

| Rotational tensor type | Hypercubic pieces | Dimension |
|---|---|---:|
| Scalar | Scalar | 1 |
| Pseudoscalar | Pseudoscalar | 1 |
| Traceless Ricci/stress type | Diagonal 3 + off-diagonal 6 | 9 |
| Weyl type | Diagonal 2 + shared-index 6 + disjoint-index 2 | 10 |

These four grouped spaces are invariant under \(O(4)\). This follows directly from the coordinate-invariant trace, complete alternation, and Ricci contraction of a pair-antisymmetric, pair-symmetric tensor. On the kernel of complete alternation, remove the scalar and traceless Ricci parts; the remaining ten-dimensional kernel is the Weyl part.

The three equalities needed to commute with continuous rotations are necessary by direct differentiation. Write

\[
a=F_{12},\ b=F_{13},\ c=F_{14},\ d=F_{23},\ e=F_{24},\ f=F_{34}
\]

inside the symmetric invariant bilinear notation. The generator \(J_{12}\) acts by

\[
J_{12}b=d,\quad J_{12}c=e,\quad
J_{12}d=-b,\quad J_{12}e=-c,\quad
J_{12}a=J_{12}f=0.
\]

It therefore gives nonzero links

\[
J_{12}(b^2+c^2-d^2-e^2)=4(bd+ce),
\]

\[
J_{12}(a^2+f^2-b^2-e^2)=-2(bd-ce),
\]

\[
J_{12}(af+be)=de-bc.
\]

These connect the two stress pieces and connect both two-dimensional Weyl pieces to the shared-index Weyl piece. Consequently an equivariant mixing map with coefficients \(z_\bullet\) commutes with all of \(O(4)\) if and only if

\[
z_{T,3}=z_{T,6},\qquad
z_{W,2d}=z_{W,6}=z_{W,2p}.
\]

Necessity follows from the displayed nonzero links. Sufficiency follows because the map is then scalar on each of the four coordinate-invariant grouped spaces. The \(O(4)\) commutant has dimension four.

The independent identity subtraction lies only in the scalar channel under full hypercubic covariance. It does not change the three tensor equalities above.

### 4. Consequences and limits for the YM route

1. In the local gauge-invariant polynomial class, the only parity-even hypercubic scalar of engineering dimension four is \(\operatorname{Tr}F_{\mu\nu}F_{\mu\nu}\), up to normalization. The pseudoscalar changes sign under reflections. Thus there is no additional parity-even marginal bulk action anisotropy of this elementary type.
2. The one-field tensor mixing matrix still has seven hypercubic channels. Lattice symmetry does not impose the three equalities required of a rotational intertwiner.
3. The equalities classify a map between two copies of the canonical tensor representation. They do not state that a particular bare-to-renormalized lattice mixing matrix must itself commute with \(O(4)\): finite counterterms may compensate anisotropic cutoff representatives. The actual requirement remains rotational covariance of the normalized limiting correlation hierarchy.
4. Even an exactly \(O(4)\)-equivariant marginal mixing matrix does not bound nonlocal or irrelevant rotation defects. The angular-defect estimates of the route still have to be proved.
5. The classification concerns the fixed finite family at one-field marginal order. It does not close higher source contacts, derivative vertices, or the full marked RG induction.

### 5. Dimensions and character orthogonality

The signed-permutation group has order 384. The seven invariant subspaces have dimensions 1, 3, 2, 6, 6, 1 and 2. In this order their character inner-product matrix is the identity. The six infinitesimal coordinate rotations impose the three compatibility relations above.


---
