# Weighted averaging on a finite mixed list has a polynomial analytic radius

This note proves a concrete uniform-in-depth estimate needed to use the promoted raw master list. It does not replace a mixed field by a uniform fine-field sup norm. It also distinguishes Balaban's new, gauge-corrected average from the literal chronological average: the inverse axial gauge is retained at the end.

The input is a current-regular real reference U_* on a buffered box B, and a microscopic relative field `exp(iηA)U_*` whose normalized size on each native cell Q is `|A|≤δ/h_Q`. The box is covered by at most D such native cells, with `h_Q≥η`; all averaging footprints under consideration are included. The number n of averaging levels is at most D. In the first-reset application this is the finite common-refinement list with n≤N+1 and D=O(R^5), N=R. A further application to a variational minimum uses the actual source Proposition 9 to obtain precisely this weighted A bound from small master raw data.

## 1. Keep the physical normalization in the averaging kernels

Let `ℓ_j=L^jη`. Write the relative logarithm at level j as

\[
 a_j=\ell_j A_j,
\]

so a_j is a bond angle and A_j is a physical one-form. In CMP98 (122), the factor L is exactly the conversion from the input angle to the output angle. The normalized linear operator Q acts on physical one-forms.

On the flat background, the positive scalar majorant of the main operator (125) is

\[
 (Qf)_c=L^{-(d+1)}\sum_{x\in B(c_-)}
                  \sum_{b\in[x,x+Le_\mu]} f_b,
 \qquad c\parallel e_\mu.
 \tag{WA.1}
\]

The fine path has L bonds and there are L^d starting points. Thus each row sums to one. For a fixed fine μ-bond b, precisely L translated starting points have their forward length-L path passing through b, counting the adjacent coarse blocks together. Each starting point belongs to exactly one block. Therefore

\[
 \sum_b Q(c,b)=1,\qquad
 \sum_c Q(c,b)=L^{-d}.
 \tag{WA.2}
\]

These are counting-measure matrix identities; the second is the ratio of fine to coarse cell volumes. On a restricted footprint the corresponding sums only decrease, provided the required halo is retained. Lie-algebra components are bounded in a fixed invariant norm; the main background parallel transports have norm one on the real reference. Their absolute operator is consequently bounded by (WA.1).

The positive error kernel used in CMP98 (140) is, up to a fixed component constant,

\[
 (Q''f)_c=L^{-d}\sum_{b\subset B(c_-)\cup B(c_+)} f_b.
 \tag{WA.3}
\]

A row contains only `C_L L^d` bonds, and a fixed fine bond belongs to the two-block footprint of at most a fixed `C_L` coarse bonds. Hence

\[
 \sup_c\sum_b Q''(c,b)\le C_L,\qquad
 \sup_b\sum_c Q''(c,b)\le C_LL^{-d}.
 \tag{WA.4}
\]

All constants include the fixed dimension and stencil conventions. Their size does not depend on the number of levels.

### Lemma WA.1: an arbitrary insertion word

Consider n successive scale changes, with Q at n−m places and Q'' at m places. Let K_w be their product, in the true scale order. Positivity, (WA.2) and (WA.4) imply

\[
 \sup_c\sum_b K_w(c,b)\le C_L^m,
 \qquad
 \sup_b\sum_c K_w(c,b)\le C_L^mL^{-dn},
 \qquad
 0\le K_w(c,b)\le C_L^m(\eta/\ell_n)^d.
 \tag{WA.5}
\]

**Proof.** The row-sum norm and the column-sum norm are each submultiplicative for nonnegative matrices. A Q contributes 1 to the row norm and exactly `L^{-d}` to the column norm. A Q'' contributes at most C_L and `C_LL^{-d}` respectively. Their products give the first two bounds; each matrix entry is bounded by its column sum. ∎

There is no factor `C_L^n` in this lemma. In physical measure notation, the last bound is an integral-kernel bound `C_L^m ℓ_n^{-d}` against the microscopic measure `η^d`. It is incorrect to omit that measure factor or to treat every native coordinate as a finest-scale coordinate.

The support of every such word lies in a fixed enlargement of the two terminal blocks. At level j a step adds a fixed multiple of ℓ_j to the footprint. The sum `Σ_{j<n}ℓ_j` is bounded by `C_Lℓ_n`, so the enlargement is independent of n.

## 2. What a native cell contributes

Suppose `|A(b)|≤δ/h_Q` for bonds in Q. There are at most `C(h_Q/η)^d` such bonds. Using the entry bound in (WA.5) and then multiplying by ℓ_n to convert back to the output angle gives

\[
 \ell_n K_w(|A|\mathbf1_Q)
       \le C C_L^m\delta (h_Q/\ell_n)^{d-1}.
 \tag{WA.6}
\]

Using the row bound instead gives `C_L^m δ ℓ_n/h_Q`. Combining them,

\[
 \ell_n K_w(|A|\mathbf1_Q)
 \le C C_L^m\delta\,
       \min\{(h_Q/\ell_n)^{d-1},\ell_n/h_Q\}.
 \tag{WA.7}
\]

Both factors in the minimum are dimensionless. In d=4 the first is the cubic suppression `(h_Q/ℓ_n)^3`. Summing at most D cells gives

\[
 \|\ell_n K_w|A|\|_\infty
              \le C C_L^m D\delta.
 \tag{WA.8}
\]

This estimate is deliberately coarse but sufficient. In particular it is uniform when the finest mesh tends to zero at fixed counted native list. A uniform bound `|A|≤δ/h_min` would lose exactly this feature.

## 3. The exact one-step nonlinear majorant

Use the new relative averaging operation of CMP98 (63), (88), whose logarithm is Q(V_0,a) in (121). Proposition 3, (122)–(124), gives

\[
 a_{j+1}=LQ(U_{*,j})a_j+C(U_{*,j},a_j),
 \tag{WA.9}
\]

where C(0)=DC(0)=0. The reference U_* is current-regular. Proposition 2 therefore bounds the plaquette ceiling at level j by

\[
 \alpha_j\le C\varepsilon_* (\ell_j/H)^2,
 \qquad \sum_{j<n}\alpha_j\le C\varepsilon_*.
 \tag{WA.10}
\]

Here H is the current scale and all ℓ_j≤H. The inequality (139) gives

\[
 |Q(U_{*,j})f|\le Q|f|+C_L\alpha_j Q''|f|.
 \tag{WA.11}
\]

On a fixed small complex angle ball, the one-step remainder is analytic with its fixed finite two-block stencil. The local Cauchy bound and `DC(0)=0` give, for `||a_j||∞≤r` in a fixed smaller ball,

\[
 |C(U_{*,j},a_j)_c|
       \le C_L r\sum_{b\text{ in its stencil}}|a_j(b)|
       \le C_L r\,(Q''|a_j|)_c.
 \tag{WA.12}
\]

The last C_L includes the fixed factor L^d. This bound holds for complex variables, with a reference in the stated real regular class; it follows by integrating the analytic first derivative along the radial segment. Divide (WA.9) by `ℓ_{j+1}=Lℓ_j`. Equations (WA.11)–(WA.12) imply the physical-field majorant

\[
 |A_{j+1}|\le
       [Q+C_L(\alpha_j+r)Q'']\,|A_j|.
 \tag{WA.13}
\]

No growing power of the ratio of the native meshes enters this one-step inequality.

Expand the finite product of (WA.13). A term with m insertions has the coefficient `∏_{j∈S}C_L(α_j+r)` and the word bound (WA.8). Summing subsets gives

\[
 \|a_i\|_\infty
 \le C D\delta\prod_{j<i}[1+C_L(\alpha_j+r)]
 \le C_0 D\delta\exp(C_Lri),
 \qquad i\le n,
 \tag{WA.14}
\]

as long as the preceding angles are at most r. The constant C_0 includes `exp(C_LΣα_j)` and is uniform for the fixed small reference ceiling.

## 4. Complex bootstrap and Cauchy estimates

Choose `r=2C_0Dδ`. If

\[
 \delta\le c/[D(n+1)]\quad\text{and hence, sufficiently,}\quad
 \delta\le cD^{-2},
 \tag{WA.15}
\]

with c small depending only on the fixed source constants, then `C_Lrn≤log(3/2)` and r lies in the one-step analytic ball. Starting at the first level, (WA.14) gives `||a_i||≤(3/2)C_0Dδ<r`. This closes the induction at every level. Thus every intermediate composition is actually defined in the complex domain, and

\[
 \boxed{\quad
 \|a_i\|_\infty\le C D\delta\quad(0\le i\le n),
 \qquad \delta\le cD^{-2}.
 \quad}
 \tag{WA.16}
\]

This is an analytic-domain statement, not just a real derivative estimate. All intermediate logarithm branches are the branches continuously fixed at A=0.

For an application to master raw data B, take the actual current reference U_* and set `V_*=M_master(U_*)`. The constraint fiber for the master data is contained in the current retained fiber. Uniqueness of the regular minimal orbit therefore gives `U_master(V_*)=U_*`, in the matched reference gauge. CMP102 Proposition 9 and its fixed-point estimates give an analytic Landau field A(B) with

\[
 \|h_Q A(B)\|_{Q,\infty}\le C\|B\|_\infty.
 \tag{WA.17}
\]

The source uses its new averaged constraint Q in this gauge. Apply (WA.16) to A(B), choosing the constant in (WA.15) smaller. The resulting new-average readout f has f(0)=0, is analytic on `||B||∞<cD^{-2}`, and satisfies `||f(B)||≤CD||B||`. Cauchy consequently gives, for its m-linear derivatives,

\[
 \|d^mf(0)\|\le m!C^mD^{2m-1},
 \qquad
 \|f(B)-df(0)B\|\le CD^3\|B\|_\infty^2
 \tag{WA.18}
\]

on a fixed smaller ball. Constants absorb the usual polarization factor. The bounds are in the maximum norm on the finite master list, not in a norm which silently counts all microscopic sites.

## 5. Return to literal raw averages; retain the axial gauge

The new relative average is not the raw chronological average of the same field in its original gauge. CMP98 (69)–(77), (87) and (104)–(106) give the exact conversion. Each inverse axial gauge matrix is a product, in its true order, of at most n native-scale factors. A factor is a relative contour transport or its group average over a block at that level, with a fixed number of bonds depending only on L. At that level the new angle is bounded by r from (WA.16). Reference transports act by unitary conjugation. Hence every factor differs from I by at most `C_Lr` on the real domain and obeys the same analytic bound in the complex domain. Its product satisfies

\[
 \|u-I\|\le \exp(C_Lnr)-1\le C_Lnr
                     \le C D^2\delta.
 \tag{WA.19}
\]

For the local group means the estimate follows from their analytic near-diagonal domain and endpoint covariance. It uses the actual source group mean, not a substituted single contour. Choosing c in (WA.15) small keeps the whole product and its inverse in a common fixed complex neighborhood. The same bound applies to the relative matrices at the endpoints of any readout bond.

Use these endpoint matrices in the exact transformation law (69)–(71). The literal raw readout F, in the matched original axial gauge, is therefore analytic on the same radius `cD^{-2}` and has

\[
 \|F(B)-F(0)\|\le C D^2\|B\|_\infty,
 \qquad
 \|d^mF(0)\|\le m!C^mD^{2m},
 \tag{WA.20}
\]

where F denotes its relative small logarithm when a Lie-valued output is needed. In particular

\[
 \|F(B)-F(0)-dF(0)B\|
                    \le CD^4\|B\|_\infty^2.
 \tag{WA.21}
\]

The inverse gauge was counted once as an ordered product. Bounding each stage by an unrelated constant and multiplying those constants would incorrectly produce a `C^n` loss. Likewise, treating the new Q average as the raw chronological readout without the endpoint matrices would omit a genuine source operation.

With normalized input `B=g_k z`, `||z||≤P_cap` and `g_kP_cap≤cD^{-2}`, division of the Lie-valued readout by the appropriate comparable coupling gives the concrete Taylor error

\[
 \boxed{\quad
 \|T(z)-T(0)-L_Tz\|
                  \le Cg_kD^4P_{\rm cap}^2.
 \quad}
 \tag{WA.22}
\]

Thus a fixed logarithmic P_cap times any fixed power of D gives an error smaller than the unchanged preparation thresholds at sufficiently small coupling.

## 6. Finite compositions and the actual remaining obligations

One may compose this primitive readout with a target mixed minimum directly. The target minimum is evaluated on the original raw data reconstructed from the master list, not on N successive inverse fluctuation charts. Its Proposition 9 domain is uniform. A subsequent raw readout uses (WA.20) again. For example, a chain of two such readouts/minimum operations has a sufficient master radius `cD^{-4}`, output bound `CD^4||B||`, and quadratic error `CD^8||B||²`. More generally a fixed number q of these operations costs only a fixed power of D. This statement follows by choosing the input radius so that each of the q intermediate outputs lies in the next declared domain; q is not replaced by the RG waiting depth.

Local logarithms, the genuine exceptional-bond constraint inverse, and the endpoint-covariant normalized gauge substitutions MT.14 have fixed local analytic domains. Ordered products of at most O(D) near-identity relative gauge factors cost an additional polynomial factor by the same argument as (WA.19). These observations identify the route for a finite catalog of actual selector maps. Every catalog entry must keep its true source gauge, reference offset and fixed terminal constraints.

This note closes the weighted averaging step and its actual axial conversion. It does not certify that every selector in two arbitrary histories has already been written as a uniformly bounded number of these primitives. Nor does it remove the exact terminal higher-average deltas on the promoted master data. A common Gaussian quotient and its complete coarea density require their own construction. The common density oscillation is needed only on the actual union by CE.9a; no inherited E/B analytic extension outside that union is asserted here.

## Primary sources

- CMP98, printed pp.34–36, (109)–(126): the actual new average, one-step analytic remainder and its main positive parallel-path kernel.
- CMP98, printed pp.37–41, (127)–(153), especially (139)–(147): composition, the Q'' kernel and physical-measure bounds. The exact column-sum argument above makes explicit the measure factors used in the mixed-cell application.
- CMP98, printed pp.29–33, (69)–(88), (104)–(106): conversion between the new average and the literal relative field by its inverse axial gauge.
- CMP102, printed pp.280–281, (19)–(21), and pp.305–309, (172)–(190), Proposition 9: the actual mixed weighted variational field and its analytic dependence.
- [mixed tree chart](mixed_tree_chart.md): the finite native cell count, boundary-preserving physical chart, exact Haar change and the retained normalized soft axial variables.
- [M04 Two List Common Refinement](M04_Two_List_Common_Refinement.md): the original raw/free lists and the promoted-master construction; terminal average constraints remain explicit.
