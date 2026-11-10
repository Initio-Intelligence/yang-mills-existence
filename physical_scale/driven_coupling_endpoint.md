# The driven homogeneous coupling endpoint

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

**Gaussian calibration hypothesis (GC).** For the signed Gaussian increments of the actual stationary source section in its thermodynamic normalization, assume $\sum_{k<n}d_k^G=d_Bn+\vartheta_n$ with $d_B>0$ and $\sup_n|\vartheta_n|\le B_G$. The coupling and stopping conclusions use this calibration and the specified source readout and replay. A physical continuum limit also requires the stated uniform normalization and full-law hierarchy estimates.

## Assumptions and conclusions

This note supplies the E-only endpoint estimate required after (7) of the B03 reset-remainder reduction. It concerns the canonical homogeneous raw E recursion with **prescribed admitted numerical couplings**. It is not an alternative physical Wilson trajectory.

Let \(Y_j=g_j^{-2}\) be a finite weak prefix satisfying the numerical comparison and compatible-geometry hypotheses used by the source homogeneous construction. Keep its actual ordinary cutoff, all block and gauge choices, and all maps fixed. In the driven recursion of the reset-remainder reduction ([reset remainders](../coupling/reset_remainders.md), §4) set the mature reset multiplier to zero at every step. Write \(H_{j+1}^{0}\) for the resulting raw E birth. Each earlier \(H_i^{0}\) enters with its own vacuum subtraction and its own Wilson projection \(\beta_i^0=P_iH_i^0\). At an outgoing step the compensation needed to retain prescribed \(Y_{j+1}\) is outside the raw birth integral.

For one common sufficiently weak ceiling, the canonical functions \(H_j^0\) have fixed absolute physical/native charts, uniformly in the prefix length, and
\[
 \left|P_{n+1}H_{n+1}^{0}-d_n^G\right|
 \le Cg_n^2=\frac C{Y_n}.
 \tag{DE1}
\]
The Gaussian decrement \(d_n^G\), its units, stationary-section convention and finite-volume limit are the retained Gaussian calibration of the coupling calculation.

The conclusion supplies the second gate in the complex-marker reduction. The first gate is proved in [Homogeneous feedback and the causal Wilson recursion](causal_coupling_recursion.md), and both gates and the actual causal replay are verified in the causal-source compatibility conditions. Combining them gives the all-depth weak trajectory stated there. This endpoint theorem alone does not prove B05 physical normalization or change the source Wilson subtraction.

## 1. Why the pure E recursion has a fixed chart at prescribed couplings

### 1.1 The raw integral and the outgoing compensation have different roles

At step \(j\), the homogeneous fluctuation exponent has the prescribed leading Wilson coefficient \(Y_j\), the actual current ordinary cutoff, and the inherited sum
\[
 \sum_{i\le j}\left[
 H_i^0(U)-H_i^0(1)-\beta_i^0 A_i(U)
 \right].
 \tag{DE2}
\]
The \(A_i\) are the source Wilson terms in their own units and localization convention. In particular \(\beta_i^0\) is the projection of the same \(H_i^0\), not the actual physical coefficient from a different bank.

The raw output is constructed before its new vacuum and Wilson terms are installed. This is the order on CMP119 pp.278–279: first the localized E-producing logarithm, then the new projected scalar, then the change of the Wilson coefficient. In the artificial recursion the latter bookkeeping is supplemented by
\[
 [\,Y_j-Y_{j+1}-P_{j+1}H_{j+1}^0\,]\,
 A_{j+1}(U).
 \tag{DE3}
\]
This is an explicit output factor. It is not included in the fluctuation logarithm defining \(H_{j+1}^0\). Consequently it does not enter the normalized reference measure or its score estimates at this step.

At the following step the leading coefficient is the stipulated \(Y_{j+1}\), by the definition of the driven recursion. Its canonical gauge/constraint construction uses that same stipulated coefficient. There is no separately carried gauge mismatch \(t_jG\) in this definition. Such a mismatch belongs to the shifted self-consistent comparator of [The Wilson trajectory on intervals admitting mature resets](../coupling/finite_window.md) (§§1–2) and is unnecessary here.

The input estimates before outgoing installation use the following facts: the numerical comparison of the prescribed couplings and cutoff radii, the fixed geometric/minimizing-map construction, the bounds on the inherited coefficients, and the identity \(\beta_i^0=P_iH_i^0\) in the Ward cancellation. They do not use \(Y_{i-1}-Y_i=\beta_i^0\). CMP109's finite Taylor/Ward calculation and CMP119 (3.49)–(3.67) make this distinction explicit: their marginal cancellation pairs an activity with its own projected Wilson tensor. The leading quadratic minimizing problem and its covariance are determined by the prescribed Wilson/gauge data, independently of the E coefficients.

Thus the single-step pure E estimates can be replayed on (DE2), with (DE3) kept outside. This is a statement about those explicit formulas. It does not invoke the physical density induction at inconsistent synthetic couplings.

### 1.2 One fixed physical chart regenerates

Choose fixed positive \(\alpha_{\rm phys,0},\alpha_{\rm phys,1}\) and the associated strict smaller input margins as in CMP109 and CMP116. Use the same finite set of scheme constants as the driven recursion; choose them to satisfy both the fixed-chart pure E and the later native estimates. The real cutoff is eventually well inside this chart because
\[
 g_jP_j\le Cg_j(\log g_j^{-2})^{p_0}\longrightarrow0.
 \tag{DE4}
\]

Suppose the old pure E births have the fixed-chart bound \(E_0e^{-\kappa d_i(X)}\) and the source gauge/Euclidean covariance. Their own projected coefficients are bounded by a fixed constant \(CE_0\alpha_{\rm phys}^{-2}\). CMP116 Lemma 1, (1.33)–(1.36), bounds their **complete renormalized fluctuation difference** on a fixed physical displacement ball. Its proof (1.24)–(1.32) sums all old carriers and grades before the current integration, retaining the own Wilson cancellation. The resulting norm is
\[
 \|\mathcal V_j^{E,0}\|_{\rm root}
 \le C_{\rm phys}E_0\,\epsilon_1 ,
 \qquad |b|<\epsilon_1\le\epsilon_{\rm fix}.
 \tag{DE5}
\]
All constants in (DE5) are fixed physical-chart constants. The factor \(\epsilon_1\) can equally be replaced by the actual physical displacement where the source estimate permits it.

The Gaussian/coarea raw birth has a fixed coefficient bound \(B_G\), independent of the numerical coupling and the old E bank. The explicit Wilson remainder, Haar terms, and (DE5) are handled by the same local positive majorant and connected expansion in CMP116 §2. Its output estimate (2.41), with the source rate reserve, has the form
\[
 \|H_{j+1}^0\|_{\rm source}
 \le B_G+\Theta_j,\qquad
 \Theta_j\le C_{\rm phys}
 \left[(1+E_0)g_j(1+P_j)+g_j(1+P_j)^3\right].
 \tag{DE6}
\]
The cubic term is the literal \(g_j^{-2}O((g_jP_j)^3)\) estimate in CMP116 (1.38)–(1.39); higher Wilson degrees are absorbed in it on \(g_jP_j<\epsilon_{\rm fix}\). The inherited difference and local measure/coarea corrections have the other displayed size. Increasing the fixed polynomial power for any equivalent source convention would not affect this induction. Choose \(E_0>2B_G\), then the common ceiling so \(\Theta_j\le E_0/2\). The published output-to-input analytic and decay margins regenerate this same fixed chart and source norm. This is an induction on individual raw births with their already resummed inherited fluctuation family, not an extensive sum of all old norms.

The formulas defining \(H_{j+1}^0\) do not depend on the auxiliary chart radius used to prove (DE6). Hence the fixed-chart family constructed here is the same canonical zero-marker family as in the narrow native construction on their common domain. This is equality of formulas/analytic germs, not an arbitrary continuation from \(J=J(U)\).

Gauge covariance, outgoing Euclidean covariance and reality are preserved by the source formulas at every step. The argument introduces no arbitrary complex marker into this fixed-chart induction. That harder question belongs to target (6).

## 2. Freeze one actual integral before changing its physical amplitude

Fix the incoming pure E family, the prescribed current \(g=g_n\), and the actual product support
\[
 D_n=\{\,a:\ |a_b|<P_n
          \text{ on the independent canonical bonds}\,\}.
 \tag{DE7}
\]
Fixed finite normalization changes of the bond radii are harmless. Its symmetry \(a\mapsto-a\) is essential. Every cutoff remains fixed during the interpolation.

Let \(u\) be the external physical minimizing-section coordinate in a fixed neighborhood of flat. Retain its complete constrained chart, covariance and coarea factors. Denote the normalized physical fluctuation map by \(q_u(b)\), with \(q_u(0)=0\); its linear part and nonlinear constraint correction are both included.

After extracting the zero-fluctuation input and the background Wilson value in the literal source fashion, write the complete fluctuation integral as
\[
 Z_n(\tau,u)=\int_{D_n}e^{-\mathcal H_{\tau,u}(a)}\,da,
 \qquad -g\le\tau\le g .
 \tag{DE8}
\]
The physical displacement in every inherited function, Haar factor and nonlinear constraint is \(b=\tau a\). The stationary Wilson contribution is
\[
 \tau^{-2}\left[
 A(U_u(q_u(\tau a)))-A(U_u)
 \right],
 \tag{DE9}
\]
with its actual stationary gauge normalization and any source-explicit factors retained. Equation (DE9) is interpreted by its removable value at \(\tau=0\).

The first variation vanishes on the solved constraint tangent at **every** admitted physical output \(u\). Therefore its Taylor expansion begins at order two, and the removable continuation persists after the finitely many \(u\) derivatives used by the curvature projection. At \(\tau=g\), (DE8) is the actual pure E-only integral at this step. At \(\tau=0\) it is the constrained Gaussian/coarea integral with the same fixed cutoff.

This is a real amplitude interpolation of one fixed-support integral. It is not a derivative of the bare-axis trajectory and does not postulate a complex \(g\)-disk of fixed radius on a support growing as \(P_n\).

## 3. Uniform score and connected bounds on this interpolation

### 3.1 Polynomial amplitude derivatives

Use (DE5) first with one fixed trial physical radius \(\epsilon_{\rm fix}\), before restricting to \(b=\tau a\). This bounds the full old-age sum on that displacement ball. Fixed-order physical Cauchy derivatives are therefore uniform on the half ball. Counting derivative endpoints costs a fixed carrier polynomial, paid by the source spatial exponential.

For the Wilson term, expanding the numerator of (DE9) to second order and differentiating the integral remainder shows that up to two \(\tau\) derivatives are bounded by fixed-degree polynomials in the canonical \(a\)'s, with smooth bounded local coefficients. The same is true after up to two physical retained-field derivatives, including derivatives of the minimizing map, the constrained precision, the nonlinear chart, and the Haar/coarea factors. The relevant map rows are the fixed-chart CMP102/CMP116 rows. No negative power of \(\tau\) remains.

Thus every score required for
\[
 \partial_\tau^2D_{u_x}D_{u_y}\log Z_n(\tau,0)
 \tag{DE10}
\]
is a sum of fixed-degree canonical polynomials with exponentially summable carrier kernels. A derivative in \(u_x\) has its actual root at \(x\); a derivative in \(u_y\) has its root at \(y\). A \(\tau\) derivative may be rootless and is summed only after connectedness has linked it to one of these roots. The maximum polynomial degree and derivative order are fixed.

### 3.2 The actual interacting reference remains uniformly controlled

At flat \(u=0\), the prescribed quadratic precision has the retained fixed gap and exponential row bound. The Wilson nonlinear canonical Hessian is \(O(gP_n)\); the fixed-chart inherited E and measure terms have canonical Hessian \(O(g^2)\), with harmless fixed cutoff-polynomial refinements still tending to zero. The same bounds hold for every \(|\tau|\le g\). Consequently the full real Hessian and its exponential conjugations retain a uniform positive gap.

This conclusion can be proved by the same product-support Neumann form used in C08: smooth the convex indicator factorwise, retain the nonnegative face term, and pass the scalar covariance inequality to the literal product balls. It gives the exponentially weighted covariance inequality without identifying the covariance with the inverse pointwise Hessian.

At flat, global compact adjoint invariance implies \(\mathbb E_\tau a_b=0\) for the semisimple Lie-algebra coordinates used here. The canonical cutoff and fixed gauge convention preserve that invariance. The gap then gives uniform local canonical moments
\[
 \|a_b\|_{L^p(\nu_\tau)}\le C\sqrt p,
 \tag{DE11}
\]
independently of the cutoff radius and prefix length. The cutoff radius still tends to infinity; no inverse global acceptance probability is used.

Here is the connected-factorization step needed for at most four insertions. First expand each score in its localized polynomial carriers and sum the carrier tails with a fixed reserve. For \(m\le4\) selected carriers, take a minimal tree on their roots and cut its longest edge. It partitions the roots into two nonempty groups at distance at least that edge length; the length is at least the tree length divided by \(m-1\). In the moment-cumulant formula, replace each mixed moment by the product of its two group moments. The completely factorized cumulant vanishes. Telescoping the replacements expresses the original cumulant as a finite sum of crossing covariances of product observables, multiplied by other moments.

Apply the scalar exponentially weighted covariance inequality to each crossing covariance. Hölder's inequality and (DE11) bound the gradients of the products and all remaining moments: their polynomial degrees and \(m\) are fixed. Large carrier diameters are paid by the reserved carrier tails before this root calculation. This proves
\[
 |\kappa_m(X_1,\ldots,X_m)|
 \le C_m\exp[-c\,\mathcal T(x_1,\ldots,x_m)/(m-1)],
 \qquad 2\le m\le4 ,
 \tag{DE11a}
\]
with the same conclusion for the anchored score kernels. The case \(m=1\) is its local moment bound. Finally sum each unanchored root along a tree. Since \(m\le4\), the rate division is a fixed loss and all lattice convolutions are finite. Reserve a further fixed part of the decay for the two external roots. No bound in this step replaces a canonical moment by the cutoff supremum \(P_n\).

### 3.3 The mixed derivative of the logarithm

Differentiate the normalized real expectation successively. The exact formula for (DE10) is the sum over partitions of its four labeled differentiations. A partition block \(I\) inserts \(-\partial_I\mathcal H_{\tau,0}\), and the partition contributes the joint cumulant of its blocks. Single-block terms are ordinary localized expectations. Coincident derivatives and all lower jets occur in this formula.

Using §3.2 on each partition and summing its internal roots gives
\[
 \left\|
 \partial_\tau^2D_{u_x}D_{u_y}\log Z_n(\tau,0)
 \right\|
 \le C e^{-c\,{\rm dist}(x,y)}.
 \tag{DE12}
\]
The constants depend on the fixed source scheme but not on \(n\), \(Y_n\), the volume, or \(P_n\). Purely external explicit factors are retained: those independent of \(\tau\) cancel in the difference from zero, and those depending on \(\tau\) obey their same fixed local derivative bound.

Equation (DE12) implies the uniform spatial second-moment bound needed by the curvature projector. This is the substantive step that removes a logarithmic cutoff factor; a supremum estimate on all \(a\in D_n\) would not do so.

## 4. Evenness and the projected \(O(g^2)\) error

Every nonconstant physical argument in (DE8) is \(\tau a\). The removable Wilson normalization \(\tau^{-2}\) is even. The support and reference free measure are invariant under \(a\mapsto-a\). Consequently
\[
 Z_n(-\tau,u)=Z_n(\tau,u)
 \tag{DE13}
\]
for all admitted real \(u\). The same equality holds after the retained-field derivatives. In particular the first amplitude derivative at zero vanishes.

Apply integral Taylor remainder at \(\tau=0\), then the spatial second-moment estimate (DE12):
\[
 \left|
 P_{n+1}\bigl[\log Z_n(g,\cdot)
                 -\log Z_n(0,\cdot)\bigr]
 \right|
 \le Cg^2 .
 \tag{DE14}
\]
The zero-fluctuation inherited action is not a new raw birth and was extracted in defining (DE8). The outgoing compensation (DE3) is likewise outside that birth. Thus (DE14) compares exactly the pure E-only new raw scalar with its cutoff Gaussian scalar.

At \(\tau=0\), the projected Gaussian includes the actual differentiated constrained covariance and coarea. The local cutoff-to-uncut Gaussian error for these finitely many rooted scores is bounded by a fixed polynomial in \(P_n\) times \(e^{-cP_n^2}\). It follows either from the Gaussian cutoff estimate or from the same positive gap and local Gaussian score expansion. This is a local normalized comparison, not division by the probability that every bond in an arbitrarily large volume lies in the cutoff.

With the stipulated large fixed cutoff exponent, that error is \(o(g^2)\). Take the compatible thermodynamic limit at fixed \(n\), using the uniform rooted decay and then the stationary Gaussian calibration. The result is (DE1).

## 5. Relation to the remaining B03 work

This theorem concerns the zero-marker **driven** family, not the old shifted comparator. Its fixed charts are regenerated directly from the pure E source formulas because each incoming coefficient is paired with its own projection and the prescribed outgoing coefficient is installed outside the raw integral.

If the separate mixed synthetic theorem (6) is established on its required invariant full native domain and amplified disk, the original amplification argument gives
\[
 |P H_{n+1}(1)-P H_{n+1}(0)|
 \le C r_n^{-2}/(A_n-1).
 \tag{DE15}
\]
Choose its fixed amplification power \(D>4\), including the stated readout logarithms. Combining (DE15) with (DE1) then supplies the local decrement estimate against \(d_n^G\) on the admitted prefix. The numerical signed-prefix continuation, actual source replay, normalization and endpoint matching still have their stated separate roles. This note does not replace any of them by an E-only assertion.

### Sources

- The B03 reset-remainder reduction, definition of the driven recursion and targets (6)–(7).
- CMP109, the fixed-chart effective action, finite Taylor/Ward decomposition and its own Wilson subtraction.
- CMP116 (1.24)–(1.36), the complete preintegration inherited E fluctuation family; §2 and (2.41), the same-chart localized raw output estimate.
- CMP119 (2.25), (3.28), (3.37)–(3.47), and pp.278–279, the canonical raw homogeneous birth and the subsequent Wilson installation.
- CMP119 (3.49)–(3.67), own-coefficient Ward cancellation.
- The signed Gaussian calculation, §2 and its cited N7.40–N7.43: the fixed-support even real-amplitude score argument, applied to the driven fixed-chart family verified above.
- The C08 application after C06, §§2–4: the product-support scalar covariance, finite connected estimates and physical-map endpoint method, used here only after verifying the pure E interpolation's own uniform Hessian and score hypotheses.

\newpage
