# Energy-weighted localization of an exact normalized core quotient

This proved lemma relaxes BC.2: an individual log-density perturbation may grow linearly in the actual old energy and rank. Its coefficient must then be small relative to the posterior energy scale. The actual raw supported coefficients and microscopic root budget remain unverified for the residual Yang–Mills operation.

## 1. Explicit hypotheses

Let \(D_0\) be a connected current core of bounded size. Let \(\nu_0(v_{D_0},du)\) be a positive probability kernel with genuinely local raw dependence. Its old space may contain many coordinates and a mixture of arbitrarily old histories. Let \(E(v_{D_0},u)\ge1\) obey, uniformly in retained data,
\[
 \nu_0(E^m)\le m!K^m,\qquad m=0,1,\ldots,\quad K\ge1.       \tag{EW.1}
\]
The matched RT.18 tail implies this with \(K=C(1+P^2)\), after increasing a fixed constant: use \(\|E\|_m\le Cm(1+P^2)\) and \(m!\ge(m/e)^m\). This implication does not prove that the native reference is already a raw-local \(\nu_0\).

Suppose the complete actual law is
\[
 q_v(du)=\frac{e^{\Sigma(v,u)}\nu_0(v_{D_0},du)}
                   {\nu_0(e^{\Sigma(v,\cdot)})},
 \qquad \Sigma=\sum_{X\supset D_0}\sigma_X(v_X,u),         \tag{EW.2}
\]
with connected actual raw carriers, all retained-only factors canceled consistently, and deterministic coefficientwise majorants
\[
 |\sigma_X|\le a_X E,\qquad
 \epsilon=\sum_Xw_\kappa(X)a_X,\qquad q:=K\epsilon<\tfrac12.
                                                               \tag{EW.3}
\]
Suprema over retained data precede the coefficient sum. There is no upper bound on the old rank or on \(E\).

For a marked expansion \(F=\sum_{Y\supset D_0}f_Y(v_Y,u)\), first assume
\[
 |f_Y|\le b_Y E,\qquad B=\sum_Yw_\kappa(Y)b_Y<\infty.      \tag{EW.4}
\]
All support unions are connected because they contain \(D_0\); their weights are submultiplicative.

## 2. The exact quotient

### Theorem EW.1

Under (EW.1)–(EW.4), \(q_vF\) has an absolutely convergent, actually supported tagged carrier expansion with weighted absolute value budget
\[
 \boxed{\ \frac{BK}{(1-q)(1-2q)}\ }.                     \tag{EW.5}
\]

**Proof.** Expand \(d=\nu_0(e^\Sigma-1)\) into ordered words. Its length-\(n\) carrier budget is at most
\[
 \frac{\epsilon^n}{n!}\nu_0E^n\le q^n.
\]
Thus
\[
 \|d\|_{\rm carrier}\le\frac q{1-q}<1,\qquad
 \|(1+d)^{-1}\|_{\rm carrier}
       \le\frac{1-q}{1-2q}.                             \tag{EW.6}
\]
The absolute exponential series is integrable since
\(\nu_0e^{\epsilon E}\le(1-q)^{-1}\).
The same argument proves nonvanishing of the relative denominator on any complex parameter domain satisfying these majorants.

The length-\(n\) marked numerator budget is at most
\[
 \frac{B\epsilon^n}{n!}\nu_0E^{n+1}
       \le BK(n+1)q^n.
\]
Its sum is \(BK/(1-q)^2\). Multiply by (EW.6). The individual integrals depend only on their declared support unions and on \(D_0\). Keep all word and inverse-series indices as separate tags. This proves the bound before cancellation among tags. \(\square\)

The theorem uses the actual denominator. A precision variation of size
\(\epsilon\sum_i z_i^2+\epsilon D_{\rm old}\) is allowed if this actual sum is dominated by \(E\). Arbitrary old rank is then paid through (EW.1), not declared bounded. The condition is \(K\epsilon<1/2\); for \(K=O(P^2)\), a proved coefficient \(g^s\) times a fixed polylogarithm would suffice. This observation does not establish that coefficient for the raw Schur precision.

## 3. Separate perturbation currents

First hold the reference law fixed. Suppose the actual normalized retained directions obey
\[
 \sum_d|D_d\sigma_X|\le a_{1,X}E,\quad
 \epsilon_1=\sum_Xw_\kappa(X)a_{1,X},
 \qquad
 \sum_d|D_df_Y|\le b_{1,Y}E,\quad
 B_1=\sum_Yw_\kappa(Y)b_{1,Y}.                           \tag{EW.7}
\]
Any enlarged derivative footprint is included. These estimates must hold on the independent insertion and kernel copies.

For those copies, one common envelope must dominate the insertion and kernel factors and satisfy (EW.1) under the endpoint reference law with the same \(K\). A proved comparison of the two envelopes along the rectangular paths also suffices. A merely diagonal moment bound does not establish the two-copy assertion.

The insertion-only derivative budget is
\[
 \frac{B_1K}{(1-q)(1-2q)}.                              \tag{EW.8}
\]
Differentiating the numerator exponential chooses one perturbation factor. Its kernel derivative is bounded by
\[
 B\epsilon_1\sum_{n\ge0}\frac{\epsilon^n}{n!}\nu_0E^{n+2}
       \le\frac{2B\epsilon_1K^2}{(1-q)^3}.              \tag{EW.9}
\]
Also
\[
 \|Dd\|_{\rm carrier}\le\frac{\epsilon_1K}{(1-q)^2},
 \qquad
 \|D(1+d)^{-1}\|_{\rm carrier}
       \le\frac{\epsilon_1K}{(1-2q)^2}.                 \tag{EW.10}
\]
The exact product rule therefore gives kernel-current budget
\[
 \boxed{\ 
 \frac{B\epsilon_1K^2(3-4q)}
      {(1-q)^2(1-2q)^2}\ }.                            \tag{EW.11}
\]
No \(D\sigma_X/\sigma_X\) occurs. A coefficient may vanish while its derivative does not. On a common differentiable support this is the actual covariance
\(D_{\rm ker}(qF)=\operatorname{Cov}_q(F,D\Sigma)\);
the bounds retain its distinct numerator and normalization tags.

If \(\nu_0\) varies with \(v_{D_0}\), its centered score is an additional rooted insertion. It must be estimated, not omitted. For example, if
\(\nu_0E^p\le\Gamma(p+1)K^p\) and
\(\sum_d|S^0_d|\le A_0E^{1/2}\), the corresponding reference-score terms are of order \(A_0BK^{3/2}\) with fixed rational powers of \((1-q)^{-1}\) and \((1-2q)^{-1}\). This follows by summing
\[
 \sum_{n\ge0}\frac{\Gamma(n+a+1)}{n!}q^n
       =\Gamma(a+1)(1-q)^{-a-1}.
\]
This is an explicit reference-score hypothesis.

For each two-copy tag \(H_a(v_{\rm ins},v_{\rm ker})\), use
\[
 B_{a,d,t}=\frac{H_a(v_t,v_t)-H_a(v,v_t)}t,\qquad
 J_{a,d,t}=\frac{H_a(v,v_t)-H_a(v,v)}t.                 \tag{EW.12}
\]
Integrate the separately bounded derivatives on these two rectangular paths. The common old support, path admission and shifted regulators are necessary. A discrete replacement has denominator one and requires its actual endpoint reference/readout budgets and footprint.

## 4. The local microscopic root remains a separate input

The elementary envelope (EW.4) produces \(BK\), so it does not solve RW.1's remote-witness issue. A stronger localized input can be stated explicitly.

For a monotone actual output regulator \(R_Y(v)\), suppose
\[
 \nu_0(|f_Y|E^n)
       \le b_Y R_Y(v)(n+1)!K^n,\qquad n=0,1,\ldots,     \tag{EW.13}
\]
uniformly on the required two-copy data. The same proof then gives the grade-one regulated value budget
\[
 \|\text{value}\|_{{\rm carrier},R}
       \le\frac{B}{(1-q)(1-2q)}.                       \tag{EW.14}
\]
The union regulator dominates \(R_Y\); no remote energy is moved to a smaller carrier. Direct and kernel records require their corresponding mixed moments and grades.

Equation (EW.13) is a concrete budget specified before applying the perturbation. It has not been verified for the actual previously transported microscopic scalar. Its \(n=0\) case already contains the missing localized old marked moment. The higher moments permit the supported perturbation series. Writing this budget as a hypothesis is not a proof of M-04.

## 5. Remaining actual inputs

RT supplies the native old energy/rank moment scale \(K\). The present theorem removes an unnecessary requirement that every raw log-density perturbation be uniformly bounded in all old variables. To apply it still requires:

1. A genuinely raw-local positive reference, including the specified older Schur precisions or a controlled transformation of them.
2. Actual raw-supported coefficients of the complete density difference satisfying (EW.3) and (EW.7), including all coarea, reconstruction, old precision and cross-interaction effects.
3. The microscopic mixed-moment budget (EW.13), or a different proved estimate supplying the same localized value and separate-current grades.
4. One compatible ambient extension and all actual discrete history changes.

The energy-weighted route is quantitatively weaker than BC.2. It does not bypass raw localization or microscopic scalar transport. The original M-04 statement remains open.

## 6. Transferring the known actual reserve to a constructed local reference

There is no need to assume a moment theorem for a new reference if its complete energy-weighted comparison with the known actual law has already been proved.

### Lemma EW.2

Suppose an actual positive law \(\nu\) obeys
\(\nu E^m\le m!K^m\), and a proposed positive reference on the same support satisfies
\[
 \nu_0(du)=\frac{e^{-\Sigma(u)}\nu(du)}{\nu(e^{-\Sigma})},
 \qquad |\Sigma|\le\epsilon E,\qquad q=\epsilon K\le\tfrac14 .
 \tag{EW.15}
\]
Then
\[
 \nu_0E^m\le m!(4K)^m,\qquad m=0,1,\ldots .           \tag{EW.16}
\]

**Proof.** Jensen's inequality and \(\nu E\le K\) give
\[
 \nu(e^{-\Sigma})\ge e^{-\nu\Sigma}\ge e^{-q}.
\]
For \(m\ge1\), the absolute exponential series gives
\[
 \begin{aligned}
 \nu_0E^m
 &\le e^q\,\nu(E^me^{\epsilon E})\\
 &\le e^q m!K^m
       \sum_{n\ge0}\binom{m+n}{n}q^n\\
 &=e^q m!K^m(1-q)^{-m-1}
 \le m!(4K)^m .
 \end{aligned}
\]
The case \(m=0\) is normalization. \(\square\)

The loss 4 is deliberately loose. To use EW.1 afterward, choose the primitive coefficient small enough that \(4K\epsilon<1/2\). All constants remain independent of old rank. If the same comparison is established for every actual exterior with the same local datum, the transferred bound is uniform for that local reference. This lemma does not construct the reference or its raw-supported comparison, and it supplies no microscopic marked estimate.
