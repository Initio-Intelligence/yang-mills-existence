# Survival estimates for the unreplaced history

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

## 1. Result and scope

There is a useful full-law estimate which is weaker than the remaining local H02 theorem. At a fixed terminal lattice, let \(\mathcal C_k\) be the occupied space-time cost of the **currently unreplaced** large-field forest, defined below from the actual positive source history. Then, for a fixed positive \(u\) and a sufficiently small common coupling ceiling,
\[
 \mathbb E_{\mathrm{full},k}\exp(u\mathcal C_k)
       \le \exp(C_u V_k).
 \tag{H2S.1}
\]
Here \(V_k\) is the volume in terminal lattice units. The expectation has the full positive Wilson/history normalization. No conditioning on a selector forcing a failure is used. The constant is independent of UV depth and volume; its dependence on the fixed terminal weak-coupling range is retained.

The cost includes an occupied-component charge at every outer renormalization step. It therefore controls the oldest continuously surviving age of each current unreplaced component, even at a step with no surviving Gaussian integration variable. This resolves the fine-birth-age loss at the level of the marked positive majorant. It is not a birth-only union bound.

Section 5.3 proves a stronger version with a growing scale-dependent weight, paid by fixed shares of the source birth reserves. It gives the explicit age tail (H2S.41), the sharper current bad-volume and pointwise bounds (H2S.40), and the single sublinear age threshold (H2S.42). Section 6.1 proves that the sector older than this threshold is negligible even with the **original bare physical insertions**, in every fixed transported \(L^q\) product or rare-cumulant norm along the accepted slow-volume Wilson sequence.

The estimate has an extensive factor on the right. It does **not** prove a volume-uniform local exponential moment, a local deletion ratio, a bound on a posterior already conditioned to contain the bad component, or the stated all-moment M03 carrier norm. Section 8 records the exact normalized comparison still needed for those stronger conclusions. Sections 6–7 give actual finite-volume tightness consequences which do follow from the marked pressure bound.

The inputs are the retained real source construction, its literal positive history law, LFR II (1.79)–(1.89), and the upper and lower ultraviolet-stability bounds of CMP119 Corollary 3. For the optional energy insertions we also use the same fixed-fraction argument already verified in H03, NR20.5–NR20.10. The C05/C06/C08 results do not substitute for these large-field inputs.

## 2. The forest and the cost are actual source objects

### 2.1 Which genealogy is retained

Fix a current outer scale \(k\). The current unreplaced large-field components are the actual components remaining in the source external large-field region. The genealogy of such a component consists of its previous large-field ancestors, propagated by ordinary growth, mergers, and failed preparations. Completing the old whole-component integral terminates that old genealogy. Earlier completed archives are not counted again.

There are two outcomes at a completion. A first-class component is deleted from the large-field region. A second-class \(Y\) remains large-field, but LFR II (1.102)–(1.104), pp.390–392, integrates its old operation and leaves a multiplier \(\tau_b(V_b)=T'_b(Y)1\), selectors and gauge factors depending only on the new raw \(V_b\). Such a \(Y\) starts a **new active birth at \(b\)**. Its reserve is the actual small mass \(\tau_b\), not a second charge of its old hidden energies. This convention uses the exact completed alternative representation; the old variables can remain in an augmented archive for observables, but are not external variables of the new active operation. Thus a still-external \(V_b/\tau_b\) slot has active age at least \(k-b\), while its already integrated archive is not counted by \(\mathcal C_k\).

There is no splitting in this active genealogy. The ordinary construction enlarges components and can merge them. LFR I p.181, after (1.22) and (1.23), excludes a failed **whole component** from the attempted region and leaves it unchanged by the remaining preparation. LFR I p.201, after (1.99), factors the external operation on the original complement of the attempted region and then renames that external region. Thus the failed original component persists in the external large-field bookkeeping. It is not to be identified with the smaller prepared determining complement \(Z_j''\).

For a set \(D\) of distinct current unreplaced components, let \(\mathscr A_j(D)\) be its actual ancestor components at outer scale \(j\), after their last completed renewal and with no intervening completed renewal. Ancestor families belonging to distinct elements of \(D\) are disjoint at each \(j\). Several ancestors of one current component may have merged. We will not charge a separate post-merger age to every earlier tag.

The substep index of a preparation is not an extra outer time. A component frozen during the rest of one preparation is counted once at that outer scale, not once for each remaining substep.

### 2.2 Literal units and the harmless occupied-cell augmentation

Let \(d'_j(Q)\) be the source linear size measured on the \(MR_j\) grid. Set
\[
 c_j(Q)=M^dR_j^{d+1}\bigl(d'_j(Q)+1\bigr),
 \qquad
 \mathcal C_k(D)=
    \sum_{j\le k}\sum_{Q\in\mathscr A_j(D)}c_j(Q).
 \tag{H2S.2}
\]
Take \(\mathcal C_k=\mathcal C_k(D_k)\) for all current unreplaced components. Changing fixed lattice-unit conventions multiplies this cost by a fixed constant.

The term without the added one is precisely the positive domain cost in LFR II (1.79), (1.80), (1.83), and (1.85). The added one is stated explicitly because a diameter convention can give \(d'_j(Q)=0\) for a single coarse cube. Section 3 proves that its entire chronological cost is allowed by the same source budget. No inference from the number of integrated coordinates is made.

This is a function of genuine positive-history geometry. It does not count a generalized-walk expansion, signed cluster terms, C05 carrier copies, or artificial old variables obtained by refining a coarse atom. Field-independent geometry marks multiply the original positive summands; they do not alter their action, their old reference normalizers, or their coefficient banks.

The elementary cube-cover bound gives
\[
 |Q|_j\le C M^dR_j^d\bigl(d'_j(Q)+1\bigr),
 \qquad
 R_j|Q|_j\le Cc_j(Q).
 \tag{H2S.3}
\]
The volume \(|Q|_j\) is on its actual native \(j\)-lattice. It is not its current coarse cover and not the rank of its remaining Gaussian integration. In particular each nonempty occupied component has \(c_j(Q)\ge c_*>0\).

## 3. Replaying the source chronological reserve with the added cost

The needed source facts are explicit in LFR II pp.383–387.

* The estimate (1.79) is stated to hold for **all** large-field regions. It bounds the same real positive operations, after bounding the effective-action and normalization terms by their native domain costs. Gaussian restrictions are dropped only at the majorant step; their actual determinants and other normalizations have already been retained.
* The factor associated with an occupied component is written on p.384 as \(\exp[-\kappa_j(Q)-2P_0(g_{j(Q)})]\). The store \(\kappa_j\) pays all future domain costs until the no-new-bad growth becomes eligible.
* Equation (1.81) bounds that future cost by
\[
 C M^dR_j^{d+2}\bigl(d'_j(Q)+1\bigr).
 \tag{H2S.4}
\]
* Equations (1.83), (1.85), and (1.87)–(1.88) perform the no-new-bad, new-birth/merger, and bounded failed-preparation steps. The strict reserve includes \(P_0(g)\gg C M^dR(g)^{d+2}\), with the stronger ordinary-birth reserve supplied by \(P_0(g)^2\).
* After (1.89), p.387 expressly extends the result to arbitrary large-field regions with the additional full-tree factor \(\exp[-\kappa_1d_k(Q)]\).

### Lemma H2S.1 — an occupied-component charge is admissible

Replace the source step cost by
\[
 C M^dR_j^{d+1}d'_j(Q)+u\,c_j(Q),
 \tag{H2S.5}
\]
where \(u\ge0\) is fixed. The chronological induction remains valid, with changed fixed constants and a smaller common coupling ceiling. A fixed positive share of its final component and full-tree decay remains.

**Proof.** The part proportional to \(d'_j\) just increases the fixed cost coefficient. We check the added occupied-component term.

For a no-new-bad run beginning at \((j,Q)\), the scaling estimate used before (1.81) implies that after at most \(C\log(d'_j(Q)+1)+C\) steps its coarsened cover fits in a bounded \(MR_n\)-cube. At most \(CR_j\) further steps are needed for the waiting condition, exactly as in the proof of (1.81). Thus its length \(K\) satisfies
\[
 K\le C\log(d'_j(Q)+1)+CR_j.
 \tag{H2S.6}
\]
The retained **global** comparison in CMP119 (2.6), \(g_j\le(1+\beta_0)g_n\) for \(n\ge j\), gives
\(\log g_n^{-2}\le\log g_j^{-2}+2\log(1+\beta_0)\). The least-\(L\)-power rounding then yields \(R_n\le CR_j\), uniformly for every later \(n\) in the admitted run. No assumption that \(K\) is small compared with \(R_j\), and no positive raw one-step coupling drift, is used. Consequently
\[
 \begin{aligned}
 \sum_{n=j+1}^{j+K} M^dR_n^{d+1}
 &\le C M^dR_j^{d+1}
       \bigl[\log(d'_j(Q)+1)+R_j\bigr]\\
 &\le C M^dR_j^{d+2}\bigl(d'_j(Q)+1\bigr).
 \end{aligned}
 \tag{H2S.7}
\]
This has exactly the order of (H2S.4), including its plus one. It applies also to a zero-diameter convention or a run in which no Gaussian variable is integrated.

For a fresh ordinary birth the source factor proportional to
\(P_0(g_j)^2(d'_j+1)\) pays the enlarged fixed coefficient in (H2S.4). For a failed preparation the component is bounded by the source eligibility condition, and its new \(P_0(g_j)\) reserve pays the enlarged \(CR_j^{d+2}\) cost.

For a new retained \(Y\) following a completed operation, its literal mass satisfies (1.89),
\(\tau_b\le\exp[-2(1+\beta_0)^{-1}P_0(g_b)]\). Split this fixed exponent into a positive base mass and a positive future store. The component is bounded, so \(P_0(g_b)\gg C_uR_b^{d+2}\) pays (H2S.4) with the new cost constant. This gives the additional renewal case without modifying \(\tau_b\) or reopening its completed hidden history.

For a merger use the same endpoint-removal tree as (1.85)–(1.88). Adding one to the linear size changes the size-subadditivity defect by a fixed constant. The future extra cost up to the common eligible time is bounded by (H2S.7); the possible extra bounded number of growth steps and extra waiting interval have cost at most \(CR_j^{d+2}\). The source merger reserve, the \(2P_0\) term in (1.87), pays that changed fixed constant by the same strict inequality. Thus the induction closes. Choose the fixed fractions before the ceiling, retaining the desired smaller positive final tree rate. ∎

This proof does not require that every occupied step contain a new integral. The universal domain expression in (1.79) is explicitly applied by the source to the hypothetical sequence \(S^n(Q)\) in (1.80). Inserting an extra scalar cost at a frozen step is exactly the situation controlled by (H2S.7).

### Proposition H2S.2 — marked unnormalized unreplaced component

Let \(\mathfrak M_{k,Q}\) denote the real positive localized source contribution to which (1.79) applies, with the source self action and normalization factors retained. A bare \(T\) symbol stripped of those factors is not intended. Its actual hidden history is retained in this notation. For each fixed \(u\),
\[
 \mathfrak M_{k,Q}\!\left[e^{u\mathcal C_k(Q)}\right]
 \le \exp[-c_uP_0(g_k)-\kappa_u d_k(Q)]
 \tag{H2S.8}
\]
on the original real admissible retained-data support, for positive fixed \(c_u,\kappa_u\) and a sufficiently small common ceiling. The component history sums are included in this statement. Distinct current components have disjoint ancestral cost assignments.

**Proof.** Multiply each positive source summand by its field-independent geometric mark. The derivation of (1.79) is unchanged except for the added cost (H2S.5). Apply Lemma H2S.1 and the general-region conclusion after (1.89). The actual unmarked coefficient banks are still the source banks; there is no synthetic large marked boundary-action invariant in this argument. ∎

The same proof permits the fixed NR20 positive-energy insertion
\[
 e^{\theta\mathcal E_{k,Q}+u\mathcal C_k(Q)}.
 \tag{H2S.9}
\]
Here \(\mathcal E\) is the literal list of nonnegative energies still displayed in the operation, and \(\theta>0\) is sufficiently small and fixed. For a completed last-stage formula, the exact outer terms are
\[
 Q_X=\tfrac12\langle DH''_{1,k,X}B,\zeta DH''_{1,k,X}B\rangle,
 \qquad
 S_X=A((g'_k)^{-2}\zeta_1|_X,
       U''_{h+2}(\exp(i g_kB),V'')),
 \tag{H2S.9a}
\]
as in NR20.2, together with every still-present old Schur energy
\(q_{j,C}=\tfrac12a_C^{\mathsf T}S_{j,C}a_C\), NR20.3–4. For an earlier stopped operation use its actual surviving displayed positive forms, not a fictitious outer \(B\) variable. Each energy loses a fixed fraction once. The actual old normalized reference denominator is not changed. The added Gaussian rank cost is dominated by the same native domain cost, just as in NR20.6–NR20.10. The stronger preparatory inequality \(2p_1-(d+5)r_0>p_0\) and the strict \(P_0\gg CR^{d+2}\) budget persist with the changed constants.

The coefficient \((g'_k)^{-2}\) in (H2S.9a) is the actual inhomogeneous source coefficient. It is not replaced by the bare \(g_0^{-2}\). Already integrated fine Wilson energies are not restored as hidden positive exponents. In particular (H2S.9) does not estimate every transported bare plaquette insertion or the entire M03 regulator. The raw-mark conclusion in Section 6.1 below uses the companion original Wilson moments instead.

## 4. What the reserve pays before normalization

For a current unreplaced component \(Q\), let \(b(Q)\) be the oldest birth in its continuously unreplaced ancestry and set \(a(Q)=k-b(Q)\). At every outer scale between those endpoints at least one ancestor is occupied. For distinct current components,
\[
 \sum_{Q\in D}(a(Q)+1)
       \le c_*^{-1}\mathcal C_k(D).
 \tag{H2S.10}
\]
This uses the disjointness of their ancestor families. It does not sum the post-merger lifetime once for every historical tag.

For any fixed \(s>0\), take \(u\ge s/c_*\) in (H2S.8). Markov's inequality inside the **positive unnormalized integral** gives, for example,
\[
 \mathfrak M_{k,Q}
   [\mathbf1_{\{a(Q)\ge A\}}]
 \le e^{-sA}\exp[-c_uP_0(g_k)-\kappa_ud_k(Q)].
 \tag{H2S.11}
\]
Thus a subsequent enumeration of at most \(CL^{4A}\) possible fine roots per current unit can be paid by choosing \(s>4\log L\), with spare decay. The source history sum itself already performs its stated shape enumeration. This observation is not a second unrestricted sum over every old microscopic cell.

Full-tree size controls the number of occupied current \(M\)-cubes, up to fixed constants and an additive constant. Hence a small fixed factor \(e^{\lambda |Q|_k}\), or a fixed-thickness enlargement of that physical footprint, can also be retained in (H2S.8). The connected full-tree factor is essential; the analogous assertion for a selectively free completed hole would be false.

For polynomial insertions in the assigned energy, (H2S.9) gives
\[
 \mathfrak M_{k,Q}[\mathcal E_{k,Q}^{m}
                 e^{u\mathcal C_k(Q)}]
 \le m!\theta^{-m}
       e^{-cP_0(g_k)-\kappa d_k(Q)}.
 \tag{H2S.12}
\]
This does not identify an arbitrary transported physical source with that energy. In particular a raw \(a^{-4m}\) factor is not renamed a current-scale prefactor. Repeated physical-scale marks inside the same owner need their own matching, or a correspondingly stronger fixed age weight.

## 5. The full normalization: a finite-volume theorem

Let \(\mathcal Z_k(u)\) be the complete positive history integral with the mark \(e^{u\mathcal C_k}\), and with all history-dependent vacuum factors and every old/fresh normalizer unchanged. Then
\[
 \mathbb E_{\mathrm{full},k}e^{u\mathcal C_k}
          =\mathcal Z_k(u)/\mathcal Z_k(0).
 \tag{H2S.13}
\]

### Theorem H2S.3 — the global marked pressure bound

For fixed \(u\) at the ceiling in Proposition H2S.2,
\[
 \log\mathcal Z_k(u)\le E_+(u,g_k)V_k,
 \qquad
 \log\mathcal Z_k(0)\ge-E_-(g_k)V_k.
 \tag{H2S.14}
\]
Consequently (H2S.1) holds with \(C_u=E_+(u,g_k)+E_-(g_k)\), uniformly when the terminal coupling ranges over a fixed admitted compact weak interval.

**Proof.** The proof of the upper half of CMP119 Corollary 3, described after (2.49) and supplied by the general-region conclusion of LFR II p.387, uses the positive component majorants and their full-tree summation. By Proposition H2S.2 the marked majorants have the same form with fixed positive rates. Its final combinatorics and regular-sector bounds are therefore unchanged in form. Apply this upper majorant to the full positive integral, normalizing the compact Haar/axial-delta factors exactly as on LFR II p.383, to obtain the first inequality in (H2S.14). Where the chosen density convention has already performed those gauge integrations, this is simply integration of the printed upper density bound against Haar probability measure. We do not bound a retained gauge delta pointwise by one or assert domination of a gauge slice by ambient product Haar measure. This is an upper estimate on the original integral with a geometric insertion, not a change of the RG action or reference measure.

The printed lower bound (2.50) is also a **density** bound. In its all-regular sector it has the form
\[
 \rho_k(V)\ge\chi_k(V)
       \exp[-g_k^{-2}A(U'_k(V))-E_-(g_k)V_k].
 \tag{H2S.14a}
\]
Integrate it over the terminal Haar product ball \(|V(b)-1|\le c g_k\), with fixed sufficiently small \(c>0\). The source small-field/minimizer bounds put this whole ball in \(\{\chi_k=1\}\), and give \(|U'_k(V)(\partial p)-1|\le Cg_k\eta^2\) on the fine lattice. In four dimensions the plaquette count cancels \(\eta^4\), so
\(A(U'_k(V))\le Cg_k^2V_k\). Equivalently one can use the admitted smooth comparison field in the constrained variational principle. The product ball has Haar mass at least
\(\exp[-C(1+\log g_k^{-2})V_k]\), since it has at most \(dV_k\) independent terminal links and each compact-group ball has mass at least \(c_G(cg_k)^{\dim G}\). This proves the second inequality of (H2S.14), with its constant enlarged by these two explicit contributions. Division proves (H2S.1).

All volumes in this argument are the current/unit-lattice volume. This is the convention obtained from the native \(\Gamma_n\) counts in (2.45)–(2.49): in the all-regular sector only \(\Gamma_k\) remains. It is the \(T_\eta^{(k)}\) volume of the predecessor convention, not the number of microscopic \(\eta\)-vertices. The fine curvature/plaquette cancellation above is precisely what preserves that volume. ∎

For prescribed distinct current cores and an actual event which forces
\(\mathcal C_k(D)\ge T\), one therefore has the genuine normalized bound
\[
 \mathbb P_{\mathrm{full},k}(E_D)
          \le \exp(C_uV_k-uT).
 \tag{H2S.15}
\]
The factor \(\exp(C_uV_k)\) must remain. It is the difference between this theorem and a local H02 deletion estimate.

### 5.1 All fixed weights on one terminal weak band

There is an optional useful strengthening when the retained AF trajectory supplies a lower age envelope
\[
 g_{k-a}^{-2}\ge c\,g_k^{-2}+c'a-C.
 \tag{H2S.16}
\]
This is available at the B03/stopped-sequence scope. Fix the original terminal weak band once. For any larger fixed \(u\), choose an age \(A_u\) so that all grades \(j\le k-A_u\) lie below the smaller ceiling required by Lemma H2S.1. Apply the modified chronological estimate only at those older grades. At the remaining \(A_u\) grades, bound the mark deterministically by the entire lattice volume:
\[
 \sum_{j>k-A_u}\sum_Q c_j(Q)\le C(u)V_k.
 \tag{H2S.17}
\]
Indeed there are only \(A_u\) grades, their actual lattices contain \(V_kL^{d(k-j)}\) cells, and their rounded \(R_j\) and other fixed source constants are bounded on this finite age interval. Connected cube-count bounds control \(d'_j\) by the number of occupied coarse cubes; the extra component count is controlled by the same volume. Pull \(e^{uC(u)V_k}\) out of the integral and apply the previous upper argument to the older mark. The unmarked late induction spends no larger cost than the one already reserved.

Thus (H2S.1) holds for **each fixed** \(u<\infty\) on one terminal weak band, with a possibly very large \(C_u\). No fixed factorial growth in \(u\), derivative order, or source degree is asserted. This strengthening is unnecessary for ordinary fixed-cost tightness but can pay any prescribed finite age exponent at fixed physical volume.

### 5.2 The terminal-coupling size of the pressure constant

For each fixed \(u\), below the ceiling needed for that \(u\), the preceding proof gives the sharper bound
\[
 \log\mathbb E_{\mathrm{full},k}e^{u\mathcal C_k}
       \le C(u)(1+\ell_k)V_k,
 \qquad \ell_k=\log g_k^{-2}.
 \tag{H2S.30}
\]
The constant \(C(u)\) is independent of \(g_k\) below that ceiling. This rate is obtained by tracking the source proof, not from the bare statement of Corollary 3.

Indeed CMP119 (2.45)–(2.48) bounds the real \(E\), \(R\), and boundary actions by fixed constants times \(\sum_j|\Gamma_j|_j\). The paragraph preceding (2.49) gives the same bound for the non-logarithmic vacuum terms. These are the actual physical determining configurations; no assertion about an arbitrary independent-current extension is used. The remaining normalization logarithms have magnitude at most
\(C(1+\ell_j)|\Gamma_j|_j\), with fixed coordinate/group multiplicities. LFR II p.380 explicitly absorbs the old logarithms into
\[
 C\ell_j|Z_j|_j
       \le C M^dR_j^{d+1}(d'_j(Z_j)+1).
 \tag{H2S.31}
\]
Here \(\ell_j\le CR_j\), since the fixed radius exponent is greater than one. All older determining layers occur in these occupied domains. Their costs, including the mark, are paid by Section 3. The remaining terminal layer has \(|\Gamma_k|\le CV_k\) and contributes at most \(C(1+\ell_k)V_k\). If the normalization convention retains a future all-regular vacuum tail, its volumes decrease geometrically and the same coupling-profile comparison bounds it by this same expression.

The final connected-component count has fixed positive full-tree decay, so its logarithm is at most \(CV_k\), independent of the growing \(R_k\). The upper marked density/integral is therefore at most \(\exp[C(u)(1+\ell_k)V_k]\). The all-regular lower density has the same terminal logarithmic budget; integration on the \(c g_k\) Haar product ball in (H2S.14a) adds only \(C(1+\ell_k)V_k\). This proves (H2S.30). No inverse-coupling action cost remains on that ball: its action is \(O(g_k^2V_k)\) before multiplication by \(g_k^{-2}\).

Taking one fixed \(u>0\), Jensen and (H2S.3) give the genuine current bad-volume estimate
\[
 \frac1{V_k}\mathbb E|Z_k^{\mathrm{active}}|_k
   \le \frac{C(1+\ell_k)}{R_k}
   \le C\ell_k^{\,1-r_0}\longrightarrow0
       \quad(g_k\downarrow0).
 \tag{H2S.32}
\]
This estimate is uniform in volume and UV depth. It concerns the actual external large-field region, including retained second-class \(Y\)'s at their renewed births; it does not use the smaller prepared determining complement.

There is also a uniform pointwise version with the actual grid symmetry. The AF upper profile gives
\(R_{k-a}/R_k\le C(1+a)^c\) for fixed constants. Hence
\[
 \sup_{a\ge0} L^{-a}R_{k-a}/R_k<\infty.
 \tag{H2S.33}
\]
All past grid sizes are powers of \(L\), times the fixed compatible source divisors. Their common period can therefore be chosen to satisfy
\(p_k\le CMR_kh_k\), while being divisible by every past partition size. Translations by this period preserve the actual chronological positive law. A common-period tile contains only a fixed number of current \(MR_k\)-blocks. The external region \(Z_k^{\mathrm{active}}\) is a union of those blocks: ordinary construction has this property, failed preparations retain the whole original component, and a retained \(Y\) is a whole original attempted component.

For a current cell \(x\), let \(B_x\) be its current \(MR_k\)-block and \(Q_x\) a common-period tile containing that block. Since membership is constant on \(B_x\),
\[
 \begin{aligned}
 \mathbb P(x\in Z_k^{\mathrm{active}})
 &=|B_x|_k^{-1}\mathbb E|Z_k^{\mathrm{active}}\cap B_x|_k\\
 &\le |B_x|_k^{-1}\mathbb E|Z_k^{\mathrm{active}}\cap Q_x|_k
 \le C\frac{1+\ell_k}{R_k}.
 \end{aligned}
 \tag{H2S.34}
\]
The last inequality uses tile translation symmetry and (H2S.32), with \(|Q_x|/|B_x|\le C\). This does not assume that arbitrary unit-cell translations preserve the complete grid. A fixed number of additional \(MR_k\) layers satisfies the same bound, either by its bounded-volume enlargement or by a finite union over neighboring blocks. Thus any fixed finite native stencil with such a fixed protective collar is regular with probability at least
\(1-C_{\mathrm{stencil}}(1+\ell_k)/R_k\).

This establishes positive probability for the actual regular sector at a sufficiently weak positive terminal coupling. It does not identify a terminal auxiliary fluctuation with the original physical observable, prove a joint exponential bound for many prescribed bad components, or remove the local comparison in Section 8.

### 5.3 A growing scale-dependent store with uniform pressure constants

The fixed-cost proof permits a stronger numerical choice without an uncontrolled constant \(C(u_k)\). The retained **full** LFR hierarchy already gives
\(p_1<p_0\) (LFR I p.183) and
\(2p_1-(d+5)r_0>p_0\) (LFR II p.383). Therefore
\(p_0>(d+5)r_0\), and in particular
\[
 p_0>(d+2)r_0,
 \qquad
 \varrho=p_0-(d+2)r_0>0.
 \tag{H2S.35}
\]
Thus (H2S.35) is already implied by the source inequalities retained for the completed LFR construction. It is the exponent form of the reserve \(P_0\gg R^{d+2}\) used in (1.81)–(1.88), not merely the weaker \(P_0\gg R^4\). No numerical cutoff, exponent, or step of the actual stopped trajectory is altered here. All real and analytic exponents were fixed before its common coupling ceiling. Write \(P_j=P_0(g_j)=A_0\ell_j^{p_0}\), and put
\[
 w_j=\delta\,\frac{P_j}{M^dR_j^{d+2}},
 \qquad
 \mathcal W_k=
   \sum_{j\le k}\sum_{Q\in\mathscr A_j(D_k)} w_jc_j(Q)
   =\delta\sum_{j,Q}\frac{P_j}{R_j}
                         (d'_j(Q)+1).
 \tag{H2S.36}
\]
The number \(\delta>0\) will be chosen sufficiently small, **once**, independently of depth, volume, \(g_k\), source degree and moment order.

#### The numerical comparison

Rounded-power bounds give \(w_j\asymp\delta\ell_j^{\varrho}\), with fixed constants including \(A_0,M,L\). For every \(n\ge j\), CMP119 (2.6) gives \(\ell_n\le\ell_j+2\log(1+\beta_0)\). Hence
\[
 w_n\le C_w w_j\quad(n\ge j),
 \qquad
 C_w^{-1}w_k\le w_j\quad(j\le k),
 \tag{H2S.37}
\]
uniformly through an arbitrarily long admitted run. This permits nonmonotone rounded radii and uses no unproved sign for the individual coupling increments.

#### The weighted chronological proof

For a no-new-bad run starting at \((j,Q)\), (H2S.4), (H2S.7), and (H2S.37) give
\[
 \sum_{n=j+1}^{j+K}w_n c_n(S^{n-j}Q)
 \le C_w w_j C M^dR_j^{d+2}(d'_j(Q)+1)
 \le C\delta P_j(d'_j(Q)+1).
 \tag{H2S.38}
\]
The charge at the initial grade has the same bound. This is the precise amount assigned to the weighted future store.

Keep three distinct parts of each source seed: a positive base component mass, the original unweighted future store, and the new weighted store. Ordinary birth seeds have the stronger \(P_j^2(d'_j+1)\) budget. At the selected common ceiling it pays (H2S.38) while keeping a fixed base mass and the unchanged unweighted store. A failed bounded preparation has a \(P_j\) seed; its unweighted cost is \(o(P_j)\), and (H2S.38) costs at most \(C\delta P_j\). The new retained second-class \(Y\) has the literal seed
\(\tau_j\le\exp[-2(1+\beta_0)^{-1}P_j]\); its bounded geometry gives the same division into positive fixed shares. Neither its old hidden energies nor its completed genealogy is marked again.

At a merger use the original endpoint-removal tree. The defect between the weighted future store of the union and the stores of its two parts is at most
\(Cw_{j+1}M^dR_{j+1}^{d+2}\le C\delta P_{j+1}\), by the same bounded-extra-growth and waiting argument in (1.87)–(1.88), with (H2S.37) over the future interval. The positive merger surplus of the retained base masses is a fixed multiple of \(P_{j+1}\). Choose \(\delta\) smaller than its required fraction, and also smaller than the fractions for the failed-preparation and retained-\(Y\) seeds. The unweighted original cost divided by \(P_j\) tends to zero by (H2S.35), so the same fixed ceiling pays that cost in every case.

This completes the chronological induction with fixed positive base and full-tree rates. Those rates do not deteriorate as \(w_k\) grows. In particular the final majorant used in Section 5.2 has fixed constants. Its regular and terminal-logarithmic factors are unchanged. We obtain
\[
 \boxed{\quad
 \log\mathbb E_{\mathrm{full},k}e^{\mathcal W_k}
       \le C(1+\ell_k)V_k .\quad}
 \tag{H2S.39}
\]
The constant in (H2S.39) is independent of every \(w_j\). This is not (H2S.30) with an unspecified \(C(w_k)\). Its proof uses fixed fractions of the actual source reserves. The same proof retains a sufficiently small fixed fraction of the displayed energies (H2S.9a), if desired; that fraction is fixed before \(\delta\).

#### Current bad volume and pointwise occupancy

Since the current term of \(\mathcal W_k\) controls \(w_kR_k|Z_k^{\mathrm{active}}|_k\), Jensen gives the sharper conclusion
\[
 \boxed{\quad
 \max\left\{
 \frac1{V_k}\mathbb E|Z_k^{\mathrm{active}}|_k,
 \ \sup_x\mathbb P(x\in Z_k^{\mathrm{active}})
 \right\}
 \le C\frac{(1+\ell_k)M^dR_k^{d+1}}{P_k}
 \le C\ell_k^{\,1+(d+1)r_0-p_0}.
 \quad}
 \tag{H2S.40}
\]
The pointwise conclusion uses the common-period/block argument of (H2S.33)–(H2S.34); a fixed number of protective \(MR_k\) layers obeys the same estimate. Because \(p_0>(d+2)r_0\) and \(r_0>1\), the right side tends to zero. All constants and the common ceiling are independent of volume and UV depth.

#### An explicit age penalty

Assume the retained lower age envelope (H2S.16). One ancestral component is occupied at every step of a continuously surviving lineage. Equations (H2S.36) and the rounded-power bounds imply
\[
 \mathcal W_k\ge
 c\sum_{a=0}^{A} \ell_{k-a}^{p_0-r_0}
 \ge c(A+1)[\log(Y_k+A)]^{p_0-r_0}
 \quad\hbox{on }E_{k,A},
\]
after a harmless adjustment for bounded initial ages. The second inequality follows by summing over \(A/2\le a\le A\) and using \(Y_{k-a}\ge cY_k+c'a-C\). Thus
\[
 \boxed{\quad
 \mathbb P(E_{k,A})
 \le\min\left\{1,
  \exp\bigl[C(1+\ell_k)V_k
       -c(A+1)(\log(Y_k+A))^{p_0-r_0}\bigr]\right\}.
 \quad}
 \tag{H2S.41}
\]
For distinct actual current components their ancestor families are disjoint. The same proof therefore retains the **sum** of their separate age penalties, together with a fixed share of their current footprint volumes, by splitting the available \(\mathcal W_k\) weight. It still carries the extensive pressure factor. It does not separately sum the post-merger ages of all original tags or infer a local conditional probability.

On a terminal compact weak band put \(t_0=p_0-r_0>1\). The single explicit threshold
\[
 A_k=\left\lceil
       \frac{k\,\log\log(e^e+k)}{[\log(e+k)]^{t_0}}
      \right\rceil
 \tag{H2S.42}
\]
satisfies \(A_k\to\infty\), \(A_k/k\to0\), and
\(A_k[\log(Y_k+A_k)]^{t_0}\ge c k\log\log(e^e+k)\)
for large \(k\). Along the accepted \(V_k=o(k)\) sequence, (H2S.41) consequently decays faster than \(e^{-Dk}\) for every fixed \(D\). This stronger conclusion replaces the optional unspecified diagonal threshold by an explicit one.

## 6. Fixed-volume tightness of the active unreplaced skeleton

Fix a physical torus and a terminal physical lattice scale, and consider the admitted UV sequence. Reindex all old scales by age \(a=k-j\). The number of terminal cells \(V_k\) is then fixed. Equation (H2S.1) gives
\[
 \sup_k\mathbb P(\mathcal C_k>M)
       \le e^{C_uV_k-uM}\longrightarrow0.
 \tag{H2S.18}
\]

On \(\{\mathcal C_k\le M\}\):

1. Every currently unreplaced component has age at most \(M/c_*\), by (H2S.10).
2. The total number of actual occupied native cells and component records is bounded by \(CM\), by (H2S.3) and the occupied charge.
3. On that finite age interval the AF upper profile bounds the numerical coupling/cutoff parameters. Hence the number of preparation substeps and all possible discrete selector/geometry labels are finite. Their number may depend badly on \(M\), which is harmless for compactness.
4. The current torus and every one of these finitely many grids are finite. There are therefore finitely many allowed active geometries and incidence patterns. A connected order which counts actual components, births or actual preparation records is bounded. This is not a bound on the order of a signed cluster expansion or on all forgotten archives.
5. The retained group variables lie in finite products of the compact gauge group. The surviving real adjoint variables have their original finite cutoff bounds on these finitely many grades. Alternatively the energy insertion (H2S.9), with positive native precision on each of the finitely many geometries, gives compact Euclidean sublevels.

Consequently the laws of the **active unreplaced skeleton and its actual retained variables** are tight in the age-indexed, label-decorated ambient state space. Compact sublevels use the closure of each admitted finite chart with its discrete label retained. A diagonal subsequence exists.

This is a state-space tightness statement. A limit can reach a hard cutoff surface, and rounding labels can have one-sided limits. The argument does not identify the limiting label with a newly recomputed strict selector, prove continuity of a conditional kernel there, or pass the complete recursion through that limit. Nor does it make the forgotten completed archives tight. Those are separate matching and full-history questions.

### 6.1 Very old unreplaced sectors vanish even with bare physical insertions

This is a consequence for actual primitive observables, not merely for history geometry. Let \(a_k=h_kL^{-k}\), where the terminal physical spacing \(h_k=h\) is fixed. Use the actual energy-normalized bare bilinears of the F01 prescription, Section 3.7–3.9,
\[
 O_{\alpha,a}(x)=a^{-4}\beta_W\operatorname{Tr}(C_A C_B),
 \qquad
 \|O_{\alpha,a}(x)\|_p\le Ca^{-4}p.
 \tag{H2S.24}
\]
The coefficient \(\beta_W\), parallel transports and bare plaquette stencil in this formula remain the original ones. The exact positive history lift preserves its original Wilson marginal. No current-scale field has been substituted in (H2S.24). Known bounded finite tensor coefficients can be retained; an unknown physical normalization or running mixing coefficient is not included in its constant.

Let
\[
 E_{k,A}=\{\text{some current unreplaced component has }a(Q)\ge A\}.
\]
Equations (H2S.1) and (H2S.10) give
\[
 p_{k,A}:=\mathbb P(E_{k,A})
       \le \min\{1,\exp(C_uV_k-u c_*A)\}.
 \tag{H2S.25}
\]
This is a full-law event estimate, including overlap and the actual number of surviving cores. It is not a sum over hypothetical fine birth sites.

For any actual source-free history cut \(\mathcal G\), any fixed \(m\), and any fixed \(q\ge1\), conditional Jensen followed by Hölder gives
\[
 \begin{aligned}
 \left\|\mathbb E\!\left[
    \mathbf1_{E_{k,A}}\prod_{i=1}^mO_{\alpha_i,a}(x_i)
       \mid\mathcal G\right]\right\|_q
 &\le \left\|\mathbf1_{E_{k,A}}
               \prod_{i=1}^mO_{\alpha_i,a}(x_i)\right\|_q\\
 &\le p_{k,A}^{1/(2q)}
         \prod_{i=1}^m\|O_{\alpha_i,a}(x_i)\|_{2mq}\\
 &\le (Cmq)^m a^{-4m}p_{k,A}^{1/(2q)}.
 \end{aligned}
 \tag{H2S.26}
\]
The event can depend on later history variables; the first line is a conditional expectation on the complete positive coupling. It need not be measurable at the earlier cut \(\mathcal G\).

Take \(A\ge\varepsilon k\), with fixed \(\varepsilon>0\), and choose a fixed
\(u>8mq\log L/(c_*\varepsilon)\). Using the same terminal band through Section 5.1, (H2S.26) is bounded by
\[
 (Cmq)^m h^{-4m}
 \exp\!\left[
    \frac{C_u}{2q}V_k-
       \left(\frac{u c_*\varepsilon}{2q}-4m\log L\right)k
 \right].
 \tag{H2S.27}
\]
It tends to zero exponentially in \(k\) at fixed terminal volume. It also tends to zero on the **same** slow-volume stopped Wilson sequence of the continuation, for example \(V_k=O(k^\vartheta)\) with fixed \(0<\vartheta<1\). Each fixed \(m,q,u\) has a finite \(C_u\), so \(C_uV_k=o(k)\); the terminal weak band and the sequence are not changed with the observable degree. This proves negligibility of the very old continuously unreplaced sector in every fixed transported \(L^q\) product norm at any source-free cut.

The corresponding rare conditional-cumulant statement is also direct. With \(Q=\mathbb E[\,\cdot\mid\mathcal G]\), every term in the partition formula for
\(\kappa_Q(\mathbf1_E,O_1,\ldots,O_m)\) is bounded by
\[
 (Q\mathbf1_E)^{1/2}
       \prod_{i=1}^m(Q|O_i|^{2m})^{1/(2m)}.
\]
The block containing \(\mathbf1_E\) uses conditional Hölder with exponent two on that factor and exponent \(2m\) on its other entries. Other blocks use the same exponents and a factor one. Ordinary Hölder then gives
\[
 \|\kappa_Q(\mathbf1_E,O_1,\ldots,O_m)\|_q
 \le (m+1)!2^m\,\mathbb P(E)^{1/(2q)}
          \prod_{i=1}^m\|O_i\|_{2mq}.
 \tag{H2S.28}
\]
The displayed coefficient is the standard sum of absolute ordered-partition coefficients. Thus these genuine source-free rare-event cumulant coefficients also vanish on the sequence in (H2S.27). When \(E\) is measurable at the cut, the analogous estimate for \(\mathbf1_E\kappa_Q(O_1,\ldots,O_m)\) follows by the same argument. No derivative of a moving hard selector is being inserted.

One may choose a single slower threshold \(A_k=\varepsilon_k k\), with \(\varepsilon_k\downarrow0\) and \(A_k\to\infty\), by a deterministic diagonal construction. For integer \(\ell\), set \(\varepsilon_\ell=1/\ell\) and choose \(u_\ell\) large enough for all \(m,q\le\ell\), for instance of order \(\ell^3\). Choose the next depth threshold so that the \(C_{u_\ell}V_k\) term is smaller than a fixed half of the negative exponent for all subsequent depths, and also \(k\ge\ell^2\). Keep \(\varepsilon_k=1/\ell\) until the next threshold. This produces one sequence and one threshold for which every fixed product and cumulant estimate above tends to zero. No uniform factorial bound in the varying \(u_\ell\) or in all source orders is inferred.

The weighted store of Section 5.3 gives an explicit, stronger replacement. Insert (H2S.41) with (H2S.42) into (H2S.26) and (H2S.28). For every fixed \(m,q\), the resulting exponent is bounded by
\[
 4m k\log L+\frac{C(1+\ell_k)}{2q}V_k
       -\frac{c}{2q}k\log\log(e^e+k)
       \longrightarrow-\infty.
 \tag{H2S.43}
\]
This proves the vanishing of the sector \(E_{k,A_k}\) for **all fixed orders and fixed moment exponents on one sequence and one explicit threshold**, with the same fixed source ceiling. The estimate remains an all-fixed-order statement; it does not assert an order-uniform M03 norm or bounds on unspecified renormalization coefficients.

For each fixed finite collection, the normalized moment difference between the original law and its restriction to \(E_{k,A}^c\) is bounded by the rare product expectation plus \(\mathbb P(E_{k,A})\) times the unrestricted moment, divided by \(1-\mathbb P(E_{k,A})\). Both terms vanish by the same estimates. Fixed-order cumulant differences follow from their finite partition formulas. This is a comparison of moments of the original Wilson sequence. It does not assert reflection positivity of the conditioned laws.

The remaining sector can still have ages tending to infinity below this threshold. Controlling its current-scale local fields and its complete physical carriers requires the regular transport/matching and local history estimates. The conclusion here is a strictly identified part of H02, not its completion.

## 7. Translation-averaged local information

There is an additive lower cost suited to spatial averaging:
\[
 \mathcal V_k=\sum_{j\le k}R_j
        |Z_j^{\mathrm{active}}|_j\le C\mathcal C_k.
 \tag{H2S.19}
\]
Assign each actual fine cell to its containing terminal cell (or to a fixed common-period terminal tile) and put its positive contribution there. This defines a positive local cost measure whose total mass is \(\mathcal V_k\).

Jensen's inequality and (H2S.1) yield
\[
 \mathbb E\mathcal C_k\le C_uV_k/u.
 \tag{H2S.20}
\]
If the actual history law is invariant under a group of translations transitive on the chosen common-period tiles, then every such tile has expected assigned cost bounded by a fixed constant times its volume. The same conclusion holds for the spatially averaged local cost without any invariance assumption. No extra translation symmetry of a fixed grid origin is assumed. On the source-compatible cubic sequence, one can use its common physical grid period rather than pretend that every unit translation preserves every old partition.

For a compact union \(K\) of such tiles this gives
\[
 \mathbb P\bigl(\mathcal V_k(K)>M\bigr)
       \le C|K|/M.
 \tag{H2S.21}
\]
Thus the additive cost measures are locally tight. Anchoring each **current** unreplaced component once, translation averaging and (H2S.10) also give
\[
 \frac1{V_k}\mathbb E\#\{Q:\ a(Q)\ge A\}
       \le C/A.
 \tag{H2S.22}
\]
There is no union bound over all possible old fine locations in this argument: it counts the actual surviving components.

These first-moment statements do not imply local exponential moments. They also do not prove tightness of the **entire carrier of every component touching \(K\)**: a connected component can extend very far from \(K\), with most of its cost charged elsewhere. Absence of percolation, local carrier-diameter tails, and local marked cumulants require more than (H2S.20). Ages of all original tags after mergers are not summed by (H2S.22).

## 8. The remaining normalized deletion/gluing theorem

For a volume-uniform local H02 estimate one needs a comparison inside the same complete positive law. A sufficient statement is the following actual ratio, with the exact input variables and integration domains displayed:
\[
 \int N_D(v)\,d\lambda_{\mathrm{out}}(v)
 \le e^{-\mathsf{Cost}(D)}
       \int G_D(v)\,d\lambda_{\mathrm{out}}(v),
 \qquad
 \int G_D\,d\lambda_{\mathrm{out}}\le\mathcal Z_k(0).
 \tag{H2S.23}
\]
Here \(N_D\) is the selected-component numerator, with the proposed insertion; \(G_D\) must be an actual admissible deleted/filled sub-sum of the **same** full denominator. Every altered coarse datum and every variable whose old selector forced the bad event must be integrated or carried through the stated change of variables. The comparison must include its multiplicity, Jacobian/coarea factors, action difference, boundary collar, and the exact history-dependent normalizers.

The small source norm \(\mathfrak M_{k,Q}1\) alone is not (H2S.23). If the retained data already force a bad label, the putative empty sector can have zero weight and the small common mass cancels in its posterior. The completed successful-component deletion in H03 has an actual empty state on its common admitted reference support. The corresponding empty state has not been established for an arbitrary unreplaced component with its retained coarse data fixed.

C05 compares the admitted analytic charts and controls the moving normalized operation on those charts. It does not construct a filling of a deleted large component whose retained data lie outside them. The global ratio in Section 5 is valid precisely because it divides by the actual global lower partition-function bound; that operation leaves the extensive factor in (H2S.15).

## 9. Preparation failures and the selector boundary

The source gives an exact distinction relevant to any future attempt at (H2S.23). LFR I p.182, (1.25), states that \(\chi_k^{(n+1)}\) does not depend on the variables in the next integral. Its failure is a retained-data event on that conditional fiber. By contrast \(\chi'_j\) in (1.27), and the extra adjoint cutoff in (1.28), are inserted **under** that integral.

Only the latter are candidates for a fresh conditional fluctuation estimate. Even there one must verify the entire compact \(V_j\) comparison domain, a common regular reference ball, the real constrained minimum, and the retained exterior force. The product-support C08 theorem on regular current coordinates does not establish those facts for an arbitrary old compact-group fiber. A Gaussian tail after conditioning on a failure would be invalid.

There is nevertheless a useful exact cancellation at the full physical level. Before component integration, LFR I p.193 says the preparatory partitions preserve the density pointwise. The integration on p.194 and reversed Faddeev–Popov operation in LFR II p.378 give equivalence only after the stated variables are integrated. If every branch is pulled back to the **same original raw variables** and carries the same physical observable/source, the complete partition is an identity. Differentiating that identity distributionally produces no net hard-selector boundary term. At finite lattice volume the original compact Wilson integral can instead be differentiated directly; its ordinary normalized score formula retains the full denominator.

This does not assert cancellation for a selected subset of histories, a history-dependent component mark, or a native direction which means different raw perturbations in different branches. For a single two-way split the boundary defect is proportional to the difference of the two pulled-back branch traces. It vanishes for the identical physical integrand; it need not vanish for the marked history kernel. Nor does this qualitative cancellation supply a uniform local bound on the summed physical source jets.

## 10. Exact application boundary

The new conclusions are:

* a marked unnormalized unreplaced-component estimate with the actual occupied outer-step charge;
* a full-normalization finite-volume exponential moment of active survival cost;
* the fixed-fraction weighted pressure bound (H2S.39), explicit age tail (H2S.41), and pointwise current bad-volume estimate (H2S.40);
* UV-uniform tightness of the finite-torus active unreplaced skeleton;
* translation-averaged local first moments and local tightness of the associated positive cost measures;
* vanishing of the explicit old-age sector (H2S.42) in every fixed raw transported product or rare-cumulant norm, without replacing the bare insertion by a current stencil.

The unresolved local H02 problem is (H2S.23), together with current-scale matching of the physical insertions and the required carrier/response topology. The stated M03 norm takes a supremum over all moments; exponential rarity by itself cannot pay its fixed exponential physical-carrier weight. Neither the global estimate nor the exact full-partition selector cancellation changes that norm. No completion of H02, M04, the full interacting continuum construction, or Yang–Mills existence is claimed here.
