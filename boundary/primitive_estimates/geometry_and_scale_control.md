# C-05: a geometric argument after completed-component integration

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

**Status:** proved abstract repair lemmas; the remaining actual-model matching is explicit. The all-history C-05 application is conditional.  
**Scope:** the repeated-component, birth-age, root-multiplicity, and physical-distance bounds in the component contraction.

## 1. Main conclusion

**Metric clarification found during the source analysis:** LFR II (1.67) charges the full length of a connected tree contained in the carrier, while requiring that tree to visit only the cubes outside the designated region. It is not the quotient metric that makes traversal inside that region free. The disappearance of a requirement to fill its interior does not make connections through it costless. The quotient-metric lemmas below are consequently an alternative for a genuinely weaker norm, not an identification of (1.67). The separate post-second-exponentiation notation on a possibly disconnected exterior set needs an explicit convention before either interpretation is imported.

The original birth of a scalar summand need not be the right induction label after a completed component is integrated and its boundary terms are resummed. A proof can instead use the complete scalar activity at its latest rebasing scale. This avoids requiring a separate estimate for every arbitrary old decomposition. It does **not** avoid the cost of physical travel through a component whose interior tree penalty has been removed.

There is a concrete mathematical replacement for that cost. If the maximal free components have uniformly bounded diameter in current units and are separated relative to their diameters, exponential decay in the metric that allows free motion inside components implies a uniform, physically weighted Hessian row estimate. The diameter produces an explicit factor

\[
(1+D)^4e^{\chi D}.
\tag{G1}
\]

A proved collar prefactor of size \(P(g^{-1},R)e^{-cR}\), with \(D=O(R)\), can pay this factor. Thus a separate exponential estimate in the original age \(k-b\) is not logically necessary for a current Hessian theorem.

The source check identifies a plausible current-size input: domains actually used in the completed-component operation are eligible at the operation's scale. What has not been established is the relative separation of all maximal components after arbitrary earlier completions and rebases, together with the required decay of the **complete current score**. Eligibility at one operation does not by itself prove those two statements.

## 2. Source anchors and their precise use

The following source facts are taken from the original papers. This note does not reproduce every printed superscript or formula.

**CMP119:** the boundary action is a sum of scale-labelled localized terms. Printed p.262 permits a weaker alternative norm after resumming terms meeting components of the large-field region, and states that the construction can proceed with that alternative assumption. The resulting carrier either contains such a component or avoids it. [B88]

**LFR II:** the three successive determining-set changes are (1.61), (1.62), and (1.63). Their added localization components contain a prescribed component and meet the preceding coincidence-domain boundary. Printed p.376 assigns a special distance factor only to the first nonempty localization and sums birth indices before (1.68). Pages 379–380 bound the complex variation of the full component operation, including inherited self-terms. Pages 384–387 control eligibility after coarsening; p.387 identifies the domain in (1.71) as the zero-waiting-time case. Pages 391–392 use a weaker second exponentiation and leave multipliers depending on retained fields. [B89-II]

These facts identify possible ingredients; none is stated here as the sought original-birth Hessian theorem.

### 2.0 A connected relative tree already pays exterior endpoint separation

The basic definition in CMP109, printed p.257, takes the full length of a connected tree that visits the carrier's cubes. LFR II (1.67) restricts which cubes must be visited, but still charges the whole tree. [B87; B89-II]

Let \(Y\) be a carrier and let \(E\) be its prescribed collection of exterior cubes of side \(M\) in current units. Define

\[
\mathfrak d(Y;E)=M^{-1}\inf\{|T|:T\subset Y\text{ is a connected tree meeting every cube of }E\}.
\]

Here \(|T|\) is its entire ambient length, including portions inside the omitted region. If \(x,y\) belong to cubes of \(E\), then

\[
\rho(x,y)\le M\mathfrak d(Y;E)+2c_dM,
\tag{G0}
\]

where \(c_dM\) bounds an individual cube diameter in the chosen ambient metric.

**Proof.** Pick a nearly minimizing tree and points where it meets the two cubes. Each endpoint is at most \(c_dM\) from its tree point. The path connecting the two tree points is a part of the connected tree and has length at most \(|T|\). Apply the triangle inequality and take the infimum.

It follows that \(e^{-\kappa\mathfrak d}\) pays an exterior endpoint weight \(e^{\chi\rho(x,y)}\) with unspent tree decay whenever \(\chi M<\kappa\). No hole-diameter estimate is needed for this implication. A Hessian application must still prove that its marked endpoints belong to the prescribed exterior cubes and that this same connected-tree norm survives the operation in question. An old anchor inside the omitted region is not covered by (G0).

For the second exponentiation the text changes the size expression to one on \(X'\setminus\bigcup_iY_i\), which can be disconnected. The original CMP109 definition concerns connected localization domains. It does not, by itself, define this later expression. A sum of the sizes of the exterior connected components, a full tree spanning all exterior components, and a quotient metric are different objects. The available text does not justify conflating them. The first of these would lose intercomponent connections; the second would retain them. The precise source convention or a direct examination of the cluster proof is required for the final application.

### 2.1 The map cases that must be matched

The following table is an analysis index, not a new transcription of the source formulas.

| Source operation | New determining set | What must be tracked in a grade proof |
| --- | --- | --- |
| (1.61) | \(B'_k(Y_1)\) | Old support \(X\), components already absorbed into \(Y_1\), and the actual metric of the first changed background |
| (1.62) | \(B_1(Y_2)\) | The gauge/background response of this determining-set change, including whether the old anchor is still an independent slot |
| (1.63)–(1.64) | \(B_k(Y_3)\) | The final background response, with no replacement of its particular distance by an unproved age count |
| Second exponentiation | Normalized operations on completed components | Which interiors now carry no tree penalty, and which scalar terms have been resummed into the new boundary activity |

Every inherited record falls into one of two logical classes: its old anchor remains represented in the metric that receives the distance factor, or it has been absorbed into a resummed component. In the second case one must either preserve an additional graded record with a proved cost, or rebase and estimate the full resummed scalar. Relabelling alone does not prove smallness.

### 2.2 What rebasing and multiplier absorption actually establish

There are three distinct operations that should not be compressed into a claim that all old births disappear.

1. **Reconstruction of old action terms:** the source reconstructs the older effective-action terms with the new determining background. Their original scale labels can remain. Only the new correction activities are resummed and assigned to the current step.
2. **Absorption into a component reference operation:** a scalar factor depending only on variables integrated inside a component can be included in its positive reference kernel. In the source's complete native extension of the component operation, the stated parameter dependence is through the quadratic form and the resummed component self-action. This is a genuine source input about that extension, including inherited terms; it is stronger than merely knowing that an unmarked mass is positive.
3. **Extraction of the final multiplier:** after normalized integration, the component mass remains a function of raw retained fields. Its derivative is zero on a slice that actually fixes those raw fields. If a later operation integrates those fields, the multiplier belongs to that later positive reference kernel; it has not vanished from the measure.

The elementary absorption identity is

\[
\int f(y)\tau(y)\,\mu(dy)
=\mu(\tau)\int f(y)\,\mu_\tau(dy),
\qquad
\mu_\tau(dy)=\frac{\tau(y)}{\mu(\tau)}\mu(dy),
\]

for \(\tau\ge0\), \(0<\mu(\tau)<\infty\). If \(\tau\) and the integration support are independent of the current parameter, no current score is created by this change of reference measure. An arbitrarily large internal self-action can thus be harmless as a reference weight. An interaction coupling variables of different components is not such a self-factor and must remain in the interaction estimate.

A valid induction using this identity must prove an all-or-nothing support rule: every old multiplier is either outside the current integrated variables and fixed, or wholly assigned to the reference kernel of a current component. The source's component-factorized operation supports this rule at the operation it describes. A proof for the independently chosen C-05 current coordinates must additionally track the raw-field pullback and the actual variable partition. No absent C-04 or CR.22 hypothesis is assumed here.

Even if all self-multipliers have been absorbed, previous **cross-component boundary activities** may retain older localization holes. The self-factor identity does not show that these activities have the metric of only the newly completed components. That remaining carrier statement is exactly where a present-scale rebasing proof must be made explicit.

### 2.3 Bounded completion size and small attachments alone do not preserve the output tree norm

The metric clarification does not make a strong post-integration spanning-tree estimate automatic. The following example distinguishes the input carriers from the new connected output carrier.

Fix \(r>1\), let \(g\downarrow0\), and set

\[
\ell_g=\log g^{-2},\qquad D_g=\lceil\ell_g^r\rceil.
\]

Take a rectangular lattice component \(H_g\) whose diameter is comparable to \(D_g\), and single exterior cubes \(Q_x,Q_y\) touching opposite sides. Put
\(X_x=H_g\cup Q_x\) and \(X_y=H_g\cup Q_y\). Each input carrier contains the whole component and only its own exterior cube.

Let the internal component variable be a fair spin \(\sigma\in\{-1,1\}\). The normalized integration operator \(\Pi\) has norm one, is positive, and is independent of the external parameters. On \(|z_x|,|z_y|<1\), take

\[
V_x=g z_x\sigma,\qquad V_y=g z_y\sigma.
\]

Each interaction has sup norm at most \(g\). Its individual relative connected tree need visit only \(Q_x\), or only \(Q_y\). That cost is bounded independently of \(D_g\), and can be zero under the convention permitting a one-point tree. If a particular convention gives a fixed cost \(c_0\), multiplying each interaction by the fixed factor \(e^{-\kappa c_0}\) gives the same example with the corresponding exponential input bound.

The reduced scalar is

\[
Z(z)=\Pi e^{V_x+V_y}
=\cosh(g(z_x+z_y)),\qquad
F(z)=\log Z(z).
\]

For small \(g\), this logarithm is holomorphic on the entire stated unit polydisc; no zero or branch issue is involved. At zero,

\[
\partial_x\partial_yF(0)=g^2.
\]

Since \(\rho(x,y)\ge c_DD_g\) for a fixed \(c_D>0\), every fixed \(\chi>0\) gives

\[
e^{\chi\rho(x,y)}|\partial_x\partial_yF(0)|
\ge\exp(\chi c_DD_g-\ell_g)\longrightarrow\infty.
\]

There is no contradiction with (G0). The **output** carrier containing both exterior cubes requires a connected tree of length comparable to \(D_g\). Neither input activity had that carrier. Normalized integration generated the connection between the two initially separate exterior attachments through the shared internal spin. Thus eligible-scale diameter, small individual amplitudes, a small unweighted component-incidence norm, and a normalized kernel bound do not **alone** preserve the stronger output physical-tree norm.

This is not an admitted Wilson-history counterexample. In particular, its current parameters are attached at the component boundary. An actual active-field collar of width comparable to \(R_k\), with decaying current-to-component maps, can make these attachments exponentially smaller and pay the output diameter as in (K23b) of [the normalized-kernel and block-oscillation analysis](block_oscillation_alternative.md). Those additional conditions are precisely what the example does not assume. A theorem supplying an input amplitude already of order \(e^{-cR_k}\), rather than merely \(g\), would likewise evade this obstruction.

## 3. The exact bookkeeping lemma for lost grades

This elementary statement makes the missing assignment precise.

Let a path be composed of paid segments and free jumps inside contracted components. Associate an integer grade \(\nu(v)\) to each represented endpoint. Suppose that a paid segment \(e=(v,w)\) has nonnegative cost \(c(e)\) satisfying

\[
|\nu(v)-\nu(w)|\le a^{-1}c(e),\qquad a>0.
\tag{G2}
\]

For a free component \(H\), let

\[
\omega(H)=\sup_{v\in H}\nu(v)-\inf_{v\in H}\nu(v).
\]

### Proposition G1. Grade ledger under contraction

For a path from a represented grade \(b\) to grade \(k\),

\[
|k-b|\le a^{-1}\sum_{e\text{ paid}}c(e)
 +\sum_{H\text{ traversed}}\omega(H),
\tag{G3}
\]

where a component is counted once for each free jump through it.

**Proof.** Telescope the grade differences along the path and use the triangle inequality. Apply (G2) on each paid segment and the definition of \(\omega(H)\) on each free jump. No spatial or probabilistic assumption is needed.

If every free component is grade-constant, a bound by paid costs survives passage to the quotient. If a component joins grades separated by \(k-b\), the entire age can occur in its free-jump term. A geometric path crossing many grades is therefore insufficient: the proof needs control of the second term of (G3) or another estimate that makes it unnecessary.

This proposition applies separately to all three determining-set changes in Section 2.1. To use it in the actual expansion one must identify the represented grades and verify (G2) for the **actual** inherited-tree and first-distance weights. A current-volume factor is not assigned a grade cost unless that inequality is proved for it.

Rebasing a consumed component replaces the old label by its current induction label. That can remove the need for (G3) as a birth estimate, but it changes the object to be bounded: the complete new activity, with its full current derivatives, must obey a stable norm.

## 4. Physical distance can be recovered from a free-component metric

Work in a metric space \((V,\rho)\). In applications, \(V\) is the current lattice, or a finite torus with its periodic graph metric in current units. Let \(\mathcal H\) be a finite family of pairwise disjoint nonempty components. Put

\[
D_H=\operatorname{diam}_\rho H,
\qquad D=\sup_{H\in\mathcal H}D_H.
\]

The **paid distance** \(q(x,y)\) is the infimum of the lengths of paths from \(x\) to \(y\) when motion outside components is charged its ambient metric length and motion between two points of the same component is free. Equivalently, it is the quotient path pseudometric obtained by identifying each \(H\) to a point.

This definition is used for the lemmas only. An actual weakened carrier cost must be shown to dominate the needed paid path before these lemmas apply; it is not silently identified with a source metric.

Assume relative separation:

\[
\operatorname{dist}_\rho(H,H')
\ge \eta\max(D_H,D_{H'}),
\qquad H\ne H',\qquad \eta>0.
\tag{G4}
\]

### Theorem G2. Distance restoration with a diameter toll

Under (G4),

\[
\rho(x,y)\le A q(x,y)+D,
\qquad A=1+\eta^{-1},
\tag{G5}
\]

for arbitrary endpoints \(x,y\).

**Proof.** Take a path whose paid length is within \(\varepsilon\) of \(q(x,y)\). Any segment between two visits to the same component can be removed and replaced by a free jump. Thus it suffices to consider a path visiting distinct components \(H_1,\ldots,H_m\).

Let \(a_0\) be the exterior length from \(x\) to \(H_1\), let \(a_i\) be the exterior length between \(H_i\) and \(H_{i+1}\), and let \(a_m\) be the final exterior length. Each internal gap satisfies

\[
a_i\ge\eta D_{H_i},\qquad 1\le i<m.
\]

Consequently,

\[
\sum_{i=1}^mD_{H_i}
\le\eta^{-1}\sum_{i=1}^{m-1}a_i+D
\le\eta^{-1}\sum_{i=0}^ma_i+D.
\]

Restoring ambient travel through each component costs at most its diameter. The ambient triangle inequality therefore gives

\[
\rho(x,y)\le\sum_{i=0}^ma_i+\sum_{i=1}^mD_{H_i}
\le A\sum_{i=0}^ma_i+D.
\]

Let \(\varepsilon\downarrow0\). A path visiting no component satisfies the stronger inequality \(\rho(x,y)\le q(x,y)\). This proves (G5).

### Corollary G3. No diameter toll for roots outside proportional collars

If \(x,y\) additionally satisfy

\[
\operatorname{dist}_\rho(x,H)\ge\eta D_H,
\qquad
\operatorname{dist}_\rho(y,H)\ge\eta D_H
\quad\text{for all }H,
\tag{G6}
\]

then

\[
\rho(x,y)\le A q(x,y).
\tag{G7}
\]

**Proof.** In the preceding path, both exterior gaps adjacent to a visited component are at least \(\eta D_H\), including the two endpoint gaps. Hence

\[
\sum_{i=1}^mD_{H_i}
\le\frac1{2\eta}\left(a_0+2\sum_{i=1}^{m-1}a_i+a_m\right)
\le\eta^{-1}\sum_{i=0}^ma_i.
\]

Use the same ambient triangle inequality.

The pairwise separation in (G4) is substantive. Disjointness by itself does not imply it. Nor does a diameter bound for each individual newly eligible component prove it for the maximal components retained from different earlier scales.

## 5. A weighted row theorem with the correct physical measure of a hole

Assume the current lattice or torus has uniform polynomial ball growth

\[
|\{y:\rho(x,y)\le r\}|\le C_d(1+r)^d,
\qquad r\ge0.
\tag{G8}
\]

The standard unit lattice and its periodic finite quotients satisfy this with a uniform constant. The relevant case is \(d=4\).

Let \(K=(K_{xy})\) be a matrix of operators between fixed-dimensional current blocks, and suppose

\[
\|K_{xy}\|\le\varepsilon e^{-\kappa q(x,y)},
\qquad \kappa>0.
\tag{G9}
\]

### Theorem G4. Uniform physical weighted row

Under (G4), (G8), and (G9), for \(0\le\chi<\kappa/A\),

\[
\sup_x\sum_y e^{\chi\rho(x,y)}\|K_{xy}\|
\le C(d,C_d,A,\kappa-\chi A)\,
\varepsilon(1+D)^d e^{\chi D}.
\tag{G10}
\]

**Proof.** Set \(s=\kappa-\chi A>0\). Theorem G2 gives

\[
e^{\chi\rho(x,y)}e^{-\kappa q(x,y)}
\le e^{\chi D}e^{-s q(x,y)}.
\]

If \(q(x,y)<n+1\), then \(\rho(x,y)<A(n+1)+D\). By (G8),

\[
\begin{aligned}
\sum_y e^{-s q(x,y)}
&\le C_d\sum_{n=0}^\infty e^{-sn}
       (1+D+A(n+1))^d\\
&\le C_d(1+D)^d\sum_{n=0}^\infty e^{-sn}(1+A(n+1))^d.
\end{aligned}
\]

The last series converges independently of the volume, cutoff, and number of components. This proves (G10).

Using the crude lower bound \(q\ge(\rho-D)/A\) inside a direct ambient sum would instead produce an unnecessarily large factor \(e^{\kappa D/A}\). The ball-counting argument above pays only the physical weight \(e^{\chi D}\), which matters in a smallness estimate.

### Corollary G5. A collar prefactor pays the diameter

Suppose uniformly in the actual history,

\[
D\le c_D R,
\qquad
\varepsilon\le P(g^{-1},R)e^{-cR},
\tag{G11}
\]

where \(P\) is a fixed polynomial with nonnegative coefficients, \(c>0\), and \(A\le A_0\). Choose fixed

\[
0<\chi<\min\{\kappa/A_0,c/c_D\}
\tag{G12}
\]

(omitting the second restriction if \(c_D=0\)). Then the weighted row is bounded by a fixed polynomial times

\[
e^{-(c-\chi c_D)R}.
\tag{G13}
\]

In particular it tends to zero if \(R\) grows faster than \(\log g^{-1}\), with all constants uniform. For example, \(R\asymp(\log g^{-2})^r\), \(r>1\), suffices.

This corollary closes a **numerical** and geometric part of the repair. It does not establish (G9) or (G11) for the complete current Hessian of the Wilson construction. A merely polynomially small prefactor, without the necessary paid distance or collar reserve, need not suffice.

## 6. A scalar holomorphic norm can avoid artificial root multiplicity

One can sometimes bound an entire Hessian row without applying a separate Cauchy estimate at every endpoint and multiplying by the carrier volume.

### Proposition G6. Dimension-independent Cauchy row estimate

Let \(F\) be holomorphic on a finite-dimensional complex polydisc

\[
\{z:|z_j|<r\text{ for every }j\},
\]

and suppose \(|F(z)|\le M\). For a fixed root \(i\),

\[
\sum_j|\partial_i\partial_jF(0)|\le\frac{4M}{r^2}.
\tag{G14}
\]

The same conclusion holds with \(M\) replaced by a bound on the root oscillation
\(F(z)-F(z\text{ with }z_i=0)\).

**Proof.** Choose complex phases \(v_j\), \(|v_j|\le1\), so that

\[
\sum_jv_j\partial_i\partial_jF(0)
=\sum_j|\partial_i\partial_jF(0)|.
\]

The function \(G(t,s)=F(te_i+sv)\) is holomorphic and bounded by \(M\) on \(|t|,|s|<r/2\). Cauchy's estimate gives

\[
|\partial_t\partial_sG(0,0)|\le4M/r^2.
\]

The derivative on the left is the aligned sum. For the root oscillation, its mixed derivatives with first index \(i\) agree with those of \(F\).

For blocks of fixed coordinate dimension, applying this argument to coordinate rows and summing a fixed number of components changes only a dimension-dependent constant. At a nonzero real point the same assertion uses an available polydisc around that point.

If a carrier has physical diameter at most \(D_X\), this gives the weighted row estimate \(4Me^{\chi D_X}/r^2\) for its Hessian. It does not remove that diameter factor. A global scalar bound extensive in the volume is also not a root-local bound. The induction still needs a summable collection of scalar root oscillations or another genuinely local scalar norm.

This observation is useful for a resummed route: counting every fine root separately may be unnecessary **after** an appropriate complete scalar bound has been proved on a common polydisc. It is not a justification for inserting that bound when only an unmarked partition-function estimate is available.

## 7. An alternative physical-measure and asymptotic-freedom summation

There is a second way an original-birth argument can avoid the factor \(L^{4(k-b)}\). It must use a measure factor already present in the actual expression.

### Proposition G7. Physical measure cancels grid refinement in a local kernel sum

For \(0<h\le H\), \(c>0\), and \(y\in\mathbb R^d\),

\[
H^{-d}\sum_{x\in h\mathbb Z^d}h^d
 e^{-c|x-y|/H}\le C(d,c),
\tag{G15}
\]

uniformly in \(h,H,y\).

**Proof.** Tile \(\mathbb R^d\) by cubes of side \(h\) centered at the lattice sites. For \(u\) in the cube centered at \(x\),

\[
|x-y|\ge|u-y|-\sqrt d\,h/2.
\]

Hence the summand times \(h^d\) is at most

\[
e^{c\sqrt d/2}\int_{Q_x}e^{-c|u-y|/H}\,du.
\]

Sum the cubes and change variables \(v=(u-y)/H\). The remaining integral is finite and independent of the scales.

If the actual normalized current expression contains \(h_b^d/H^d\) with each birth root, (G15) pays their spatial refinement. It must not be inserted by dimensional expectation. In particular, a dimension-four normalization of one class of irrelevant terms does not prove that every inherited boundary term carries this measure.

### Proposition G8. Summing superlogarithmic birth prefactors under an AF drift

Let \(t_b>0\) and suppose, for \(b\le k\),

\[
t_b\ge t_k+c_*(k-b),\qquad c_*>0.
\tag{G16}
\]

Fix \(a>0\), \(r>1\), and nonnegative \(s,q\), and define, for sufficiently large \(t\),

\[
f(t)=t^s(1+\log t)^q e^{-a(\log t)^r}.
\]

Then

\[
\sum_{b\le k}f(t_b)
\le f(t_k)+c_*^{-1}\int_{t_k}^{\infty}f(u)\,du
\longrightarrow0
\quad(t_k\to\infty),
\tag{G17}
\]

once \(t_k\) is beyond the point where \(f\) is decreasing.

**Proof.** Logarithmic differentiation shows eventual monotonicity:

\[
\frac{t f'(t)}{f(t)}
=s+\frac{q}{1+\log t}-ar(\log t)^{r-1}<0
\]

for sufficiently large \(t\). Use (G16) and the integral comparison for a decreasing function. With \(v=\log u\), the integral tail becomes

\[
\int_{\log t_k}^{\infty}(1+v)^q
 e^{(s+1)v-av^r}\,dv.
\]

It is finite and tends to zero because \(r>1\). This proves (G17).

The proposed application is \(t_b=g_b^{-2}\). The actual verified trajectory must establish the uniform drift (G16) in the chosen normalization. If the physical root measure and such a drift both hold, a separate exponential age factor is unnecessary. Neither premise is derived by this proposition.

## 8. What remains to connect these repairs to the actual C-05 sector

The two repair strategies require different, explicit inputs.

### 8.0 Mixed births reduce to a one-step component rule

The following conditional geometry theorem shows that no separate combinatorial loss in the number of past completions is necessary if the correct whole-component rule holds.

### Proposition G9. Relative separation survives laminar rebasing

Let \(h_j>0\) be physical lattice scales, let \(R_j>0\), and put \(S_j=h_jR_j\). Suppose

\[
S_i\le C_s S_j\quad(i\le j),\qquad C_s\ge1.
\tag{G18}
\]

At stage \(j\), assume there is a family \(\mathcal P_j\) of pairwise disjoint candidate components such that:

- distinct members have ambient distance at least \(sS_j\), with \(s>0\);
- every surviving completed hole from an earlier stage is wholly contained in a single member of \(\mathcal P_j\);
- a newly completed hole is a whole member \(P\in\mathcal P_j\), has diameter at most \(C_DS_j\), and replaces every earlier completed hole contained in \(P\).

Then at any current stage \(k\) the surviving maximal completed holes satisfy

\[
\operatorname{dist}(H,H')
\ge\frac{s}{C_DC_s}\max(\operatorname{diam}H,\operatorname{diam}H'),
\tag{G19}
\]

and have diameters at most \(C_DC_sR_k\) in current units \(h_k\).

**Proof.** Consider two surviving holes and let \(j\) be the later of their birth stages. If they were born simultaneously, they are distinct members of \(\mathcal P_j\). If one was older, it was contained in some member of \(\mathcal P_j\). That member cannot be the new hole: otherwise the older hole would have been consumed and would not survive. In either case their distance is at least \(sS_j\).

The younger diameter is at most \(C_DS_j\). If the older birth was \(i\le j\), its diameter is at most \(C_DS_i\le C_DC_sS_j\). This proves (G19). Finally every surviving hole was born at some \(i\le k\), so its diameter is at most \(C_DC_sS_k\); divide by \(h_k\).

The proposition isolates the exact geometric checks. No claim is made that an arbitrary decomposition into lattice components satisfies the positive separation premise. Components touching at corners, for example, may have zero ambient separation; a buffer or a suitable merging convention must be accounted for. Nor is whole-component containment supplied merely by naming a new carrier “maximal.” These rules must be identified in the actual geometric construction.

If the source's current operation exposes only newly completed components, the same-stage part of this proof is enough. If older completed holes remain in its carrier norm, all three premises above provide a sufficient invariant. This distinction is preferable to assuming either that all historical holes remain forever or that they have all disappeared.

### Corollary G10. The physical scale comparison follows from an upper AF drift

Fix \(L>1\), \(r>0\), and \(C\ge0\). Suppose the inverse squared couplings \(t_i=g_i^{-2}\) obey

\[
e\le t_i\le t_j+C(j-i)\quad(i\le j),
\qquad h_i/h_j=L^{i-j}.
\tag{G20}
\]

Let \(R_i\) be the least nonnegative integral power of \(L\) not smaller than \((\log t_i)^r\). Then (G18) holds with the finite constant

\[
C_s=L\sup_{n\in\mathbb N_0}
L^{-n}\left(1+\frac Ce n\right)^r.
\tag{G21}
\]

**Proof.** The rounding rule gives
\((\log t_i)^r\le R_i<L(\log t_i)^r\), with the weak upper inequality sufficient if a threshold is attained. Put \(n=j-i\). Since \(t_j\ge e\),

\[
\begin{aligned}
\log t_i
&\le\log(t_j+Cn)\\
&=\log t_j+\log(1+Cn/t_j)\\
&\le\log t_j+Cn/e.
\end{aligned}
\]

Also \(\log t_j\ge1\), so

\[
\frac{S_i}{S_j}
=L^{-n}\frac{R_i}{R_j}
\le L L^{-n}\left(\frac{\log t_i}{\log t_j}\right)^r
\le L L^{-n}\left(1+\frac Ce n\right)^r.
\]

The supremum in (G21) is finite because exponential decay in \(n\) dominates its fixed polynomial growth. This proves the claim.

This removes the physical-size comparison as an independent geometric premise once the appropriately normalized upper coupling drift has been proved. It does not establish that drift for the intended Wilson trajectory. The exact N2-F input and the coupling dictionary must still be checked; no absent trajectory theorem is imported here.

### Strategy A: rebase and use the complete scalar/current response

1. Identify the maximal components that are free in the **final** scalar carrier norm after all relevant previous completions. Record their last completion scales and remove consumed subcomponents from the active family.
2. Prove relative separation (G4), or a different pathwise bound sufficient for (G5), in the actual current physical metric. One-step size/eligibility alone is insufficient.
3. Prove a uniform bound on the current diameters. A component whose old fine diameter was large can be small in current units; the scale change and coupling dependence must be included explicitly.
4. Prove the complete-current derivative estimate (G9) with a collar reserve (G11), or a scalar root-oscillation norm from which it follows. This includes all inherited scalar terms and responses of the normalized integration kernel.
5. Use Theorem G4 or Proposition G6 with a legitimate common complex domain, then sum the remaining localized carriers with unspent decay.

[The normalized-kernel and block-oscillation analysis](block_oscillation_alternative.md) provides a separate sufficient method for item 4. The present geometric lemmas explain how to pay the physical distance that a fixed integrated component can transmit freely.

### Strategy B: keep original birth records and use the actual physical measure

1. Extract the exact derivative normalization and root measure for every relevant record class.
2. Show that each class really contains the factors needed for (G15), with a localized kernel uniform in volume and history.
3. Prove a birth-coupling prefactor and the drift (G16) strong enough to use (G17).
4. Justify the differentiated expansion on the common domain and all remaining spatial sums.

This strategy cannot use a fictitious volume factor, nor treat all boundary activities as dimension-four irrelevant vertices without proof.

### The precise irreducible missing statement

A viable actual-model repair would prove one of the following, uniformly over the admitted histories:

> **Rebased form:** the full current response after repeated completion has an absolutely summable localization in a paid component metric, with maximal-component path geometry and collar reserve sufficient for (G10).

or

> **Original-record form:** the exact root measures and surviving charged kernels permit an absolute spatial and birth sum, with no unpaid refinement factor, as in (G15)–(G17).

Neither statement is proved by the source-free scalar stability result alone. The first is weaker than requiring every old summand to retain exponential decay in its original age, and is the more promising replacement after the source resummations.

## 9. Result and limitations

This note supplies three substantive repair mechanisms with complete proofs:

- a grade ledger that records exactly what free contractions can erase;
- a geometric and weighted-row theorem that pays free component traversal by a controlled diameter, including a small-coupling corollary;
- a direct physical-measure and AF summation that can replace the original age entropy when its actual normalization premises hold.

## References

- **[B88]** T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, Communications in Mathematical Physics **119** (1988), 243–285. [DOI](https://doi.org/10.1007/BF01217741). Relevant printed pages: 260–264.
- **[B87]** T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. I*, Communications in Mathematical Physics **109** (1987), 249–301. [DOI](https://doi.org/10.1007/BF01215223). The connected-tree definition is on printed p.257.
- **[B88-II]** T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. II. Cluster Expansions*, Communications in Mathematical Physics **116** (1988), 1–22. [DOI](https://doi.org/10.1007/BF01239022). Its published (1.31) is the scaling comparison referred to with older section numbering in the later papers.
- **[B89-II]** T. Balaban, *Large Field Renormalization. II. Localization, Exponentiation, and Bounds for the R Operation*, Communications in Mathematical Physics **122** (1989), 355–392. [DOI](https://doi.org/10.1007/BF01238433). Relevant printed pages: 373–380, 384–387, and 391–392.
