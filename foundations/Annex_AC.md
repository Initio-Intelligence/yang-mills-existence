# Latent rare histories, full reset jets and a spatial mixing certificate

**Annex AC.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 0. Results and hypotheses

Neither H-02 nor H-03 is completed by this note. The actual inherited low-margin probabilities and the spatial mixing of the actual normalized history posterior have not been bounded. The results below make two further parts of those problems exact.

First, a rare history may be latent inside the conditional law being averaged. There is still a bound with its full unconditional probability factor for the **change of conditional cumulants** caused by modifying marks only on that history. One does not have to retain the rare event as an output coordinate, normalize on its complement, or assume a lower bound on its conditional probability. The result extends to a complete finite logarithmic source jet without adding a factorial exponent to its existing combinatorial budget.

Second, an averaged coupling bound for a cut of the actual history posterior implies an all-order spatial cumulant estimate. A longest-edge cut of a minimum spanning tree gives the required tree-length range, with a fixed factorial exponent. This is a concrete sufficient mixing certificate; the certificate itself remains unproved for the full Balaban history law.

All probability laws used below are normalized positive laws. Signed polymer activities are never used as history probabilities. Every construction is finite at a cutoff, and every statement about arbitrary source order is an identity or estimate for finite jets of every order, not a claim about convergence of an infinite source series.

### 1. Conditional replicas retain the correct probability

Let a finite-cutoff positive history space have law

\[
 d\mu(y,h)=d\nu(y)\,\pi_y(dh).
 \tag{H.1}
\]

The retained datum is \(y\). The variable \(h\) includes every variable to be averaged at the specified operation. It need not consist only of discrete labels. The standard Borel spaces and actual disintegration are the ones constructed in Annex W. Write

\[
 (QF)(y)=\int F(y,h)\,\pi_y(dh).
 \tag{H.2}
\]

For a partition \(\mathcal P\) of \(\{1,\ldots,k\}\), introduce one independent conditional replica \(h_B\) for each block:

\[
 d\mu_{\mathcal P}
 =d\nu(y)\prod_{B\in\mathcal P}\pi_y(dh_B).
 \tag{H.3}
\]

Independence is conditional on \(y\), and is asserted only for the new replicas in (H.3). The original histories need not have any independence property. Every single pair \((y,h_B)\) has marginal \(\mu\).

Let \(E\) be an event on the input space, with \(q=\mu(E)\). It need not be measurable with respect to \(y\). If \(B_*\) is one block of a partition, then

\[
 \mu_{\mathcal P}\bigl((y,h_{B_*})\in E\bigr)=q.
 \tag{H.4}
\]

This identity is what permits an event factor after products of conditional moments have appeared. It does not replace \(\pi_y(E)\) by \(q\) pointwise.

#### Lemma H.1 — a replica event estimate

Let positive integers \(d_1,\ldots,d_k\) have sum \(m\). Suppose functions \(Z_i\) obey

\[
 \|Z_i\|_{L^p(\mu)}\le b_i p^{s d_i}
 \quad(p\ge1),\qquad s\ge0.
 \tag{H.5}
\]

Choose any partition \(\mathcal P\), write \(B(i)\) for the block containing \(i\), and choose a distinguished block \(B_*\). For \(0<q\le1\), put \(\lambda=\log(1/q)\). Then

\[
 \int\mathbf1_E(y,h_{B_*})
       \prod_{i=1}^k|Z_i(y,h_{B(i)})|\,d\mu_{\mathcal P}
 \le q e^m(m+\lambda)^{s m}\prod_i b_i.
 \tag{H.6}
\]

The bound is zero when \(q=0\).

**Proof.** For \(0<q<1\), set \(r=1+\lambda/m\). Apply Hölder to the event with exponent \(r/(r-1)\), and to the \(i\)-th function with exponent \(rm/d_i\). Their reciprocal exponents sum to one. Since each replica has the correct marginal, (H.5) yields

\[
 q^{1-1/r}\prod_i b_i(rm/d_i)^{s d_i}
 \le q e^{\lambda/r}(rm)^{s m}\prod_i b_i.
\]

Here \(\lambda/r\le m\) and \(rm=m+\lambda\). This proves (H.6). For \(q=1\), omit the event and use Hölder with exponents \(m/d_i\). For \(q=0\), (H.4) proves the assertion. No conditional normalizer was estimated. \(\square\)

### 2. Changing marks on a latent bad history

For functions \(A_1,\ldots,A_k\), their conditional cumulant is the finite expression

\[
 \kappa_Q(A_1,\ldots,A_k)
 =\sum_{\mathcal P\in\Pi_k}
  (-1)^{|\mathcal P|-1}(|\mathcal P|-1)!
  \prod_{B\in\mathcal P}Q\!\left(\prod_{i\in B}A_i\right).
 \tag{H.7}
\]

All the products in (H.7) are integrable under the moment assumptions below. Complex marks are allowed; the cumulant is multilinear, with any desired conjugations included in the specified marks themselves.

#### Theorem H.2 — latent rare-edit stability

Let \(A_i,B_i\), \(1\le i\le k\), satisfy \(A_i=B_i\) outside the same event \(E\), and suppose

\[
 \max\{\|A_i\|_p,\|B_i\|_p\}\le b_i p^{s d_i},
 \qquad p\ge1,\qquad \sum_i d_i=m.
 \tag{H.8}
\]

Then

\[
 \int\left|\kappa_Q(A_1,\ldots,A_k)
                 -\kappa_Q(B_1,\ldots,B_k)\right|d\nu
 \le q\,2^k k k! e^m(m+\lambda)^{s m}\prod_i b_i.
 \tag{H.9}
\]

For \(k=1\), the left side is the difference of conditional means and the formula remains valid. The right side is interpreted as zero for \(q=0\).

**Proof.** Multilinearity gives the exact telescope

\[
 \kappa_Q(A_1,\ldots,A_k)-\kappa_Q(B_1,\ldots,B_k)
 =\sum_{j=1}^k
  \kappa_Q(B_1,\ldots,B_{j-1},A_j-B_j,A_{j+1},\ldots,A_k).
 \tag{H.10}
\]

For each term in its partition formula, designate the block containing the difference. Its absolute value is bounded by the product of conditional absolute moments, with \(\mathbf1_E\) in the designated block. Integrating represents that product on (H.3). Apply Lemma H.1, using the bound \(2b_j p^{s d_j}\) for the difference and the original bounds for the other marks.

The sum of absolute cumulant coefficients is at most \(k!2^{k-1}\). Indeed, ordered set partitions can be encoded by a permutation of the \(k\) labels and a choice of cuts in its \(k-1\) gaps. Their count bounds the coefficient sum. Multiplying by the two from the difference and by the \(k\) telescoping terms proves (H.9). \(\square\)

The event in this theorem is inside a conditional replica. This differs from a bound of the form \(\int\mathbf1_E|\kappa_Q|\), which places the event outside the conditional cumulant. The latter cannot be used when an input event has been averaged away without explicitly enlarging the output. Theorem H.2 avoids that enlargement for the stated **comparison** of cumulants.

For full product coefficients, telescoping directly before conditioning yields

\[
 \int\left|Q\!\left(\prod_i A_i\right)
              -Q\!\left(\prod_i B_i\right)\right|d\nu
 \le 2k q e^m(m+\lambda)^{s m}\prod_i b_i.
 \tag{H.11}
\]

There is no cumulant partition factor in (H.11).

#### Application to the actual compact Wilson input

On the cofinal reserve class of Annex A, the energy-normalized 21-field representatives obey

\[
 \|O_{\alpha,a}(x)\|_p\le C a^{-4}p,
 \qquad p\ge1.
 \tag{H.12}
\]

The microscopic Wilson marginal is unchanged by the complete positive history lift. Therefore (H.12) holds on that lift for every actual inherited event \(E\), with its actual normalized probability \(q\). Taking \(B_i=\mathbf1_{E^c}A_i\), and using conditional Jensen when \(A_i\) is an exactly transported original mark, gives

\[
 \int|\kappa_Q(A_1,\ldots,A_m)
          -\kappa_Q(\mathbf1_{E^c}A_1,\ldots,\mathbf1_{E^c}A_m)|d\nu
 \le q C^{m+1}m!(m+\log(1/q))^m a^{-4m}.
 \tag{H.13}
\]

The same coefficient dictionary and source-free positive law as Annex W are used. Additional running mixing coefficients must be included explicitly in the input budgets; (H.13) does not absorb them into \(C\).

This is an actual finite-Wilson comparison for arbitrary inherited events. It does **not** give the missing upper bound on \(q\), and its physical field budget is still \(a^{-4}\), not the desired current-scale \(h^{-4}\). The clipping in (H.13) is an estimation device, not a proposed replacement of the physical field or a claim that clipping preserves locality or OS positivity.

### 3. Stability of the whole reset jet

Fix a finite set of distinct source labels. For every nonempty subset \(I\), let \(A_I\) and \(B_I\) be the coefficients of two incoming logarithmic jets. Repeated field types are allowed: the auxiliary source labels remain distinct. Set

\[
 A_I^+=\sum_{\mathcal P\in\Pi(I)}
              \kappa_Q(A_J:J\in\mathcal P),
 \qquad
 B_I^+=\sum_{\mathcal P\in\Pi(I)}
              \kappa_Q(B_J:J\in\mathcal P).
 \tag{H.14}
\]

These are exactly the coefficients of \(\log Qe^{\Psi_A}\) and \(\log Qe^{\Psi_B}\). Thus every already generated multi-field vertex is retained.

#### Theorem H.3 — complete rare-edit jet bound

Assume \(p_0\ge1\), \(s\ge0\), \(C\ge1\), \(b>0\), and

\[
 A_J=B_J\quad\hbox{outside }E,
\]

\[
 \max\{\|A_J\|_p,\|B_J\|_p\}
 \le C^{d+1}(d!)^{p_0} b^d p^{s d},
 \qquad d=|J|,\quad p\ge1.
 \tag{H.15}
\]

There is \(C_*\), depending only on \(C\), such that for every \(I\) of size \(m\ge1\),

\[
 \boxed{
 \int|A_I^+-B_I^+|\,d\nu
 \le q C_*^{m+1}(m!)^{p_0}
          (m+\log(1/q))^{s m}b^m.
 }
 \tag{H.16}
\]

This construction is compatible under truncation at every source order.

**Proof.** Apply Theorem H.2 to the \(k\) block marks in each partition of \(I\), with block degrees \(d_1,\ldots,d_k\). Their total degree is \(m\). The product of moment constants contributes at most

\[
 C^{m+k} b^m\prod_{j=1}^k(d_j!)^{p_0}.
\]

It remains to bound a purely finite partition sum. For fixed \(k\),

\[
 \sum_{\substack{\mathcal P\in\Pi_m\\|\mathcal P|=k}}
 k!\prod_{J\in\mathcal P}(|J|!)^{p_0}
 =m!\sum_{\substack{d_1+\cdots+d_k=m\\d_j\ge1}}
        \prod_{j=1}^k(d_j!)^{p_0-1}.
 \tag{H.17}
\]

This follows by first ordering the blocks and then choosing their labels. Since \(p_0\ge1\), each product on the right is at most \((m!)^{p_0-1}\). There are \(\binom{m-1}{k-1}\) ordered compositions. The remaining factors \(k2^k C^k\), summed over \(k\), are bounded by a constant to the power \(m+1\), because \(k\le m\le2^m\). Equation (H.16) follows. The formula for a coefficient of order \(m\) uses no coefficient of higher order, proving truncation compatibility. \(\square\)

The estimate does not add a factorial exponent to \(p_0\) through the reset partition sum. The degree-dependent moment factor remains explicit. An actual iteration still needs a useful current-scale input budget, spatial localization, and a summable probability/geometry budget. None follows just from (H.16).

#### Corollary H.3a — an explicit carrier-sum threshold

Suppose corrections are indexed by finite carriers \(D\) containing a fixed anchor, with integer size \(r(D)\ge1\). Assume that at most \(A^r\) such carriers have size \(r\), with \(A\ge1\), that each correction is a comparison of the form (H.16) with the same constants, and that its actual event probability satisfies, for \(\sigma>0\),

\[
 q_D\le e^{-\sigma r(D)}.
 \tag{H.16a}
\]

For a carrier weight \(e^{\kappa r(D)}\), the strict inequality

\[
 \sigma>\kappa+\log A
 \tag{H.16b}
\]

is sufficient to give

\[
 \sum_{D\ni x}e^{\kappa r(D)}
        \int|A_{I,D}^+-B_{I,D}^+|\,d\nu
 \le C_{C,\sigma,\kappa,A,s}^{m+1}(m!)^{p_0+s}b^m.
 \tag{H.16c}
\]

No independence or disjointness among the carrier events is required.

**Proof.** Choose \(\varepsilon\in(0,1)\) such that
\((1-\varepsilon)\sigma>\kappa+\log A\). For \(\lambda\ge0\), maximizing
\(e^{-\varepsilon\lambda}(m+\lambda)^{sm}\) gives

\[
 e^{-\lambda}(m+\lambda)^{sm}
 \le C_{s,\varepsilon}^{m+1}(m!)^s
                   e^{-(1-\varepsilon)\lambda}.
\]

This includes \(s=0\). Apply it to \(\lambda_D=\log(1/q_D)\), use (H.16a), and sum the resulting geometric series over \(r\ge1\). Its ratio is
\(\exp[\kappa+\log A-(1-\varepsilon)\sigma]<1\). This proves (H.16c). \(\square\)

This identifies an explicit competition between probability suppression and carrier count. It does not prove (H.16a) for an inherited sector, or a current-scale bound for the input jets. If the actual carriers have extra factors growing with their size, those factors must be included in the sum rather than hidden in \(C\).

### 4. A concrete spatial certificate for the actual posterior

Let \(A_i(y,h)\), \(i=1,\ldots,m\), be marks assigned to spatial anchors \(x_i\), and suppose

\[
 \|A_i\|_p\le C b_i p^s,\qquad p\ge1.
 \tag{H.18}
\]

For a nontrivial cut \(I\sqcup J=\{1,\ldots,m\}\), let \(\sigma_y\) be the joint conditional law of the two vectors \(A_I,A_J\), and let \(\sigma_y^I\otimes\sigma_y^J\) be the product of its two marginals. Define the **actual conditional cut defect**

\[
 q_{I|J}
 =\int \|\sigma_y-\sigma_y^I\otimes\sigma_y^J\|_{\mathrm{TV}}\,d\nu(y),
 \tag{H.19}
\]

where total variation is \(\sup_E|P(E)-Q(E)|\in[0,1]\). The definition is in terms of the normalized history posterior, not the fresh R reference law.

At a finite lattice, for finite history labels, a measurable maximal coupling is explicit. On a common finite value set its common part is the pointwise minimum of the two probability masses; couple that part identically and couple their disjoint residual parts. More generally the same construction uses the two densities with respect to their sum on a standard Borel space. The conditional densities and resulting kernels may be chosen measurably; alternatively the following theorem can take a specified measurable coupling with failure probability \(q\) as its input, without invoking optimality.

#### Theorem H.4 — averaged cut mixing implies a cumulant bound

For every nontrivial cut and \(q=q_{I|J}>0\),

\[
 \int |\kappa_{\pi_y}(A_1,\ldots,A_m)|\,d\nu(y)
 \le q C_1^{m+1}m!(m+\log(1/q))^{s m}\prod_i b_i.
 \tag{H.20}
\]

It is zero if \(q=0\). The same statement holds using any proved upper-bound coupling failure probability, with the monotonic replacement described below.

**Proof.** Conditional on \(y\), couple the original vector \(A\) to a vector \(B\) with law \(\sigma_y^I\otimes\sigma_y^J\). The two vectors agree outside a coupling failure event of unconditional probability \(q\). Their individual coordinates have the same marginal laws, so (H.18) holds for both. The conditional cumulant of all \(B_i\) is zero: its formal logarithmic generating jet is a sum of the jets for the two independent subvectors, hence has no mixed coefficient involving both. Apply Theorem H.2 on this enlarged conditional probability space, with all degrees equal to one, and absorb \(m2^m\) into \(C_1^{m+1}\). \(\square\)

For \(s>1\), the function \(q(m+\log(1/q))^{sm}\) need not be monotone on all \((0,1]\). A safe consequence of (H.20), valid for every \(s\ge0\), is

\[
 \boxed{
 \int |\kappa_{\pi_y}(A_1,\ldots,A_m)|\,d\nu(y)
 \le C_s^{m+1}(m!)^{s+1}q^{1/2}\prod_i b_i.
 }
 \tag{H.21}
\]

To prove it, write \(q=e^{-\lambda}\), \(\lambda\ge0\), and maximize
\(e^{-\lambda/2}(m+\lambda)^{sm}\). If \(s=0\) the expression is at most one. If \(s>0\), the maximum occurs at \(\lambda=\max(0,(2s-1)m)\), and is at most \(C_s^m m^{sm}\le C_s'^m(m!)^s\). Substitution in (H.20) proves (H.21). This bound is monotone in the proved upper bound on \(q\).

#### Corollary H.5 — a tree-length estimate with a fixed factorial exponent

Let \(\tau(x_1,\ldots,x_m)\) be the length of a minimum spanning tree in the chosen physical metric, and let \(h>0\) be the current scale. Suppose, for the actual marks and posterior, every nontrivial cut satisfies the quantitative certificate

\[
 q_{I|J}\le
 \min\{1,D^m\exp[-c\,d(x_I,x_J)/h]\},
 \qquad D\ge1,\quad c>0.
 \tag{H.22}
\]

Then, for \(m\ge2\),

\[
 \boxed{
 \int |\kappa_{\pi_y}(A_1,\ldots,A_m)|\,d\nu(y)
 \le C_{s,C,D}^{m+1}(m!)^{s+1}
 \exp\!\left[-\frac{c\,\tau(x_1,\ldots,x_m)}{2(m-1)h}\right]
 \prod_i b_i.
 }
 \tag{H.23}
\]

**Proof.** A longest edge of a minimum spanning tree has length at least \(\tau/(m-1)\). Removing it gives a cut. Every edge crossing that cut has length at least the removed edge: a shorter one would produce a spanning tree of smaller total length. Consequently the cut distance in (H.22) is at least \(\tau/(m-1)\). Apply (H.21), and absorb \(D^{m/2}\) into the constant. \(\square\)

For marks supported on spatial carriers, use their actual supports in the cut distance. Anchor distance can replace support distance only after subtracting the corresponding carrier radii or proving a localization estimate. A nominal insertion label does not make a globally history-dependent mark local.

The conclusion has the range dependence needed by the existing shell-summation architecture. If the input budget were \(b_i\le Ch^{-4}\), it would also have the current-scale physical prefactor. This conditional statement supplies neither that budget nor (H.22) for the interacting history posterior.

The theorem bounds the conditional cumulant averaged over \(y\). An additional external history parameter can be held fixed throughout the proof, but uniformity in that parameter requires the input moment and cut-coupling bounds with the same constants for every admitted parameter. It cannot be obtained by averaging over that parameter first. Retained-coordinate derivatives require the corresponding score/current marks and their own moment and coupling budgets. The outer cumulants of conditional means remain the separate H-05 obligation.

### 5. What the new estimates do and do not remove

#### 5.1 No hidden normalization on a good sector

Equations (H.9), (H.13) and (H.16) do not form \(\pi_y(\cdot\mid E^c)\). They remain valid on retained data where \(\pi_y(E)=1\), and they have no factor \(1/\pi_y(E^c)\). The reference or clipping values are compared inside the unchanged normalized law. This removes one avoidable denominator from estimates of proposed rare-history corrections.

The probability \(q\) remains the actual full-law probability. A small unnormalized branch mass or a fresh-reference failure probability cannot replace it.

#### 5.2 A mixture can still have nonlocal reset responses

Let \(h=\pm1\) have equal probability, and place \(A_1=h\), \(A_2=h\) at arbitrarily distant anchors. There is no retained datum. Each mark has bounded moments, while \(\kappa(A_1,A_2)=1\). The joint sign law has total variation distance \(1/2\) from the product of its marginals, independent of the anchor distance. Thus (H.22) fails, exactly where the proof of spatial decay requires it.

This is a check of the certificate's necessity as an added input to the displayed sufficient argument. It is not a Yang–Mills counterexample and does not assert that cut total variation is the only possible route to H-03. Weighted couplings or direct cumulant estimates may be more efficient for continuous or strongly constrained histories.

#### 5.3 Full jet comparison is not locality of its coefficients

The factorial estimate (H.16) is integrated over retained data and has no spatial factor. Even if an event is rare, a correction supported on it may depend on a large carrier. Its carrier norm must be paid using the actual geometry. At the same time, a cutoff-wide clipping event can destroy the locality of a mark. The theorem licenses the stated bound, not an unexamined field redefinition.

### 6. Application conditions

| Statement | New proved work | Still required by the original hypotheses |
|---|---|---|
| **H-02** | Rare-edit estimates for latent history events under the actual normalized law; all-order extension to complete reset jets; no good-sector conditional denominator. | A current-scale bound for the actual inherited low-margin and unreplaced events, with overlap and geometric costs sufficient to pay the insertion/carrier losses. Neither the needed probability nor the current-scale field budget follows from the new theorem. |
| **H-03** | An averaged conditional cut-coupling criterion implying all-order tree-length decay with fixed factorial growth; actual normalized posterior specified; full jets retained. | Prove the cut certificate or a sufficient direct spatial response estimate for the actual history posterior, uniformly in the remaining history and at the required current scale. |


### Sources

The probability identities and estimates in this note are proved directly. Their finite Wilson application uses the already proved compact Wilson reserve and field bounds retained in Annex A, the positive-history construction in Annex W, and the exact reset-jet identity retained in Annex I. No new external mathematical theorem about Yang–Mills is imported. The maximal-coupling formulation can be replaced throughout by a supplied finite measurable coupling, as stated above.


---


---
