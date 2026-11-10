# The actual continuous core and two-outer-energy component reserve

**Annex BC.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


This annex separates three costs that are easily combined too pessimistically: the physical support of the continuously integrated variables after preparation, the retained-data footprint of their normalized law, and the full footprint of an unnormalized successful-component activity. These are different sets and different estimates.

### 1. The unchanged strong norm

The M-03 norm uses the actual ambient retained variables, the native regulator

\[
 R_{h,X}=1+\sum_{p:\,\operatorname{foot}(p)\subset X}\beta_p s(V_p)
                +\sum_{i:\,\operatorname{foot}(i)\subset X}|z_i|^2,
 \qquad
 w_h(X)=e^{\kappa(|X|+\mathsf t_h(X))}.
 \tag{RN19.1}
\]

Its value envelope takes a supremum over elementary shifted retained states. Its difference/current envelope sums all corresponding finite-difference suprema, including discrete history changes. The pointwise part divides by a power of the shifted **output** native regulator. The input regulator cannot be retained after its variables have been erased unless a genuine pullback inequality proves the comparison.

The results below do not change these requirements. A pointwise estimate for an unnormalized marked numerator is useful because its small mass can pay an exponential footprint weight. Dividing by that same mass generally loses this payment. Conversely, jointly summing a successful geometry with its mass before normalization can retain the payment; a precise deletion lemma appears in Section 6.

### 2. The continuously integrated core is smaller than the eligible component

An eligible component X in LFR I printed p.177 has diameter at most 100 M R_k in current units. That is not the size of the final replacement integration domain.

#### Proposition RN19.1 — the final continuous core

After the successful preparatory steps of the literal primary operation, the physical support of the remaining continuously integrated coordinates in that component is contained in a fixed current-block enlargement C of the final domain Lambda, with

\[
 \operatorname{diam}_h C\le C_d\,100M,
 \qquad |C|_h\le C_d(100M)^d.
 \tag{RN19.2}
\]

The statement concerns support in physical current blocks. It does not bound the number of old-scale coordinates located in those blocks. It also does not assert that a remaining history label or the retained-data dependence of the kernel has the same footprint.

**Proof.** LFR I printed p.192 defines Lambda in (1.73) by adding one current M-layer to the prepared domain Z'_k. The text explicitly states that Lambda is a rectangular parallelepiped contained in a cube of side 100M and that it is the domain on which the field variables are integrated. The subsequent integrations must still be checked, rather than identified with the fresh reference denominator.

The first integral in (1.76), printed p.194, is over the older region Z_h and is left unchanged while the second integral is prepared. The nested prepared domains described in (1.10)–(1.12), and displayed again immediately before the gauge construction on p.195, give

\[
 \Lambda\supset Z'_k\supset\cdots\supset Z'_{h+1}
       \supset (\Omega''_{h+1})^c\cap X
       \supset Z_h\cap X.
 \tag{RN19.3}
\]

Here h=k−N is the source's older step index, not the physical spacing used in (RN19.1). The last inclusion uses the ordinary nesting of the next small-field domain inside the current small-field domain. The old operation T_h is localized in Z_h, as in CMP119 (2.19)–(2.21); its integrated coordinates are thus in the last set in (RN19.3).

The other remaining coordinates are the relative fluctuation on

\[
 B_0=\mathcal B'_k\cap\Lambda\cap\Omega''_{h+1},
 \tag{RN19.4}
\]

as specified by LFR I (1.81), printed p.195. The exact final operations LFR I (1.100) and LFR II (1.71), pp.378–379, retain these B coordinates, T_h and a V_h integral on the complementary older region with its displayed fixed old-scale collar. In particular, the final V_h domain is written using the enlarged complement of Omega''_(h+1), not merely the uncollared complement displayed in (RN19.3). LFR I p.195 identifies this older domain with the prepared Z'_h layers; p.199 describes the corresponding boundary layer of thickness 2 M_1 in the h-scale. Its physical thickness is bounded by a fixed number of current blocks because the h-scale is finer than the current scale. Include that collar, the bonds crossing its boundary and the prescribed gauge graphs in C. Then C lies in a fixed enlargement of the 100M cube. No claim that the final collar is literally contained in the unmodified Lambda is needed. Counting the current blocks of this enlarged fixed cube proves (RN19.2). The locality assertion here is for the raw integration coordinates after the stated preparatory operations; reconstructing a fine background from them can have additional retained-data dependence. ∎

The same small-domain fact is independently visible in the fresh denominator argument: LFR II printed pp.357–358 gives (1.8) with the fixed constant d(100M)^(d+1). That denominator argument alone would not identify the old posterior. Proposition RN19.1 instead follows every remaining continuous integration in (1.71).

#### Lemma RN19.2 — joining input carriers through the continuous core

Let S_1,...,S_l be actual input carriers, each meeting the fixed continuous core C of Proposition RN19.1, enlarged once to a connected current-block cover if necessary. Its cardinality and tree length retain the fixed bounds in (RN19.2). Then

\[
 w_h\left(C\cup\bigcup_{j=1}^l S_j\right)
       \le w_h(C)\prod_{j=1}^l w_h(S_j),
 \qquad w_h(C)\le C_{M,d,\kappa}.
 \tag{RN19.5}
\]

**Proof.** Join a shortest tree of each S_j to the fixed tree of C at a point of intersection. The resulting union is connected, has at most the sum of the cardinalities and tree lengths, and contains the required set. Exponentiate the resulting two subadditivity inequalities. ∎

For a fixed geometry and retained datum, a cumulant of order at least two vanishes if one of its arguments is independent of every integrated variable. Hence a genuinely generated cumulant of inputs independent of integrated history labels must have every participating input carrier meet the continuous core. Formula (RN19.5) pays the connector needed for those inputs with a fixed factor. It does not pay additional retained-data dependence of the normalized kernel.

In particular, assigning an arbitrary old core correlation the diameter 100MR_k solely because X has that diameter is unnecessarily pessimistic after the successful preparations. **It is still invalid to replace the full kernel carrier by C without proving its retained-data and history-label locality.** The actual native-variation connection set printed on LFR II p.379 is B_0 union (Gamma''_k intersect X-tilde), with subscript k. Its second set contains current determining variables throughout the component and is not an old h-scale core. Annex BB, equation (MG19.17),, records the underlying size distinction explicitly.

### 3. An exponential reserve for two actual outer energies

Write T'_k(X;U) for the real positive unnormalized operation in LFR II (1.71). Use exactly its old integration variables, selectors, coarea factors and normalization constants. Among its displayed exponent terms are two nonnegative real functions:

\[
 \begin{split}
 Q_X&=\tfrac12\langle D H''_{1,k,X}B,\,\zeta D H''_{1,k,X}B\rangle,\\
 S_X&=A\!\left((g'_k)^{-2}\zeta_1|_X,
        U''_{h+2}(\exp(i g_k B),V'')\right),\qquad
 \mathcal E_X=Q_X+S_X.
 \end{split}
 \tag{RN19.6}
\]

The notation is the source's notation in (1.71); S_X is the localized Wilson action with its actual nonnegative coupling weight. Q_X is nonnegative because the real cutoff zeta is nonnegative. These are the **two displayed outer energies**. They are not defined to be the full M-03 regulator and do not silently include every older free coordinate.

#### Proposition RN19.3 — fractional-action reserve on the admitted source class

Fix theta_0=1/4. The source parameter order and one sufficiently small common coupling ceiling can be chosen so that, uniformly over the literal admitted eligible operations and their real native backgrounds,

\[
 T'_k(X;U)\bigl(e^{\theta_0\mathcal E_X}\bigr)
       \le e^{-P_0(g_k)},
 \qquad P_0(g)=p_0(g)\text{ in LFR II}.
 \tag{RN19.7}
\]

This is an unnormalized estimate. No lower bound for T'_k(X;U)1 is asserted.

**Proof and source-parameter check.** Multiplication by the exponential in (RN19.7) replaces the coefficients of precisely Q_X and S_X in (1.71) by 3/4. It leaves every cutoff, domain, older operation, field coordinate and normalizing determinant unchanged. In particular, this is an insertion in the original operation; it is not a replacement of the original measure by a newly chosen renormalized trajectory.

There is no hidden change to an older normalized reference operation. CMP119 (2.19)–(2.21), printed p.258, represents T_h as the ordered product of localized positive integrations with their existing characteristic functions, Gaussian forms, renormalization delta constraints and gauge-fixing factors. The source states that an earlier R operation preserves that general form, with its altered characteristic functions and possibly empty fluctuation domain. Those old forms and their normalization factors are left exactly as they occur in the baseline T_h. Any already completed old scalar factor is likewise unchanged. The insertion multiplies only the two displayed outer exponent terms of LFR II (1.71); it neither redefines the old kernels nor invokes a bound for an old normalized kernel with a new reference action. The extraction below is performed on this single unchanged positive integral with the two outer coefficients reduced.

The real extraction proof in LFR II pp.380–383 uses lower bounds for the positive Wilson and quadratic forms to extract the factors associated with old and preparatory large-field selectors. Multiplying either relevant positive form by a number in [3/4,1] reduces the corresponding extraction coefficient by at most 3/4. Nonlinear comparison errors and bounded action terms are treated by the same absolute upper bounds as in that proof. They can be absorbed by reducing the fixed positive lower coefficient once more, for example to gamma_* = gamma_0/2, and enlarging a fixed constant C_* in the positive domain cost.

For clarity, the resulting upper bound has exactly the structure of the printed (1.79):

\[
 \begin{split}
 \sup_{\text{admitted histories}}\;&
 \exp\left\{C_*\sum_{j\le k}M^dR_j^{d+1}d'_j(Z_j)\right\}\\
 &\times\prod_{\text{new bad components at }j}
 \exp\left\{-\tfrac12\gamma_* A_1^2P_0(g_j)^2
                  [d'_j(Z^{(i)}_j)+1]-2P_0(g_j)\right\}\\
 &\times\prod_{\text{preparatory failures at }j}e^{-P_0(g_j)}.
 \end{split}
 \tag{RN19.8}
\]

The full primary operation sums the admissible histories before this supremum bound is taken. The source's counting and Gaussian volume factors are already included in the first exponential. No additional count of all microscopic bonds of the torus is introduced.

The coefficient reduction is harmless for the preparatory factors as well. For the worst such factor the source proves, on printed p.383, a bound of the form

\[
 e^{-c R_j^{-(d+5)}p_1(g_j)^2},
 \qquad 2p_1-(d+5)r_0>p_0.
 \tag{RN19.9}
\]

Replacing c by a fixed positive smaller constant still gives e^{-P_0(g_j)} at one smaller ceiling. The other preparatory factors have stronger bounds. The initial bad-field extraction has a term of order P_0^2, so the fixed store 2P_0 in (RN19.8) also remains available after reducing its quadratic coefficient.

The treatment of integration volumes is particularly important. Let d_G be the Lie-group dimension and let n_B be the number of free B bonds after removing the displayed axial tree. The last line of (1.71) contains exactly

\[
 \left[-\tfrac12d_G\log g_k^{-2}+\log\sigma_0\right]n_B,
 \qquad
 e^{[-\frac12d_G\log g_k^{-2}+\log\sigma_0]n_B}
       =(\sigma_0g_k^{d_G})^{n_B}.
 \tag{RN19.8a}
\]

Combined with dB times sigma(g_k B), this is the Haar-coordinate Jacobian under B'=g_k B on the retained small exponential chart. The tree delta removes exactly the tree coordinates, so the factor counts the free coordinates. As stated on printed p.383, the source includes this logarithmic factor in the integration measure, drops the remaining positive B quadratic to zero, and bounds the resulting restricted normalized compact measure by one. The same argument applies to 3Q_X/4. There is no coefficient-dependent Gaussian determinant to cancel for this outer B estimate, and no additional rank loss.

The older Gaussian forms in T_h are unchanged by the insertion. To quantify the maximal cost even if one uses a common fractional-action comparison when extracting old bad-field factors, let r_j be the actual rank of the Gaussian majorant charged to the j-scale volume in LFR II (1.79). These are the older fluctuation forms in CMP119 (2.21), or LFR I (1.25), with the indices relabeled to the volume convention of (1.79); in the original CMP119 convention A_j is integrated on Z_(j+1) intersect Omega_(j+1). Reducing a fixed positive coefficient by 3/4 changes the full Gaussian majorant integral by (4/3)^(r_j/2). This comparison is only an upper bound for the integral; it does not change the actual old kernel or its normalizer. The number of Lie coordinates gives

\[
 r_j\le C_{d,G,L}|Z_j\cap\Omega_j|_j
       \le C_{d,G,L}M^dR_j^d d'_j(Z_j),
 \tag{RN19.8b}
\]

where the volume in the first expression is at that old j-scale; the fixed L-dependent constant allows the one-step bond-count conversion in this relabeling. The second inequality is exactly the old-scale volume-to-component bound used on LFR II p.380 for its actual admissible enlarged Z_j and its own d'_j convention. It is not a claim for arbitrary sets with an unrelated diameter convention. Thus any such loss is bounded by
\(\exp[C\sum_jM^dR_j^d d'_j(Z_j)]\), which is absorbed by the existing positive cost in (RN19.8), since R_j>=1. This argument is valid for arbitrary old depth: it retains the complete scale-by-scale sum, and the chronological induction below pays it. It does not bound the number of old coordinates by the fixed current volume of Proposition RN19.1. The other compact group integrals are bounded by one as in the source. These facts account for every continuous integration class in (1.71).

Finally, the chronological induction (1.80)–(1.88) is an induction for this numerical structure with fixed positive extraction coefficient and fixed positive domain-cost constant. Its proof uses the strict source parameter separations. A sufficient way to state the resulting requirements is

\[
 \begin{split}
 &P_0(g)\gg C_* M^dR(g)^{d+2},\\
 &\gamma_* A_1^2 P_0(g)^2
      \gg P_0(g)+C_*M^dR(g)^{d+2},\\
 &c_*R(g)^{-(d+5)}p_1(g)^2\gg P_0(g).
 \end{split}
 \tag{RN19.10}
\]

All constants are fixed before the ceiling is chosen. These are the same strict power-order requirements used in the source proof; multiplying their constants by fixed numbers changes only the ceiling. In particular its choice N=R_j in (1.80) is retained. The induction therefore leaves the store 2P_0 of the earliest surviving bad component just as in (1.89), giving exp[-2(1+beta_0)^(-1)P_0(g_k)]. The weaker (RN19.7) follows for the admitted fixed beta_0<1, after taking the common ceiling small enough for the inequalities above. This supplies the claimed source-scoped insertion estimate. ∎

The proof depends on the source extraction and admissibility hypotheses exactly as the C-05 argument does. Independent verification of every numerical ceiling and the actual Wilson-normalized trajectory remains part of the base estimates. The useful new assertion is the explicitly identified fractional-action insertion (RN19.6), not an unproved claim that all native regulators are equivalent to it.

#### Corollary RN19.4 — polynomial moments with fixed factorial growth

For every integer m>=0,

\[
 T'_k(X;U)\bigl[(1+\mathcal E_X)^m\bigr]
 \le e^{\theta_0}\theta_0^{-m}m!\,e^{-P_0(g_k)}.
 \tag{RN19.11}
\]

**Proof.** For s>=0, s^m<=m! theta_0^(-m) exp(theta_0 s). Apply it to s=1+E_X and use (RN19.7). ∎

This argument preserves a fixed factorial budget. In contrast, replacing a compact marked field by a bound of order g^(-2m) and then paying it with exp[-c(log g^(-2))^q] produces a bound of order exp(C m^(q/(q−1))) after optimizing in g. That is not a fixed factorial-power estimate. Such a compact-supremum shortcut is not used here.

### 4. Every finite unnormalized source jet in the energy class

Let I have m labels. Suppose all incoming log-jet coefficients on a component satisfy the actual pointwise bound

\[
 |A_B(x,\eta)|\le C^{d+1}(d!)^s b^d r(x)^d
                   [1+\mathcal E_X(x,\eta)]^d,
 \qquad d=|B|,\quad s\ge1,\quad r(x)\ge1.
 \tag{RN19.12}
\]

The function r is retained data, fixed inside this operation. It is not automatically the output M-03 regulator. For independent scalar variables \(t_i\) indexed by I, put \(t_B=\prod_{i\in B}t_i\). Define the unnormalized jet by applying T'_k(X) to the finite formal exponential of sum \(t_BA_B\). The coefficient selected by \(\partial_I=\prod_{i\in I}\partial_{t_i}\) is therefore the usual labeled partition sum; \(t_B\) is not an additional independent source coordinate.

#### Theorem RN19.5 — unnormalized full-jet coefficient bound

For every m>=1,

\[
 \left|\partial_I T'_k(X)
        \exp\!\left(\sum_{B\ne\varnothing}t_BA_B\right)\bigg|_{t=0}\right|
 \le e^{-P_0(g_k)} C_1^m(m!)^{s+1} b^m r(x)^m.
 \tag{RN19.13}
\]

The result is compatible under truncation in source order. It requires no convergent exponential-source series.

**Proof.** The coefficient is the sum over partitions of I of T'_k(X) applied to the product of the corresponding A_B. Its total power of 1+E_X is m. By (RN19.11), that integral costs at most C^m m! exp(-P_0). For a fixed number l of blocks, order them and sum their positive sizes d_1+...+d_l=m. Since s>=1,

\[
 \sum_{\substack{\pi\in\Pi(I)\\|\pi|=l}}
       \prod_{B\in\pi}(|B|!)^s
 \le \frac{(m!)^s}{l!}\binom{m-1}{l-1}.
 \tag{RN19.14}
\]

The remaining sum over l, including C^l, is at most (1+C)^m. This proves (RN19.13). All operations are in the finite source algebra, so lower-order truncation gives the same coefficient. ∎

If a common native chart is used and the complete input coefficient is frozen as a function of the old integration variables at a real chart center, the primary small exponential tilt in LFR II (1.73) bounds the complex unnormalized integral by a fixed multiple of its real absolute integral. Formula (RN19.13) therefore holds on that native disc for this kernel response. Native derivatives of order j cost j! rho^(-j), where j is distinct from the source order m; finite-difference suprema within the inner half-disc cost the corresponding first-derivative radius. Direct changes of the incoming coefficients require their own transported input records. This assertion does not include arbitrary raw retained-coordinate pullbacks or a moving selector support.

There is also a useful quantified polynomial loss rule. Write P_0(g)=ell(g)^(p_0) and R(g)<=C ell(g)^(r_0), with the source's fixed exponents. For any fixed u>=0 and a>0,

\[
 \sup_g R(g)^{um}e^{-aP_0(g)}
       \le C_{a,u}^m(m!)^{ur_0/p_0}.
 \tag{RN19.15}
\]

Indeed set v=P_0(g) and maximize v^(ur_0 m/p_0) exp(-a v). Thus a *proved polynomial* regulator comparison in R could be absorbed at a fixed additional factorial power while retaining part of the component mass. A factor exponential in ell times m does not obey this conclusion.

### 5. Paying the full footprint for unnormalized successful components

For the source-native operation all expressions in (1.71) are localized in X, with the stated fixed collars included. Let X^+ be that actual source-native footprint. Since X lies in a cube of side 100MR_k,

\[
 |X^+|_h+\mathsf t_h(X^+)\le C_M(1+R_k)^d.
 \tag{RN19.16}
\]

The number of possible such current-block sets containing one fixed anchor is at most exp[C_M(1+R_k)^d]. This deliberately crude bound follows by choosing a containing cube, then a subset of its blocks. It bounds the allowed eligible shapes without replacing a more refined source count by an unjustified smaller count.

Because P_0(g_k)/R_k^d tends to infinity under the source parameter order, one can retain a fixed fraction of (RN19.13) and obtain

\[
 \sup_a\sum_{X^+\ni a}w_h(X^+)
        e^{-P_0(g_k)/2}
       \le C e^{-P_0(g_k)/4}.
 \tag{RN19.17}
\]

This is a full physical footprint bound for these **unnormalized** component contributions. It is the same type of payment used in the source's (1.92)–(1.97). Printed p.389 explicitly combines the component mass with exp[2 kappa (100R_k)^d], using

\[
 -2(1+\beta_0)^{-1}P_0(g_k)+1+2\kappa(100R_k)^d
       \le-\tfrac32P_0(g_k).
 \tag{RN19.18}
\]

The weakened reserve needed in (RN19.17) merely asks for another fixed part of that strict separation. No mass that has already canceled in a conditional ratio is used.

Equations (RN19.13), (RN19.15) and (RN19.17) therefore give a fixed-factorial, fully weighted unnormalized bound for actual successful-component jets in the stated outer-energy class. They do not identify the entire M-03 regulator with that energy, do not bound the normalized fixed-component posterior, and do not control all retained-coordinate currents.

### 6. A positive normalization lemma for joint successful-geometry erasure

The following precise lemma identifies one way the component payment can survive a normalization. Its geometric hypotheses must be checked in the actual representation before applying it.

Let C range over admissible finite families of compatible components. Suppose the family is closed under deletion. Let M_X be a positive finite measure for the internal variables of X, and write

\[
 Z=\sum_{C\text{ admissible}}\int e^{H_C(\eta_C)}
                              \prod_{X\in C}M_X(d\eta_X)>0.
 \tag{RN19.19}
\]

Retained data are fixed here. For a fixed required family S, assume that removing S from any C containing it gives the same remaining measures and coordinates, and that on their common physical support

\[
 H_{D\cup S}(\eta_D,\eta_S)-H_D(\eta_D)
       \le\sum_{X\in S}\lambda_X.
 \tag{RN19.20}
\]

#### Lemma RN19.6 — normalized deletion estimate with marked masses retained

For nonnegative component functions F_X,

\[
 \mathbb E\left[\mathbf1_{\{S\subset C\}}
                   \prod_{X\in S}F_X(\eta_X)\right]
 \le e^{\sum_{X\in S}\lambda_X}
              \prod_{X\in S}M_X(F_X).
 \tag{RN19.21}
\]

**Proof.** In the numerator use (RN19.20) and perform the S-integrals. The remaining sum is over those D for which D union S is admissible. By deletion closure those D form a subfamily of the families summed in Z, with exactly the same positive summands. Their sum is at most Z. Divide by Z. ∎

No comparison of partition functions on different tori is required. The proof does not divide by M_X(1). It is therefore compatible with the unnormalized marked reserve of Section 5. If cross interactions have a common geometry-local representation and a uniform absolute incidence sum, that sum supplies the lambda_X in (RN19.20).

For the source's successful X-sector, the factorized form (1.72), exact localization of V(Y) and the mass estimate make this a concrete application to investigate. It is not enough merely to observe a scalar cluster bound: one must verify deletion-closed admissible history families, a common retained field/coordinate representation after deletion, and equality of terms whose full footprints miss the deleted components. The source's localization statements on pp.374, 377 and 379 support that program but do not by themselves specify this entire comparison. The lemma is not imported as an already checked actual deletion theorem.

### 7. The exact normalization cost for this energy reserve

The unnormalized reserve also gives a sharper diagnostic than multiplying every normalized bound by a reciprocal component mass. It identifies the precise logarithmic mass information that would suffice for polynomial moments of the two outer energies.

#### Lemma RN19.7 — logarithmic mass cost

Let \(M\) be any positive finite measure, let \(\mathcal E\ge0\), and suppose \(M(e^{\theta\mathcal E})\le A\) with \(\theta>0\). On a positive-mass fiber define

\[
 m=M(1),\qquad Q=M/m,\qquad L=\log(A/m)\ge0.
 \tag{RN19.22}
\]

For every real \(p\ge1\),

\[
 \|1+\mathcal E\|_{L^p(Q)}
 \le 1+\theta^{-1}(L+Cp),
 \qquad
 \|(1+\mathcal E)^q\|_{L^p(Q)}
 \le [1+\theta^{-1}(L+Cqp)]^q
 \quad(q\ge1).
 \tag{RN19.23}
\]

**Proof.** Markov's inequality gives
\(Q(\theta\mathcal E>L+t)\le e^{-t}\) for every \(t\ge0\). Thus the nonnegative variable \(\theta\mathcal E\) is stochastically dominated by \(L+E\), where E has the unit exponential distribution. Its p-th norm is \(\Gamma(p+1)^{1/p}\le Cp\). Minkowski gives the first bound; replacing p by qp and raising to q gives the second. ∎

In Proposition RN19.3 one may take \(A=e^{-P_0(g_k)}\), \(\theta=\theta_0\), and the actual \(m_X=T'_k(X;U)1\). The resulting quantity is

\[
 L_X=-P_0(g_k)-\log m_X\ge0.
 \tag{RN19.24}
\]

No upper bound for \(L_X\) has been established here. If a subsequent proof bounded \(L_X\) by the actual shifted output native regulator, (RN19.23) would control normalized polynomial outer-energy moments at the correct polynomial grade, with a fixed factorial cost in source order. The source's upper bound for \(m_X\) is not such a bound: it supplies no lower bound for the mass and hence no upper bound for \(L_X\). This lemma also says nothing by itself about other native energies, selector currents or the full carrier footprint.

### 8. What remains for H-03

The work here proves or isolates useful pieces but leaves the estimate open.

1. **The full marked chart and labels.** Proposition RN19.1 shrinks the continuous integration support. A live history label can still have a larger defining footprint, and the normalized kernel can depend on retained fields outside that support. Those dependencies must be localized, not discarded.
2. **The complete native regulator.** The explicit outer energy (RN19.6) does not include every term of M-03's retained/native list. A bound such as R_in<=C R_k^u R_out(1+E_X), with the actual pulled-back shifted versions and a fixed u, would be useful; no such full inequality has been proved here. A comparison for only a fresh reference is insufficient.
3. **Joint geometry erasure.** The successful-sector normalization must be implemented with its actual marked posterior and verified common geometry, as in Section 6. Keeping a fixed component and dividing by its mass instead loses (RN19.17).
4. **Residual components and all currents.** The fixed Y-components in (1.103)–(1.104) have a different role. Their normalized old posterior still requires the actual retained/selector/geometry currents and an internal or retained-data carrier theorem. The unnormalized reserve is an upper bound; it is not a lower bound for their masses. Raw-coordinate paths and pointwise shifted regulators remain essential.

No actual Yang–Mills counterexample is claimed. In particular, a lower bound on the mean old energy on a selected bad event is not by itself a covariance lower bound, and an auxiliary component-wide reflection label has a component-wide input footprint in M-03. Neither observation can be used to manufacture a false disproof of the original spatial-reset requirement.

### Sources

- Balaban, *Large Field Renormalization I*, CMP 122 (1989), printed pp.177, 179, 192–198, especially (1.10)–(1.12), (1.73), (1.76), (1.81), for the prepared domains, the small final continuous core and the exact remaining old integrations.
- Balaban, *Large Field Renormalization II*, CMP 122 (1989), printed pp.357–358, 378–389, especially (1.71), (1.73), (1.77)–(1.89) and (1.92)–(1.97), for the positive outer energies, fractional-action extraction, chronological costs and successful-component volume payment.
- Balaban, *Convergent Renormalization Expansions*, CMP 119 (1988), (2.19)–(2.21), for localization of the old positive operations.
- The existing M-03 construction, Annex Y, and the reset and geometry annexes, are retained with their original scope restrictions.

See LFR II, pp. 378–379 and 383.
