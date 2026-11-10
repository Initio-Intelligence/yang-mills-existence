# Old Gaussian energy, rank and native-envelope reserves

This note proves an additional estimate on the **actual unnormalized old operation**, including all its surviving Gaussian coordinates, and a common positive envelope on its admitted native chart. It also gives an actual-source reason that a curvature-only lower bound for every bad selector is false in the displayed soft-gauge convention. It does not identify the old posterior with the fresh reference law, infer a lower mass from an upper mass, or claim a full M-03 operator theorem. Whether the H-03 spatial-response requirement follows from the separate full-law spatial theorem is not decided here; none of the strong-norm gaps below is removed by it.

### 1. Exact energies and exact normalizers

Fix a literal eligible component \(X\) at step \(k\), with all the admissibility and parameter hypotheses in LFR I–II. Let \(M_{X,\xi}\) denote the positive operation \(T'_k(X;\xi)\) in LFR II (1.71), on the full remaining old-variable and old-history space. It includes its selectors, coarea factors, old reference normalizers, self action and internal-history sums. Its native retained argument is \(\xi=(U,J)\). In positive-measure statements the reference is an actual real compact configuration with \(J=0\), as on LFR II p.380; a general native analytic deformation need not itself be a positive law. Write

\[
 m_{X,\xi}=M_{X,\xi}(1),\qquad
 \nu_{X,\xi}=m_{X,\xi}^{-1}M_{X,\xi}
 \tag{NR20.1}
\]

on the active set \(m_{X,\xi}>0\). No lower estimate for this mass is part of the definition.

There are two outer nonnegative energies, exactly as in RN19.6:

\[
 \begin{split}
 Q_X&=\tfrac12\langle D H''_{1,k,X}B,\zeta D H''_{1,k,X}B\rangle,\\
 S_X&=A((g'_k)^{-2}\zeta_1|_X,
             U''_{h+2}(\exp(i g_kB),V'')),
 \qquad \mathcal E_X=Q_X+S_X .
 \end{split}
 \tag{NR20.2}
\]

Here \(h=k-N\) is the source's older step index, not the physical spacing in M-03.

Now retain every positive Gaussian exponent **still present** in \(T_h\). The ordinary factor is CMP119 (2.21), or LFR I (1.25), restricted to its old component. In actual free coordinates it is

\[
 q_{j,C}(a)=\tfrac12 a_C^{\mathsf T}S_{j,C}a_C,\qquad
 S_j=K_{OO}-K_{OI}(K_{II})^{-1}K_{IO},\qquad
 K_j=C_j^*\Delta^{(j)}C_j .
 \tag{NR20.3}
\]

The actual background-current term, exceptional-bond map and principal covariance are retained. These are the coefficients identified in OR17.8 using CMP99 (3.155)–(3.158) and Theorem 3.15. Cross-component terms assigned to the effective action are not included a second time. On the real admitted source domain these within-component forms have the positivity used on LFR II printed p.383.

Define, branch by branch,

\[
 \mathcal G_X=\sum_{(j,C)\ {\rm still\ integrated}}q_{j,C},
 \qquad \mathcal F_X=\mathcal E_X+\mathcal G_X .
 \tag{NR20.4}
\]

Earlier completely integrated operations now represented as scalar factors are not reintroduced as hidden coordinates. A modified old factor contributes its surviving displayed positive Gaussian form on its actual surviving coordinate set; an empty fluctuation set contributes zero. Raw compact variables, soft gauge factors, characteristic functions and already integrated constants remain in the original measure.

\(\mathcal F_X\) is **not** defined to be the full M-03 regulator. In particular it does not silently include every native plaquette energy at every surviving old scale. Equation (NR20.3) is a precision energy, not a newly chosen Euclidean-coordinate norm.

### 2. A reserve for the actual old Gaussian energies

#### Theorem NR20.1 — fractional reserve with arbitrary old depth

There is a fixed \(\theta>0\), which may be chosen sufficiently small with \(\theta\le1/8\), such that the source parameter order and one common small coupling ceiling give

\[
 \boxed{M_{X,\xi}\bigl(e^{\theta\mathcal F_X}\bigr)
                  \le e^{-P_0(g_k)}} ,
 \tag{NR20.5}
\]

uniformly in the actual admitted real native data, total volume and arbitrary depth of the internal old histories. Here \(P_0(g)\) is the function denoted \(p_0(g)\) in LFR II. This is an unnormalized estimate.

**Proof.** The insertion replaces each displayed positive outer and surviving old Gaussian exponent coefficient by \(1-\theta\). It changes no chart, constraint, coarea factor, reference density or normalizer. In particular an old normalized reference operation is not replaced by one with a smaller precision. We estimate the original positive integral with the stated insertion.

The source extraction on LFR II pp.380–383 bounds all other exponent terms and normalization terms by a positive domain cost, then uses fixed fractions of the positive Wilson/quadratic energies to extract the old and preparatory bad-field factors. Reducing the positive coefficients preserves that argument with a smaller fixed extraction coefficient. Choose the fractions before the coupling ceiling. The strict source inequalities leave room both for extraction and for the remaining Gaussian majorant. Each energy is reduced once at its own step; the number of fractions is not chosen according to old depth.

The additional integration change beyond RN19.3 is the old Gaussian comparison. On the exact \(r_{j,C}\)-dimensional free subspace, at fixed remaining data,

\[
 \int e^{-(1-\theta)q_{j,C}(a)}\,da
   =(1-\theta)^{-r_{j,C}/2}\int e^{-q_{j,C}(a)}\,da .
 \tag{NR20.6}
\]

This is the full Gaussian majorant after dropping the old characteristic restrictions, exactly where the source invokes Gaussian positivity on p.383. It uses the actual Schur precision and its actual determinant. A coarea factor present before the free-coordinate parametrization is retained on both sides; its remaining-data dependence is treated by the same source domain bound. Equation (NR20.6) is a comparison of majorants, not an equality for the selected integral.

In the relabeled volume convention of LFR II (1.79), the rank satisfies

\[
 \sum_C r_{j,C}\le C_{d,G,L}|Z_j\cap\Omega_j|_j
      \le C_{d,G,L}M^dR_j^d d'_j(Z_j).
 \tag{NR20.7}
\]

The first inequality counts the independent Lie coordinates which actually remain. Deleting a tree, imposing the linear constraint or taking a component restriction decreases the count. The fixed \(L\)-dependent factor permits the indexing conversion from CMP119, where \(A_j\) is on \(Z_{j+1}\cap\Omega_{j+1}\). The second is the admissible enlarged-domain estimate on LFR II p.380, with its own \(d'_j\). The total new loss is at most

\[
 \exp\!\left[C_\theta\sum_{j\le h}
                   M^dR_j^d d'_j(Z_j)\right].
 \tag{NR20.8}
\]

Enlarge the existing coefficient of
\(C\sum_jM^dR_j^{d+1}d'_j(Z_j)\) to absorb this. The entire old-scale sum remains. It is not bounded by current volume or by a bounded count of old variables.

For the outer \(B\) integral, the logarithmic factor in the last line of (1.71) is \((\sigma_0g_k^{d_G})^{n_B}\). Together with \(dB\,\sigma(g_kB)\) and its tree delta this is the normalized compact Haar-coordinate measure, as verified in RN19.8a. Drop the remaining positive outer quadratic and bound that restricted compact integral by one, as on p.383. There is no outer Gaussian determinant loss. The other compact integrals and all unchanged reference constants are treated exactly as in the source.

We have therefore obtained source (1.79) with a smaller fixed positive extraction coefficient and a larger fixed domain-cost coefficient. Its worst preparatory factor is still

\[
 \exp[-c_\theta R_j^{-(d+5)}p_1(g_j)^2],
 \qquad 2p_1-(d+5)r_0>p_0 .
 \tag{NR20.9}
\]

The chronological induction (1.80)–(1.88), with the source's \(N=R_j\), pays the complete scale sum. Its strict requirements include

\[
 P_0(g)\gg C_\theta M^dR(g)^{d+2},\qquad
 c_\theta A_1^2P_0(g)^2
    \gg P_0(g)+C_\theta M^dR(g)^{d+2}.
 \tag{NR20.10}
\]

Changing fixed constants changes only the common ceiling. The final store from (1.89) gives the weaker (NR20.5). This proves arbitrary-depth uniformity with every old reference unchanged. ∎

The imported positivity and chronological extraction retain the scope of the established source-free construction. This theorem adds an explicitly identified marked insertion; it is not an independent verification of its coupling trajectory.

The same proof allows an explicit **old-coordinate-count store**. Let
\(D_X=\sum_{j,C}r_{j,C}\) be the actual number of surviving independent Gaussian Lie coordinates on a history branch. For each fixed \(u\ge0\), the ceiling may be chosen so that

\[
 M_{X,\xi}\!\left[e^{\theta\mathcal F_X+uD_X}\right]
                      \le e^{-P_0(g_k)} .
 \tag{NR20.9a}
\]

Indeed \(uD_X\) adds at most \(uC\sum_jM^dR_j^d d'_j(Z_j)\) to the same chronological domain cost. No new analytic argument is needed, and \(u\) is fixed before source order is varied. Thus polynomial factors counting those old coordinates can also be paid with fixed factorial growth before individual normalization. This is a random rank under the actual history sum, not an assertion that the rank is bounded by the small current core.

#### Corollary NR20.1a — the ordinary old native free coordinates

Let \(\mathscr O_X\) be the free coordinates still integrated through the **ordinary** old factors of CMP119 (2.21), in their dimensionless birth-scale convention, and set

\[
 Z_X=\sum_{(j,i)\in\mathscr O_X}|a_{j,i}|^2 .
 \tag{NR20.10a}
\]

There is a fixed \(\lambda_0>0\), independent of old scale and admitted history, such that

\[
 \mathcal G_X\ge\tfrac12\lambda_0 Z_X,\qquad
 M_{X,\xi}\!\left[e^{\theta_1(\mathcal E_X+Z_X)}\right]
             \le e^{-P_0(g_k)},\qquad
 \theta_1=\theta\min\{1,\lambda_0/2\}.
 \tag{NR20.10b}
\]

**Proof.** The paragraph following CMP99 (3.158), printed p.428, states the positive lower bound \(K_j\ge\lambda_0I\) for the actual free-coordinate precision, independent of step and background under the admitted conditions (3.35)–(3.36). This is the primary bound used in C-06, HC.8–HC.10 and HA15.1–HA15.7. The real background admission includes its current and second-order conditions, not only a curvature restriction.

The source's larger current free region is \(\Omega_{j+1}\) before the inner \(\Lambda_{j+1}\) variables are integrated. That larger region already has the fixed collar from the preceding bad region, by CMP119 (3.2)–(3.5) and the C-06 hypotheses, Section 3. It therefore satisfies the unit-lattice hypothesis of CMP99 Section E. The later restriction to the inner \(\Lambda\) is not used to move an old retained coordinate across a missing collar. Apply the primary bound on this full admitted current free space with its fixed exceptional-bond map.

For the exact Schur complement in (NR20.3),

\[
 a^{\mathsf T}S_ja
  =\min_b (b,a)^{\mathsf T}K_j(b,a)
  \ge\lambda_0|a|^2 .
 \tag{NR20.10c}
\]

Restricting \(a\) to one retained component preserves the lower bound. Sum the resulting inequalities over the actual ordinary old factors. This proves the first inequality in (NR20.10b). The second follows pointwise from
\(\theta_1(\mathcal E_X+Z_X)\le\theta\mathcal F_X\)
and Theorem NR20.1. ∎

The \(a_{j,i}\) here are the actual source dimensionless free variables at their own \(j\)-scale, which are the corresponding ordinary slots of M-03's native list. No simultaneous physical rescaling to the current \(k\)-scale is made. A mark's physical factor remains separate. The statement includes no raw compact-link plaquette and makes no unverified identification for a hidden coordinate which has undergone a different completed-R chart. A modified factor can be included only when its surviving coordinate and form are literally the same identified ordinary ones. Thus this is a genuine partial native-regulator comparison, not a declaration that the full regulator has been bounded.

More explicitly, the norm in (NR20.10c) is the unweighted sum on the **birth-scale unit lattice**, in an orthonormal basis for the source Lie-algebra inner product. This is the unit-lattice operator of CMP99 Section E and HC.1/HA15.7; it is not a layer-weighted physical-space norm. A fixed change to M-03's Hilbert–Schmidt Lie basis changes only \(\lambda_0\) by a fixed group-normalization factor. A slot is included in the native comparison only when its recorded M-03 dimensionless coordinate coincides with this source coordinate under that fixed conversion. In the convention \(\log U=g_j a_j=h_j A^{\rm phys}_j\), a physical potential instead has \(a_j=h_jA^{\rm phys}_j/g_j\); its square cannot be inserted without that factor. Physical-volume weights, if introduced in another notation, must first be converted back to this unit-lattice quadratic form. None is omitted from a claimed bound on arbitrary raw variables.

#### Corollary NR20.2 — all finite old-energy powers

For real \(r\ge1\),

\[
 M_{X,\xi}[(1+\mathcal F_X)^r]
   \le e^\theta\left(\frac r{e\theta}\right)^r e^{-P_0(g_k)}.
 \tag{NR20.11}
\]

For integers \(m\ge0\), a convenient weaker bound is

\[
 M_{X,\xi}[(1+\mathcal F_X)^m]
       \le e^\theta\theta^{-m}m!e^{-P_0(g_k)}.
 \tag{NR20.12}
\]

**Proof.** Apply \(x^r\le(r/(e\theta))^re^{\theta x}\), or \(x^m\le m!\theta^{-m}e^{\theta x}\), to \(x=1+\mathcal F_X\), then use (NR20.5). ∎

The finite-jet partition proof in RN19.5 now applies with \(\mathcal F_X\) in place of \(\mathcal E_X\). If every incoming degree-\(d\) log coefficient has the pointwise bound
\(C^{d+1}(d!)^s b^d r(\xi)^d(1+\mathcal F_X)^d\), \(s\ge1\), the full unnormalized degree-\(m\) coefficient is bounded by

\[
 e^{-P_0(g_k)}C_1^m(m!)^{s+1}b^m r(\xi)^m.
 \tag{NR20.13}
\]

All higher incoming vertices are retained. Membership of a general M-03 coefficient in this energy class is not assumed.

### 3. A common envelope on the actual native chart

On the fixed-support native chart of LFR II pp.379–380 only \(Q_X\) and the self activity \(V(X^\sim)\) depend on the native pair. In those coordinates the outer Wilson term, old operation, old selectors and old Gaussian forms are unchanged. The source bounds the quadratic variation and the resummed variation of \(V\) separately. Shrink the common chart so that

\[
 M_{X,\xi}(d\eta)=e^{\sigma_\xi(\eta)}M_{X,0}(d\eta),\qquad
 \sup_{\xi,\eta}|\sigma_\xi|\le\delta_\sigma,\qquad
 \sup_{\xi,\eta}|Q_{X,\xi}-Q_{X,0}|\le\delta_Q
 \tag{NR20.14}
\]

with fixed small constants. The first is the actual pointwise comparison (1.73)–(1.75); the second is its separately bounded quadratic contribution, not an inference from cancellation in \(\sigma\). Define

\[
 \mathcal F_X^\natural(\eta)
   =1+\sup_{\xi\ {\rm admitted\ native}}|\mathcal F_{X,\xi}(\eta)|.
 \tag{NR20.15}
\]

#### Corollary NR20.3 — native shifted energy envelope

For every admitted native \(\xi\), with total variation for its possible complex measure,

\[
 |M_{X,\xi}|[e^{\theta\mathcal F_X^\natural}]
 \le e^{\delta_\sigma+\theta(1+\delta_Q)}e^{-P_0(g_k)} .
 \tag{NR20.16}
\]

The power bounds (NR20.11) follow for this envelope with the fixed extra factor. This controls one supremum envelope **before** integrating it.

**Proof.** Exact native independence of the other energy terms gives
\(\mathcal F_X^\natural\le1+\mathcal F_{X,0}+\delta_Q\).
Use this and \(|e^{\sigma_\xi}|\le e^{\delta_\sigma}\) in the common measure, then apply (NR20.5) at the real center. ∎

This is narrower than the full M-03 shifted envelope. It does not cover arbitrary raw retained links, hard selectors, geometry changes or current maps outside the fixed-support chart. Those variations may change the measure or the old forms. Taking a supremum over unavailable charts would not prove their bound.

The normalized cost remains explicit. At the real center set

\[
 L_X=-P_0(g_k)-\log m_{X,0}\ge0 .
 \tag{NR20.17}
\]

For the positive real slice, RN19.7 and the mass comparison \(e^{-\delta_\sigma}m_{X,0}\le m_{X,\xi}\le e^{\delta_\sigma}m_{X,0}\) yield

\[
 \|\mathcal F_X^\natural\|_{L^p(\nu_{X,\xi})}
       \le C_\theta[1+L_X+p],\qquad p\ge1 .
 \tag{NR20.18}
\]

This is the enlarged-energy and native-envelope version of the logarithmic estimate. No upper bound for \(L_X\) has been proved here. The upper bound \(m_X\le e^{-P_0}\) cannot supply one.

### 4. Full-footprint payment when the mass is retained

An eligible \(X\), including its fixed dependency collars, fits in a current cube of side \(C_MR_k\). Both the cube volume and a spanning-tree length are \(O(C_MR_k^d)\). The number of candidate shapes through an anchor, including containing-cube placements, is at most \(\exp(C_MR_k^d)\). Therefore, for every fixed footprint rate \(\kappa\), a smaller common ceiling gives

\[
 \sup_b\sum_{X\ni b}
 e^{\kappa(|X^+|+\mathsf t(X^+))}
 |M_{X,\xi}|[(\mathcal F_X^\natural)^m]
       \le C^{m+1}m!e^{-P_0(g_k)/2}.
 \tag{NR20.19}
\]

Here \(X^+\) is the actual fixed-collar carrier. The sum is over literal eligible geometric species; each measure already contains its internal-history sum. To prove the formula, use the deliberately rough bound \(2^{C_MR_k^d}\) on subsets of a containing cube, apply (NR20.12)/(NR20.16), and use \(P_0(g_k)\gg R_k^d\). No internal history is counted again.

On the actual positive real slice this is the form needed by a common positive successful-component gas. For example, if its exact deletion identity preserves the retained variables and remaining measures and has

\[
 H_{D\cup S}-H_D\le\sum_{X\in S}\lambda_X,
 \tag{NR20.20}
\]

then RN19.6 gives the normalized full-law pinned estimate

\[
 \mathbb E\!\left[\mathbf1_{S\subset D}
            \prod_{X\in S}(\mathcal F_X^\natural)^{m_X}\right]
 \le\prod_{X\in S}e^{\lambda_X}
                    M_X[(\mathcal F_X^\natural)^{m_X}].
 \tag{NR20.21}
\]

This is an implication until the actual common-gas/deletion identities are verified. There is no component \(m_X^{-1}\) on its right. Conversely its small right side does not bound \(\nu_X\) after conditioning on presence of \(X\); that is a different normalization.

### 5. An actual selector obstruction to curvature-only shortcuts

This section uses the **displayed soft gauge fixing** in CMP119 (1.5)–(1.8), pp.246–248. The source also permits an averaged hard tree gauge; the statement is not asserted for that alternative without a separate check.

#### Proposition NR20.4 — a pure-gauge \(Q_1\)-bad configuration

For sufficiently small \(g_0\) and the source order \(A_0\gg A_1\), there is a configuration admitted by the soft gauge factor such that every fine plaquette and the first coarse configuration are the identity, \(P_0=P_1=\varnothing\), but \(Q_1\ne\varnothing\).

**Proof.** Let \(\varepsilon_0,\delta_0\) be exactly the source thresholds in (1.1), (1.8), so \(\delta_0/\varepsilon_0=A_1/A_0\) and \(\delta_0/g_0\) is a fixed positive multiple of \(P_0(g_0)\). Choose an interior noncentral fine site \(x\) of one first block and a fixed nonzero Lie generator \(T\). Set \(u=1\) at every site except \(x\), and choose \(u(x)=\exp(aT)\) so that
\(3\delta_0<\|u(x)-1\|<4\delta_0\). Take

\[
 U(e)=u(e_-)u(e_+)^{-1}.
 \tag{NR20.22}
\]

All fine plaquettes are one. Gauge covariance of the actual block average gives \(V_1=1\), since \(u\) is one at every coarse block center. The axial local minimizing backgrounds \(U_{1,\Box}(V_1)\) in (1.2) are consequently one, so the \(P_0,P_1\) tests are strictly good.

The soft gauge contours satisfy \(U(y,z)=u(y)u(z)^{-1}\). They equal one except at \(x\), where their distance is less than \(4\delta_0<\varepsilon_0\). Every characteristic factor in (1.5) is therefore one and its exponential is positive. An interior bond incident to \(x\) is not an exceptional interblock bond \(b_0(c)\), and

\[
 \|U(b)U_{1,\Box}(b)^{-1}-1\|>2\delta_0 .
 \tag{NR20.23}
\]

The selector (1.8) puts a cube whose enlarged tested stencil contains that bond into \(Q_1\). ∎

These strict inequalities persist in a neighborhood, by continuity of the admitted local minimizing map. At fixed finite cutoff one can make the Wilson energy of that neighborhood arbitrarily small while keeping the \(Q_1\)-bad inequality. Thus a curvature-only implication

\[
 \text{some actual \(P/Q/R\) selector is bad}
 \ \Longrightarrow\
 \sum_p\beta_p s(U_p)\ge cP_0(g)^2
 \tag{NR20.24}
\]

is false for the displayed soft-gauge convention. The soft gauge energy pays this event. This does not contradict the source extraction, which retains gauge factors and positive fluctuation forms, and it is not a counterexample to H-03 or to a theorem for the actual restricted gauge-invariant field family.

#### Lemma NR20.5 — quantitative local soft-gauge seed weight

On the flat physical orbit with coarse center gauges fixed, the normalized gauge coordinates in (1.5) have product density

\[
 \prod_{z\ne y}
   \frac{\mathbf1_{\{\|v_z-1\|<\varepsilon_0\}}
                 e^{-g_0^{-2}s_0(v_z)}}{z(g_0)}\,dv_z,
 \qquad s_0=1-\operatorname{Re}\operatorname{tr}.
 \tag{NR20.25}
\]

For a finite local seed region containing \(D\) gauge coordinates, put the coordinate at \(x\) in a radius-\(c g_0\) ball about the value in Proposition NR20.4 and its other \(D-1\) coordinates in such balls about one. This event has conditional probability at least

\[
                  \exp[-CP_0(g_0)^2-CD].
 \tag{NR20.26}
\]

Outside coordinates are fixed or retain their product marginal; no torus-volume cost is imposed.

**Proof.** Compact-group Haar density in a fixed exponential chart is bounded above and below, and
\(c|v|^2\le s_0(\exp v)\le C|v|^2\). Since \(\varepsilon_0/g_0\to\infty\),

\[
       cg_0^{d_G}\le z(g_0)\le Cg_0^{d_G}.
 \tag{NR20.27}
\]

Every radius-\(c g_0\) numerator ball has Haar volume at least \(c'g_0^{d_G}\). Its action is \(O(1)\) about one and \(O(P_0(g_0)^2)\) at the seed. Divide by the exact normalizers and multiply. The bad margin survives because \(\delta_0/g_0\to\infty\). ∎

This is an actual local gauge-selector seed probability, conditional on the stated physical orbit. It is **not** a lower bound for the later fully integrated \(m_X(U)\). It has not proved that every prescribed final eligible \(X\) is seed-realizable, that all preparatory coarea fibers have uniformly controlled thickness, or that arbitrary retained data can be compared to the flat case.

### 6. Exact remaining normalized-regulator questions

Two distinct questions remain.

1. **Normalization.** A fixed-component posterior estimate needs an upper bound for \(L_X\) in (NR20.18), controlled by the actual output native regulator or by an explicitly retained alternative. A seed at birth is insufficient without exact final geometry, chronological restrictions, fine-coordinate volume and retained-data comparisons. The bounded native tilt is local in its admitted chart; it is not a global comparison to the flat datum.
2. **The rest of the native-energy dictionary.** Corollary NR20.1a now controls the ordinary old dimensionless free slots by their actual uniformly coercive Schur forms. The full shifted M-03 regulator also contains its stated surviving old plaquette list and any differently transformed free coordinates. These still need the correct physical scale factors, actual coordinate maps, footprints and every allowed shift. One reconstructed Wilson action does not automatically dominate an extensive list of old-scale plaquettes.

For successful components in a joint full law, the masses can instead remain available as in (NR20.21), once its actual representation is verified. For residual fixed components, a law-level spatial theorem can use the actual conditional input moments without a mass lower bound. An unconditional moment bound cannot be substituted for a rare-sector conditional one; any global passage must use a true-marginal disintegration or replica construction.

This note thus adds an actual old-Gaussian reserve, a genuine native supremum envelope, full-footprint payment for that energy class and an actual-source selector test. It leaves the full ambient M-03 normalized-regulator theorem unproved.
