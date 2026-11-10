# Regular jet transport, pressure and coupling windows

## 4.25 Fixed background domains and complete current-coupling derivatives for the regular E family

This subsection closes the two obligations O–CT-domain and O–CT-derivative of §4.22.3 for the **universal whole-lattice regular E family**, in the corrected cutoff convention of §4.19 and within a sufficiently weak admitted interval. It does not extend arbitrary old R/B activities or nonlinear group selectors. It constructs the regular family from its original datum on a fixed domain; it does not assume that an arbitrary shrinking-domain function has an extension. The additional running-coordinate identification is stated separately in §4.26.

Write `B109` for Bałaban, CMP 109 (1987), 249–301, `B116` for Bałaban, CMP 116 (1988), 1–22, and `B119` for Bałaban, *Convergent renormalization expansions for lattice gauge theories*, CMP 119 (1988), 243–285.

#### 4.25.1 The corrected cutoff, free coordinates, and the old-activity norm

For the fixed positive integer p printed in B119 p.244 and its fixed cutoff constant A, put

\[
 t(g)=\log g^{-2},\qquad R(g)=A t(g)^p,\qquad
 \theta(g)=gR(g),\qquad 0<g<1.
 \tag{4.182; P: definitions}
\]

The raw cutoff is θ; the rescaled free-coordinate cutoff is R. The B119 raw threshold is `δ_k=g_k(A_1/A_0)p_0(g_k)`, hence has exactly this form. There is an explicit correction in the primary-text dictionary: B119 p.267 makes the change `A′=g_k A`, and (3.15), p.268, contains `g_k C A`, but the printed (3.16) bounds the already rescaled A by `δ_k`. Applying the printed bound literally would define a different cutoff. In the consistently rescaled construction the bound is `δ_k/g_k`; LFR I (1.9), p.178, writes that ratio explicitly. This is the raw/rescaled correction proved in §4.19, which is part of the conventions of this paper. The present theorem is not a proof for the uncorrected literal reading of B119 (3.16).

B109 pp.267–268 linearizes the constraint by `B′=B−h D̃(B)`, where h is supported only on the eliminated bonds `b_0(c)`. The remaining variables are free Lie-algebra coordinates B. On the non-eliminated bonds the transformation leaves B unchanged; after the rescaling by g the cutoff is therefore exactly a product of free-coordinate norm balls of radius R(g). The subsequent linear map C restores the linear constraint, and the nonlinear map restores the original block constraint. Neither operation introduces a further moving cutoff on the free coordinates.

In the B119 regular region, p.269 explicitly states that only the small-field characteristic functions from (3.16) remain. On the full regular lattice their product says `|B(b)|<R(g)` for each free bond. Supremum cutoffs over the covering cubes give the same conjunction. External characteristic functions that restrict the final background are factors of the RG density; they are not part of the analytic regular activity that is being extended.

**The activity map and its unprojected input.**

On a fixed finite regular torus, before taking the connected local expansion, the non-Gaussian regular increment has the form

\[
 I_k(g,H;U,J)=
 \int d\mu_{\mathcal C_k(U,J)}(B)\,
 \prod_{b\in F_k}{\bf1}_{\{|B(b)|<R(g)\}}
 \exp V_k(g,H;U,J,B).
 \tag{4.183; L: B109 (2.12)–(2.13), p.268; B119 (3.28), p.272}
\]

Here F_k is the set of free bonds. The covariance is the normalized constrained Gaussian covariance; it depends on the background and the fixed geometry, but not on g when H is held fixed. The interaction contains the exact Wilson remainder, gauge and coordinate Jacobians, and the difference of the entire old **E-family** regular action at the fluctuated and unfluctuated backgrounds. This is the old family defining the universal regular Wilson coefficient. It does not include the R/B terms of the complete density: B119 p.272 uses E_k in the last logarithm of (3.28), while p.279 treats (3.26) separately to obtain R^(k+1). B109 (2.11)–(2.13), pp.267–268, explicitly cancels the apparently singular linear/quadratic terms: the remaining interaction is analytic in gB at g=0 after the displayed powers g⁻² are combined with their cubic-or-higher numerators.

Let Ψ_k(g,H) be the connected localized activity obtained from log I_k. The g-independent normalized Gaussian determinant activity is denoted G_k, so that the full fresh regular activity is `G_k+Ψ_k`. The pure powers of g from the finite-dimensional change of variables give the explicitly separated Gaussian vacuum normalization (terms proportional to the number of free coordinates times log g). They belong to the vacuum-energy ledger, not to H. They are neither omitted from the physical partition function nor claimed to satisfy the bound for Ψ. The old determinant activities, when shifted by the fluctuation, are included in V_k and in the B116 localization estimates; they are not silently removed from the current-g derivative. Their incoming dependence on the bare coupling is zero in this fixed source-free background convention.

The old family H supplied to Ψ_k contains generations 1 through k (the empty family for k=0). It ranges over the Banach space of all such regular activity sequences with norm

\[
 \|H\|_{\kappa,\alpha}
  =\sup_{1\le j\le k}\sup_X e^{\kappa d_j(X)}
       \sup_{(U,J)\in\mathcal U_j^c(X,\alpha_0,\alpha_1)}
           |H_j(X;U,J)|.
 \tag{4.184; P: definition}
\]

The fixed positive radii α are the B109 p.263 radii. Each H_j is the **unprojected fresh regular E activity**. When forming the incoming old action E_k, its vacuum value and Wilson projection are subtracted by the prescribed fixed linear assembly maps. Those assembly maps are included in Ψ and its norm estimates. H_j itself is not the Wilson-subtracted remainder; in particular P H_j need not vanish. Gauge covariance and the other linear symmetry conditions are imposed on this Banach space. The usual fixed reserve in the decay exponent and the enlarged intermediate background domain of B116 (1.34) are retained. A direction may vary every old generation at once; the norm is a maximum, not a sum that would introduce k.

B109 (1.20)–(1.22), p.264, defines the Wilson projection P. On this fixed domain its bound is

\[
 |\mathcal P F|\le C_{\rm mom}\alpha^{-2}
                   \|F\|_{\kappa,\alpha}=:C_P\|F\|_{\kappa,\alpha}.
 \tag{4.185; P: Cauchy and the exponentially summable second spatial moment}
\]

The factor α⁻² is retained. It is harmless for scale summation only because α is now fixed; it is not set equal to a shrinking B119 radius.

#### 4.25.2 Fixed-domain closure for the prescribed logarithmic cutoff — P

**Theorem (P, within the checked B109/B116 regular geometry).** Fix the regular construction constants, the decay reserve and the absolute background radii α. There is a positive coupling threshold γ_c such that, for every finite real sequence `0<g_j≤γ_c`, the regular whole-lattice maps using precisely the cutoffs (4.182) produce formal old and fresh activity iterates on the same fixed domains (4.184). On a sequence satisfying the exact coupling-coefficient recursion, these are the actual regular activities of that RG density. An arbitrary sequence is not asserted to represent the original Wilson density. The constants are independent of the number of generations and the admitted torus volume. For an admitted old family, including on a fixed enlarged ball needed for differentiation,

\[
 \|\Psi_k(g,H)\|_{\kappa,\alpha}
     \le C E_0\theta(g),\qquad \|H\|_{\kappa,\alpha}\le 2E_0.
 \tag{4.186; P}
\]

The regular activities appearing in B119 on its shrinking domains are restrictions of this constructed family, with the same real cutoff and counterterm convention. This does not extend arbitrary additional E/R/B functions that are supplied only on a shrinking domain.

**Proof.** Choose the absolute background radii and the fixed constants α₂, α₄, α₆, M, κ, κ₁ in the order used by B109/B116. Inspection of the relevant inequalities gives two separate requirements on the raw cutoff ε₁. The first is an *upper* smallness requirement: in B116 (1.21)–(1.22), p.7, the inverse contour radius is proportional to `α₂⁻¹ ε₁`; (1.34)–(1.36), p.9, have a background domain independent of ε₁ and an activity bound proportional to ε₁. Equations (2.18), p.16, and (2.28), p.18, retain the fixed inverse factors α₄⁻¹ and α₆⁻¹. There is no requirement that the background radii become smaller as ε₁ becomes smaller.

The second requirement is a *lower* bound on the rescaled cutoff ε₁/g. The tail estimate (2.22), p.16, has a factor `exp[−c(ε₁/g)²|P|]`. The sums (2.31)–(2.34), pp.18–19, require this ratio to be sufficiently large and require its exponential to be smaller than a fixed constant times E₀ε₁. Accordingly it suffices to impose the finite list

\[
 \theta(g)\le \epsilon_*,\qquad
 R(g)^2\ge C_*,\qquad
 e^{-c_*R(g)^2}\le c_{**}E_0\theta(g),
 \qquad 0<g\le\gamma_c.
 \tag{4.187; P: sufficient uniform numerical conditions}
\]

All starred constants here are fixed construction constants. The list has a solution: as g tends to zero, θ(g) tends to zero, R(g) tends to infinity, and

\[
 \frac{e^{-cA^2t^{2p}}}{g t^p}
   =t^{-p}\exp[-cA^2t^{2p}+t/2]\longrightarrow0,
 \qquad t=\log g^{-2},\quad p\ge1.
 \tag{4.188; P}
\]

(The inessential fixed A factor can be absorbed into the constants.) Substitute ε₁=θ(g) throughout the real B116 majorants. The old-generation sum (1.26)–(1.33), pp.8–9, is already performed over the whole old family. It introduces no number-of-generations factor. The localized potential bounds, normalized Gaussian estimates, cutoff-tail sums, connected polymer expansion and final activity bound therefore give (4.186). The exponential decay reserve pays the fixed polynomial carrier and moment factors, exactly as in the original proof.

This substitution does not consume a new background margin at each generation. The input is the original α-domain. The preintegration localization is analytic on the enlarged domain shown in B116 (1.34); the Gaussian/polymer estimates return the same α-domain, as explicitly stated immediately before (2.14), p.15. B109's maps into older scales are the maps used in proving that assertion. Thus one has the same admitted input and output domain at every step, not a sequence α, α/2, α/4, … .

Begin at the specified source-free initial datum. Choose E₀ to dominate the g-independent Gaussian activity and the finitely many fixed extraction constants. Shrink γ_c once so that the new non-Gaussian contribution lies within the remaining fixed margin of that activity ball. This is the same inductive closure used in the regular construction, now with the stronger scale-dependent bound (4.186). Applying the step successively constructs the fixed-domain family. No continuation of an unknown incoming activity has been postulated.

Finally, B119 (3.28), p.272, identifies its interior logarithm with the B109 fluctuation integral, restricted to the regular region. Page 269 has already removed the redundant selectors there. After the common localization operations, B119 p.278 states that every term whose carrier lies inside the next regular region is independent of that region and coincides with the whole-lattice term of the regular construction; p.279 assigns these terms to the regular E family. Taking the full lattice, using the same cutoff in the displayed integral, and proceeding inductively from the same datum proves equality of the families. Their restrictions therefore agree with the B119 shrinking-domain functions. ∎

**Scope of γ_c.** This theorem supplies an explicit finite smallness test for the construction threshold. It does not silently declare an arbitrary previously fixed N2-F threshold to satisfy that test. If the program's γ is already the sufficiently small Balaban construction threshold, the inequalities are among its construction choices. Otherwise one must record the use of `min(γ,γ_c)` and the corresponding permitted terminal-coupling range in R0. No statement about the larger interval follows just by changing its name.

#### 4.25.3 Exact normalized complex dilation and current/old-family derivatives — P

**Theorem (P, in the fixed-domain scope of §4.25.2).** There is c>0 independent of g, k and volume such that Ψ_k has a joint holomorphic extension in the current coupling w on `|w−g|<cg`, the admitted fixed-domain background, and a fixed enlarged old-family ball. It agrees with the actual real map for positive real w in that interval. At inputs `‖H‖≤E₀`, with the enlarged ball `‖H‖≤2E₀` reserved for Cauchy estimates, and for `a+b≤2`,

\[
 \big\|\partial_g^aD_H^b\Psi_k(g,H)
                 [h_1,\ldots,h_b]\big\|_{\kappa,\alpha}
 \le C_{ab} E_0^{1-b}\theta(g)g^{-a}
                      \prod_{i=1}^{b}\|h_i\|_{\kappa,\alpha}.
 \tag{4.189; P}
\]

In particular the old-family derivative is O(θ), the current derivative is O(`θ/g`), the current second derivative is O(`θ/g²`), and the mixed derivative is O(`θ/g`). All fixed background projection losses remain in C_ab and C_P.

**Proof.** Fix a real centre g and use the principal logarithm in its relative disk. Define

\[
 q(w)=\frac{R(w)}{R(g)}
      =\left(1-\frac{2\operatorname{Log}(w/g)}{t(g)}\right)^p.
 \tag{4.190; P}
\]

For c small, q is holomorphic and nonzero, and `|q−1|≤C_pc/t(g)`. Take the exact change of free coordinates `B=q(w)z`. For real positive w this is the ordinary real change of variables taking the actual radius R(w) to the fixed radius R(g). For complex w it defines the extension by the same fixed-domain integral. The geometric constrained map remains C, the nonlinear constraint solver is evaluated at wqz, and the Jacobian terms in V are unchanged except for that exact substitution. Scalar dilation preserves every linear constraint; the nonlinear constraint is imposed by the same analytic chart, not by moving its constraint surface independently.

The Gaussian normalization is essential. If D is the number of real free coordinates and `Q=𝒞⁻¹`, analytic determinant branches chosen at w=g give the **exact** identity. All complex quadratic forms here use their analytic bilinear extension, not a conjugate-linear replacement:

\[
 (2\pi)^{-D/2}(\det\mathcal C)^{-1/2}
 q(w)^D e^{-q(w)^2 zQz/2}\,dz
       =d\mu_{q(w)^{-2}\mathcal C}(z).
 \tag{4.191; P}
\]

Thus the extension is

\[
 I_k^{\rm hol}(w,H)=
 \int d\mu_{q(w)^{-2}\mathcal C_k}(z)
     \prod_{b\in F_k}{\bf1}_{\{|z(b)|<R(g)\}}
     e^{V_k(w,H;q(w)z)}.
 \tag{4.192; P}
\]

There is no extra extensive vacuum factor from `q^D`. The whole Gaussian integral without cutoffs and interaction is exactly one throughout this disk. Absolute-bounding its Jacobian before cancelling the Gaussian normalization would lose this fact and would not prove (4.189).

For real positive w the integral (4.192) equals the prescribed integral (4.183) at w, including its normalization. For complex w it is holomorphic by finite-dimensional dominated differentiation. On the bounded interacting coordinates, `|wqz|≤2θ(g)` after reducing c. The original analytic background maps therefore remain inside the same fixed buffered domains. The full nonlinear constraint solver and its Jacobian are evaluated on their original admitted analytic balls. The singular-looking Wilson terms in (2.12) have already been cancelled as stated in §4.25.1; w stays away from zero in any event.

It remains to verify that the holomorphic extension has the **local**, volume-independent estimate (4.186), not merely an exponential bound on the full integral. The normalized covariance replacement in (4.191) is a scalar multiplication. Every localized quadratic form is multiplied by q²; its inverse covariance is multiplied by q⁻²; the analytic square root is multiplied by q⁻¹. This preserves the exact algebraic localization, covariance-decoupling and determinant identities used in B116. In particular it does not introduce new supports or a growing-range operator. The scalar commutes with every restriction, interpolation and the geometric linear maps.

On the original complex-background domain, the Gaussian comparison in B116 (2.15)–(2.25), pp.15–17, has a fixed strict positivity reserve. The new scalar differs from one by an arbitrarily small fixed amount. Reduce c so that its quadratic-form perturbation consumes at most half that reserve. All normalized determinant ratios and Gaussian estimates then obey the same bounds, with fixed enlarged constants. In a localized comparison one may still obtain a factor `exp(C|q−1||Z|)`; this is absorbed by the fixed decay reserve just as the α₅ term is in B116. It multiplies a nonempty polymer. It does not create an empty-polymer vacuum activity, since (4.191) keeps that term identically one.

The B116 localized interaction bound is unchanged with ε₁ replaced by 2θ(g): it uses analyticity and the inequality `|wqz|≤2θ(g)`. The complementary-cutoff tails are bounded by `exp(−c′R(g)²|P|)` because the fixed-domain z cutoff is R(g) and the normalized complex Gaussian retains coercivity. The two alternatives in B116 (2.33), p.19, remain exactly the alternatives “at least one localized interaction” or “at least one cutoff-tail component.” The first supplies a factor C E₀θ(g), and the second supplies `exp(−c′R(g)²)`, which is smaller than that factor after applying (4.187) with the reduced fixed c′. Hence the connected polymer expansion converges normally and

\[
 \sup_{|w-g|<cg}\sup_{\|H\|\le2E_0}
       \|\Psi_k^{\rm hol}(w,H)\|_{\kappa,\alpha}
       \le C E_0\theta(g).
 \tag{4.193; P}
\]

This also verifies holomorphy in the fixed weighted activity norm. No new physical cutoff has been chosen: (4.192) is a lift of the prescribed real hard-cutoff integral.

Apply Cauchy's formula in w and in complex old-family directions. For a single direction use radius proportional to `E₀/‖h‖`; for two directions split that margin between them. The normal convergence just proved permits termwise differentiation of the connected local series. The resulting first and second Cauchy inequalities are (4.189), with constants depending only on the fixed radii and construction constants. ∎

#### 4.25.4 The complete moving-cutoff derivative

For each fixed finite carrier, the real integrals in (4.183) and (4.192) are identical on an open interval. Their first and second real derivatives are therefore equal. Differentiation of (4.183) by the usual finite-dimensional transport formula produces the interior derivative, every moving-boundary term, same-face second derivatives, and pairwise-face intersections. Differentiation of (4.192) produces exactly their sum, expressed through the fixed-domain Jacobian and quadratic/interacting integrand derivatives. The mixed H/current-g derivative has the same equality with the old-family insertion present. Thus (4.189) controls the **complete localized derivative**, including those surface contributions. It does not claim an unrelated norm on every individually isolated face term.

This statement uses the product norm-ball cutoff of the regular whole-lattice map. It is not a theorem about nonlinear group selectors, source-dependent variable-weight minimizers, recent R terms, or retained-history moving interfaces. Those objects have not been converted to (4.192).

## 4.26 Coherent regular two-jet closure conditional on the running-coordinate dictionary

#### 4.26.1 Projection, feedback and the summable rates

The new bound is weaker than uniform boundedness of the current-g second derivative, but it has the rate needed after conversion to `X=g⁻²`. Define

\[
 h(g)=\theta(g)g^2=A g^3(\log g^{-2})^p,
 \qquad
 f(g)=\theta(g)g^4=A g^5(\log g^{-2})^p.
 \tag{4.194; P: definitions}
\]

If a differentiable coherent family has `u=X′` and `v=X″`, then

\[
 g'=-\tfrac12 g^3u,\qquad
 g''=\tfrac34 g^5u^2-\tfrac12g^3v.
 \tag{4.195; P}
\]

Consequently `Ψ_g g′` has size O(h|u|), and the combination `Ψ_gg(g′)²+Ψ_g g″` has size O(f|u|²+h|v|). These are statements about the actual regular map derivatives of §4.25.3; boundedness of u and v is not assumed in obtaining these rates. The old-family feedback has norm at most Cθ, and the mixed derivative has norm at most `Cθ/g`.

The Wilson projection (4.185) gives the same h and f rates with a fixed multiplier C_P. It introduces no factor g⁻², because the projected field radius is the fixed α radius. This is the precise improvement over substituting the shrinking radius into the old fixed-domain estimate.

**Lemma (P): summability on a positive-drift trajectory.** Suppose a finite real sequence obeys `X_k=g_k⁻²`, `X_k−X_{k+1}≥d>0`, and `g_k≤γ_c`. Then, after choosing γ_c small enough that the displayed functions are monotone,

\[
 \sum_{k<K}h(g_k)\le C_{d,p,A}\,
        g_K(1+\log g_K^{-2})^p,
 \qquad
 \sum_{k<K}f(g_k)\le C_{d,p,A}\,
        g_K^3(1+\log g_K^{-2})^p.
 \tag{4.196; P}
\]

Both constants are independent of K. To prove this, use `X_k≥X_K+d(K−k)` and compare the sums of `x⁻³ᐟ²(log x)^p` and `x⁻⁵ᐟ²(log x)^p` to their integrals. Substituting x=eᵗ reduces the tails to `∫_{t_K}^∞e⁻ᵗᐟ²tᵖdt` and `∫_{t_K}^∞e⁻³ᵗᐟ²tᵖdt`. Repeated integration by parts gives (4.196). ∎

N2-F supplies positive numerical drift on a sufficiently weak interval, since its decrement is at least `b₀log L−C_rγ²`. Applying that fact to the *physical regular family* still requires the normalization and baseline identification in R0. The proof of the summability lemma of §4.26.1 itself has no common-family hypothesis and uses no derivative of `r_k`.

#### 4.26.2 The exact recursion and its conditional two-jet closure

**Hypothesis R0-reg (O as a program identification, not assumed from N2-F).** In consistently normalized variables X=g⁻², the actual source-free universal coefficient and actual regular activity family obey the exact recursion

\[
 H_{k+1}=G_{k+1}+\Psi_k(g_k,H_{\le k}),\qquad
 X_{k+1}=X_k-\mathcal P_k H_{k+1},
 \tag{4.197; O: exact running-coefficient dictionary}
\]

with the fixed bounded projection appropriate to that normalization. Here H_j is the unprojected fresh regular E activity, and the old action supplied to Ψ is assembled from the H_j by the prescribed linear vacuum and Wilson subtractions. Thus the projection in the second formula is not identically zero. The pure log-g Gaussian vacuum normalization stays in its separately tracked vacuum term. The baseline values are the desired asymptotically free trajectory, satisfy the construction restrictions above, and have positive drift d. Any fixed numerical normalization factor can be included in P_k. The initial old datum has zero derivative under a variation of the consistently normalized bare X₀. Gaussian terms G_j have no explicit coupling dependence in the fixed source-free background convention. This is a statement about the actual coefficient dictionary, not about interpreting the derivative of a numerically interpolated `r_k`.

**Theorem (C on R0-reg): coherent regular two-jet closure.** Along the baseline recursion, perturb X₀ by λ and propagate the actual regular maps. For every finite K this gives a local real-analytic germ. Its first two derivatives at λ=0 satisfy bounds independent of K. Specifically, for

\[
 u_k=\partial_\lambda X_k(0),\quad
 v_k=\partial_\lambda^2X_k(0),\quad
 U_k=\max_{i\le k}|u_i|,\quad
 V_k=\max_{i\le k}|v_i|,
 \tag{4.198; P: definitions}
\]

there are fixed constants C and C_H such that

\[
 \|H_{k+1}'\|\le C_H h(g_k)U_k,
 \qquad
 \|H_{k+1}''\|\le
       C_H\{f(g_k)U_k^2+h(g_k)V_k\},
 \tag{4.199; C}
\]

and

\[
 U_K\le\exp\!\left(C\sum_{k<K}h(g_k)\right),\qquad
 V_K\le C\exp\!\left(C\sum_{k<K}h(g_k)\right)
                   \sum_{k<K}f(g_k).
 \tag{4.200; C}
\]

After one fixed further smallness choice on the admitted interval, all u_k lie between 1/2 and 3/2. The conclusion controls the actual complete E-family response of the universal coefficient at two constant-scalar insertions. It does not control marked R/B or nonconstant scalar sources.

**Proof.** For finite K, the holomorphic maps in §4.25.3 and the local analytic branch `g=X⁻¹ᐟ²` construct the coherent germ recursively; the radius of that germ is not asserted here to be uniform in K. The input/output ball has a fixed buffer, so all finitely many compositions are defined near λ=0.

Write A_k for the maximum of the first-derivative norms of the incoming old family, and B_k for the analogous maximum of second derivatives. The exact chain rule is

\[
 H_{k+1}'=\Psi_g g_k'+D_H\Psi[H_{\le k}'],
 \tag{4.201; P}
\]

\[
 \begin{aligned}
 H_{k+1}''={}&\Psi_{gg}(g_k')^2+\Psi_g g_k''
 +2D_H\Psi_g[H_{\le k}']g_k'\\
 &+D_H^2\Psi[H_{\le k}',H_{\le k}']
 +D_H\Psi[H_{\le k}''].
 \end{aligned}
 \tag{4.202; P}
\]

No unknown coupling tangent has been dropped. Equations (4.189) and (4.195) give

\[
 \|H_{k+1}'\|\le C h_k|u_k|+q_k A_k,
 \qquad q_k=C\theta(g_k),
 \tag{4.203; C}
\]

and

\[
 \|H_{k+1}''\|
 \le C(f_k|u_k|^2+h_k|v_k|)
 +C\theta(g_k)g_k^2 A_k|u_k|
 +C\theta(g_k)E_0^{-1}A_k^2+q_kB_k.
 \tag{4.204; C}
\]

Here h_k=h(g_k) and f_k=f(g_k). Positive drift makes g_k increase, and γ_c can be chosen so that h and f also increase on the admitted interval. Take `sup q_k<1/4`. Starting with zero incoming derivatives, (4.203) then proves the first bound (4.199) by induction in the maximum-over-ages norm. In (4.204), substitute `A_k≤C_H h_kU_k`. The mixed term is bounded by a constant times `θ_k f_kU_k²`; the quadratic old-family term is bounded by a constant times `θ_k² f_kU_k²`. These are absorbed into the first term after increasing a fixed constant. The final term is a strict contraction on the old second-derivative envelope. The same induction gives the second bound (4.199). There is no sum over ages left unpaid.

Differentiating the exact coefficient recursion (4.197) and using the fixed projection norm now gives

\[
 U_{k+1}\le(1+C h_k)U_k,\qquad
 V_{k+1}\le(1+C h_k)V_k+C f_kU_k^2.
 \tag{4.205; C}
\]

With u₀=1 and v₀=0, iteration gives (4.200), adjusting the fixed C. The summability lemma of §4.26.1 makes both right-hand sides independent of K. Moreover `|u_k−1|≤exp(CΣh_i)−1`, so a sufficiently weak fixed interval makes this at most 1/2. ∎

This proof does not assume a common-family strengthening of N2-F. It supplies its own regular-family tangent equations once the exact physical coefficient recursion is identified. In particular, it makes no claim that `r_k′` in the quoted numerical interface equals a derivative obtained by freezing or varying older physical activities.

This closes the displayed feedback inequalities once R0-reg is verified. It does not supply an ultraviolet-depth-independent analytic radius for the fully composed bare-source family, does not match a larger preassigned coupling interval, and does not control the spatially varying source, tensor, R or B sectors. Those statements remain separate in R0/R1/R3. The original N2-F quote is unchanged.

## 4.27 An alternative R2 route through complex pressure and literal chessboard factors

The fractional inverse-mass estimate (4.81) is one sufficient route. The following different route is logically available; its hypotheses are not proved by this note.

**Proposition (C: application conditional on the following three hypotheses).** Suppose the unchanged finite-lattice Wilson construction, with every history retained in its complete integral, has been shown, on a fixed complex finite-source domain stable under the required reflected copies, to satisfy all of the following.

1. The actual old physical source is carried through every transformation, including every compulsory old kernel and every selector branch. After extracting the same source-zero vacuum and an explicit source-excess vacuum, the exact representation and bounds are

\[
Z_a[j]=e^{V_a+E_a[j]}W_a[j],\qquad
E_a[0]=0,\qquad
|W_a[j]|\le e^{C_+N_T},\qquad
W_a[0]\ge e^{-C_-N_T}.
\tag{4.206; C: required all-history estimate}
\]

2. The vacuum has a deterministic source-local decomposition, on that same complex domain,

\[
E_a[j]=\sum_c L_a(j|_c)+R_a[j],\qquad
|\operatorname{Re}R_a[j]|\le C_LN_T,
\tag{4.207; C: required local-vacuum comparison}
\]

where \(L_a(0)=0\), \(L_a\) is analytic and translation/reflection covariant, and \(L_a(\bar j)=\overline{L_a(j)}\). For supported sources with margin, the reflected local factors must be the literal reflections of the original plaquette observable; the P2 source-placement dictionary must be checked.

3. The source-free Wilson measure has the appropriate chessboard inequality for those local factors, including its conjugate-reflection version for complex functions. The copied source patterns stay in the domain of (4.206)–(4.207), after a fixed radius reduction if necessary.

Then a source \(j\) supported in a single cell has a cutoff- and volume-independent normalized bound

\[
\left|e^{-L_a(j)}\frac{Z_a[j]}{Z_a[0]}\right|
\le e^{C_++C_-+C_L}.
\tag{4.208; C conclusion, proved from (4.206)–(4.207) and chessboard}
\]

The generalized chessboard inequality yields the corresponding bound exponential only in the number of active cells for products of local source factors. Finite-dimensional Cauchy then controls their fixed-order source derivatives on smaller source domains. At any fixed finite number of active profiles, connected coefficients follow from the finite moment–cumulant formula. This proposition does not assert the uniform all-order factorial growth or contact-support theorem needed elsewhere in the program.

**Proof.** Define the literal local observable \(F_j(U)=\exp(J_j(U)-L_a(j))\). A disseminated product of its reflected/conjugated copies is precisely the fully copied Wilson source exponential times its copied local vacuum factors. Equations (4.206)–(4.207), with the one final denominator \(W_a[0]\), bound the absolute expectation of that product by \(\exp((C_++C_-+C_L)N_T)\). Taking the \(N_T\)-th root by chessboard proves (4.208). For a product in several distinct cells, the generalized inequality gives a product of the corresponding single-factor chessboard norms; each costs only the same fixed exponential constant. Cauchy applies on the fixed smaller complex domain. All old compulsory masses remain in (4.206), and none has been inverted locally. ∎

**Exact residual for this alternative (O).** Prove (4.206) for the actual finite-source history family, with the real old payload and all inherited analytic radii retained; prove the source-local vacuum comparison (4.207); and establish the literal reflection/replication matching. The raw reserve in §4.3 and the initial conditional innovation estimate in §4.24 supply useful pieces. They do not establish the predictable old-source interaction, the required complete historical analytic bounds, or the vacuum/contact comparison. The incoming atom classification of the [source estimates](../source_estimates/README.md), (S62), p.603, uses the historical coupling domains of (S44a), p.595, the delayed-admission estimate (S44b), p.596, and the old-readout coverage claimed on pp.612–613. These inputs still require proof for the actual source family.

This proposition concerns literal local source factors, not exterior-dependent conditional innovations. Its hypotheses include the complex pressure bound, the local vacuum bound on that same complex domain, and the exact reflection placement. Real N1-S bounds, a numerical coupling trajectory, or ordinary Gaussian concentration do not supply these hypotheses automatically. The extension to coincident products, a common local field algebra and the corrected all-order OS growth remains R3/R4.

**Representation-stage clarification.** The bounds in (4.206) are integrated pressure bounds. They may be sought after the regular E and erased-R connected integrations and their source-dependent vacuum extractions have been performed. They do not assert a pointwise bound on the fully unreduced original-field exponential. Section 4.32 proves that the latter proposed bound by physical volume plus bad-record count fails, even for a permitted scalar cell source. Keeping the old physical source means evaluating or integrating its actual old readout, not retaining every original variable pointwise in the final effective bound.

## 4.28 Entering any required weak interval without changing N2-F

This is an explicit-threshold restatement of the forward-invariant-sublevel argument already proved in §4.9.1, not an additional independent closure. The revised existence target permits choosing one sufficiently small terminal coupling. This freedom resolves the numerical weak-ceiling issue without replacing the γ in the assumed interface. It does not by itself identify the numerical coordinate with the physical running coefficient.

**Theorem (P).** Use N2-F in its stated numerical variable \(x_k=g_k^{-2}\). For any required threshold \(A\), choose

\[
D=b_0\log L,\qquad
M=\max\{0,C_r\gamma^2-D\},\qquad
A\ge\max\{\gamma^{-2},\,2C_r/D\}.
\tag{4.209; P: definitions and hypotheses}
\]

If \(x_K>A+M\), then the entire trajectory stays above A and has positive drift:

\[
x_k\ge x_K+\frac D2(K-k)\ge A,\qquad
\frac D2\le x_k-x_{k+1}\le D+C_r/A
\quad(0\le k<K).
\tag{4.210; P}
\]

Consequently, for any prescribed numerical ceiling \(\gamma_c>0\), one may increase A to at least \(\gamma_c^{-2}\) and choose
\(0<g_*\le\min\{\gamma/2,(A+M+1)^{-1/2}\}\).
Then N2-F supplies a trajectory with \(g_k\le g_*\le\gamma_c\) at every scale, uniformly in K. This selects a permitted terminal coupling; it makes no claim for all larger terminal couplings in the original interface.

**Proof.** By N2-F(ii), every \(x_k\ge\gamma^{-2}\). The recurrence and remainder bound give
\(x_{k+1}-x_k=-D+r_k(x_k)\le-D+C_r\gamma^2\le M\).
Whenever \(x_k\ge A\), they give
\(D/2\le x_k-x_{k+1}\le D+C_r/A\).

Suppose some \(x_j<A\). Since \(x_K>A+M\ge A\), there is a last such j, with \(j<K\). Its next value satisfies
\(A\le x_{j+1}<A+M\).
All subsequent values lie above A by the choice of j and therefore decrease. Thus
\(x_K\le x_{j+1}<A+M\), a contradiction. There is no such j. Summing the lower decrement now gives (4.210). ∎

If the physical Balaban variable is established to be \(X_{B,k}=c\,x_k\), with a fixed positive conversion c, the same proof imposes its construction threshold by taking \(A\ge c^{-1}\gamma_{B,c}^{-2}\). The bare identity \(c=2N^2\) is already proved; applying that conversion at every running scale is still the explicitly separate R0 identification.

This lemma uses neither N2-F's derivative clause nor a common-family interpretation of its remainders. Together with the summability estimate (4.196), it supplies arbitrarily small numerical feedback budgets by selecting a sufficiently small terminal coupling. A restricted choice of terminal coupling is sufficient for YM-E; it does not prove original N1-S on its entire stated interval.
