# Physical matching at cofinal cutoffs

The identification of the cumulative Gaussian marginal with a linear drift up to a uniformly bounded remainder is a separate hypothesis (GC). An arithmetic consequence of that drift does not prove GC or match a prescribed physical endpoint.

**B-05 remains open.** The normalized F-01 measurements leave a bare-coupling degree of freedom even at a finite cutoff. An independently normalized Wilson observable can be used for a continuous scalar shot if its level set is calibrated to the native marginal projection. The finite-volume Wilson integral gives the requisite continuity for that different observable. A last-step gap example below rules out recovering this calibration or the prescribed native endpoint from the B-03 drift estimate and cofinal selection alone.

## Which physical condition is fixed?

the stated criterion asks for one compatible family inside the source ceilings satisfying the chosen finite physical normalization at the common scale \(\ell_0\). The source-free normalization N2-F fixes the numerical endpoint before the construction. With the corrected dictionary, if the program target is \(g_* \), then
\[
  Y_K=Y_*:=2N^2g_*^{-2},\qquad
  \beta_{W,K}=Y_{0,K}/N,\qquad a_K=L^{-K}\ell_0.
\]
Here \(\beta_{W,K}\) is the bare coefficient of \(S=\sum_p(N-\Re\operatorname{Tr}U_p)\). If the target is already in native units, it is simply \(Y_*=(g^B_*)^{-2}\). At positive depth the prescription is the homogeneous polarization in the chosen decomposition. Its definition does not say it equals the Hessian of an arbitrary normalized finite-torus marginal. B-05's stated criterion does not require all of the stronger differentiability assertions of N2-F.  · N2 §§2–3, ICR-N2-1 · Actual projection and replay

At fixed admissible torus and mesh let \(b=Y_0/N\), and write \(n_h(b)\) for the seven unrenormalized F-01 measurements. All are real analytic in real positive \(b\). Indeed \(S\) and the finitely many group stencils are bounded at fixed mesh. The numerator integrals for ordinary moments are entire in \(b\), by the compact Haar integral with weight \(e^{-bS}\); fixed polynomial bare factors, when present, preserve analyticity. The strictly positive partition function is locally nonzero in a complex neighborhood of every real \(b\). Finite products and differences give the centered integrals. Wherever all \(n_h>0\), the seven positive roots and the identity coefficient depend real analytically on \(b\):
\[
 z_h(b)=\sqrt{\lambda_h/n_h(b)},\qquad c(b)=z_S(b)m(b).
\]
Therefore every \(b\) in an open interval around any nonsingular point solves all eight equations after fitting the eight coefficients. The derivative of every resulting normalization residual along that interval is zero. If there is a nonsingular witness for one fixed geometry, the nonnegative analytic functions also give nonsingularity there except at a locally finite set of positive bare values (finite union of isolated zero sets). Neither the exception set nor a lower bound is uniform in the changing lattice. F-01(F.34) is precisely the Jacobian in the eight field coefficients with \(b\) fixed. It cannot be inverted to fix the ninth unknown \(b\). The positive comparison on larger ultracold cubes is a witness on those geometries, with a different endpoint. Annex X, F.22–34 · Actual weak-family reflected measurements

## A continuous Wilson measurement and the missing equality

For an independently specified bounded physical stencil or bounded multiscale test \(A_K\) with a fixed, bare-independent sampling rule, the literal finite Wilson response \(M_K(b)=\mathbb E_b A_K\) is real analytic, with \(M_K'(b)=-\operatorname{Cov}_b(A_K,S)\). The same conclusion holds for ratios with a nonzero denominator on the shooting interval. A fixed random readout conditional on the microscopic links is covered by taking its conditional expectation first. For a bare-dependent history kernel, this proof requires either retaining its derivative/continuity or identifying its expectation with the fixed microscopic test.

Specifically, suppose at cofinal depths there are *admitted* bare intervals on which the native trajectories satisfy the terminal and intermediate geometry tests, and the continuous \(M_K\) brackets a predetermined \(m_*\). It suffices to prove, on the same intervals, the scalar implication
\[
 M_K(b)=m_* \quad\Longrightarrow\quad Y_K(Nb)=Y_* .
\]
Here \(Y_K(y)\) denotes the actual endpoint starting at native inverse coupling \(y\). An intermediate value gives an exact shot even when \(Y_K\) has jumps elsewhere. One sufficient comparison near that level is \(|Y_K(Nb)-Y_*|\le C_K|M_K(b)-m_*|\); no uniformity of \(C_K\) is required for this finite implication. An additive error tending to zero yields only asymptotic matching. The compact Wilson integral supplies neither sign brackets for a prescribed physical observable nor the implication. The uniform signed prefix controls the principal slope in scale, while the needed equality links two different readouts at a fixed scale. Equality of partition functions or a vacuum subtraction alone cannot fix the split into \(YA+E\), since the replacements \(Y\mapsto Y+c,\ E\mapsto E-cA\) leave this sum identical. This algebraic observation concerns what follows from equality of densities alone. The source fixes its own split by an additional projection. Native projection, HS.24–27

**A last-step gap persists for every cutoff depth.** As a test of the numerical implication, take \(d>0,\ c>0,\ M\) with \(c/M<d/2,\ c/M^2<1\), and \(t>M+2d\). For admitted \(y\ge M\), set
\[
 F(y)=y-d+\frac c y
 \begin{cases}-1,&y<t, \\+1,&y\ge t.\end{cases}
\]
Each branch is strictly increasing. Its decrement is in \([d/2,3d/2]\) and has remainder bounded by \(c/y\), with zero Gaussian transient. Thus all raw suffix slopes hold, even at one step. Yet the range of *each final step* misses \((t-d-c/t,t-d+c/t)\), so \(Y_*=t-d\) cannot even be approached by changing depths, initial values or subsequences. For example, backward iteration on the upper branch from any \(y>t\) produces positive endpoints on coherent arbitrarily long admitted trajectories, with a stabilized label and exact compatible scalar recurrence. The example concerns an inference from B-03 and compactness. It gives no evidence that the Wilson projector itself jumps. Appendix H's interval and Appendix I's one-sided label keep precisely the information to which the example applies. PE.13, PE.25–26 and §8 · HS.23–28

## A scalar test for compatibility of conditional physical readouts

There is a weaker alternative to total-variation convergence for passing bounded retained probes. On a fixed retained finite geometry, let \(X_n\) be the outer raw state in common Polish coordinates, \(U_n\) a retained inner output, and \(Q_n(X_n,dU)\) its genuine conditional law. Assume the actual joint laws converge weakly to \(\mu(dx)Q(x,du)\) on these coordinates. This premise can be obtained on a tight subsequence for ordinary finite-dimensional raw variables. For each real bounded continuous inner probe \(f\), draw two conditionally independent inner continuations from that *same* kernel at the same exterior. Write
\[
 D_n(f)=\mathbb E[f(U_n^{(1)})f(U_n^{(2)})]
       =\mathbb E[(Q_nf)(X_n)^2].
\]
A necessary and sufficient condition for approximation of the conditional response by common continuous exterior probes is
\[
 \lim_n D_n(f)=\int |Qf|^2\,d\mu
 \quad\Longleftrightarrow\quad
 \inf_{\phi\in C_b}\limsup_n
 \mathbb E|(Q_nf)(X_n)-\phi(X_n)|^2=0.
\]
Indeed for fixed real \(\phi\) the cross moment is \(\mathbb E[\phi(X_n)f(U_n)]\), which converges by joint weak convergence. Expanding the square gives the limsup defect \(\limsup D_n(f)-\|Qf\|_{L^2(\mu)}^2+\|Qf-\phi\|_{L^2(\mu)}^2\). Density of bounded continuous functions gives the equivalence, using the same expansion with liminf and nonnegativity for the universal lower bound. Bounded products of finitely many such responses can then pass by telescoping and Cauchy–Schwarz, clipping each approximating continuous probe to the corresponding fixed sup norm. Countably many fixed probes admit a common diagonal sequence. This tests the response to the chosen probes only. Identifying \(Q\) with the specific source kernel still requires its defining conditional identities at the limiting state.

The right side can be tested against actual native integral approximants, without lower bounds on rare component masses if the joint laws keep the selected outer branch mass. A branch of positive but small mass is weighted by that mass once for both continuations. The oscillating example FK.17–18 gives a strictly positive mean-square defect for its raw mass function. A similar defect for bounded conditional means arises by taking Bernoulli continuations whose conditional success parameter equals that mass function. Thus a one-copy weak-law theorem cannot establish this compatibility by itself. Appendix P identifies archive-dependent raw multipliers, the constrained finite-dimensional coordinates, and hard-selector interfaces that still need estimates for the actual model. This criterion gives an observable-specific test for those cases in which nonlinear products of conditional probes are required. It does not retroactively impose whole-kernel convergence as a necessary clause of the source-free B-05 statement. Appendix P, FK.12–20 · Actual scope of positive-history extraction

The remaining source-free test is either a genuine native shot with compatible actual cutoff data, or an exact calibration and admitted bracket for a prespecified physical observable. A single common subsequence can preserve the HS homogeneous identities once exact shots exist and its uniform extraction hypotheses hold. Where canonical mixed-history operations are asserted, their separate limiting identification still has to be made. Neither selection of the terminal band nor refitting the seven field coefficients resolves the finite physical shot.
