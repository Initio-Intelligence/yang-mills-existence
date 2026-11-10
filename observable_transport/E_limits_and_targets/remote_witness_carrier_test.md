# A remote energy witness does not pay a local history contrast

This is a representation-independent test for the M-03 norm. It is a proved conditional criterion, not a claim that the particular transported microscopic Yang–Mills scalar satisfies its lower-bound hypothesis.

## 1. The distinction needed by the residual argument

The matched residual trial mass gives a normalized old-energy bound of order \(1+P(g)^2\). Proposition AH.1 pays this by an actual fresh curvature witness somewhere on the complete residual test footprint. The prepared integration core \(D_0\), however, has bounded current diameter, while that witness can be a distance of order \(R(g)\) away. The source realization in [M04 Residual Strata Analysis](../A_support_and_normalization/M04_Residual_Strata_Analysis.md), Sections 4–8, admits this separation.

There is no implication

\[
 \nu_{r,v}(E_{\rm old})\le C[1+E_{Y}\(v\)]
 \quad\Longrightarrow\quad
 \nu_{r,v}(E_{\rm old})\le C[1+E_{D_0}\(v\)].
 \tag{RW.1}
\]

The loss in the second assertion matters even after the retained geometric label has been made local. Conversely, a large old-energy upper bound does not prove a large physical-scalar lower bound. The actual normalized old history sum includes physical and gauge-type births; a native scalar of the current old field is not automatically the already transported microscopic scalar. The test below keeps these distinctions explicit.

## 2. A norm lower bound from one exact discrete contrast

Let \(h'\) be the output scale, \(o\) an insertion anchor, and \((A_a,B_a,J_a)\) any compatible M-03 carrier representation of one scalar output. The carriers \(X_a\) include \(o\) and every actual dependency footprint. Tags remain distinct. Let \(v'\) be obtained from \(v\) by one permitted discrete history replacement, with denominator one. Suppose the scalar reference field \(\varphi_{h'}\) has the same value at these two data. A fixed identity term also has the same value.

For each tag write its pointwise current budget, in the exact M-03 normalization, as

\[
 n_a=h'^4 w_\kappa\(X_a\)\,c_{3/2}
       \sup_x\frac{B_a^{\natural}(x)+J_a^{\natural}(x)}
                         {\widehat R_{h',X_a}(x)^{3/2}},
 \qquad c_{3/2}=(3/2)^{-3/2}.
 \tag{RW.2}
\]

The full M-03 norm is at least \(\sum_a n_a\). If the direction is outside the true dependency footprint of a tag, that tag's contrast is zero. If it is inside, compatibility and the definition of the summed envelope give

\[
 |A_a\(v'\)-A_a\(v\)|
 \le c_{3/2}^{-1}h'^{-4}n_a
       \frac{\widehat R_{h',X_a}\(v\)^{3/2}}{w_\kappa\(X_a\)}.
 \tag{RW.3}
\]

This statement uses the actual shifted regulator, including the particular discrete replacement. It does not assume that a label change preserves that regulator.

### Theorem RW.1

Suppose there are numbers \(r>0\), \(K_0,K_1\ge1\), for which the two endpoint data satisfy

\[
 \widehat R_{h',X}\(v\)\le K_0
       \quad\text{for every possible nonzero carrier }X\subset B_r\(o\),
 \qquad
 \widehat R_{h',X}\(v\)\le K_1\quad\text{for all }X.
 \tag{RW.4}
\]

Here \(B_r\(o\)\) is the current-block graph ball. Then every such representation obeys

\[
 \|\mathbf A\|_{h',\kappa}
 \ge
 \frac{c_{3/2} h'^4 |A\(v'\)-A\(v\)|}
      {\max\{K_0^{3/2},K_1^{3/2}e^{-\kappa r}\}}.
 \tag{RW.5}
\]

The same lower bound applies to the remainder after subtracting any fixed scalar multiple of \(\varphi_{h'}\) and any field-independent identity coefficient.

**Proof.** A carrier contained in \(B_r\(o\)\) has the quotient on the right of (RW.3) at most \(K_0^{3/2}\), since \(w_\kappa\ge1\). A carrier leaving that ball contains the anchor and a point of graph distance at least \(r\). Its shortest connecting subgraph therefore has at least \(r\) edges. The exact M-03 weight gives \(w_\kappa\(X\)\ge e^{\kappa r}\), even if \(X\) was not originally declared connected. Thus its quotient is at most \(K_1^{3/2}e^{-\kappa r}\). Sum (RW.3) over the actual distinct tags and use absolute convergence supplied by a finite norm. This proves (RW.5). If the norm is infinite, the inequality is automatic. The scalar and identity have zero contrast by hypothesis, so the argument is unchanged after their subtraction. \(\square\)

No cancellation between activities has been used to estimate the norm from above. The triangle inequality is used only in the permissible direction that lower-bounds every representation of the same exact contrast. A global footprint for the history coordinate makes the bound stronger, because then every nonzero carrier already pays that footprint.

## 3. The remote-witness regime

Suppose a family of such endpoint pairs has \(K_0\le C\), \(K_1\le C\(1+P(g)^2\)\), and \(r\ge cR(g)\to\infty\). If \(P(g)\) is a fixed power of \(\log g^{-1}\) and \(R(g)\) is a positive power of that logarithm, then

\[
 K_1^{3/2}e^{-\kappa r}\longrightarrow0.
 \tag{RW.6}
\]

Consequently a contrast

\[
 h'^4|A\(v'\)-A\(v\)|\ge a(g)
 \tag{RW.7}
\]

forces \(\|\mathbf A\|_{h',\kappa}\ge c\,a(g)\). In particular, if \(a(g)\to\infty\) while the specified one-step input budget stays bounded, the uniform M-04 remainder bound cannot hold for that input and that actual output convention.

A single normalized link perturbation at a completely flat current field excites only a fixed number of current plaquettes, with uniformly bounded dimensionless energy. This can supply \(K_0=O(1)\) in a fresh-field-only neighborhood. It must be checked on the actual padded native list: a retained old free coordinate or an inherited plaquette would change (RW.4). Likewise, the coarse energy of the remote pulse and every permitted shift must be included when verifying \(K_1\).

## 4. What must still be proved for the actual M-04 scalar

The source constructions currently verify that a residual witness may be remote from the prepared core. They do not yet verify all of the following together:

1. Two positive actual output states related by the chosen allowed label replacement, with the same nearby continuous data and the bounds (RW.4). An arbitrary artificial inactive label is insufficient.
2. A growing contrast (RW.7) for the **actual already transported microscopic scalar**, under the full old posterior. It must include the previously integrated annuli, all old histories and cross terms, and the fixed input centering.
3. An explicit bounded one-step input budget for that same scalar family. A large output alone does not refute an estimate whose legitimate incoming budget is already larger.

The pure-gauge birth of NR20.4 prevents a deterministic inference from a retained bad component to a large physical Wilson energy. Even if physical births dominate asymptotically, that would require a comparison of their actual posterior masses and the associated scalar transport; it is not supplied by the trial lower bound. Conversely, an upper bound \(O(P^2)\) cannot be read as a matching lower bound.

Thus RW.1 is a useful rigorous test of any proposed bounded-core proof. It explains why a remote native energy witness cannot simply be moved to a core regulator. It is not a counterexample to M-04, and it does not change the stated norm or the M-04 statement.
