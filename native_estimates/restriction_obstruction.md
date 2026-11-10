# Locality on nested domains and the literal two-layer condition

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 2. Theorem 4.1

### 2.1 The readings

**(G1) "maximal possible domains".** [R] (1.4), p.77 source: "\(\Omega_j=B^j(\Omega_j^{(j)})\), \(\Omega_j\) is a sum of cubes of a size \(M_1L^j\eta\), \((L^j\eta)^{-1}\mathrm{dist}(\Omega_j^c,\Omega_{j+1})>RM_1\)." Given \(\Omega_p\), the admissible big blocks for \(\Omega_{p+1}\) form a family closed under unions, and a larger \(\Omega_p\) admits more blocks. Hence the componentwise-largest sequence exists, and it is the only sequence that is maximal in any sense. deduction. (G1) is not a reading.

**(G2) finer data determine coarser constraints.** [A] (43), p.24 source: "\(\bar U^{k+1}_c=(\overline{\bar U^k})_c=\exp[\,i\sum_{x\in B(c_-)}L^{-d}\frac1i\log\bar U^k(\Gamma_{c,x})(\bar U^k(c))^{-1}]\bar U^k(c)\), \(c\subset\Omega^{(k+1)}\) … Let us notice that this definition is local in the sense that \(\bar U^k_c\), \(c\subset\Omega^{(k)}\), depends only on the bond variables \(U_b\) for \(b\subset B^k(c_-)\cup B^k(c_+)\)." So \(\bar U^q\) is the \((q-p)\)-fold average of \(\bar U^p\), it is a global operation, and it does not depend on the sequence. The constraints are "\(\bar U^j=V\) on \(\Lambda_j\)" with the bond convention "bonds with at least one end-point" ([V] p.277, [R] (1.13)).

*Claim deduction, given these two quotes.* Let \(\nu_Z\le\nu_{Z'}\). Every \(Z'\)-constraint \(\bar U^q(b)=V'(b)\) is a function of the \(Z\)-data and of the field off \(\Omega_1(Z)\).

*Proof.* Sub-claim, by induction on \(q\): if every point of the two end blocks \(B^q(b_\pm)\) of a level-\(q\) bond \(b\) has \(Z\)-level \(\le q\), then \(\bar U^q(b)\) is determined. A level-\(q\) block is either inside or outside \(\Omega_q(Z)\). If one end block is inside, \(b\) touches \(\Lambda_q(Z)\) and \(\bar U^q(b)\) is a \(Z\)-datum. Otherwise all points of both blocks have \(Z\)-level \(\le q-1\), and \(\bar U^q(b)\) is a function of \(\bar U^{q-1}\) on the bonds in and between the two blocks, to which the induction hypothesis applies. For \(q=0\) the bond either touches \(\Lambda_0(Z)\), where the field is prescribed, or lies outside \(Z\).

Now let \(b\) touch \(\Lambda_q(Z')\), say \(b_-\in\Lambda_q(Z')\). Then \(\nu_Z\le\nu_{Z'}=q\) on \(B^q(b_-)\). If \(\nu_Z\le q\) on \(B^q(b_+)\) too, the sub-claim applies. If not, \(B^q(b_+)\subset\Omega_{q+1}(Z)\); the neighbouring block \(B^q(b_-)\) then lies in \(\Omega_q(Z)\) by the separation in (1.4), so \(b_-\in\Lambda_q(Z)\) and \(\bar U^q(b)\) is itself a \(Z\)-datum. \(\square\)

**(G3) nested axial conditions.** [R] (1.15), p.78 (source input; source; the relative form (1.19) of p.79): "for \(x_j\in\Lambda_j\), \(j=1,\dots,k\), we put \(\bar U^{j-1}(\Gamma_{x_j,x_{j-1}})=1\) for \(x_{j-1}\in B(x_j)\), …, \(U(\Gamma_{x_1,x})=1\) for \(x\in B(x_1)\)", and for (1.19): "for \(x_0\in B^j(x_j)\), \(x_j\in\Lambda_j\), \(1\le j\le k\), we define a sequence of points \(x_0,x_1,\dots,x_{j-1},x_j\) by the conditions \(x_n\in B(x_{n+1})\) … The conditions (1.19) determine uniquely an element in each orbit given by the subgroup (1.14)." The product in (1.19) telescopes: \(\prod_{b\subset\Gamma}R(\bar U_0^n(\Gamma_{\cdot,b_-}))\tilde U'^n_b=\bar U^n(\Gamma)\,\bar U_0^n(\Gamma)^{-1}\). So \(\mathrm{Ax}(\mathfrak B,U_0)\) says that \(U\) and \(U_0\) have the same averaged tree holonomies, and \(\mathrm{Ax}(\mathfrak B,U_0)=\mathrm{Ax}(\mathfrak B,1)\) whenever \(U_0\in\mathrm{Ax}(\mathfrak B,1)\) deduction. The axial gauge of the reconstruction functions is the one relative to \(1\): [V] (181), p.307 source: "For the minimal configurations in the axial gauge we have \(U_k(V^v)=U_k(V)^{\tilde v}\), where \(\tilde v\) is constant on blocks \(B^j(y)\), \(y\in\Lambda_j\), and equal to \(v(y)\)", which holds for (1.15) and not for a gauge relative to a \(V\)-dependent base point. The chain of \(x_0\) stops at its level, and the averages are sequence-independent, so the \(Z\)-conditions are a subset of the \(Z'\)-conditions when \(\nu_Z\le\nu_{Z'}\)..

**(R190), normalisation.** [V] (66), p.288 source: the kernel sums are "\(\sum_{c'\in\mathfrak B_k}(L^{j'}\eta)^dH(b',c')\mathfrak D(A';c',b)\)". (69): "\(\sup_{b\subset B^j(c_-)\cup B^j(c_+)}L^j\eta\lvert H(b,c')\rvert\le B_0(L^{j'}\eta)^{-d}e^{-\delta_0d(c_-,c'_-)}\)". (71): "\(\lvert(I+\mathfrak N)^{-1}(c,c')\rvert\le2(L^{j'}\eta)^{-d}e^{-\frac12\delta_0d(c_-,c'_-)}\)", so even the identity has a kernel of size \((L^{j'}\eta)^{-d}\). (72): "the factor \((L^j\eta)^{-d}\) comes from the change of scale". Hence the factor \((L^{j'}\eta)^{-d}\) in (190) is the density with respect to the volume element \((L^{j'}\eta)^d\), and integrated against \(b\) at a top-level target point (190) gives \(O(1)\sum_{y'}e^{-r\,d(y,y')}\lvert b(y')\rvert\). This is *stronger* than the form the note uses, which carries an extra \((L^{j'}\eta)^{-1}\ge1\). The normalisation question is settled in favour source input. The plain sum is controlled by [3] Lemma 2.1, (2.61): \(\sup_y\sum_{y'\in\mathfrak B}e^{-\alpha\delta_0d(y,y')}\le c_1(\alpha)\).

**(R190), rate and status. Two defects.**

1. *Rate.* [V] (190), p.308 source: "\(\cdot(L^{j'}\eta)^{-d}\exp(-\tfrac18\delta_0d(y,y'))\)". (189) has \(-\frac14\delta_0\). The note's (R190) and its \(T(D)\) use \(\frac12\delta_0\), which is the rate of the *linear* bound (161). With the printed rate, \(T(D_0)\le C_Te^{-\delta_0D_0/16}\), the bound of \(S_{1/2}\) by \(B_3\) is not available (use \(c_1(\frac18)\)), and \(M_0\) grows by a factor of about 4. Check (4) of finite comparison shows how much weaker \(T\) is.
2. *Hypotheses.* [V] p.308 source: "To prove an exponential decay we have to investigate more closely the kernel \(((\delta^2/\delta A'^2)V)(A')\). This is, unfortunately, a very awkward and complicated problem, although quite straightforward. … **We do not perform these calculations here**, we have obtained all necessary results to do the calculations and estimates, let us formulate a final result only. We have [(189)]." (190) is derived from (189). So **(190) at non-zero data is a source assertion without a source proof.** This confirms finding F1 of the C-05 note. At zero data \(\delta\mathcal H/\delta B=H_1\) ([V] (177): "the expansion of \(\mathcal H\) begins with the first order term \(H_1B\)"), and that case is the linear propagator bound.

**(1.17) on \(\Omega_n\).** For real data, [V] Theorem 1 source: the minimal orbit lies in \(\mathfrak U_k(\{\Omega_j\},B_3\varepsilon_1)\), i.e. \(\lvert\partial U-1\rvert<B_3\varepsilon_1L^{-2j}\) on \(\Omega_j\). With \(\varepsilon_1=2\alpha_0'(L^n\xi)^2\) this is \(2B_3\alpha_0'\xi^2\) on all of \(\Omega_n\). The printed "on \(\tilde X^{-2}\)" is a sub-region. Settled for real data. For complex data see §2.6.

### 2.2 Step A (identity on \(Z\)): correct

The argument is the one Bałaban uses himself at [V] (150), p.301 source: "The configuration \(U'_k\) is a minimum of the functional (5) in the space (6) with \(V'\) instead of \(V\), hence it is a minimum of this functional in the space (150), because this space is defined by more restrictive functional conditions and a sufficiently small neighborhood of \(U'_k\) in (150) is contained in (6)."

Checked: [V] works on \(\Omega_0\subset T_\eta\) with the field prescribed on \(\Lambda_0\) (p.277–278: "gauge field configurations on \(\Omega_0\)", action summed over \(p\subset\Omega_0\)), so \(Z\) is an admissible \(\Omega_0\). Variable bonds have both ends in \(\Omega_1(Z)\), so the two actions differ by a constant on \(\iota\mathcal M_Z\) whatever the convention for boundary plaquettes. Uniqueness is used in the space (6) for \(Z\) with \(\varepsilon_0=B_3\varepsilon_1^\circ\), \(\varepsilon_1^\circ=O(B_3\varepsilon_1)\) ([V] p.278: "\(V\) satisfies (7) with \(\varepsilon_1=O(\varepsilon_0)\)"); this is a ceiling \(O(B_3^2a_0)\le a_0^{[V]}\), as the note says. conditional from (V1), (G2), (G3).

### 2.3 Step B (collar bound): correct

[R] p.87 source: "By Proposition 2 of [3] the bounds \(\lvert\partial U-1\rvert<\alpha_0\eta^2\) imply \(\lvert\partial\bar U^j-1\rvert<\dots<2\alpha_0L^{2j}\eta^2\) … let us apply Lemma 1 to \(V_0=\bar U_0^{k-1}\), \(V'V_0=(\overline{U'U_0})^{k-1}\) … Thus the conditions (1.33)–(1.35) imply \(\lvert(\overline{U'U_0})^j-\bar U_0^j\rvert=\lvert\tilde U'^j-1\rvert<11d^2\alpha_0+\alpha_1\) on \(\Omega_j^{(j)}\). (1.65)". Use the note that the displayed derivation uses the plaquette conditions and the axial gauge only, not the second-order condition (1.9). The bound holds on \(\Omega_j(Z')^{(j)}\) for every \(j\), which is what gives the lower-level data on \(\Gamma\).

One imprecision: the gauge transformation that puts \(U\) in \(\mathrm{Ax}(\mathfrak B(Z'),W')\) does change the \(Z\)-data, by a transformation that is \(1\) on \(\mathfrak B(Z')\) but not on the lower-level points of \(\mathfrak B(Z)\). By (181) this changes \(R_n[Z](U)\) by a block-constant gauge transformation which equals \(1\) on the top-level blocks of \(Z\) (their centres lie in \(\Lambda_n(Z)\subset\Lambda_n(Z')\)). So nothing changes on \(Z^{(n)}\)..

### 2.4 Step C (decay): must be re-based

As written, Step C rests on (190) at the non-zero data \(tB\). By §2.1 this is an unproved source statement with the wrong rate. The step does not need it.

> **Lemma 2.1 (decay step without (190)).** Let \(V_0\) be real data satisfying [V] (7) with \(\varepsilon_1^*\), the largest \(\varepsilon_1\) admitted by [V] Proposition 9, and let \(\rho:=2C_1\varepsilon_1^*\). Assume:
> - (V2) \(\mathcal H\) is analytic on \(\{\lvert B\rvert_\infty<\rho\}\), \(\mathcal H(0)=0\), \(D\mathcal H(0)=H_1\), and \(\mathcal H\) satisfies [V] (19) with \(\varepsilon_2=B_5\varepsilon_1^*\) there ([V] (173), (177), Proposition 9);
> - (V3′) the linear bound: for a top-level point \(x\in\Delta(y)\), \(\max\{\lvert H_1b\rvert,\lvert\nabla H_1b\rvert,\lvert D^*DH_1b\rvert,\lvert\Delta H_1b\rvert\}(x)\le B_H\sum_{c}e^{-\frac12\delta_0d(y,c_-)}(L^{j(c)}\eta)^{-1}\lvert b(c)\rvert\) ([V] (161) for the operators without background; [P] (3.126)–(3.133) and (3.134)–(3.138) for \(H\), \(H_1\) in a regular background).
> Then for \(\lvert B\rvert_\infty\le\rho/2\), with \(N(B):=\mathcal H(B)-H_1B\) and \(\lVert\cdot\rVert\) the maximum of the four top-level norms,
> \[
> \lVert N(B)\rVert\le\frac{2B_5\varepsilon_1^*}{\rho^2}\,\lvert B\rvert_\infty^2=\frac{B_5}{C_1\rho}\lvert B\rvert_\infty^2.
> \]
> If \(B\) is supported on \(\Gamma\) and \(\lvert B\rvert\le b_{\max}\), then at every top-level point at distance \(\ge D_0\) from \(\Omega_n(Z)^c\)
> \[
> h\ \le\ d\,B_H\,b_{\max}\,T_{1/2}(D_0)\,S_{1/2}\ +\ \frac{B_5}{C_1\rho}\,b_{\max}^2.
> \]

*Proof.* For fixed \(B\) put \(g(t):=\mathcal H(t\rho B/\lvert B\rvert_\infty)\), analytic on \(\lvert t\rvert<1\) with values in the Banach space of the norm \(\lVert\cdot\rVert\), bounded by \(K:=B_5\varepsilon_1^*\), with \(g(0)=0\). The Taylor coefficients satisfy \(\lVert c_m\rVert\le K\), so \(\lVert g(t)-tg'(0)\rVert\le K\lvert t\rvert^2/(1-\lvert t\rvert)\le2K\lvert t\rvert^2\) for \(\lvert t\rvert\le\frac12\). Take \(t=\lvert B\rvert_\infty/\rho\). The second display is the corresponding splitting of the distance applied to \(H_1B\), which is exact for a geodesic distance. \(\square\) deduction, given (V2), (V3′).

Consequences.

- With \(b_{\max}=44d^2B_3a_0\ell_n^2\) the real bound becomes
\[
\Theta_{\mathbb R}=\big[K_{\rm lin}T_{1/2}(D_0)+K_{\rm nl}\,a_0\ell_n^2\big]\,a_0,\qquad K_{\rm lin}=\frac{11}{9}\frac{\max\{C_p,C_J\}B_HB_3^2}{L^3B_0},\quad K_{\rm nl}=2\max\{C_p,C_J\}\frac{B_5}{C_1\rho}(44d^2B_3)^2.
\]
The rate is \(\frac12\delta_0\), so the corresponding \(T(D)\), \(C_T\) and \(S_{1/2}\le B_3/(72d^3L^3B_0)\) stand as printed, with \(K_9\) replaced by \(B_H\).
- The new term is not small in \(M\). It is small in the coupling: \(K_{\rm nl}a_0\le\beta/4\) is a ceiling of the same kind as (K5). In the scaled use for (X-far) it carries the extra factor \(L^{-2(m+1)}\ell_n^2\).
- Status of (V3′): the first-order and Hölder norms in a background are [P] (3.133) (source input; text: "\(\lvert H_{\mu\nu}(x,y')\rvert,\lvert\nabla H(x,y')\rvert,\lVert\zeta\nabla H(\cdot,y')\rVert_\beta\le O(1)[\dots]e^{-\frac12\delta_0d(y,y')}\)"), obtained from Theorems 3.1–3.3 and the random-walk expansions of Theorems 3.7–3.10, which have displayed proofs; the passage to \((QGQ^*)^{-1}\) is "analyzed in the same way … We will not repeat these considerations here". [P] p.422 states the exception: "with the exception of the inequality involving the covariant Laplace operator in (3.42)". The second-order norms are available for the second representation ([V] (179)–(180), p.306: "the new operator \(\tilde G\) has exactly the same properties as \(\Delta_a^{-1}\)"; CMP109 p.272 explains the use of the Landau gauge to replace \(D^*D\) by \(\Delta-P_1\)). So: **plaquette clause, re-based on displayed proofs up to the "same way" remark; current clause, re-based on a one-sentence source statement.** The argument assumes either.
- This is simpler than the repair proposed in the C-05 note (its Lemma 3 needs a decoupling expansion of \(\mathcal H\) on a general multiscale sequence). Lemma 3 is needed where genuine *decay of the nonlinear response* is used, e.g. (S3) of L1\(^*\) for far carriers (CMP109 (3.8)–(3.9)); the locality theorem needs only its smallness.

### 2.5 Step D (plaquettes, currents, gauge factor): correct

For the real corollary the gauge factor is not needed, since \(\lvert\partial W-1\rvert\) and \(\lvert J_n(W)\rvert\) are invariant under unitary transformations. It is needed for the *difference* \(F\) in Step E, and there the citation is right: by §2.1 (G3), the transformation from the Landau gauge relative to \(\hat W\) to \(\mathrm{Ax}(\mathfrak B(Z),\hat W)=\mathrm{Ax}(\mathfrak B(Z),1)\) is the \(u_1\) of [R] (1.70)–(1.72) (c)-1\rvert\le2\sum_{n=0}^{j-1}\max_{x\in B(x_{n+1})}\lvert\frac1i\log(\bar R^n_{0,x_{n+1}}\bar U_1^n)(\Gamma_{x_{n+1},x})\rvert\)"), and it is local in the chain of blocks of \(x\).

### 2.6 Step E (complex data): correct as an implication; its boundary input is not established

**What is right.** The family \(\mathbf U_z\), the analyticity of \(F\) on a neighbourhood of the closed half-disc (the data of \(\mathbf U_z\) differ from the real data of \(\mathbf U_{\mathrm{Re}z}\) by \(O(a_1\ell_p)\le O(a_1)\), inside the ball of Proposition 9 under an absolute ceiling on \(a_1\)), the bound on the diameter from part deduction with \(a_*\), the subharmonicity of \(\log\lVert F\rVert\), and \(\omega_0=\frac4\pi\arctan\frac12=1-\frac4\pi\arctan\frac13\). The quantity bounded at \(z=i\) is the one clause (iv) needs: the plaquette and current of the axial representative of \(U_n(Z;M'(\mathbf U))\) for the given representative \(\mathbf U\).

**What is not established: the bound on the arc.** The note takes \(F_{\max}=4B_3a_*\xi^2\) from (V8) = CMP109 (1.17) applied to \(\mathbf U_z\). CMP109 p.263 source: "We have \(M'(\mathbf U)=\bar{\mathbf U}^p\) on \(\Lambda_p\), \(\lvert\partial\bar{\mathbf U}^p-1\rvert<2\alpha_0'(L^p\xi)^2\). From Proposition 9 [15] we obtain \(\lvert\partial U_n(M'(\mathbf U))-1\rvert<B_32\alpha_0'L^{-2n}(L^n\xi)^2=2B_3\alpha_0'\xi^2\) …". Proposition 9 is stated for \(V=V'V_0\) with \(V_0\) real satisfying (7) with \(\varepsilon_1\) and "\(\lvert V'-1\rvert<C_1\varepsilon_1\)" ([V] (172)), and its conclusion is (19) with \(\varepsilon_2=B_5\varepsilon_1\). For \(\mathbf U=\exp(i\xi A')U\):

- the complex part of the data at level \(p\) is \(V'=\bar{\mathbf U}^p(\bar U^p)^{-1}\approx\exp(iL^p\xi\,Q_pA')\), of size \(\alpha_1'L^p\xi\): first order in the block length;
- the admitted size is \(C_1\varepsilon_1=2C_1\alpha_0'(L^n\xi)^2\): second order.

So the hypothesis of Proposition 9 with the \(\varepsilon_1\) of (1.17) fails as soon as \(\alpha_1'>2C_1\alpha_0'L^n\xi\): at every sufficiently deep level, and already at the top level when \(\alpha_1'>2C_1\alpha_0'\) (on the running chart the radius ratio is \(\propto M\), (K1) of L1\(^*\)). Applying Proposition 9 with the \(\varepsilon_1\) it actually admits gives
\[
\lvert\partial U_n(M'(\mathbf U))-1\rvert\ \lesssim\ \big(2B_3\alpha_0'+C\,B_5\,\alpha_1'(L^n\xi)^{-1}\big)\xi^2 ,
\]
which is not uniform in the depth \(s-n\). The gauge freedom (181) does not help on a general domain: a complex configuration with small curvature is within \(C_1\varepsilon_1\) of a real one, after a complex gauge transformation, only on cubes of bounded size (this is CMP109 (3.26), with the factor \(M\)).

Conjecturally, (1.17) is *true* for complex data with some constant. In the abelian case it follows from the real theorem by linearity. In general the first-order response to \(A'\) is a gauge transformation plus a term controlled by \(\nabla A'\). But a proof needs an estimate that uses the smoothness of \(A'\) (the reconstruction nearly reproduces slowly varying fields), and no displayed source estimate does that. Status of (1.17) for complex data: **source input as an assertion; not proved in the source; not proved here.**

**Effect on Step E.** With the honest arc bound the result is \(\Theta_{\mathbb C}\propto\ell_n^{-(1-\omega_0)}=L^{0.41(s-n)}\) (check (3)). Enlarging the half-disc to radius \(R\sim\log\ell_n^{-1}\) removes the power but leaves a factor linear in the depth. Neither is acceptable, since (X-far) needs all levels \(n\le j\) with no slack in \(j-n\).

**What Step E needs.** Only a crude bound, with any constant:

> **(CR) Complex regularity of reconstructions.** There is \(K_c<\infty\), depending on \(d,L\) and at most polynomially on \(M\), such that for every scale \(s\), level \(n\le s\), domain \(Z\) and complex \(\mathbf U\) satisfying (i)–(iii) on \(Z\) with radii \((a,a_1)\) below a ceiling: \(\lvert\partial U_n(Z;M'(\mathbf U))-1\rvert\le K_c\,(a+a_1^\nabla+a_1^2)\,\xi^2\) and \(\lvert J_n\rvert\le K_c(a+a_1^\nabla+a_1^2)\ell_n^2\) on \(Z^{(n)}\), where \(a_1^\nabla\) bounds \(\lvert\nabla_UA'\rvert\).

CMP109 (1.17) asserts (CR) with \(K_c=2B_3\) and without the \(a_1\) terms. Given (CR), Step E gives \(\Theta_{\mathbb C}=(2K_ca_*)^{1-\omega_0}\,\Theta_{\mathbb R}(a_*)^{\omega_0}\). conditional.

**Three further points on part conditional.**

1. *The same premise sits under earlier work.* L1\(^*\) uses (1.17) "repeatedly" (§2.2), and the manuscript's Annex AD obtains the reconstructed-field clause for *complex* insertions from it ((E14.32): "relative-field and insertion perturbations whose required norms are all less than \(u_j=c_{\rm loc}\min\{\alpha_{0,j},\alpha_{1,j}\}\) … CMP109 p.263 supplies its reconstructed-field clauses, with its displayed factor \(2B_3\)"). A perturbation of size \(c_{\rm loc}\alpha_0\) changes the level-\(n\) data by \(c_{\rm loc}\alpha_0\ell_n\), again first order. So (CR), in a Lipschitz form, is also what (S5) (the A-ball) and (E14.32) need. This is independent of (iv\(_t\)).
2. *The complex identity.* Step A extends to complex data by analytic continuation (both sides are analytic in the data and agree on real data). The note does not need this, but Lemma 5.1, Step 5 of L1\(^*\) (CMP109 (3.38)) does, and it is the reason clause (iv) holds on all of \(X\) for the near configurations.
3. *Age-freeness needs two radii.* The note's \(\mathcal K_s(Z';a_0,a_1)\) uses one radius for \(\lvert A'\rvert\) and \(\lvert\nabla_UA'\rvert\), and \(a_*=a_0+4C_Aa_1\). In the (X-far) use at age \(m\) the scale-\(j\) values are \(\lvert A'\rvert\le a_1'L^{-(m+1)}\) and \(\lvert\nabla A'\rvert\le a_1'L^{-2(m+1)}\) (L1\(^*\) §4.2). With the single radius, \(a_*/a_0\) grows like \(L^{m+1}\), and the statement "the relative loss \(\Theta_{\rm rel}\) is scale-free" (note §6.2) is false as derived. It is true with \(a_*:=a_0+C_A(4a_1^\nabla+16a_1^2)\), which is what the proof of Step E uses. The theorem should be restated with \((a_0;a_1,a_1^\nabla)\).

### 2.7 Lemma 3.1 and the region \(Z^{(n)}\): the metric

Lemma 3.1(2) uses "\(\mathrm{dist}_1(x',\Omega_p^c)\ge R_1M_1\ell_p+dM_1\ell_{p+1}\Rightarrow\) the block of \(x'\) is admissible". Admissibility is \(\mathrm{dist}(c,\Omega_p^c)>R_1M_1\ell_p\) in the source's metric, which is not specified. If it is \(\ell^\infty\) or Euclidean the implication fails by a factor up to \(d\). The source's region is made of cube layers, i.e. \(\ell^\infty\). Fix: define \(Z^{(n)}\) and the collar with \(\mathrm{dist}_\infty\). Then \(\mathrm{dist}_\infty\ge R\) implies the same in \(\ell^2\) and \(\ell^1\), the block diameter is \(M_1\ell_{p+1}\), and the collar is at most \(2(1+L)R_1M_1\ell_{n-1}\) for every reading of the source's metric. The contour distance \(d(\cdot,\cdot)\) dominates the \(\ell^\infty\) distance, so Step C is unaffected. With \(\mathrm{dist}_\infty\), "\(\tilde\square^3=\square_0^{(k+1)}\)" is an exact equality; with \(\mathrm{dist}_1\) it is exact only for convex domains..

### 2.8 The theorem as it stands after the analysis

> **Theorem 4.1′.** Let \(Z\subset Z'\), \(1\le n\le s\), \(Z^{(n)}:=\{x\in Z:\mathrm{dist}_\infty(x,Z^c)\ge2M\ell_{n-1}\}\), \(D_0:=(2M-2(1+L)R_1M_1)/L-1>0\), and \(\mathbf U\) satisfy the plaquette parts of (i)–(iii) on \(Z'\) with radii \((a_0;a_1,a_1^\nabla)\) below a ceiling. Put \(a_*:=a_0+C_A(4a_1^\nabla+16a_1^2)\).
> (a) Real \(\mathbf U\): on \(Z^{(n)}\), \(\lvert\partial W-\partial W'\rvert\le\Theta_{\mathbb R}(a_0)\xi^2\), \(\lvert J_n(W)-J_n(W')\rvert\le\Theta_{\mathbb R}(a_0)\ell_n^2\), \(\Theta_{\mathbb R}(a)=[K_{\rm lin}T_{1/2}(D_0)+K_{\rm nl}a]a\). Inputs: (V1), (V2), (V3′), (V5), (V6), (V7). No reading remains, and (190) is not used.
> (b) Complex \(\mathbf U\), assuming (CR): the same with \(\Theta_{\mathbb C}=(2K_ca_*)^{1-\omega_0}\Theta_{\mathbb R}(a_*)^{\omega_0}\).

Condition replacing (K8): \(\Theta_{\mathbb C}\le\frac\beta2a_0\), i.e.
\[
(2K_c)^{1-\omega_0}\,\frac{a_*}{a_0}\,\big[K_{\rm lin}C_Te^{-\delta_0D_0/4}+K_{\rm nl}a_*\big]^{\omega_0}\le\frac\beta2.
\tag{K8′}
\]
It holds for \(M\ge M_0\) (first term) and below a coupling ceiling that depends on \(M\) (second term). The order "first \(L\), then \(M\), then the ratios, then the ceilings" is respected.

## 3. The literal clause and the nesting failure

### 3.1 The literal reading is right

CMP109 p.262 source: "\(\lvert\partial U_n(M'(\mathbf U))-1\rvert<\alpha_0\xi^2\), \(\lvert J_n(M'(\mathbf U))\rvert<\alpha_0(L^n\xi)^2\) on \(\tilde X^{-2}\), (1.16) and the same bounds hold for \(U\) instead of \(\mathbf U\). The domain \(\tilde X^{-2}\) is obtained from \(X\) by taking away two layers of cubes from \(\pi_j\) which are closest to the boundary of \(X\). Thus it is a domain \(X'\) such that \(\tilde X'^2=X\)." One region for all levels \(n\le j\), in cubes of \(X\)'s own class.

The source does not itself keep to "cubes of \(\pi_j\)" when the domain has another class. CMP109 p.273 (source input; text): "We take the function \(U_j\) constructed for the cube \(\square_0=\tilde\square^5\) as in the condition (iv) … hence \(\tilde\square^4\subset\square_{k+1}\)"; p.275: "the space \(U^c_{k+1}(\square_0,(1+2\beta)\alpha_0,(1+2\beta)\alpha_1,\alpha_0)\). This space is defined by the same conditions (i)–(iv), only the configurations \(\mathbf U,\mathbf J\) are defined and satisfy (i)–(iii) on the whole lattice"; p.278: membership "implies in particular the inequalities … on \(\tilde\square^3\)". So for the scale-\((k+1)\) space on a domain of class \(\mathbf D_k\) the layers are cubes of \(\pi_k\): thickness \(2M\) in step-\(k\) units, against \(2LM\) for a polymer of \(\mathbf D_{k+1}\). CMP116 inherits the definition by reference ("conditions I.(i)–(iv)", p.22) and asserts the inclusions: p.7 "we take its subspace \(U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\). All terms (1.23) with the localization domain \(Y\) are defined and analytic on this space"; p.9 "All these spaces contain the subspace \(U^c_{k+1}(Y,\dots)\)"; p.15 "The potentials are also analytic functions on the subspace \(U^c_{k+1}(X,\alpha_0,\alpha_1)\)". CMP119 p.259 uses the same E-spaces by reference. Its B-spaces (2.34)–(2.39), p.261 source input, are defined separately, with reconstructed conditions "on \(X\cap(\Omega_n\backslash\Omega_{n+1})\) for \(n=1,\dots,j-1\), or on \(X\cap\Omega_j\) for \(n=j\)": no layers are removed there.

The note's table of thicknesses (§3.3) and its four nesting verdicts are correct. deduction, given the quotes.

### 3.2 (S-Res-1) is false for the literal spaces

Two facts.

**(i) For small polymers the literal clause is void.** If \(X\in\mathbf D_{k+1}\) is fewer than five \(LM\)-cubes wide in some direction, \(\tilde X^{-2}=\emptyset\), and the literal \(U^c_{k+1}(X,\alpha_0,\alpha_1)\) is defined by (i)–(iii) alone. A potential domain \(Y\subset X\) of class \(\mathbf D_k\) at least five \(M\)-cubes wide has \(Y^{-2}\ne\emptyset\). (S-Res-1) then says: (i)–(iii) with \(\alpha_0\) imply clause (iv) on \(Y^{-2}\) with \((1+\beta)\alpha_0\). deduction; check (2).

**(ii) Clause (iv) does not follow from (iii) with a loss \(1+\beta\).** Take \(\mathbf U\) real with values in a \(U(1)\) subgroup. By uniqueness the minimiser is \(U(1)\)-valued, and to leading order in the field it minimises \(\sum_pF(p)^2\) under Bałaban's block-average constraints. For the one-step average [A] (42), \(\bar A(c)=L^{-d}\sum_{x\in B(c_-)}A(\Gamma_{c,x})\), and the tree contours cancel around a block plaquette, so
\[
(d\bar A)(P)=\sum_pw_P(p)F(p),\qquad w_P(p)=L^{-d}\#\{x\in B(y):\ p\subset\text{the }L\times L\text{ square at }x\}.
\]

| \(L\) | 2 | 3 | 5 | 7 |
|---|---|---|---|---|
| \(\lVert P\rVert_{\infty\to\infty}\) (plaquette) | 2.91 | 3.47 | 3.57 | 3.88 |

(check (1); numerically the 1D value tends to 2 as \(L\) grows, so the plaquette value tends to 4). The extremal sign patterns have exponentially decaying influence, so they can be cut off within a few blocks. Hence there are real configurations with \(\lvert\partial U-1\rvert\le\alpha_0\xi^2\) everywhere whose level-1 reconstruction has a plaquette of size \(\approx2.9\,\alpha_0\xi^2\) at a point of \(Y^{-2}\). Such a configuration lies in the literal space of a small polymer \(X\) and its restriction is not in \(U^c_{k+1}(Y,(1+\beta)\alpha_0,\dots)\) for \(\beta<1.9\).

For a large polymer the same pattern placed in the strip \(X\setminus\tilde X^{-2}\) gives the same conclusion; clause (iv) on \(\tilde X^{-2}\) is kept by Theorem 4.1′(a) applied to a sub-domain on which the configuration is trivial.

Hypotheses: deduction for the abelian quadratic theory in the plane; additional assumption for the transfer to \(d=4\) (planar configurations, slow cutoff in the other directions) and for the \(O(\alpha_0^2)\) corrections. The note's "plausibly false" can be upgraded to "false to leading order". The same computation shows \(K_{\rm amp}\ge2.9\), so the route "clause (iv) from (i)–(iii)" needs a loss of at least that size at every level, in line with L1\(^*\)'s exclusion of the (1.17) route.

**Consequence.** With the literal definition the claim on CMP116 p.15 fails, and CMP116 Lemma 1 / CMP119 Theorem 1 are not established on the literal native spaces. The induction has to be run on smaller native spaces. (iv\(_t\)) is such a choice.

For (X-far) at ages \(1\le m<m_\flat\) the literal statement is probably true (it needs \(K_{\rm amp}(1+\beta)\le\frac12L^{2(m+1)}/\Gamma_m\), and \(K_{\rm amp}\approx3\)–\(4\) would do for \(m\ge1\)), but only \(K_{\rm amp}\le2B_3\) is proved. The note's "not derivable" is the right description.

## 4. Compatibility of (iv\(_t\))

### 4.1 Comparison with the literal clause

For a native space (\(X\in\mathbf D_j\)) the literal region is \(\{\mathrm{dist}_\infty\ge2M\ell_j\}\) for every level; the (iv\(_t\)) region for level \(n\) is \(\{\mathrm{dist}_\infty\ge2M\ell_{n-1}\}\), which contains it since \(n-1<j\). For the scale-\((k+1)\) spaces on \(\mathbf D_k\)-domains the two agree at the top level and (iv\(_t\)) is larger below. So **(iv\(_t\)) is the stronger condition and the (iv\(_t\))-spaces are subsets of the literal ones**; the two are never incomparable. As an inductive statement "\(\mathbf E^{(j)}(X)\) is analytic and bounded on the space" it is the weaker one..

An equivalent wording: *level \(n\) is controlled on \(Z\) minus two layers of cubes of \(\pi_{n-1}\)*. This is the source's sentence with \(\pi_j\) replaced by \(\pi_{n-1}\), and it is what the source does at the only place where it uses the clause as a hypothesis (level \(k+1\), cubes of \(\pi_k\), on \(\square_0\)).

### 4.2 The actual map is not changed

The spaces enter the sources only as analyticity domains of the localized terms: CMP109 p.263 ("We assume that the function \(\mathbf E^{(j)}(X,g_{j-1},\mathbf U,\mathbf J)\) is defined and analytic on the space \(U^c_j(X,\alpha_0,\alpha_1)\)"), CMP119 p.259 (property (ii) of the E-terms). The renormalization transformations, gauge fixing, and the small- and large-field characteristic functions are defined on real fields. LFR I p.190 (source input; text) gives the direction of dependence: the complex spaces "are modelled on the definition (1.24) of the characteristic functions \(\chi_k^{(n)}\), and on the definition of the spaces \(U^c_k(X,\alpha_0,\alpha_1)\)", "in agreement with the restrictions introduced by the characteristic function". The decomposition into small and large fields does not reference clause (iv). The extended functions are given by the same formulas on the smaller domain, and they agree with the real densities at real points. So the effective densities, the map \(V_k\mapsto V_{k+1}\) and the coupling recursion are unchanged; (iv\(_t\)) changes the domain on which an inductive *bound* is asserted. B-03's "actual map" requirement is not at stake..

What must be checked instead is that every configuration fed to an analytic extension lies in the smaller space, and that the Cauchy radii survive.

### 4.3 Uses, one by one

| Use | Where | Needs | Under (iv\(_t\)) |
|---|---|---|---|
| Hypothesis: level \(k+1\) on \(\tilde\square^3\) | CMP109 (3.40)–(3.41); L1\(^*\) Lemma 5.1 Step 0 | \(\tilde\square^3\subset\square_0^{(k+1)}\) | equality (with \(\mathrm{dist}_\infty\)) |
| Membership of near configurations \(U_j(\square_0,\cdot)\vert_X\) | CMP109 (3.36)–(3.38), Lemma 4 | reconstruction of a minimiser is itself | Step A, on all of \(X\); complex data by continuation (§2.6, 2). Survives |
| Far carriers | CMP109 (3.16); CMP116 p.9 | (X-far) | Corollary 4.2 with nested regions; real: Theorem 4.1′deduction; complex: needs (CR) |
| Potentials on the cube and on \(Y\) | CMP116 p.7 | (S-Res-2) | as above |
| Births on polymer spaces | CMP116 p.15; Lemma L2 | (S-Res-1) | as above; false under the literal clause (§3.2) |
| A-ball | CMP109 (3.13)–(3.14), (4.4); (S5) | response of all reconstructions to a smooth perturbation | not region-sensitive; rests on a Lipschitz form of (CR) in either convention |
| Actual backgrounds in the spaces | CMP109 p.263 | real (1.17) or the identity | [V] Theorem 1 on \(\Omega_n\supset Z^{(n)}\), for \(M\ge(1+L)R_1M_1\) |
| Manuscript, Annex AD (E14.26)–(E14.32), Annex AE, and the proposition resting on them (C-02, C-03, C-04) | "smaller basic domain" | (1.17): (i)–(iii) with \(\alpha_0'\le\alpha_0/(16B_3)\) imply (iv) | region-insensitive; real centres by Theorem 1; complex tubes rest on (CR), as before |
| Euclidean covariance, gauge invariance, monotonicity in the radii | CMP109 p.263; (H3), (H4) | — | \(Z^{(n)}\) is defined by a distance, so it is covariant; orbits and monotonicity as before |
| B-terms, R-step outputs | CMP119 (2.34)–(2.39); LFR I (1.64)–(1.69); LFR II (1.65) | own definitions | untouched |

Only level-adapted native-domain inclusions are used below.

**Not covered by this analysis.** Inclusions between the multiscale spaces of CMP119/LFR and the E-spaces, e.g. LFR II p.373: "the space \(U^c_k(Y_1,\alpha_0,\alpha_1)\) is contained in the analyticity domain of the term \(\mathbf E(X)\) … It is simple to see for all the old terms, because … the regularity conditions … are weaker than the regularity conditions for the new determining set". These are assertions of the same kind as (S-Res). With (iv\(_t\)) the E-space is smaller, so they are not easier. They belong to C-05 and the R-operation, not to B-03's E/R-potential chain. The C-05 team should be told of the convention.

### 4.4 Is the literal clause essential anywhere?

It would be if some configuration were known to lie only in the literal space and had to be inserted into an E- or R-term. There is no identifiedne: every insertion in CMP109 §3, CMP116 §1 and Annexes AD/AE is a minimiser (identity), a real regular configuration ((1.17), real), or a small perturbation of one ((S5)/(E14.32)). Status conditional, limited to what was read (§1).
