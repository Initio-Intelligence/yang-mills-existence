# A phase cone for a partially integrated prefix

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

This note treats the direct dependence of an inherited boundary scalar on an old **real** fluctuation coordinate that a later preparation integrates. It proves a bounded normalized pure-kernel operation on those coordinates. It does not identify that pure operation with an interacting posterior, and it does not infer a norm for arbitrary complex walk-decoupled Gaussian measures.

The exact source is LFR I (1.25), (1.53)–(1.60), pp. 182, 187–189; the free-coordinate convention is CMP119 p. 249. The quadratic coefficient input is CMP99 Section B, pp. 399–405, together with the actual constrained precision and principal inverses in its Section E. The already checked OR17/PF results specify these operators on the actual prepared history.

## 1. The direct old-coordinate issue

An inherited scalar may have the form

\[
 F(\xi,a_h,\ldots,a_{b-1};a_{\rm ext}),
 \qquad \xi=(U,J),
 \tag{P1}
\]

where the displayed fluctuation coordinates are real, the older exterior variables are fixed, and \(F\) is holomorphic in the admitted native pair. The bound on \(F\) is uniform for the real fluctuation variables on their actual cutoff support. No holomorphy in the \(a_j\) is required.

The native patch Taylor estimate cannot replace integration of a directly occurring \(a_j\). We instead retain \(F\) as one bounded test function and normalize the literal pure quadratic part of the partial source integral. All inherited boundary terms, and the nonlinear effective-action terms treated by the ordinary cluster construction, remain in the interaction exponential. The denominator introduced here is retained explicitly.

## 2. Exact free coordinates and support

At each stage \(j=h+n\), LFR I (1.60) has two integrations:

\[
\begin{split}
 &\int da_j\big|_{Z_{j+1}\cap\Omega_{j+1}}\,
       \chi^{(j)}(Z_{j+1}\cap\Omega_{j+1})\,
       e^{-\frac12\langle a_j,C_j^*
                    \Delta_{\Lambda_{j+1}}^{(j)}C_j a_j\rangle},\\
 &z^{(j)}\int db_j\big|_{\Omega_{j+1}^c\setminus Z''_{j+1}}\,
       \chi'^{(j)}
       e^{-\frac12\langle b_j,C_j^*\Delta^{(j)}C_jb_j\rangle+\cdots}.
\end{split}
\tag{P2}
\]

The omitted terms are the displayed \(P^{(j)}\), the differences of \(E,R,B,B^{(n)}\), and the displayed Wilson-action difference in (1.60). This is an exact source split, not a replacement of the Wilson law by a Gaussian.

CMP119 p. 249 defines the integration variable \(A\) **after** solving the linear averaging delta constraints. On a fixed set of exceptional bonds, the constrained field is \(A'=C(U)A\), \(Q(U)C(U)A=0\); the remaining free bonds carry the independent real variable \(A\). The Jacobian of the eliminated constraints is \(z^{(j)}\). Consequently source analyticity of \(B(U,J,A)\) with real \(A\) fixed is already analyticity in these independent free coordinates. There is no additional substitution of a complex \(A\) into an arbitrary bounded old function.

The source manipulations preceding (1.60) matter:

1. The factor \(\chi_k^{(n+1)}\) is explicitly independent of the variables of the current integral, by the text following (1.25), and remains outside it.
2. Equations (1.28)–(1.29) remove the earlier background-dependent restrictions on the successful branch. The remaining old-field restriction is (1.9), a restriction on the free real \(A_j\).
3. The new successful restriction \(\chi'^{(j)}\), (1.55), is a restriction on the free real \(B_j\). Only its actual upper bound is needed below; both old and new rescaled variables obey \(|a_j|,|b_j|\le C P_j\).
4. On a failed selector the change preceding (1.59) acts on the newly introduced \(B_j\), not on an independently retained old \(A_j\). The resulting selector (1.59) is explicitly independent of background fields. Its analytic Jacobian and action displacement are the PF terms and must be retained. A stopped prefix contains only the earlier successful integrations; the failed displacement is kept in its actual remaining factor.

Thus a fixed history branch has a common finite-dimensional real support for its successful partial integrations. The discrete history/selector labels are not analytically differentiated. If a source decomposition sums such labels, the same statement applies on their disjoint union.

If a displayed \(P^{(j)}\) term contains a genuine degree-two cross term in the independent \(A_j,B_j\), that term must be placed in the full constrained quadratic form when this split is used. Its label \(P^{(j)}\) is not a reason to treat it as small. This reassembly uses the actual constrained/Schur precision; it does not introduce a new covariance. Cross-component quadratic pieces that the source has already assigned to the boundary interaction stay there and are not counted again.

## 3. Elementary phase-cone lemma

Let \(D\) be a common parameter domain and \(\mathcal A\) a fixed finite-measure real support. Suppose \(w_\xi(a)\) is a measurable density, holomorphic in \(\xi\) for almost every \(a\), with local integrable domination. Suppose, for every \(\xi\in D\), there is a scalar angle \(\theta(\xi)\) such that on the positive support

\[
 w_\xi(a)=|w_\xi(a)|e^{i\phi_\xi(a)},\qquad
 |\phi_\xi(a)-\theta(\xi)|\le\eta<\pi/2 .
\tag{P3}
\]

Neither \(|w_\xi|\) nor \(\theta(\xi)\) has to be holomorphic. Assume \(\int |w_\xi|>0\). Set

\[
 \tau(\xi)=\int_{\mathcal A}w_\xi(a)\,da,\qquad
 \Pi_\xi F=\tau(\xi)^{-1}
                 \int_{\mathcal A}w_\xi(a)F(\xi,a)\,da .
\tag{P4}
\]

Then \(\tau\ne0\), \(\Pi_\xi1=1\), and

\[
 \|\Pi_\xi\|_{L^\infty(\mathcal A)\to\mathbb C}
       \le \sec\eta .
\tag{P5}
\]

The operation is holomorphic on holomorphic bounded test families, regardless of their regularity in \(a\).

**Proof.** Rotate the denominator by \(e^{-i\theta(\xi)}\). Its real part is at least \(\cos\eta\int|w_\xi|\). The numerator is at most \(\|F\|_\infty\int|w_\xi|\) in modulus. This proves (P5). Fixed-support dominated integration proves holomorphy of numerator and denominator; division by the nonzero denominator gives holomorphy of the quotient. No lower bound on \(\tau\), no dimension bound, and no continuity of \(F\) in \(a\) enters the operator estimate. \(\square\)

This argument compares the complex measure with its own positive absolute value at each parameter. It therefore needs no Lipschitz estimate for an \(N\)-fold map relative to one fixed real center. The uniform native-chart admission of each actual stage suffices.

The mass is not discarded:

\[
 \int w_\xi e^{V(\xi,\cdot)}
       =\tau(\xi)\,\Pi_\xi e^{V(\xi,\cdot)} .
\tag{P6}
\]

Its holomorphic logarithm, on the source branch, remains in the ordinary action/forcing ledger. If a later variable is still integrated, \(\tau\) is a function of that variable at its actual position in the ordered integral. It cannot be moved outside that integration merely because it has been called a normalization.

## 4. Small phase of the actual pure coefficients

Write \(\widehat\alpha_r\) for a uniform bound on the dimensionless complex parts of the admitted stage backgrounds during the current attempt at scale \(r\), including the source's top-band enhancement:

\[
 \widehat\alpha_r\le Cg_r\ell_r^{q+Q+p_{\rm prep}},
 \qquad \ell_r=\log g_r^{-2}.
\tag{P7}
\]

The exponent is fixed. It includes \(L_0^{2N_0}\), which is at most a fixed polynomial in \(R_r,N_0\) by LFR I p. 192. The source successive-insertion assertion on p. 191, including its current clause, admits every stage on its modified native chart. PF.1 embeds the chosen common strong core. Neither assertion multiplies a fresh map norm once per stage.

The operator input is quantitative. CMP99 Section B proves that complex operators are small perturbations of their real counterparts. For example (3.59), (3.61), and (3.63) contain an explicit \(O(\alpha_1)\); the resolvent identity (3.65) and its following paragraph give all stated kernel bounds for the remainder with this additional small factor. The current correction in the actual precision (3.156), its local free-coordinate map \(C\), and the principal inverse in Theorem 3.15 are part of the same coefficient construction.

In each real local gauge, compact adjoint transformations preserve both the real free coordinates and their cutoff norm. The native field and independent-current complex perturbations are of size \(\widehat\alpha_r\) in the source's weighted operator spaces. Reality of the coefficients at a real native pair and the preceding perturbation estimate give

\[
 \sup_x\sum_y |\operatorname{Im}K_j(x,y)|
       \le C\widehat\alpha_r
\tag{P8}
\]

in dimensionless \(j\)-coordinates. The sum is the actual source row with its native measure before conversion to the independent \(j\)-grid variables. It is not a raw sum over fine lattice points. For a Schur block use its exact constrained principal inverse and the same resolvent bounds. A complex gauge is not used to rotate a real old field in this estimate.

Consequently, if \(D_j\) is the number of free coordinates at stage \(j\),

\[
 \left|\operatorname{Im}
      \frac12\langle a,K_j a\rangle\right|
       \le C\widehat\alpha_r D_j P_j^2 .
\tag{P9}
\]

The estimate includes genuine degree-two cross terms. Any fixed external quadratic factor is kept outside the normalized integral; any actual cross force retained in this base is estimated with its genuine endpoint row and its real cutoff bounds. In particular no artificial \(g_j^{-1}J\,a\) force is introduced by re-expanding around an arbitrary off-minimum background: the constrained criticality cancellation has already been performed in the exact source formula (1.60).

Local coarea factors are nonzero on the same fixed absolute chart and have a logarithm real on the real chart. Their imaginary logarithm has the analogous trace bound \(C\widehat\alpha_r D_j\). Haar factors can be retained in the pure kernel if desired: their local analytic logarithms at the small angular variable \(g_j C_j a\) have the same, or a smaller, bound. If they are left in the ordinary interaction instead, they are estimated there once. A bounded old \(B\)-term is not included in this phase estimate, since its variation on its running analytic ball need not have an extra \(g_r\).

## 5. Sum over a whole admissible partial prefix

Here the complete geometric eligibility condition is essential. LFR I p. 177 requires both the current \(100MR_r\) bound and that the preceding regions inside the chosen component satisfy the corresponding size condition at their own scales; the following sentence identifies the last-\(N_r\) regions as rectangles. The source then uses that geometry in its p. 192 construction of the bounded rectangular \(\Lambda\). On this admitted rectangular history, for one attempted component \(P\),

\[
 D_j\le C(LMR_{j+1})^4 .
\tag{P10}
\]

This is a native \(j\)-grid count, not the number of \(j\)-cells in a current-scale bounding box. The latter would introduce the false factor \(L^{4(r-j)}\). A hypothetical merger family with an unbounded number of widely separated ancestors is not justified merely by the no-new-bad flag; it must also satisfy the actual source size/rectangular-history clause before (P10) is used.

The real preparation choice gives \(N_r\le C\ell_r^{p_N}\), with fixed \(p_N\), by LFR I p. 198 following (1.94). The fixed analytic exponents are chosen afterward. AF comparisons over this finite window make \(R_j,P_j\) polynomially comparable to \(R_r,P_r,\ell_r\). Hence the complete phase of the ordered partial pure density, conditional on any unintegrated later variables, obeys

\[
 \sup_a|\phi_\xi(a)-\theta(\xi)|
 \le C\widehat\alpha_r
          \sum_{j=h}^{t}D_j(1+P_j)^2
        +\eta_{\rm rel}
 \le Cg_r\ell_r^A+\eta_{\rm rel}.
\tag{P11}
\]

Here \(\eta_{\rm rel}\) is the actual PF relocation-Jacobian contribution if such a factor belongs to the retained branch. PF's density/Jacobian bounds give

\[
 \eta_{\rm rel}\le C g_r^{-a}\ell_r^{A'}e^{-cR_r}=o(1).
\tag{P12}
\]

Choose the common coupling ceiling once so that the right side of (P11) is less than, for example, \(1/4\). Equations (P3)–(P5) give

\[
 \|\Pi_{P,[h,t]}^{\rm pure}\|\le\sec(1/4)<2
\tag{P13}
\]

for the complete partial integral. There is one such factor for the whole normalized block, not \(2^{t-h+1}\). This proof is pointwise in the native parameters and uniform in all real old free variables on their actual support.

## 6. Full localization disks: the last directly integrated slot

One must not claim (P13) for an arbitrary directly walk-decoupled precision \(K(s)\). At complex \(s\), such a precision can already have an order-one imaginary part at zero coupling. The native phase proof does not cover that operation.

There is a source-compatible restricted statement for the old direct-coordinate branch. If the incoming scalar was already present at scale \(b\le r-1\), its directly occurring old fluctuation variables have indices \(j\le b-1\). Let \(j_*\) be the last such variable actually integrated in the current prefix. Normalize the partial operation only through \(j_*\), conditional on the later variables. Every integration strip involved then lies in

\[
 Z_{j+1}\cap P\subset Z_b\cap P\subset Z_{r-1}\cap P,
 \qquad j\le j_*\le b-1\le r-2 .
\tag{P14}
\]

The ordinary growth defining the current component supplies a current \(MR_r\) guard between these strips and \(P^c\). Use a source localization excluded set containing the **whole original attempted component \(P\)**. Every walk changed by a localization variable then travels from a displayed integration strip to \(P^c\). CMP116 (1.6)–(1.11) retains a positive part of this distance on the full prescribed disks \(|s_\square|\le e^{\kappa_1}\). The short-walk factor \(e^{16\kappa_1}\) is fixed before the source parameters and strong core are chosen. Thus

\[
 \sup_x\sum_y|K_j(s;x,y)-K_j(1;x,y)|
       \le C\ell_r^B e^{-cR_r}
\tag{P15}
\]

for these actual affected rows, with the corresponding local coarea estimate. Their finite polynomial volume and cutoff sum changes (P11) only by

\[
 C\ell_r^{B'}e^{-cR_r}.
\tag{P16}
\]

This establishes the same bounded partial operation on these **full external-localization disks**. It shrinks only the fixed native core/coefficient ceiling after the fixed localization constants; it does not shrink the source \(s\)-disks.

The conditioning at \(j_*\) is material. The complete prefix may also integrate a top \(B_{r-1}\) in a strip near \(\partial P\), which is not in (P14). That top kernel is not declared to satisfy (P15). After the last direct old slot has been integrated, its resulting bounded scalar is holomorphic in the actual remaining native arguments. Further integrations act on this scalar through their source native-map insertions, and must use the ordinary source expansion and the Q26/PF attachment estimates. Its partial normalization mass remains in the ordinary forcing at its actual location. An activity newly created with an \(A_{r-1}\) slot during the combined current RT step retains its explicit new source records; it is not hidden inside an arbitrary older test to which (P14) would be applied.

### 6.1 A positive excluded halo also protects the top rows

For a genuinely new direct-slot response which has already received its input guard, a broader excluded set removes the top-row restriction. Define a deterministic support footprint \(D(P)\) by adding two current \(MR_r\) layers to the **whole original** component \(P\), including the fixed local operator stencils within that width. Collapse only \(P\) in the quotient metric; \(D(P)\) is not a free-travel region.

Every variable of the whole successful partial prefix lies in \(P\). Its distance to \(D(P)^c\) is therefore at least \(cMR_rh_r\), including variables in the top strip. In the source graded metric this is at least \(c'R_r\). Set the new localization variables only outside \(D(P)\). The CMP116 (1.11) argument permits an arbitrary excluded subset of its localization cubes, so the change in any relevant coefficient row on the full source disks retains the factor in (P15). The actual native row measure and the polynomial eligible coordinate count then give the same phase addition (P16) for the **whole** partial kernel.

The geometry has two separate uses. The physical diameter of \(D(P)\) is \(O(MR_rh_r)\), and its current root-completion cost is \(O(R_r^4)\). These are paid by the already extracted fresh response guard. At the next ordinary step the compatible cover and four added proper-scale layers contain \(D(P)\) plus the fixed stencils. Thus it is a legitimate persistent footprint for a new small failed-prefix record. The source's four-layer reserve is not exhausted: two layers are used here, and the fixed stencil width is absorbed for sufficiently large \(R_r\).

The footprints of two different components may overlap. Such deterministic overlap is not an integration edge and creates no new zero-cost connector. Any ordinary interaction containing actual integration variables in both components remains a marked connecting interaction; it cannot be absorbed into a single-component reference kernel. This preserves the source factorization used by the connected expansion.

This option proves the contour guard for actual pure-coefficient rows of the entire prefix. Applying it to an ordinary-tilted density still requires the separate ordinary scalar phase estimate: localizer-dependent ordinary response terms use their own full-tree/native-map records and the same halo-crossing reserve. No old arbitrary boundary interaction is silently included in the phase cone. The smaller excluded set \(P\) and the conditional statement (P14) remain a valid narrower alternative.

## 7. What the bound supplies, and what it does not

For an old test with a deterministic admitted supremum bound \(A_F\), (P13), or its localization version above, gives

\[
 \left|\Pi^{\rm pure}F\right|\le 2 A_F,\qquad
 \left|\Pi^{\rm pure}F-F_{\rm ref}\right|
       \le 3 A_F
\tag{P17}
\]

when \(|F_{\rm ref}|\le A_F\). An actual current/native dependence in the test is retained. Since \(\Pi^{\rm pure}1=1\), a part exactly independent of all the integrated variables factors out without any norm loss.

For derivatives in a native parameter, on a common interior chart, differentiating the fixed-support integral gives the exact identity

\[
 D(\Pi F)=\Pi(DF)+\Pi(F\,D\log w)
                       -\Pi(F)\Pi(D\log w).
\tag{P18}
\]

This includes the moving normalization. Each coefficient-response insertion can be decomposed with the actual localized source operator rows. It requires no derivative of \(F\) in an old \(a_j\). Higher derivatives can be obtained by Cauchy on the common native/current chart after the bounded scalar and its genuine support majorant have been assembled.

The positive connected expansion must still include the interaction exponential in (P6), its marks, its ordinary forcing mass, and every genuine shared slot. A bounded pure-kernel operation is not a theorem for the arbitrary interacting posterior. The role of this lemma is narrower and exact: it removes the unjustified need for complex old-\(A_j\) analyticity at a later direct averaging operation, and supplies one bounded operation for that block. The component/endpoint guard and the fresh positive record bounds must be supplied by the actual carrier argument, not by the operator norm alone.

## 8. Source checks and limits of the claimed result

The following claims have been checked in the primary text:

| Claim | Source |
|---|---|
| Free variables are introduced after linear delta elimination; the constrained field is \(CA\) | CMP119 p. 249 |
| Source expands at the constrained critical point, so the potentially dangerous linear term vanishes | CMP119 p. 250 |
| Actual successful prefix has the two fixed free-coordinate integrals in (P2) | LFR I (1.60), pp. 188–189 |
| Outer selector is independent of integration variables; remaining successful old/new cutoffs are real-coordinate cutoffs | LFR I after (1.25), (1.29), (1.55) |
| Failed new-field shift produces a background-independent selector | LFR I (1.59), p. 188 |
| Successive insertion is uniform on the modified native spaces, including current | LFR I p. 191 |
| Top-band enhancement is only polynomial in \(R_r,N_0\) | LFR I p. 192 |
| Small complex operator perturbations carry an explicit small native factor | CMP99 (3.59), (3.61), (3.63)–(3.65) and following text |
| Full source localization disks preserve walk decay with one fixed \(e^{16\kappa_1}\) loss | CMP116 (1.6)–(1.11) |

The coefficient statement used here is the existing actual ordinary precision/principal-inverse statement, not an assumed spectral gap of the full Wilson interaction. No independent gap, mixing, or bounded posterior susceptibility is invoked.

The phase-cone and last-direct-slot statements are available as supporting results at this source scope. They do not, alone, complete the remaining interacting positive-transfer assembly of C-05.
