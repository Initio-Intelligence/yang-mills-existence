# Exact history resampling and normalized source scores

**Annex I.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

The complete transported-observable theorem M0 is **not proved** in this note. The native conditional moment theorem concerns a specified homogeneous regular law and its newly evaluated current fields. It does not identify those fields with the conditional expectations of renormalized microscopic Wilson insertions. The new work below does not change that distinction.

There is an exact improvement to the way the remaining theorem can be formulated. Auxiliary history variables can be averaged at every step, even when the next source-free map needs such variables, provided they are resampled from their **baseline conditional law** before reuse. The whole marked source jet is transported through this extra positive operation. The unmarked state and every final Schwinger coefficient are preserved. This removes an unnecessary prohibition on averaging live auxiliary labels.

The price is explicit: history averaging creates conditional covariance and higher cumulant responses. Its conditional kernel can be nonlocal. Neither its positivity nor its norm contraction supplies their spatial decay or current-scale normalization. Thus this is a useful exact representation theorem, not a missing ultraviolet estimate hidden in a change of notation.

The second part identifies exactly when a reference-kernel score disappears under such an averaging. The entire normalized reference likelihood jet cancels when all of its reference variables are averaged and the other marked coefficient depends only on the retained data. First-score mean zero does not justify deleting individual higher logarithmic derivatives or correlations with marks that still depend on those reference variables.

The source analysis also verifies the coupling-regularity statement in CMP109 and its qualification: the notation for a beta function suppresses its dependence on all preceding couplings. The checked one-parameter smoothness is not a proved local-source derivative bound or a bound on every total derivative along the complete history construction.

Here P denotes a proof from the stated hypotheses, L a scoped primary input, and O an unproved application to the actual complete Wilson observable induction.

### 1. The positive augmented state

At a finite cutoff, work before the introduction of signed polymer activities. Let the source-free augmented state be

\[
X=(V,\omega)\in\mathcal V\times\Omega,
\qquad
\mu(dV,d\omega)=\nu(dV)\,\pi(d\omega\mid V).
\tag{1.1}
\]

Both spaces are standard Borel. In the finite lattice construction this includes compact link variables, finitely many discrete selectors/history labels, and the finite-dimensional chart variables used on a branch. An admissible-state subset can be incorporated by declaring that \(\pi(\cdot\mid V)\) is supported on its fiber.

The field \(V\) is the coordinate or collection of retained data chosen for the next matching norm. The symbol \(\omega\) denotes everything one proposes to average. Some components may be needed by the next source-free operation; they will be resampled rather than erased from the state space. The augmented state must contain every input used by that next operation. If the construction has further path-dependent inputs, include them in \(X\) first; no Markov property after an unauthorized omission is assumed.

The disintegration in (1.1) exists. At points with zero \(\nu\)-mass its value is irrelevant and can be fixed arbitrarily. Where a density or a finite history sum is available, it is simply the ratio of the known source-free joint density to its marginal. No source-dependent denominator or new sourced minimizing field is used.

Define

\[
(\Pi F)(V)
=\int F(V,\omega)\,\pi(d\omega\mid V).
\tag{1.2}
\]

### 2. Exact averaging and resampling

#### Theorem 2.1 — history resampling with unchanged baseline law, P

Define the source-free Markov kernel

\[
\mathcal R\bigl((V,\omega),dV'\,d\omega'\bigr)
=\delta_V(dV')\,\pi(d\omega'\mid V).
\tag{2.1}
\]

It has the following properties.

1. \(\mu\mathcal R=\mu\).
2. On functions it is the conditional-expectation projection \(\Pi\), lifted back to the augmented state:
   \[
   (\mathcal RF)(V,\omega)=\Pi F(V).
   \tag{2.2}
   \]
3. If the old state is sampled from \(\mu\) and then \(\mathcal R\) is applied, the marked numerator transport is the same projection:
   \[
   Q_{\mathcal R}F
   =\mathbb E[F(X)\mid X']
   =\Pi F(V').
   \tag{2.3}
   \]
4. \(\Pi^2=\Pi\), \(\Pi1=1\), and
   \[
   \int\Pi F\,d\mu=\int F\,d\mu,\qquad
   \|\Pi F\|_{L^p(\mu)}\le\|F\|_{L^p(\mu)}
   \quad(1\le p\le\infty).
   \tag{2.4}
   \]
5. On \(L^2(\mu)\), the projection is self-adjoint. In particular,
   \[
   \|F-\Pi F\|_2^2=\|F\|_2^2-\|\Pi F\|_2^2.
   \tag{2.5}
   \]

**Proof.** Under the joint old/new law, conditional on \(V\), the two labels \(\omega,\omega'\) are independent with the same distribution \(\pi(\cdot\mid V)\). This proves (2.2)–(2.3). Integrating the new conditional law gives (1), and the conditional-expectation identities and Jensen inequality give (2.4). For \(F,G\in L^2\),
\(\int\overline F\,\Pi G\,d\mu=\int\overline{\Pi F}\,\Pi G\,d\nu
=\int\overline{\Pi F}\,G\,d\mu\).
This proves self-adjointness, idempotence, and the orthogonal decomposition (2.5). \(\square\)

#### Corollary 2.2 — future maps may still use the labels, P

Let \(\mathcal K_k\) be the next source-free Markov operation, carrying \(\mu_k\) to \(\mu_{k+1}\). Its selectors, integration coordinates and reference factors may depend on \(\omega_k\). Insert \(\mathcal R_k\) before it. Then

\[
\mu_k\mathcal R_k\mathcal K_k
=\mu_k\mathcal K_k
=\mu_{k+1}.
\tag{2.6}
\]

The marked transport for the inserted two-step operation is

\[
Q_{\mathcal R_k\mathcal K_k}F
=Q_k\Pi_kF.
\tag{2.7}
\]

The label resampled by \(\mathcal R_k\) is admissible for its current field because it is sampled from the original conditional fiber. Thus the next operation remains well-defined almost surely. One has changed the joint coupling between the incoming mark and future history choices, but not any unmarked state law or integrated marked expectation.

**Proof.** Equation (2.6) uses stationarity from Theorem 2.1. For an output test \(H\), the defining joint-law identity for conditional expectation gives
\[
\int H\,Q_{\mathcal R_k\mathcal K_k}F\,d\mu_{k+1}
=\int (\mathcal K_kH)\,\Pi_kF\,d\mu_k
=\int H\,Q_k\Pi_kF\,d\mu_{k+1}.
\]
This proves (2.7). \(\square\)

An arbitrary finite sequence can therefore have such a reset at every stage. Every unmarked marginal of the original source-free construction remains the same. Future histories are still sampled from their actual baseline laws at each stage; what changes is their pathwise correlation with the original marked variables.

This corrects the overly restrictive formulation that a live label cannot be averaged because a later step uses it. It can be averaged **and resampled**. Simply deleting it while keeping a next map that requires it would not define an operation.

#### Corollary 2.3 — the complete source jet is preserved, P

Let \(G_k(t)\) be a marked polynomial or formal series truncated above source degree \(M\), with \(G_k(0)=1\). Apply \(\Pi_k\) coefficient by coefficient, then apply the next original positive transport. At every finite source order,

\[
\int \Pi_kG_k(t)\,d\mu_k
=\int G_k(t)\,d\mu_k.
\tag{2.8}
\]

After any number of inserted resets and original operations, every integrated coefficient equals its original cutoff Wilson coefficient.

The proof is linearity and (2.4), applied to finitely many coefficients. No positivity of the coefficients or convergence of an infinite source series is needed. The baseline Markov law is positive; its signed marked coefficients need not be.

It is essential to reset \(G_k\) itself. Replacing it by
\(\exp(\sum_i t_i\Pi_kF_{i,k})\) generally changes every order above one.

### 3. The responses generated by a reset

#### 3.1 Exact source-jet rule

Put \(\Psi=\log G\) and \(A_I=\partial_I\Psi(0)\) for nonempty sets of distinct source labels. The reset logarithm is

\[
\Psi^+=\log\Pi e^\Psi.
\]

The finite cumulant expansion gives

\[
\boxed{
A_I^+
=\sum_{\mathcal P\in\Pi(I)}
\kappa_\pi(A_B:B\in\mathcal P).
}
\tag{3.1}
\]

Here \(\kappa_\pi\) is a conditional cumulant in the label law \(\pi(\cdot\mid V)\). In particular,

\[
A_i^+=\Pi A_i,\qquad
A_{ij}^+=\Pi A_{ij}
+\operatorname{Cov}_\pi(A_i,A_j).
\tag{3.2}
\]

The same formula includes all responses already created by earlier integrations. For instance, \(A_{ij}\) need not vanish before the reset.

**Proof.** In the truncated polynomial algebra,
\[
\log\Pi e^\Psi
=\sum_{r=1}^{M}\frac1{r!}\kappa_\pi(\Psi,\ldots,\Psi).
\]
Extracting the coefficient with label set \(I\) groups its labels into a partition; all sums are finite. This yields (3.1). \(\square\)

#### 3.2 Direct product errors and their norms

For single marks \(F_1,\ldots,F_m\), the extra product error is

\[
D_m^\pi
=\Pi\Bigl(\prod_{i=1}^mF_i\Bigr)
-\prod_{i=1}^m\Pi F_i.
\tag{3.3}
\]

Let \(\eta_i=F_i-\Pi F_i\). Conditional centering gives the exact expansion

\[
D_m^\pi
=\sum_{\substack{I\subset\{1,\ldots,m\}\\|I|\ge2}}
\Pi\Bigl(\prod_{i\in I}\eta_i\Bigr)
\prod_{j\notin I}\Pi F_j.
\tag{3.4}
\]

For \(1\le p<\infty\),

\[
\|D_m^\pi\|_p
\le2\prod_i\|F_i\|_{pm},
\tag{3.5}
\]

and also

\[
\|D_m^\pi\|_p
\le
\sum_{|I|\ge2}
\prod_{i\in I}\|\eta_i\|_{pm}
\prod_{j\notin I}\|F_j\|_{pm}.
\tag{3.6}
\]

The first inequality is conditional Jensen and Hölder for the two terms of (3.3); the second applies the same inequalities to (3.4). The corresponding \(p=\infty\) statements use the sup norms.

For conditional cumulants of arbitrary marks,

\[
\boxed{
\|\kappa_\pi(F_1,\ldots,F_m)\|_p
\le m!2^{m-1}\prod_i\|F_i\|_{pm}.
}
\tag{3.7}
\]

For a partition with blocks \(B\), conditional Jensen and Hölder bound
\(\prod_B\Pi(\prod_{i\in B}F_i)\) in \(L^p\) by the same product of \(L^{pm}\) norms. The absolute partition coefficient sum is
\(\sum_{\mathcal P}(|\mathcal P|-1)!\), bounded by \(m!2^{m-1}\) using ordered partitions encoded by a permutation and cuts. This proves (3.7).

These bounds are denominator-free after averaging over the physical marginal. They can control response magnitudes when the input marks have useful norms. They supply no separation factor on their own.

#### 3.3 Variance removed from a mark is retained in the hierarchy

For real \(F,G\in L^2(\mu)\),

\[
\operatorname{Cov}_\mu(F,G)
=\mathbb E_\nu[\operatorname{Cov}_\pi(F,G)]
+\operatorname{Cov}_\nu(\Pi F,\Pi G).
\tag{3.8}
\]

In particular, the norm decrease (2.5) reappears as the integrated second-order response. It is not erased.

A simple finite example makes the spatial limitation explicit. Take a single auxiliary sign \(\omega=\pm1\) with equal probabilities, no physical retained variable, and two marks assigned to arbitrarily separated labels,
\[
F_n(x)=n\omega,\qquad F_n(y)=n\omega.
\]
The reset makes both single marks zero, but
\[
D_2^\pi(x,y)=n^2.
\tag{3.9}
\]
Thus arbitrarily good post-reset single-mark norms do not imply a bounded or decaying full two-point function. This is a counterexample to that inference, not a model of Yang–Mills.

The conditional law \(\pi(d\omega\mid V)\) can itself correlate remote regions. Applying Theorem 2.1 therefore does not preserve a previously available spatial polymer norm without an additional theorem. Its exactness is compatible with a difficult new response estimate.

### 4. Exactly when a reference score cancels

#### 4.1 A normalized reference family

Let \(K_\theta(da\mid v)\) be a differentiable family of probability kernels on a common support, with \(K_0\) positive there. Assume the required finite derivatives are integrable so that differentiation under the integral is justified. Define its likelihood jet and logarithmic score jets by

\[
L_\theta(a,v)=\frac{dK_\theta}{dK_0}(a\mid v),
\qquad
c_r(a,v)=\left.\partial_\theta^r\log L_\theta(a,v)\right|_{\theta=0}.
\tag{4.1}
\]

Let \(\Pi_K\) average the entire reference variable \(a\), retaining only \(v\). Normalization gives the exact formal identity

\[
\boxed{\Pi_K L_\theta=1.}
\tag{4.2}
\]

If a marked jet \(G(t,v)\) depends only on the retained data, then

\[
\boxed{\Pi_K[G(t,v)L_\theta(a,v)]=G(t,v).}
\tag{4.3}
\]

Every derivative in both \(t\) and \(\theta\) follows coefficient by coefficient. This is the precise all-order cancellation of an independent normalized reference likelihood.

At first and second orders, normalization says

\[
\Pi_Kc_1=0,\qquad
\Pi_K(c_2+c_1^2)=0.
\tag{4.4}
\]

Equivalently,
\[
\Pi_Kc_2+\operatorname{Var}_{K_0}(c_1)=0.
\tag{4.5}
\]

The second logarithmic derivative therefore does not separately average to zero. Its cancellation uses the covariance response in the reset logarithm.

For example, take \(K_\theta=N(\theta,1)\). Then
\(c_1(a)=a\), \(c_2(a)=-1\). Their separate expectations are \(0,-1\), while the full second jet has expectation
\(-1+\mathbb E a^2=0\).

#### 4.2 Application to a single positive R replacement

For a source-independent integration of the old variable \(u\), followed by a normalized reference draw \(u'\), write

\[
\rho'_\beta(u',v)
=K_\beta(u'\mid v)\,M_\beta(v),
\qquad
M_\beta(v)=\int\rho_\beta(u,v)\,du.
\tag{4.6}
\]

The exact transport of an old observable is

\[
Q_\beta F(u',v)
=
\frac{\int\rho_\beta(u,v)F(u,v)\,du}
{M_\beta(v)}.
\tag{4.7}
\]

It depends only on \(v\). The same is true for the entire transported old source jet. Consequently (4.3) applies to a variation of the normalized reference factor **at this operation**, if all of \(u'\) is averaged and the retained-data law \(M_\beta\) is treated separately.

For the bare scalar score \(\rho_\beta=e^{-\beta S}\),

\[
-\partial_\beta\log\rho'_\beta
=Q_\beta S-\partial_\beta\log K_\beta.
\tag{4.8}
\]

Averaging in \(u'\) removes the first reference score and leaves
\(-\partial_\beta\log M_\beta=Q_\beta S\). The full likelihood-jet identity, rather than a separate deletion of higher logarithmic scores, gives its all-order version.

This sharpens the earlier generic warning about mean-zero currents. A reference score is indeed orthogonal to every transported old mark that has become a function only of \(v\) at this single replacement. It is not automatically orthogonal to a mark that depends on the fresh reference field, or to a later quantity whose construction has already used that field.

#### 4.3 The cancellation has precise limits

If \(G=G(a,v)\) still depends on \(a\), generally
\[
\Pi_K(Gc_1)\ne0.
\tag{4.9}
\]
For \(K_\theta=N(\theta,1)\) and \(G(a)=a\), the left side is one.

If only some reference variables are averaged and \(a\) is retained in the matching state, the score need not disappear. If a subsequent coarse map mixes \(a\) into its new retained variable, the projected score can again be nonzero. A later global mean-zero identity does not supply spatial locality.

Finally, the theorem assumes a common-support differentiable reference family. Moving hard selectors, changes of charts or deterministic maps, and singular source-dependent supports require their own derivatives or interface terms. Equation (4.3) does not make those terms vanish.

The representation (4.6) separates the normalized reference factor from the old integrated density. It does not bound the derivative of \(M_\beta(v)\), which is precisely the scalar matching quantity that remains to be estimated.

### 5. Scalar scores after arbitrary frozen positive channels

This section records a precise target for a possible coupling-response proof. It does not derive the needed uniform bound.

Let \(\mu_\theta\) be the finite-cutoff Wilson measure with real local parameters,

\[
d\mu_\theta(U)
=
\frac{e^{-\sum_i\theta_i A_i(U)}}{\mathbb E_{\mu_0}e^{-\sum_i\theta_i A_i}}
d\mu_0(U).
\tag{5.1}
\]

The finitely many \(A_i\) may be plaquette energies or fixed smeared linear combinations. At a finite compact cutoff they are bounded. Let \(\mathcal K\) be any fixed source-free positive channel, including any finite sequence of the resets above, and let \(V\) be its output. Write \(\nu_\theta=\mu_\theta\mathcal K\).

The normalized likelihood ratio of the output is exactly

\[
\frac{d\nu_\theta}{d\nu_0}(V)
=
\frac{
\mathbb E_{\mu_0,\mathcal K}
[e^{-\sum_i\theta_iA_i}\mid V]}
{\mathbb E_{\mu_0}e^{-\sum_i\theta_iA_i}}.
\tag{5.2}
\]

Its first two logarithmic derivatives are

\[
\partial_i\log\frac{d\nu_\theta}{d\nu_0}\bigg|_0
=-\mathbb E[A_i\mid V]+\mathbb E A_i,
\tag{5.3}
\]

\[
\partial_i\partial_j\log\frac{d\nu_\theta}{d\nu_0}\bigg|_0
=\operatorname{Cov}(A_i,A_j\mid V)
-\operatorname{Cov}(A_i,A_j).
\tag{5.4}
\]

At every order, the derivative is \((-1)^m\) times the corresponding conditional cumulant minus the unconditional cumulant. These formulas follow by differentiating (5.2), justified by boundedness at the finite cutoff.

For the first score vector, conditional Jensen gives the Fisher-information matrix inequality

\[
\operatorname{Cov}\!\left(\mathbb E[A\mid V]\right)
\preceq \operatorname{Cov}(A).
\tag{5.5}
\]

The difference is the positive matrix \(\mathbb E\,\operatorname{Cov}(A\mid V)\). This is exactly the second-order response discarded by single-mark projection.

For the global scalar coupling, \(A=S\), so the current scalar insertion is a derivative of the **frozen-channel physical marginal**. This avoids fictitious derivatives of a source-dependent reference draw, but its uniform local derivative norm remains unknown. The right side of (5.5) has the microscopic ultraviolet size. The inequality alone does not replace that size by the current physical scale.

An effective-action formula proved for a different, coupling-dependent channel cannot be substituted into (5.3) without the channel-current terms. Conversely, keeping the channel frozen makes (5.3) exact but requires the actual frozen-channel derivative estimates.

### 6. What the primary coupling regularity does and does not supply

#### 6.1 Checked source statements — L

The article of CMP109, printed p.263, states that a localized \(E^{(j)}\) is analytic in its admitted gauge-field/current domain, is \(C^\infty\) in the displayed coupling parameter on a fixed interval (or analytic), and obeys the field activity bound (1.18).

Printed p.264, following (1.22), states that the beta function is smooth on its admitted interval and uniformly bounded there together with all derivatives. Theorem 3 asserts the displayed small-field inductive assumptions when the couplings and construction parameters satisfy its restrictions.

Printed p.298, in the final paragraph before the references, explicitly explains that \(\beta_j\) also depends on all the preceding couplings, although the notation displays only \(g_{j-1}\).

These are meaningful parameter-regularity inputs in the stated small-field construction. They are not a theorem about the complete local source field \(j(x)\), nor a checked bound on every mixed derivative in all earlier coupling variables and moving history data.

#### 6.2 The missing total derivative is identifiable

If one writes the actual dependence as
\[
b_j=b_j(g_0,\ldots,g_{j-1}),
\]
then along a bare-parameter path \(\lambda\mapsto(g_0(\lambda),\ldots,g_{j-1}(\lambda))\),
\[
\frac{d}{d\lambda}b_j
=\sum_{r=0}^{j-1}\partial_{g_r}b_j\,
\frac{dg_r}{d\lambda}.
\tag{6.1}
\]
Higher derivatives contain the corresponding mixed history derivatives. Uniform bounds on derivatives in the last displayed argument alone do not bound (6.1).

This failure is elementary even for analytic bounded functions. On a fixed real coupling cube, take
\[
b_j(g_0,\ldots,g_{j-1})
=b_*+\varepsilon\sin(N_jg_0),\qquad j\ge2.
\tag{6.2}
\]
The values are uniformly bounded and every positive derivative in \(g_{j-1}\) is zero. Nevertheless \(\partial_{g_0}b_j=\varepsilon N_j\cos(N_jg_0)\) can be arbitrarily large. This is a counterexample to the proposed inference from displayed-argument bounds; it is not asserted to be a Balaban beta function.

Likewise, a uniform activity bound on a complex **field** domain does not imply a uniform derivative in a different real coupling parameter. Multiplication by \(\sin(Ng)\) preserves the field-domain norm and smoothness while making the coupling derivative large. A uniform complex coupling neighborhood or a proved differentiated activity induction would rule out this example; neither can be inferred merely from field analyticity.

Even a total derivative for a homogeneous coupling would still be only the integral of the local insertion. A local source theorem has to distinguish source positions, control the corresponding carrier norms, and retain the generated partial-collision responses.

### 7. The remaining matching theorem after the exact reset reduction

The new representation permits choosing the single-mark state after each reset to be a function of \(V_k\) alone. Write

\[
\widehat F_{i,k}=\Pi_kF_{i,k}.
\]

This removes artificial large norms caused solely by an unnecessarily retained auxiliary label. A sufficient next theorem must nevertheless prove both:

\[
\|\widehat F_{i,k}\|_{L^p(\nu_k)}
\le Ap^s h_k^{-4}\ell(h_k)^b,
\tag{7.1}
\]

and a current-scale, spatially decaying bound for **every** product error from the original integration operations and the new resets. In particular, it must include

\[
\Pi_k\Bigl(\prod_iF_{i,k}\Bigr)
-\prod_i\Pi_kF_{i,k}
\tag{7.2}
\]

with the same type of shell decay required in the original S0 interface. The exact full-product telescope remains valid when these additional positive operations are inserted as extra steps.

The conditional moments can be applied to (7.1) only after \(\widehat F_{i,k}\) has been identified with the controlled native fields plus all remainders. A constant or background-dependent coefficient does not become a deterministic vacuum subtraction merely because a history was averaged.

For the scalar route, one possible concrete proof would establish a localized derivative expansion for the frozen-channel marginal in (5.2), with all vacuum terms separated and the actual current coupling dictionary retained. The missing estimate is its field-dependent local derivative norm, not the elementary score identity.

The complete construction still needs normalized inherited-history bounds, retained-data covariance, rotation restoration, ultraviolet identification, and the operator/phase theorem. None of those statements follows from the reset representation.

### 8. Completion conditions and references

| Statement | Status |
|---|---|
| Averaging and resampling auxiliary labels while preserving the complete unmarked construction | P: Theorem 2.1 and Corollary 2.2 |
| Preservation of every finite full source jet through those resets | P: Corollary 2.3 |
| Exact covariance/cumulant responses and integrated \(L^p\) bounds for a reset | P: Section 3 |
| All-order cancellation of a fully averaged normalized reference likelihood | P under the stated common-support differentiability; Section 4 |
| Cancellation of arbitrary moving-selector or later coupled reference currents | Not asserted |
| Scalar local-source score identity for an arbitrary frozen positive channel | P at finite cutoff; Section 5 |
| Uniform current-scale norm or spatial decay for the reset responses | O |
| Local-source derivatives of the complete effective marginal | O |
| Exact matching of transported microscopic Wilson fields to native current fields | O |
| Full M0/F0 or Yang–Mills existence | Not proved |

Source for the coupling statements:

T. Balaban, *Renormalization group approach to lattice gauge field theories. I. Generation of effective actions in a small field approximation and a coupling constant renormalization in four dimensions*, Communications in Mathematical Physics **109** (1987), 249–301, DOI [10.1007/BF01215223](https://doi.org/10.1007/BF01215223). The statements above concern printed pp.263–264 and p.298. The field-domain, coupling and source-variable scopes are kept distinct.

The positive-history and localized R framework is the one specified in the main paper and in the source-free construction of the earlier annexes. The exact conditional-expectation, reset, likelihood and Fisher-information identities in this note are proved directly; no additional unpublished theorem is imported.


---
