# The complete two-step regular density relative to a broad analytic comparison

This is a corollary of the specified second-step primitive application CA and the combined density theorem TD. It adds the new Q-defect correction to the transported old correction. The operation is the same new physical averaging operation used in BA/CA/TD, with both homogeneous P/Q-regular regions equal to the full lattice and each R partition summed with its actual mass. It is not the original fixed-history operation after erasing its labels.

## 1. Definitions and exact identity

Use the complete inherited smooth density of TD.1,

\[
 D_1(a;W)=\exp\{-\tfrac12 a^{\mathsf T}K_1(U_2(W))a
                         +W_1(a;U_2(W),J_2(W))\}.
 \tag{AD.1}
\]

Its precision includes the source force/constraint correction and averaged soft gauge. Its perturbation includes the inherited analytic effective action, classical and gauge remainders, Haar, exceptional-bond coarea and the other source Jacobians. Keep all retained-only terms in the **same** factor `C_1(W)` as TD.3.

Let `delta_1` be the physical next Q threshold, and put

\[
 P_Q=\delta_1/g_1,\qquad P_{\rm aux}=c_*P_Q,
 \tag{AD.2}
\]

where the fixed positive `c_*` is chosen sufficiently small as in BA.18b. In particular it may be decreased once to leave a strict containment margin larger than two between the auxiliary ball and the boundary of every local-frame Q domain. This does not change the source operation. The auxiliary cutoff is introduced only after its R partition has been summed. **It is not the printed later R-good radius in CMP119 (3.16).**

With the same Lebesgue/Haar-normalization convention in all three integrals, define

\[
 Z_{{\rm aux},2}(W)=
       \int\prod_e\mathbf1_{B_{P_{\rm aux}}}(a_e)D_1(a;W)\,da,
 \qquad
 \delta E_{{\rm new},2}(W)=
       \log\frac{Z_{PQ,2}(W)}{Z_{{\rm aux},2}(W)},
 \tag{AD.3}
\]

where `Z_{PQ,2}` and `Z_{QQ,2}` are exactly TD.2. All integrals are positive on the admitted real native domain. Define

\[
 \rho_{{\rm aux},2}=\chi_2 C_1 Z_{{\rm aux},2},
 \qquad E_2=\delta E_{{\rm new},2}+\Delta_2.
 \tag{AD.4}
\]

Then the physical density identity is exact:

\[
 \boxed{\rho_{QQ,2}=\rho_{{\rm aux},2}\,e^{E_2}.}
 \tag{AD.5}
\]

Indeed the two positive ratios telescope:
`Z_QQ,2/Z_aux,2=(Z_QQ,2/Z_PQ,2)(Z_PQ,2/Z_aux,2)`.
The old correction is still TD's logarithm **after** next integration; it has not been replaced by its conditional average. No retained-only factor or normalization is dropped.

## 2. New Q correction with the inherited precision

### Proposition AD.1

On the same native two-level domain and buffered elementary paths as CA/TD, for a fixed positive carrier rate,

\[
 \|\delta E_{{\rm new},2}\|_{\kappa,{\rm anc},1}
                 \le C_L e^{-cP_{\rm aux}^{2}}.
 \tag{AD.6}
\]

The norm is precisely TD.5: the sum of absolute individual connected raw-W carrier tags, with value and once-normalized raw-current envelopes. Every new nonzero tag contains a new Q defect. Constants may depend on the two fixed levels and the fixed source conventions, not on total volume or coupling.

**Proof.** The generalized QC application is already established in CA Section 7. The following records explicitly why changing the comparison radius to (AD.2) preserves each of its primitive inputs.

First, BA.18a bounds the difference of the actual next saddle and every literal local Q reference by `C epsilon_1 exp(-cR_2)=o(delta_1)`. On an independent starred slot the free link is exactly `exp(i g_1 a_e)V_{*,e}`. Thus the physical Q domain is contained in a ball of radius `(2+o(1))P_Q`, and contains a fixed small ball of radius proportional to `P_Q`. This concerns the complete intersection of all overlapping tests at that slot. In a compact component-local frame, CA.10 adds only a bounded normalized displacement tending to zero. After fixing `c_*` small enough and then the coupling, the resulting real domain contains `B_{2P_aux}` and lies in `B_{C_L P_aux}`. The group norm and the source Lie-algebra norm have fixed local comparison constants. No lower margin for a *forced conditional mean* is used.

Second, CA Sections 2 and 5 supply the actual inherited, raw-supported complete coefficient family. The covariance is the positive Gram/marginal family with one matrix generating both its inverse and determinant. Its complex discrepancy is tunably small with the fixed ordinary localization buffer. Its component restrictions, the exact constrained frames and every Q reference have the same full raw carriers. The first raw-current envelopes are part of CA.5, CA.17 and CA Section 7. These are the inputs to QC; the bare first-Wilson precision is not substituted for `K_1`.

Third, use exactly the finite identity in each slot

\[
 \rho_e=1+(\mathbf1_{B_{P_{\rm aux}}}-1)
                       +(\rho_e-\mathbf1_{B_{P_{\rm aux}}}).
 \tag{AD.7}
\]

The last alternative is represented in its compact local frame by its annulus and homotopy boundary chain, as in QC.17. The annulus is at radius at least `P_aux`; the side chain is at radius at least `2P_aux-O(1)`, with bounded imaginary displacement. More precisely, the actual Q upper radius `(2+o(1))P_Q` and the bounded, indeed vanishing, normalized frame displacement put the local domain and its entire homotopy below `3P_Q+O(1)<3.5P_Q` at small coupling. Thus they lie on the identity plateau of CA's coefficient cutoff; the smaller `P_aux` is not used to choose that plateau. The Gaussian quadratic itself is never capped. These choices leave the physical Q and auxiliary integrals unchanged. The native geometric tube is available because `g_1P_Q=delta_1` tends to zero.

For a term with n new Q defects, the complete normalized Gaussian majorant and exact ordinary integration therefore give

\[
 C^nP_Q^{Cn}\exp(\eta r_I)
                       e^{-c nP_{\rm aux}^{2}}.
 \tag{AD.8}
\]

Here eta is the tunably small rank-loss coefficient, and `r_I` is the local marginal rank. The fixed constant per slot is paid only on the defect marginal; no `C^{r_I}` factor is introduced. All interactions and coarea factors use their inherited strict Gaussian and spatial reserve from BA/CA.

Only a new Q defect acquires its full Q-reference box and its growing frame halo. Ordinary analytic supports receive the fixed ordinary collar. The source hierarchy and the fixed fraction in (AD.2) imply

\[
 P_{\rm aux}^{2}/R_2^4\longrightarrow\infty.
 \tag{AD.9}
\]

Consequently the spatial footprint, the fixed-dimensional shell/chain factors, and the polynomial current incidences are paid by a fixed fraction of the tail in (AD.8). The outside grid and its parameter radius remain fixed, as in QC.6--QC.25. The resulting common component gas has a strict decorated KP margin.

Take the connected logarithms of the Q and auxiliary gases using their common regular/failed-auxiliary registry. Their difference contains at least one new Q-defect species in every cluster. The positive rooted cluster majorant gives (AD.6) for values. For first raw currents use real shells for the moving Q factors and the same exact inverse/determinant and complete interaction currents. The auxiliary ball has no raw-W motion, since coupling and radius are specified. Each current cluster still contains a new Q defect, and its polynomial cost is paid from the same reserved tail/rate margin. This proves (AD.6). No probability of a whole-volume all-good event has been divided out. ∎

## 3. The complete two-step decomposition

Combining AD.6 with TD.6, and taking a common smaller positive carrier rate, gives

\[
 \boxed{\quad
 \|E_2\|_{\kappa,{\rm anc},1}
       \le C_L\left(e^{-cP_0^2}
                         +e^{-cP_{\rm aux}^{2}}\right).
 \quad}
 \tag{AD.10}
\]

The addition uses the separate connected tag lists; it does not require cancellation between their absolute norms. The base `rho_aux,2` is the smooth analytic comparison produced by the inherited small-field construction with a fixed free-coordinate product domain. The real coarse selector `chi_2` is displayed separately. As usual its whole logarithm can be extensive; (AD.10) is an anchored density statement.

This completes a native two-step analytic-base decomposition for the specified R-averaged regular operation. It does not provide an ambient second-step extension, complementary P/Q sectors, all-depth closure, or the microscopic marked theorem at the second step. The two corrections retain their different defect births and their parametric integral representations. In particular AD.10 does not authorize treating their sharp-domain dependence as raw holomorphic input at a third step.

References: BA.5a, BA.14--BA.18b; CA.1--CA.25, especially Section 7; QC.17--QC.28 and its common connected logarithm; TD.1--TD.16.
