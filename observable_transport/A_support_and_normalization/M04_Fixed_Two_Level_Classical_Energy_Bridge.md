# A finite-two-level classical energy bridge and the remaining marked inputs

This note records a classical consequence of the existing BR construction; it is not the full stochastic marked estimate MS.25.

## 1. Normalization and statement

Use the homogeneous two-level native geometry of CA. Let h2 = L^2 h0 and let U2(W) be its actual microscopic constrained minimum on the admitted orbit, with W the final coarse field. Write

\[
\beta_i=\frac1{N g_i^2},\qquad
E_X^{(2)}(W)=\sum_{p\subset X}\beta_2 s(W_p),\qquad
\frac{\beta_0}{\beta_2}=\left(\frac{g_2}{g_0}\right)^2.
\tag{CB.1}
\]

The source adjacent-coupling inequalities bound this ratio at the two fixed levels. Its value is not set to one. All coefficient constants below may depend on L, the two levels and fixed source localization conventions. No depth-uniform claim is made.

For a fixed microscopic plaquette p, the native BR variational family gives a connected raw-W carrier expansion of its classical Wilson readout,

\[
\beta_0\mathsf s(U_{2,p}(W))=\sum_{Y\ni p^{(2)}}v_{p,Y}(W_Y),
\tag{CB.2}
\]

with nonnegative deterministic envelopes a_Y such that

\[
|v_{p,Y}(W_Y)|
 \le a_Y\frac{\beta_0}{\beta_2} E_Y^{(2)}(W),
\qquad
\sum_{Y\ni p^{(2)}}e^{\nu n(Y)}a_Y\le C_L.
\tag{CB.3}
\]

All gauge, averaging, reference and fixed incidence footprints are included in Y. The holomorphic Wilson polynomial is used on the component outside-parameter discs, with its modulus bounded by the same real-center energy majorant. The carrier rate is fixed after the fixed source geometric parameters. A fixed finite scalar stencil changes only its initial footprint and C_L.

This estimate controls the classical minimum, before any Gaussian integration. In microscopic scalar units it says, explicitly,

\[
h_2^4\,|\alpha\beta_0\sigma_{h_0,Y}(U_2)|
\le C_L L^8 |\alpha|\left(\frac{g_2}{g_0}\right)^2
                         a_Y E_Y^{(2)}(W).
\tag{CB.4}
\]

Here the fixed stencil convention is absorbed in C_L; h2^4/h0^4 = L^8 is displayed. The identity part of a scalar is still h2^4 c. Neither this identity term nor any fluctuation trace is absorbed into E^(2). The regular reference has the stronger source spacing estimate BR.23, but no additional depth-uniform scale gain for the entire nonlinear correction is used in (CB.3)–(CB.4).

## 2. Both variational inputs have actual raw-energy bounds

The BR reference Uref(W) has local raw dependence and is regular on the microscopic lattice. At fixed depth two, BR.21–23 give, on a fixed enlargement X of a current patch,

\[
\beta_0\sum_{p\ {
m read\ in}\ X}s(U_{{ref},p})
 +\beta_0\sum_{f\ {
m read\ in}\ X}|J_f(Uref)|^2
\le C_L\frac{\beta_0}{\beta_2}E_{X^{+c}}^{(2)}(W).
\tag{CB.5}
\]

J is the actual source-normalized force appearing in BR.29. Conversion between its fine-grid normalization and an unweighted fixed-depth coordinate sum is part of the fixed C_L. The number of fine coordinates over one current block is fixed at these two levels. No fine-rank factor depending on a varying number of RG steps is suppressed.

The second input is the actual prescribed-average mismatch

\[
B_c=\log\{W_c[\mathcal M^2Uref]_c^{-1}\}.
\tag{CB.6}
\]

It cannot be omitted merely because Uref is regular. BR.22 makes its straight subdivided edge transport exactly W. In the literal nonlinear average, each averaging contour differs from that straight transport by holonomies of a fixed set of intervening fine plaquettes. The fixed-depth path comparison of BR.25–26 therefore bounds B_c by a fixed multiple of the local curvature defect delta_X from BR.21. This is the actual local defect, not only the chosen geometric ceiling: both the fine curvature and the mismatch vanish on flat local data. The small matrix logarithm is Lipschitz in this comparison domain.

The source fundamental trace gives delta_X squared bounded by a fixed finite sum of s(W_p) on that enlarged patch. Squaring the preceding path bound and summing the finitely many current incidences yields

\[
\beta_0\sum_{c\ {
m read\ in}\ X}|B_c|^2
\le C_L\frac{\beta_0}{\beta_2}E_{X^{+c}}^{(2)}(W).
\tag{CB.7}
\]

Every averaging contour and its fixed gauge footprint is retained in X+c. Flat nontrivial holonomy is allowed: the argument compares local closed contours, not absolute connection potentials in a global weak-link gauge.

Equations (CB.5) and (CB.7) are the two required input bounds. A force-only argument would not cover the actual approximate BR reference.

## 3. Distinguished force-or-mismatch leaf

Use the actual fixed point BR.29, schematically

\[
A_1=-\mathcal GJ-\mathcal G\mathcal N(A_1+H_1B),\qquad
A=A_1+H_1B-HD(A_1+H_1B).
\tag{CB.8}
\]

The complete decoupled operator and nonlinear bounds are those already used in BR. The nonlinear derivative is a strict contraction on the declared fixed small geometric ball. At J = B = 0 the relative correction is zero, even though the propagators may retain the flat background transports.

Every Picard tree therefore has a J or B leaf. Distinguish one, bound all other small input leaves by the geometric ceiling, and sum the differentiated scalar contraction majorant. Its inverse factor is bounded by the contraction reserve. This is the same distinguished-leaf argument as MQ.35, now for the pair (J,B). It gives a local supported coefficient majorant

\[
|A_{e,X}|\le c_{e,X}
 \left(\sum_{f\in\operatorname{foot}X}|J_f|^2
              +\sum_{c\in\operatorname{foot}X}|B_c|^2\right)^{1/2},
\qquad
\sup_e\sum_X e^{\nu_0n(X)}c_{e,X}\le C_L.
\tag{CB.9}
\]

Local gauge-invariant reconstruction maps preserve this bound. An arbitrary absolute gauge potential is not substituted for A. The complex continuation is that of the actual variational equations and their common coefficients; only the physical endpoint is asserted to be the minimum. Component Cauchy extraction retains each distinguished leaf's complete raw footprint, and no internal walk tag is exposed as a physical carrier.

Taylor expansion of the holomorphic plaquette trace about the real compact reference gives the component estimate

\[
\beta_0|\mathsf s(U_{2,p})|
\le C_L\beta_0\left[s(U_{{ref},p})
                      +\sum_{e\in\partial p}|A_e|^2\right].
\tag{CB.10}
\]

For coefficient products, the two correction carriers meet the fixed plaquette stencil. Cauchy--Schwarz bounds the product of their two local square-root energy envelopes by the energy on their union. The weighted absolute convolution is finite after a fixed rate reduction. Cross terms with the reference plaquette use the same inequality. Combining (CB.5), (CB.7) and (CB.9) proves (CB.3), with every support retained. There is no inverse coupling factor beyond the explicit beta0/beta2 ratio.

At the physical endpoint, exact variational nesting identifies U1(M U2) with U2 on the admitted minimal orbit: any competitor with M U = M U2 is also a competitor with M^2 U = W. Uniqueness on the source orbit gives the identification. The averaged gauge terms choose representatives; the microscopic Wilson stencil is gauge invariant. Thus (CB.3) applies to the zero-innovation background of the nested microscopic reconstruction.

## 4. What is still required for the marked theorem

The classical estimate does not by itself prove MS.25 or the absolute second-step marked bound. The following are distinct additional checks.

1. **Common two-layer fluctuation leaves.** In the exact nested reconstruction, retain the source-independent factors g0 z0 and g1 z1, with the actual constrained coordinate maps and joint component identities. The desired positive majorant has the factors beta0 g0^2 = 1/N and beta0 g1^2 = (g1/g0)^2/N. It must hold in the same old/new coefficient family, not just for two separately reconstructed endpoint fields.
2. **Joint marked Gaussian/source reserve.** A local energy root must be inserted into the full two-layer normalized integral while preserving its old conditional Gaussian normalizer and new Gaussian reserve. The native P0^2 estimate used for the rare correction does not prove the adaptive energy-root bound for the nonrare smooth baseline. In particular one cannot multiply an uncontrolled next-quadratic tilt for every copied old marked payload.
3. **Canonical rectangular current family.** The separate insertion and kernel copies at the second step must preserve actual old and new moving domains and their common normalization. The diagonal core construction and the composite physical-pushforward current theorem do not prove that stronger family or the propagation of previously filed B/J records.

No depth recurrence, uniform-depth coupling estimate or complementary large-field argument follows from (CB.3). This note only narrows the fixed-two-level classical part of the next marked task using the existing raw reference, force and average-mismatch bounds.

Dependencies: BR.21–29 and its actual variational/component construction; MQ.35's distinguished-leaf majorant; CA's fixed-depth native chart and actual inherited saddle conventions; MS.25 for the larger marked target.
