# Marked history geometry, selector currents and regulator limitations

**Annex BA.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Result and precise scope

The completed scalar C-05 theorem does not by itself complete the marked history reset. Three distinct operations must be separated:

1. The normalized old-component operation in its own fixed native source coordinates. The primary source supplies a pointwise exponential tilt on a common support, including its nonsmall self action. This gives domination for arbitrary marked numerators, not merely for the unmarked scalar integral.
2. Its representation in the actual current coordinates before its hidden variables are integrated. This additionally requires a marked coordinate/gauge identity. The C-05 proof explicitly used exact integration to avoid a pointwise complex-gauge assertion for certain hidden raw fields.
3. Variation of the remaining raw data or the live selector/geometry labels. These changes can move supports and normalizers. Neither a native analytic chart nor a scalar boundary Hessian bound controls them automatically.

The source analysis below identifies an actual selector exception to a blanket gauge-invariance argument. The elementary results proved here give a guarded extension on a product current domain, the exact selector-gluing identity, a quantitative obstruction to bounding the M-03 shifted-history norm from full-law moments, and a necessary payment for a connected response inside a nonsmall component. They are useful checks on an H-03 proof. They are not counterexamples to Yang–Mills.

### 2. The primary pointwise normalized-kernel statement

Fix a component \(X\) and the outer geometry in Balaban's LFR II (1.71)–(1.72). Let \(\eta\) comprise the old component's continuous variables, discrete histories, and graph choices. The real positive unnormalized operation is \(M_0(d\eta)\), including the old self-component action. In the native analytic variables used on printed pp.379–380, the source writes

\[
 M_z(d\eta)=e^{\sigma(z,\eta)}M_0(d\eta),
 \qquad \sigma(0,\eta)=0,
 \qquad \sup_{|z|<\rho,\eta}|\sigma(z,\eta)|\le s.
 \tag{HG18.1}
\]

The support and all the factors outside the exponent are fixed in this particular chart. Printed p.379 says that only the quadratic form in \(B\) and the self term \(V(X^{\sim})\) depend on \((U,J)\); their first-order variation is small uniformly in the variables still integrated. The estimate of \(V(X^{\sim})\) is not an assertion that its value is small. Its value stays in \(M_0\).

The formulas (1.73)–(1.75), printed p.380, apply to an arbitrary function of the integration variables. Thus they justify a marked domination statement in their actual native chart. They do not identify the chart with every possible retained-link variation.

Include the actual cross action \(H_z(\eta)=\sum_{Y\ni X}V_Y(z,\eta)\), with a summable source majorant

\[
 \sup_{|z|<\rho,\eta}|H_z(\eta)|\le\lambda,
 \qquad
 \pi_0(d\eta)=\frac{e^{H_0(\eta)}M_0(d\eta)}{M_0(e^{H_0})}.
 \tag{HG18.2}
\]

The exact old posterior is

\[
 Q_zF=\frac{\pi_0(e^{\Theta_z}F)}{\pi_0(e^{\Theta_z})},
 \qquad
 \Theta_z=\sigma(z,\cdot)+H_z-H_0.
 \tag{HG18.3}
\]

Set \(r_*=\log(3/2)\) and

\[
 \rho_* =\frac{\rho r_*}{s+\lambda+r_*}.
 \tag{HG18.4}
\]

The Cauchy coefficient estimate for the analytic function \(\sigma+H\) gives

\[
 \|\Theta_z\|_\infty
 \le(s+\lambda)\frac{|z|}{\rho-|z|}\le r_*
 \quad (|z|\le\rho_*).
\]

Consequently

\[
 \left|\frac{dQ_z}{d\pi_0}\right|\le3,
 \quad
 |\partial_z^qQ_zF|_{z=0}
 \le 3q!\rho_*^{-q}\pi_0|F|,
 \tag{HG18.5}
\]

and, by summing the Taylor coefficient majorants,

\[
 \sup_{0<|t|\le\rho_*/2}
 \left|\frac{Q_tF-Q_0F}{t}\right|
 \le\frac6{\rho_*}\pi_0|F|.
 \tag{HG18.6}
\]

Indeed \( |\pi_0(e^{\Theta_z})|\ge2-e^{r_*}=1/2\), whereas \(|e^{\Theta_z}|\le3/2\). The Cauchy estimate may then be applied to the density relative to \(\pi_0\), before multiplying by \(F\) and integrating. This proves (HG18.5)–(HG18.6) without assuming that the mark is analytic. Under a full incoming law \(\mu(dx,d\eta)=\nu(dx)\pi_x(d\eta)\), conditional Jensen gives the corresponding \(L^p(\nu)\) bound by \(3q!\rho_*^{-q}\|F\|_{L^p(\mu)}\), when the displayed radius is uniform in \(x\).

These statements recover the HP.1 mechanism on its exact source scope. Higher input vertices and the complete finite reset jet are handled by HP.2–HP.3; no new partition loss is introduced here.

#### What C-05 now supplies, and what it does not identify

C-05 supplies the full \(2P_k\) current contour, a whole strong native ball, normalized endpoint estimates, and a real gauge identity for every scalar primitive with its surviving old arguments fixed. See AB17.8–AB17.13, AD17.3, and CR.2. A uniform factorization

\[
 M_{\chi(z)}(d\eta)
   =e^{\sigma_\chi(z,\eta)}M_{\chi(0)}(d\eta)
 \tag{HG18.7}
\]

on a single padded hidden-variable space, with the source bound in (HG18.1), would apply (HG18.5) to the actual current map \(\chi\). The required checks are that the map lands in the source chart, that its change of variables preserves the common hidden support, and that the transformed numerator is the actual transported numerator. The map may be independent of the mark; its full direct response still has to be carried separately.

One must not replace these checks by the scalar result after integrating \(\eta\). AB17 §2.3 expressly states that fine hidden raw fields inside the completed operation have already been integrated, so no pointwise complex-gauge claim was required there. AB17 §3.2 and CR.2 fix the *surviving* raw endpoints. They do not state (HG18.7) for every hidden endpoint of an arbitrary marked numerator.

### 3. The exact marked gauge-transfer lemma and its source limitation

#### Lemma HG18.1 — marked real gauge transfer before complex continuation

Let \(G\) act measurably on a hidden-variable space. Let \(M_v\) be positive finite measures, and suppose the exact kernel covariance

\[
 M_{v^g}=g_*M_v
 \tag{HG18.8}
\]

holds for a specified real gauge \(g\). If \(F_v\) is a covariant marked family,

\[
 F_{v^g}(\eta^g)=F_v(\eta),
 \tag{HG18.9}
\]

then

\[
 \frac{M_{v^g}(F_{v^g})}{M_{v^g}(1)}
 =\frac{M_v(F_v)}{M_v(1)}.
 \tag{HG18.10}
\]

The same identity holds coefficientwise for the full exponential source jet and its finite logarithm. If a real family \(v(z)\) can be replaced by a source-admitted family \(v(z)^{g(z)}\), where (HG18.8)–(HG18.9) hold for every real \(z\), the source chart can be used to define the holomorphic kernel after this exact real change, provided its stated fixed-support source extension is the one under consideration. Estimates for an arbitrary frozen numerator then follow from (HG18.5). A moving marked family still requires its own coordinate regularity; covariance alone does not make it holomorphic. No change of a compact Haar contour by a complex gauge is used.

**Proof.** Apply (HG18.8) to the numerator and denominator. The pushforward formula and (HG18.9) identify both integrals. Finite jets are finite algebraic combinations of these identities. \(\square\)

For an arbitrary frozen function \(F\), rather than the covariant family (HG18.9), the transformed numerator is \(F\circ g(z)^{-1}\). Its direct finite difference is present. The lemma does not set that term to zero, and it does not say that separate carrier records obtained by an arbitrary localization are individually gauge invariant.

#### The source factors that can be checked directly

Normalized Haar measure is invariant under real left/right gauge multiplication. Relative Lie-algebra variables transform by the adjoint action, which is orthogonal in the source invariant norm. Their norm cutoffs, zero tree constraints, and covariant quadratic forms therefore transform correctly. Group averaging constraints are covariant under the actual restricted fine gauge; the scalar E/R/B action obeys the source's simultaneous real gauge covariance. The localized R reference numerator and denominator must be transformed together. These identities explain why (HG18.8) is a plausible target for a correctly augmented source construction.

They do not check every archived selector.

#### The explicit selector exception

CMP119, printed p.250, immediately after (1.16), distinguishes two invariance statements. The expressions in (1.14)–(1.16) are invariant under the simultaneous fine gauge transformations (1.17), **except for the approximate-fluctuation characteristic function** \(\chi'_0(Q_1)\). That characteristic function is invariant under a gauge of the new coarse field together with its block-constant extension \(u_0\). The source then introduces the free-field split (1.18) so that the problematic selector can be replaced on the regular cells. The general-step counterpart is the use of (3.16)–(3.19).

This is the precise reason an arbitrary smooth residual gauge from the C-05 converter cannot simply be declared to preserve all bad-history selectors. Archived versions of those factors are part of the earlier operations in (2.21) and of the component operation (1.71). Their fixed-component sums or their gauge disintegrations must be checked at the marked level. Gauge invariance of the original Wilson observable alone is insufficient to prove a statement about a conditional kernel whose selector event is not invariant under that gauge.

There are two possible repairs, neither silently assumed here:

- Prove that summing the actual internal histories of the fixed component restores (HG18.8), retaining the eligibility tests and every normalization; or
- Carry the induced selector/support change as a signed-kernel current and prove its required bounds.

The complete regular marginal has already removed its inner selectors in C-07. That theorem is not a proof that every archived component-conditioned kernel has the same support.

### 4. A guarded off-support extension that is genuinely local in current coordinates

The M-03 default reference extension can create an artificial jump outside an active chart. There is a useful repair when a full product current margin has actually been proved.

#### Lemma HG18.2 — product-current clipping

Let the real current coordinates be a finite product of normed finite-dimensional spaces. Suppose a positive probability kernel \(Q_z\) is defined for

\[
 \mathcal D_{2P}=\{z:\ \|z_i\|<2P\text{ for every }i\},
 \qquad P\ge4,
\]

and has a bounded analytic continuation on that product domain. The physical support is contained in \(\overline{\mathcal D_P}\). Define, independently at each coordinate,

\[
 T_i(z_i)=
 \begin{cases}
 z_i,&\|z_i\|\le P+1,\\
 (P+1)z_i/\|z_i\|,&\|z_i\|>P+1.
 \end{cases}
 \tag{HG18.11}
\]

Then \(T\) is the identity on the physical support and on each of its one-coordinate perturbations of size at most one. Each \(T_i\) is \(2\)-Lipschitz in its norm, so the extension \(\widetilde Q_z=Q_{Tz}\) has bounded finite differences whenever \(Q_z\) has bounded first derivatives on \(\overline{\mathcal D_{P+1}}\). The extension introduces no new coordinate dependency: \(T_i\) depends only on \(z_i\).

If for a frozen marked numerator one has

\[
 |D_iQ_zF|\le L_i(F)
 \quad(z\in\overline{\mathcal D_{P+1}}),
\]

then

\[
 |\widetilde Q_{z+te_i}F-\widetilde Q_zF|
 \le2|t|L_i(F).
 \tag{HG18.12}
\]

**Proof.** The radial retraction onto a norm ball has Lipschitz constant at most two: add and subtract the point obtained by using the first radius at the second point, and use the reverse triangle inequality for the norms. Apply the ordinary line-segment derivative bound to the two retracted points. The other conclusions follow coordinatewise. \(\square\)

This can remove a default extension artifact for an already verified product-current kernel. It is not a proof of (HG18.7). It does not give a uniform extension in arbitrary raw retained variables. In particular, radial retraction of an entire strong native field norm would generally depend on every block and hence could create a global carrier; that operation is not substituted for the coordinatewise construction above.

### 5. Exact selector gluing and why normalized branches do not glue by themselves

#### Lemma HG18.3 — unnormalized marked gluing

Let \(r_y(d\eta)\) be a positive finite measure and let \(\chi_h(y,\eta)\ge0\) be a finite partition of unity. Put

\[
 r_{h,y}=\chi_h r_y,
 \quad Z_h(y)=r_{h,y}(1),
 \quad Z(y)=\sum_hZ_h(y)>0.
\]

On active fibers define \(q_{h,y}=r_{h,y}/Z_h(y)\) and \(p_h(y)=Z_h(y)/Z(y)\). For every integrable \(F_y\),

\[
 \sum_h p_h(y)q_{h,y}F_y
 =\frac{r_y(F_y)}{Z(y)}.
 \tag{HG18.13}
\]

Zero-mass branches contribute zero without assigning their conditional means a canonical value. Every derivative or finite difference must be taken on this exact weighted identity. On a smooth common support it includes both \(\sum_h p_hD(q_hF)\) and \(\sum_h(Dp_h)q_hF\). Across hard interfaces it is the unnormalized marked numerators that must glue.

If a replacement is geometry dependent, with fresh density \(k_h(u'\mid y)\), the actual posterior weights are instead

\[
 p_h(u',y)
 =\frac{Z_h(y)k_h(u'\mid y)}{
       \sum_lZ_l(y)k_l(u'\mid y)}.
 \tag{HG18.14}
\]

The fresh factors cancel only inside a fixed-\(h\) old-field conditional expectation. They do not cancel from (HG18.14).

**Proof.** Multiply each active conditional expectation by its weight and cancel \(Z_h\); then sum the unnormalized measures. Formula (HG18.14) is Bayes' formula for the actual joint positive measure. \(\square\)

#### A default extension can fail even when the unsplit law is harmless

Let \(u\) be uniform on \([0,1]\) and, for \(-1/2<y<1/2\), select the branch

\[
 h=1\quad\Longleftrightarrow\quad y>0\ \hbox{and}\ u>1-y.
\]

For \(y>0\), its mass is \(y\) and \(q_{1,y}u=1-y/2\). Extend the inactive kernel for \(y\le0\) by the reference point mass at \(u=0\). The conditional marked function jumps from zero to one at \(y=0\). At \(0<y<1/2\), the allowed increment \(t=-2y\) gives

\[
 \sup_{0<|t|\le1}\left|
       \frac{q_{1,y+t}u-q_{1,y}u}{t}\right|
 \ge\frac{3}{8y}.
 \tag{HG18.15}
\]

On the actual branch law, whose \(y\)-density is proportional to \(y\), the \(p\)-th moment of this envelope diverges for every \(p\ge2\). Yet summing the two branches with their exact weights gives the original conditional mean \(1/2\). Both facts follow by elementary integration.

This example does not prove that a better extension is impossible. Here extending by the point mass at \(u=1\) on the inactive side fixes the discontinuity for Lipschitz marks. It proves that the reference convention and an interior analytic estimate alone do not supply the M-03 finite-difference bound. An actual matching extension or the full weighted gluing must be exhibited.

There need not always be such a continuous extension. The positive two-state unnormalized weights \(y_1^2\) and \(y_2^2\), with mark \(+1\) and \(-1\), give

\[
 Q_yF=\frac{y_1^2-y_2^2}{y_1^2+y_2^2}
 \quad(y\ne0).
 \tag{HG18.16}
\]

The numerator and the two weights are entire, but the normalized mean has different limits along the two axes. A common physical margin is therefore substantive information.

### 6. Full-law moment bounds do not control shifted retained-history envelopes

#### Proposition HG18.4 — one-block regulator and shift obstruction

There is a family of exact positive one-block resets with uniformly bounded incoming M-03 value/direct-difference norm, all unshifted full-law moment bounds of the stipulated degree, and no cross interaction, for which the outgoing M-03 norm is unbounded.

**Construction and proof.** Take the current scale \(h=1\), one Euclidean coordinate \(z\), and one discrete retained label \(y\in\{0,1\}\). Let

\[
 \Pr(y=1)=e^{-n},
 \qquad z=\sqrt n\,y,
 \qquad n\ge1.
 \tag{HG18.17}
\]

Use \(R_{\rm in}=1+z^2\), the exact M-03 elementary translations \(z\mapsto z+t\), \(|t|\le1\), and the discrete replacement of \(y\). Define the degree-one input

\[
 A(z,y)=z^2,
 \quad B_{z,t}=2z+t,
 \quad B_y=0,
 \quad J=0.
 \tag{HG18.18}
\]

The input value envelope is \((|z|+1)^2\), and the direct-difference envelope is at most \(2|z|+1\). The regulator quotients in M.11 are bounded by fixed constants on the entire ambient space. For the averaged value part, the only nonconstant term is controlled by

\[
 \sup_{p\ge1}\frac{n e^{-n/p}}p
 =\sup_{0<x\le n}xe^{-x}\le e^{-1}.
 \tag{HG18.19}
\]

The analogous bound for \(\sqrt n e^{-n/p}/p\) is smaller. The grade-\(3/2\) direct-difference moment is uniformly bounded too, because

\[
 \sup_{p\ge1}p^{-3/2}\sqrt n\,e^{-n/p}
 =n^{-1}\sup_{0<x\le n}x^{3/2}e^{-x}\le C.
 \tag{HG18.20}
\]

Thus the incoming single-carrier M-03 norm is bounded independently of \(n\).

Now integrate \(z\) conditionally on the retained \(y\). The exact normalized kernel is \(q_y=\delta_{\sqrt n y}\), so

\[
 QA(y)=ny.
 \tag{HG18.21}
\]

The output has only the discrete label, hence the specified native output regulator is \(R_{\rm out}=1\). The allowed discrete replacement of \(y\) makes the output sharp value envelope equal to \(n\) at **both** values of \(y\). Its degree-one moment norm is therefore \(n\), already at \(p=1\). The new kernel-current record under the label replacement has magnitude \(n\) as well. Hence the output M-03 norm diverges.

On the other hand, the *unshifted* output moments obey

\[
 \|QA\|_{L^p}=n e^{-n/p}\le p/e,
 \tag{HG18.22}
\]

uniformly. Conditional moment contraction is completely consistent with the failure of the shifted envelope and pointwise regulator. \(\square\)

The example is an abstract positive reset, not the Wilson law. It proves that the stated H-01 identities, unconditional moment estimates, and harmless scalar boundary action do not imply the missing M-03 transport. It also explains why the actual remaining-history normalization matters. Erasing the label \(y\) jointly would give the small constant \(ne^{-n}\); retaining it gives (HG18.21). A proof may choose an exact joint erasure, but it must then estimate the actual posterior (HG18.14), rather than reuse the fixed-label conditional law.

### 7. A nonsmall component needs a genuine connected-carrier payment

The source's normalized component base may contain arbitrary correlations under the currently imported estimates. To isolate the logical implication, take a connected component with two local hidden spins at sites \(x\) and \(y\), at distance \(r\), with law assigning probability \(1/2\) to each of \((+1,+1)\) and \((-1,-1)\). Their individual coordinate footprints and incoming marks are local. Put all cross actions equal to zero. Then

\[
 \kappa(\eta_x,\eta_y)=1.
 \tag{HG18.23}
\]

Every representation of this connected degree-two response by carriers containing the two prescribed anchors has M-03 geometric weight at least \(e^{\kappa(2+r)}\). Indeed \(|X|\ge2\) and \(\mathsf t_h(X)\ge r\); the triangle inequality prevents a sum of absolute coefficients from costing less than the magnitude one of the response. Thus a fixed-constant strong connected-carrier bound cannot be inferred from the cross-interaction estimates alone when the allowed component diameter grows.

The eligible source components have diameter \(O(MR_k)\), so a radius with that explicit running cost is possible. A uniform original M-03 bound needs either an internal marked estimate, a genuine full-law probability payment made before conditional normalization, or a proved alternative carrier representation with the same original requirements. The small masses of the newly summed successful components used in LFR II pp.388–389 have canceled when those same components are normalized conditionally and cannot be spent a second time. Fixed surviving components have a different role: the alternative on p.391 leaves their domains fixed and does not require a tree factor for those domains in that unmarked expansion. The scalar C-05 estimate deliberately uses a weaker exterior-component carrier norm; it does not prove the M-03 exponential volume and connecting-tree bound.

### 8. Application to the conditional law

The following conclusions are justified:

| Item | Scope |
|---|---|
| Arbitrary marked numerator in the source's fixed native component chart | The pointwise tilt and domination are primary-source statements; (HG18.3)–(HG18.6) retain all normalizers. |
| Actual current pullback before completed-component integration | Requires the common hidden-variable identity (HG18.7), or the fully checked marked gauge transfer. C-05's integrated scalar identity alone does not identify it. |
| Product-current off-support convention | Lemma HG18.2 supplies a local clipping repair once the actual full kernel chart exists. |
| Blanket fine-gauge invariance of archived selectors | Invalid as an unqualified inference; CMP119 p.250 states an explicit exception. |
| Erasing geometry/selector labels | Lemma HG18.3 gives the exact weighted posterior and the needed gluing identity. Its actual strong bounds remain to be proved. |
| Pointwise regulator and shifted remaining-history norm | Not supplied by full-law moments; Proposition HG18.4 gives an explicit obstruction to that inference. |
| Exponential connected-carrier payment for nonsmall components | Not supplied by the scalar exterior-component norm or the small cross action alone. |

The remaining source-specific work is therefore concrete: prove the marked common-coordinate identity through the actual archived selectors; control the raw retained/geometry directions, including shifted kernels and regulator transport; and pay the connected-carrier norm with the actual normalized law. The thin interaction expansion of Annex AZ can improve the carrier representation but does not remove these independent requirements.

### Sources

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP **119** (1988), 243–285: printed p.250, (1.16)–(1.18), for the explicit selector covariance exception; (2.21), (2.40)–(2.42), for old operations and scalar primitive covariance; (3.16)–(3.19), for the removal of the old approximate selector on regular cells.
- T. Balaban, *Large Field Renormalization. I*, CMP **122** (1989), 175–202: (1.100)–(1.102), printed p.201, for the localized positive quotient and its cutoff; the relative cutoff is a condition on the actual log coordinate.
- T. Balaban, *Large Field Renormalization. II*, CMP **122** (1989), 355–392: (1.65), printed p.375, for the source prepared-domain map; (1.68)–(1.75), printed pp.377–380, for the self/cross distinction and the positive normalized component tilt; pp.388–389 and (1.103)–(1.104), pp.391–392, for the component-mass and fixed-domain limitations.

All counterexamples in this note test implications between stated abstract estimates. None is asserted to model or disprove the actual Yang–Mills construction.
