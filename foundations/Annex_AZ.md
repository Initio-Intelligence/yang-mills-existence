# Exact reset-jet interaction carriers and the relative source theorem

**Annex AZ.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

**The H-03 estimate is not closed by this annex.** It concerns the exact reset in the specified physical value/difference/current framework, uniformly over the remaining history. The source-native result below is a substantive additional part of that estimate, but does not yet control the complete M-03 norm.

The new result is an absolutely convergent **thin-carrier expansion of every finite reset jet of the actual normalized old-component posterior**. Each activity is carried by the base component, the actual input footprints and the actual interaction carriers. No entire-radius ball is substituted for their union. The factorial exponent of the incoming source hierarchy is preserved. The source bounds make this expansion uniform in a relative norm which charges the exterior of the nonsmall components. The conditional normalizer and the nonsmall self action remain present throughout.

This improves the radial localization theorem HP.3 of Annex AK: it gives the exact individual carrier series and an explicit sufficient condition for its weighted sum. It also identifies precisely why the completed scalar C-05 theorem does not furnish the stronger marked norm. The primary unmarked expansion uses **unnormalized small-component factors** to pay whole-component volume when those components are summed. Such a factor cannot be reused after normalizing that same component. The alternative normalized expansion keeps the remaining component domains fixed and expressly does not require their own decay factors; it consequently supplies no replacement payment for the stronger marked weight.

The proof is at the declared source-free construction and coupling scope. No new source-free construction or independent asymptotically free trajectory is asserted.

The actual source application in Section 4 is specifically the fixed component operation LFR II (1.71)–(1.72) for which the final primitive bound (1.68) and the eligible-carrier count HL.G3 have been checked. It retains every old variable and internal history still integrated by that operation. It is not asserted for a new, repeatedly normalized carrier geometry with additional surviving older holes merely because the scalar C-05 expansion has a relative norm. The algebraic theorem in Sections 2–3 applies to that later geometry only after its own uniform weighted cross-action sum has been supplied.

### 1. The actual positive kernel and its analytic reference

Fix an eligible component \(X_i\) and a geometry admitted by LFR II (1.71)–(1.72). Let \(\eta_i\) collect all old variables, old history labels, graph choices and local integrations in the positive component operation. Let \(x\) collect its retained native data and the other component variables. Write

Here \(X_i\) is a generic component label in this note; it is not restricted to the primary source's post-split class denoted \(X_j\), as opposed to its retained large-field class \(Y_j\).

\[
 M_{i,x}(d\eta_i),\qquad
 \nu_{i,x}=\frac{M_{i,x}}{M_{i,x}(1)},\qquad
 H_{i,x}=\sum_{Y:\ i\in J(Y)}V_Y(x,\eta_i).
 \tag{HR18.1}
\]

The self-component action \(V(X_i^{\sim})\), the older selectors, local Jacobians and the real reference factors are in \(M_{i,x}\). Its mass is positive on the active sector. No lower bound on that mass is needed. The exact old conditional posterior is

\[
 Q_x(d\eta_i)
 =\frac{e^{H_{i,x}(\eta_i)}\nu_{i,x}(d\eta_i)}
        {\nu_{i,x}(e^{H_{i,x}})}.
 \tag{HR18.2}
\]

The factors from a freshly sampled independent reference field cancel in this old conditional expectation. They do not turn \(Q_x\) into the fresh reference law. Also, if a geometry label itself is forgotten, its conditional probability contains its old mass and replacement likelihood; (HR18.2) is not a license to cancel these factors across different geometries.

Use the actual full-law disintegration

\[
 d\mu(x,\eta_i)=d\bar\mu(x)\,Q_x(d\eta_i).
 \tag{HR18.3}
\]

The outer law may be any of the corresponding actual marginal laws for which the input bounds are stated. A moment estimate after conditioning on a rare sector is not inferred from an unconditional moment estimate. All moment hypotheses below are explicitly for the law in (HR18.3).

#### 1.1 Fixed native charts and pointwise domination

LFR II pp.379–380, (1.73)–(1.75), represents the native analytic deformation of the old operation by a small pointwise exponential on its original fixed positive support. On a sufficiently small admitted native disc \(D_\rho=\{|z|<\rho\}\), after recentering,

\[
 \nu_{i,x,z}(d\eta_i)
 =\frac{e^{\sigma_x(z,\eta_i)}\nu_{i,x}(d\eta_i)}
        {\nu_{i,x}(e^{\sigma_x(z,\cdot)})},
 \quad \sigma_x(0,\eta_i)=0,
 \quad \sup_{x,z,\eta_i}|\sigma_x|\le\log(3/2).
 \tag{HR18.4}
\]

Consequently the mass-one complex measure satisfies

\[
 |\nu_{i,x,z}|\le K_0\nu_{i,x},\qquad K_0=3.
 \tag{HR18.5}
\]

This follows directly from \(|\nu_{i,x}(e^\sigma)|\ge1-\nu_{i,x}|e^\sigma-1|\ge1/2\). The source's self action is included in \(\sigma\); it is not discarded because its unperturbed value is large. The derivative of the component normalizer is included in (HR18.4).

Assume the actual interaction carriers obey the common-disc bounds

\[
 \sup_{x,z,\eta_i}|V_Y(x,z,\eta_i)|\le b_Y,
 \qquad \lambda_0=\sum_{Y:\ i\in J(Y)}b_Y<\infty.
 \tag{HR18.6}
\]

On the real slice \(|H_{i,x}|\le\lambda_0\), so

\[
 \nu_{i,x}\le e^{2\lambda_0}Q_x,
 \qquad |\nu_{i,x,z}|\le K Q_x,
 \quad K=K_0e^{2\lambda_0}.
 \tag{HR18.7}
\]

This domination uses the true normalized posterior as its positive reference and introduces no inverse component mass.

The assertion in (HR18.4) is about the **admitted source-native chart**, with the old integration variables and support fixed. It is not automatically a theorem about every elementary raw retained-coordinate variation in M-03. The completed C-05 proof integrates completed components before making some of its scalar complex-gauge extensions. That scalar extension cannot be reused for an arbitrary marked numerator without a pointwise preintegration map or a justified marked change of variables. This scope issue is discussed again in Section 7.

### 2. Exact expansion of the full source jet

Let \(I\) be a set of \(m\ge1\) distinguished source labels. For nonempty \(B\subseteq I\), let \(A_B(x,\eta_i)\) be the incoming logarithmic-jet coefficient. All such higher vertices are retained. In the square-free finite source algebra, put

\[
 \Psi(t)=\sum_{\varnothing\ne B\subseteq I}t_B A_B,
 \qquad t_B=\prod_{a\in B}t_a.
 \tag{HR18.8}
\]

The exact reset coefficient is

\[
 A_I^+(x,z)=\left.\partial_I
     \log Q_{x,z}(e^{\Psi(t)})\right|_{t=0},
 \quad
 Q_{x,z}(F)=
 \frac{\nu_{i,x,z}(F e^{H_{i,x,z}})}
      {\nu_{i,x,z}(e^{H_{i,x,z}})}.
 \tag{HR18.9}
\]

No convergent exponential of unbounded source marks is assumed. The source algebra is finite; every coefficient uses finitely many moments. The interaction expansion below is a different, genuinely convergent series in the bounded cross action.

For a partition \(\mathcal P\in\Pi(I)\), let \(k=|\mathcal P|\), and let \(\mathbf Y=(Y_1,\ldots,Y_n)\) be an ordered interaction list, allowing repetitions. Define

\[
 a_{\mathcal P,\mathbf Y}(x,z)
 =\frac1{n!}\,
 \kappa_{\nu_{i,x,z}}
       (A_B:B\in\mathcal P,V_{Y_1},\ldots,V_{Y_n}).
 \tag{HR18.10}
\]

For \(n=0\), this is the cumulant of the incoming coefficients under the full nonsmall component base. It is not replaced by a product of one-point means.

#### Proposition HR18.1 — the exact interaction-carrier expansion

If \(2K\lambda_0<1\), with a uniform strict reserve, then

\[
 A_I^+(x,z)
 =\sum_{\mathcal P\in\Pi(I)}\sum_{n\ge0}
        \sum_{Y_1,\ldots,Y_n}a_{\mathcal P,\mathbf Y}(x,z)
 \tag{HR18.11}
\]

whenever the required source moments are finite. Under the weighted and moment hypotheses in Theorem HR18.2, the series is absolutely convergent in the displayed weighted \(L^p\) norms, uniformly on the common native disc.

**Proof.** First replace \(H\) in (HR18.9) by (uH). For \(|u|\le r\),

\[
 |\nu_{i,x,z}(e^{uH})-1|
 \le K_0(e^{r\lambda_0}-1).
 \tag{HR18.12}
\]

Thus the denominator is nonzero on a disc containing \(u=1\) if the common ceiling makes \(\lambda_0\) sufficiently small. For example \(2K\lambda_0\le1/2\) guarantees a nonzero denominator throughout \(|u|\le3/2\), since \(K\ge K_0\ge1\) and

\[
 K_0(e^{(3/2)\lambda_0}-1)
 \le K(e^{3/(8K)}-1)
 \le e^{3/8}-1<1.
 \tag{HR18.13}
\]

For merely \(2K\lambda_0<1\), a smaller \(r>1\) works because \(K_0(e^{\lambda_0}-1)<1\). Integrability of each finite product of input marks and the bounded exponential justify holomorphy of all finite source coefficients. One may equivalently use bounded truncations of the marks and pass to the required finite moments.

Differentiating a normalized exponential tilt gives

\[
 \frac{d}{du}\kappa_{Q_{u,x,z}}(F_1,\ldots,F_k)
 =\kappa_{Q_{u,x,z}}(F_1,\ldots,F_k,H),
 \tag{HR18.14}
\]

for inputs fixed in \(u\). This identity follows by differentiating the finite formal logarithm of the joint moment series; the derivative of its denominator is included. Its \(n\)-fold iteration at \(u=0\), followed by the source partition identity, gives (HR18.10) after multilinearly expanding each copy of \(H=\sum_YV_Y\). The Taylor series at \(u=0\) converges to (HR18.9) at \(u=1\). The absolute bounds in Theorem HR18.2 justify all subsequent rearrangements. \(\square\)

#### 2.1 Actual carriers of the terms

Let \(C_i\) contain the exact source-coordinate footprint of the component base, and let \(S_B\) contain the footprint of the input coefficient \(A_B\). The activity in (HR18.10) is carried by

\[
 X(\mathcal P,\mathbf Y)
 =C_i\cup\bigcup_{B\in\mathcal P}S_B
       \cup\bigcup_{j=1}^{n}Y_j.
 \tag{HR18.15}
\]

If a component base or a source coordinate has a larger actual footprint, it must be added to \(C_i\) or the corresponding \(S_B,Y_j\). No current-link footprint is inferred from a native storage location.

Every non-self interaction in (HR18.10) meets the reset component. The carriers therefore attach to a common base core. The union in (HR18.15) is used literally; no bounding ball is assigned to it. An input coefficient which is independent of the integrated variables is deterministic for this cumulant. Any cumulant of order at least two containing such an argument vanishes. Its sole order-one, \(n=0\) contribution is its unchanged transport. Thus the genuinely generated reset responses attach only to input vertices which depend on the reset variables.

### 3. The weighted all-order estimate

Let \(w\ge1\) be a weight on these declared carrier unions. Suppose its geometric union rule is

\[
 w(X(\mathcal P,\mathbf Y))
 \le W_{\mathcal P}\prod_{j=1}^n w_i(Y_j),
 \qquad
 \Lambda_w=\sum_{Y:\ i\in J(Y)}w_i(Y)b_Y.
 \tag{HR18.16}
\]

Here \(W_{\mathcal P}\) is the exact base/input carrier cost; it is not set to one unless the chosen relative norm really permits that. A convenient finite-family version has \(W_{\mathcal P}\le W_I\) for all partitions of \(I\). An activity-array version follows by summing the input carrier costs before applying the same argument.

Assume the full-law input moment bounds

\[
 \|A_B\|_{L^p(\mu)}
 \le C^{d+1}(d!)^{p_0}\,b^d p^{sd},
 \quad d=|B|,\quad p\ge1,
 \quad p_0\ge1,\quad s\ge0.
 \tag{HR18.17}
\]

These are hypotheses on the incoming current-scale jet, not a claim that its microscopic normalization already has that scale. A reset does not change \(b=a^{-4}\) to \(b=h^{-4}\).

#### Theorem HR18.2 — thin-carrier reset bound with fixed factorial exponent

Suppose (HR18.4)–(HR18.7), (HR18.16)–(HR18.17) hold and

\[
 2K\Lambda_w\le\frac12.
 \tag{HR18.18}
\]

Put \(D=C(1+4KC)\). For every \(m\ge1,p\ge1\),

\[
 \boxed{
 \sum_{\mathcal P,n,\mathbf Y}
 w(X(\mathcal P,\mathbf Y))
 \|a_{\mathcal P,\mathbf Y}(\cdot,z)\|_{L^p(\bar\mu)}
 \le 2W_I D^m(m!)^{p_0}b^m(mp)^{sm}.
 }
 \tag{HR18.19}
\]

The bound is uniform on the native disc. For \(q\ge0\), the same weighted sum of the \(q\)-th native derivatives at its center has the additional factor \(q!\rho^{-q}\). On its inner half-disc, the weighted sum of the supremum finite-difference envelopes has the additional factor \(2/\rho\). Multiple native directions retain their corresponding Cauchy radii and multi-index factorials.

**Proof.** For \(k\) incoming coefficients of degrees \(d_1,\ldots,d_k\) summing to \(m\), a product of conditional moments occurring in the cumulant partition formula is bounded by conditional independent replicas and Hölder:

\[
 \left\|\prod_{D\in\pi}
 Q_x\!\left(\prod_{j\in D\cap\{1,\ldots,k\}}|A_{B_j}|\right)
 \right\|_{L^p(\bar\mu)}
 \le\prod_{j=1}^k
       \|A_{B_j}\|_{L^{pm/d_j}(\mu)}.
 \tag{HR18.20}
\]

Blocks with no incoming \(A\) contribute one after their bounded interaction factors have been removed. Every replica has the original full-law marginal in (HR18.3). No independence between actual old histories is inserted.

With \(r=k+n\), domination (HR18.7), the interaction bounds, and the elementary cumulant coefficient count give

\[
 \begin{aligned}
 \|\kappa_{\nu_{i,x,z}}
   (A_{B_1},\ldots,A_{B_k},V_{Y_1},\ldots,V_{Y_n})\|_p
 &\le (2K)^{k+n}(k+n)!
       \prod_{j=1}^{n}b_{Y_j}
       \prod_{j=1}^k
          \|A_{B_j}\|_{L^{pm/d_j}(\mu)} .
 \end{aligned}
 \tag{HR18.21}
\]

Indeed \(\sum_{\pi\in\Pi_r}(|\pi|-1)!\le r!2^{r-1}\), obtained by encoding ordered partitions as permutations with cuts, and each moment block costs at most one factor \(K\). The relaxed coefficient \((2K)^rr!\) is sufficient for all \(r\ge1\).

After the interaction carrier sum, the series in its length \(n\) is exact:

\[
 \sum_{n\ge0}\frac{(k+n)!}{n!}(2K\Lambda_w)^n
 =\frac{k!}{(1-2K\Lambda_w)^{k+1}}.
 \tag{HR18.22}
\]

This is the step that prevents an unbounded factorial loss from arbitrarily many interaction carriers. It is not a truncation of their number.

By (HR18.17), the last product in (HR18.21) is bounded by

\[
 C^{m+k}b^m(mp)^{sm}
        \prod_{j=1}^k(d_j!)^{p_0},
 \tag{HR18.23}
\]

where only factors \(d_j^{-sd_j}\le1\) have been dropped. Finally,

\[
 k!\sum_{\substack{\mathcal P\in\Pi(I)\\|\mathcal P|=k}}
       \prod_{B\in\mathcal P}(|B|!)^{p_0}
 \le(m!)^{p_0}\binom{m-1}{k-1}.
 \tag{HR18.24}
\]

To see this, order the blocks, then sum over their positive sizes; the left side becomes \(m!\sum_{d_1+\cdots+d_k=m}\prod_j(d_j!)^{p_0-1}\). Each product is bounded by \((m!)^{p_0-1}\).

Put \(v=2K\Lambda_w\le1/2\). Combining (HR18.21)–(HR18.24), the remaining sum is bounded by

\[
 W_I C^m(m!)^{p_0}b^m(mp)^{sm}
 \frac1{1-v}
 \sum_{k=1}^m
    \left(\frac{2KC}{1-v}\right)^k
       \binom{m-1}{k-1}
 \le2W_I D^m(m!)^{p_0}b^m(mp)^{sm}.
 \tag{HR18.25}
\]

All estimates before taking \(L^p\) retain one positive conditional-product majorant independent of the angle of \(z\). Cauchy's formula and Minkowski's inequality therefore apply term by term and to their absolute sum. Summing the Taylor-coefficient majorants on \(|t|\le\rho/2\) gives the factor \(2/\rho\) for the genuine supremum finite-difference envelope. No interchange of an \(L^p\) norm with an uncontrolled supremum is used. \(\square\)

For \(b=h^{-4}\) and \(s=1\), the averaged value grade is exactly the M-03 grade \(h^{-4m}(mp)^m\). A native kernel-current costs the stated inverse radius, and fits the averaged difference/current grade (m+1/2) after retaining that cost. This says nothing yet about the pointwise regulator part or the other retained-coordinate directions of M-03.

### 4. Actual source application in a relative carrier norm

The source geometry here is the fixed eligible geometry of LFR I p.177 and LFR II (1.71)–(1.72), with the coupling and parameter choices retained from the stated source scope. The set \(Z\) and the interaction carriers are the literal ones of that operation, with the final bound (1.68). In particular, this paragraph does not replace \(Z\) by an arbitrary collection of older holes created by repeated alternative normalizations. Let \(R=R_k\). Eligible components are contained in cubes of side \(100MR\), so their physical diameters are \(O(MRh)\), and their numbers of \(M\)-cubes are \(O(R^4)\).

The source cross-carrier bound is

\[
 b_Y\le\alpha_k
    e^{-\kappa_a d_{k,Z}(Y)},
 \qquad \alpha_k\le C e^{-cR},
 \tag{HR18.26}
\]

with a fixed positive rate reserve in \(\kappa_a\). The second inequality is the extraction from the **final completed** carrier in LFR II (1.68), proved as CR.15 in Annex AU. Self terms are excluded from (HR18.26). They remain in \(\nu_i\).

The geometric count HL.G3 gives, for fixed source-admitted geometry,

\[
 \#\{Y:i\in J(Y),\ n\le d_{k,Z}(Y)<n+1\}
 \le C(1+R)^4 A_4^{n+1}.
 \tag{HR18.27}
\]

It counts exterior lattice trees and the fixed component attachments. It does not count arbitrary independent shapes inside a component. Its constants are independent of total volume and of the integrated old-history values.

For this theorem, contract each fixed component interior to a site. Also make the base footprint \(C_i\) free. Charge the remaining \(M\)-cubes and the length of a connecting graph in that contracted graph. Denote these two costs by \(N_i(X)\) and \(\ell_i(X)\). Use

\[
 w_i^{\mathrm{rel}}(X)
 =\exp\{aN_i(X)+\lambda\ell_i(X)\},
 \quad a,\lambda>0.
 \tag{HR18.28}
\]

A fixed small incidence penalty for each included component can be added, if desired. It is paid by the same exterior-tree count. The whole physical interior volume of such a component is not charged by (HR18.28).

All carrier terms attach to the root component. Exterior cube counts are subadditive under union, and their rooted contracted connecting graphs can be joined at that root without an extra interior cost. Hence (HR18.16) holds in this weight with its actual input carrier cost. Rounding the source tree to the \(M\)-grid and traversing it twice gives

\[
 N_i(Y)+\ell_i(Y)
 \le C_4\{1+d_{k,Z}(Y)\}.
 \tag{HR18.29}
\]

The source tree meets every exterior cube; a path of length \(d_{k,Z}(Y)\) meets at most a dimension-only constant times \(1+d_{k,Z}(Y)\) unit cubes. An included component meets the exterior connected set, and becomes a single contracted site. Thus no factor \(R^4\) appears in (HR18.29).

Choose the fixed weights and source entropy reserve so that

\[
 \omega=\kappa_a-\log A_4-C_4(a+\lambda)>0.
 \tag{HR18.30}
\]

This is a parameter-order requirement: choose the source decay constant sufficiently large, then the fixed analysis weights, then the common coupling ceiling. These constants do not run with \(k\) or derivative order. Equations (HR18.26)–(HR18.29) give the actual weighted sum

\[
 \boxed{
 \Lambda_{\mathrm{rel},i}
 =\sum_{Y:i\in J(Y)}w_i^{\mathrm{rel}}(Y)b_Y
 \le C_{a,\lambda,\omega}(1+R)^4e^{-cR}
 \longrightarrow0.
 }
 \tag{HR18.31}
\]

The convergence is uniform in the remaining source-admitted eligible geometry and old history values. Taking the ceiling smaller makes (HR18.18) hold, for example with \(K=6\): the native component density costs at most \(K_0=3\), and \(e^{2\lambda_0}\le2\) for this choice of ceiling.

#### Corollary HR18.3 — the actual source-native relative reset theorem

For the exact old posterior (HR18.2) of the fixed primary operation just specified, under its admitted fixed native chart and the displayed incoming moment/carrier budgets, every source order has the thin-carrier representation (HR18.11). Its relative weighted sum is bounded by (HR18.19), with fixed source factorial exponent \(p_0\), uniformly in total volume, the other admitted component histories in that operation and its integrated internal old histories. Its native kernel derivatives and finite-difference envelopes have the explicit common-chart radius costs from Theorem HR18.2.

This is a spatial estimate: the core has physical radius \(O(MR_kh)\), and the actual exterior connections are exponentially charged. It is stronger than merely bounding an integral or assigning its output to an entire radial ball. It is still a **relative** estimate; the physical interior footprints of all nonsmall components remain free in this norm.

For a repeated scalar-normalization representation with surviving earlier tagged holes, CR.20 gives a useful scalar absolute norm after its specified incidence resolution and chronological bookkeeping. It cannot simply be substituted for (HR18.27): the carrier family, allowed free sets and pointwise marked kernel have to be identified. An application of Theorem HR18.2 to that representation needs its actual resolved-tag weighted sum \(\Lambda_w\) on the preintegration marked chart. That is a concrete additional transfer check, not an extra claim of Corollary HR18.3.

#### 4.1 No component-mass payment has been reused

The proof of (HR18.31) uses the cross-interaction coefficient and geometry, not \(M_{i,x}(1)\). That mass canceled in (HR18.2). The \(n=0\) terms retain all base cumulants. For example, two marks inside the same reset component can have order-one covariance throughout that component, and this is compatible with Corollary HR18.3. The source component radius is kept explicitly.

#### 4.2 Families of fixed geometries retained in the outer law

One need not condition the whole probability measure on one rare geometry. Let \(x=(g,\xi)\), where \(g\) is the actual retained geometry label, and take the full disintegration (HR18.3) on the disjoint union of its active component fibers. Suppose the native radius, the density constant \(K\), the weighted cross sum and the base/input cost \(W_I\) have the uniform bounds displayed above. Apply the local expansion on each fiber, with that fiber's true carriers and its relative weight. Define its absolute envelope by

\[
 \mathcal E_I(g,\xi)
 =\sum_{\mathcal P,n,\mathbf Y}
       w_g(X(\mathcal P,\mathbf Y))\,
       |a_{\mathcal P,\mathbf Y}(g,\xi)|.
 \tag{HR18.31f}
\]

Then, under the **unconditioned** incoming moment hypothesis (HR18.17) for this full law,

\[
 \|\mathcal E_I\|_{L^p(\bar\mu)}
 \le2W_I D^m(m!)^{p_0}b^m(mp)^{sm}.
 \tag{HR18.31g}
\]

No inverse probability of a geometry and no sum of such inverse probabilities occurs. To prove this, use conditional Hölder in each moment block before summing interaction lists. For a fixed input partition \(\mathcal P\), every product of input moments is bounded by the same positive envelope

\[
 \mathcal H_{\mathcal P}(x)
 =\prod_{B\in\mathcal P}
     \left[Q_x|A_B|^{m/|B|}\right]^{|B|/m}.
 \tag{HR18.31h}
\]

All interactions have already been bounded pointwise by their \(b_Y\). The weighted interaction sums can therefore be made on each fiber, using its uniform \(\Lambda_w\), before the \(L^p\) norm. Finally Hölder in \(x\) gives
\(\|\mathcal H_{\mathcal P}\|_p\le\prod_{B\in\mathcal P}\|A_B\|_{pm/|B|}\).
The identical partition count proves (HR18.31g).

This retains the geometry label; it does not average or forget that label. It also does not exchange the norm with a geometry-dependent carrier sum. The global sum of individual carrier \(L^p\) norms can be stronger than the \(L^p\) norm of (HR18.31f). Proving that stronger global M-03 carrier/current sum still requires the actual common carrier representation and its geometry costs. The fixed-geometry estimate (HR18.19) and the full-law envelope estimate (HR18.31g) have deliberately different left sides.

#### 4.3 A discrete current for changing another fixed component history

The thin expansion also localizes an actual class of discrete kernel currents. Keep the outer geometry and native background fixed, and change the old variables/history of one other component \(j\ne i\). This keeps the base \(\nu_{i,x,z}\) fixed, as required by the source factorization, and changes only those cross terms with \(j\in J(Y)\). Freeze the incoming \(A_B\) in this comparison, so that only the newly generated kernel current is being estimated. Put

\[
 \Lambda_{w,ij}
 =\sum_{Y:\ i,j\in J(Y)}w_i(Y)b_Y.
 \tag{HR18.31a}
\]

Let \(\Delta_j a_{\mathcal P,\mathbf Y}\) be the difference of the exact activities in (HR18.10) for these two component histories, on the common chart. Under Theorem HR18.2's hypotheses,

\[
 \sum_{\mathcal P,n,\mathbf Y}w(X)
       \|\Delta_j a_{\mathcal P,\mathbf Y}\|_{L^p(\bar\mu)}
 \le16K\Lambda_{w,ij}W_I
       [C(1+8KC)]^m(m!)^{p_0}b^m(mp)^{sm}.
 \tag{HR18.31b}
\]

The expectation on the right still uses the original actual full law in (HR18.3); no moment estimate under the shifted history is inserted. If the incoming coefficients change as well, their direct and previous-current differences are separate terms under (HR18.41).

**Proof.** Each cumulant in (HR18.10) is multilinear in its interaction arguments. Telescope the \(n\) changed arguments. The \(r\)-th summand has one difference \(\Delta_jV_{Y_r}\), which vanishes unless \(i,j\in J(Y_r)\), and otherwise is bounded by \(2b_{Y_r}\). The other arguments retain their old or new values, each bounded by its same \(b_Y\). Their weighted ordered-carrier sum is therefore bounded by

\[
 2n\Lambda_{w,ij}\Lambda_w^{n-1}.
 \tag{HR18.31c}
\]

The positive reference for the cumulant remains \(Q_x\), since the unchanged base obeys (HR18.7) relative to that reference. With \(v=2K\Lambda_w\), the extra interaction sum is

\[
 4K\Lambda_{w,ij}
   \frac{d}{dv}\frac{k!}{(1-v)^{k+1}}
 =4K\Lambda_{w,ij}
      \frac{k!(k+1)}{(1-v)^{k+2}}.
 \tag{HR18.31d}
\]

Use \(v\le1/2\), \(k+1\le2^k\), and (HR18.24). The same source-partition sum as before gives (HR18.31b). The common positive majorants also give its native derivatives and inner-disc finite-difference envelopes with their previous radius costs. \(\square\)

For the relative weight of (HR18.28), this is a genuine remote-component estimate. If two components have separation \(d_M(X_i,X_j)\), any carrier using both must have relative size at least \(d_M(X_i,X_j)-C R- C\), by the source geometric bound HL.G4. Reserve a fixed half of the rate \(\omega\) in (HR18.30) for this constraint; the remaining half still sums the source entropy. Then

\[
 \Lambda_{\mathrm{rel},ij}
 \le C(1+R)^4e^{-cR}
       e^{-c'[\,d_M(X_i,X_j)-C R-C\,]_+}.
 \tag{HR18.31e}
\]

The comparison changes one actual other-component history on fixed geometry, and its right side is uniform over its allowed old values. It does not compare distinct base geometries, erase a geometry label, or bound the sum over every alternative discrete value in the full M-03 current norm. Those operations have different costs and remain explicit in Section 7.

### 5. The exact stronger carrier test

The original M-03 weight is

\[
 w_h(X)=e^{\kappa[|X|+\mathsf t_h(X)]},\qquad \kappa>0
 \text{ fixed}.
 \tag{HR18.32}
\]

It charges all physical current blocks in the actual dependency footprint, including the interiors treated as free in (HR18.28). To apply Theorem HR18.2 directly in this norm one needs the actual full-footprint union rule and a sufficiently small sum of the form

\[
 \Lambda_{\mathrm{full},i}
 =\sum_{Y:i\in J(Y)}b_Y\,
     e^{\kappa\,\operatorname{cost}_{\mathrm{full},i}(Y)},
 \tag{HR18.33}
\]

together with a controlled base/input-core factor \(W_I\). Here \(\operatorname{cost}_{\mathrm{full},i}(Y)\) must count every new component interior and every genuine coordinate footprint in the output carrier. Removing those terms from (HR18.33) changes the norm.

The source estimate (1.68) bounds the relative tree through exterior cubes. The eligibility upper bound yields only a comparison with a running component-size constant; for example the elementary count gives

\[
 |Y|_M+\mathsf t_M(Y)
 \le C(1+R)^4\{1+d_{k,Z}(Y)\}.
 \tag{HR18.34}
\]

An included component is adjacent to an exterior cube, there are at most a dimension-only multiple of the number of exterior cubes such components, and each has at most \(C R^4\) cubes. A spanning tree of the connected union has at most its number of cubes minus one edges. This proves the displayed comparison, without asserting that it is sharp.

Using this comparison to sum (HR18.33) gives a series with terms bounded by

\[
 C(1+R)^4\alpha_k
 \exp\left\{
  -\bigl[\kappa_a-\log A_4-C\kappa(1+R)^4\bigr]n
       +C\kappa(1+R)^4\right\}.
 \tag{HR18.35}
\]

The bracket is not positive uniformly as \(R\to\infty\). Choosing a larger but fixed \(M\) or a larger but fixed source rate does not fix this running loss. Even improving the elementary comparison using a fixed-width collar leaves a growing volume-to-boundary ratio for four-dimensional boxes. A separate factor \(e^{-cR}\) in \(\alpha_k\) cannot compensate an exponential full-volume cost per arbitrarily many component attachments. This is a failure of this **available majorant**, not a lower bound on the actual Yang–Mills activities.

The primary source displays the missing payment explicitly. On LFR II p.389, before (1.95), a factor

\[
 e^{2\kappa(100R_k)^4}
 \tag{HR18.36}
\]

is paid, in that particular expansion, by the unnormalized suppression factors for the **newly summed small components \(X_j\)**: the product over their indices \(h\) in (1.93) is combined with the first product in (1.92), using the bound (1.89). It is not a statement that every retained \(Y_i\) has the same suppressed mass. In the normalized alternative on p.391 the \(Y_i\) domains are fixed; the corresponding first sums and first suppression product are absent, and the source explicitly explains why its unmarked convergence does not require decay for those fixed domains.

Thus a small-component factor, when available in the unnormalized full law, is potentially useful to a full-law marked-history estimate. Once that component is normalized as in (HR18.2), its mass has canceled. For the fixed \(Y_i\) alternative there is also no newly supplied full-interior payment in the normalized expansion. The relatively weighted scalar theorem CR.20–CR.21 deliberately treats such a component as an incidence atom and does not prove (HR18.33).

An explicit operation cost growing like \(e^{C R_k^4}\) can be recorded for a bounded one-component core. It does not provide the uniform strong estimate (HL.42), and does not by itself pay the cost of arbitrarily many external component footprints. A valid full-law reserve for those costs belongs to the H-02/H-04 analysis unless a stronger internal marked locality theorem is proved first.

### 6. Why control of the nonsmall base is a separate mathematical input

The preceding obstruction is not merely an unfortunate bound for the cross action. The \(n=0\) terms in (HR18.11) already contain the normalized self-component law. The following finite probability example isolates the logical role of its external locality.

Let \(b_1,\ldots,b_N\) be retained signs at distinct sites in one component, and let an old sign \(\sigma\) be stored at an insertion anchor. Fix \(a>0\), and define the positive component measure

\[
 \nu_b(\sigma)
 =\frac{e^{a\sigma\prod_{j=1}^N b_j}}{2\cosh a},
 \qquad \sigma\in\{-1,1\}.
 \tag{HR18.37}
\]

Its total mass is one, its cross interaction is zero, and it is independent of any additional current/native variable. Its scalar current Hessian and all scalar native responses are zero. For the bounded local input \(F=\sigma\), however,

\[
 Q_bF=\tanh(a)\prod_{j=1}^N b_j.
 \tag{HR18.38}
\]

Any exact carrier representation of (HR18.38) in which an activity on a proper subset of the \(b_j\) is independent of an omitted \(b_j\) must include activities whose carrier contains all \(N\) sites. Apply the Walsh coefficient

\[
 \mathcal W(f)=2^{-N}\sum_{b\in\{-1,1\}^N}
                  f(b)\prod_{j=1}^N b_j.
 \tag{HR18.39}
\]

It annihilates every activity missing one site, and \(|\mathcal W(f)|\le\|f\|_\infty\). Thus the sum of the supremum norms of the full-footprint activities is at least \(\tanh(a)\). Their weighted supremum carrier sum is at least

\[
 e^{\kappa N}\tanh(a).
 \tag{HR18.40}
\]

With the M-03 constant-regulator convention \(\widehat R=2\), this gives the same lower bound up to the fixed factor \(1/2\) for the pointwise value part of that norm. The input norm can be bounded independently of \(N\): its only active coordinate is the local sign \(\sigma\), its value and discrete-difference envelopes are bounded, and its regulator can be constant. The example therefore excludes a uniform strong-norm contraction deduced solely from positivity, normalized scalar control, an admitted irrelevant analytic chart and small cross interactions.

This example is **not a Yang–Mills model**, does not claim that the actual source component has a parity interaction, and does not disprove the intended H-03 theorem. It shows why a marked locality/conditional-regulator argument for the actual nonsmall component cannot be replaced by a scalar boundary estimate.

### 7. What remains to apply the result in the physical M-03 framework

The exact decorated transport rule remains

\[
 \delta_\tau(QA)
 =Q_{\tau x}(B_\tau+J_\tau)
       +\frac{Q_{\tau x}-Q_x}{t}(A)
 \tag{HR18.41}
\]

for a continuous step \(t\ne0\), with denominator one for a discrete change. It keeps the direct record, previous current and new normalized-kernel current separate. The analytic \(z\)-derivative in Theorem HR18.2 estimates the newly generated current only for the admitted fixed-support native variation with the input frozen.

Four actual transfer questions are still unresolved by the sources and arguments in this note.

1. **The preintegration marked map.** The completed scalar C-05 representation is an exact marginalization. Its scalar gauge extension fixes surviving raw slots. For an arbitrary incoming mark, one still needs a common preintegration chart, or an exact marked coordinate/gauge transformation, for every old variable which the mark uses. The map must stay in LFR II's admitted domain uniformly over its old histories and must keep the direct pullback and its full chain rule. Scalar equality after integration does not identify the marked complex integrand.

2. **Raw retained directions and interfaces.** Current/native deformations which keep raw retained slots and the outer geometry fixed do not cover every M-03 elementary direction. A retained raw field can change the nonsmall self law and its real reference. A hard selector or a geometry change may change support. The signed measure in (HR18.41), including its normalizer, then replaces a formal analytic score. An improved off-support extension can remove artificial jumps only if it agrees on the entire physical support and has a proved margin. It cannot remove a genuine on-support jump without a corresponding boundary-current estimate.

3. **The pointwise regulator.** Theorem HR18.2 controls the averaged part of the norm. It does not establish an estimate of the form
   \[
   Q_x\bigl(\widehat R_{h,X}^{\,m}\circ\chi\bigr)
      \le C^{m+1}(m!)^r\widehat R_{h,Y}(x)^m,
   \tag{HR18.42}
   \]
 including the actual scale factor, chart path lengths and output footprint. The old self action can contain many old coordinates. Full-law \(L^p\) contraction gives no uniform pointwise conditional inequality such as (HR18.42).

4. **The complete physical carrier transfer and payment.** For the repeatedly normalized representation chosen in C-05, first identify the actual preintegration marked carrier family with its surviving older tags and prove the corresponding weighted cross sum; the original fixed-geometry count (HR18.27) is not a substitute for that check. Then the relative sum has to be upgraded using accurate physical dependency footprints or paid by a rigorously proved full-law marked reserve. The strong carrier series (HR18.33) and the base factor \(W_I\) must be bounded. The source's unnormalized mass cannot be used after it has canceled in the conditional law.

The current-scale incoming budget is a hypothesis of an operator estimate such as H-03. Proving that budget at all earlier scales remains M-07 and the matching/renormalization estimates. This note neither assumes that full induction has already closed nor relabels a bare cutoff budget as a current-scale one.

### 8. Sector hypotheses and consequences

| Required item | Result in this note |
|---|---|
| Exact old posterior and all normalizers | Kept in (HR18.1)–(HR18.7). |
| Nonsmall self action and old histories | Kept in the positive base; \(n=0\) cumulants are not dropped. |
| Every higher incoming source vertex | Included through all partitions in (HR18.11). |
| Exact thin carrier representation | Proved in (HR18.10)–(HR18.15); no full-radius ball enlargement. |
| Absolute convergence and fixed source factorial growth | Proved by (HR18.22)–(HR18.25), with convergence radius in the cross-action parameter strictly greater than one. |
| Actual source-native relative carrier sum | Proved in Corollary HR18.3 for the specified primary fixed component operation and its literal carrier family, with all its internal histories retained. |
| Repeatedly normalized older-tag geometry | The algebraic theorem applies if its own actual preintegration weighted sum is supplied; no automatic application of the original HL.G3 count is made. |
| Native kernel derivative and finite-difference records | Proved with their explicit Cauchy-radius cost; input differences remain separate. |
| Actual preintegration physical marked pullback | Still open. |
| Raw retained/support-changing currents | Still open. |
| Pointwise regulator and full-volume weighted norm | Still open; their exact inequalities are displayed. |

This annex supplies an additional actual source-level posterior theorem and a precise stronger application test. It does not change any catalogue statement, application criterion or dependency.

### Primary sources and local proof dependencies

- T. Balaban, *Large Field Renormalization. I. The Basic Step of the R Operation*, CMP **122** (1989), 175–202: eligible components, p.177; exact replacement, (1.100)–(1.102), p.201.
- T. Balaban, *Large Field Renormalization. II. Localization, Exponentiation, and Bounds for the R Operation*, CMP **122** (1989), 355–392: (1.67)–(1.69), pp.376–377; (1.71)–(1.75), pp.378–380; the component-volume payment on p.389; (1.103)–(1.104), pp.391–392.
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. I*, CMP **109** (1987), 249–301: p.257 defines the finite connected \(M\)-cube carriers and their tree size. DOI <https://doi.org/10.1007/BF01215223>.
- Annex AG: exact posterior HL.1, source domains HL.6–HL.7, eligible geometry HL.8–HL.9. These scopes are retained.
- Annex AK: the moment-only fixed-chart reset theorem HP.1–HP.3, and the earlier radial-ball summation warning.
- Annex AU: CR.15, actual completed-carrier coefficient extraction; CR.20–CR.21, the deliberately relative scalar cluster norm.
- Annex AW gives the conditional scalar boundary estimate. The marked numerator requires separate control.
- Annex Y: the unchanged strong norm M.11–M.12 and exact decorated conditional transport M.28–M.42.

The finite probability and combinatorial arguments in Sections 2–3 and 6 are proved in this note. The relative-geometry sum in Section 4 is proved from the explicitly identified primary-source geometry and cross-action bounds; it is not an imported marked Yang–Mills theorem.
