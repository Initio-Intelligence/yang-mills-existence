# Tensor quadratic admission and the marked transition

This note belongs to the revised Yang–Mills existence route. It supplements, and does not replace, the regular-family analysis of §§4.25–4.26 in [Regular jet transport, pressure and coupling windows](regular_jets.md). Its labels mean **P**: proved here; **L**: checked primary assertion used with its hypotheses; **C**: a proved implication under explicitly displayed additional hypotheses; **O**: not proved. No interface beyond the verbatim N2-F quoted in [Lattice conventions and hypotheses](../lattice_conventions.md), §2, is assumed. In particular, a source-free stability theorem is not assumed to extend to a sourced density.

## 1. Outcome and scope

**R1 is not completed.** The new result below establishes a relative constrained Hessian bound for all 21 components of a clover curvature-pair source at an already regular background with one averaging scale. It includes the nonlinear constraint curvature and does not differentiate the source. Its Gaussian inverse and determinant consequences are uniform in the fine spacing in the relative energy norm. The determinant estimate retains the actual number of Gaussian coordinates. It does not turn that number into a physical-cell count.

The remaining step is an estimate for the actual source-dependent local activities produced after regular integration and then passed through a mixed regular/large-field transition. It must include the dependence of old source readouts on retained fields. A raw bound on the original, wholly unintegrated source minus its vacuum counterterm is false, as the Wilson-measure argument in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md), §§2–3, proves. Accordingly, the residual norm in §4 is expressly a norm **after the designated regular integrations**, before cancellation of compulsory large-field masses. This is a real restriction on the admissible representation, not a change in the physical source.

### 1.1 What the previous regular-family result actually imports

Write **B109** for Bałaban, CMP 109 (1987), 249–301, **B116** for Bałaban, CMP 116 (1988), 1–22, and **B99** for Bałaban, CMP 99 (1985), 389–434. Printed journal pages are used throughout.

B109 p.263 explicitly assumes that each regular activity is analytic on its fixed complex background domain, depends only on its localization, is smooth in the coupling through zero, and satisfies

\[
 |E^{(j)}(X,g_{j-1},U,J)|\le E_0e^{-\kappa d_j(X)}.
 \tag{R1.1; L: B109 (1.18), p.263}
\]

B109 Theorem 3, p.264, propagates the inductive assumptions (1.1)–(1.22) under the stated regular renormalization transformations and sufficiently small construction parameters. It is a source-free theorem with its printed geometry and regular-domain hypotheses.

The Gaussian activity is not merely inferred from a cited reference. B116 p.21, in the paragraph immediately after (2.41), explicitly states that

\[
 \log Z^{(k)}(U_{k+1})-\log Z^{(k)}(1)
   =\sum_X G_{k+1}(X;U,J),
 \qquad
 |G_{k+1}(X;U,J)|\le \tfrac12E_0e^{-\kappa d_{k+1}(X)},
 \tag{R1.2; L: B116 p.21, paragraph after (2.41)}
\]

after the choices described there: its initially obtained decay exponent is \(\delta_0M\), its initial prefactor is an absolute constant, and \(E_0\) and \(M\) are chosen so that this is the required half-budget. The paragraph explicitly supplies localization in \(X\), analytic extension in \((U,J)\), and the (I.1.18) bound. Here \(J\) is Balaban's determining background variable; it is not the external tensor source of this note.

The underlying generalized random-walk derivation is referred there to [16], formula (63), CMP 102, pp.255–275. That formula is not reproduced or re-derived here. Thus (R1.2) is a checked **L assertion from B116 p.21**, not a new proof of that earlier construction. The previous universal regular-family argument may use this fixed, source-free Gaussian family as an L input, while proving its non-Gaussian activity map and its parameter derivatives on that fixed family. It does **not** thereby prove localization for an arbitrarily source-dependent Gaussian operator, or for the Gaussian family of a displaced sourced minimum.

Consequently the fixed-G regular claim remains valid as an L input, even though the referenced earlier proof is not reproduced here. Its scope must continue to say *fixed source-free G, admitted regular domains*. Any claim of a fresh proof of (63), or a sourced Gaussian extension from the same citation, would exceed the cited text.

### 1.2 Why the tensor calculation needs a separate proof

The scalar Hessian section of [Wilson source weights and localization of the vacuum term](wilson_weights_and_cell_localization.md) proves a one-scale bound for arbitrary diagonal Wilson weights. A clover source also contains mixed products of curvature components. Its first variation is therefore not obtained by simply multiplying the Wilson curvature by a scalar weight. In particular, B99's curl arises after a cyclic rearrangement inside a trace; the untraced plaquette derivative needed for a clover has an additional curvature-small term. The proof below keeps that term explicitly. This prevents an incorrect use of the identity \(J_f=D^*(fF)\) outside its Wilson setting.

**Related results.** The full R1 norm below is still unclosed. [Raw core sources in the large-field operation](../raw_core.md) proves one actual module: strict original-variable core sources through the erased-R complex kernel, connected expansion and flat vacuum subtraction, with whole-operation ownership and the stated reserve hierarchy. Its exact remaining complementary density jets are (MR.27). [Cross-shell Gaussian source transport and local vacuum](cross_shell_gaussian_source.md) closes the whole flat Gaussian source, and [Uniform cyclic Gaussian carriers](../cyclic_carriers.md) controls growing pinned Gaussian exterior carriers. The actual mixed E/B, boundary and reconstruction map and its invariant complete norm remain open.

## 2. All clover tensor directions in a fixed constrained quadratic form

### 2.1 Exact hypotheses and normalization

Let the fine lattice spacing be \(\eta\), and let \(h\ge\eta\) be the single averaging scale. Work on a finite periodic or boundary geometry admitted by B99's propagator theorems. Fix a **real source-free** background satisfying B99 (3.35)–(3.36), p.396, with \(\varepsilon=M\alpha_0\) sufficiently small. In particular, its plaquette matrices obey the gauge-invariant consequence

\[
 \|P_p-I\|\le C\varepsilon\eta^2h^{-2}.
 \tag{R1.3; P from the L regularity hypotheses}
\]

Use B99's Hermitian fluctuation coordinates: a positive link changes as \(U_b(t)=e^{i\eta tA_b}U_b\), and negative links are the inverses of the corresponding positive links. All fine inner products use measure \(\eta^d\) and normalized trace \(\operatorname{tr}=\operatorname{Tr}/N\). Denote B99's covariant curl by \(D\). Let \(\Psi\) be its fixed nonlinear constraint chart, whose quadratic jet is (3.127), p.421. Its tangent space and the two comparison forms are

\[
 \mathcal T=\{A:QA=0,\ RD^*A=0\},\qquad
 q(A)=\|DA\|_2^2,\qquad P(A)=h^{-2}\|A\|_2^2.
 \tag{R1.4; P: definitions}
\]

There are six positively ordered planes \(I=(\mu,\nu)\), \(\mu<\nu\). Let \(F_I(x)\) be exactly the anti-Hermitian traceless clover in P2, equivalently one quarter of the sum of the four traceless anti-Hermitian parts of its oriented plaquette matrices. For a real symmetric six-by-six matrix field \(J_{IJ}(x)\), define

\[
 \mathcal Q_J^\eta(U)=
 \sum_x\eta^{d-4}\sum_{I,J}J_{IJ}(x)
        \operatorname{Re}\operatorname{tr}(F_I(x)F_J(x)),
 \qquad
 \|J\|_\infty=\sup_x\sum_{I,J}|J_{IJ}(x)|.
 \tag{R1.5; P: definition}
\]

The space of real symmetric matrices here has dimension 21. With P2's sum over all ordered values of \(\mu,\nu,\rho,\sigma\), antisymmetry in each pair gives the exact conversion

\[
 J_{(\mu,\nu),(\rho,\sigma)}=4N j^{\mu\nu\rho\sigma},
 \qquad \mu<\nu,\quad\rho<\sigma.
 \tag{R1.5a; P}
\]

The factor four comes from the two orderings of each antisymmetric pair, and \(N\) from normalized trace. The sum in (R1.5) runs over all six-by-six entries, so its off-diagonal terms are already counted in both orders; there is no further factor two. The scalar Wilson source in these same conventions has weight \(Nj^{(0)}\), while the bare normalized Wilson coefficient is \(X_{B,0}=2N^2x_0\). No source coefficient is silently identified with a differently normalized action coefficient.

Define \(\mathcal H_W=D^2(A_1^\eta\circ\Psi)(0)\), where \(A_1^\eta=\sum_p\eta^{d-4}(1-\operatorname{Re}\operatorname{tr}P_p)\), and define \(\mathcal H_J=D^2(\mathcal Q_J^\eta\circ\Psi)(0)\).

### Theorem 2.1. Fixed-background full tensor quadratic admission — P

Under precisely the hypotheses above, constants \(c,C>0\), independent of \(\eta,h\), lattice volume and the bounded field \(J\), satisfy

\[
 \mathcal H_W(A)\ge ch^{-2}\|A\|_2^2,
 \qquad q(A)+P(A)\le C\mathcal H_W(A),
 \qquad |\mathcal H_J(A)|\le C\|J\|_\infty\mathcal H_W(A),
 \quad A\in\mathcal T.
 \tag{R1.6; P}
\]

No derivative of \(J\) is required. Consequently, for real \(J\) and \(X>C\|J\|_\infty\),

\[
 (X-C\|J\|_\infty)\mathcal H_W
 \le X\mathcal H_W-\mathcal H_J
 \le (X+C\|J\|_\infty)\mathcal H_W.
 \tag{R1.7; P}
\]

The theorem concerns the same fixed background and the same chart on both sides. It makes no assertion that a sourced minimum satisfies those hypotheses.

### 2.2 The untraced plaquette derivative

Write a positively oriented plaquette as \(P=U_1U_2U_3^{-1}U_4^{-1}\), with \(A_i\) attached to the four positive links in this expression. B99 (3.4), p.391, gives

\[
 \eta DA(p)=A_1+\operatorname{Ad}_{U_1}A_2
                 -\operatorname{Ad}_{U_4}A_3-A_4.
 \tag{R1.8; L: B99 (3.4), p.391, in this plaquette notation}
\]

Directly differentiating the four matrix factors, including the inverse-link derivatives, gives its actual left logarithmic velocity

\[
 \begin{aligned}
 K_p:=P'(0)P^{-1}
 &=i\eta\{A_1+\operatorname{Ad}_{U_1}A_2
      -\operatorname{Ad}_{P}(\operatorname{Ad}_{U_4}A_3+A_4)\}\\
 &=i\eta^2DA(p)
   +i\eta(I-\operatorname{Ad}_P)
                   (\operatorname{Ad}_{U_4}A_3+A_4).
 \end{aligned}
 \tag{R1.9; P}
\]

This is an identity, with no small-field expansion. By (R1.3) the second term has norm at most \(C\varepsilon\eta^3h^{-2}(|A_3|+|A_4|)\). Cyclically changing the plaquette base point conjugates by a path of at most three links. Differentiating that conjugation adds a commutator of the path velocity with \(P\); it too is bounded by curvature times \(C\eta\sum|A_b|\). Reversing the plaquette uses the derivative of its inverse and has the same estimate. Therefore all four plaquettes in a clover have the same principal-curl-plus-small-remainder decomposition.

Let \(\mathcal P_x\) and \(\mathcal B_x\) be fixed finite sets of plaquettes and bonds containing the clover and the short base-point paths. Their overlap multiplicities are absolute lattice constants. Matrix multiplication, the traceless skew projection and (R1.9) imply

\[
 \begin{aligned}
 |F_I(x)|&\le C\varepsilon\eta^2h^{-2},\\
 |DF_I(x)[A]|&\le C\eta^2\sum_{p\in\mathcal P_x}|DA(p)|
             +C\varepsilon\eta^3h^{-2}\sum_{b\in\mathcal B_x}|A_b|,\\
 |D^2F_I(x)[A,A]|&\le C\eta^2\sum_{b\in\mathcal B_x}|A_b|^2.
 \end{aligned}
 \tag{R1.10; P}
\]

For the last bound, expand the derivative of each product of four link matrices. Every second derivative contains either \(\eta^2A_b^2\) or \(\eta^2A_bA_{b'}\), with unitary factors of norm one. The finite sum is bounded by the displayed expression using \(2|A_b||A_{b'}|\le|A_b|^2+|A_{b'}|^2\). This argument also covers the finitely many additional factors in a base-point conjugation. It does not require a small second derivative of the clover itself.

### 2.3 Ambient tensor Hessian and its force

Differentiate (R1.5) twice. The products of first derivatives are bounded by the square of the second line of (R1.10). The products of an undifferentiated clover and its second derivative are bounded by its first and third lines. Summing with \(\eta^{d-4}\), using bounded overlap and \(\eta\le h\), gives

\[
 |D^2\mathcal Q_J^\eta(U)[A,A]|
 \le C\|J\|_\infty\{q(A)+\varepsilon P(A)\}.
 \tag{R1.11; P}
\]

For example, the product of two principal first derivatives contributes \(\eta^{d-4}\eta^4|DA|^2\), which is exactly the fine \(L^2\) curl form. The square of the small first-variation error contributes at most \(C\varepsilon^2\eta^2h^{-4}\|A\|_2^2\le C\varepsilon^2P(A)\). A clover times a second derivative contributes \(C\varepsilon h^{-2}\|A\|_2^2\). These are the three scale counts needed in (R1.11).

Let \(J_Q\) denote the fine-link first-variation force, so that \(D\mathcal Q_J^\eta(U)[A]=\langle A,J_Q\rangle\). The **exact linear decomposition** of the first derivative used in (R1.10), followed by adjunction of its principal curl, gives

\[
 J_Q=D^*B_J+R_J,\qquad
 \|B_J\|_\infty\le C\|J\|_\infty\varepsilon h^{-2},\qquad
 \|R_J\|_\infty\le C\|J\|_\infty\varepsilon^2\eta h^{-4}.
 \tag{R1.12; P}
\]

Here \(B_J\) is obtained by collecting, for each plaquette, all terms linear in its \(DA(p)\) from the finitely many clovers containing it. The short unitary transports enter its coefficients. The other terms define \(R_J\). The factors \(\eta^{-4}\), \(\varepsilon\eta^2h^{-2}\), and \(\eta^2\) give the first bound; replacing the last factor by \(\varepsilon\eta^3h^{-2}\) gives the second. This construction is valid for rough bounded \(J\). In particular no difference operator is applied to \(J\); moving \(D\) to the lifting below is essential.

### 2.4 The nonlinear constraint contribution

Use the normalized lift \(H\) for \(QA=B\). With the fine and coarse scalar products, B99 (3.133), p.422, implies

\[
 \|H^*\|_{\infty\to\infty}\le C,
 \qquad\|(DH)^*\|_{\infty\to\infty}\le Ch^{-1}.
 \tag{R1.13; P from L: B99 (3.133), p.422}
\]

Indeed, its kernels have sizes \(Ch^{-d}\) and \(Ch^{-d-1}\), respectively, with exponential block-distance decay. Summing against fine volume \(\eta^d\) gives (R1.13), because one block contributes \(O(h^d)\) and the exponential sum over blocks is bounded uniformly in volume. The paragraph following (3.133) distinguishes this normalized lift from the lift for \(hQA=B\). We use the corresponding quadratic-constraint convention \(C^{(2)}=hC_j^{(2)}\), printed on p.421.

For clarity, the second kernel is the curl of the lift in its fine argument. It is bounded by a fixed sum of the covariant first-derivative kernels in (3.133). Equivalently, in a regular local gauge the ordinary first-derivative bound and \(|A_{\rm bg}|\le C\varepsilon/h\) bound the covariant derivative, and hence \(DH\), by \(Ch^{-d-1}\). This conversion occurs before taking the adjoint and summing; no derivative of the tensor source is introduced.

Equations (R1.12)–(R1.13) and \(\eta\le h\) yield

\[
 \|H^*J_Q\|_\infty
 \le \|(DH)^*B_J\|_\infty+\|H^*R_J\|_\infty
 \le C\|J\|_\infty\varepsilon h^{-3}.
 \tag{R1.14; P}
\]

B99 (3.127) fixes the second jet of the nonlinear averaging chart. Applying the ordinary second-derivative chain rule to the new action gives the exact identity

\[
 \mathcal H_J(A)=D^2\mathcal Q_J^\eta(U)[A,A]
                   -2\langle C^{(2)}(A),H^*J_Q\rangle.
 \tag{R1.15; P using L: B99 (3.127), p.421}
\]

The calculation (3.136)–(3.137), pp.422–423, is linear in the coefficient \(H^*J\). It uses only its supremum bound of order \(\varepsilon h^{-3}\) at this step. Substituting (R1.14) gives a pointwise local operator bound of order \(C\|J\|_\infty\varepsilon h^{-2}\). Because it holds for every input, it bounds the row absolute sums of that operator's kernel. The quadratic form is real symmetric, so the column sums have the same bound. The Schur test therefore gives

\[
 |2\langle C^{(2)}(A),H^*J_Q\rangle|
 \le C\|J\|_\infty\varepsilon P(A).
 \tag{R1.16; P from the checked L calculation}
\]

No fine-bond count is inserted into this Schur bound. Its use of (3.136)–(3.137) imports that printed nonlinear-averaging estimate, including its admitted geometry; it is not an estimate for a different sourced chart.

### 2.5 Comparison with the source-free Wilson form

B99 Theorem 3.11, p.416, gives positivity of the source-free operators. Theorem 3.12, p.423, extends those positivity and propagator conclusions to \(G_1\), under both (3.35) and (3.36), with the stated exception concerning a covariant-Laplacian estimate. Its local \(L^2\) bound (3.46), p.398, gives a block kernel bound \(\|P_yG_1P_z\|_{2\to2}\le Ch^2e^{-c d(y,z)}\). The block Schur test yields \(\|G_1\|_{2\to2}\le Ch^2\). In (3.128), p.421, the gauge and averaging penalty terms vanish on \(\mathcal T\); consequently

\[
 \mathcal H_W(A)=\langle A,G_1^{-1}A\rangle\ge cP(A).
 \tag{R1.17; P from the specified L inputs}
\]

The ambient Wilson curvature terms are displayed in B99 (3.10), p.392. Their norms, together with the same chart correction, imply

\[
 |\mathcal H_W(A)-q(A)|\le C\varepsilon\{q(A)+P(A)\}.
 \tag{R1.18; P}
\]

For sufficiently small \(\varepsilon\), (R1.17) absorbs the last term and yields \(q+P\le C\mathcal H_W\). Combining this with (R1.11), (R1.15), and (R1.16) proves (R1.6). Linearity in \(J\) proves (R1.7). ∎

The excluded covariant-Laplacian estimate in Theorem 3.12 is not used. In particular, this proof cannot be reused without additional work to claim the regularity of a newly displaced minimum. It also has only one averaging scale, so it does not establish a Schur estimate with changing layer weights in a complete nested history.

## 3. Gaussian consequences, with the actual coordinate count retained

Let \(H\) be the positive matrix representing \(\mathcal H_W\) on the finite-dimensional real tangent space \(\mathcal T\), with dimension \(D_{\rm fl}\). Let \(H_J\) represent \(\mathcal H_J\). Complexify by linear extension in \(J\), and increase the fixed constant in Theorem 2.1 if necessary. Then

\[
 B_J=H^{-1/2}H_JH^{-1/2},\qquad
 \|B_J\|\le C\|J\|_\infty.
 \tag{R1.19; P}
\]

The bound for complex \(J\) follows by splitting it into real and imaginary parts and polarizing the real symmetric form. It is a relative **energy operator** bound; it is not a localized random-walk norm bound.

### Corollary 3.1. Holomorphic inverse and determinant jets — P

For \(X>0\) and \(C\|J\|_\infty<X\), the quadratic covariance and the Gaussian log ratio exist with their branch fixed at \(J=0\), and

\[
 \begin{aligned}
 (XH-H_J)^{-1}
   &=X^{-1}H^{-1/2}(I-X^{-1}B_J)^{-1}H^{-1/2},\\
 \|(I-X^{-1}B_J)^{-1}\|
   &\le(1-C\|J\|_\infty/X)^{-1},\\
 F_X(J)&=-\tfrac12\operatorname{Tr}\log(I-X^{-1}B_J).
 \end{aligned}
 \tag{R1.20; P}
\]

The Neumann series and the log series converge normally on each smaller ball. For every \(m\ge1\),

\[
 |D^m F_X(0)[J_1,\ldots,J_m]|
 \le \frac{D_{\rm fl}}2(m-1)!\left(\frac C X\right)^m
                                      \prod_{i=1}^m\|J_i\|_\infty.
 \tag{R1.21; P}
\]

**Proof.** Use (R1.19) in the Neumann series. The degree-\(m\) term of the log series is \((2m)^{-1}X^{-m}\operatorname{Tr}(B_J^m)\). Its multilinear derivative contains \(m!\) ordered products. Each trace has absolute value at most \(D_{\rm fl}\prod_i\|B_{J_i}\|\); division by \(2m\) gives (R1.21). This argument does not assume that the matrices for distinct directions commute. ∎

The Gaussian coordinate factor in this estimate is \(D_{\rm fl}\), not \(N_T\). On a long fine lattice those counts differ substantially. Localizing this trace, subtracting its source-dependent local vacuum, and comparing it across geometries require further estimates. Neither (R1.21) nor the source-free Gaussian assertion (R1.2) supplies those sourced estimates automatically.

### Corollary 3.2. One-scale source-force cost — P

Let \(V=\sum_x\eta^4\) denote the physical four-volume of the one-scale core, enlarged by the fixed-width collars used above. Restrict the force \(J_Q\) to \(\mathcal T\). Then

\[
 \|H^{-1/2}J_Q\|_2
       \le C\|J\|_\infty\varepsilon h^{-2}V^{1/2}.
 \tag{R1.22; P}
\]

**Proof.** Pair (R1.12) with \(A\in\mathcal T\), moving the curl onto \(A\). The coefficient bounds and Cauchy–Schwarz give

\[
 \begin{aligned}
 |\langle A,J_Q\rangle|
 &\le C\|J\|_\infty V^{1/2}
     \{\varepsilon h^{-2}q(A)^{1/2}
               +\varepsilon^2\eta h^{-4}\|A\|_2\}\\
 &\le C\|J\|_\infty\varepsilon h^{-2}V^{1/2}
                           \mathcal H_W(A)^{1/2},
 \end{aligned}
 \tag{R1.23; P}
\]

where \(\eta\le h\), \(\varepsilon\le1\), and (R1.6) were used. The dual energy norm identity gives (R1.22). ∎

For a **centered** real Gaussian with perturbed quadratic form obeying \(C\|J\|_\infty\le X/2\), adding the linear source force and completing the square gives

\[
 \tfrac12\langle J_Q,(XH-H_J)^{-1}J_Q\rangle
    \le C\|J\|_\infty^2\varepsilon^2X^{-1}Vh^{-4}.
 \tag{R1.24; P}
\]

This controls the added source-force square without constructing a displaced minimizing field. At a noncritical background with a pre-existing Wilson linear force, the full logarithm also contains its cross term with \(J_Q\); (R1.24) does not include or bound that cross term. Its root count is the number of scale-\(h\) blocks, \(Vh^{-4}\). Controlling the ultraviolet sum with the required physical source weights is a separate issue. A one-scale square completion does not identify or bound the nonlinear old source readout after a later R reset.

## 4. The exact post-regular marked state and the unproved transition

### 4.1 A finite-cutoff definition independent of any hoped-for estimate

Fix the real source-zero construction, its cutoffs, selector branches, gauges, reference kernels and all coordinate maps. Insert the actual scalar/clover source in the original action and carry it through these same operations. All these operations are finite-dimensional at fixed cutoff. Keeping auxiliary labels until their last compulsory integration makes their complete flag sum a positive integral-preserving operation. Regular Gaussian integrations and their non-Gaussian weights are performed at the stages prescribed by the construction. This describes an exact finite-cutoff family without asserting any uniform marked norm.

Let \(v\) denote the variables still explicit at stage \(k\): current links, the nested domains and selector flags, and the old links or fluctuation coordinates not yet integrated. Let \(\mathcal K_k(dv\mid U)\) be the **actual frozen composite positive kernel** obtained from the construction, with every remaining compulsory factor retained. In particular it is not the normalized kernel obtained by deleting a rare component mass. For a bare source direction \(f\), write \(V_f(U)\) for its literal Wilson/clover insertion in P2. Then

\[
 M_k[j](dv)=\int\mathcal K_k(dv\mid U)
       \exp(V_j(U))\exp(-S_a[0](U))\,d\mathrm{Haar}(U).
 \tag{R1.25; P: exact finite-cutoff definition}
\]

This definition uses the original source observable. It does not replace it by a source evaluated on the newly drawn R-reference field. It also does not claim that the nonlinear source-free selector maps become holomorphic functions of all fields. Their real branch indicators remain part of the underlying measure. Because they are frozen in \(j\), differentiating (R1.25) in the source does not differentiate those indicators.

Suppose the prescribed local vacuum recipe has been applied through stage \(k\), as a finite formal two-jet, with derivatives \(c_{k,f}\) and \(c_{k,fg}\). These are the identity coefficients actually extracted during that finite construction. They are not chosen to equal \(\log Z[j]\). The renormalized raw first and second derivative measures are exactly

\[
 \begin{aligned}
 M^{\rm ren}_{k,f}
   &=\mathcal K_k(V_f e^{-S_0}d\mathrm{Haar})-c_{k,f}M_k[0],\\
 M^{\rm ren}_{k,fg}
   &=\mathcal K_k(V_fV_g e^{-S_0}d\mathrm{Haar})
     -c_{k,f}\mathcal K_k(V_g e^{-S_0}d\mathrm{Haar})
     -c_{k,g}\mathcal K_k(V_f e^{-S_0}d\mathrm{Haar})\\
   &\hspace{1em}+(c_{k,f}c_{k,g}-c_{k,fg})M_k[0].
 \end{aligned}
 \tag{R1.26; P}
\]

The identities follow by differentiating \(e^{-C_k[j]}M_k[j]\). They define the exact kernels that a claimed R1 norm must control. Finite-cutoff existence of these derivatives is immediate from compactness of the original link space. Uniformity and a local analytic decomposition are the hard assertions.

### 4.2 Required record for each carried source atom

An admitted decomposition of (R1.26) must attach the following record to **each** connected analytic source atom or still-explicit raw source factor. An atom without such a record is not assigned norm zero: it is unclassified, and the proposed complete norm below is infinite.

| Field in the record | Required literal information |
|---|---|
| Identity and birth | A persistent atom identifier, its creation scale \(b\), its scalar/tensor type, and its one or two source labels. Birth is when the activity or raw factor is actually created, not the scale to which it is later copied. |
| Retained readout | The exact variables on which it is evaluated: current background, an old link, an old fluctuation, or a named composition of reconstruction maps. If an R replacement draws a fresh variable, the old physical readout is retained or integrated by its actual old kernel. |
| Carrier and endpoints | Its localization \(X\), anchor, the layer of every determining endpoint, and its carrier enlarged by all short transports, source sites and boundary collars. A fine outer endpoint cannot be counted as a single old unit-lattice endpoint. |
| Analytic domain | The actual B109/B119/LFR complex domain for its determining variables, the inner domain used for estimates, and the positive margin to the boundary. For a raw real factor, record its real support instead; no imaginary extension is claimed. |
| Projection ledger | The identity and the complete dimension-four curvature-pair coefficients extracted from that atom, including their signs and the scale at which they are added to the global vacuum or running coefficients. |
| Physical source scale | The generation length \(\ell_b\), the source positions in its carrier, and the scaled source seminorms \(\sum_{|\alpha|\le5}\ell_b^{|\alpha|}\|\partial^\alpha f\|_\infty\). Any Taylor remainder retains its actual source displacement, measured in this scale. |
| Owner | Either an ordinary regular anchor, or one specified historical geometry/energy record \((h,Z_h,\mathrm{type})\). Its capacity is \(M^4R_h^5d'_h(Z_h)\), in the notation of the LFR-II count. The multiplicity with which the capacity is charged must be bounded. |
| Transition history | Which actual regular integration, retained R, erased R, recent R, reconstruction or boundary localization created the present expression. This history fixes the kernel and excludes replacing it by a more favorable reference expectation. |

The owner is an accounting assignment to be proved. A source mark is not paid by a large-field record merely because its carrier is near some bad block at a later scale. Its actual old variables and the scale of its support must be covered by that record with controlled multiplicity.

### 4.3 One explicit sufficient norm

Here is a precise way to make a two-jet admission claim reviewable. It is a sufficient target, not a theorem that this particular strong norm must be finite.

For a regular or boundary analytic atom \(A_{b,X}^{(m)}\), \(m=1,2\), choose the actual inner/outer domain and normalized local cochain coordinates specified in its record. Normalize each determining coordinate by **its own layer radius**, and retain that layer's integration or counting measure. Define its endpoint seminorm to be the sum of absolute multilinear derivative kernels of orders zero through five, with the fifth polynomial moment of all endpoint distances from the anchor. The summation is over actual endpoints and their specified layer measures. If the kernel has not been reduced to old unit-lattice endpoints by a proved chain rule, it is summed on the original fine layer. Denote this completely specified seminorm by \(|A|_{b,X,5}\). Take the supremum over the inner complex domain and source directions of scaled \(C^5\) norm at most one. Finally use the rooted polymer norm

\[
 \|A^{(m)}\|_{\rm an}
  =\sup_b\sup_{\Delta\text{ a }b\text{-block}}
       \sum_{X\ni\Delta}e^{\kappa' d_b(X)}
          \sup_{\|f_i\|_{b,5}\le1}|A_{b,X}^{(m)}[f_1,\ldots,f_m]|_{b,X,5},
 \quad 0<\kappa'<\kappa.
 \tag{R1.27; P: definition}
\]

The endpoint norm includes the zeroth derivative; hence a small Taylor remainder cannot hide an uncontrolled outer-domain supremum. Covariant derivatives or overlapping charts are compared using the explicit transition functions recorded with the atom. Their norm bounds are part of admission.

More explicitly, an endpoint index \(\xi\) records its layer, bond or site, determining-variable type, and one element of a fixed Lie-algebra basis. Write \(\mu_\xi\) for the layer measure in units of \(\ell_b\), and use coordinates normalized by the recorded layer radius. Define derivative kernels by

\[
 D^nA(z)[a_1,\ldots,a_n]
 =\sum_{\xi_1,\ldots,\xi_n}
   \left(\prod_i\mu_{\xi_i}\right)
   K_{A,n}(z;\xi_1,\ldots,\xi_n)
   \prod_i a_i(\xi_i).
 \tag{R1.27a; P: definition}
\]

The endpoint seminorm used in (R1.27) is

\[
 |A|_{b,X,5}
 =\sup_{z\in\mathfrak D^-_{b,X}}
    \sum_{n=0}^{5}\frac1{n!}
    \sum_{\xi_1,\ldots,\xi_n}
       \left(\prod_i\mu_{\xi_i}\right)
       \bigl(1+\operatorname{diam}_b(X\cup\{x_{\xi_i}\})\bigr)^5
       |K_{A,n}(z;\xi_1,\ldots,\xi_n)|.
 \tag{R1.27b; P: definition}
\]

For \(n=0\), the inner sum means \((1+\operatorname{diam}_bX)^5|A(z)|\). All source sites already belong to the recorded carrier \(X\), so they are included in this moment. One may replace the diameter by a larger explicit rooted tree moment; doing so changes the chosen sufficient norm and must be stated. The formula makes the layer measures, fine endpoint counts and radius normalization directly checkable.

For a still-explicit real raw factor with base kernel \(\sigma_a^0(d\zeta\mid v)\), retain its signed first/second derivative kernels \(\sigma_a^{(m)}\). For a nonnegative assigned capacity \(w_a(f_1,\ldots,f_m)\), define the raw seminorm by the **measure inequality**, on every allowed real exterior,

\[
 |\sigma_a^{(m)}|(d\zeta\mid v)
       \le C_a\,w_a(f_1,\ldots,f_m)^m\sigma_a^0(d\zeta\mid v),
 \qquad m=1,2.
 \tag{R1.28; P: definition of the admissible constant }C_a
\]

When separate capacities are used for separate directions, replace \(w_a^m\) by their product. The capacity contains the actual source supremum on that raw carrier and its assigned historical count. The sum of capacities must obey a once-owned budget

\[
 \sum_a w_a(f)\le C\|f\|_{C^5}
       \left(N_T+\sum_{(h,Z_h)\text{ owned}}M^4R_h^5d'_h(Z_h)\right),
 \tag{R1.29; O: required ownership estimate}
\]

or an explicitly stronger localized version for a cell-supported \(f\). Equation (R1.28) retains the base mass on both sides. No factor \(1/\sigma_a^0 1\) is dropped. A raw factor that fails (R1.28) can instead be admitted by a separately proved averaged norm; that would require a stated change to this sufficient criterion, not a claim that (R1.28) has been verified.

Define the complete two-jet norm as the infimum, over decompositions that reproduce the **actual** measures (R1.26) and carry all the records above, of the sum of the analytic norm (R1.27), the raw constants in (R1.28) with their rooted sums, and the smallest ownership constant in (R1.29). A decomposition missing a domain, a readout, a projection or an owner is inadmissible. The infimum over an empty class is infinity. This definition gives a literal mathematical target without presuming a favorable decomposition exists.

The known regular extraction estimates control (R1.27) **after** its incoming domain, endpoint and scaled-source hypotheses have been verified. The raw energy reserve controls explicit primitives satisfying (R1.28) **after** their owners have been verified. Neither statement fills an unclassified record.

### 4.4 Exact transition rules and the first unknown kernel

| Transition | Exact source rule | What is established / what is still required |
|---|---|---|
| Regular T integration | Add the fresh source insertion to all inherited marked activities evaluated on the actual reconstructed fluctuation; integrate with the fixed regular kernel; take the connected local logarithm; extract its identity and full dimension-four jet. | The universal regular map acts on admitted old E inputs. The mixed old R/B and spatial-source inputs need admission in (R1.27). |
| Retained R branch | Keep its old variable and its original readout; multiply by the selected source-zero branch factor. | Exact transport is immediate. The owner must cover that old readout and every attached boundary mark. |
| Erased R branch | Integrate the old marked kernel, then attach the normalized fresh reference. Its source remains the old conditional integral. | The identities below are exact. The resulting exterior-dependent mean is not a scalar vacuum unless extraction proves it is. |
| Recent R activity | The difference between the actual local regular calculation and its whole-domain counterpart remains a recent-R activity with the original source slots. | Source-free recent-R smallness exists. Its marked analytic carrier norm, including old inputs, remains unproved. |
| Boundary localization | Apply the published interpolation/localization map to the entire marked atom, including its readout, carrier, constraints and raw masses. | It is bounded on an admitted source Banach space. The images of all historical raw atoms have not been shown to lie in one such space. |
| Nonlinear reconstruction or selector | Compose the readout with the actual source-zero reconstruction; retain the real branch indicator in the raw measure. | Source differentiation creates no moving-selector term when the selector is frozen. Layerwise analytic margins and endpoint bounds of inherited atoms on mixed images are still required. |

The smallest concrete erased-R expression already displays the difficulty. Let \(v\) be its exterior, \(\sigma_v(d\zeta)\) its **actual old positive conditional measure**, including all non-source factors, and \(q_v(du)\) its normalized new reference. After the designated regular integrations let the still-carried source logarithm have jet \(A_f(v,\zeta),A_{fg}(v,\zeta)\). The source-zero mass and the raw jets after erasure are

\[
 \begin{aligned}
 R_0(v,du)&=q_v(du)\int\sigma_v(d\zeta),\\
 R_f(v,du)&=q_v(du)\int\sigma_v(d\zeta)A_f(v,\zeta),\\
 R_{fg}(v,du)&=q_v(du)\int\sigma_v(d\zeta)
                  \{A_{fg}(v,\zeta)+A_f(v,\zeta)A_g(v,\zeta)\}.
 \end{aligned}
 \tag{R1.30; P: exact erased-R jets}
\]

At a real exterior with nonzero old mass, taking the logarithm of this factor gives the conditional mean of \(A_f\), and the conditional mean of \(A_{fg}\) plus the conditional covariance of \(A_f,A_g\). This identity does not bound those quantities. It retains all exterior dependence of the old kernel. On a complex exterior, the continued kernel need not be positive and the denominator must be controlled on the actual domain before that normalized logarithm may be used.

**Open estimate O–MR1.** For the actual incoming \(A_f,A_{fg}\) produced by all prior regular integrations, decompose (R1.30), with its retained and boundary companion branches, into (a) identity/dimension-four projections entered into the prescribed ledger, (b) analytic atoms in (R1.27), and (c) raw atoms in (R1.28), with (R1.29), uniformly in every admissible exterior, depth and history. The same assertion is required for the recent-R difference. The source-zero LFR quotient estimate and the old reference normalization do not prove it, because they contain neither these old physical readouts nor their field/source endpoint norms.

This is an actual kernel estimate, not a request for an additional theorem about an arbitrarily chosen comparison measure. In particular, replacing \(A_f(v,\zeta)\) by a source on the fresh reference variable \(u\), or replacing \(\sigma_v\) by a convenient Gaussian, changes (R1.30) and is not a proof of O–MR1.

## 5. A two-jet closure inequality with the unknown term isolated

### 5.1 Correct stage for the raw norm

The post-integration convention must be stated more strongly than “integrate some small fields.” Completed regular connected activities **and completed erased-R connected activities** stay integrated. Their extracted vacuum terms belong to the vacuum ledger, and their remaining source dependence belongs to the corresponding analytic E/R/B activity. They are not reopened as independent raw fine-field marks merely to apply a positive count bound.

The raw part of (R1.28)–(R1.29) is therefore reserved for genuinely still-explicit old variables and compulsory surviving integrations. An erased-R branch may appear as the input of (R1.30) while that transition is being analyzed. After its connected vacuum and local terms have been extracted, its residual is an effective activity unless it is still part of an explicitly retained mandatory kernel. Reopening every completed fine erased component would produce a number of possible roots of order the fine volume. A small per-root tilt need not then have a bounded physical-volume sum. This is the same ultraviolet counting issue that the vacuum extraction is designed to resolve.

This staging also explains why the flat-field obstruction in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md), §3, is relevant. The source-dependent vacuum can be ultraviolet extensive while the literal original source vanishes on flat fields. Thus the desired norm cannot be a pointwise bound for the fully unreduced original source minus that vacuum on every original configuration. The exact physical measure remains (R1.25); only its legitimate post-integration representation is being estimated.

### 5.2 Known regular forcing, with its admission conditions retained

For the constant-scalar regular family, use the notation

\[
 \theta_k=A g_k(\log g_k^{-2})^p,\qquad
 h_k=\theta_kg_k^2,\qquad f_k=\theta_kg_k^4,\qquad q_k=C\theta_k.
 \tag{R1.31; P: definitions}
\]

Let \(u_k\) and \(v_k\) be the first and second derivative of the actual consistently normalized Wilson coefficient in a coherent constant-source direction. Let \(a_k,b_k\) be the maximum first/second norm of its incoming universal regular E family. The regular-map calculation in §§4.25–4.26 of [Regular jet transport, pressure and coupling windows](regular_jets.md) gives

\[
 \begin{aligned}
 a_{k+1}^{\rm fresh}
   &\le Ch_k|u_k|+q_ka_k,\\
 b_{k+1}^{\rm fresh}
   &\le C\{f_k|u_k|^2+h_k|v_k|\}
      +Ch_ka_k|u_k|+C\theta_kE_0^{-1}a_k^2+q_kb_k.
 \end{aligned}
 \tag{R1.32; C on the actual running-coordinate dictionary R0-reg}
\]

Here all old E derivatives are included. The proof is the chain rule for the admitted regular map \(\Psi(g,H)\), using \(g'=-g^3u/2\), \(g''=3g^5u^2/4-g^3v/2\), and the fixed-domain bounds \(\Psi_g=O(\theta/g)\), \(\Psi_{gg}=O(\theta/g^2)\), \(D_H\Psi=O(\theta)\), \(D_H\Psi_g=O(\theta/g)\), \(D_H^2\Psi=O(\theta/E_0)\). This gives exactly the five terms on the second line. The unsourced Gaussian family in this calculation is the checked L input (R1.2).

No use of N2-F alone identifies \(u_k,v_k\) with derivatives of a physical source family. That identification is R0-reg. Under its positive-drift condition, \(\sum_k h_k\) and \(\sum_k f_k\) converge uniformly in the ultraviolet depth: write \(X_k=g_k^{-2}\ge X_K+d(K-k)\), compare with the integrals of \(x^{-3/2}(\log x)^p\) and \(x^{-5/2}(\log x)^p\), and use their finite tails.

There are also known **operators**, conditional on incoming regular-image admission, for nonconstant-source irrelevant memory and freezing. If \(a_{b,m}\) is the admitted generation-\(b\) marked amplitude, \(\rho_b\) its actual field radius, and \(\delta_k\) the admitted interpolation displacement divided by the current radius, their rooted contributions are bounded by

\[
 \begin{aligned}
 S_{k,m}^{\rm irr}
 &\le C\delta_k\sum_{b\le k}L^{-\alpha(k-b)}
             \sum_{n=3}^{6}(\rho_k/\rho_b)^n a_{b,m},\\
 S_{k,m}^{\rm var}(f_1,\ldots,f_m)
 &\le C\sum_{b\le k}\frac{\ell_b}{\ell_0}
             \sum_{n=2}^{5}(\rho_k/\rho_b)^n a_{b,m}
       \sum_iD_{5,\ell_0}(f_i)
                 \prod_{\ell\ne i}\|f_\ell\|_{C^5,\ell_0}.
 \end{aligned}
 \tag{R1.33; C on the displayed regular-image and generation-source admission}
\]

The second line is the contribution after old-anchor counting at the current root: the field factor \(L^{-4(k-b)}\) cancels the number of old anchors, while \(\ell_b/\ell_0\le L^{-(k-b)}\). The first line has the analogous \(4+\alpha\) field Taylor gain. For \(\rho_b\asymp X_b^{-1/2}(\log X_b)^q\) on a positive-drift trajectory, each radius ratio is at most a fixed polynomial in \(k-b\). A spare exponential absorbs that polynomial. These facts make both age kernels summable. They do not prove the initial marked amplitudes or their mixed-image admission. In particular, one may not replace the generation-scaled source hypothesis by a fixed physical \(C^5\) operator norm without justification.

### 5.3 Definition of the remaining forcing

At a finite cutoff, perform the next **actual** frozen RT transition on the post-integration state. Remove only the following identified pieces, each in its own real branch and with its raw measure factors retained: the universal admitted E-map contribution in (R1.32), the regular-image operators in (R1.33), and the exact copies or positive pushforwards of raw factors already admitted by (R1.28). Their source slots, projections and carrier maps are explicit in the record. Define \(\mathcal U_{k,m}\) to be the infimum of the complete norm of §4.3 over decompositions of the remaining degree-\(m\) kernel, for \(m=1,2\). The infimum is infinity if the residual has no admitted decomposition.

This definition includes, in particular, the residual of the actual expressions (R1.30) after their permitted local projections; the boundary/recent-R localization of those expressions; and all mixed-image source atoms not satisfying the regular admission. It excludes no old physical readout. It does not count a term twice: a known piece is removed only once, in the branch and transition where it was computed.

With \(S_{k,m}=S_{k,m}^{\rm irr}+S_{k,m}^{\rm var}\), the resulting prospective induction has the explicit form

\[
 \begin{aligned}
 A_{k+1}^{(1)}
 &\le Ch_k|u_k|+q_kA_k^{(1)}+S_{k,1}+\mathcal U_{k,1},\\
 A_{k+1}^{(2)}
 &\le C\{f_k|u_k|^2+h_k|v_k|\}
     +Ch_kA_k^{(1)}|u_k|
     +C\theta_kE_0^{-1}(A_k^{(1)})^2
     +q_kA_k^{(2)}+S_{k,2}+\mathcal U_{k,2}.
 \end{aligned}
 \tag{R1.34; C: exact known-piece estimate, with the unknown norm retained}
\]

Here \(A_{k+1}^{(m)}\) denotes the new admitted effective-activity output norm after subtraction of the exact raw copies; existing raw kernels keep their own records and capacities. Thus (R1.34) does not incorrectly assign a strict \(q_k\) contraction to an unintegrated raw source factor. In a nonconstant or tensor marginal direction the corresponding regular marginal forcing must first be identified; the constant-scalar terms on the right of (R1.34) are not asserted to describe that unknown flow.

The first line is a triangle inequality combined with (R1.32)–(R1.33). The second line additionally retains the quadratic product and mixed terms from the chain rule. It is useful precisely because every currently unbounded new source contribution is in the literal, defined quantity \(\mathcal U_{k,m}\). It is not a proof that \(\mathcal U_{k,m}\) is small.

**Open estimate O–MR2.** Prove a contractive or age-summable majorant for these actual \(\mathcal U_{k,1},\mathcal U_{k,2}\), including the raw ownership constant, with the same physical-scale root budget and analytic margins as (R1.27)–(R1.29). For the Wilson projection, prove that the projected residual increments are summable in scale, so that they can enter the \(u_k,v_k\) equations without an ultraviolet-depth loss. For the identity projection, prove its local source Taylor/copying bound before removing it from this norm. A mere uniform bound on \(\mathcal U_{k,m}\) per fine block does not suffice.

There is at present no proved numerical upper bound for O–MR1 or O–MR2 in this note. In particular, the new tensor quadratic bound in §2 does not supply it: it controls an already regular one-scale Gaussian energy, whereas (R1.30) contains inherited effective interactions, old readouts, mandatory masses and the mixed exterior dependence of a complete history.

## 7. What remains, stated as work on concrete objects

1. **O–MR1: old readouts after a real mixed transition.** Evaluate (R1.30) for the inherited source functions produced by the previous actual integrations. Keep their dependence on the physical exterior and on every old variable. Supply a domain and carrier record for each resulting analytic atom, or a once-owned capacity for each remaining raw atom. The most informative next calculation is one complete regular-plus-erased-R transition with a specified old source atom, including its boundary terms; a new abstract cumulant identity would not do this.

2. **O–MR2: the uniform complete two-jet bound.** Prove a uniform contractive/age-summable estimate for the literal residual \(\mathcal U_{k,m}\) defined in §5.3. Pay the physical source root count at each birth scale, rather than a fine-block count summed over all ultraviolet generations. Carry every identity and tensor projection into its own coefficient ledger. The required Wilson projection must have a summable influence on the actual coefficient flow.

3. **O: source-dependent Gaussian localization where it is actually needed.** Theorem 2.1 proves an energy-norm perturbation estimate at a real one-scale background. It does not show the localized inverse, determinant, complex reconstruction or mixed-scale derivative bounds required by the full source norm. These must either be proved for a sourced Gaussian operator, or avoided by a rigorously closed expansion about the fixed source-free Gaussian family. In the latter route the non-Gaussian incoming marked norm still has to be established.

4. **O: full tensor marginal transport.** There are 21 independent curvature-pair source components. Their complete local coefficient flow, normalization, collision terms and all-order growth are not determined by Theorem 2.1. Positivity of a quadratic form says nothing by itself about the ultraviolet product of its renormalization matrices. This is the R3 issue, treated in [Tensor channels, scalar derivatives and contact regularity](regular_tensor_channels.md) rather than absorbed into R1 by terminology.

5. **O: source-local vacuum and normalization of survivors.** Completing R1 supplies analytic source transport, but the full existence program still needs the source-local vacuum comparison, the correct full-history normalization, and the remaining OS/continuum/nontriviality requirements listed in [Lattice conventions and hypotheses](../lattice_conventions.md), §5. The exact one-link SU(2) integration in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md), §4, is a real initial example of a predictable exterior source remaining as a local loop interaction after flat-source subtraction; it does not iterate unchanged once the effective density contains those new non-Wilson interactions.

No additional interface is requested here. In particular, the unknown mixed-kernel estimate is not moved into a strengthened N2-F. No claim that R1, R2, R3, N1-S or YM-E has been completed follows from this note.
