# Integrated raw densities and positive marginalization

## 1. The completed transport statement and its scope

This note combines two proved actual-model inputs: the normalized Wilson energy theorem in [Wilson normalization of local energy budgets](../energy_budgets.md), (CA.2), and the all-SU(N) first-star source theorem in [Scalar-source bounds for a Wilson link in SU(N)](r1_su_n_global_star.md), Theorem 2.1 and (G21). It proves transport of the actual source density, and every finite source derivative of that density, through an arbitrary number of complete positive, source-independent marginalizations. The initial probability law is the exact first-layer exterior marginal of the original Wilson measure. Every inherited first-star source is retained as its actual exterior function.

This is a completed normalized transport theorem in an integrated raw norm. It does not require prior admission of the source into a pointwise analytic field norm. It also does not provide the physical-volume R2 bound: its root budget is the number of sourced fine plaquettes divided by the bare coupling. The distinction is quantitative, and is displayed below. A final counterexample proves that integrated exponential control alone cannot supply the missing pointwise logarithmic source domain on every compulsory component.

Use SU(N), the literal plaquette action s_p=N−Re Tr U_p, and the N2-F bare coefficient β=β_K. Let μ be the normalized original Wilson law on a compatible torus. Fix a set I of links with no common plaquette. Let P_I be the union of their six-plaquette stars, and P_ext the remaining plaquettes. The set I can be arbitrary, including empty. Denote its exact source-free exterior marginal by μ_ext. With the notation of the global star theorem,

\[
 d\mu_{\rm ext}(v)=Z[0]^{-1}
   e^{-\beta\sum_{p\in P_{\rm ext}}s_p(v)}
   \prod_{b\in I}Z_\beta(v_b;0)
   \prod_{e\notin I}dU_e.
 \tag{T.1; P}
\]

This formula has total mass one by exact Haar integration. No conditional component is separately rescaled.

Give every plaquette an independent complex source z_p. Sources outside an arbitrary specified finite set P_0 are zero. The set P_0 may be the whole torus; no support separation is required. For each b∈I let z_b be its six actual source values. Define

\[
 \begin{aligned}
 A(z)&=\sum_p|z_p|,\qquad r(z)=\max_p|z_p|,\\
 F_1(z;v)&=\sum_{p\in P_{\rm ext}}z_ps_p(v)
                      +\sum_{b\in I}\Phi_\beta(z_b;v_b),\\
 G_1(z;v)&=\exp F_1(z;v),\qquad
 L_I(z)=\sum_{b\in I}L_\beta(z_b).
 \end{aligned}
 \tag{T.2; P: actual first-layer readout and deterministic flat vacuum}
\]

The original scalar source is recovered by z_p=j^(0)(x_p). The exact physical identity is

\[
 e^{-L_I(z)}\frac{Z[z]}{Z[0]}
       =\int G_1(z;v)\,d\mu_{\rm ext}(v).
 \tag{T.3; P}
\]

There is no fresh centering of the old Φ_b at a later integration.

**Related results.** [Raw core sources in the large-field operation](../raw_core.md) proves analytic erased-R admission and connected flat vacuum extraction for strict original-variable core sources, whose complete support stays in one actual operation. It uses the printed capacity ledger rather than inferring analyticity from the Lᵖ bound below. Complementary E/B and boundary readouts remain open. [Cross-shell Gaussian source transport and local vacuum](cross_shell_gaussian_source.md) separately proves the full flat Gaussian source theorem; neither result turns this note's general fine-anchor bound into an interacting physical-cell estimate by contraction alone.

## 2. Uniform integrated admission and every subsequent complete positive transition

**Theorem 2.1 (P).** There are constants r_*,c_*,C_* >0, independent of the cutoff, torus, source, and set I, such that, whenever

\[
 r(z)<r_*,\qquad 1\le p<\infty,\qquad p\,r(z)\le c_*\beta,
 \tag{T.4; P: admitted source and integrability domain}
\]

one has

\[
 \|G_1(z)\|_{L^p(\mu_{\rm ext})}
       \le \exp\!\left(\frac{C_*}{\beta}A(z)\right).
 \tag{T.5; P}
\]

Let Q(dw|v) be any complete positive probability kernel, independent of z, with input law exactly μ_ext. It may be a composition of any finite number of such kernels and may retain all its history labels. Put ν=μ_ext Q and ν_z=(G_1(z)μ_ext)Q. Then

\[
 \begin{aligned}
 G_Q(z;w)&=\frac{d\nu_z}{d\nu}(w)
              =\mathbb E_{\mu_{\rm ext}Q}[G_1(z;v)\mid w],\\
 \|G_Q(z)\|_{L^p(\nu)}
       &\le \exp\!\left(\frac{C_*}{\beta}A(z)\right),\\
 \int G_Q(z)\,d\nu
       &=e^{-L_I(z)}Z[z]/Z[0].
 \end{aligned}
 \tag{T.6; P}
\]

The density is positive ν-almost everywhere for real z. It is holomorphic as an L^p-valued function on any source domain whose closure satisfies the strict versions of (T.4). No logarithm of G_Q at individual retained configurations is asserted.

**Proof of initial admission.** The all-real star theorem gives
|Φ_β(z_b;v_b)|≤C(Σ_{p∋b}|z_p|)W_b(v_b).
The actual minimum satisfies W_b(v_b)≤S_b(U), where S_b is the sum of the six original plaquette actions and U is any completion of the retained exterior. Every remaining plaquette p∈P_ext may be assigned once to one of its positive boundary links e(p); that link is outside I. Since s_p≤S_{e(p)}, there are nonnegative deterministic weights η_b(z) with

\[
 |F_1(z;v(U))|\le\sum_b\eta_b(z)S_b(U),\qquad
 \max_b\eta_b(z)\le C_0r(z),\qquad
 \sum_b\eta_b(z)\le C_0A(z).
 \tag{T.7; P}
\]

For example use η_b=CΣ_{p∋b}|z_p| for b∈I and add the assigned |z_p| to each e(p) outside I. A link belongs to only six plaquettes, so all multiplicities in (T.7) are bounded. Choose r_* so that every six-entry source lies in the proven star domain.

The normalized Wilson energy theorem gives constants κ,C_E with
log μ exp(κβΣ_b w_bS_b)≤C_EΣ_bw_b for 0≤w_b≤1. Apply it with w_b=pη_b/(κβ); (T.4), with c_*=κ/C_0, ensures w_b≤1. Since μ_ext is the actual marginal of μ,

\[
 \int e^{p|F_1(z)|}\,d\mu_{\rm ext}
   \le\exp\!\left(\frac{C_Ep}{\kappa\beta}
                          \sum_b\eta_b(z)\right)
   \le\exp\!\left(\frac{C_*p}{\beta}A(z)\right).
 \tag{T.8; P}
\]

Taking a p-th root proves (T.5).

**Proof of transport.** The Radon–Nikodym identity in (T.6) is the defining conditional-expectation formula for the joint positive law μ_ext(dv)Q(dw|v). Conditional Jensen gives |E(G_1|w)|^p≤E(|G_1|^p|w), proving the norm contraction. The total-mass identity follows because Q has row mass one. Iterating or composing complete positive kernels gives the same proof and constants, with every inherited factor retained. At each finite lattice there are finitely many bounded source terms, so their finite source derivatives may be integrated under a common local majorant; (T.8) gives the stated uniform L^p bounds on smaller domains. This proves holomorphy and the claims. ∎

For a measurable compulsory component H of the retained history space and p>1, Hölder gives the mass-sensitive consequence

\[
 \int_H|G_Q(z)|\,d\nu
   \le \nu(H)^{\,1-1/p}
           \exp\!\left(\frac{C_*}{\beta}A(z)\right).
 \tag{T.9; P}
\]

This keeps a positive power of the actual old component mass. It does not replace that mass by one. Dividing by ν(H) to normalize the component separately would introduce ν(H)^{-1/p}; no uniform bound for that inverse factor follows. Similarly, summing the right side of (T.9) over a very large partition may incur a history-entropy loss. Those extra operations are not part of the theorem.

The statement applies directly to the usual exact successive Haar integrations: their source-free retained marginals and conditional probabilities are the actual ones. For a Balaban history expansion, Q must first be identified as a complete positive lift with this same marginal. A signed R-operation activity expansion is not automatically such a Q merely because its sum reconstructs the physical measure.

There is also a precise application to the real erased-R formula (R1.30) of [Tensor quadratic admission and the marked transition](tensor_quadratic_admission.md). Let λ(dv)σ_v(dζ) be its actual old positive joint measure, including its nonconstant compulsory mass, and let q_v(du) have total mass one. Write F_1=A_f and F_2=A_{fg}+A_fA_g for the first and second old density jets. The erased kernels are R^(m)(v,du)=q_v(du)∫σ_v(dζ)F_m(v,ζ), and R^(0)(v,du)=q_v(du)σ_v1. Conditional Jensen, without renormalizing the exterior law or the whole component, gives

\[
 \left\|\frac{d(\lambda R^{(m)})}{d(\lambda R^{(0)})}
       \right\|_{L^p(\lambda R^{(0)})}
 \le \|F_m\|_{L^p(\lambda\sigma)},\qquad m=1,2.
 \tag{T.9a; P: exact real erased-R contraction}
\]

On exteriors of zero old mass both kernels vanish and the density is set to zero. The assertion holds for finite positive measures of total mass below one as well as probability measures. It proves that this real erasure operation itself costs no factor in the averaged raw norm, even with an arbitrarily small and nonconstant old mass. If the old joint law and incoming density jets are the complete positive lift already covered by (T.6) and (T.11), those same bounds feed directly into (T.9a). Identifying that lift for the full marked Balaban expansion is an additional dictionary obligation; (T.9a) does not identify a signed recent-R difference with a positive probability kernel, and it makes no complex-exterior or pointwise conditional-mean claim.

## 3. Exact source-jet radii and the fine-anchor limitation

Let f^1,…,f^m be arbitrary finite plaquette arrays, and put z=Σ_{r=1}^mλ_rf^r. Set F_r=max_p|f_p^r| and A_r=Σ_p|f_p^r|. Directions with F_r=0 give the zero mixed derivative and may be omitted. For any positive radii R_r satisfying

\[
 \sum_rR_rF_r<r_*,
       \qquad p\sum_rR_rF_r<c_*\beta,
 \tag{T.10; P: an explicit admissible source polydisc}
\]

the Bochner-valued Cauchy formula and (T.6) give

\[
 \left\|\partial_{\lambda_1}\cdots\partial_{\lambda_m}
        G_Q\!\left(\sum_r\lambda_rf^r\right)\Big|_{\lambda=0}
       \right\|_{L^p(\nu)}
 \le
   \exp\!\left(\frac{C_*}{\beta}\sum_rR_rA_r\right)
          \prod_rR_r^{-1}.
 \tag{T.11; P}
\]

This is a derivative of the actual inherited density. Every same-star contact and every mixed product already generated by exponentiation is included; none is silently discarded. Differentiation also commutes with the conditional-expectation formula, because Q is source independent.

For a concrete uniform choice take 0<θ<min(r_*/2,c_*\beta/(2p)) and R_r=θ/(mF_r). Then

\[
 \begin{aligned}
 \left\|D^mG_Q(0)[f^1,\ldots,f^m]\right\|_{L^p(\nu)}
 &\le m!\left(\frac e\theta\right)^m
   \exp\!\left(\frac{C_*\theta}{\beta}n_{\rm eff}\right)
                         \prod_rF_r,\\
 n_{\rm eff}&=\frac1m\sum_r\frac{A_r}{F_r}
                   \le\left|\bigcup_r\operatorname{supp}f^r\right|.
 \end{aligned}
 \tag{T.12; P}
\]

The inequality m^m≤e^m m! gives the factorial. For every fixed p, θ can be chosen independent of K, since β≥2Nγ^{-2}. Restricting the derivative to a compulsory event H gives the additional factor ν(H)^{1−1/p} by the same Hölder argument as in (T.9).

There is a substantial quantitative gap between this theorem and physical-volume R2. If P_0 consists of the fine plaquettes in D physical cells, then its cardinality is of order L^{4K}|D|. A bounded source therefore has A(z)≤r(z)|P_0|, and the exponent in (T.5) is only bounded here by

\[
 \frac{C_*r(z)}{\beta_K}|P_0|
       \le C\,r(z)\frac{L^{4K}}{\beta_K}|D^+|.
 \tag{T.13; P}
\]

Here D^+ includes the fixed boundary collar needed to count plaquette anchors. Along N2-F, β_K grows linearly to leading order in K. The right side is not uniform as the cutoff is removed. A factor (a/ℓ_0)^4 may not be inserted into the original scalar source to change this count. The separate dimension-four-weighted energy budget in (CA.24)–(CA.25) has such a factor by definition; the physical source in the preamble does not.

The first flat-star vacuum L_I is local and already subtracted in this result. Further local vacuum contributions, as well as the field-valued identity/dimension-four contact projections, must still be extracted from the inherited source. Complete positive marginalization preserves the proved raw norm but cannot itself perform that extraction.

## 4. A precise obstruction to the stronger inference and the remaining bridge

**Proposition 4.1 (P: abstract counterexample).** Uniform integrated exponential-energy bounds, actual normalization, and complete positive marginalization do not imply a fixed pointwise source-logarithm radius on every retained compulsory component.

**Proof.** Fix κ>0. For M>0 let H be an event of probability q_M=e^{-2κM}. Conditional on H, let X equal +M and −M with probabilities 1/2 each; outside H let X=0. Define the nonnegative energy A=M1_H. The complete marginalization retains only the event label H and averages the sign. Then

\[
 \mathbb E e^{\kappa A}
       =1-q_M+q_Me^{\kappa M}\le2,\qquad
 G_M(z;H)=\mathbb E[e^{zX}\mid H]
       =\begin{cases}
          1,&H\text{ does not occur},\\
          \cosh(Mz),&H\text{ occurs}.
        \end{cases}
 \tag{T.14; P}
\]

For any fixed p≥1 and |z|≤κ/p,

\[
 \|G_M(z)\|_{L^p}^p
       \le1-q_M+q_Me^{pM|z|}\le2,
       \qquad
 G_M\!\left(\frac{\pi i}{2M};H=1\right)=0.
 \tag{T.15; P}
\]

Thus the complete source-density transport has a uniform integrated analytic domain, retaining the exact rare mass q_M. Nevertheless the normalized density on the positive-probability component H=1 has a zero at distance π/(2M) from the origin. A single-valued pointwise logarithm on a fixed source disk is impossible as M grows. No component mass was lost or artificially replaced in the example. ∎

This example defeats the inference from integrated raw control to pointwise logarithmic admission on each retained history. It is not a Wilson counterexample, and it does not disprove a physical free-energy bound after summing all histories and making the proper local subtractions. It identifies exactly why Jensen contraction cannot finish that proof.

The results above cover the following concrete operations.

| Operation | What is proved |
|---|---|
| Original Wilson average | Uniform exponential moments of β-weighted local star and bare clover energy budgets, under the actual normalized law |
| First disjoint link layer | Exact all-SU(N) inherited source, deterministic local flat vacuum, fixed source domain at every real exterior, and a retained action reserve |
| Further complete positive marginalizations | Exact inherited densities and every source jet in the integrated L^p norm, with no inverse component mass |
| A fixed second star patch | Exact reopening and integration of the first inherited source; the separate second-patch notes give regular complex admission, explicit field-valued source contacts, and all-real energy/source bounds for the bounded acyclic patch |

**The unresolved bridge (O).** For one actual constrained Balaban step with its permitted old large-field components, prove a local source extraction that turns the actual inherited density into: (a) a specified deterministic local vacuum contribution, (b) its full dimension-four field-valued outputs, including the generated same-point source contacts, and (c) a remainder whose analytic regular-field norm and integrated large-field norm are stable with a physical determining-block count. The estimate must keep the original component masses and actual source placements. Its constants must be uniform over the permitted scale histories, rather than depend on a fixed finite patch size.

The present note supplies the integrated raw transport part of such a mixed norm. It removes the need to prove that part by inventing a new centered mark or dividing by an arbitrarily rare event. It does not supply local identity extraction, the complex-field operator bound after that extraction, or a proof that the complete marked cluster operation closes in the mixed norm. A valid alternative could work directly with density activities and avoid individual logarithms, but it must prove its local multiplication, projection, and connected-expansion estimates; (T.14)–(T.15) show that those estimates cannot be replaced by a pointwise logarithm inferred from L^p control.

Even the original source support count is still visible in (T.13). Eliminating that ultraviolet count by a source-local vacuum prescription, while retaining the actual nonidentity contacts, is the first quantitative obligation not supplied by the complete positive transport theorem. Full R1, physical-volume R2, N1-S, and the Yang–Mills existence target remain open at that bridge.
