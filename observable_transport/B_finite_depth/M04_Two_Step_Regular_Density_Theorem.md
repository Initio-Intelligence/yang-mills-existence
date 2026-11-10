# The old Q-density correction survives a second regular integration

This note combines the first Q-defect expansion, the actual second analytic base, the constrained core-frame application and the exact merged-core normalization.

## 1. Exact operation and conclusion

Use the two homogeneous native P/Q-regular regions, both equal to the full lattice. Perform the first mass-weighted R average of RA, and then apply the new full-lattice physical averaging operation of BA.5a, summing its R partition as well. This is the explicitly specified averaged route. It is not an assertion that the original history-dependent future kernels are sufficient after their R labels have been erased.

Let `g_0,g_1` be the integrating couplings, `W=V_2`, and `P_0=delta_0/g_0`. Retain the same source hierarchy and bounded adjacent coupling ratios as the preceding proofs. Let

\[
 D_1(a;W)=
   \exp\{-\tfrac12 a^TK_1(U_2(W))a+W_1(a;U_2(W),J_2(W))\}.
 \tag{TD.1}
\]

This is the complete smooth inherited second normal form from BA. It includes the first effective-action difference, next classical and gauge remainders, Haar, exceptional-bond coarea and constraint Jacobians. Its precision is the actual force-corrected inherited one. All retained-only factors are kept in `C_1(W)` below.

With the exact constrained reconstruction `Psi_W`, define

\[
 Z_{PQ,2}(W)=\int\chi_{Q,1}(a,W)D_1(a;W)\,da,
\]
\[
 Z_{QQ,2}(W)=\int\chi_{Q,1}(a,W)D_1(a;W)
                  e^{\delta E_1(\Psi_W(a))}\,da,
 \qquad
 \delta E_1=\log(Z_{Q,0}/Z_{P,0}).
 \tag{TD.2}
\]

The first subscript records the first integration's P comparison or actual Q integral; both second integrals retain the actual next Q cutoff. These definitions use the actual Q radius, not the shrinking printed later R-good radius. On this native domain all real integrals are positive and finite. BA proves that the old selector is redundant on the full next Q fiber before its R split.

The two physical subdensities satisfy exactly

\[
 \rho_{PQ,2}=\chi_2 C_1 Z_{PQ,2},\qquad
 \rho_{QQ,2}=\chi_2 C_1 Z_{QQ,2},
\]
\[
 \rho_{QQ,2}=\rho_{PQ,2}e^{\Delta_2},\qquad
 \Delta_2(W)=\log\frac{Z_{QQ,2}(W)}{Z_{PQ,2}(W)}.
 \tag{TD.3}
\]

In particular

\[
 \Delta_2(W)=
 \log\mathbb E_{\nu^P_{Q,1}(\cdot\mid W)}
             e^{\delta E_1(V_1)}.
 \tag{TD.4}
\]

The logarithm is taken after the second integral. It is not replaced by an average of `delta E_1`.

For a connected tagged decomposition `E=sum_alpha E_alpha`, define the native anchored value/current norm by

\[
 \|E\|_{\kappa,\mathrm{anc},1}
 =\sup_b\sum_{\alpha:\,b\in Y_\alpha}
  e^{\kappa n(Y_\alpha)}
  \left(\sup|E_\alpha|
       +\sup_W\sum_d\sup_{0<|t|\le1}
                   |\delta^{\rm norm}_{d,t}E_\alpha(W)|\right).
 \tag{TD.5}
\]

Here `n(Y)` is the existing physical volume/tree size. Every carrier contains its true raw-W determining footprint. Suprema and elementary paths use the native second-step domain and the verified buffer. The direction normalization and couplings are specified. This is an unmarked-density norm, not a redefinition of the microscopic scalar's separate inherited records.

### Theorem TD.1 — two-step native density transport

For sufficiently small coupling there is a fixed positive carrier rate, independent of volume and coupling, for which

\[
 \boxed{\qquad
   \|\Delta_2\|_{\kappa,\mathrm{anc},1}
       \le C_L e^{-cP_0^2}.
       \qquad}
 \tag{TD.6}
\]

The constants may depend on the fixed group, L, two fixed native levels and the chosen strict localization margins. Every nonzero connected tag of `Delta_2` contains an old Q defect. Its two-layer integral representation keeps that defect's real domain and Gaussian reserve visible.

The whole vacuum logarithm can be extensive. The theorem does not imply a volume-independent bound on `|Delta_2|`, a whole-law total-variation bound, an ambient second-step theorem, full microscopic marked transport at the second step, or an all-depth induction.

## 2. The strict first-step payload budget

The QC connected logarithm gives the exact first correction as

\[
 \delta E_1(V_1)=\sum_{\tau}H_\tau(V_1).
 \tag{TD.7}
\]

The index retains the original logarithmic cluster and its individual localization choices. Each `H_tau` is a connected old payload with at least one Q defect. Keep its integral representation from NP, rather than replacing it by a bounded function. Write `n_tau>=1` for its old defect occurrences, including distinct latent copies when a logarithmic cluster contains products, and `r_tau` for its local old marginal rank.

The first QC proof supplies a strict *integrand* envelope: the analytic connector factors, their full supports and a positive Gaussian store are present before old integration. Its absolute sums still converge after a fixed small quadratic/rank tilt, a fixed carrier-rate loss and one first-current insertion. This is the reserve used in QC.18 and its connected expansion, not an additional estimate of a normalized output.

Concretely, denote the remaining connector envelope by `A_tau`. Allocating a smaller positive part of the first tail gives an anchored summable budget of the form

\[
 \sup_x\sum_{\tau:\,x\in X_\tau}
  e^{\nu n(X_\tau)}A_\tau e^{\eta_0 r_\tau}
                    e^{-c_0 n_\tau P_0^2}
       \le C e^{-c_1P_0^2},
 \tag{TD.8}
\]

with spare positive constants `eta_0,c_0,c_1` and a strict rate margin. The same statement holds for the decorated first-current envelopes after reducing those margins. This follows by retaining the individual defect tails in QC.18, applying the same rooted cluster majorant with slightly enlarged ordinary weights, and using the strict smallness of its ordinary and failed-P/Q species. Local ranks in repeated logarithmic factors are charged to their own activity envelopes; they are not bounded by the union volume while multiplicities are discarded.

The cap and carrier substitution in CA change a connector envelope by `exp(C q_new |X|)`, with `q_new -> 0`, and by a fixed two-level covering/collar conversion. Choose the final carrier rate below that converted native rate once. Analytic connectors receive no growing R halo.

Each old defect core does receive its next reference and frame buffer. Their union has size at most

\[
 C_L\Bigl(\sum_i n_{\tau_i}\Bigr)
                   (R_1/L+R_2+m)^4.
 \tag{TD.9}
\]

The positive tail margin in (TD.8) pays this size, since `P_0^2/R_1^4 -> infinity` and the adjacent R radii are comparable. A newly anchored coarse block can meet an enlarged core only when an old defect lies in its stated R-sized neighborhood. The resulting fixed-dimensional polynomial count is paid by the same spare tail. Thus the transformed old payload fugacities have an anchored decorated budget

\[
 \varepsilon_{\rm old}\le C_L e^{-c_2P_0^2}.
 \tag{TD.10}
\]

This budget already includes the growing core geometry, small rank losses, fixed raw-cover conversion and the permitted first-current costs. Its use below does not charge the original tail again.

## 3. Arbitrarily many old payloads share one next Gaussian integral

Expand the old exponential exactly at finite volume:

\[
 e^{\lambda\delta E_1(V_1)}
 =\sum_{m\ge0}\frac{\lambda^m}{m!}
       \sum_{\tau_1,\ldots,\tau_m}
                    \prod_{i=1}^m H_{\tau_i}(V_1).
 \tag{TD.11}
\]

The latent old integration variables in distinct factors are separate copies, conditioned on the same next real variable B. Coincident physical supports do not identify these copies or create extra independent physical rare events; they are the exact product-integral representation of (TD.11).

Merge all overlapping full core stencils. Use one common exact constrained frame on each merged component. CA.22 is uniform in real capped B and contains **no residual quadratic tilt in B per old payload**. Consequently the product bound at fixed B is

\[
 C^m\prod_{i=1}^m A_{\tau_i}\,
 e^{\eta\sum_i r_{\tau_i}}
              e^{-c\sum_i n_{\tau_i}P_0^2}.
 \tag{TD.12}
\]

The next Gaussian is then integrated once. Its single frame displacement is supported on the union S and has a per-coordinate bound independent of m. CA.23 therefore costs `exp(C|S|)` and one small next-rank loss. It does not cost `exp(C m |B|^2)`. Equation (TD.9) pays the union cost from the already allocated old budget. This is why (TD.11) can be summed without exhausting the next Gaussian reserve at high old-payload multiplicity.

The same reasoning applies to one first current: it differentiates one factor, one frame or one actual domain. CA.25 includes the old Q shells and the whole next Q shells on S, the complete inverse/determinant response and the measure terms. Rank and incidence polynomials use the reserved rate/tail margin. The factor counting the differentiated position is the usual derivative of an exponential generating series; it does not change the available anchored fugacity class.

## 4. One common component gas, including the old exponential

Let `z_gamma` denote the unmarked next-Q component activities of the analytic base. BA and CA supply their complete native common family; the generalized QC construction uses the auxiliary broad comparison radius only after exact R summation. Its ordinary activities and new Q defects obey a strict decorated anchored KP bound at the final carrier rate. The Gaussian normalization and retained-only classical factors are separated identically in every case.

Apply that same component expansion to (TD.11). Keep next Q whole on old core stencils, and expand cutoff alternatives only off them. The unnormalized product estimates (TD.12) and the common frame/covariance construction apply before assigning connected components. Every component containing no old payload is **exactly** a base activity `z_gamma`: CA's root-deletion identity checks the coordinate map, covariance, determinant, complete action and Q-reference domains, and CN.1 states the required equality. A disjoint component is not replaced by an approximately equal activity.

Let `u_gamma(lambda)` collect components containing at least one old payload. Their tags include the old occurrences, all analytic connectors, frame and Q-reference footprints, and outside-localization choices. Their supports are connected only when the component construction actually joins them. The exact partition functions, after the same common prefactor, are therefore

\[
 Z(0)=\sum_{\Gamma\ {\rm compatible}}
                      \prod_{\gamma\in\Gamma}z_\gamma,
\]
\[
 Z(\lambda)=\sum_{\Gamma\ {\rm compatible}}
               \prod_{\gamma\in\Gamma}
                       [z_\gamma+u_\gamma(\lambda)].
 \tag{TD.13}
\]

Separate species with the same carrier may be retained; the bracket is notation for their union. At physical endpoints, `Z(0)` and `Z(1)` are exactly the two integrals in (TD.2), with their identical prefactor removed. In particular, the full old exponential is included in the denominator gas at `lambda=1` whenever a conditional expectation under that law is formed.

Here is the quantitative summation needed for (TD.13). Use the strict first-step envelope (TD.8) and the CA joint product bound as additional colored input vertices in the next component expansion. Fixed-grid outside localization has the same Cauchy factors and connected-union weights as the base construction; old cores are initial vertices with the enlarged supports already paid in (TD.10). Summing the ordinary analytic vertices, and then the rooted overlap trees of ordinary and old vertices, is the same positive tree majorant as the source/QC component proof. Its input is the sum of the base budget and the old budget. The exact `1/m!` in (TD.11) is retained in this enumeration.

One can see the linear old smallness without a factorial estimate depending on m. Multiply every old input vertex by a nonnegative counting variable s. Choose a fixed small component budget `a_*` inside the base strict margin, and set

\[
 s_*={a_*\over\varepsilon_{\rm old}}\ge2.
 \tag{TD.14}
\]

Choose `a_*` small enough that this inflated input leaves the final decorated KP margin as well as the component-expansion margin. This is a uniform choice: the positive component/tree series converges on a fixed larger input neighborhood and is continuous there in the old intensity, its old-containing part vanishes at zero old intensity, and the base output has a strict decorated KP margin. The same fixed choice therefore works for every sufficiently small coupling and every volume.

At s=s_* the total input budget is still inside that common convergent majorant and its output remains inside the reserved decorated KP bound. The anchored component sum is bounded by a fixed constant, including its reserved carrier weight and first-current decoration. Its subseries containing an old vertex has nonnegative majorant coefficients and every term has degree at least one in s. Returning to s=1 therefore gives a factor at most `s_*^{-1}`. It follows that

\[
 \sup_b\sum_{\gamma:\,b\in Y_\gamma}
 w_\kappa(Y_\gamma)e^{a|Y_\gamma|}
 \left(\sup_{|\lambda|\le1}|u_\gamma(\lambda)|
                    +t_*\,\text{its first-current envelope}\right)
       \le C\varepsilon_{\rm old}.
 \tag{TD.15}
\]

The counting variable multiplies already bounded old integral vertices. It does not modify the next Gaussian action or spend a new Gaussian reserve. The uniformity in m proved in Section 3 is essential for using the same majorant at s_*.

This derives the smallness of the added unmarked core activities. It does not assume a normalized marked bound or normalize each core separately. The sum of base and added activity budgets satisfies the same strict decorated KP criterion for all `|lambda|<=1`, with room to spare.

## 5. Connected logarithm and proof of the theorem

Take the absolutely convergent connected logarithms of (TD.13). Their difference contains exactly those colored clusters with at least one old-core activity. A cluster containing only base activities cancels coefficientwise. Each surviving cluster has a genuine connected union carrier.

The weighted hard-core rooted tree bound applies to the sum of the base and old activity envelopes. To retain the old smallness, use the same old counting parameter s as above inside its fixed strict margin. The anchored connected-cluster majorant remains bounded at s_*, while its old-containing subseries starts at degree one. Its value at s=1 is therefore at most `C/s_*`. Equivalently one may distinguish an old vertex and use the rooted tree recursion with the base's strict susceptibility margin.

By (TD.10), this proves

\[
 \sup_b\sum_{\alpha:\,b\in Y_\alpha}
          w_\kappa(Y_\alpha)\sup|\Delta_{2,\alpha}|
       \le C_L e^{-cP_0^2}.
 \tag{TD.16}
\]

For finite raw currents use endpoint telescoping on the same tagged cluster series and the decorated KP majorant. A current on a base factor retains the old factor in its cluster; a current on an old factor has CA.25's old reserve. The incidence polynomial is paid by the already reserved carrier-rate margin. The same old counting argument proves the current part of (TD.6).

CN.10–CN.24 gives the equivalent normalized insertion calculation. Its excluded-vacuum factor is computed from the **full same gas** appropriate to the chosen lambda. It restores exactly the denominator response and its supports. No inverse core mass or whole-volume all-good probability is introduced.

Equation (TD.3) restores the common physical density factors. This completes the proof of Theorem TD.1. The resulting coefficient integrals retain their old and next real domains and latent variables; the proof makes no raw-W holomorphy assertion for them. ∎

## 6. What this establishes toward the iteration

The old first-Q density correction can pass through one further actual homogeneous regular physical integration with its rare factor, true carriers and first native currents intact. The full old-source exponential, including its unmarked core species, is present in the next normalization. This is stronger than the exact positive pushforward alone or a bound for one unnormalized core.

The completed theorem is still a two-step statement. Its current buffer, raw covering constants and reserve allocation have been verified at two fixed levels. It supplies neither a depth-independent recursive class nor the complementary P/Q sectors. It also does not prove the second-step microscopic marked scalar theorem, all second-step source jets, the full physical connected hierarchy or the continuum/nontriviality conditions for Yang--Mills existence. Those conclusions cannot be inferred from (TD.6) alone.

The original fixed-history M04 statement remains unchanged and uncompleted. The present result belongs to the explicitly different R-averaged density route.

## Proof dependencies

* RA and QC: the exact first R average, first density identity, strict connected Q-defect expansion and retained Gaussian reserve.
* NP: original Q cores, exact physical fiber coordinates and the local real-domain integration formulation.
* BA: the actual second inherited action, force-corrected soft-gauge precision, complete native analytic family and full-Q old-selector redundancy.
* CA: the common raw background/frame construction, native admission, joint covariance/determinant estimate, product old reserve, component identities and local first currents.
* CN: exact normalization against the same unmarked gas, weighted excluded-vacuum carriers, current records and forest bookkeeping.
