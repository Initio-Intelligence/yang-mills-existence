# Actual first-step boundary means: the averaged soft gauge does not furnish an interior-cutoff margin

**Scope.** This note uses the actual flat first Wilson step of CMP119, with the averaged soft gauge chosen in (1.5)–(1.7), the source independent coordinates, and a source-derived first-step region. It does not substitute a scalar SPD model for the Yang–Mills precision. It proves an exact boundary-to-mean identity and a lower bound for the actual precision's conditional-mean operator. The conclusion is a failure of a proposed *uniform conditional-mean margin*. It is not a failure theorem for the full M04 scalar carrier norm or for Yang–Mills existence. A separate singleton calculation below concerns the independently variable local-mask amendment, and is explicitly not identified with a source-derived integration region.

## 1. Source conventions and the exact quadratic matrix

Work in fine-lattice units at the first step, put the current coarse field equal to the identity, and take the preliminary regular region to be the whole lattice. Thus the exact critical field and all local comparison critical fields are the identity. In particular, the relocation (CMP119 (1.21)–(1.24)) is the identity. Choose the smoothed gauge, not the alternative hard-tree gauge mentioned on CMP119 p.247.

The source block size is an odd fixed integer \(L>11\): CMP109 p.251. Write \(L=2\ell+1\), and let a fine block centered at a coarse vertex \(y\) be

\[
 B(y)=y+\{-\ell,\ldots,\ell\}^{4}.
 \tag{AB.1}
\]

Use Hermitian Lie-algebra coordinates and the positive inner product \(\langle X,Y\rangle=\operatorname{tr}(XY)\), where the trace is the source normalized trace. All formulas below are componentwise in this inner product. A single scalar color direction therefore suffices for the operator lower bound.

Let \(d\) be the oriented lattice coboundary from bond fields to plaquettes. Let \(\tau_y a(x)\) be the average of the line sums of \(a\) over the source shortest coordinate-order paths from \(y\) to \(x\). The paths and their averaging are CMP109 pp.252–254, (0.8), (0.11), (0.12). In particular, if \(\phi(y)=0\) at every coarse center, then

\[
 \tau_y(d\phi)(x)=\phi(x),\qquad Q(d\phi)=0.
 \tag{AB.2}
\]

Here \(d\phi(e)=\phi(e_+)-\phi(e_-)\); reversing all gauge signs leaves every assertion unchanged. The first identity holds for each path separately, so it is exact for the averaged gauge.

For clarity, the derivative of the group-valued coarse average in *angle* units is

\[
 Q_{\rm ang}a(c)=L^{-4}\sum_{s\in B(0)}
 \left[\tau_{c_-}a(c_-+s)
 +\sum_{t=0}^{L-1}a_\mu(c_-+s+t e_\mu)
 -\tau_{c_+}a(c_++s)\right],
 \quad c_+=c_-+Le_\mu.
 \tag{AB.3}
\]

This follows by differentiating CMP109 (0.12), using (0.8). If the source derivative is denoted by \(Q=L^{-1}Q_{\rm ang}\), its zero space is the same. A face-crossing fine bond in the corridor for \(c\) has coefficient \(L^{1-4}\) in \(Q_{\rm ang}\): there are \(L\) longitudinal starting points with its transverse coordinates, and the internal endpoint contours do not cross a coarse face.

Let \(E=\{b_0(c)\}\) be the source distinguished face bonds, and let \(F\) be their complement. CMP119 p.249, between (1.14) and (1.15), states that the nonlinear linearizing transformation changes only \(E\), and then solves the linear equations by eliminating those same bonds. Consequently the actual linear map \(C\) is

\[
 (Cz)_e=z_e\quad(e\in F),\qquad
 (Cz)_{b_0(c)}=-L^{3}(Q_{{\rm ang},F}z)(c).
 \tag{AB.4}
\]

Each exceptional value uses only the two adjacent blocks. One must not impose a second condition \(Qz=0\) on the independent values \(z\in\mathfrak g^F\). The condition is \(QCz=0\).

CMP119 p.247, (1.6)–(1.7), puts the Wilson action and the averaged gauge action under the *same* factor \(g_0^{-2}\). CMP109 (0.2) fixes the normalized trace. Their quadratic expansion at the identity is therefore exactly

\[
 \frac12\|dCz\|_2^2+\frac12\|\tau Cz\|_2^2
 =\frac12\langle z,Kz\rangle,
 \qquad K=C^*(d^*d+\tau^*\tau)C.
 \tag{AB.5}
\]

Plaquettes are counted once with \(\mu<\nu\), as specified on CMP119 p.253. There is no nonzero background-force/constraint-curvature correction at the identity. Haar factors, the nonlinear exceptional-bond Jacobian, and higher Wilson and soft-gauge terms belong to the complete perturbation \(W_g\); they are not silently removed from the conditional law.

The internal path average never uses a face-crossing bond. Hence

\[
 \tau C=\tau|_F.
 \tag{AB.6}
\]

This simple identity is decisive below. It uses the actual averaged gauge and actual exceptional coordinates, rather than a replacement gauge choice.

The already proved block Poincaré argument in [first step precision gap](first_step_precision_gap.md) gives \(K\ge\lambda_L I\). Its proof retains \(\tau_{\rm av}\). The matrix has fixed finite range and a fixed absolute row bound, with constants depending on \(L\) and the fixed group, not the volume.

## 2. Which crossing bonds are integrated

CMP109 p.251 defines the bond set associated with a continuous domain to be the bonds intersecting it. CMP119 p.247, (1.9), states explicitly that the starred set takes the bonds having at least one endpoint in the domain and removes the distinguished bonds. CMP119 p.251 then performs conditional integration over the independent field restricted to \(\Lambda_1\).

Thus, for a region \(\Lambda\) which is a union of coarse \(L\)-blocks, the integrated index set and the retained index set are

\[
 I=\Lambda^*\subset F,\qquad O=F\setminus I.
 \tag{AB.7}
\]

In particular, a nonexceptional fine bond crossing a face from an exterior block into an interior block belongs to \(I\). The retained set \(O\) is the complement of this **bond index set**. It is not a second independent application of the incident-bond convention to the complementary sites. The latter interpretation would incorrectly put the same crossing bond on both sides of a disintegration.

The first-step source regions are unions of \(LMR_1\)-cubes and hence are unions of the blocks (AB.1). Their large collars do not alter this local crossing-bond convention.

For the untruncated Gaussian part of the exact conditional law, the conditional mean is

\[
 m_I(a)=-K_{II}^{-1}K_{IO}a,
 \qquad a\in\mathfrak g^O.
 \tag{AB.8}
\]

The matrix inverse exists by the uniform gap. Formula (AB.8) describes the actual quadratic matrix in the complete normal form. It does not assert that the cut-off conditional law has that mean.

## 3. Exact conditional harmonic extension of an exterior pure gauge

### Theorem AB.1

Let \(\phi\) vanish at every coarse center and on every vertex in the integrated blocks. Let \(z\) be the restriction of \(d\phi\) to the independent bonds \(F\), and let \(a=z_O\). Then

\[
 -K_{II}^{-1}K_{IO}a=z_I.
 \tag{AB.9}
\]

This identity is exact for the actual first-flat constrained precision (AB.5), for every source-shaped region \(\Lambda\).

**Proof.** Since \(Qd\phi=0\), the exceptional-bond solve gives \(Cz=d\phi\). Thus \(dCz=0\) and \(\tau Cz=\phi\). For an integrated independent coordinate \(i\), either it is internal to an integrated block, or it crosses a coarse face. In the first case the column \((\tau C)_i\) is supported on that integrated block, where \(\phi=0\). In the second case the column is zero, because internal center-to-vertex paths do not use face bonds. Therefore

\[
 (Kz)_i=\langle dCe_i,dCz\rangle
       +\langle\tau Ce_i,\phi\rangle=0
       \quad(i\in I).
 \tag{AB.10}
\]

Equivalently, the full pure gauge has zero Wilson quadratic, the exterior soft-gauge quadratic is already fixed by the retained internal bonds, and the interior soft-gauge quadratic vanishes. It minimizes the complete quadratic energy over the integrated variables. Strict positivity of \(K_{II}\) makes it the unique minimizer and proves (AB.9). ∎

No estimate of a propagator, no diagonal-dominance assumption, and no cancellation of a determinant is used here. In particular, the result is not sensitive to a long-distance covariance bound being too weak.

## 4. A source-shaped face with boundary gain at least \((L-3)/2\)

Choose a flat face of a first-step retained rectangular component, away from its macro-corners. Put one exterior fine block at center zero, with the integrated neighbor at center \(Le_1\). Set

\[
 H=\ell-1=(L-3)/2,\qquad
 p=(\ell,1,0,0),\qquad q=p+e_1.
 \tag{AB.11}
\]

The bond \(e=(p,q)\) is integrated and nonexceptional: its transverse coordinate is not the central corridor coordinate. This central choice is literal, not an assumed convention: CMP109 p.267, after (2.10), defines \(b_0(c)\) as the fine bond contained in the straight coarse bond \(c\) and belonging to its crossing corridor. Define the scalar function on the exterior block by

\[
 f(x)=(H-|x-p|_1)_+,
 \tag{AB.12}
\]

and put it equal to zero on all other blocks. It vanishes at the block center and on each face other than the one shared with the integrated neighbor. It is 1-Lipschitz on every retained bond. Its only large jump after extension by zero is across the shared face, whose nonexceptional crossing bonds are integrated. At the chosen crossing bond, \(df(e)=-H\).

Choose a fixed Lie-algebra element \(T\) of source norm one, and put

\[
 \phi(x)=\theta P f(x)T,\qquad 0<\theta<1,
 \qquad a=(d\phi)|_O.
 \tag{AB.13}
\]

Every retained independent entry obeys \(|a_i|\le\theta P\). Nevertheless Theorem AB.1 gives

\[
 m_I(a)_e=-\theta HPT.
 \tag{AB.14}
\]

For the actual source choice \(L>11\), \(H\ge5\). Taking \(\theta=3/4\) gives an untruncated conditional mean of magnitude at least \(15P/4\), while every retained collar entry is at most \(3P/4\).

In operator language, on the actual allowed center-fixed exterior gauge-gradient subspace,

\[
 \big\|K_{II}^{-1}K_{IO}\big\|_{\ell^\infty(O)\to\ell^\infty(I)}
 \ge (L-3)/2.
 \tag{AB.15}
\]

The norm is the actual independent-coordinate norm, with the same fixed Lie norm in each slot. In particular, it cannot be bounded by \(1-\vartheta\) for a positive universal margin \(\vartheta\).

### Admission with the source R labels and their padding

This is not a fine-scale singleton substituted for \(\Lambda_1\). The face can be taken from an actual rectangular first R-born hole. Keep the strict R-bad seeds deep in that component, as in the center-fixed pure-gauge seed construction. Add (AB.13) in one boundary block, separated from those seeds and from macro-corners. Since all added retained free entries are strictly below \(P\), every overlapping good R test stays good; the deep bad tests stay unchanged. The resulting derived \(\Lambda_1\) is the same.

The starred Q test permits values below \(2P\), so the boundary values (AB.13), the strict seed values \(3P/2\), and a choice of integrated free values equal to zero are all strictly Q-good. At the flat coarse field the comparison backgrounds are the identity, and the exceptional nonlinear correction does not change starred coordinates. The source explicitly drops the older fine-curvature and soft-gauge hard tests on this globally Q-good region when \(A_0\) is sufficiently larger than \(A_1\): CMP119 p.248. This supplies an active conditional fiber, not an inadmissible formal boundary assignment.

The remote seed can be chosen in the same color direction, with center-fixed potential supported wholly in retained blocks. Its pure-gauge extension has zero integrated entries, so (AB.9) says that it contributes zero to the conditional mean. It does not modify (AB.14). The \(MR_1\) padding therefore does not cure this example: it separates bad seeds from the boundary but does not force the R-good collar to be a smaller fraction of \(P\).

The untruncated Gaussian mean itself need not satisfy the Q or R restrictions, and is not being asserted to be an admitted field. Its failure to satisfy the integration cutoff is precisely the conclusion.

## 5. The exact complete conditional law and the limit of this result

At the fixed flat geometry, after retaining every actual Haar, exceptional-Jacobian, soft-gauge, and Wilson remainder factor, the conditional density has the form

\[
 q_{g,I,a}(dz)=
 \frac{\mathbf1_{\{|z_i|<P:i\in I\}}
       \exp[-\tfrac12\langle z,K_{II}z\rangle
                  -\langle z,K_{IO}a\rangle+W_g(z,a)]\,dz}
      {\int_{\{|w_i|<P:i\in I\}}
       \exp[-\tfrac12\langle w,K_{II}w\rangle
                  -\langle w,K_{IO}a\rangle+W_g(w,a)]\,dw}.
 \tag{AB.16}
\]

Retained-only factors cancel in this ratio. The fixed outside selectors are part of the active fiber and do not supply a new interior-margin restriction. The quadratic center in (AB.16) is exactly (AB.8), regardless of how the complete perturbation is later organized.

Theorem AB.1 closes the narrow question of whether the actual constraints, averaged soft gauge, and large-field padding imply a uniform conditional-Gaussian mean inside the broad product cutoff: **they do not**. A proof based on such a margin must be replaced by an argument that treats the cutoff completion at a saturated center, or by a correctly normalized average over the offending retained sectors.

This statement does not prove a scalar carrier obstruction. At the untruncated pure-gauge center the physical Wilson curvature is zero. Gauge-coordinate amplification is not itself an amplified physical scalar. The hard cutoffs can change the physical response, but a representation-wide scalar lower bound would require further analysis and is not claimed here. Nor does a large mean contradict the proved real conditional moment/response estimates, whose full retained regulator pays for large retained data.

For comparison, finite range, a uniform gap and the ordinary exponentially decaying Green bound still give a volume-independent upper bound

\[
 \|K_{II}^{-1}K_{IO}\|_{\infty\to\infty}\le C_L.
 \tag{AB.17}
\]

Thus the issue is the missing strict contraction relative to the *literal* cutoff radius, not an uncontrolled volume factor.

## 6. An independent singleton check using the actual Wilson scalar

The following calculation is useful for the proposed independent local-mask family and for conditional block-sampling arguments. It is also an actual one-coordinate conditional of the globally R-good first-step product-cutoff law, after all its other free coordinates are conditioned at the admitted values below. A singleton is not a source-derived top-level \(\Lambda_1\), so this section is not used to upgrade Section 4 into a scalar no-go theorem.

Choose an internal nonexceptional bond \(e=(p,q)\), at least two steps from all block faces, with

\[
 p=(1,1,1,1),\qquad q=(2,1,1,1).
\]

Let \(\phi(p)=-T\), \(\phi(q)=T\), and let it vanish at every other vertex. Its independent gradient \(v=(d\phi)|_F\) has \(v_e=2T\) and \(|v_j|\le1\) at all other independent bonds. Again \(Cv=d\phi\).

Exactly one fourth of the source coordinate-order paths from the block center to \(q\) use \(e\), while no such path to \(p\) uses it. Hence

\[
 (Kv)_e=\tfrac14T.
 \tag{AB.18}
\]

In scalar color units the diagonal \(k_e=K_{ee}\) is at least \(2(d-1)=6\). Indeed the six plaquettes containing this interior edge see its unit coefficient and no exceptional correction; the soft-gauge contribution and all other plaquettes are nonnegative. For the singleton integrated set and retained data \(a=\theta Pv_{e^c}\), the exact Gaussian center is therefore

\[
 m_e=\theta P\left(2-\frac1{4k_e}\right)T,
 \qquad
 2-\frac1{4k_e}\ge\frac{47}{24}.
 \tag{AB.19}
\]

All retained entries can be at most \(3P/4\), while this center has magnitude at least \(47P/32>P\).

Choose any one of the six plaquettes containing \(e\). All its other bonds are fixed nonexceptional bonds. On the single-color ray the actual plaquette is

\[
 U(\partial p)=\exp\{\pm i g(z_e-2\theta PT)\}.
 \tag{AB.20}
\]

For a general Lie-algebra value of \(z_e\), the exact product is conjugate, up to cyclic ordering in the trace, to \(e^{igz_e}e^{-2i\theta gPT}\). Consequently its small-field Wilson quadratic is

\[
 g^{-2}[1-\operatorname{Re}\operatorname{tr}U(\partial p)]
 =\tfrac12\operatorname{tr}(z_e-2\theta PT)^2+O(gP^3),
 \qquad |z_e|\le P.
 \tag{AB.21}
\]

For \(\theta>1/2\), norm equivalence in the fixed Lie algebra gives a positive lower bound \(c_G(2\theta-1)^2P^2\), uniformly on the whole singleton cutoff, once \(gP\) is small. This is an actual local Wilson observable; it is not the unphysical coordinate square \(z_e^2\).

For \(G=SU(2)\), its operator-norm Lie ball is a Euclidean ball up to a fixed trace factor. The complete first-step remainder obeys the already verified single-coordinate derivative bound \(|\partial_{z_e}W_g|\le CgP^2\), uniformly in the volume on this common first-step chart. The normalized singleton law therefore concentrates, after scaling by \(P\), at the constrained quadratic minimizer. At \(\theta=3/4\), (AB.19) places that minimizer at \(T\) on the unit sphere. Elementary finite-dimensional Laplace concentration, with \(P\to\infty\) and \(gP\to0\), gives

\[
 P^{-2}q_{g,e,a}\!left(g^{-2}[1-\operatorname{Re}\operatorname{tr}U(\partial p)]\right)
 \longrightarrow \tfrac18\operatorname{tr}(T^2)>0.
 \tag{AB.22}
\]

At zero retained boundary the same local observable has expectation \(O(1)\). This verifies a physical scalar wall response in an actual-kernel singleton conditional. Its \(P^2\) scale is paid by the local retained energy regulator, and it supplies no large-support lower bound by itself.

## 7. What remains constructive

The exact source coefficient result suggests treating the averaged gauge sector and its broad-cutoff completion before attempting a uniform support expansion. Averaging the first R sectors in the original complete positive operation is a different operation from bounding every normalized retained R fiber separately. The present theorem is compatible with exponential suppression of those sectors in their actual outer mass. Any such averaging proof must retain the common normalization and the primitive Wilson mark; it cannot be replaced by the false pointwise mean-margin premise disproved above.

**Conclusion:** the actual first-flat boundary-margin question is resolved negatively by (AB.9)–(AB.15). The remaining M04 question requires an argument that permits these actual saturated fibers or an explicitly authorized averaged interface with its own marked estimate.
