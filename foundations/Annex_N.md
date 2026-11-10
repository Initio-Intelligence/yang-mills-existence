# All-order Gaussian coefficient removal and joint-test budgets

**Annex N.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Result and exact scope

This note removes the restriction \(m\leq6\) from the native Wick comparison. The new bound has a **fixed factorial exponent two**, with constants uniform in the source order, volume and admitted Gaussian cutoff. Its cutoff error is \(e^{-cP^2}\), without a factor \(P^{2m+6}\). That factor is absorbed into the Gaussian tail with its entire order cost recorded in \((m!)^2\).

The main statement is

\[
\boxed{
\begin{aligned}
K_m^P(g)
&=L_m^\infty+\frac{g^2}{2}C_{2,m}^\infty+\mathcal E_m(g,P),
\\
|\mathcal E_m(g,P)|
&\leq C^{m+1}(m!)^2h^{-4m}
\bigl(|g|^4+e^{-cP^2}\bigr)
\exp\!\left[-\frac{\gamma\tau(x_1,\ldots,x_m)}{8(m+4)}\right],
\qquad m\geq1 .
\end{aligned}}
\tag{T.1}
\]

The law is exactly the fixed homogeneous no-R, identity-background native integral of the parity theorem. Its inherited regular action, constrained physical chart and cutoff are frozen during the signed computational coupling interpolation. Its leading and second coefficients are the ordinary finite-volume Gaussian Wick coefficients of its actual constrained precision. No microscopic-transport identification or complete-history estimate is added by (T.1).

The note also proves:

1. the corresponding full-moment expansion, with the same fixed factorial exponent;
2. a genuine joint Schwartz-test estimate, of order \(6m\), at each fixed physical shell scale \(h\);
3. a full-diagonal ultraviolet summation lemma with explicit \((q,p)=(6,7)\), whenever the stated physical shell-kernel majorant is available.

The factor \(h^{-4m}\) in the unsummed fixed-shell estimate is retained. The third statement handles localized connected shell kernels on coincidence-flat tests; it does not identify the full Wilson connected hierarchy with a sum of those native kernels. Exact matching, retained-data cumulants, generated collision vertices, history control, rotations, operator bounds and phase hypotheses remain separate.

Status: **P** means the displayed assertion is proved from the stated inputs. The native application uses the scoped regular-law results already proved.

### 1. Inputs retained

Let \(\mathcal I\) be the finite current coordinate lattice, with a metric satisfying

\[
\sup_x\sum_{y\in\mathcal I}e^{-a d(x,y)}
\leq C(1+a^{-4}),\qquad 0<a\leq1,
\tag{T.2}
\]

uniformly over the admitted volumes. Coordinate-block dimensions are bounded by a fixed \(d_*\).

For the centered Gaussian precision \(H\), retain

\[
H\geq\lambda I,\qquad H_{ii}\leq\Lambda I,\qquad
A_H=\sup_i\sum_j\int_0^\infty
\|(e^{-tH})_{ij}\|_{\mathrm{op}}\,dt\leq A .
\tag{T.3}
\]

The two Gaussian laws are

\[
\nu_\infty(dz)=Z_\infty^{-1}e^{-zHz/2}\,dz,\qquad
\nu_P=\nu_\infty\!\left(\,\cdot\,\middle|\,
\prod_i\{|z_i|\leq P\}\right),\qquad P\geq1 .
\tag{T.4}
\]

For the native precision, the Wick supplement derives the semigroup bound in (T.3) from the uniform gap and exponential matrix locality. It also verifies the weighted real covariance estimate under both laws. These are retained inputs, not conclusions of a gap alone.

The Gaussian cutoff theorem gives

\[
|\nu_P(f)-\nu_\infty(f)|
\leq C A_H P^{d_*-1}e^{-\lambda P^2/2}
\sum_i\operatorname{Lip}_i(f)
\tag{T.5}
\]

for bounded blockwise Lipschitz \(f\). It proves a uniform one-block Gaussian density bound under \(\nu_P\), so that

\[
\sup_{i,P}\|z_i\|_{L^p(\nu_P)}
+\sup_i\|z_i\|_{L^p(\nu_\infty)}
\leq C\sqrt p,\qquad p\geq1 .
\tag{T.6}
\]

The proof of (T.5) is the normalized boundary-flux/OU-divergence proof in the Gaussian cutoff theorem. In particular, no division by the probability of the entire cutoff event is used here.

For a polynomial \(Q\) in scalar coordinates, use the displayed coefficient representation

\[
Q(z)=\sum_{d=0}^{D}\sum_{a_1,\ldots,a_d}
c^{(d)}_{a_1\cdots a_d}z_{a_1}\cdots z_{a_d},
\qquad
\|Q\|_1=\sum_{d,a_1,\ldots,a_d}|c^{(d)}_{a_1\cdots a_d}|.
\tag{T.7}
\]

For one anchored at \(x\), also use

\[
\|Q_x\|_{\theta,1}
=\sum_{d,a_1,\ldots,a_d}
|c^{(d)}_{a_1\cdots a_d}|
e^{\theta\tau(x,j(a_1),\ldots,j(a_d))}.
\tag{T.8}
\]

Here \(j(a)\) is the coordinate block. The degree-zero term has weight one. These norms refer to the chosen representation, and are multiplicative upper bounds under products. No minimization over polynomial representations is needed.

### 2. Quantitative polynomial cutoff removal at arbitrary degree

#### Proposition 2.1 — the degree cost is explicit, P

There are constants \(C\geq1\) and
\(\kappa=d_*/2+1\), depending only on the parameters in (T.3), such that for every polynomial of degree at most \(D\geq1\),

\[
|\nu_\#(Q)|
\leq \|Q\|_1 C^{D+1}(1+D)^{D/2},
\qquad \#\in\{P,\infty\},
\tag{T.9}
\]

and

\[
\boxed{
|\nu_P(Q)-\nu_\infty(Q)|
\leq
\|Q\|_1 C^{D+1}(1+D)^{D/2+\kappa}
e^{-\lambda P^2/8}.}
\tag{T.10}
\]

Both constants are independent of the volume, \(D\), and \(P\). A constant polynomial has zero cutoff error.

**Proof.** For a monomial of degree \(d\), Hölder with exponent \(d\), followed by (T.6), gives

\[
\nu_\#|z_{a_1}\cdots z_{a_d}|
\leq (C\sqrt{\max(1,d)})^d .
\]

Summing coefficients, and enlarging \(C\), proves (T.9).

Let \(\pi_P\) be blockwise radial projection onto the radius-\(P\) balls and set \(Q_P=Q\circ\pi_P\). It agrees with \(Q\) on the constrained domain and satisfies

\[
\sum_i\operatorname{Lip}_i(Q_P)
\leq D\|Q\|_1(1+P)^{D-1}.
\]

Therefore (T.5) bounds the clipped comparison by

\[
|\nu_P(Q)-\nu_\infty(Q_P)|
\leq C A_H D\|Q\|_1
(1+P)^{D+d_*-2}e^{-\lambda P^2/2}.
\tag{T.11}
\]

The crucial all-order step is to absorb the polynomial in \(P\) now, before summing partitions. For every \(s\geq0\),

\[
\sup_{P\geq1}
(1+P)^s e^{-3\lambda P^2/8}
\leq C_\lambda^{s+1}(1+s)^{s/2}.
\tag{T.12}
\]

For example, use \(1+P\leq2P\) and maximize
\(P^s e^{-3\lambda P^2/8}\); the \(s=0\) case is immediate. Replacing the harmless power in (T.11) by \(D+d_*\), and retaining \(e^{-\lambda P^2/8}\), gives

\[
|\nu_P(Q)-\nu_\infty(Q_P)|
\leq
\|Q\|_1 C^{D+1}(1+D)^{D/2+d_*/2+1}
e^{-\lambda P^2/8}.
\tag{T.13}
\]

For the remaining full-Gaussian projection tail, telescope a degree-\(d\) monomial across its \(d\) coordinate occurrences. Radial projection decreases the absolute value of each scalar coordinate, so each term is bounded by

\[
\prod_{\ell=1}^{d}|z_{a_\ell}|\,
\mathbf1_{\{|z_{i_r}|>P\}}
\]

for one occurrence \(r\). The Gaussian block tail is

\[
\mathbb P_{\nu_\infty}(|z_i|>P)
\leq 2^{d_*/2}e^{-\lambda P^2/4}.
\]

Cauchy–Schwarz and Hölder at order \(2d\) consequently give

\[
\nu_\infty|Q-Q_P|
\leq
\|Q\|_1 C^{D+1}(1+D)^{D/2+1}
e^{-\lambda P^2/8}.
\tag{T.14}
\]

Combine (T.13) and (T.14). \(\square\)

The point of (T.10) is that it contains no unrecorded \(C_D\). It remains useful when the total polynomial degree grows linearly with the source order.

For the fixed centrally symmetric convex block templates covered by the Gaussian theorem, the same proof works with \(c>0\) in place of \(\lambda/8\). The constant depends on the specified inradius, outradius and surface-area bounds; scalar-coordinate products in the tail proof are bounded by block-norm products. No moving or nonsymmetric cutoff is included.

### 3. All-order cumulant comparison with a fixed factorial exponent

#### Proposition 3.1 — arbitrary total degree, P

Let \(Q_1,\ldots,Q_N\) have degrees \(d_1,\ldots,d_N\), put
\(D=\sum_i d_i\geq1\), and let \(A_i=\|Q_i\|_1\). Then

\[
\boxed{
|\kappa_{\nu_P}(Q_1,\ldots,Q_N)
-\kappa_{\nu_\infty}(Q_1,\ldots,Q_N)|
\leq
C^{D+N+1}N!(1+D)^{D/2+\kappa}
e^{-\lambda P^2/8}\prod_i A_i .}
\tag{T.15}
\]

The formula includes \(N=1\). If all degrees vanish, the difference is zero.

**Proof.** Write the cumulant as

\[
\kappa_\nu(Q_1,\ldots,Q_N)
=
\sum_{\pi\in\Pi_N}
(-1)^{|\pi|-1}(|\pi|-1)!
\prod_{B\in\pi}
\nu\!\left(\prod_{i\in B}Q_i\right).
\tag{T.16}
\]

For a block \(B\), its product polynomial has degree
\(D_B=\sum_{i\in B}d_i\) and coefficient norm at most
\(\prod_{i\in B}A_i\). Telescope the product of block moments between the two laws. Each term has exactly one moment difference, controlled by (T.10), and ordinary moments controlled by (T.9).

The moment-degree factors obey

\[
\prod_{B\in\pi}(1+D_B)^{D_B/2}
\leq (1+D)^{D/2}.
\]

The extra factor from the changed block is at most
\((1+D)^\kappa\). Constants in all blocks together cost at most
\(C^{D+N+1}\), uniformly in the partition. The number of telescoping terms is \(|\pi|\), so the entire coefficient sum is

\[
\sum_{\pi\in\Pi_N}|\pi|!
\leq N!2^{N-1}.
\tag{T.17}
\]

To see (T.17), an ordered partition can be encoded by a permutation of the labels and a choice of cuts between consecutive labels; allowing all such encodings only overcounts. Absorb \(2^{N-1}\) into \(C^{D+N+1}\). \(\square\)

#### Corollary 3.2 — the almost-quadratic degree budget, P

Fix \(b\geq0\). If

\[
\sum_i d_i\leq 2N+b,
\tag{T.18}
\]

then

\[
\boxed{
|\Delta\kappa_N|
\leq
C_b^{N+1}(N!)^2
e^{-\lambda P^2/8}
\prod_i A_i .}
\tag{T.19}
\]

The exponent two is independent of \(N\).

**Proof.** Under (T.18),

\[
(1+D)^{D/2+\kappa}
\leq C_b^{N+1}N^{N+b/2+\kappa}.
\]

Use \(N^N\leq e^N N!\). The remaining power
\(N^{b/2+\kappa}\) has a fixed exponent and is absorbed into
\(C_b^{N+1}\). Insert this in (T.15). \(\square\)

This is sharper than treating every argument as a degree-four polynomial. That treatment would lose the almost-quadratic total degree and produce an unnecessarily larger factorial exponent.

### 4. Spatial decay and the at-most-two extensive anchors

For this section, retain the weighted real covariance estimate under both Gaussian laws, as verified in the Wick supplement. Fix one \(\theta>0\), and choose \(0<\gamma<\theta\) within that covariance budget.

Suppose \(Q_i\) is anchored at \(u_i\), has degree \(d_i\leq4\), and
\(\|Q_i\|_{\theta,1}\leq A_i\). Equation (T.6), coefficient summation and the weighted first derivative give, for \(p\geq1\),

\[
\|Q_i-\nu_\#Q_i\|_p
\leq C A_i p^{d_i/2},
\qquad
\left\|\|\nabla Q_i\|_{\gamma,u_i}\right\|_p
\leq C A_i p^{(d_i-1)/2}.
\tag{T.20}
\]

Constants are uniform because the individual degrees are at most four. A degree-zero argument contributes no cumulant of order at least two and may be omitted from that case.

#### Lemma 4.1 — uniform two-law tree bound, P

If \(\sum_i d_i\leq2N+2\), then for \(N\geq2\),

\[
\begin{aligned}
&|\kappa_{\nu_P}(Q_1,\ldots,Q_N)|
+|\kappa_{\nu_\infty}(Q_1,\ldots,Q_N)|
\\
&\qquad\leq
C^{N+1}(N!)^2
\exp\!\left[-\frac{\gamma\tau(u_1,\ldots,u_N)}{N-1}\right]
\prod_i A_i .
\end{aligned}
\tag{T.21}
\]

**Proof.** Use the real cut theorem at moment order \(2N\). Its partition coefficient is at most
\((N-1)!2^{N-2}\), and there are at most \(N^2\) crossing gradient pairs. The two gradient factors in (T.20) reduce the total moment power by one. Thus the moment part is at most

\[
C^N\left(\prod_iA_i\right)
N^{(\sum_i d_i)/2-1}
\leq
C^N\left(\prod_iA_i\right)N^N .
\]

Combining the factors and using \(N^N\leq e^N N!\) leaves a fixed polynomial in \(N\) times \(C^N(N!)^2\). Absorb that polynomial into \(C^{N+1}\).

Delete a longest edge of a minimum spanning tree on the anchors. Every crossing edge of the resulting cut has length at least
\(\tau/(N-1)\); the real cut theorem therefore supplies the displayed decay. This is precisely the two-gradient cut argument, with the total degree tracked rather than replaced by four for every mark. \(\square\)

Combining (T.19), with \(b=2\), and (T.21) by
\(\min(a,b)\leq\sqrt{ab}\), gives

\[
\boxed{
|\Delta\kappa_N|
\leq
C^{N+1}(N!)^2 e^{-\lambda P^2/16}
\exp\!\left[-\frac{\gamma\tau(u_1,\ldots,u_N)}{2(N-1)}\right]
\prod_i A_i .
}
\tag{T.22}
\]

For \(N=1\), use (T.19) directly and omit the spatial factor.

#### Lemma 4.2 — fixed-number anchor sums do not change the factorial exponent, P

Retain \(m\geq1\) external anchors \(x_1,\ldots,x_m\) and sum
\(r\in\{0,1,2\}\) additional anchors \(y_1,\ldots,y_r\), with
\(N=m+r\). Suppose all coefficient norms of the additional marks are bounded uniformly in their anchors. Then the bound in (T.22), summed over those \(r\) anchors, is at most

\[
C^{m+1}(m!)^2 e^{-\lambda P^2/16}
\exp\!\left[-\frac{\gamma\tau(x_1,\ldots,x_m)}{8(m+4)}\right]
\prod_{i=1}^{m}A_i ,
\tag{T.23}
\]

with the uniform norms of the at-most-two added marks absorbed into \(C\).

**Proof.** For \(r=0\), the assertion is a weakening of (T.22); the one-argument case has no spatial factor. For \(r\geq1\), put
\(T=\tau(x_1,\ldots,x_m,y_1,\ldots,y_r)\). Doubling a tree walk and shortcutting through the external anchors gives

\[
T\geq\frac12\tau(x_1,\ldots,x_m).
\]

Also \(T\geq d(y_l,x_1)\) for every \(l\), and consequently
\(T\geq r^{-1}\sum_l d(y_l,x_1)\). Split the exponential in (T.22) into two equal factors to obtain

\[
e^{-\gamma T/[2(N-1)]}
\leq
e^{-\gamma\tau(x_1,\ldots,x_m)/[8(N-1)]}
\prod_{l=1}^{r}
e^{-\gamma d(y_l,x_1)/[4r(N-1)]}.
\tag{T.24}
\]

Equation (T.2) bounds the sum of the last product by
\(C_r(1+N^{4r})\). This is a fixed polynomial because \(r\leq2\).
Furthermore,
\[
(N!)^2\leq(m!)^2(m+2)^{2r}.
\]
All polynomial costs are absorbed into \(C^{m+1}\), and the displayed spatial denominator is weakened to \(8(m+4)\). \(\square\)

Summing a labeled-tree bound over all \(N-1\) vertices would introduce an unnecessary additional factorial cost. Here only two extensive vertices are summed, and (T.24) records that fact.

### 5. The all-order native Wick theorem

Keep the fixed shell, frozen inherited action \(E_*\), fixed nonlinear chart and common cutoff of the parity theorem. Its Gaussian coefficient polynomials are

\[
O_{i,r}=\frac{h^{-4}}{(r+1)(r+2)}
D^{r+2}\mathcal P_i(0)[z^{r+2}],\qquad r=0,1,2,
\tag{T.25}
\]

\[
W_r=-\frac1{(r+1)(r+2)}
D^{r+2}\mathcal A(0)[z^{r+2}]
+D^r\mathcal K(0)[z^r],\qquad r=1,2 .
\tag{T.26}
\]

The proven physical derivative estimates give

\[
\deg O_{i,r}\leq r+2,\qquad
\|O_{i,r}\|_{\theta,1}\leq C h^{-4}.
\tag{T.27}
\]

Use the exact radial decomposition

\[
W_r=\sum_y R_{r,y},\qquad
R_{r,y}(z)=\int_0^1
\langle z_y,D_yW_r(sz)\rangle\,ds .
\tag{T.28}
\]

Its coefficient budgets are

\[
\deg R_{1,y}\leq3,\quad
\deg R_{2,y}\leq4,\quad
\|R_{r,y}\|_{\theta,1}\leq C .
\tag{T.29}
\]

These are fixed-degree tensors; taking an arbitrary number of external marks requires no physical derivatives beyond those already used in the coefficient and remainder proofs.

Define

\[
L_m^\#=\kappa_{\nu_\#}(O_{1,0},\ldots,O_{m,0}),
\qquad \#\in\{P,\infty\}.
\tag{T.30}
\]

Define \(C_{2,m}^{\#}\) by the exact five-term second-response formula:

\[
\begin{aligned}
C_{2,m}^{\#}
={}&
\sum_i\kappa_\#(O_{1,0},\ldots,O_{i,2},\ldots,O_{m,0})
\\
&+2\sum_{i<j}\kappa_\#
(O_{1,0},\ldots,O_{i,1},\ldots,O_{j,1},\ldots,O_{m,0})
\\
&+2\sum_i\kappa_\#
(O_{1,0},\ldots,O_{i,1},\ldots,O_{m,0},W_1)
\\
&+\kappa_\#(O_{1,0},\ldots,O_{m,0},W_2)
\\
&+\kappa_\#(O_{1,0},\ldots,O_{m,0},W_1,W_1).
\end{aligned}
\tag{T.31}
\]

Every occurrence of \(W_r\) means the anchored sum (T.28). The last line has two separate cumulant arguments. At least one external mark is always present.

#### Theorem 5.1 — all-order Gaussian coefficient replacement, P

For every \(m\geq1\),

\[
\boxed{
|L_m^P-L_m^\infty|
+|C_{2,m}^P-C_{2,m}^\infty|
\leq
C^{m+1}(m!)^2h^{-4m} e^{-\lambda P^2/16}
\exp\!\left[-\frac{\gamma\tau(x_1,\ldots,x_m)}{8(m+4)}\right].
}
\tag{T.32}
\]

Both coefficients separately have the same factorial and spatial bound without the Gaussian error factor. All anchor sums are absolutely controlled, uniformly in volume.

**Proof.** Every term in (T.31), after (T.28), has \(N=m+r\) arguments with \(r\leq2\). Individual degrees are at most four. Its total degree is at most

\[
D\leq2N+2.
\tag{T.33}
\]

For clarity, the five lines have respective maximum degrees
\[
2m+2,\quad 2m+2,\quad 2m+4,\quad
2m+4,\quad 2m+6,
\]
while their argument counts are
\[
m,\quad m,\quad m+1,\quad m+1,\quad m+2.
\]
Thus (T.33) holds in every case. The leading coefficient has \(D=2m\).

The coefficient-norm product is bounded by \(C^{m+2}h^{-4m}\). Apply (T.22) and Lemma 4.2. There are at most \(C(m+1)^2\) external derivative placements in (T.31), another fixed polynomial absorbed by \(C^{m+1}\). This proves (T.32).

For the separate coefficient bounds, use (T.21) and the same anchor summation without the cutoff-comparison factor. The \(N=1\) moment is controlled by (T.9). \(\square\)

#### Theorem 5.2 — all-order native expansion with ordinary Wick coefficients, P

Under the stated native-law assumptions, for all \(m\geq1\),

\[
\boxed{
\begin{aligned}
K_m^P(g)
&=L_m^\infty+\frac{g^2}{2}C_{2,m}^\infty+\mathcal E_m(g,P),
\\
|\mathcal E_m(g,P)|
&\leq C^{m+1}(m!)^2h^{-4m}
\bigl(|g|^4+e^{-cP^2}\bigr)
\exp\!\left[-\frac{\gamma\tau(x_1,\ldots,x_m)}{8(m+4)}\right].
\end{aligned}}
\tag{T.34}
\]

For the Euclidean block balls one may take \(c=\lambda/16\), after choosing a common smaller spatial rate \(\gamma\). Constants are uniform in the admitted finite volume, \(P\), \(g\), and \(m\).

**Proof.** The parity theorem already gives

\[
K_m^P(g)=L_m^P+\frac{g^2}{2}C_{2,m}^P+R_{4,m}^P(g),
\]

\[
|R_{4,m}^P(g)|
\leq
|g|^4 C^{m+1}(m!)^2h^{-4m}
e^{-\gamma\tau/[4(m+4)]}.
\]

Insert (T.32), absorb the fixed bound on \(1+g^2\), and weaken the common spatial rate as displayed. \(\square\)

The laws defining \(L_m^\infty\) and \(C_{2,m}^\infty\) are ordinary finite-dimensional centered Gaussians with covariance \(H^{-1}\). Wick contraction is therefore legitimate for every coefficient in (T.31). This does not identify that covariance with a continuum propagator, and does not declare the second coefficient universal.

#### Corollary 5.3 — logarithmic windows uniformly in the source order, P

Suppose the admitted physical endpoints have

\[
P(g_*)=a_0[\log(g_*^{-1})]^p,\qquad p>\frac12.
\tag{T.35}
\]

There exists a single \(g_0>0\), independent of \(m\), such that
\(e^{-cP(g_*)^2}\leq g_*^4\) for \(0<g_*\leq g_0\). Consequently (T.34) at \(g=g_*\) has an \(O(g_*^4)\) remainder with the same fixed factorial exponent for **all source orders simultaneously**.

**Proof.** With \(t=\log(g_*^{-1})\), the required inequality is
\(ca_0^2t^{2p}\geq4t\), which holds for all sufficiently large \(t\). Its threshold has no source-order dependence because the \(P\)-power was already paid in the factorial bound. \(\square\)

The cutoff is held at the endpoint value \(P(g_*)\) throughout each signed computational interpolation. No derivative of a moving cutoff is omitted. This is a fourth-order parameter remainder at arbitrary source order, not an all-orders perturbative expansion in \(g\).

### 6. Full moments: the factorial exponent stays two

Let

\[
M_m^P(g)=\nu_g\!\left(\prod_{i=1}^mO_i(g)\right).
\]

For each nonempty label subset \(B\), let \(L_B^\infty\) and
\(C_{2,B}^\infty\) denote the corresponding connected coefficients. Set

\[
\mathfrak M_m^\infty
=\sum_{\pi\in\Pi_m}\prod_{B\in\pi}L_B^\infty,
\tag{T.36}
\]

\[
\mathfrak C_{2,m}^\infty
=\sum_{\pi\in\Pi_m}\sum_{B\in\pi}
C_{2,B}^\infty
\prod_{A\in\pi,\ A\ne B}L_A^\infty .
\tag{T.37}
\]

The first quantity is exactly the full Gaussian moment of the quadratic native fields. The second is the compatible normalized full-moment response assembled from (T.31).

#### Lemma 6.1 — partition budget, P

For every \(m\geq1\),

\[
\sum_{\pi\in\Pi_m}\prod_{B\in\pi}(|B|!)^2
\leq 2^{m-1}(m!)^2.
\tag{T.38}
\]

**Proof.** Order the \(k\) blocks and write their sizes as a composition
\(n_1+\cdots+n_k=m\). Dividing the ordered count by \(k!\) gives

\[
\sum_{\pi\in\Pi_m}\prod_{B\in\pi}(|B|!)^2
=
m!\sum_{k=1}^{m}\frac1{k!}
\sum_{\substack{n_1,\ldots,n_k\geq1\\
n_1+\cdots+n_k=m}}\prod_{j=1}^{k}n_j!.
\]

Since \(\prod_jn_j!\leq m!\), the right side is at most
\((m!)^2\sum_k\binom{m-1}{k-1}/k!\leq2^{m-1}(m!)^2\). \(\square\)

#### Theorem 6.2 — full-moment expansion, P

For every source order,

\[
\boxed{
M_m^P(g)
=\mathfrak M_m^\infty
+\frac{g^2}{2}\mathfrak C_{2,m}^\infty
+\mathfrak E_m(g,P),
}
\tag{T.39}
\]

\[
\boxed{
|\mathfrak E_m(g,P)|
\leq
C^{m+1}(m!)^2h^{-4m}
\bigl(|g|^4+e^{-cP^2}\bigr).
}
\tag{T.40}
\]

The full coefficients themselves obey the same factorial bound without the small error factor.

**Proof.** The full moment is the partition polynomial in the connected functions. The parity theorem bounds every connected derivative through order four by
\(C^{|B|+1}(|B|!)^2h^{-4|B|}\), after dropping its spatial factor.
Differentiating the partition polynomial at most four times adds a factor bounded by a fixed power of the number of blocks, hence by \(m^4\). Equation (T.38) bounds the sum of products of the connected budgets. The factors \(C^{m+|\pi|}\) and \(m^4\) are absorbed into one \(C^{m+1}\).

The full moment is even in \(g\) by the same exact \((g,z)\mapsto(-g,-z)\) change of variables. Taylor's theorem therefore gives its fourth-order remainder with the bound in (T.40).

To replace its zeroth and second cutoff-Gaussian coefficients, use the partition formulas (T.36)–(T.37) with \(P\) in place of \(\infty\), telescope each product, and insert (T.32). At most two marked block choices occur: one for the second response and one for the changed coefficient. Their cost is at most \(m^2\), absorbed in \(C^{m+1}\). Every product carries exactly \(h^{-4m}\), and (T.38) retains factorial exponent two. \(\square\)

No connected spatial decay is asserted for a full moment; its disconnected products need not decay when their clusters are separated.

### 7. Direct joint-test continuity at a fixed physical scale

This section makes the distribution-space statement explicit. It does not infer a joint-kernel estimate from a bound only on tensor-product tests.

Write the current coordinate sites as integer vectors \(x\), with
physical positions \(hx\) in the grid \(h\mathbb Z^4\), with
\(0<h\leq1\), and use any finite subset or chosen torus fundamental domain. For a full-moment kernel define the lattice distribution

\[
\mathcal M_{m,h}^P(g;F)
=h^{4m}\sum_{x_1,\ldots,x_m}
M_m^P(g;x_1,\ldots,x_m)
F(hx_1,\ldots,hx_m),
\quad F\in\mathcal S(\mathbb R^{4m}).
\tag{T.41}
\]

Define the coefficient and error distributions by the identical summation. The maximum over the fixed finite field-label family changes only \(C^{m+1}\).

#### Proposition 7.1 — fixed linear test order, P

For

\[
\nu_s(F)=
\max_{|\alpha|\leq s}\sup_X
(1+|X|^2)^{s/2}|\partial^\alpha F(X)|,
\]

the full-moment error obeys

\[
\boxed{
|\mathfrak E_{m,h}(g,P;F)|
\leq
C^{m+1}(m!)^2h^{-4m}
\bigl(|g|^4+e^{-cP^2}\bigr)\nu_{6m}(F).
}
\tag{T.42}
\]

The full moments and their coefficients have the corresponding bound without the small error factor.

**Proof.** The elementary lattice estimate

\[
\sup_{0<h\leq1}
h^4\sum_{x\in\mathbb Z^4}(1+|hx|^2)^{-3}<\infty
\tag{T.43}
\]

follows by comparison with the integrable weight on neighboring cubes.
Moreover

\[
(1+\textstyle\sum_i|X_i|^2)^{-3m}
\leq\prod_i(1+|X_i|^2)^{-3}.
\]

Thus

\[
h^{4m}\sum_{x_1,\ldots,x_m}
|F(hx_1,\ldots,hx_m)|
\leq C^m\nu_{6m}(F).
\]

Insert (T.40). The argument applies to arbitrary joint \(F\), using its actual kernel and a direct absolutely convergent sum. \(\square\)

Equation (T.42) is uniform in volume and Gaussian cutoff, but **not in the ultraviolet shell scale \(h\)**. Its \(h^{-4m}\) is the physical dimension-four normalization, and has not been removed by changing the field definition. In particular, (T.42) alone is not J2 or S0 for the Wilson continuum hierarchy.

The estimate applies to coincidence-flat tests as a subspace, but does not itself exploit their flatness. That exploitation is the next lemma.

### 8. What coincidence flatness buys for a localized connected shell

The following statement records the physical summation cost. It is useful for the new all-order error kernels and for any eventual exact transported kernel with the same majorant.

#### Proposition 8.1 — full-diagonal shell summation, P

Let \(m\geq2\), \(0<a\leq h\leq1\), and let a connected kernel on the Euclidean physical grid \(a\mathbb Z^4\) satisfy

\[
|T_{m,h}(X_1,\ldots,X_m)|
\leq
C_0^{m+1}(m!)^2h^{-4m}\varepsilon_h
\exp\!\left[
-\frac{\gamma\tau(X_1,\ldots,X_m)}{8(m+4)h}
\right].
\tag{T.44}
\]

Here \(\tau\) is the minimum-tree length for the ordinary physical metric, and \(\varepsilon_h\geq0\). Let \(F\) be a Schwartz function whose normal derivatives through order four, including its value at order zero, vanish on the full diagonal. Coincidence-flat Schwartz functions satisfy this condition. Then

\[
\boxed{
\left|
a^{4m}\sum_{X_1,\ldots,X_m}
T_{m,h}(X_1,\ldots,X_m)F(X_1,\ldots,X_m)
\right|
\leq
C^{m+1}(m!)^7h\,\varepsilon_h\,\nu_{6m}(F).
}
\tag{T.45}
\]

The same assertion holds with integrals in place of the grid sums.

**Proof.** Put \(r_i=X_i-X_1\), \(i\geq2\). Taylor's integral remainder in the relative coordinates, through degree four at \(r=0\), gives

\[
|F(X_1,\ldots,X_m)|
\leq
C\Bigl(\sum_{i=2}^m|r_i|_1\Bigr)^5
(1+|X_1|^2)^{-3}\nu_{6m}(F).
\tag{T.46}
\]

All intermediate points in that Taylor formula retain the first coordinate \(X_1\), so the Schwartz weight has the stated lower bound. The multi-index coefficient sum is included exactly by the fifth power of the \(\ell^1\) relative-coordinate norm.

Every \(r_i\) is a path displacement in a spanning tree; hence
\(\sum_{i\geq2}|r_i|_1\leq C(m-1)\tau\).
Absorb \(\tau^5\) into half the exponential in (T.44):

\[
\tau^5e^{-\gamma\tau/[8(m+4)h]}
\leq C_\gamma (m+4)^5h^5
e^{-\gamma\tau/[16(m+4)h]}.
\tag{T.47}
\]

Bound the last minimum-tree exponential by the sum over all labeled trees. There are \(m^{m-2}\) such trees. Successively summing leaves, using \(a\leq h\), bounds each tree's relative-coordinate integral by

\[
\left[C_\gamma(m+4)^4h^4\right]^{m-1}.
\tag{T.48}
\]

The remaining \(X_1\) sum of the weight in (T.46) is uniformly bounded by (T.43), with \(a\) in place of \(h\). The powers of \(h\) are
\[
h^{-4m}h^5h^{4(m-1)}=h.
\]

The tree count and range factors obey
\[
m^{m-2}(m+4)^{4(m-1)}
\leq C^m(m!)^5.
\]
The extra fixed powers from (T.46)–(T.47) are absorbed into \(C^{m+1}\). Multiplying by the \((m!)^2\) in (T.44) gives (T.45). \(\square\)

For a geometric shell sequence \(h_j=L^{-j}h_0\), Proposition 8.1 gives

\[
\left|\sum_j T_{m,h_j}(F)\right|
\leq
C^{m+1}(m!)^7\nu_{6m}(F)
\sum_jh_j\varepsilon_{h_j},
\tag{T.49}
\]

whenever the last sum is finite. In particular a uniformly bounded
\(\varepsilon_{h_j}\) suffices. The new native Gaussian-cutoff error has
\(\varepsilon_{h_j}=e^{-cP_j^2}\); its fourth-order comparison error has
\(\varepsilon_{h_j}=|g_j|^4+e^{-cP_j^2}\).

**Geometry restriction.** The estimate uses physical Euclidean distances. On finite tori it applies locally when the compact test support lies in a nonwrapping patch so that the required tree-distance majorant is the same there. It is not an unproved global replacement of periodic distance by Euclidean distance. The separate fixed-shell joint bound (T.42) has no such spatial premise.

**Contact restriction.** This is a full-diagonal Taylor subtraction statement with normal order four. It does not prove the complete hierarchy of partial-diagonal counterterms generated by collisions inside transported subclusters. The one-point term, for which there is no relative coordinate, still requires its separate identity subtraction.

**Matching restriction.** The actual Wilson connected hierarchy has not been shown to equal a sum of the native connected kernels in (T.44). Conditional cumulants of retained means and all generated response vertices remain necessary. Formula (T.49) proves summability after the physical kernel representation is supplied; it does not supply that representation.

### 9. What is closed, and what remains

| Item | Status |
| --- | --- |
| Gaussian cutoff removal only at fixed source order | Closed for the almost-quadratic degree family: (T.19) is uniform in all source orders with factorial exponent two. |
| Wick coefficient comparison restricted to \(m\leq6\) | Closed in the fixed native regular law: Theorems 5.1–5.2 hold for every \(m\). |
| Extensive insertion sums in the second coefficient | Closed in that scope: there are at most two additional anchors, and their order cost is polynomial. |
| Cutoff error \(P^{2m+6}e^{-cP^2}\) obstructing uniformity in \(m\) | Closed by the degree-explicit estimate; the error is \(C^{m+1}(m!)^2e^{-cP^2}\). |
| Compatible full moments | Closed in that scope through the partition formulas and Lemma 6.1. |
| Joint-test continuity rather than tensor-product-only estimates | Proved at each fixed \(h\), with explicit \(q=6\), \(p=2\), and the retained physical factor \(h^{-4m}\). |
| Ultraviolet summation of a localized connected shell majorant | Proved on the stated flat-test/physical-distance domain, with \(q=6\), \(p=7\), and shell gain \(h\). |
| Exact microscopic matching and complete normalized history law | Still open. Native/reference theorems do not establish M0, C0, H0 or the actual full-law S0 estimate. |
| Running normalization, rotations, physical UV coefficients and operator/phase estimates | Still open in their previously stated scopes. |

This annex removes an all-order limitation in the regular Gaussian comparison and records the actual factorial and distribution-space budgets. It does not complete four-dimensional Yang–Mills existence.

### Proof dependencies

- The parity theorem (Annex J) supplies the actual fixed native law, physical derivatives through order six, and its all-order fourth-parameter-derivative bound.
- The Gaussian cutoff theorem (Annex K) supplies normalized boundary flux, the full-space OU comparison, and uniform block moments. Its sole convexity import is the precisely scoped Prékopa marginal theorem already cited there.
- The Wick comparison (Annex K, Section 5) supplies the actual homogeneous precision/semigroup identification, weighted polynomial coefficient norms and the two-law covariance scope.
- The real cut theorem supplies the two-gradient cumulant estimate; its partition coefficient is explicitly tracked in Lemma 4.1.

The degree-explicit cutoff bound, all-order replacement, fixed-factorial full-moment assembly, and explicit joint-test estimates above are derived here.


---
