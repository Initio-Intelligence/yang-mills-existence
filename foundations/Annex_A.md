# Compact Wilson energy and arbitrary-event estimates

**Annex A.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

This note proves two improvements on the actual compact Wilson probability law. It does **not** prove the inherited low-margin estimate in the complete Balaban history measure, the matching of transported marks to current-scale local fields, or four-dimensional Yang–Mills existence.

1. An exact maximal-tree gauge fixing and an open-box plaquette-frame comparison remove the polynomial factor in the bare inverse coupling from the local energy reserve along the proposed cofinal lattice sequence. The finite-volume correction is explicit.
2. Once an event has probability \(q\), polynomial moment bounds give a marked estimate with \(q\) itself, multiplied by a power of \(m + \log(1/q)\). This applies to inherited events as well as fresh ones. It avoids the stronger, generally false requirement that every original-input-measurable weight inherit the same probability factor.

The first result is an unconditional, interacting, large-fields-retained estimate. The second is a general probability estimate applied to the first result and the exact positive transports. Neither identifies a coarse effective energy with the transported raw Wilson energy.

The source-free inputs are Wilson reflection positivity, the chessboard and conditional-cumulant estimates, and the vanishing raw bad-bridge sector. The fresh-reference argument uses a predictable supermartingale and treats the inherited low-margin remainder separately.

### 1. Conventions and geometry

Let \(N \ge 2\) and

\[
 G=SU(N),\qquad D=N^2-1,\qquad d\ge2,
 \qquad \Lambda_n=(\mathbb Z/n\mathbb Z)^d,
 \qquad V=n^d,
\]

with even \(n \ge 4\). Links and elementary unoriented plaquettes are counted once in positive coordinate orientations. Haar measures are normalized. Define

\[
 s(U)=N-\operatorname{Re}\operatorname{Tr}U
     =\tfrac12\|U-I\|_{\mathrm{HS}}^2,
 \quad S=\sum_p s(U_p),\quad
 Z^P_n(\beta)=\int e^{-\beta S}\,dH,
 \quad e_p=\beta s(U_p).
 \tag{1.1}
\]

Here \(P\) means periodic boundary conditions. The coupling convention is:

\[
 \beta=2Nx_0,\qquad X_B=N\beta=2N^2x_0.
 \tag{1.2}
\]

The results hold for every \(\beta \ge 0\); the asymptotically free trajectory is needed only when applying the cofinal corollary to the proposed Yang–Mills sequence.

We use the open box with the same \(n^d\) vertices and only links whose two endpoints are in that box. Write \(Z^F_n\) for its free-boundary partition function. The counts of independent links after spanning-tree gauge fixing are

\[
 q_P=dV-(V-1)=(d-1)V+1,
\]

\[
 q_F=d(n-1)n^{d-1}-(V-1)
     =(d-1)V-dn^{d-1}+1.
 \tag{1.3}
\]

Thus

\[
 q_P-q_F=dn^{d-1}.
 \tag{1.4}
\]

The difference is a surface term. Keeping this difference, rather than replacing both counts by unspecified multiples of \(V\), is essential.

### 2. Exact gauge-fixed partition-function comparison

#### Theorem 2.1 — matched ultraviolet powers

There are constants \(0<c_\ell\le1\le C_u\), depending only on \(N,d\), such that

\[
 \boxed{
 c_\ell^{q_P}(1+\beta)^{-Dq_P/2}
 \ \le\ Z^P_n(\beta)
 \ \le\ Z^F_n(\beta)
 \ \le\ z(\beta)^{q_F}
 \ \le\ C_u^{q_F}(1+\beta)^{-Dq_F/2},
 }
 \tag{2.1}
\]

where

\[
 z(\beta)=\int_{SU(N)}e^{-\beta s(U)}\,dU.
 \tag{2.2}
\]

All constants are independent of the number of sites and of \(\beta\). In particular, no factor of the form \(\beta^{c V}\) is hidden in a constant.

#### Proof: exact tree gauge fixing

For a connected finite graph choose a root and a spanning tree. Successively change variables by vertex gauge transformations, fixing every tree link to \(I\), while retaining the \(V-1\) tree transport variables as independent group variables. Multiplication and inversion preserve normalized Haar measure. A gauge-invariant integrand does not depend on those tree transport variables, which integrate to one. The resulting integral is exactly the integral over the \(E-V+1\) non-tree links with tree links set to \(I\). No Faddeev–Popov determinant or residual gauge-volume factor occurs in this finite compact change of variables. The root gauge is fixed throughout.

For the periodic graph there are \(q_P\) free links. Choose constants \(r_0 > 0\) and \(c_G > 0\) such that

\[
 \operatorname{Haar}\{U:\|U-I\|_{\mathrm{HS}}\le r\}
 \ge c_G r^D,\qquad 0<r\le r_0.
 \tag{2.3}
\]

This follows from nonsingular Haar density in a coordinate chart at the identity. Restrict each free link to radius \(r = r_0 (1+\beta)^{-1/2}\). A product of four unitaries telescopes, and inverse links have the same distance to the identity. Consequently

\[
 s(U_p)\le 2\sum_{l\in\partial p,\ l\text{ free}}
                  \|U_l-I\|_{\mathrm{HS}}^2.
 \tag{2.4}
\]

Each free link belongs to \(2(d-1)\) elementary plaquettes, so

\[
 S\le 4(d-1)\sum_{l\text{ free}}\|U_l-I\|_{\mathrm{HS}}^2.
 \tag{2.5}
\]

On the restricted event,

\[
 \beta S\le4(d-1)r_0^2 q_P.
\]

Its Haar measure is at least

\[
 (c_G r_0^D)^{q_P}(1+\beta)^{-Dq_P/2}.
\]

After decreasing a fixed positive constant to at most one this proves the first inequality in (2.1).

#### Proof: deleting wrap plaquettes

Delete all plaquettes which cross a periodic seam. Their action terms are nonnegative. The remaining action depends only on the open-box links, and all wrap links integrate to one. Therefore

\[
 Z^P_n(\beta)\le Z^F_n(\beta).
 \tag{2.6}
\]

This comparison is between the unnormalized partition functions. It makes no claim about monotonicity of normalized plaquette observables.

#### Proof: an exactly integrable open-box plaquette frame

The required subset of plaquettes is constructed by induction on dimension. For \(d=1\) the graph is a tree and the gauge-fixed integral is one, so \(q_F=0\).

In dimension \(d\), label one coordinate by \(t=0,\ldots,n-1\). Fix to the identity all links in the \(t\) direction. These links form a forest of open chains. Add a spanning tree in the \(t=0\) slice; together these links form a spanning tree of the full box.

Keep all plaquettes in the \((t,i)\) planes. Also keep the recursively constructed \((d-1)\)-dimensional plaquette frame in the \(t=0\) slice. Delete every other plaquette action. In this gauge the kept temporal plaquette through a spatial link \(e\) has action

\[
 s\big(U_e(t+1)U_e(t)^{-1}\big).
 \tag{2.7}
\]

For each spatial edge, integrate \(U_e(n-1)\), then \(U_e(n-2)\), and so on down to \(U_e(1)\). At each integration the upper member of that chain occurs only in one remaining plaquette factor; Haar invariance gives exactly \(z(\beta)\), independently of the next link below it. The final integral in the \(t=0\) slice is the lower-dimensional frame integral.

There are

\[
 E_{d-1}=(d-1)(n-1)n^{d-2}
\]

spatial edges per slice. Thus the number of factors satisfies

\[
 q_d=(n-1)E_{d-1}+q_{d-1},\qquad q_1=0.
 \tag{2.8}
\]

An elementary induction gives

\[
 q_d=(d-1)n^d-dn^{d-1}+1=q_F.
 \tag{2.9}
\]

Deleting nonnegative action terms increases the integral. The retained frame integral equals \(z(\beta)^{q_F}\) exactly. This proves the third inequality in (2.1).

#### Proof: the one-plaquette Laplace integral

The function \(s(U)\) is nonnegative and vanishes only at \(I\). In a sufficiently small exponential coordinate chart at \(I\), its Hessian is strictly positive and Haar density is bounded above. Hence that part of the integral is at most a constant times \((1+\beta)^{-D/2}\). On the compact complement, \(s\) has a strictly positive minimum \(\delta\); the remaining integral is at most \(\exp(-\delta \beta)\), which obeys the same polynomial upper bound after increasing the constant. This proves the last inequality in (2.1). All constants depend only on the compact group and on \(d\). ∎

#### Corollary 2.2 — local pressure ratio with an explicit surface correction

For every \(\beta'\) in \([\beta/2,\beta]\),

\[
 \boxed{
 \left(\frac{Z^P_n(\beta')}{Z^P_n(\beta)}\right)^{1/V}
 \le C_{N,d}(1+\beta)^{Dd/(2n)}.
 }
 \tag{2.10}
\]

Indeed, (2.1) gives

\[
 \frac{Z^P_n(\beta')}{Z^P_n(\beta)}
 \le C_u^{q_F}c_\ell^{-q_P}
      2^{Dq_F/2}(1+\beta)^{D(q_P-q_F)/2}.
 \tag{2.11}
\]

Now use \(q_P/V \le d\), \(q_F/V \le d-1\), and (1.4). For example, one may take

\[
 C_{N,d}=c_\ell^{-d}C_u^{d-1}2^{D(d-1)/2}.
 \tag{2.12}
\]

The surface correction has not been suppressed in (2.10).

### 3. Constant local reserve on the cofinal Wilson sequence

For a closed unit \(d\)-cube \(C\), let \(E_C\) be the sum of \(e_p\) over all its plaquette faces. Every plaquette belongs to

\[
 M_d=2^{d-2}
\]

such cubes. For a plaquette set \(X\), let \(b(X)\) be the minimum number of closed unit cubes covering it, and let \(E_X = sum_{p \in X} e_p\).

The Wilson site-reflection positivity and closed-block chessboard inequality (Section 8) give, for a set \(A\) of distinct cubes,

\[
 \mathbb E_{\beta,n}\exp\left(\eta\sum_{C\in A}E_C\right)
 \le
 \left[\frac{Z^P_n((1-\eta M_d)\beta)}{Z^P_n(\beta)}
 \right]^{|A|/V}.
 \tag{3.1}
\]

The abstract chessboard input uses even block counts; it does not require a power of two. Shared boundary links are allowed. This is the standard Wilson site-reflection geometry, not a new reflection-positivity assertion about an RG history measure.

#### Theorem 3.1 — cofinal constant reserve

For \(0 \le \eta \le 1/(2 M_d)\) and every plaquette set \(X\),

\[
 \boxed{
 \mathbb E_{\beta,n}e^{\eta E_X}
 \le
 \left[C_{N,d}(1+\beta)^{Dd/(2n)}\right]^{b(X)}.
 }
 \tag{3.2}
\]

If a sequence \((\beta_\nu,n_\nu)\) obeys

\[
 B_*:=\sup_\nu\frac{\log(1+\beta_\nu)}{n_\nu}<\infty,
 \tag{3.3}
\]

then, with \(K = C_{N,d} \exp(Dd B_*/2)\),

\[
 \boxed{\mathbb E_{\beta_\nu,n_\nu}e^{\eta E_X}\le K^{b(X)}}
 \tag{3.4}
\]

uniformly in the cutoff, volume, plaquette locations and shape of \(X\).

**Proof.** In (3.1), \((1-\eta M_d) \beta \ge \beta/2\). Apply Corollary 2.2. For a cover of \(X\), positivity gives \(E_X \le sum_{C \in A} E_C\); minimize the cover. Equation (3.3) gives (3.4). ∎

For \(d=4\), the allowed exponent is any \(\eta \le 1/8\). The particular cofinal geometry

\[
 a_\nu=L^{-K_\nu}\ell_0,\qquad
 T_\nu=2L^{M_\nu}\ell_0,\qquad
 n_\nu=2L^{K_\nu+M_\nu}
\]

satisfies (3.3) if the independently verified AF trajectory gives

\[
 \beta_\nu\le C(1+K_\nu).
 \tag{3.5}
\]

Equation (3.5) is an application hypothesis here, not a newly proved coupling-flow theorem. The reserve theorem itself needs only (3.3).

#### Corollary 3.2 — uniform moments of the raw finite field family

For a stencil with \(b(X) \le v_0\) and \(r \ge 1\), exponential-tail integration gives

\[
 \|E_X\|_r
 \le \eta^{-1}\big(v_0\log K+2r\big)
 \le C_{v_0}r.
 \tag{3.6}
\]

For integer \(r\) one may replace \(2r\) by \(r\). The factor two avoids any need for a sharp real-order Gamma-function estimate.

Let \(C_A\) be any member of a fixed finite plaquette-curvature stencil, formed from Hermitian sine parts of plaquette holonomies, finite parallel transports and fixed linear combinations. Since

\[
 \left\|\frac{U-U^*}{2i}\right\|_{\mathrm{HS}}^2
 \le\|U-I\|_{\mathrm{HS}}^2=2s(U),
\]

unitary parallel transports preserve the norm, and trace Cauchy–Schwarz bounds a bilinear by a constant times the sum of the corresponding plaquette actions. Therefore every fixed component of an energy-normalized bilinear satisfies

\[
 |\beta\,\operatorname{Tr}(C_A C_B)|\le C E_X,
 \qquad
 \|\beta\,\operatorname{Tr}(C_A C_B)\|_r\le Cr.
 \tag{3.7}
\]

In four dimensions the bare physical local field

\[
 O_{\alpha,a}(x)=a^{-4}\beta\,\operatorname{Tr}(C_A C_B)
\]

thus obeys

\[
 \|O_{\alpha,a}(x)\|_r\le C a^{-4}r.
 \tag{3.8}
\]

The same estimate holds after subtracting its expectation, at the cost of a factor two. Additional running mixing coefficients and product subtractions are not silently included in \(C\): they need their own bounds. Most importantly, (3.8) still has the physical cutoff power \(a^{-4}\).

#### Corollary 3.3 — exact all-history average

For every composite frozen positive transport \(Q\) from the Wilson input to an output space containing its actual positive histories,

\[
 \int Qe^{\eta E_X}\,d\mu_{\rm out}
 =\mathbb E_{\beta,n}e^{\eta E_X}
 \le K^{b(X)}.
 \tag{3.9}
\]

Conditional Jensen gives the corresponding \(L^r\) contraction for transported original marks. This uses the actual positive history lift before signed polymer expansion. It does not require a pointwise reserve on each conditioned history, and it does not grant reflection positivity to the history variables.

### 4. Rare inherited histories: a probability factor with a logarithmic cost

#### Lemma 4.1 — optimal-tail form for an arbitrary event

Let \(Y \ge 0\) satisfy

\[
 \mathbb E e^{\eta Y}\le K_0,\qquad K_0\ge1,
\]

and let \(B\) be **any** event of probability \(q\). For \(q > 0\) and \(r \ge 1\),

\[
 \boxed{
 \mathbb E[\mathbf1_B Y^r]
 \le q\,\eta^{-r}
       \big[\log(K_0/q)+2r\big]^r.
 }
 \tag{4.1}
\]

For integer \(r\), \(2r\) may again be replaced by \(r\). When \(q=0\), the left side is zero.

**Proof.** Markov's inequality and the event probability give

\[
 \mathbb P(B\cap\{Y>t\})\le\min(q,K_0e^{-\eta t}).
 \tag{4.2}
\]

Conditional on \(B\), this tail is bounded by that of

\[
 T+Z,\qquad T=\eta^{-1}\log(K_0/q),
\]

where \(Z\) is exponential with rate \(\eta\). Tail integration and Minkowski give

\[
 \big(\mathbb E[Y^r\mid B]\big)^{1/r}
 \le T+\eta^{-1}\Gamma(r+1)^{1/r}.
 \tag{4.3}
\]

For real \(r \ge 1\), comparison with the integer order \(\lceil r\rceil\) bounds the last Gamma root by \(2r\). For integer \(r\), \((r!)^{1/r} \le r\). Multiply by \(q\). ∎

There is no independence, fresh-noise assumption, or conditioning-margin hypothesis in this lemma. In the Wilson application take \(Y=E_X\) and \(K_0=K^(b(X))\). The event may depend on the entire original input, on later auxiliary randomness, or on both, because passing to the joint history coupling leaves the marginal exponential bound on \(Y\) unchanged.

If \(B\) is output-measurable and \(Q\) is the conditional expectation of an original mark given that output, conditional Jensen also gives

\[
 \mathbb E[\mathbf1_B|QF|^r]
 \le\mathbb E[\mathbf1_B|F|^r].
 \tag{4.4}
\]

This can be combined directly with (4.1) when \(F\) is bounded by a power of the original energy.

#### Theorem 4.2 — arbitrary-event bounds from a polynomial moment budget

Suppose marks \(A_1,\ldots,A_m\) satisfy, for all real \(r \ge 1\),

\[
 \|A_i\|_r\le b_i C r^s
 \tag{4.5}
\]

with fixed \(s \ge 0\). For every event \(B\) of probability \(q > 0\), put \(\lambda = \log(1/q)\). Then

\[
 \boxed{
 \mathbb E\left[\mathbf1_B\prod_{i=1}^m|A_i|\right]
 \le q(eC)^m(m+\lambda)^{sm}\prod_i b_i.
 }
 \tag{4.6}
\]

Let \(Q\) be a positive normalized conditional-expectation transport and let

\[
 J_m=\kappa_Q(A_1,\ldots,A_m)
\]

be the corresponding conditional cumulant, equivalently the mixed derivative of \(\log Q \exp(\sum t_i A_i)\) at zero. Then

\[
 \boxed{
 \mathbb E[\mathbf1_B|J_m|]
 \le q(2eC)^m m!\,(m+\lambda)^{sm}\prod_i b_i.
 }
 \tag{4.7}
\]

The same bound as (4.6) holds for the full transported coefficient \(Q(prod_i A_i)\). For that conclusion \(B\) is an event on the output probability space, or any joint probability space extending it. Formula (4.7) has the same interpretation. All these conclusions are zero when \(q=0\).

**Proof.** If \(q=1\), use Hölder with exponent \(m\) for each mark. Otherwise set

\[
 p=1+\lambda/m>1.
\]

Hölder first on the event and then among the \(m\) marks gives

\[
 \mathbb E\left[\mathbf1_B\prod_i|A_i|\right]
 \le q^{1-1/p}\prod_i\|A_i\|_{mp}.
 \tag{4.8}
\]

Here \(mp=m+\lambda\) and

\[
 q^{1-1/p}=q e^{\lambda/p}\le q e^m.
\]

This proves (4.6). Conditional contraction proves the same product-moment bound for \(Q(prod_i A_i)\).

For conditional cumulants the previously proved partition estimate is

\[
 \|J_m\|_p\le m!2^{m-1}\prod_i\|A_i\|_{pm}.
 \tag{4.9}
\]

For completeness, each partition term is a product of conditional moments. Hölder across its blocks, conditional contraction and Hölder inside each block bound its \(L^p\) norm by the displayed product of \(L^{pm}\) norms. The sum of absolute cumulant coefficients is at most \(m!2^{m-1}\), by encoding ordered partitions by a permutation and cuts. Apply the same event Hölder inequality with the chosen \(p\). ∎

For the fields in (3.8), \(s=1\) and \(b_i=a^{-4}\). Thus an arbitrary inherited event of probability \(q\) has the explicit original-mark estimate

\[
 \mathbb E[\mathbf1_B|J_m|]
 \le q C^m m!\,(m+\log(1/q))^m a^{-4m}.
 \tag{4.10}
\]

The probability factor has no fixed Hölder loss. The cost is an explicit logarithmic factor. This is stronger than choosing one fixed \(p>1\) in the earlier rare-history estimate; it is not a spatial-decay theorem or a renormalization theorem.

### 5. Why the fresh weighted factor cannot hold for arbitrary inherited events

#### Proposition 5.1 — exact obstruction

Let \(\mathcal F_0\) be the sigma-field containing the complete original input. For an event \(B\), the following are equivalent:

\[
 \mathbb E[W\mathbf1_B]\le q\mathbb E W
 \quad\text{for every nonnegative integrable }F_0\text{-measurable }W;
 \tag{5.1}
\]

\[
 \mathbb P(B\mid F_0)\le q\quad\text{almost surely}.
 \tag{5.2}
\]

In particular, if \(B\) is \(\mathcal F_0\)-measurable and has positive probability, then (5.1) requires \(q \ge 1\).

**Proof.** The conditional-expectation identity proves \((5.2)\Rightarrow(5.1)\). Conversely take \(W\) to be the indicator of each \(\mathcal F_0\)-measurable set on which the conditional probability exceeds \(q\); a positive-measure such set contradicts (5.1). If \(B\) itself is \(\mathcal F_0\)-measurable, take \(W=\mathbf1_B\). ∎

Consequently the fresh-reference theorem should retain its exact predictable scope. It proves a factor for weights known before the specified genuinely fresh draws because the conditional probability is bounded there. For original-input-determined badness, the same factor for all original weights is generally impossible. An inherited event involving intermediate randomness need not be \(\mathcal F_0\)-measurable; nevertheless (5.2), rather than its unconditional probability, remains the exact requirement for a universal original-weight bound.

The appropriate replacement is the actual averaged estimate (4.6) or (4.7), with a specified polynomial moment class. The original energy reserve supplies such a class. A current-scale matching theorem would have to supply it for the current local renormalized marks.

### 6. What an inherited low-margin theorem still has to prove

The decomposition has the form

\[
 \mathbb E[W\mathbf1_{\{\text{many failures}\}}]
 \le
 \mathbb E[W\mathbf1_{\{\text{many low margins}\}}]
 +w\mathbb EW.
 \tag{6.1}
\]

For the first term there are now two distinct required inputs, rather than a demand for a universal conditional factor:

1. **Actual unweighted geometric probability.** Bound the probability of the specified inherited low-margin event, with its preparatory failures and unreplaced components, in the normalized joint measure of the complete positive Wilson histories. For a multi-component estimate, the bound must retain the dependence on the selected component set or connecting geometry.
2. **Current-scale moment budget.** Match the transported source jets, including responses and remainders, to renormalized current-scale fields or vertices with a bound of the form \(\|A_{\alpha,k}\|_r\le Cb_{\alpha,k}r^s\). The desired physical prefactor is governed by the current scale \(h_k\), not the original cutoff \(a\), after the required local subtractions.

Given those two inputs, Theorem 4.2 supplies their marked combination with no pointwise all-history estimate. For example, if an event indexed by \(D\) has probability \(q_D\), the product estimate is

\[
 \mathbb E\left[\mathbf1_{E_D}\prod_{i=1}^m|A_{\alpha_i,k_i}|\right]
 \le q_D C^m[m+\log(1/q_D)]^{sm}
       \prod_i b_{\alpha_i,k_i}.
 \tag{6.2}
\]

For conditional-cumulant jets add the explicit \(m!\) factor from (4.7). The estimate is directly an averaged bound under the actual normalized law. It does not require the false inequality (5.1) for every possible weight.

Neither required input has been established for the complete low-margin sector here. The constant Wilson reserve makes the original moment budget cleaner, but it does not replace current-scale matching.

#### Rate conditions: why isolated rarity is still insufficient

Write \(t=\log(a^{-1})\). On the indicated weak-coupling trajectory, a representative available isolated-failure probability is

\[
 q_a=\exp\{-c(\log t)^\gamma\}
 \tag{6.3}
\]

for fixed \(\gamma>0\). For every fixed positive \(m,s\),

\[
 a^{-4m}q_a[m+\log(1/q_a)]^{sm}\longrightarrow\infty.
 \tag{6.4}
\]

Indeed the logarithm is \(4mt-c(\log t)^\gamma+O(\log \log t)\), and the linear term in \(t\) dominates. Thus even the improved \(q\) factor does not make an estimate with raw physical fields summable. This is failure of this proposed bound to close the argument, not a proof that the actual correlations diverge.

The previously proved raw bad-bridge sector has the additional probability \(\exp(-c r/a)\) when a bad cluster connects separated supports. That factor can absorb the raw powers and gives coincidence-flat vanishing. A general inherited event is not automatically such a raw connecting cluster: many fine plaquettes below a raw threshold can collectively influence a coarse field.

### 7. Conditions of possible closure mechanisms

| Mechanism | What is established | Additional statement required |
|---|---|---|
| Raw Wilson pressure and chessboard | The constant reserve (3.4), with all original large fields retained | Identification of a later effective energy or margin with a quantity controlled by this reserve |
| Fresh reference randomness | the conditional reserve and predictable rare-failure factor | Probability of low-margin reference centers, preparatory failures and unreplaced components in the outer law |
| Arbitrary inherited event | Marked bound (4.7) once its probability and mark moments are known | Actual geometric event probabilities and a current-scale moment budget |
| Compact conditional energy | A conditional reserve for excess over a conditional minimum | A retained flux can already be bad at that minimum; a bound on excess does not pay that retained flux |
| A larger core for surgery | Geometrically available in parts of the RG construction | An injective or controlled-multiplicity change of the full history, with action gain, boundary compatibility, measure/Jacobian control and the complete reference/counterterm ratio |
| Coarse reflection/chessboard | Original Wilson reflection positivity | A reflection-local pullback of the actual coarse selector and a bound on its fully disseminated constrained partition ratio |
| Frozen observable transport | Exact averages and original-mark \(L^r\) contraction | Localization and cancellation producing current-scale fields plus controlled remainder vertices |

#### Why the coarse chessboard idea is not yet a proof

A deterministic block observable can be reflection positive under the original law if its pullback respects the reflection and the positive-half-space algebra. A positive Markov map alone does not imply this property. The localized R construction additionally has history selectors, backgrounds, retained data and reference draws. Before applying a chessboard theorem to the actual low-margin flag, one must prove that these data yield the requisite local reflection-compatible observable or enlarged probability law.

Even after that is proved, the fully disseminated event inserts constraints into a positive density. Source-free global upper and lower stability bounds, with uncanceled factors proportional to the entire volume, do not by themselves bound the probability of one local event uniformly in the expanding volume. An analogue of the matched partition-ratio calculation in Sections 2–3 is needed for the *constrained coarse effective density*. No such analogue has been proved here.

#### Why retaining the conditional minimum does not pay the outer flux

The existing two-plaquette \(SU(2)\) example fixes a retained product for which a filling under the old wider cutoff exists while no filling under the new sharper cutoff exists. Its conditional fluctuation minimum is regular, and its excess-energy law has good moments, but the sharper failure has probability one at that fixed retained datum. This does not claim that every such datum is an admitted Balaban history. It does show why an estimate only on fluctuations around a fixed conditional minimum cannot replace a probability bound on the retained datum in the outer law.

The published thresholds retain this distinction: LFR I's extension construction uses a wider cutoff; the CMP 119 new cutoff is narrower; and the old allowed last-layer field size used after the R operation is wider still. The implication checked in LFR II is from success of the new cutoff to success of preparatory selectors, not a uniform margin in the reverse direction. Those facts cannot be promoted to a fresh-failure estimate for every inherited center.

### 8. Related literature

Related primary context for the partition powers and multiple reflections is:

Paulo A. Faria da Veiga and Michael O'Carroll, **On Yang–Mills Stability Bounds and Plaquette Field Generating Function**, *Reports on Mathematical Physics* **95** (2025), 303–380, DOI [10.1016/S0034-4877(25)00035-7](https://doi.org/10.1016/S0034-4877(25)00035-7). Preprint: [arXiv:2205.07376v2](https://arxiv.org/pdf/2205.07376), 54 pages.

Its main generating field in equations (30) and (32), printed page 11, is a scaled trace-sine plaquette field, not the full dimension-four bilinear family. For \(SU(2)\) in the fundamental representation the trace of every group element is real, so this particular trace-sine field is identically zero. Remark 16, printed page 30, also mentions an action-based alternative; that remark should not be omitted when describing the paper's scope.

Theorem 4, equation (83), printed page 31, retains different periodic lower- and upper-bound link counts; their surface difference matters in a simultaneous cofinal limit. The present note proves its own explicit correction in (2.10) and checks the sufficient cofinal condition (3.3). No continuum physical-field identification, tensor-family theorem or inherited RG-selector estimate is imported from the paper.

Other published inputs:

- T. Balaban, *Large Field Renormalization. I*, *Communications in Mathematical Physics* **122** (1989), 175–202: the localized R replacement and integral preservation, equations (1.100) and (1.102), and the distinct reference/extension cutoff information.
- T. Balaban, *Large Field Renormalization. II*, *Communications in Mathematical Physics* **122** (1989), 355–392: source-free stability, the normalized reference estimates, and the retained large-field components. Its component activities are not being reinterpreted here as normalized outer event probabilities.
- T. Balaban, *Convergent expansions in lattice gauge theories*, *Communications in Mathematical Physics* **119** (1988), 243–285: the source-free induction and new small-field selector, with the precise domains and cutoffs retained.
- M. Biskup, *Reflection positivity and phase transitions in lattice spin models*, Theorem 5.8, equation (5.34): the abstract even-block chessboard inequality used with the explicitly verified Wilson site-reflection geometry. This import is only the abstract reflection theorem, not an RG-history assertion.

### 9. Remaining theorem statements after the argument

The two improvements remove the bare-coupling loss in the raw reserve on the chosen geometry and the unnecessary fixed Hölder loss in marked rare-event estimates. They do not remove the following missing results:

1. A fully verified J0 trajectory and source-free construction with the stated normalization and admissible cofinal geometry.
2. Actual normalized geometric probabilities for all inherited low-margin, preparatory-failure and unreplaced sectors of the complete positive history law, or a different proved mechanism that controls their marked averages directly.
3. Full transported-jet matching and localization at the current physical scale, retaining every response and remainder generated by the finite field family, with contact subtractions compatible at all orders.
4. Uniform distribution-space and order-growth estimates for that full hierarchy, beyond the raw magnitude bounds proved here.
5. Rotation restoration, uniform short-distance identification/nontriviality, and the separately required operator/phase-transfer estimates.

The gap identified in item 2 is formulated precisely as follows: it is not a need for an impossible universal weighted probability bound at fixed original input. It is a need for a true averaged probability or direct marked estimate under the full normalized law, together with the current-scale information in item 3.


---
