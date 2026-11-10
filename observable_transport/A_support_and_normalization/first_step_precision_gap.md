# The first-step constrained precision at the local lift

This note proves the finite-range positive-gap input for the buffered-resolvent lemma, at the first globally regular Wilson step. Its ingredients are the exact local lift and free-coordinate elimination printed in CMP119 (1.3), (1.14)–(1.17), the block-local averaging operation of CMP98, and the local Wilson/constraint Taylor expansion. It makes no claim about a later completed residual component.

## 1. A flat block Poincaré inequality

Let a be a Lie-algebra-valued fine-lattice one-cochain. Let Q be the derivative of the actual coarse averaging map at the identity. The source soft gauge variable is the symmetrized path average in CMP109 (0.11); its linearization τ_av a(y,x) is the average of the line sums over the prescribed shortest coordinate-path permutations from a coarse center y to x. Its quadratic form is a fixed positive multiple of Σ_{y,x}|τ_av a(y,x)|², as displayed in CMP109 (0.8). It is not a single tree-path sum. Write τ_tree for any one fixed coordinate-ordered axial-tree choice. The following properties of Q follow from the finite local averaging paths and its exact coarse readout:

* Q is a bounded linear operator with a fixed O(L) fine-lattice dependency range.
* For a vertex function φ vanishing at every coarse center, Q(dφ)=0.
* The linear coarse-face lift Q^f has zero internal bonds and constant value b_c on each fine bond crossing coarse face c, and Q Q^f b=b.

The bounds depend on fixed L and the group dimension, not on the number of blocks.

### Lemma PG.1

For Qa=0,

\[
 \sum_e|a_e|^2\le C_L\left(\sum_p|(da)_p|^2
                         +\sum_{y,x}|\tau_{\rm av} a(y,x)|^2\right). \tag{PG.1}
\]

**Proof.** First compare the actual averaged contour with the chosen tree contour. Their difference is an average of loop circulations inside a fixed L-block. Discrete Stokes on the finitely many elementary path interchange surfaces gives ||τ_tree a−τ_av a||²≤C_L||da||². It therefore suffices to establish (PG.1) with τ_tree in place of τ_av.

Choose the vertex function φ(x) equal, with the appropriate orientation, to τ_tree a(y,x), and φ(y)=0. Then a'=a−dφ has zero path sum on every block axial tree. It obeys Qa'=Qa=0 and da'=da.

For an internal fine bond, its value a'_e is the circulation on the loop made from that bond and the two paths to its block center. Fill this loop by elementary plaquettes within the block. Discrete Stokes expresses a'_e as a sum with fixed, L-dependent integer coefficients of the local da plaquettes. For a bond crossing the face between two neighboring coarse blocks, compare its path from the first center to the second with the path through the source's distinguished bond b0(c). Their difference is a loop in those two adjacent blocks, and discrete Stokes bounds the difference of the two cross-face values by local da. Thus

\[
 a'=Q^f b+r,
\]

where b_c is the distinguished cross-face value and every r_e is a linear combination of da on a fixed enlarged fine block. Fixed local multiplicities give ||r||²≤C_L||da||².

Applying Q and using its exact lift identity gives b=−Qr. Hence ||b||²≤C_L||r||² and ||a'||²≤C_L||da||². Finally ||dφ||²≤C_LΣ|τ_tree a(y,x)|², since each vertex has bounded fine degree. Add the two bounds and then use the initial comparison of τ_tree with τ_av to obtain the actual-source inequality (PG.1). The construction is block-local, so a periodic global holonomy does not change the estimate. ∎

At the identity the constrained quadratic Wilson form plus soft axial gauge form is therefore at least c_L||a||² on ker Q. The actual independent-coordinate embedding C0 keeps every free coordinate unchanged and only solves for b0(c). Thus ||C0z||≥||z||. It follows that the actual flat independent-coordinate precision K_flat obeys

\[
 K_{\rm flat}\ge\lambda_L I,\qquad\lambda_L>0.         \tag{PG.2}
\]

Fixed trace and Hessian normalization conventions are included in λ_L.

## 2. The actual first-step reference precision is finite range

Put U0=Q^fV, the exact local raw coarse-link lift. CMP119 p.249 states that the nonlinear constraint-linearizing map differs from the identity only at b0(c), and that the linear equation Qa=0 solves a(b0(c)) using only bonds in B(c−)∪B(c+). Thus C(U0) is local. The bare Wilson Hessian couples only bonds of a plaquette; the soft gauge Hessian couples only paths in one L-block. The second derivative introduced by the nonlinear constraint elimination is also confined to the same two-block paths. Its coefficient is the actual first variation J(U0).

Consequently the complete constrained quadratic precision at this reference is finite range in the free bond coordinates and has a fixed raw-V dependency range. Include the constraint-curvature Hessian here. Haar/coarea logarithms and higher potential terms stay in the full perturbation W. No quadratic term is removed merely because U0 is not stationary.

On a fixed small local geometric chart these finite matrices and all local inverses used to solve the b0 constraints vary smoothly. At flat data they reduce to K_flat. The Wilson force satisfies |J_e(U0)|≤CΣ_{p∋e}||U0,p−I||, so its constraint-curvature contribution tends to zero with the local curvature.

## 3. Local gauges supply the gap without a global weak-link chart

Assume every retained coarse plaquette has ||V_p−I||≤ε. Choose a fixed cube partition of unity χ_Q with Σχ_Q²=1, cube side M, bounded overlap, and Lipschitz constant C/M. Enlarge each Q by the fixed entry footprint of the precision. On this finite enlarged coarse cube, use the coordinate-ordered axial gauge. Every transformed coarse link is a product of a bounded number, at most C M², of transported plaquette holonomies. Because the transports are unitary,

\[
 \|V_e^v-I\|\le C M^2\varepsilon.                    \tag{PG.3}
\]

The lift transforms by the block-constant fine gauge u0(x)=v(y) on B(y). CMP119 (1.17) gives this covariance for the constraint and action coordinates. It acts orthogonally on the free Lie-algebra variables. Hence the local principal precision is unitarily conjugate to a matrix whose coefficients differ from their flat values by at most C(L,M)ε in absolute row norm. In particular,

\[
 P_QK_0(V)P_Q\ge[\lambda_L-C(L,M)\varepsilon]I_Q.     \tag{PG.4}
\]

This estimate uses only a local gauge on a fixed cube. It neither assumes a globally small logarithm of V nor discards nontrivial torus holonomy.

Let r be the fixed free-coordinate range and K_* a fixed bound for its absolute row sums on the local chart. The exact IMS error has entries

\[
 \left(\sum_Q\chi_QK_0\chi_Q-K_0\right)_{ij}
 =-\tfrac12(K_0)_{ij}\sum_Q(\chi_Q(i)-\chi_Q(j))^2.
\]

Its operator norm is at most C K_*r²/M². Choose M large enough that this is less than λ_L/4, and then choose ε small enough that C(L,M)ε≤λ_L/4. Combining (PG.4) with Σχ_Q²=1 gives

\[
 K_0(V)\ge\lambda_L I/2.                              \tag{PG.5}
\]

Both choices are made once, before the coupling tends to zero. The source all-regular first-step coarse-curvature ceiling tends to zero with the admitted coupling, so it eventually lies in this class. This proves the real geometric gap for the local lift, including its nonzero Wilson force.

## 4. What this supplies

The finite-range raw dependence and (PG.5) are precisely the real hypotheses needed to apply Theorem PR.1 to K0 and to K0−σI for fixed 0<σ<λ_L/2. It then gives an all-t resolvent and inverse square root with genuinely supported, absolutely summable physical coefficients. The nonlinear correction from U0 to the true minimizer still needs the source's connected decoupling bound in the same coefficient norm. The interacting marked numerator, all retained history changes and the full M-04 conclusion do not follow solely from this positive-gap lemma.
