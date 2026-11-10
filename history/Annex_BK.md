# Exact scalar rooted calculus and a full-carrier summation criterion

**Scope: M-04 remains open.** This note proves an incoming analytic scalar budget, an exact rooted numerator/denominator expansion with compatible current records, and a quantitative graded carrier criterion for that expansion. It then identifies the source-specific estimate which that criterion still requires. A finite positive model shows why the established regular-law estimates and a relative carrier bound do not alone imply that missing estimate.

The stated M-04 test is equality with the actual transported scalar \(Q_kF_k\), followed by a remainder estimate in M-03 uniform in scale. The source-dependent definition of \(F_k\), all responses and the actual normalized law remain fixed. In particular a newly inserted coarse plaquette is not substituted for \(Q_kF_k\).

### 1. A genuine incoming budget which the initial scalar satisfies

Let \(h\) be the input spacing, and let \(S\) be the fixed plaquette/link stencil of the F-01 scalar. The repaired scalar component is a fixed nonzero multiple of the Wilson density, by F-01 and the identity \(\operatorname{Tr}\widetilde q_h=2w_h\). A representative centered incoming scalar therefore has the form

\[
 F_h(U)=h^{-4}\alpha\,\beta
       \sum_{p\in\mathcal P(S)}a_p\,s(U_p)-c,
 \qquad
 s(U)=N-\operatorname{Re}\operatorname{Tr}U ,
 \tag{SR20.1}
\]

where the number of plaquettes and the coefficients \(a_p\) are fixed. The exposed coefficient budget is
\(b=|\alpha|+h^4|c|\). The actual finite F-01 normalization coefficients may be inserted into this formula; no uniform bound on their running is asserted.

For a real compact configuration, complexify a finite set of links by

\[
 U_e(\zeta)=
 \exp\!\left(\frac{\zeta_eT_e}{\sqrt{1+\beta}}\right)U_e,
 \qquad |\zeta_e|\le\rho,
 \tag{SR20.2}
\]

where the generators have fixed norm, \(\rho>0\) is fixed and the stencil contains a fixed number of links. Negative orientations use the inverse. The holomorphic extension of \(s\) is
\[
 \mathsf s(P)=N-\tfrac12\operatorname{Tr}(P+P^{-1}).
 \tag{SR20.3}
\]

#### Lemma SR20.1 — local complex energy control

With \(E_S(U)=\beta\sum_{p\in\mathcal P(S)}s(U_p)\), there is a fixed \(C_\rho\) such that

\[
 \sup_{|\zeta_e|\le\rho}|F_h(U(\zeta))|
 \le C_\rho b h^{-4}[1+E_S(U)].
 \tag{SR20.4}
\]

Consequently every ordered \(r\)-fold derivative in the normalized link coordinates at the real center satisfies

\[
 |D^rF_h(U)|
 \le C^{r+1}r!\,\rho^{-r}b h^{-4}[1+E_S(U)].
 \tag{SR20.5}
\]

The constants are independent of \(\beta>0\), \(h\), volume and the real compact configuration.

**Proof.** A plaquette has a fixed number of factors. At a real center the trace of each differentiated generator alone is zero. Subtracting the identity from the remaining compact plaquette gives the first variation bound

\[
 \left|\frac{d}{dt}\mathsf s(P(t\zeta))\bigg|_{t=0}\right|\le
 C(1+\beta)^{-1/2}\sqrt{s(P)}
        \sum_e|\zeta_e|.
 \tag{SR20.6}
\]

Along the complex radial path \(t\zeta\), every compact factor has norm one and every added exponential has norm at most \(e^{C\rho}\). The second variation is bounded by
\(C_\rho(1+\beta)^{-1}(\sum_e|\zeta_e|)^2\).
Taylor's integral formula, multiplied by \(\beta\), therefore bounds the change by
\[
 C_\rho\left[
 \sqrt{\beta s(P)}\sum_e|\zeta_e|
       +\Big(\sum_e|\zeta_e|\Big)^2\right].
 \tag{SR20.7}
\]
Here \(\beta/(1+\beta)\le1\). The finite stencil and \(2ab\le a^2+b^2\) prove (SR20.4), including the identity coefficient. For coordinate-chart derivatives apply multivariable Cauchy on a fixed smaller polydisc. For ordered invariant derivatives with noncommuting generators on the same link, introduce \(r\) ordered exponential increments with individual radius \(\rho/r\). Their total increment size remains bounded by \(\rho\), so the same energy estimate applies. Cauchy then costs \((r/\rho)^r\le e^r r!\rho^{-r}\). This proves (SR20.5) for both conventions. \(\square\)

Thus an incoming one-step hypothesis consisting of actual carrier support, a local complex energy bound such as (SR20.4), its exposed coefficient sum, and the already specified direct/current records is nonvacuous. The microscopic scalar satisfies its analytic part before any conditional expectation is taken. The real moment part follows from the same compact Wilson energy reserve used in M-03. This does not prove that every previously transported scalar already satisfies that hypothesis; propagation of the input budget remains an induction task.

The established NP19.1–NP19.4 estimates control the corresponding real regular conditional value majorant, including the actual retained exterior force and, on a wholly deepest original regular patch, the minimizing reference energy. They do not estimate each absolute marked Gaussian/cluster term separately. That distinction is retained below.

### 2. The exact rooted identity

Fix one geometry and one actual source-free regular integral. After the source's Gaussian and localizations, write the zero-source polymer gas as

\[
 \Xi(v)=\sum_{\Gamma\ {\rm compatible}}
                    \prod_{\gamma\in\Gamma}H_\gamma(v).
 \tag{SR20.8}
\]

Every activity includes its full field and history dependence. Let \(v\) denote the actual retained variables, rather than only the native analytic parameters used to estimate them. Compatibility is the source relation: two localization domains cannot share a cube or a cube wall. Fixed collar enlargements can be used to express this as intersection of connected covers.

For a localized incoming mark \(F\), carry that mark through the same Gaussian integrations and localizations. Denote the one-root activity by \(R_Z(v)\). In the source numerator this is \(H'(Z)\), with exactly one marked integrand. No minimizing field or integration map is changed by the mark. The numerator has the form

\[
 \mathcal N_F(v)=
 \sum_Z R_Z(v)\,
 \Xi_{\not\sim Z}(v),
 \tag{SR20.9}
\]

where \(\Xi_{\not\sim Z}\) contains only background polymers compatible with \(Z\). This is the structure of CMP119 (3.44). The mark is linear in this construction. Every finite analytic input for which the localization is performed has this identity at finite cutoff; its uniform marked bound is a separate matter.

Let
\[
 \log\Xi(v)=\sum_B E_B(v)
 \tag{SR20.10}
\]
be the convergent connected cluster representation, with complete activity tags retained. Removing all polymers incompatible with \(Z\) deletes precisely those connected clusters containing at least one such polymer. Denote that subfamily by \(B\bowtie Z\); the detailed cluster tag is kept if its union alone does not encode the incidence. Then

\[
 \frac{\Xi_{\not\sim Z}(v)}{\Xi(v)}
   =\exp\!\left[-\sum_{B\bowtie Z}E_B(v)\right].
 \tag{SR20.11}
\]

#### Proposition SR20.2 — actual rooted carrier identity

Whenever the corresponding marked series converges absolutely,

\[
 Q_vF_v
 =\sum_Z\sum_{n\ge0}\frac1{n!}
     \sum_{B_1,\ldots,B_n:\, B_i\bowtie Z}
       R_Z(v)\prod_{i=1}^n[-E_{B_i}(v)] .
 \tag{SR20.12}
\]

Each displayed term is a function on the actual carrier
\[
 X=Z\cup B_1\cup\cdots\cup B_n
 \tag{SR20.13}
\]
with fixed connecting collars included. This assertion requires the factors in that term to have those actual supports. It follows from multiplication of the factors, not from a support property of their numerical bounds.

**Proof.** Divide (SR20.9) by (SR20.8), use the connected cluster identity (SR20.11), and expand the last exponential. Each \(B_i\) is connected internally and meets the root under the stated compatibility relation; hence their covered union is connected. A function depending on the coordinates of each factor depends on their union. Absolute convergence permits the resummation. The same computation is valid first as a formal first-order marked source coefficient; a quantitative sufficient convergence criterion is proved in Section 4. \(\square\)

The primary construction CMP119 (3.44)–(3.47), pp.277–278, already performs this numerator/denominator cancellation for its specified action-response insertions. CMP116, Section 2, first localizes the Gaussian expressions in their external variables and then bounds the integrals before the polymer resummation. Its unmarked Gaussian majorant is the appropriate place to insert a root with (SR20.4). Neither source states the M-03 marked operator bound proved conditionally in Section 4.

If the regular density has already used LFR II (1.103)–(1.104), its entire boundary exponential and normalized fixed-component operations are inside the baseline of (SR20.8). A root numerator must use that same baseline. Moving one of those factors into an unrelated reference law changes \(Q_vF_v\).

### 3. Compatible direct and normalized-kernel currents

Write
\[
 R_Z(v)=\mathcal R_{Z,v}(F_v)
 \tag{SR20.14}
\]
for the linear marked-root integration/localization operator. On a common padded family of records, let the incoming exact difference be
\(\delta_\tau F=B_\tau^F+J_\tau^F\).
The root records are

\[
 \begin{split}
 B^R_{Z,\tau}
 &=\mathcal R_{Z,\tau v}(B_\tau^F),\\
 J^{R,{\rm old}}_{Z,\tau}
 &=\mathcal R_{Z,\tau v}(J_\tau^F),\\
 J^{R,{\rm new}}_{Z,\tau}
 &=\frac{\mathcal R_{Z,\tau v}-\mathcal R_{Z,v}}{t}(F_v).
 \end{split}
 \tag{SR20.15}
\]

For discrete changes take \(t=1\). These formulas include every change of the root operator's density, support, localization, geometry and normalizer. In particular
\[
 \delta_\tau R_Z
 =B^R_{Z,\tau}+J^{R,{\rm old}}_{Z,\tau}
                     +J^{R,{\rm new}}_{Z,\tau}.
 \tag{SR20.16}
\]

Set \(e_B=-E_B\). For a tagged term of (SR20.12), suppress its factor \(1/n!\) temporarily and write \(A=R_Z\prod_i e_{B_i}\). Its compatible records are

\[
 B^A_\tau=B^R_{Z,\tau}\prod_i e_{B_i}(\tau v),
 \tag{SR20.17}
\]

\[
 \begin{split}
 J^A_\tau
 ={}&(J^{R,{\rm old}}_{Z,\tau}+J^{R,{\rm new}}_{Z,\tau})
                  \prod_i e_{B_i}(\tau v)\\
 &+R_Z(v)\sum_{j=1}^n
        \delta_\tau e_{B_j}(v)
        \prod_{i<j}e_{B_i}(\tau v)
        \prod_{i>j}e_{B_i}(v).
 \end{split}
 \tag{SR20.18}
\]

#### Proposition SR20.3 — exact compatible rooted records

For every tagged term,
\[
 \delta_\tau A=B^A_\tau+J^A_\tau .
 \tag{SR20.19}
\]
The first line of (SR20.18) retains old and new root currents separately; its second line is the denominator-cluster response. Summing them gives the exact normalized-kernel current, including the centering contribution from the denominator.

**Proof.** Add and subtract \(R_Z(v)\prod_i e_{B_i}(\tau v)\), and use the finite telescoping product identity on the remaining product. Substitute (SR20.16). This proves (SR20.17)–(SR20.19) for finite differences, without a smooth-score assumption. \(\square\)

If a history change alters the allowed polymer family or compatibility relation, pad the families and include the corresponding zero/one indicators in the factors before differencing. More explicitly replace \(e_B\) by
\(e_{Z,B}(v)=-\mathbf1_{\{B\bowtie_v Z\}}E_B(v)\), with the full footprint of that indicator included. Its difference, not only the difference of \(E_B\), occurs in (SR20.18). There can also be indicators inside the root operator in (SR20.15). No bound for these new terms follows merely from the displayed identity. On an admitted fixed geometry all indices are unchanged and this complication is absent.

For these formulas to produce valid M-03 triples on carrier \(X\), the declared support must include the footprints of all its value and current factors and every direction on which the separate records depend. A cancellation \(B+J=0\) does not permit deleting nonzero separate records.

### 4. A full M-03 bound from rooted pre-normalization estimates

This theorem is a quantitative criterion. Its hypotheses concern the actual pre-normalization root activities and complete background cluster activities, not merely the final conditional value.

Use the exact M-03 functions \(v_{h',1,Z}\), \(g_{h',1,Z}\), \(j_{h',1,Z}\), the actual outer law \(\mu_{h'}\), and the full native regulator. Let \(r_Z\) be the sum of these three quantities for the compatible root triple, keeping old and new current parts separately in the sum. The root's first source order has value grade one and current grade \(3/2\).

For a background cluster define
\[
 a_B=\sup_v |E_B|^\sharp(v).
 \tag{SR20.20}
\]
Let \(D_B^\natural\) be its summed finite-difference envelope, exactly as in M-03, and put
\[
 c_B=\mathfrak m_{1/2}(D_B^\natural;\mu_{h'})
    +2^{1/2}\sup_v
           \frac{D_B^\natural(v)}{\widehat R_{h',B}(v)^{1/2}} .
 \tag{SR20.21}
\]
The constants and physical \(h'^4\) factor remain in the root norm; no such factor is attached to the zero-source action. All suprema in this section are on the specified ambient versions and include every M-03 elementary shift. Restriction to an admitted chart alone would give only that restricted conclusion.

Use fixed connected covers so that incidence is realized by intersection. Equivalently retain a fixed collar constant \(C_{\rm inc}\). Suppose
\[
 \begin{split}
 \sup_b\sum_{B\ni b}w_{h',\kappa}(B)a_B&\le\varepsilon_0,\\
 \sup_b\sum_{B\ni b}w_{h',\kappa}(B)c_B&\le\varepsilon_1,
 \end{split}
 \tag{SR20.22}
\]
and
\[
 \mathcal B_{\rm root}
   :=\sum_Zw_{h',\kappa+\delta}(Z)\,r_Z<\infty,
 \qquad C_{\rm inc}\varepsilon_0\le\delta/2 .
 \tag{SR20.23}
\]
The constant \(\varepsilon_1\) need not be small.

For the geometry-dependent factors just specified, use their actual carrier bounds \(a_{Z,B},c_{Z,B}\) instead. The exact sufficient replacement for (SR20.22) is
\[
 \sum_Bw_\kappa(B)a_{Z,B}\le
           C_{\rm inc}\varepsilon_0|Z|,
 \qquad
 \sum_Bw_\kappa(B)c_{Z,B}\le
           C_{\rm inc}\varepsilon_1|Z|,
 \tag{SR20.22a}
\]
for every root, with complete indicator/direction footprints included and each declared factor carrier meeting the root cover. This is a hypothesis to be verified, not a consequence of padding. In the fixed-geometry case (SR20.22) implies (SR20.22a) by counting incident blocks. The proof below uses only the latter two sums, so covers both cases.

#### Theorem SR20.4 — full graded rooted summation

The tagged expansion (SR20.12), with records (SR20.17)–(SR20.18), converges in the actual M-03 norm and obeys

\[
 \|\mathbf QF\|_{h',\kappa}
 \le C\left(1+\frac{\varepsilon_1}{\delta}\right)
                 \mathcal B_{\rm root}.
 \tag{SR20.24}
\]

The constant is independent of cutoff, volume and the number of integrated coordinates. Any fixed one-step conversion \(h'=Lh\) is retained explicitly when estimating \(\mathcal B_{\rm root}\) from an incoming norm; it contributes \(L^4\), not an unbounded depth factor.

**Proof.** For intersecting connected covers,
\[
 w_\kappa\!\left(Z\cup\bigcup_i B_i\right)
       \le w_\kappa(Z)\prod_iw_\kappa(B_i).
 \tag{SR20.25}
\]
The same inequality with fixed incidence constants follows by adding the stated collars. Both cardinality and connecting-tree length are subadditive on such a union.

For averaged grades, Hölder gives the exact inequality
\[
 \mathfrak m_{d+e}(FG)\le
                \mathfrak m_d(F)\mathfrak m_e(G).
 \tag{SR20.26}
\]
Indeed choose the two Hölder exponents \((d+e)/d\) and \((d+e)/e\) at each probability moment order \(p\). The two factors become \(((d+e)p)^d\) and \(((d+e)p)^e\). The pointwise regulator grades satisfy the same product estimate because the union regulator dominates each individual regulator and
\(d^de^e\le(d+e)^{d+e}\).

The value envelope of a tagged product is bounded by
\(R_Z^\sharp\prod_i a_{B_i}\).
The direct and root-current envelopes are bounded by their root envelopes times the same product. The remaining term in (SR20.18) is bounded by
\[
 R_Z^\sharp\sum_j D_{B_j}^\natural
                       \prod_{i\ne j}a_{B_i}.
 \tag{SR20.27}
\]
Formula (SR20.26) with \(d=1,e=1/2\), and the corresponding pointwise estimate, give exactly the required current grade \(3/2\). Thus the norm of the tagged product is at most
\[
 C r_Z\left[
       \prod_i a_{B_i}
       +\sum_j c_{B_j}\prod_{i\ne j}a_{B_i}\right].
 \tag{SR20.28}
\]

Every incident cluster touches one of at most \(C_{\rm inc}|Z|\) blocks. Sum the first product over the ordered \(B_i\)'s and \(n\), including \(1/n!\), and use (SR20.22). This costs at most
\[
 e^{C_{\rm inc}\varepsilon_0|Z|}.
 \tag{SR20.29}
\]
The second product sum costs in addition at most
\(C_{\rm inc}\varepsilon_1|Z|\).
Finally,
\[
 [1+C_{\rm inc}\varepsilon_1|Z|]\,
 e^{C_{\rm inc}\varepsilon_0|Z|}
 \le C(1+\varepsilon_1/\delta)e^{\delta|Z|}.
 \tag{SR20.30}
\]
The spare \(\delta\) in (SR20.23) pays this factor. Summing the root carriers proves (SR20.24), with absolute convergence of the separate records. The convergent series therefore represents the same exact conditional value and compatible currents. \(\square\)

This result solves the support issue **when its actual factor hypotheses have been verified**. It does not infer those hypotheses from a pointwise bound on \(QF\). In particular (SR20.23) is an intermediate marked Gaussian/localization estimate still to be proved from the genuine incoming budget in Section 1; it is not being renamed an incoming hypothesis to declare M-04 complete.

### 5. Why the retained fixed-component gap is substantive

The established scalar C-05/C-08 construction controls native current endpoints and source relative carriers. The alternative LFR II (1.103)–(1.104) leaves fixed residual components \(Y\) in its scalar action. Printed p.391 explicitly removes their internal tree cost because their domains are not summed in that expansion. That is adequate for the source's scalar logarithm and the previously proved current-position estimates.

For (SR20.22), however, a factor depending on all raw variables in \(Y\) has the full physical carrier \(Y\), even if its current endpoint lies outside it. A small coefficient \(e^{-cR}\), where \(|Y|\) can be of order \(R^4\), does not by itself pay \(e^{\kappa|Y|}\). The small scalar multiplier \(T'_k(Y)1\) remains in the outer probability law; it cannot pay the pointwise part of a normalized conditional mark merely by being small.

The following exact example shows that this is not resolved by the already established regular conditional moment estimates.

#### Proposition SR20.5 — a sharp full-carrier diagnostic

Let \(Y_R\) be a connected four-dimensional cube with \(N_R\asymp R^4\) sites, at distance comparable to \(R\) from the integrated root. Let \(\sigma_j\in\{-1,1\}\), \(j\in Y_R\), be retained discrete coordinates. Join \(Y_R\) to the root by a fixed thin path. Take \(P_R=R+2\), fix \(a>0\), and put
\[
 \chi_R(\sigma)=\prod_{j\in Y_R}\sigma_j,\qquad
 \vartheta_R(\sigma)=\tfrac12(1+\chi_R(\sigma)),\qquad
 \epsilon_R=\frac{e^{-aR}}{8P_R^2}.
 \tag{SR20.31}
\]
At an anchored integrated site take the positive truncated conditional law
\[
 q_\sigma(dz)=
 \frac{\mathbf1_{[-P_R,P_R]}(z)}{Z_\sigma}
 \exp\!\left[-\tfrac12z^2+
          \epsilon_R\vartheta_R(\sigma)z^2\right]dz .
 \tag{SR20.32}
\]
Give \(\sigma\) its uniform outer law. This defines a finite-dimensional positive probability model with compact product support for the integrated variable, matching the support structure used in C-07. The root mark is \(F(z)=z^2\).

The integrated law has a fixed coercivity gap, zero mean, uniformly Gaussian moment bounds and a perturbation with Hessian at most \(2\epsilon_R\). On its entire product support \(|W|\le e^{-aR}/8\); on the doubled complex current disc it is at most \(e^{-aR}/2\). Its dependence is confined to one current coordinate and one fixed retained set \(Y_R\). If that fixed set's interior has zero carrier cost, the remaining thin path has cost \(O(R)\); choosing the fixed \(a\) larger than its prescribed relative-weight rate gives a uniformly small relative activity bound. The incoming one-mark M-03 norm is uniformly bounded: the input regulator contains \(1+z^2\), the root carrier is fixed, and the mark is independent of every \(\sigma_j\).

Nevertheless every actual carrier representation of the conditional output has M-03 value norm at least
\[
 c\,e^{\kappa N_R}\epsilon_R ,
 \tag{SR20.33}
\]
which is unbounded as \(R\to\infty\). The output native regulator is one because no continuous energy coordinate survives.

**Proof.** Let \(m_P(s)\) be the second moment of the normalized density proportional to \(e^{-z^2/2+s z^2}\) on \([-P,P]\). Differentiation on this fixed compact support gives
\[
 m_P'(s)=\operatorname{Var}_{P,s}(z^2).
 \tag{SR20.34a}
\]
This variance is bounded below by a fixed positive constant for every \(P\ge2\), \(0\le s\le1/8\). To see this, the two events \(|z|\le1/4\) and \(1\le|z|\le5/4\) have probabilities bounded below uniformly: their intervals have fixed length, their density numerators have fixed positive lower bounds, and the normalizer is bounded above by the full Gaussian integral with exponent \(-3z^2/8\). On two independent copies lying in these two events the difference of their squares is at least \(15/16\). The identity
\(\operatorname{Var}(z^2)=\tfrac12\mathbb E[(z^2-z'^2)^2]\)
proves the lower bound.

The exact conditional value consequently has the form
\[
 Q_\sigma F
 =a_R+b_R\chi_R,\qquad
 b_R=\tfrac12[m_{P_R}(\epsilon_R)-m_{P_R}(0)]
       \ge c\epsilon_R ,
 \tag{SR20.34}
\]
with \(a_R=\tfrac12[m_{P_R}(\epsilon_R)+m_{P_R}(0)]\).
For any function independent of at least one coordinate of \(Y_R\), its Walsh coefficient against \(\chi_R\) under the uniform measure is zero. Hence in any representation \(QF=\sum_XA_X\) by actual supported functions, only carriers containing every site of \(Y_R\) can contribute the nonzero coefficient
\(b_R\).
Its magnitude is at most the sum of the suprema of those \(A_X\)'s. Each such carrier has weight at least \(e^{\kappa N_R}\), and its shifted output regulator is exactly two. The pointwise value term in M-03 therefore proves (SR20.33). This reasoning applies to any absolutely summable representation, not only to the reference-point decomposition.

For the input, the normalizer is bounded below by its integral over \([-1,1]\), while its density numerator is bounded above by \(e^{-3z^2/8}\). Thus \(\|z^2\|_p\le Cp\) uniformly, including all \(p\ge1\). Its unit-shift value envelope is bounded by \(C(1+z^2)\), on the full ambient Euclidean extension. Its direct finite-difference envelope is at most \(2|z|+1\), with no discrete direction contribution. Both its averaged grade \(3/2\) and the corresponding pointwise native-regulator quotient are uniformly bounded; its incoming current record is zero.

Finally \(e^{\kappa N_R}\epsilon_R\) diverges because \(N_R\asymp R^4\) and \(P_R=R+2\). Subtracting an identity term or any fixed local scalar readout depending on a proper subset of \(Y_R\) leaves the highest Walsh coefficient unchanged, so that subtraction cannot remove the lower bound for the remainder. \(\square\)

This is not a Yang–Mills counterexample. It proves that the regular coercivity/moment estimates, a small native-current perturbation, a small integration core and a relative fixed-component bound do not imply the full physical carrier assertion. Actual localization of the retained dependence, or an actual coupling which retains a small unnormalized mass in each marked term, is additional information.

### 6. Exact status of M-04

The root expansion (SR20.12) and the separate current formulas are exact and give genuine function supports. The full graded summation theorem shows precisely how those supports and a source-sized absolute root estimate would yield the M-03 bound. The initial scalar has a verifiable incoming analytic energy budget.

The following source applications remain unproved:

1. A termwise marked Gaussian/localization estimate (SR20.23) from that incoming budget, on the same full density as C-08, including every background, E/B/R and coarea contribution. A bound for the whole conditional expectation from NP19 does not bound its absolute localized terms.
2. The full physical version of (SR20.22) for the actual residual fixed-component dependence, together with every ambient raw, selector and history current. The source's relative fixed-Y norm is not that version.
3. The same exact output's scalar/identity extraction in the specified F-01 reference basis, with the resulting remainder and all its records bounded in M-03. This must use the output proved in the first two steps, not a native replacement field.

The sufficient root criterion does not complete M-04, and the diagnostic example does not disprove the actual model. **M-04 remains open as stated.**
