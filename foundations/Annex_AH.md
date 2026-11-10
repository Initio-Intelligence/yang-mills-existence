# Complete regular E/R derivative-carrier sums

**Annex AH.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Exact target and inputs

C-04 asks for the actual current-coordinate value, gradient and Hessian majorants, summed over old scales and carriers with the running radii and preparation losses retained. It requires a small weighted Hessian budget and local derivative budgets. The theorem below supplies these for the source's regular E/R contribution. B, the heterogeneous classical action, coordinate Jacobians and posterior/interface currents have their own original statements; they are not omitted from the complete law by completing C-04.

Use the actual current free coordinates of C-01/C-07, with their unit-scale Euclidean quadratic norm. A bond has a fixed orthonormal Lie-algebra basis of dimension \(D=\dim\mathfrak g\). Archived history data remain fixed parameters in this conditional statement. Let \(\rho_k(i,j)\) be periodic lattice distance between current-coordinate bonds in current lattice units. Fix any admitted torus large enough for the source's localization partition.

The completed Theorems E14.3 and R14.3 supply actual localized functions

\[
 V_{k,Y}=\mathcal E_{k,Y}+\mathcal R_{k,Y},\qquad
 W_k^{ER}=\sum_Y V_{k,Y},
 \tag{DS.1}
\]

on one common contour containing \(\|z\|_\infty\le P_k\), where

\[
 P_k=A_1\ell_k^{p_0},\quad \ell_k=\log g_k^{-2},\quad
 |V_{k,Y}|\le K_k e^{-\kappa_*d_k(Y)},\qquad
 K_k=\mathfrak K_E+C_Rg_k^{\kappa_0-11},\quad \kappa_0\ge12.
 \tag{DS.2}
\]

The current scalar-coordinate radii are \(r_z=c_GP_k\), with one fixed \(c_G>0\). The native background, independent current and preparation radii \(r_b,r_J,r_s\) are those of (E14.52)/(RM.14). These radii are independent of the later derivative order. All old-scale summations, the matching E coupling subtraction, the R vacuum subtraction and the true completed R denominators are already included in (DS.2). This proof does not differentiate a source-free real value bound.

The source's localization is exact in these variables: a term with carrier \(Y\) depends only on the admitted fields restricted to \(Y\). A derivative in a current coordinate outside that carrier vanishes. Source-local field or current extensions are part of that actual function, not additional substitutions suppressed here.

The two source geometry facts used below are explicit: \(d_k(Y)\) is shortest connecting-tree length divided by the localization cube size \(M\), with an equivalent tree made of cube edges; the localized sums have exact carrier support and allow a sufficiently large fixed decay parameter. See CMP109 p.257 before (0.24), and CMP116 (1.26), (1.33)–(1.36).

### 2. An explicit anchored carrier count

Work in the rescaled \(M\)-cube lattice. Include the finite zero-length cases. Let \(n(Y)\) be the integer length of the source's equivalent cube-edge tree. To avoid assuming that two equivalent length conventions are exactly equal, fix their geometric comparison constant \(C_{\rm tree}\ge1\) so that

\[
 n(Y)\le C_{\rm tree}\bigl(d_k(Y)+1\bigr),\qquad
 \widehat\kappa=\kappa_*/C_{\rm tree},\qquad
 \widehat K_k=e^{\kappa_*}K_k.
 \tag{DS.2a}
\]

The comparison is a fixed cube-geometry fact: replace a connecting tree by its cube-edge representative. The source states this equivalent definition; allowing \(C_{\rm tree}\) and an endpoint cube makes the argument valid whether or not its convention gives equality. Neither constant depends on cutoff, volume or history. In particular (DS.2) implies

\[
 |V_{k,Y}|\le\widehat K_k e^{-\widehat\kappa n(Y)}.
 \tag{DS.2b}
\]

The metric-equivalence loss is charged to the decay rate, not merely to a prefactor.

For a current bond \(i\) belonging to \(Y\), choose an incident cube and one of its vertices on a shortest edge tree. There are at most \(2^{2d}\) choices, where \(d=4\). A rooted tree with \(n\) edges is encoded by its canonical depth-first walk, of length \(2n\), with at most \(2d\) choices at each step. At most \(2^d(n+1)\) cubes can meet its vertices. A carrier associated to that tree is a subset of these cubes, so the number of possible subsets is at most \(2^{2^d(n+1)}\). Conditions requiring a domain to be connected, regular or contained in an admitted region only reduce this bound.

Consequently the number of actual distinct carriers at length \(n\), after the source has combined terms having the same carrier, is bounded by

\[
 N_i(n)\le B_d A_d^n,
 \qquad B_d=2^{2d+2^d},\qquad
 A_d=(2d)^2 2^{2^d}.
 \tag{DS.3}
\]

This deliberately large bound is independent of torus volume. The same encoding works on a periodic cube graph: its degree is at most \(2d\), and a tree traversal determines its vertices on that graph. Winding does not introduce an uncounted root or translate.

If \(i,j\) are coordinates in \(Y\), connect each to a point of this tree in its cube, and connect those points along the tree. Thus, with a fixed endpoint constant \(c_d=2d+4\),

\[
 \rho_k(i,j)\le M\bigl(n(Y)+c_d\bigr).
 \tag{DS.4}
\]

Distances on a torus are periodic distances, so this remains an upper bound there. Fixed carrier enlargements in an equivalent source convention merely enlarge \(B_d,c_d\) by fixed factors. The present proof uses the actual final carrier, not a smaller pre-localization support.

Choose the source decay and preparation parameters once, before the running coupling ceiling, so that

\[
 \widehat\kappa>\log A_d+1,
 \qquad 0<\gamma M<\widehat\kappa-\log A_d.
 \tag{DS.5}
\]

This is a finite strengthening of the source's sufficiently-large decay choice. CMP116 allows the localization loss to leave a fixed fraction of the primitive decay, with its fixed preparation constants retained; first choose that primitive decay and the required decoupling parameter, then a sufficiently large fixed \(M\) as in its (1.11). The theorems E14.3/R14.3 are used with this common choice. No parameter is increased with derivative order or cutoff. The independent complete construction/trajectory certification remains part of J0.

Put

\[
 \mathscr S_\gamma
 =\frac{B_d\exp(\gamma M c_d)}
 {1-A_d\exp[-(\widehat\kappa-\gamma M)]}<\infty.
 \tag{DS.6}
\]

Equations (DS.3)–(DS.4) imply the uniform anchored sum

\[
 \sup_i\sum_{Y:i\in I_Y}
 e^{\gamma\operatorname{diam}(I_Y)}e^{-\widehat\kappa n(Y)}
 \le\mathscr S_\gamma.
 \tag{DS.7}
\]

All multiplicities from old scales and different source preparations are already included in the per-carrier majorant (DS.2). They are not counted again as new carriers in (DS.3).

### 3. Value, gradient and weighted Hessian bounds

#### Theorem DS.1 — the actual regular E/R Hessian is uniformly small

On every admitted real regular support, the actual contributions (DS.1) satisfy

\[
 \sup_i\sum_{Y:i\in I_Y}|V_{k,Y}|
 \le \widehat K_k\mathscr S_0,
 \tag{DS.8}
\]

\[
 \sup_i\sum_{Y:i\in I_Y}
 e^{\gamma\operatorname{diam}(I_Y)}
 \|D_iV_{k,Y}\|
 \le\frac{C_{G,1}\widehat K_k\mathscr S_\gamma}{P_k},
 \tag{DS.9}
\]

and

\[
 \boxed{
 \sup_i\sum_j e^{\gamma\rho_k(i,j)}
 \|D_iD_jW_k^{ER}\|_{\mathrm{op}}
 \le \varepsilon_{ER}(g_k)
 :=\frac{4D\,\widehat K_k\mathscr S_\gamma}{c_G^2P_k^2}.
 }
 \tag{DS.10}
\]

Here \(C_{G,1}\) is a fixed basis constant, for example \(\sqrt D/c_G\). Given any prescribed \(\eta>0\), one common small-coupling ceiling makes \(\varepsilon_{ER}(g_k)\le\eta\) for every scale in the admitted trajectory and every remaining admitted history.

**Proof.** The value bound follows immediately from (DS.2b) and (DS.7). Scalar-coordinate Cauchy bounds each first derivative by the enlarged carrier majorant (DS.2b) divided by \(r_z\). The Euclidean norm of the fixed-dimensional block gradient costs at most \(\sqrt D\), proving (DS.9).

For the Hessian, apply Theorem BD.2 to the actual simultaneous current polydisc, keeping the native external variables fixed in their admitted contour. For each scalar output component \(a\) of a bond \(i\),

\[
 \sum_{j,b}|\partial_{ia}\partial_{jb}V_{k,Y}|
 \le \frac{4\widehat K_ke^{-\widehat\kappa n(Y)}}{r_z^2}.
 \tag{DS.11}
\]

Each block operator norm is bounded by the sum of the absolute values of its matrix entries. Summing the \(D\) output components, and using
\(e^{\gamma\rho_k(i,j)}\le e^{\gamma\operatorname{diam}(I_Y)}\), gives the factor \(4D\) in (DS.10), followed by (DS.7). Derivatives of a carrier not containing \(i\) vanish. Absolute convergence of these anchored sums justifies the differentiated sum, uniformly in the volume. There is no spurious factor equal to the number of fine coordinates inside a carrier.

For the last assertion use \(g_k\le1\), \(\kappa_0-11\ge1\), and set \(K_*=e^{\kappa_*}(\mathfrak K_E+C_R)\). All constants in \(K_*\) and \(\mathscr S_\gamma\) were fixed before reducing the coupling ceiling. It suffices to impose

\[
 \ell_k\ge
 \left(\frac{4D K_*\mathscr S_\gamma}
 {c_G^2A_1^2\eta}\right)^{1/(2p_0)}.
 \tag{DS.12}
\]

This is compatible with the fixed logarithmic and small-coupling conditions of the two contour theorems. It uses their source-order-independent \(q>p_0\), without changing \(q\). \(\square\)

For scalar physical weights \(\omega_i\ge\omega_*>0\) in these same coordinates, the weighted version of (DS.10) is at most \(\omega_*^{-2}\varepsilon_{ER}(g_k)\). The unit current coordinates here take \(\omega_i=1\). A new heterogeneous norm with no verified lower bound is not covered by renaming these weights; its precision, coordinate transfer and coercivity requirements remain C-06. This theorem does not assert the complete action is convex.

### 4. Fixed all-order local jets, including native external variables

Here a **local analytic source direction** means an explicitly given perturbation of the admitted slots \((z,b,J,s)\). It does not mean a new inhomogeneous Wilson-action source whose induced E/R vertices have not yet been constructed. The latter marked matching remains M-04/M-06.

For directions \(h_l=(h_l^z,h_l^b,h_l^J,h_l^s)\), define the actual finite-parameter pullback

\[
 \mathcal V_{k,Y}(t_1,\ldots,t_m)
 =V_{k,Y}\left(z+\sum_lt_lh_l^z,
 b+\sum_lt_lh_l^b,
 J+\sum_lt_lh_l^J,
 s+\sum_lt_lh_l^s\right).
 \tag{DS.13}
\]

Use the verified native norms, and write

\[
 q_l=\max\left\{
 \frac{\|h_l^z\|_\infty}{r_z},
 \frac{\|h_l^b\|_{\rm native}}{r_b},
 \frac{\|h_l^J\|_\infty}{r_J},
 \frac{\|h_l^s\|_\infty}{r_s}
 \right\}.
 \tag{DS.14}
\]

If \(q_l=0\), the corresponding derivative vanishes. Otherwise the polydisc \(|t_l|<(m q_l)^{-1}\) lies in the same admitted contour, by the triangle inequality in each slot. Cauchy therefore gives

\[
 \left|\partial_{t_1}\cdots\partial_{t_m}
 \mathcal V_{k,Y}(0)\right|
 \le e^m m! \widehat K_ke^{-\widehat\kappa n(Y)}
       \prod_{l=1}^m q_l.
 \tag{DS.15}
\]

For local directions, a term can contribute only if its carrier meets the support of every differentiated direction. Anchoring on the first direction's support \(S_1\), let \(N(S_1)\) be the number of localization cubes meeting that support, with the fixed endpoint convention used in (DS.3). Then

\[
 \sum_Ye^{\gamma\operatorname{diam}(I_Y)}
 \left|\partial_{t_1}\cdots\partial_{t_m}
 \mathcal V_{k,Y}(0)\right|
 \le N(S_1)\mathscr S_\gamma e^m m!\widehat K_k
       \prod_{l=1}^m q_l.
 \tag{DS.16}
\]

One may anchor on any chosen direction. The support factor is local; it does not become the torus volume for a fixed local test. Pure current directions of supremum norm one have \(q_l=(c_GP_k)^{-1}\). Native external directions retain their actual \(\alpha_{0,k}\) radii. Raw fine-link directions retain the extra \(\xi\), or \(\xi^{1+\beta}\), radius from E14.3/R14.3. Thus no uniform bare external-coordinate bound is asserted where the admitted radius runs to zero.

The exponent of \(m!\) in this directional jet estimate is fixed at one. The proof bounds directional multilinear forms and anchored Hessian rows; it does not claim a dimension-free sum of the absolute coefficients of every high-order derivative tensor. A nonlinear parameter-to-slot map must be substituted into (DS.13) with its actual higher jets and chain-rule terms; the theorem supplies the slot derivative budgets but does not assume that additional map is linear.

### 5. Application and remaining applications

Equations (DS.8)–(DS.12) give the required complete regular E/R value, gradient and arbitrarily small weighted Hessian budgets. Equations (DS.13)–(DS.16) give explicit local joint jets with fixed factorial growth and the actual running radii. All old-scale and preparation losses are already accounted for by the completed native contour theorems, and the actual carrier geometry is summed in (DS.3)–(DS.7).

For the regular E/R part, the preceding estimates bound the current-coordinate value, gradient and Hessian. Their application to the complete Wilson density requires CL and the remaining boundary, classical, Jacobian and posterior contributions.

### Sources

- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. I*, CMP 109 (1987), 249–301, p.257, definition of localization domains and their tree length; [DOI](https://doi.org/10.1007/BF01215223).
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. II. Cluster Expansions*, CMP 116 (1988), 1–22, (1.11), (1.26), and Lemma 1, (1.33)–(1.36); [DOI](https://doi.org/10.1007/BF01239022).
- The complete actual-domain and old-scale proofs used here are Theorems E14.3 and R14.3 in Annexes AD and AE. The simultaneous-row argument is proved in Annex AF, Theorem BD.2.


---
