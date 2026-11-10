# Physical normalization, ultraviolet bounds and source transport

**Scope:** existence without a mass-gap assumption; the original compact Wilson law, its prescribed 21 curvature-bilinear fields and seven physical channel normalizations.  
**Result:** an explicit new ultraviolet summation consequence of the C08 conditional cumulant theorem, together with the exact remaining full-law and normalization requirements. No Yang–Mills existence theorem is claimed.

## 1. Source record and the target that has to be met

1. [Regular conditional covariance, moments and cumulants](../boundary/conditional_probability.md), especially C8A.23–C8A.28 and Sections 8–11.
2. [Sufficient conditions for a continuum hierarchy](../physical_scale/continuum_criteria.md), ER.1–ER.8.
3. [Reflected susceptibilities and physical normalization](../physical_scale/physical_normalization.md), PN.26–PN.42 and PN.48–PN.52.
4. [Separated marked estimates for successful local resets](../physical_scale/separated_marked_estimates.md), RS.29–RS.37 and its final scope statement.
6. [A stopped sequence with a positive weak endpoint](../physical_scale/positive_stopped_endpoint.md), PE.18–PE.23 and its distinction between an emergent scalar endpoint and prescribed physical matching.

The retained C08 conclusion is a theorem about an actual selected *regular conditional law*. It supplies native current fields and their gradients, the full score, a fixed Hessian majorant, covariance, conditional means, and native scalar/tensor cumulants. It does not identify every transported microscopic insertion with a native stencil and does not control the entire outer distribution of conditional means. Those restrictions matter in every application below.

The continuum estimates below assume the displayed C08 inequalities. Their application to every actual Wilson history requires the composed response with earlier innovations fixed.

For a joint test on \((\mathbb R^4)^m\), use the theorem group's dominating Schwartz seminorm
\[
 \nu_r(F)=\max_{|\alpha|\le r}\sup_X
       (1+|X|^2)^{r/2}|\partial^\alpha F(X)|,
 \tag{EC.0}
\]
with a maximum over its finitely many tensor coefficients when present. Coincidence-flat means that every derivative vanishes whenever any pair of arguments coincides.

The fixed existence target in the theorem group decomposition requires one original Wilson sequence and one common continuum hierarchy, with physical normalization, corrected OS regularity, full Euclidean covariance, positivity, the requested energy/phase properties and the stipulated interacting ultraviolet coefficients. No mass gap is needed here. Not every sufficient technical norm in the fixed decomposition is logically necessary for every possible proof: ER.7 is already a weaker route to the hierarchy than proving every original intermediate M03 norm.

## 2. The two sharp numerical inputs for the existing continuum reduction

Write the actual physical field budget as in ER.1:

\[
 b_a=\frac{\|Z_a\|}{\beta_a}+a^4|c_a|.
 \tag{EC.1}
\]

The physical-normalization note proves, on its admitted stopped sequence,

\[
 b_a\asymp B_a:=\frac{\|Z_a\|}{\beta_a}
 =\max_h\sqrt{\frac{\lambda_h}{D_{h,a}}},
 \qquad D_{h,a}=\beta_a^2 n_{h,a}.
 \tag{EC.2}
\]

Here h labels the seven hypercubic channels; it is not a lattice mesh in this equation. The fixed targets \(\lambda_h>0\) are the F01 reflected normalization values. Formula EC.2 uses PN.28 and PN.37–PN.38. The identity coefficient adds no independent growth budget.

### Proposition EC.1: the weak normalization requirement is seven lower bounds

For a fixed finite \(\gamma\ge0\), the coefficient estimate

\[
 b_a\le C a^{-\gamma}
 \tag{EC.3}
\]

is equivalent, up to fixed channel constants, to

\[
 D_{h,a}\ge c\lambda_h a^{2\gamma}
 \quad\text{in every channel, on the same sequence.}
 \tag{EC.4}
\]

**Proof.** Square the maximum in EC.2 and use that the number of channels and all \(\lambda_h\) are fixed. \(\square\)

Strict positivity of every \(D_{h,a}\) at every finite cutoff does not imply EC.4. For example a positive numerical sequence \(D_a=e^{-1/a}\) has inverse square root larger than every fixed power of \(a^{-1}\). This is an elementary warning about the inference, not a counterexample for the Wilson data. The finite positivity theorem FN and its countable avoidance construction supply nonsingularity but no rate of avoidance of zero; they must not be substituted for EC.4.

The second input is ER.7. With its original recent-history event, microscopic position collar, same cofinal sequence, and same physical fields,

\[
 R_{m,n}(F)=a_n^{4m}\sum_{\boldsymbol\alpha,X}
 (1-\chi_n(X))F_{\boldsymbol\alpha}(X)
 \mathbb E_n\!\left[\mathbf1_{E_n^c}
       \prod_{i=1}^m\Phi_{\alpha_i,n}(x_i)\right]
\]

must obey

\[
 |R_{m,n}(F)|\le C^{m+1}(m!)^p\nu_{qm}(F)
 \quad\text{with fixed }C,p,q.
 \tag{EC.5}
\]

The expectation is the actual full Wilson/history expectation, unnormalized on \(E_n^c\). Replacing it by a selected regular conditional law changes EC.5. It includes recent and intermediate histories, successful, residual and unreplaced sectors, outer means, all higher source partners and the actual normalization.

For the exact F01 fields, the one-point case is already reduced by their full-law centering. Since \(\mathbb E_n\Phi_{\alpha,n}(x)=0\) and ER sets \(\chi_n=0\) when \(m=1\),

\[
 R_{1,n}(F)=-a_n^4\sum_{\alpha,x}F_\alpha(x)
       \mathbb E_n[\mathbf1_{E_n}\Phi_{\alpha,n}(x)].
 \tag{EC.5a}
\]

Under EC.3, ER.6 and its once-chosen H2S age threshold make EC.5a tend to zero in its displayed fixed Schwartz seminorm (one may take \(\nu_8\) there). It also gives a uniform one-point bound after increasing the constant to cover finitely many initial cutoffs. Thus the one-point recent full moment is not an additional unproved requirement once the exact centering and the normalization budget are retained. This cancellation does not say that conditional means vanish, and it does not delete their outer cumulants at higher orders.

The already written ER.1–ER.2 reduction proves that EC.3 and EC.5 remove the old-history and position-collar errors and yield one common coincidence-flat mixed hierarchy. It is unnecessary to reprove that diagonal extraction. The work still required is to establish the two actual estimates, and then the additional Euclidean, reconstruction and identification inputs of Section 6 below.

## 3. A new conditional ultraviolet bound obtained from C08

This section gives a concrete strengthening of the continuum use of C08. It controls native conditional cumulants on flat tests with a fixed factorial exponent, not only at fixed separated points.

Rescale the fixed reference length to one. Let \(0<h\le1\) be the current physical mesh, and let \(\nu_{h,v}\) be an admitted selected regular conditional law. Its actual source anchors form a subset of a four-dimensional lattice of spacing h with fixed bounded local multiplicity. Distances \(\rho_h\) are in current lattice units. Fixed blocking ratios are absorbed in constants. On the central-half-torus convention of ER, physical distances of supported anchors agree with their nonwrapped distances, and

\[
 |x-y|\le C h(1+\rho_h(x,y)).
 \tag{EC.6}
\]

Let \(\tau_h\) be the minimum spanning-tree length in \(\rho_h\). For the C08 native scalar/tensor family, C8A.26 gives, for \(m\ge2\),

\[
 |\kappa_{\nu_{h,v}}(O_{\alpha_1,x_1},\ldots,O_{\alpha_m,x_m})|
 \le C^{m+1}(m!)^2h^{-4m}
       P(h)^m e^{-\theta\tau_h/(m-1)}.
 \tag{EC.7}
\]

Here we used the actual bound \(Q_x\le CP(h)\) stated after C8A.23. The constants are uniform in the admitted retained datum v. C8A.28 supplies

\[
 \sup_{x_1}\sum_{x_2,\ldots,x_m}
 e^{-\theta\tau_h/(m-1)}\le C_\theta^m(m!)^5.
 \tag{EC.8}
\]

Define the native conditional cumulant functional

\[
 \mathcal K_{m,h,v}(F)=h^{4m}
  \sum_{\boldsymbol\alpha,X}F_{\boldsymbol\alpha}(X)
  \kappa_{\nu_{h,v}}(O_{\alpha_1,x_1},\ldots,O_{\alpha_m,x_m}).
 \tag{EC.9}
\]

This definition is not an assertion that \(\mathcal K\) is an exact connected shell of the original microscopic source. Identifying such shells remains an actual transport problem.

### Theorem EC.2: flat-test conditional cumulant bound

Assume EC.6–EC.8. For every smooth joint test flat on the coincidence diagonals, supported in the ER central region when the lattice is periodic,

\[
 |\mathcal K_{m,h,v}(F)|
 \le C^{m+1}(m!)^7 h^2 P(h)^m\nu_{6m}(F),
 \qquad m\ge2.
 \tag{EC.10}
\]

No coupling ceiling depends on m, and no probabilistic independence is used.

**Proof.** Fix the pair of arguments 1 and 2. Flatness gives
\(D_2^\alpha F(x_1,x_1,x_3,\ldots,x_m)=0\) for every multi-index \(\alpha\). Taylor's theorem along the segment from \(x_1\) to \(x_2\), to order six, therefore gives

\[
 |F(X)|\le C|x_2-x_1|^6
       (1+|x_1|^2)^{-3}\nu_6(F).
 \tag{EC.11}
\]

The derivative is evaluated at a point whose first coordinate is still \(x_1\), so the displayed spatial weight is valid throughout the segment. The directional sixth derivative costs only a fixed four-dimensional combinatorial constant. The same estimate holds for every tensor coefficient.

The path in any spanning tree connects \(x_1\) to \(x_2\); hence \(\rho_h(x_1,x_2)\le\tau_h\). Combining EC.6 and EC.11 gives the factor \(Ch^6(1+\tau_h)^6\). The additive one permits fixed source-block/stencil offsets without a false zero-distance identification. For \(m\ge2\),

\[
 (1+\tau_h)^6 e^{-\theta\tau_h/(m-1)}
 \le C_\theta(m-1)^6
               e^{-\theta\tau_h/[2(m-1)]}.
 \tag{EC.12}
\]

Use EC.8 at \(\theta/2\), and the four-dimensional lattice root estimate

\[
 \sum_{x_1}(1+|x_1|^2)^{-3}\le C h^{-4}.
 \tag{EC.13}
\]

The estimate is uniform on subsets and on the central part of compatible growing tori; fixed local multiplicity changes only C. Inserting these bounds in EC.9 yields

\[
\begin{split}
 |\mathcal K_{m,h,v}(F)|
 &\le C^{m+1}(m!)^2P(h)^m h^6\nu_6(F)\,
           h^{-4}(m-1)^6 C^m(m!)^5\\
 &\le C_1^{m+1}(m!)^7h^2P(h)^m\nu_{6m}(F).
\end{split}
\]

The factors \(h^{4m}\) and \(h^{-4m}\) cancel before the root count. The fixed power \((m-1)^6\) is absorbed into \(C_1^m\), not into a new m-dependent ceiling. The finite number of tensor labels is absorbed in the same way. Finally \(\nu_6\le\nu_{6m}\). This proves EC.10. \(\square\)

The power \(h^2\) is the difference between the sixth-order vanishing used on the test and the remaining four-dimensional physical root count. It is not an extra dynamical irrelevant factor claimed for the bare operator.

### Corollary EC.3: uniform logarithmic absorption and scale summation

Suppose, in addition, that the *same* physical-scale profile has

\[
 P(h)\le C(1+\log(1/h))^b
 \tag{EC.14}
\]

for one fixed finite b. Then for every fixed \(0<\delta<2\),

\[
 |\mathcal K_{m,h,v}(F)|
 \le C_\delta^{m+1}(m!)^{7+b}h^\delta\nu_{6m}(F).
 \tag{EC.15}
\]

For the geometric meshes \(h=L^{-j}\),

\[
 \sum_{h\le\varepsilon}|\mathcal K_{m,h,v_h}(F)|
 \le C_\delta^{m+1}(m!)^{7+b}
       \frac{\varepsilon^\delta}{1-L^{-\delta}}\nu_{6m}(F).
 \tag{EC.16}
\]

The retained data \(v_h\) can vary arbitrarily within the admitted class. The same estimates hold after an arbitrary positive outer probability average supported on that admitted class, applied to each of these conditional cumulant functions.

**Proof.** Put \(t=\log(1/h)\). Maximizing
\(e^{-(2-\delta)t}(1+t)^{bm}\) for \(t\ge0\), followed by
\(m!\ge(m/e)^m\), gives

\[
 e^{-(2-\delta)t}(1+t)^{bm}
 \le C_{b,\delta}^{m+1}(m!)^b.
 \tag{EC.17}
\]

This proves EC.15 from EC.10. The geometric series proves EC.16. A uniform pointwise-in-v absolute bound passes through any probability average. That last operation averages the conditional cumulant; it does not identify the result with the full-law cumulant. \(\square\)

The postulated fixed-physical-scale AF envelope implies EC.14 when its terminal inverse coupling is bounded uniformly: \(g(h)^{-2}\le C(T+\log_L(1/h))\) with fixed T, and \(P(h)=A_1[\log g(h)^{-2}]^{p_0}\), give a bound of the form EC.14. PE.20 records precisely the bounded-terminal-interval age comparison in its retained source/calibration scope. If the terminal inverse coupling diverges with the cutoff, EC.14 with cutoff-independent constants must be checked separately. This corollary is not a new construction of the trajectory.

### Corollary EC.4: fixed separated supports have a superalgebraic fine-scale tail

At fixed m, suppose the support of F lies in a fixed compact physical set and its anchor spanning-tree length is at least \(d>0\). Under EC.7 and EC.14,

\[
 |\mathcal K_{m,h,v}(F)|
 \le C_{m,F}h^{-4m}(1+\log(1/h))^{bm}
       e^{-c d/[(m-1)h]}.
 \tag{EC.18}
\]

Consequently, for every N, the sum over \(h\le\varepsilon\) is at most
\(C_{m,F,d,N}\varepsilon^N\), uniformly in v.

**Proof.** The physical lattice quadrature of \(|F|\) is bounded on its fixed compact support, while \(\tau_h\ge c d/h-C_m\), with the fixed-order offset absorbed in \(C_{m,F}\). Apply EC.7. An exponential \(e^{-c'/h}\) absorbs any prescribed fixed power of \(h^{-1}\) and logarithm. Leave one additional positive power to sum the geometric meshes. \(\square\)

EC.15 is stronger for the all-order flat-test application because its seminorm order and factorial exponent are fixed. EC.18 makes the physical separation mechanism transparent at each fixed order.

### Corollary EC.4a: fixed inverse-coupling powers in spatially localized reset jets

There is a useful restricted improvement over a rare-value-only optimization. Suppose the literal successful-local coefficients in RS.30, at current physical mesh h, satisfy

\[
 |h^{4|B|}A_{B,X}|
 \le C_0^{|B|}(|B|!)^s
     \left[(g(h)^{-2})^\alpha
          (1+\log g(h)^{-2})^b\right]^{|B|}B_X^{|B|},
 \quad \alpha,b\ge0,
 \tag{EC.22}
\]

with fixed \(s,\alpha,b\), the exact local support of RS.30, and the same admitted conditional law as RS.32. This is an explicit conditional input, not a claimed microscopic-to-current-scale matching theorem. Put
\(T(h)=(g(h)^{-2})^\alpha(1+\log g(h)^{-2})^b\).
In every source partition, \(\sum_{B\in\pi}|B|=m\). Hence its coefficient factor is precisely \(T(h)^m\), and the proof of RS.32 gives the complete finite-jet bound

\[
 |\Gamma_{[m]}(v;X)|
 \le C^{m+1}(m!)^{s+3}h^{-4m}T(h)^m
          e^{-cP(h)}e^{-\gamma\tau_h(X)/m}.
 \tag{EC.23}
\]

For \(m\ge2\), apply the same order-six flat-test Taylor argument as EC.11–EC.13. The anchored divided-tree sum costs \(C^m(m!)^5\), so

\[
 \left|h^{4m}\sum_X F(X)\Gamma_{[m]}(v;X)\right|
 \le C^{m+1}(m!)^{s+8}h^2T(h)^m
                 e^{-cP(h)}\nu_{6m}(F).
 \tag{EC.24}
\]

If, on this same family, \(g(h)^{-2}\le C(T_0+\log(1/h))\) with fixed \(T_0\), then \(T(h)\le C(1+\log(1/h))^{\alpha+b}\). The optimization EC.17 therefore proves, for each fixed \(0<\delta<2\),

\[
 \left|h^{4m}\sum_X F(X)\Gamma_{[m]}(v;X)\right|
 \le C_\delta^{m+1}(m!)^{s+8+\alpha+b}
          h^\delta e^{-cP(h)}\nu_{6m}(F).
 \tag{EC.25}
\]

The geometric fine-scale sum obeys the analogue of EC.16. An input \(g(h)^{-\sigma|B|}\) has \(\alpha=\sigma/2\). All ceilings and exponents are chosen once, independently of source order.

This conclusion is consistent with the warning after RS.36a: the rare factor alone cannot absorb a fixed inverse-coupling power per source grade at fixed factorial cost. Here the extra \(h^2\) comes from physical flat-test summation and supplies that cost, using the actual physical AF comparison. The argument requires a conditional spatially localized jet and current-scale normalization. It does not turn a bare \(a^{-4m}\) microscopic insertion into an \(h^{-4m}\) insertion, and it does not control an outer value term for which no spatial decay has been established.

## 4. Why these estimates do not yet prove ER.7

There are two distinct missing identifications.

First, EC.7 concerns the native C08 scalar/tensor family. The actual input in ER.7 is the *transported microscopic physical source*, including every higher generated source partner. The fixed-depth M04 results do not identify its arbitrary-depth output with that family plus a remainder satisfying EC.15. In particular, a proof for three native regular layers does not supply one uniform estimate after an unbounded number of moving-Q operations, residual sectors and history changes. The new scale-sum theorem does remove a possible downstream counting obstacle once that identification is supplied.

Second, an average of conditional cumulants is only one part of the full cumulant. The exact identity is useful at every order.

### Proposition EC.5: complete law of total cumulance

Let \(\mu(dv,dz)=\pi(dv)\nu_v(dz)\), with all joint moments of the finite family \(X_1,\ldots,X_m\) available. For a nonempty block \(B\subseteq[m]\), put

\[
 k_B(v)=\kappa_{\nu_v}(X_i:i\in B).
\]

Whenever the displayed products are integrable,

\[
 \kappa_\mu(X_1,\ldots,X_m)
 =\sum_{\mathcal P\in\Pi_m}
    \kappa_\pi(k_B(v):B\in\mathcal P).
 \tag{EC.19}
\]

**Proof.** Work in the finite squarefree source algebra, so no moment-generating-function radius is needed. The conditional logarithmic source is
\(\sum_{\varnothing\ne B\subseteq[m]}t_B k_B(v)\). The tower identity gives

\[
 \log\mathbb E_\mu e^{\sum_i t_iX_i}
 =\log\mathbb E_\pi
       \exp\!\left(\sum_{\varnothing\ne B}t_B k_B(v)\right).
\]

Taking the coefficient of \(t_1\cdots t_m\) produces every set partition of the labels once. The outer cumulant of its block coefficients is exactly the corresponding term in EC.19. All operations are finite algebraic identities. \(\square\)

For m=2 this is total covariance. At order three it reads

\[
\begin{split}
 \kappa_\mu(X_1,X_2,X_3)
 ={}&\mathbb E_\pi k_{123}
       +\kappa_\pi(k_1,k_2,k_3)\\
 &+\operatorname{Cov}_\pi(k_1,k_{23})
  +\operatorname{Cov}_\pi(k_2,k_{13})
  +\operatorname{Cov}_\pi(k_3,k_{12}).
\end{split}
 \tag{EC.20}
\]

The new conditional ultraviolet estimate controls the one-block term \(\mathbb E_\pi k_{[m]}\) for its native marks. It does not control the outer cumulants in all the other partitions. Their arguments include conditional means and higher conditional vertices depending on common retained data. Dropping them changes the original Wilson law.

The successful-reset note already retains the analogous full finite-jet partition identity RS.35c. It obtains a complete *value* bound for its specified successful-local class but expressly no spatial decay for an arbitrary outer marginal. This is genuine useful progress and does not constitute the missing general ER.7 estimate. A residual component whose mass has canceled in its normalized base cannot receive the successful-presence rare factor.

## 5. A concrete sufficient replacement for the remaining transport application

The point of EC.15 is that the next estimate can be stated more weakly than the strongest original M03 carrier/current norm, if one pursues ER rather than the entire fixed transport program.

A sufficient next input would be an **exact** connected decomposition of the actual recent physical source into:

1. native conditional scale functionals controlled by EC.15, with actual channel coefficients having fixed per-order logarithmic budgets;
2. the successful-local finite jets controlled by RS.32–RS.36, after their microscopic matching is proved;
3. residual/unreplaced and outer-partition terms with joint-test bound \(C^{m+1}(m!)^p\nu_{qm}\), uniformly in cutoff and total depth;
4. the actual terminal and one-point pieces, and compatible contact/approximation errors on the same test space.

Every item must refer to the same physical normalization and the original full law. Merely defining the residual as the difference between the desired source and the controlled classes supplies no estimate for it. A stronger route may instead prove M04–M07/H04–H05 in their fixed norms. The direct decomposition above is a sufficient alternative, not a theorem that those remaining terms already obey the displayed bounds.

The scalar endpoint progress should also be preserved accurately. The BP/DE/PE chain supplies, at its retained source and calibration scope, an emergent positive scalar endpoint on one cofinal family. It does not identify an arbitrarily prescribed physical coupling, prove the full effective-state/history-map compatibility, or provide the quantitative physical normalization data in EC.4. The C-to-existence analysis addresses its exact dependencies; this note does not erase that progress or turn it into a completed physical matching theorem.

Existence at some suitable positive endpoint does not logically require solving the fixed B05 problem of matching a preassigned endpoint. If the PE sequence satisfies the source hypotheses and the needed physical identification is established there, it is an eligible sequence for an existence proof. Similarly, a direct proof of EC.5 for original Wilson expectations can bypass a theorem asserting convergence of every effective state or history map. The direct ER route needs its exact input estimates, not every stronger sufficient interface of an earlier plan.

## 6. A nonduplicative completion checklist for this route

The following are proof interfaces for the stated program, not a claim of mathematical necessity for every conceivable construction.

| Interface | Existing usable result | Actual missing input |
|---|---|---|
| One physically identified Wilson sequence | Exact positive source representation, stopped compatible geometry and emergent positive scalar endpoint at the retained source/calibration scope | Verify the actual source/physical dictionary and all hypotheses on the chosen sequence. Prescribed B05 endpoint matching and convergence of every effective state/history map are stronger route-specific tasks, not prerequisites for a direct original-law ER.7 proof at an eligible emergent endpoint. |
| Quantitative field normalization | Explicit F01 system, seven-channel finite positivity, PN identity-budget reduction, exact determinant formulas | Seven lower bounds EC.4 (or stronger logarithmic bounds), actual channel mixing and summable normalized remainders where the chosen route uses them |
| Full microscopic hierarchy | C08 native conditional estimates; successful-local reset jets; exact source algebra; the new EC.15–EC.16 scale sum; bounded mixed-kernel composition | ER.7/EC.5 for the actual physically normalized transported microscopic fields, all sectors and outer partitions included |
| Full Euclidean covariance | Exact discrete symmetries, finite hypercubic tensor decomposition and conditional angular reduction | Vanishing action, observable, running-matrix and contact angular defects on this same interacting hierarchy, uniformly along the finite rotation paths |
| Reconstruction and a physical state | ER conditional common extraction, exact finite Wilson reflection positivity, corrected reconstruction and phase-selection bridge theorems | Verification of corrected OS hypotheses, actual field/energy domains and periodic-state passage, then the common phase set and required disconnected symmetries |
| Yang–Mills identification | Bare Wilson action and group conventions, native/comparator UV calculations | Physical two-point running, a specified nonzero interacting connected coefficient with uniform remainder and correct order of limits, and the continuum local operator/identity correspondence required by the target |

The shortest currently written route therefore starts with the admitted PE family, proves EC.3 and EC.5 for its original physically normalized Wilson correlations, and applies ER's common flat-test compactness implication. It need not wait for every fixed M03 norm, an arbitrary prescribed B05 endpoint, or a separate limit theorem for every history map. EC.3 and EC.5 do not alone provide the last three rows.

The normalization and nondegeneracy tasks should not be counted twice. PN.7 already proves that, if the exact F01-normalized full hierarchy converges on one common sequence, then all seven separated reflected measurements remain exactly \(\lambda_h>0\). A finite symmetry average gives a positive Gram form on the complete 21-dimensional field family. Thus no separate post-limit nonzero-field axiom is needed once that actual convergence is proved. On the other hand, free curvature bilinears can also have such positive norms. Those norms do not identify the continuum dynamics as interacting Yang–Mills.

Likewise, the existence of a connected three-point function somewhere is not a general interaction certificate for composite fields: free-field bilinears can have nonzero higher connected moments. The fixed U02 target specifies the physical channel and coefficient, while U03 requires its interacting remainder and the order of limits. The work record explicitly distinguishes a nonzero stress-channel comparator from the separated scalar Gaussian coefficient, which vanishes in the stated comparator. Those distinctions must survive the final identification argument.

The rotation requirement can be presented as the concrete sufficient bound

\[
 |S_{m,a}(F_R)-S_{m,a}(F)|
 \le C^{m+1}(m!)^p\epsilon_a\nu_{qm}(F),
 \qquad\epsilon_a\longrightarrow0,
 \tag{EC.21}
\]

with the proper tensor action and constants uniform along the actual finite rotation paths. Hypercubic invariance alone does not imply EC.21, and an estimate on a zero-terminal-coupling comparison family does not establish it on the physically matched family. R02–R05 separate the action, observable/contact and path-uniformity requirements.

Finally, the A02 reconstruction explicitly reconstructs the initial mixed hierarchy without assuming clustering. The later E/V applications supply the requested energy and phase properties. No mass gap is used in EC.1–EC.21, and no claim about a spectral gap is needed to formulate these remaining tasks.

## 7. Conclusion of this calculation

The new proved calculation is the ultraviolet estimate EC.10–EC.18, conditional only on the precisely displayed C08 native cumulant bounds and, for its scale-summed physical form, the fixed physical AF envelope. Its factorial growth and test-seminorm order are fixed. It works under arbitrary positive averaging of those conditional cumulant functions.

The same calculation identifies why it is not yet the desired existence theorem: the actual microscopic matching, the non-one-block terms of EC.19, and the quantitative reflected data EC.4 remain unproved here. The existing ER compactness theorem becomes applicable only after those actual-model estimates have supplied EC.3 and EC.5. Full rotations, corrected reconstruction/physical-state applications and Yang–Mills ultraviolet identification still have their own explicit requirements.

This note supplies a usable regular-sector continuum estimate and a precise next target. It does not change an open original-law requirement into an assumption and then report Yang–Mills existence as proved.

### Independent calculation conditions

## 8. A compensated normalized-source route around a pointwise innovation estimate

The M04 analysis gives an exact reason to combine the response terms before taking absolute values. In [Moving ancestor bases, fixed innovations, and exact latent-gauge current transport](../observable_transport/D_native_nonlinear/M04_Moving_Base_Response_and_Latent_Gauge_Current.md), MB.9–MB.11 imply

\[
 D_W\Xi[\mathfrak d_W\xi]
 =\mathfrak d_{\Xi}\widetilde\xi
       -D_x\Xi[A_{\widetilde\xi}x].
 \tag{EC.26}
\]

At a fixed raw innovation x, removal of the output gauge leaves the second term. MB.12–MB.17 gives a finite gauge-invariant plaquette detector of that term, without the proposed ancestor-distance suppression. This does not establish a counterexample to the literal C05 stopped history class: its prepared grade is a geometric datum, and a fixed innovation level is not automatically that grade. It does show why a direct critical-minimum row cannot be transferred to a fixed-innovation composition without checking the extra term.

The issue is concrete in the C-05 argument. SD.6d–SD.6e restores the original density pulled back through the actual composed source maps, while ST.7–ST.8 applies a normalized response row to that composition. The actual-history argument H32–H36 of [Conditioning, deletion and mass factors for the retained history](../boundary/primitive_estimates/history_masses.md) used the integration of recent preparation-collar innovations. Such a statement is not, by itself, a pointwise estimate after those innovations have been reintroduced by unrolling. Nor is an exponential loss across the full prefix automatically harmless: the full depth satisfies \(N_r\le C_NR_r\), while only the distinct top band \(N_0=O(\log R_r)\) permits \(L^{CN_0}\) to be absorbed as a fixed profile polynomial. These are source-application questions requiring a literal variable/geometry identification or a compensated estimate.

The following algebraic identity supplies an alternative interface. It generalizes MB.22 to every finite source grade and retains the source-dependent denominator exactly.

### Proposition EC.6: normalized finite-source material-current identity

Let \(D_t\) be a moving integration domain, \(\rho_t>0\) its complete unnormalized density, and \(\Psi_t(u,x)\) a finite squarefree source polynomial with zero constant source coefficient. All earlier source partners, actual Jacobians, Gaussian factors, archived masses and retained-data dependence are included in these objects. Put

\[
 \mathfrak Z_t=\int_{D_t}\rho_t,
 \qquad N_t(u)=\int_{D_t}\rho_t e^{\Psi_t(u)},
 \qquad G_t(u)=\log\frac{N_t(u)}{\mathfrak Z_t}.
 \tag{EC.27}
\]

Assume the ordinary differentiation/transport formulas hold, including their boundary terms. A finite disjoint history decomposition can be included by summing every displayed integral and boundary functional over its literal branches. Let \(s_t=\partial_t\log\rho_t\), choose a latent coordinate velocity \(w_t\), and write

\[
 D_w=\partial_t+w_t\cdot\nabla,
 \qquad A_t=s_t+\rho_t^{-1}\operatorname{div}(\rho_tw_t).
 \tag{EC.28}
\]

If \(\mathfrak B_t(f)\) denotes the actual moving-domain boundary functional and
\(\mathfrak F_{w,t}(f)=\int_{\partial D_t}f\,w_t\cdot n\), put
\(\mathfrak C_t^w=\mathfrak B_t-\mathfrak F_{w,t}\).
Define \(\mathbb E_t^\Psi f=N_t(u)^{-1}\int\rho_te^{\Psi_t}f\) formally in the finite source algebra, and let \(\mathbb E_t\) be the positive zero-source law. Then

\[
\begin{split}
 \partial_tG_t(u)
 ={}&\mathbb E_t^\Psi[D_w\Psi_t]
       +\mathbb E_t^\Psi[A_t]-\mathbb E_t[A_t]\\
 &+\frac{\mathfrak C_t^w(\rho_te^{\Psi_t})}{N_t(u)}
       -\frac{\mathfrak C_t^w(\rho_t)}{\mathfrak Z_t}.
\end{split}
 \tag{EC.29}
\]

The two denominators are distinct and neither is omitted. Because \(N_t(0)=\mathfrak Z_t>0\), their formal inverses and the logarithm exist at every finite grade without an analytic source radius.

**Proof.** Differentiate the numerator, then integrate the latent divergence once:

\[
 \partial_tN_t
 =\int_{D_t}\rho_te^{\Psi_t}(D_w\Psi_t+A_t)
       +\mathfrak C_t^w(\rho_te^{\Psi_t}).
 \tag{EC.30}
\]

Setting the source to zero gives
\(\partial_t\mathfrak Z_t=\int\rho_tA_t+\mathfrak C_t^w(\rho_t)\).
Subtract \(\partial_t\log\mathfrak Z_t\) from \(\partial_t\log N_t\). This is EC.29. Each source coefficient is a finite algebraic identity. \(\square\)

For a pure gauge motion, use the actual induced latent velocity, together with the pushed-forward density, domain and source labels. Where this is an exact symmetry, the material source, centered material score and residual flux vanish as a completed expression. This requires transforming the complete retained exterior as well, or restricting the motion to its stabilizer. A partial conditional integral with an earlier raw exterior x fixed need not be invariant: when its covariance identity is \(H_t(T_tx)=H_0(x)\), differentiation gives

\[
 \partial_tH_t(x)=-D_xH_t(x)[v_t(x)],
 \qquad v_t=\partial_tT_t\circ T_t^{-1}.
 \tag{EC.29a}
\]

That exterior material derivative must be retained or canceled by its later exact outer integration. The complete symmetry cancellation can hold even when the fixed-innovation integrand derivative in EC.26 is nonzero. This is precisely why the completed current, including its boundary and normalization terms, should be estimated before its origins are separated.

### Moment form retaining the recent-history event

For any finite source-dependent \(f_t\), the same proof gives

\[
 \partial_t\mathbb E_t f_t
 =\mathbb E_t[D_wf_t]
   +\operatorname{Cov}_t(f_t,A_t)
   +\frac{\mathfrak C_t^w\bigl(\rho_t(f_t-\mathbb E_tf_t)\bigr)}
          {\mathfrak Z_t}.
 \tag{EC.31}
\]

Take \(f_t=\mathbf1_{E_n^c}e^{\Psi_t}\) on the actual fixed-branch decomposition. Count selector motion exactly once: either as the weak derivative of the indicator on the unpartitioned domain, or as the selected-branch boundary current with its indicator constant on each branch. EC.31 then retains the *unnormalized* recent-history moments required by ER.7; no division by \(\mathbb P(E_n^c)\) has been introduced. Its denominator remains the complete original \(\mathfrak Z_t\), not a selected-event mass. The physical F01 normalization belongs to the original source coefficients and must be retained through the identity. If outer variables are still present, apply their exact positive expectation, including their source-dependent weights when using logarithmic source coordinates. The whole-source moment formulation automatically retains the outer terms; an average of conditional log coefficients alone would not.

### A precise sufficient estimate, still open for the full Wilson construction

Suppose an exact chronological interpolation of the same microscopic recent source has been constructed, with an endpoint bound and completed increments given by EC.31. After the actual outer expectation and physical source-position sum, let \(\mathcal J_{m,h,t}(F)\) denote the complete m-source coefficient of its right side. The following are sufficient:

\[
\begin{split}
 |R_{m,n}^{\rm endpoint}(F)|
     &\le C^{m+1}(m!)^{p_0}\nu_{q_0m}(F),\\
 |\mathcal J_{m,h,t}(F)|
     &\le C^{m+1}(m!)^p h^\delta\nu_{qm}(F),
       \qquad 0\le t\le1,
\end{split}
 \tag{EC.32}
\]

with fixed \(\delta>0\), geometric physical meshes h, and an exact telescoping identity for the original source. Integrating in t and summing the geometric h-powers proves ER.7, with fixed factorial and seminorm exponents. If a coarser endpoint contains finitely many scales, they are included in the first bound.

EC.32 estimates one normalized, integrated, physically tested response. It does not require an ancestor-decay bound for every pointwise fixed-innovation derivative. EC.24–EC.25 show how a spatially localized conditional part can meet the required ultraviolet summation, while EC.29–EC.31 specify the additional compensated density and boundary pieces that must be retained. The actual all-history estimate EC.32, its exact source matching and the endpoint bound have not been proved here. This is a weaker sufficient interface for ER.7, not a completion claim for C05, M04 or Yang–Mills existence.
