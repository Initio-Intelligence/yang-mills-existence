# Joint-distribution hierarchy and connected-shell assembly

**Annex U.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

This note closes two **interface statements**, not the actual interacting
Schwinger-hierarchy estimate.

- **S-01 — proved abstract theorem:** connected distributions with a fixed
  linear Schwartz order and a fixed factorial exponent give full
  distributions on arbitrary joint coincidence-flat tests with the **same**
  order and exponent. The construction is independent of extensions across
  coincidence diagonals. The converse Möbius transformation, a quantitative
  stability estimate, and weak sequential continuity have the same property.
- **S-02 — proved conditional assembly theorem:** an exact connected-shell
  representation, a summable physical tree-kernel majorant, a terminal
  estimate, and a separately normalized one-point function give the full
  OS growth bound and a uniform ultraviolet-tail estimate. They also give
  convergence of the full hierarchy once the finitely resolved connected
  shells and the terminal terms converge.

The S-02 shell majorant and exact representation have **not** been proved for
the complete normalized Wilson/RG histories. Thus S-02 is a completed
implication whose principal Yang--Mills premises remain open. It is not
a completed actual-model S0 estimate.

The derivations below use standard Hahn--Banach extension and finite
regular measure representation of bounded functionals on \(C_0\). Their
use is made explicit, including the norm budgets; no unquantified
nuclearity argument or assertion about tensor-product tests is inserted.

### 1. Test spaces and the statement boundary

For \(m\geq1\), put
\[
X_m=(\mathbb R^4)^m,\qquad
\Delta_m=\bigcup_{1\leq i<j\leq m}\{x_i=x_j\}.
\tag{S.1}
\]
Let \(\mathcal S_0(X_m)\) be the closed subspace of Schwartz functions
whose derivatives of every order vanish on \(\Delta_m\). Set
\(\mathcal S_0(X_1)=\mathcal S(\mathbb R^4)\). The required seminorm is
\[
\nu_r(F)
=\max_{|\alpha|\leq r}\sup_{X\in X_m}
 (1+|X|^2)^{r/2}|\partial^\alpha F(X)|,
\qquad r\in\mathbb N_0.
\tag{S.2}
\]
All weights use the ordinary Euclidean norm on all \(4m\) coordinates.
The space dimension is allowed to grow with \(m\); the estimates below
record that growth rather than holding dimension artificially fixed.

A component-label tuple from a fixed finite field family is understood
in every distribution. The estimates are componentwise and uniform in
those labels. Summing the labels changes only an exponential-in-\(m\)
constant.

For a functional \(T\) on \(\mathcal S_0(X_m)\), write
\[
\|T\|_{r,*}
=\sup_{F\in\mathcal S_0(X_m),\,F\ne0}
 \frac{|T(F)|}{\nu_r(F)}.
\tag{S.3}
\]
A bound in this norm is stronger than merely having an unspecified
Schwartz-continuity bound at each fixed order.

If \(\pi\) is a partition of \(\{1,\ldots,m\}\), denote its coordinate
blocks by \(B\). A joint function flat on every diagonal internal to
each \(B\) belongs to a larger space \(\mathcal S_\pi\).
In particular,
\[
\mathcal S_0(X_m)\subset\mathcal S_\pi.
\tag{S.4}
\]
Cross-block flatness will not be needed to define a block tensor product.

### 2. An explicit tensor-product construction with no order loss

#### Lemma 2.1 — a bounded measure representation

Let \(T\) be a functional on \(\mathcal S_0(\mathbb R^d)\) obeying
\[
|T(f)|\leq B\,\nu_r(f)
\tag{S.5}
\]
for an integer \(r\geq0\). Here the notation \(\mathcal S_0\) can mean
any fixed closed subspace of Schwartz space, including the internal
coincidence-flat space for one coordinate block. There exist finite
complex measures \(\mu_\alpha\), \(|\alpha|\leq r\), such that
\[
\widetilde T(f)
=\sum_{|\alpha|\leq r}
 \int_{\mathbb R^d}
 (1+|x|^2)^{r/2}\partial^\alpha f(x)\,d\mu_\alpha(x),
\tag{S.6}
\]
defines a tempered-distribution extension of \(T\), and
\[
\sum_{|\alpha|\leq r}\|\mu_\alpha\|_{\mathrm{TV}}\leq B.
\tag{S.7}
\]
In particular, no factor equal to the number of derivatives occurs.

**Proof.**
Let \(I_r=\{\alpha:|\alpha|\leq r\}\), and map \(f\) into
\[
J_r f(x,\alpha)
=(1+|x|^2)^{r/2}\partial^\alpha f(x)
\]
in \(C_0(\mathbb R^d\times I_r)\), with its supremum norm.
Schwartz decay makes every component vanish at infinity, and
\(\|J_rf\|_\infty=\nu_r(f)\).
The \(\alpha=0\) component makes this map injective. Thus
\(J_rf\mapsto T(f)\) is a bounded functional of norm at most \(B\)
on the image of the stated test subspace.

Hahn--Banach extends it to \(C_0(\mathbb R^d\times I_r)\) with the same
norm. Its finite complex measure has total variation at most \(B\).
Restricting that measure to the finitely many copies indexed by
\(\alpha\) gives (S.6)--(S.7). For an arbitrary Schwartz function the
right side is absolutely convergent and bounded by \(B\nu_r(f)\),
so it is a tempered distribution extending \(T\). \(\square\)

The choice of extension need not be unique. The next lemma proves
that its relevant tensor products on flat tests are unique.

#### Lemma 2.2 — joint-test tensor estimate and extension independence

For the blocks \(B\in\pi\), let \(T_B\) be defined on the internal
coincidence-flat Schwartz space of its variables, and suppose
\[
|T_B(f)|\leq b_B\nu_{r_B}(f),\qquad r_B\in\mathbb N_0.
\tag{S.8}
\]
For every \(F\in\mathcal S_\pi\), the block product
\[
\left(\bigotimes_{B\in\pi}T_B\right)(F)
\tag{S.9}
\]
is well-defined, independent of the extensions in Lemma 2.1, and satisfies
\[
\boxed{
\left|
\left(\bigotimes_{B\in\pi}T_B\right)(F)
\right|
\leq
\left(\prod_{B\in\pi}b_B\right)
\nu_{\sum_B r_B}(F).
}
\tag{S.10}
\]
It is associative, covariant under permutations of coordinate blocks,
and multilinear in the \(T_B\)'s.

**Proof.**
Choose the measure representations (S.6) for every block. Define (S.9)
by the finite sum of the integrals
\[
\int
\left[\prod_{B\in\pi}(1+|x_B|^2)^{r_B/2}\right]
\left[\prod_{B\in\pi}\partial_{x_B}^{\alpha_B}\right]F(X)
\prod_{B\in\pi}d\mu_{B,\alpha_B}(x_B).
\tag{S.11}
\]
The order of the derivative is at most \(\sum_Br_B\), while
\[
\prod_{B\in\pi}(1+|x_B|^2)^{r_B/2}
\leq
(1+|X|^2)^{(\sum_Br_B)/2}.
\tag{S.12}
\]
Consequently the integrand in (S.11) is bounded by
\(\nu_{\sum_Br_B}(F)\). Summing the products of measure variations
and using (S.7) gives (S.10). This also proves the absolute
integrability required to change the integration order.

Now change the extension of one block \(B_0\). Hold the other block
coordinates fixed, as well as their derivatives in (S.11).
The resulting function of \(x_{B_0}\) is Schwartz and flat on all its
internal coincidence diagonals: derivatives in other coordinates
preserve that property. The difference of the two extensions is zero
on that function. Integrating first over \(x_{B_0}\), and then over
the other variables, gives zero. Repeating this for each block proves
independence. Absolute convergence and ordinary product measures give
associativity, permutation covariance and multilinearity. \(\square\)

This is a construction for an arbitrary **joint** \(F\). It is not an
estimate first stated only for a simple tensor and then promoted without
proof to the joint test space. It also works when the connected
distributions are supplied only on \(\mathcal S_0\); there is no
requirement that a chosen extension across diagonals be physically
preferred.

### 3. S-01: connected and full hierarchies have the same OS budget

#### Theorem 3.1 — quantitative partition and Möbius passage

Let \(q\in\mathbb N_0\), \(p\geq1\), and \(A\geq1\). For every
\(k\geq1\), suppose the connected distribution \(T_k\) is defined on
\(\mathcal S_0(X_k)\) and
\[
|T_k(f)|\leq A^{k+1}(k!)^p\nu_{qk}(f).
\tag{S.13}
\]
Define \(S_0=1\), and on \(\mathcal S_0(X_m)\) set
\[
S_m
=\sum_{\pi\in\Pi_m}
 \bigotimes_{B\in\pi}T_{|B|}.
\tag{S.14}
\]
The coordinate and field labels in each block are the inherited ones.
Then (S.14) is well-defined, independent of every diagonal extension,
and
\[
\boxed{
|S_m(F)|
\leq C^{m+1}(m!)^p\nu_{qm}(F).
}
\tag{S.15}
\]
One can take \(C=2A^2\). There is **no increase in \(q\) or \(p\)**.

Conversely, if full distributions \(S_k\) have a bound of the form
(S.13), then
\[
T_m
=\sum_{\pi\in\Pi_m}
 (-1)^{|\pi|-1}(|\pi|-1)!
 \bigotimes_{B\in\pi}S_{|B|}
\tag{S.16}
\]
has the same type of bound, with the same \(q,p\) and a changed
exponential constant. The two operations are inverses on the flat
test spaces.

**Proof.**
Lemma 2.2 applies to each partition with \(r_B=q|B|\), so its total
order is exactly \(qm\). Its contribution is bounded by
\[
A^{m+|\pi|}
\prod_{B\in\pi}(|B|!)^p\,\nu_{qm}(F).
\tag{S.17}
\]
Since \(A\geq1\) and \(|\pi|\leq m\), the power of \(A\) is at most
\(A^{2m}\).

For \(p\geq1\),
\[
\prod_{B\in\pi}(|B|!)^p
\leq (m!)^{p-1}\prod_{B\in\pi}|B|!.
\tag{S.18}
\]
Ordering \(r\) blocks and summing over their positive sizes gives
\[
\sum_{\substack{\pi\in\Pi_m\\|\pi|=r}}
 \prod_{B\in\pi}|B|!
=\frac{m!}{r!}\binom{m-1}{r-1}.
\tag{S.19}
\]
Thus
\[
\sum_{\pi\in\Pi_m}\prod_{B\in\pi}(|B|!)^p
\leq 2^{m-1}(m!)^p.
\tag{S.20}
\]
Equations (S.17)--(S.20) prove (S.15).

For the inverse formula, the extra Möbius coefficient gives
\[
\begin{aligned}
\sum_{\pi\in\Pi_m}(|\pi|-1)!
 \prod_{B\in\pi}(|B|!)^p
&\leq
(m!)^p\sum_{r=1}^{m}\frac1r\binom{m-1}{r-1}\\
&=(m!)^p\frac{2^m-1}{m}
\leq 2^m(m!)^p.
\end{aligned}
\tag{S.21}
\]
Lemma 2.2 gives the same test order. Finally, multilinearity and
associativity make the usual finite partition cancellation proving
the moment--cumulant inversion valid here. Each computation involves
only finitely many partitions at a fixed \(m\); no exponential-source
series is assumed to converge. \(\square\)

If a starting estimate has \(0\leq p<1\), it may first be enlarged to
\(p=1\). No assertion of preserving an exponent less than one is
needed for the OS application.

#### Corollary 3.2 — quantitative stability and contact invariance

Suppose \(T_k,\widehat T_k\) satisfy (S.13) with the same \(A,q,p\),
and, for a number \(\varepsilon\geq0\),
\[
\|(T_k-\widehat T_k)\|_{qk,*}
\leq\varepsilon A^{k+1}(k!)^p,\qquad k\geq1.
\tag{S.22}
\]
Their full hierarchies satisfy
\[
\boxed{
|(S_m-\widehat S_m)(F)|
\leq\varepsilon C^{m+1}(m!)^p\nu_{qm}(F),
}
\tag{S.23}
\]
with \(C\) independent of \(m,\varepsilon\).
The analogous statement holds for the inverse Möbius operation.

**Proof.**
Telescope a product over the blocks of one partition. There are
\(|\pi|\leq m\) changed-factor terms, each with the same product
budget as (S.17) and the extra factor \(\varepsilon\).
Multiply (S.20) by \(m\) and absorb \(m\leq2^m\) into \(C^{m+1}\).
For the inverse operation the product-telescope factor changes
\((|\pi|-1)!\) to \(|\pi|!\); (S.19) then gives the bound
\((m!)^p2^{m-1}\) directly. \(\square\)

If two connected extensions differ only by distributions annihilating
the flat test spaces, their restricted \(T_k\)'s coincide. Their full
restrictions therefore coincide as well. In particular, finite-order
partial-diagonal contact changes do not create a hidden separated
ambiguity through the partition operation. This does not choose or
bound a contact extension on non-flat tests.

#### Proposition 3.3 — weak sequential continuity on the flat spaces

Let \(T_{k,n}\) satisfy a common bound (S.13), and suppose
\[
T_{k,n}(f)\longrightarrow T_k(f)
\quad\text{for every }k,\ f\in\mathcal S_0(X_k).
\tag{S.24}
\]
Then their full hierarchies satisfy
\[
S_{m,n}(F)\longrightarrow S_m(F)
\quad\text{for every }m,\ F\in\mathcal S_0(X_m),
\tag{S.25}
\]
where \(S\) is formed from the limits by (S.14).
The same assertion holds for the inverse Möbius transformation.

**Proof.**
Fix \(m,F\), and any subsequence of \(n\). For the finitely many
orders and component tuples needed by the partitions of
\(\{1,\ldots,m\}\), choose the measure extensions in Lemma 2.1.
Their variations have uniform bounds.

For completeness, their needed compactness follows by diagonal
extraction of integrals against a countable dense subset of each
\(C_0(\mathbb R^{4k}\times I_{qk})\). The common norm bound extends the
limit to all of \(C_0\); measure representation gives a finite measure
limit with no larger variation. A further subsequence therefore has
simultaneous weak-star measure limits for these finitely many blocks.
Each limit represents an extension of \(T_k\), by (S.24).

For fixed multi-indices, the weighted derivative of \(F\) in (S.11)
belongs to \(C_0\) on the product coordinate space. Products of the
bounded measures converge against that function: on a large compact
box approximate a continuous function uniformly by finite sums of
products of one-block \(C_0\) functions, and then use its vanishing
at infinity and the common variation bounds to control the rest.
Such finite-sum approximation can be made directly with a finite
rectangular partition of unity.

It follows that along this further subsequence every term of (S.14)
converges to the product of the limiting extensions. Lemma 2.2 makes
that answer independent of which extensions or further subsequence
were selected. Every subsequence thus has a further subsequence with
the same numerical limit \(S_m(F)\), proving (S.25).
The finite sum (S.16) is handled identically. \(\square\)

The proposition supplies the continuity that cannot be obtained by
merely invoking pointwise convergence on simple tensor tests.

### 4. S-02: connected shells and a terminal law assemble the hierarchy

#### 4.1 Precise premises

Set the fixed physical stopping scale to one. Let
\[
h_j=L^{-j},\qquad L>1,\qquad K_n\longrightarrow\infty,
\qquad 0<a_n\leq h_{K_n}.
\tag{S.26}
\]
All torus tests use a nonwrapping interior embedding as in Annex E.
Equivalently, the assumptions below may be made on the ordinary
Euclidean grid \(a_n\mathbb Z^4\), with compactly supported embedding
weights bounded by one. The metric in the tree bound below is the
ordinary physical Euclidean metric on the relevant supports, not an
unjustified replacement of periodic distance.

Assume an actual compatible cutoff hierarchy has connected
distributions \(C_{m,n}\). For \(m\geq2\), require the exact identity
on \(\mathcal S_0(X_m)\)
\[
C_{m,n}
=C^{\mathrm{ter}}_{m,n}
+\sum_{j=0}^{K_n}T_{m,n,j}.
\tag{S.27}
\]
Identity (S.27) must be established for the **same** initial
renormalized fields and normalized full law. It is not licensed by
having a useful native kernel at each scale.

The following are quantitative inputs, uniform in \(m,n,j\) and the
field-label tuple:

1. **One-point normalization.** For fixed \(A_1,q_1\),
   \[
   |C_{1,n}(f)|\leq A_1^2\nu_{q_1}(f).
   \tag{S.28}
   \]
   This can include an exact zero normalization, but no subtraction is
   supplied by this theorem.
2. **Terminal connected bound.** For fixed \(A_T\geq1\),
   \(p_T\geq0\), \(q_T\in\mathbb N_0\),
   \[
   |C^{\mathrm{ter}}_{m,n}(F)|
   \leq A_T^{m+1}(m!)^{p_T}\nu_{q_Tm}(F).
   \tag{S.29}
   \]
3. **Physical connected-shell majorant.** The shell distribution is
   the actual sum or integral of a kernel satisfying
   \[
   |t_{m,n,j}(X)|
   \leq
   A_0^{m+1}(m!)^{p_0}h_j^{-4m}w_j
   \exp\!\left[-\frac{c\,\tau(X)}{(m+d_0)h_j}\right],
   \tag{S.30}
   \]
   where \(p_0\geq0\), \(c>0\), \(d_0\geq0\) are fixed,
   and \(\tau(X)\) is the minimum spanning-tree length. The fixed
   nonnegative sequence \(w_j\) satisfies
   \[
   W=\sum_{j\geq0}h_jw_j<\infty.
   \tag{S.31}
   \]
   On the fine grid, the distribution includes the measure factor
   \(a_n^{4m}\); the kernel is not a distributional delta function
   with its measure factor omitted.

Exact point contacts may be included in (S.27), since they vanish
on the stated test space. Nonzero-width contact remainders require
their own quantitative norm bound; they cannot be dropped by naming
them local.

#### Lemma 4.1 — the shell norm

Premise (S.30) implies
\[
\boxed{
\|T_{m,n,j}\|_{6m,*}
\leq
A_2^{m+1}(m!)^{p_0+5}h_jw_j,
\qquad m\geq2.
}
\tag{S.32}
\]
The constant is independent of \(a_n,h_j,m,n\).

**Proof and prior-result attribution.**
This is the physical shell lemma already proved in Annex N,
Proposition 8.1, with its initial factorial exponent \(2\) replaced
by \(p_0\). Its proof gives precisely an additional factorial power
five.


For \(r_i=X_i-X_1\), flatness at the full diagonal and fifth-order
Taylor remainder give
\[
|F(X)|
\leq C\left(\sum_{i=2}^{m}|r_i|_1\right)^5
(1+|X_1|^2)^{-3}\nu_{6m}(F).
\tag{S.33}
\]
The intermediate points retain \(X_1\), so the stated weight holds.
Every \(r_i\) is a path displacement in a minimum tree; their
total norm is at most \(C(m-1)\tau(X)\).
Absorb the fifth power of \(\tau\) into half the exponential in
(S.30). This costs \(C(m+d_0)^5h_j^5\), besides the preceding
factor \(C(m-1)^5\).

The remaining minimum-tree exponential is bounded by the sum over
the \(m^{m-2}\) labeled trees. For each tree, successive leaf sums
or integrals cost
\[
\left[C(m+d_0)^4h_j^4\right]^{m-1};
\]
the lattice estimate is uniform because \(a_n\leq h_j\).
The remaining weighted root sum or integral is bounded by a fixed
constant. The physical powers multiply to
\[
h_j^{-4m}h_j^5h_j^{4(m-1)}=h_j.
\tag{S.34}
\]
The tree count and the range factors are bounded by
\(C^{m+1}(m!)^5\); the extra fixed powers of \(m\) are absorbed
in the exponential constant. This proves (S.32).
No new analytic shell estimate beyond the cited prior lemma is
claimed here. \(\square\)

#### Theorem 4.2 — full OS budget and a uniform shell tail

Under (S.26)--(S.31), set
\[
q=\max\{6,q_1,q_T\},\qquad
p=\max\{1,p_T,p_0+5\}.
\tag{S.35}
\]
Then the actual full hierarchy obeys
\[
\boxed{
|S_{m,n}(F)|
\leq C^{m+1}(m!)^p\nu_{qm}(F)
}
\tag{S.36}
\]
uniformly in \(n,m\). In particular, for \(p_0=2\),
\(q_T,q_1\leq6\), and \(p_T\leq7\), the output is
\[
(q,p)=(6,7).
\tag{S.37}
\]

For \(J\geq0\), form an auxiliary connected hierarchy by keeping
the same one-point and terminal terms and only the shells with
\(j\leq\min(J,K_n)\). Let \(S^{\leq J}_{m,n}\) be its full
partition hierarchy. Then
\[
\boxed{
|(S_{m,n}-S^{\leq J}_{m,n})(F)|
\leq
W(J)\,C^{m+1}(m!)^p\nu_{qm}(F),
\quad
W(J)=\sum_{j>J}h_jw_j\longrightarrow0.
}
\tag{S.38}
\]
No positivity assertion is made for the auxiliary truncated
hierarchy.

**Proof.**
Summing (S.32) in (S.27), adding (S.29), and using (S.28) for
order one gives
\[
|C_{m,n}(F)|
\leq A^{m+1}(m!)^p\nu_{qm}(F)
\]
for one fixed \(A\). Monotonicity of the seminorm in its integer
index justifies using the common \(q\). The factor \(W\) is
absorbed in \(A^{m+1}\).
Theorem 3.1 gives (S.36) for joint tests.

Both the full and truncated connected hierarchies have the same
uniform budget. Their difference is bounded by (S.32) summed over
\(j>J\), with the factor \(W(J)\). Apply Corollary 3.2 to get
(S.38). Compatibility with the given cutoff full moments follows
from the exact connected identity and the ordinary finite
moment--cumulant identity at that cutoff; Lemma 2.2 supplies its
joint-test meaning on \(\mathcal S_0\). \(\square\)

#### Theorem 4.3 — dominated cofinal passage for the full hierarchy

In addition, suppose for every fixed \(m,j\) and every flat joint
test the shell distributions \(T_{m,n,j}\) converge as \(n\to\infty\)
once \(K_n\geq j\). Suppose the terminal distributions and the
one-point distributions also converge on their stated test spaces.
Then
\[
C_m
=C_m^{\mathrm{ter}}+\sum_{j\geq0}T_{m,j},\qquad m\geq2,
\tag{S.39}
\]
is a well-defined distributional sum with the same connected
budget, and
\[
S_{m,n}(F)\longrightarrow
\sum_{\pi\in\Pi_m}
\left(\bigotimes_{B\in\pi}C_{|B|}\right)(F).
\tag{S.40}
\]
The output obeys (S.36).

**Proof.**
For a fixed finite \(J\), use the assumed convergence of its
finitely many shells and the terminal term. The tail of the
connected sum is bounded uniformly by \(W(J)\) times the fixed
order's seminorm budget, so it tends to zero independently of
\(n\). This proves connected convergence to (S.39).
Proposition 3.3 gives full convergence. Alternatively, (S.38)
first removes the full-hierarchy tail uniformly and Proposition
3.3 applies to the finitely resolved connected sum. \(\square\)

If those resolved-shell limits have not been shown, the common
bound still supports the previously proved cofinal compactness
argument. No uniqueness of the resulting subsequence follows from
the present theorem.

### 5. How these two results differ from the earlier annexes

| Earlier result | What was already proved | What is added here |
|---|---|---|
| Annex N, Lemma 6.1 and Theorem 6.2 | The partition factorial budget and a full-moment expansion for the specified native point kernels | S-01 starts with general connected **distributions on the flat test spaces**, constructs their products on arbitrary joint tests, proves extension independence, preserves the exact \(q,p\), and proves stability and weak continuity |
| Annex N, Proposition 7.1 | Direct joint-test summation for an actual fixed-shell kernel, retaining its ultraviolet factor | S-01 no longer requires a pointwise kernel or uses a tensor-test bound as a substitute |
| Annex N, Proposition 8.1 | The physical full-diagonal shell estimate and its summable \(h_j\) gain | S-02 uses that lemma as an explicit input; it supplies the terminal-plus-shell-to-**full** distribution construction, the full-hierarchy tail estimate, and dominated cofinal passage |
| Annex E and Annex O | Exact contact algebra and a one-layer microscopic contact error | No all-scale matching or new contact-support result is claimed in S-01/S-02 |
| Earlier compactness theorem | A uniformly bounded full hierarchy has a subsequential continuum limit | S-02 supplies a sufficient distribution-level input interface with explicit \(q,p\), without claiming its Wilson premises |

The shell lemma and partition counting of Annex N are not new here.
The new content is the general joint distribution passage and its
complete conditional assembly interface.


---
