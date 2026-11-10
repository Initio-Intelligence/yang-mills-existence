# Rectangular second-step currents: an admitted fixed-domain family and the remaining QQ frame gate

This note keeps the canonical current filing of MS.23a–24. It proves real rectangular admission and the structural three-copy family when the first conditional law is P. It also identifies the exact compatibility condition missing from a direct reuse of the diagonal CA frame for full QQ transport. The obstruction below concerns that particular simultaneous-frame construction; it is not an impossibility theorem for canonical QQ currents.

## 1. Actual rectangular data and real admission

Use the same two homogeneous regular levels as BA/CA. Couplings, gauges, coordinate charts and grids remain fixed. Let

\[
 W(\theta)=\tau_{d,\theta}W,\qquad |\theta|\le1,
                                                        \tag{RC.1}
\]

be a buffered elementary retained path at the final level. Its physical link displacement is O(g2). Insertion and kernel copies are any real points of this same path. The next free variable a is in the actual Q fiber of the kernel copy. The full-fiber bound is the one using P_Q, not the smaller auxiliary comparison radius:

\[
 |a_e|\le(2+o(1))P_Q.                              \tag{RC.2}
\]

### Lemma RC.1 — old admission across a buffered elementary rectangle

For sufficiently small coupling, every field

\[
 V_1^{I}=\Psi_{W_I}(a),\qquad
 a\in Q(W_K),                                    \tag{RC.3}
\]

is admitted for the first regular P and Q conditional kernels, uniformly in the insertion and kernel points W_I,W_K on (RC.1). The same holds for any third copy W_M on this path. This statement does not assert that a belongs to Q(W_I).

**Proof.** CA.5 gives a summed normalized derivative budget for the actual next saddle. Include the local face lift and the full fixed-L exceptional solve in the reconstruction. On the bounded physical free-coordinate tube g1|a|<=C g1 P_Q, these analytic maps and their first derivatives have uniform fixed-depth bounds. At a starred free link the identity is exactly

\[
 \Psi_{W,e}(a)=e^{ig_1a_e}V_{*,e}(W).             \tag{RC.4}
\]

Exceptionals are obtained from the actual fixed-target local solve. Thus a single normalized W perturbation changes every required physical reconstruction link by at most C_L g2 times the path length. The supported coefficient bound also gives a summable column estimate: a coefficient responding at an output e to the varied input d contains both footprints, so its carrier weight bounds its response by an exponentially summable function of their distance. Consequently

\[
 \sup_e\|\Psi_{W_I}(a)_e-\Psi_{W_K}(a)_e\|
       \le C_Lg_2|\theta_I-\theta_K|,
\]
\[
 \sum_e {\|\partial_\theta\Psi_{W(\theta)}(a)_e\|\over g_1}
       \le C_L.                                  \tag{RC.5}
\]

All fixed readout and gauge footprints are included. This uses the common coefficient family, not an unproved inverse reconstruction estimate.

At W_K, source CMP119 (3.7)–(3.9), printed p.266, gives a fixed strict margin in the old local curvature and axial tests on the entire next Q fiber. In (3.8) the next curvature contribution is reduced by L^{-2}, and the remaining term can be kept a fixed fraction below the old threshold by the source A1/A0 choice. Therefore the left sides are at most theta_* epsilon1 with theta_*<1 fixed. This is the same slack used in BA.16; the calculation precedes the next R split.

The first local minimizing maps and local gauge readouts have uniformly summed native first derivatives on their buffered geometric tube. Applying those bounds to (RC.5) changes the old test quantities by at most C_L g2. The ratio g2/epsilon1 tends to zero, since adjacent coupling ratios are bounded and epsilon1/g1 is the source logarithmic window. Choose g so that this change is less than half the old slack. The old tests remain strictly true for V1^I, including each literal local determining box. The old Q normalizer is then positive by the first regular construction. The auxiliary P case is contained in the same argument. ∎

This proves admission on real rectangles. It does not make a sharp Q domain holomorphic in either raw retained copy.

## 2. A genuine three-copy family for first P, second P or Q

Let q0,P(dz|V) be the actual normalized first P conditional law, including its Gaussian, all measure/coarea factors and normalizer. Let q1,eta(da|W1) be the normalized second analytic-base law with eta equal either to the fixed auxiliary P cutoff or to the actual next Q cutoff. The first P density has already been incorporated once in this second analytic base, as in BA/TD.

For a microscopic scalar F, define the real three-copy family

\[
 \mathcal A(W_M,W_0,W_1)
 =\int q_{1,\eta}(da\mid W_1)
       \int q_{0,P}(dz\mid\Psi_{W_0}(a))
       F\bigl(\Phi_{\Psi_{W_M}(a)}(z)\bigr).
                                                        \tag{RC.6}
\]

Its source version replaces F by exp(sum t_j F_j) and takes the outer logarithm after both integrations. All gauge-preimage factors required by the actual physical kernel are retained; they are harmless normalized factors for these gauge-invariant microscopic marks.

At the diagonal (RC.6) is the exact first-P/second-eta microscopic conditional field. It is not a new physical law at off-diagonal copies; it is the explicit insertion/kernel filing needed for the canonical finite differences. Lemma RC.1 makes all its real conditional laws actual admitted laws on the required rectangles. No reference-point extension is used there.

Write W'=tau_{d,t}W. The exact telescoping is

\[
 \mathcal A(W',W',W')-\mathcal A(W,W,W)
 =\bigl[\mathcal A(W',W',W')-\mathcal A(W,W',W')\bigr]
\]
\[
 \quad+\bigl[\mathcal A(W,W',W')-\mathcal A(W,W,W')\bigr]
 +\bigl[\mathcal A(W,W,W')-\mathcal A(W,W,W)\bigr].
                                                        \tag{RC.7}
\]

The first bracket is the lifted old insertion/reconstruction record, the second is the lifted old normalized-kernel record, and the third is the new normalized-kernel record. The first two together give the next insertion-copy variation, while their old origins remain separately tagged. The same endpoint identity applies coefficientwise to the conditional source logarithm. This does not move an old kernel record into a newly invented direct record by cancellation.

### Lemma RC.2 — fixed-domain inner analyticity with a single moving outer Q family

For eta=P_aux all integration domains in (RC.6) are fixed. For eta=Q, the only moving cutoff domains belong to the outer kernel copy W1. A common localization family may fix those Q domains by the existing QC frame while continuing both inner copies analytically on its outside-parameter and contour domains.

**Proof.** Use the actual W1 Q-frame and coordinate map a=A_s(B;W1) on its defect stencils. Keep all complete W1 Q-reference boxes and the declared growing defect halo. The inner kernel field is

\[
 \Psi_{W_0,s_0}(A_s(B;W_1)),
\]

and the mark field uses W_M and its common registry in the same way. There is no first Q cutoff in either inner integral. Its z-domain is the fixed first P ball, so neither inner field needs to be specified on an old moving-Q core.

On the physical real outer support, the cap is the identity and Lemma RC.1 gives actual old admission. On the auxiliary and contour family, the outer physical free angles are bounded by C g1 P_Q, their imaginary displacements are O(g1), and the two real-copy changes are O(g2). The background corrections remain O(epsilon2) on their fixed outside polydiscs. Consequently every inner field has geometric size bounded by

\[
 C_L(\epsilon_2+g_1P_Q+g_2),                    \tag{RC.8}
\]

including its stated complex continuation. This tends to zero and lies strictly inside the fixed first native geometric tube. The inner old fluctuations have physical size O(g0 P0), also inside that tube.

The coordinate caps are fixed real functions, independent of the retained copies and outside parameters. They equal the analytic identity on moved coordinates; unmoved capped coordinates remain real. No smooth ambient retained-field guard is evaluated on complex data. Thus the complete inner action, reconstruction, normalized Gaussian and coarea coefficients have the same admitted analytic continuation. The inner P normalizer is retained through its actual source-free connected construction, not bounded by a pointwise inverse of a whole-volume good-event probability.

Use one common outside grid and the union of all ordinary carriers from all three copies. Their local composition has only fixed collars. A growing halo is assigned only to a genuine outer Q defect. On separated components, the common coefficient restrictions, covariance and determinant branch agree with the independent component construction. The extra retained copies merely give different values to the same raw-coordinate registry; they do not introduce a new history flag or an unrecorded dependency.

The outside/source polydiscs can be chosen uniformly for both real endpoints and their buffered paths. For derivatives of smooth coefficient copies, a fixed normalized elementary complex disc has physical radius O(g2), and (RC.8) has room for it. The full Q kernel, however, is not asserted holomorphic in raw W1. Its retained variations use the real symmetric-difference shells of QS, with the coefficient family continued on the same fixed outside/source polydisc at each real endpoint. ∎

This lemma supplies the actual rectangular domain, analytic continuation and component interface. An absolute energy-graded root estimate still has to be supplied for that same joint family; it is not inferred from admission. In particular, a source-only old marginal's rank loss must be paid per primitive constituent before its connected sum, as in the MS proof.

## 3. Regulator comparison for the three real copies

All real W_M,W0,W1 values used in (RC.7) lie on the same elementary path (RC.1). Thus, for every declared full carrier Y,

\[
 R_Y(W_M),\ R_Y(W_0),\ R_Y(W_1)
      \le \sup_{|u|\le1}R_Y(\tau_{d,u}W)
      \le \widehat R_Y(W).                       \tag{RC.9}
\]

The carrier must include the varied coordinate's full footprint when it actually occurs. This is exactly the shifted regulator convention; three independent new physical energy sums are not required for these endpoint rectangles.

A fixed complex disc for that one normalized link adds at most a constant to each affected plaquette energy majorant. Indeed the local expansion of the holomorphic Wilson polynomial at a compact link gives

\[
 \beta_2|\mathsf s(W_p(\zeta))|
    \le C_r[\beta_2\mathsf s(W_p(\theta))+1],
 \qquad |\zeta-\theta|\le r,                     \tag{RC.10}
\]

because beta2 times the squared physical step g2 squared is bounded. Only a fixed number of plaquettes meet the varied coordinate. The constant 1 is already part of R. This establishes the raw-copy regulator comparison needed by a coefficientwise force/energy proof.

It does not bound an arbitrary complexified reconstructed minimum by a real energy solely from pointwise analyticity. The force/prolongation coefficient estimate must retain its actual curvature leaves and full supports. Once that joint estimate is supplied, (RC.9)–(RC.10) combine the three copies without an additional cutoff-dependent energy factor.

## 4. Why the diagonal CA frame does not automatically give full QQ rectangles

In the full QQ version the exact off-diagonal source integrand includes

\[
 S_1(t;V_I)+H_1(t;V_I)-H_1(0;V_I)+H_1(0;V_K),
\]
\[
 V_I=\Psi_{W_I}(a),\qquad V_K=\Psi_{W_K}(a),     \tag{RC.11}
\]

with the denominator containing the same actual kernel-copy factor exp(H1(0;V_K)). The insertion and kernel old Q-domain data therefore cannot be identified off the diagonal. Even when the kernel is only the P analytic base, a nonanalytic insertion core requires the next kernel Q factors on its stencil to be kept whole during the old-core localization.

On a genuine independent starred bond, let V_I,s and V_K,s be the two next saddle backgrounds in an outside family. A common coordinate change produces free physical fields

\[
 I_s=e^{ig_1A_s(B)}V_{I,s},\qquad
 K_s=e^{ig_1A_s(B)}V_{K,s}.                       \tag{RC.12}
\]

Their relative field is invariant under every such common change:

\[
 I_s^{-1}K_s=V_{I,s}^{-1}V_{K,s}.                \tag{RC.13}
\]

### Lemma RC.3 — exact compatibility condition for simultaneous CA-type freezing

On a common starred slot, a shared free-coordinate change can make both physical copies independent of s only if V_I,s^{-1}V_K,s is independent of s. If this condition holds and the two desired fixed fields have that same ratio, the insertion-copy CA map also fixes the kernel copy on that slot. Thus this is the necessary and sufficient free-slot compatibility condition for that construction.

The proof is (RC.13) and direct substitution. Nonlinear exceptional solves cannot remove the condition, because the slot is genuinely independent. They still have to be included for the rest of the physical stencil.

For example, freezing the insertion field gives

\[
 e^{ig_1A_s(B)}=e^{ig_1B}V_{I,D}V_{I,s}^{-1}.
\]

The whole kernel Q test on that slot becomes

\[
 \left\|e^{ig_1B}V_{I,D}V_{I,s}^{-1}
             V_{K,s}V_{K,\square}^{-1}-I\right\|
       <2\delta_1.                              \tag{RC.14}
\]

Although its literal local kernel reference V_K,square is fixed by its raw kernel box, the relative saddle factor generally remains in (RC.14). Freezing the kernel field by a second common change reintroduces the same factor, inversely, in the insertion field. The net change still satisfies (RC.13).

At the diagonal the ratio is identity, which is why CA.13–14 works. The existing off-diagonal coefficient estimates bound the variation of this ratio but do not state an exact constant-ratio identity. Smallness is not the equality needed to fix real intersection domains under complex outside parameters.

This lemma does not exclude a different domain-preserving construction, a proved additional gauge identity, an enlarged exact physical fiber, or a new real localization method. In particular it does not prove that an actual canonical QQ current norm is infinite. It isolates the missing identity in the attempted direct extension of CA.

## 5. What real shell control supplies, and its remaining limitation

For real parameters, a change of the center matrices in (RC.14) is controlled by QS's finite symmetric-difference shell estimate. The old real admission proved in Section 1 remains available. These facts permit real finite-difference estimates of the mixed integral with all determinant, inverse, reconstruction and normalizer terms retained.

They do not alone produce the holomorphic outside family used for full physical carrier localization. After insertion freezing, a complex change of the relative factor in (RC.14) moves a hard kernel domain through an old nonanalytic insertion payload. Applying Stokes in that same B coordinate would require analyticity of the payload there; it has not been supplied. Conversely, choosing the kernel frame leaves the old insertion domain moving. A small real shell bound cannot be silently promoted to a holomorphic continuation of an intersection indicator.

There is a useful actual real estimate before this carrier issue. Let H1(0;V) be the first unmarked Q/P logarithmic correction. Its first native current bound and the summable path estimate (RC.5) give

\[
 |H_1(0;\Psi_{W_I}(a))-H_1(0;\Psi_{W_K}(a))|
     \le C_L e^{-cP_0^2}|\theta_I-\theta_K|.       \tag{RC.15}
\]

To justify the path integration, use the strict old margin from Lemma RC.1 and approximate the path by elementary old-coordinate changes. Their normalized total length is bounded by (RC.5); the intermediate fields remain inside the same buffered chart. The first supported current series is absolutely summable, so this approximation has a uniform limit. The analogous first source-defect difference carries its total fixed-polydisc source budget as well.

Thus off-diagonal old mass mismatches are small in an actual real sense, without dividing by a rare mass. Equation (RC.15) is not a supported expansion of the entire rectangular function in the final raw variables. A further joint localization theorem is required to convert these mixed-domain real bounds into the canonical full-carrier B/J estimate.

## 6. Established interface and next precise gate

The real rectangular admission and the three-copy fixed-inner-domain family are established here. They support the first-P/second-P_aux baseline and its extension to first-P/second-Q with only the outer moving domain, provided the joint microscopic energy/root estimate is proved in that family. The old direct, old kernel, and new kernel subrecords remain explicit.

For full QQ, the diagonal composite-current theorem MS remains valid. Its proof does not supply the extra off-diagonal domain identity. The next specific task is a joint real-domain localization or an exact additional frame/fiber construction handling the relative factor in (RC.14), with the original common denominator and full carriers. No conclusion about full Yang--Mills existence or canonical M04 closure follows merely from the real admission or small mismatch estimate.

Primary/companion checks: CMP119 (3.7)–(3.9), (3.15), (3.17)–(3.19); BA Sections 4–6; CA.2–CA.6, CA.11–CA.15 and CA.25; MQ/QS exact real-domain and shell constructions; MS.23a–MS.24; Annex Y M.1–M.5 and the canonical endpoint identity.
