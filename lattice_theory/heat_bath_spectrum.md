# Wilson heat-bath spectral reduction

## Scope

On the finite four-dimensional periodic Wilson lattice of the source, an exact finite-range positive part of the bare scalar covariance can be absorbed, through second source order, into a deterministic Taylor contact with a vanishing physical-cell error. The remaining nonlocal contribution is carried, up to a vanishing fixed-test error, by a shrinking interval of the spectrum of a specified reversible heat-bath operator at eigenvalue one. All inner products below use the actual normalized Wilson measure. The spectral parameter is an auxiliary update rate, unrelated here to the physical Hamiltonian.

The construction yields an equivalent remaining estimate for the second scalar jet. Its contact coefficients can depend on the torus. The prescribed local vacuum and the residual slow covariance require a further estimate. No dynamical spectral gap, pure phase, or continuum measure is assumed.

The subsequent sections use further features of the Wilson law. Section 8 proves a same-coupling chessboard inequality for spatial scalar responses and a leading local covariance law on a susceptibility-selected sequence. Sections 9–11 prove a Gaussian curvature-energy law at microscopic separations, an explicit growing separation window at prescribed weak coupling, and a quantitative bound on the mean Wilson energy. Section 12 identifies the remaining temporal transfer weight, proves microscopic saturation of the two-plane conditional score by near-plane predictors, and locates the first unsupplied norm gain in a scale iteration. The stated microscopic windows do not extend to a fixed positive physical separation on the stopped trajectory. Full interacting R2 remains open.

## 1. The update and its exact spatial support

Write $e_x=\sum_{\mu<\nu}s_{p_{\mu\nu}(x)}$, $X_x=e_x-\mu e_x$, and $F_f=\sum_x f(x)e_x$, as in (CP.1), (CP.22). Sites are physical points of spacing $a$. The connection graph has one vertex per positive link and one edge between distinct links in a common plaquette. Its degree is at most 18, including at side length $n=2$. Fix a proper coloring with 19 colors, allowing empty colors. A random update uniformly chooses a torus translation of the coloring and then a uniform color. For the resulting independent link set $I$, let $K_I F=\mathbb E_\mu(F\mid U_{I^c})$, and $P=\mathbb E_I K_I$. Averaging translations makes $P$ translation covariant even on tori without a chosen checkerboard period. Color averaging is independent of the configuration. All estimates hold for any such translation-invariant average of independent color classes. On even tori we use the eight classes specified in §6 when making the lower-bound comparison there.

Each plaquette meets $I$ in at most one link. Disintegration of the Wilson density therefore gives a product of exact conditional one-link laws, with the other links in the six incident plaquettes specifying the factors. Each $K_I$ is an orthogonal projection in $L^2(\mu)$. Thus $0\le P\le1$, $P1=1$, and, for real functions,
\[
 \langle F,(1-P)G\rangle=\mathbb E_I\mathbb E_\mu\operatorname{Cov}(F,G\mid U_{I^c}).
 \tag{1}
\]
This expression vanishes for disjoint link supports, since conditional on the exterior their remaining color variables form disjoint subcollections of the product law. Also, $K_I F$ is supported in the closed one-neighborhood of the link support of $F$ in the connection graph. The integrals for every updated link outside the support cancel independently. Iteration gives graph propagation by at most $j$ links for $P^jF$.

For a real polynomial $p$ of degree $m\ge1$, with $p(1)=1$ and $0\le p\le1$ on $[0,1]$, define
\[
 B_{xy}=\langle X_x,(1-p(P))X_y\rangle,\qquad
 S_{xy}=\langle X_x,p(P)X_y\rangle .
 \tag{2}
\]
Both matrices are positive semidefinite and their sum is the actual covariance. The supports of $X_x$ have link tails at sup distance at most $a$ from $x$; adjacent graph links have tails at torus sup distance at most $a$. Factor $1-p(t)=(1-t)q(t)$, with degree of $q$ at most $m-1$, and apply (1) to $X_x,P^jX_y$. This proves
\[
 B_{xy}=0\qquad\text{if } d_{T,\infty}(x,y)>(m+2)a. \tag{3}
\]
In particular (2) preserves exactly the separated covariance in $S$ outside that radius.

## 2. An operator estimate on the finite-range piece

The single-star estimate (CA.2) implies $\mathbb E_\mu S_b^2\le C\beta^{-2}$ on the compatible N2-F trajectory, by $t^2\le2e^t$ for $t\ge0$. Here $S_b$ is the sum of the six incident plaquette energies. Fix $I$ and the exterior. The sum $F_u$, for any real site array $u$, is an exterior function plus the sum of independent star functions $H_b=\sum_{p\ni b}u(x_p)s_p$, $b\in I$. At fixed exterior their variances add. Since $H_b^2\le(\sum_{p\ni b}|u(x_p)|^2) S_b^2$, (1) gives
\[
 \langle F_u,(1-P)F_u\rangle\le C\beta^{-2}\sum_x|u(x)|^2 . \tag{4}
\]
The absolute multiplicity in the sum over all links and plaquettes at a given anchor is $4\cdot6=24$. Centering has no effect on (4). Consequently if $1-p(t)\le M(1-t)$ on $[0,1]$,
\[
 \|B\|_{\ell^2(\text{sites})\to\ell^2(\text{sites})}\le C\beta^{-2}M. \tag{5}
\]
Uniformly, $\|X_x\|_{L^2(\mu)}\le C\beta^{-1}$ follows from the same star moment bound and the triangle inequality.

## 3. A filter with uniform estimates

For integer $k\ge1$ and $0<\delta\le1/2$ use the first-kind Chebyshev polynomial $T_k$ and set
\[
 p(t)=\left[
 \frac{T_k(2t/(1-\delta)-1)}
 {T_k((1+\delta)/(1-\delta))}
 \right]^2,\quad m=2k.
 \tag{6}
\]
On the mapped interval $[-1,1]$, $|T_k|\le1$, and from 1 to the mapped endpoint $T_k(\cosh v)=\cosh(kv)$ increases. Thus $0\le p\le1$ and $p(1)=1$. The denominator is $\cosh(2k\operatorname{artanh}\sqrt\delta)$. Hence
\[
 \sup_{[0,1-\delta]}p\le4e^{-4k\sqrt\delta},\qquad
 1-p(t)\le 8k^2(1-t). \tag{7}
\]
For the second bound, $|T'_k(\cos\theta)|=k|\sin(k\theta)/\sin\theta|\le k^2$ on $[-1,1]$. On the hyperbolic portion $T'_k(\cosh v)=k\sinh(kv)/\sinh v\le k^2\cosh(kv)$, using $\tanh(kv)\le kv\le k\sinh v$. Differentiate the square in (6), divide by the denominator squared, use $2/(1-\delta)\le4$, and integrate the resulting derivative bound. Thus (5) applies with $M=8k^2$.

## 4. Strict order-four contact and cutoff error

Let $R=(2k+2)a<T/4$ and use the unique short lift $r=y-x$ in each coordinate when $B_{xy}\ne0$. Write $P_x^4g(r)=\sum_{|\alpha|\le4}\partial^\alpha g(x)r^\alpha/\alpha!$. Define the local quadratic contact by its symmetric bilinear jet
\[
 Q_B(f,g)=\tfrac12\sum_{x,y}B_{xy}
 [f(x)P_x^4g(y-x)+g(x)P_x^4f(y-x)]. \tag{8}
\]
At each $x$ this uses only source values and derivatives at $x$. The coefficients are translation invariant. Symmetry of $B$ then makes the odd total-degree moments zero. Neither this assertion nor the proof requires a point-scalar reflection law for the original lower-vertex representative.

For tests supported in $D_f,D_g$ physical cells, with $|D|$ denoting the count in their union and $\|\cdot\|_*=\|\cdot\|_{C^5,\ell_0}$, put $\epsilon=a/\ell_0$. If $R\le\ell_0/8$, then
\[
 \left|\sum_{x,y}B_{xy}f(x)g(y)-Q_B(f,g)\right|
 \le C |D|\beta^{-2}\epsilon (k+1)^7\|f\|_*\|g\|_* . \tag{9}
\]

**Proof of (9).** Split rows $x$ into blocks $A$ of side comparable to $R$ and columns $y$ into the same blocks $A'$. In each direction, partition the $n$ sites into intervals of $m+2$ to $2(m+2)$ sites, by merging a possible short last interval with its predecessor. Only a bounded number of neighbor blocks can contribute for a given $A$ by (3). Use local periodic lifts of any contributing pair (splitting a pair into a bounded number of rectangular pieces if lifts at a periodic cut require it). All contributing $x,y$ are within $C R$ of one chosen block center $z$. For sufficiently small $R/T$ these lifts give $r=y-x$ on all contributing entries. For the estimates one may impose $R<T/32$, which holds under $T\ge2\ell_0$ at all sufficiently small cutoffs; for the other bounded ratios, subdivide blocks by a fixed factor first.

Subtract the degree-four polynomial $Q(y)=P_z^4g(y-z)$ throughout $g(y)-P_x^4 g(y-x)$. Polynomials of degree at most four cancel exactly. Set $h=g-Q$; its derivatives satisfy $|\partial^\alpha h|\le C R^{5-|\alpha|}\sup|D^5g|$ through degree four throughout these blocks. Expand each factor $(y-x)^\alpha$ as a sum of products of powers of $y-z$ and $x-z$. This expresses $f(x)[h(y)-P_x^4 h(y-x)]$ as a fixed finite sum of separable row and column factors. On this block pair each product of their sup norms is bounded by $C\|f\|_\infty R^5\sup|D^5g|$. Only row blocks intersecting the support of $f$ contribute to this unsymmetrized expression.

Cauchy–Schwarz and (5),(7) bound each resulting bilinear form by the same sup-norm product times $C\beta^{-2}k^2\sqrt{\#A\,\#A'}$. All blocks have comparable lattice counts, and the total count of the contributing row blocks, enlarged by their boundaries, is at most $C|D|(\ell_0/a)^4$. Indeed $R\le\ell_0/8$, so each physical cell together with its block neighborhood has at most $C(\ell_0/a)^4$ sites. Summing, symmetrizing, and using $R/\ell_0=(2k+2)\epsilon$ proves (9). This bound uses the signed matrix norm in (5); an entrywise absolute-value estimate would lose additional powers of $k$.

## 5. Remaining second-jet estimate

For sufficiently small $\epsilon$, take $k=\lfloor\epsilon^{-1/7}\rfloor$, $\delta=(3\log(1/\epsilon)/k)^2\le1/2$, and put $\Pi=\mathbf 1_{\{t>1-\delta\}}(P)$. These are asymptotic choices. The finitely many lower trajectory depths have bounded $a^{-1}$ and are handled for raw fixed tests by boundedness of plaquette actions. Define $Y_f=F_f-\mathbb E_\mu F_f$ and
\[
 S_{\rm slow}(f,g)=\langle Y_f,p(P)\Pi Y_g\rangle.
\]
For $v_f=|D_f|\|f\|_*$ and $v_g=|D_g|\|g\|_*$, the triangle inequality gives $\|Y_f\|_2\le C\beta^{-1}\epsilon^{-4}v_f$. Functional calculus and (7) bound the part of $p(P)$ on $1-\Pi$ by $4\epsilon^{12}$. Thus for the unchanged source one has
\[
 \left|\operatorname{Cov}_\mu(F_f,F_g)-Q_B(f,g)-S_{\rm slow}(f,g)\right|
 \le C\beta^{-2}\left(|D|\|f\|_*\|g\|_*+\epsilon^4v_fv_g\right).
 \tag{10}
\]
The right side tends to zero for fixed physical supports along N2-F where $\beta\to\infty$. For sources whose supports are farther apart than $R$, the entire $B$ pairing vanishes identically, and the error in replacing the separated covariance by $S_{\rm slow}$ is bounded by $C\beta^{-2}\epsilon^4v_fv_g$. For a running multiplicative normalization the error and both extracted quadratic forms scale by the square of that normalization.

For the actual prescribed quadratic jet $c_{a,2}$, (10) proves that a uniform fixed-test estimate on the second derivative is equivalent, within its explicit error, to a uniform estimate of
\[
 S_{\rm slow}(f,g) - \big[c_{a,2}(f,g)-Q_B(f,g)\big]. \tag{11}
\]
For separated supports with zero mixed prescribed contact this entails an actual bound on the slow overlap. Such a bound may allow a constant phase covariance. For overlapping supports a further short-distance contact can reside inside $S_{\rm slow}$. Formula (11) retains precisely the difference to the prescribed counterterm, including any torus-copying obligation. Long correlation lengths and a uniform positive update gap are independent questions; the proof needs no gap. No bound on the remaining slow overlap follows from (4), which weights its spectral measure by $1-t$.

This result concerns the actual source-zero second logarithmic derivative. It gives no estimate on a fixed complex source disk, on the mean, or on other source orders. It leaves the two-jet and full interacting R2 open.

## 6. Size of the extracted quadratic contact on even tori

Use eight classes, each determined by the link direction $\mu$ and the parity of the sum of the three transverse lattice coordinates. Two distinct parallel links on a plaquette differ by one transverse step. Even $n$ makes that step reverse the parity across periodic seams as well. All eight classes are independent sets, each contains $n^4/2$ links, and translations permute the classes. Uniform averaging already gives a translation-covariant $P$. Choose this operator throughout (1)–(11) in this section.

Let $H_b=\sum_{p\ni b} f(x_p)s_p$. Conditional independence gives the stronger identity
\[
 \langle Y_f,(1-P)Y_f\rangle
   =\tfrac18\sum_b \mathbb E_\mu\operatorname{Var}(H_b\mid U_{b^c}). \tag{12}
\]
Indeed the conditional law at $b$ with the entire color exterior fixed agrees with its one-link law given all other links. Its staples involve no other link of that color. The conditional variance of the sum of the updated stars therefore has exactly the eight-class average in (12).

For the uniform star write $v_\beta=\mathbb E_\mu\operatorname{Var}(S_b\mid U_{b^c})$. Translation and axis permutations make this independent of $b$. The conditional-star Laplace estimate gives $\beta^2 v_\beta\to d_A/2$, where $d_A=N^2-1$, along compatible tori. One can also see the uniformity directly as follows. Use the fixed good-star threshold of (CP.8)–(CP.10). On this event the centered potential at its minimum has uniform global quadratic confinement, a uniformly positive and bounded Hessian, and uniform third derivatives by compactness. Rescale exponential coordinates by $\sqrt\beta$. Along any sequence of good-star Hessians extract a convergent subsequence. Taylor's theorem and the Gaussian bound from (CP.10) give convergence of the first two moments of the rescaled excess energy to those of its limiting Gaussian quadratic energy. In orthonormal coordinates its law is $\chi^2_{d_A}/2$, independently of the limiting positive Hessian. Dominated convergence uses a fixed chart, a Gaussian times a degree-four polynomial there, and exponentially small contributions on the compact exterior. Thus the conditional variance times $\beta^2$ tends uniformly to $d_A/2$ on good stars. Since the star minimum $W_b\le S_b$, (CA.2) bounds the bad exterior probability by $C e^{-c\beta}$; there $S_b\le12N$. Both errors vanish after averaging, which proves the asserted asymptotic.

For a fixed real smooth compactly supported test, the literal anchors satisfy
\[
 |H_b-f(x_b)S_b|\le C\epsilon\|f\|_*S_b
\]
with $x_b$ the positive link tail. Conditional Cauchy–Schwarz followed by averaging and (CA.2) implies that each corresponding variance in (12) differs from $f(x_b)^2v_\beta$ by at most $C\epsilon\|f\|_*^2\beta^{-2}$. Only links within one lattice spacing of the support contribute. Summing (12), using four positive links per site and the Riemann sum for the fixed test, gives
\[
 \lim_{a\to0}\beta^2a^4\langle Y_f,(1-P)Y_f\rangle
       =\frac{d_A}{4}\int f(x)^2\,dx . \tag{13}
\]
The same assertion holds for a fixed periodic test on a fixed physical torus.

Let $\eta=4e^{-4k\sqrt\delta}<1$ at sufficiently small cutoffs. Then
\[
 1-p(t)\ \ge\ (1-\eta)(1-t),\qquad 0\le t\le1 . \tag{14}
\]
On $[0,1-\delta]$ this follows from (7). On $[1-\delta,1]$ the map $p$ is convex. Indeed the Taylor coefficients of $T_k(1+s)$ are nonnegative, since its zeros $\cos((2j-1)\pi/(2k))$ lie strictly below 1 and its leading coefficient is positive. Squaring and positive affine rescaling preserve convexity on the interval in question. The chord from $(1-\delta,p(1-\delta))$ to $(1,1)$ bounds $p$ from above, giving (14) with the stronger factor $(1-\eta)/\delta$ on this interval.

Functional calculus, (13), and (14) apply to the diagonal $B$ pairing. Replacing this pairing by (8) costs $O_f(\beta^{-2})$ by (9) with the cutoff choice of §5. Thus the finite-range part alone carries a compulsory quadratic coefficient in the sense
\[
  \liminf_{a\to0}\beta^2a^4 Q_B(f,f)
             \ \ge\ \frac{d_A}{4}\int f(x)^2\,dx . \tag{15}
\]
The equality in (13) concerns one update. The inequality in (15) allows a larger contribution in $Q_B$ and further local divergences in the remaining slow covariance. It measures the diagonal bilinear jet, without assigning any individual Taylor coefficient or the complete prescribed vacuum.

## 7. Growing hidden boxes capture the full lower bound of Annex O

A different heat-bath operator gives a stronger result on the same scalar second jet. Write $n=T/a$. For $l\mid n$, $2\le l<n$, tile the fine periodic lattice by four-dimensional cubical boxes of side $l$ fine spacings. Reveal every link lying in a box boundary subcomplex and hide the other links. Equivalently, a link in direction $i$ is hidden when none of its three transverse coordinates is on a tiling cut. All plaquettes touching a hidden link lie entirely in its box, and no plaquette touches the interiors of two boxes. Conditional on the common exterior, the hidden box laws therefore factorize, with the boundary of each box supplying all its conditional data. Write $K_{l,z}$ for conditional expectation given the visible links at offset $z$, and $P_l=l^{-4}\sum_{z\in\{0,\ldots,l-1\}^4}K_{l,z}$. The operator is translation covariant and $0\le P_l\le1$.

The covariance identity (1) applies to this average, with the corresponding visible sigma fields. Its integrand vanishes whenever the two link functions involve no common hidden box, by conditional independence. Two disjoint supports may involve the same box, so mere disjointness no longer suffices. Tails of all links in a closed box have coordinate diameters at most $la$. Each $K_{l,z}$ enlarges the link-tail support in torus sup distance by at most $(l+2)a$, since only boxes touched by hidden links of the input need integration and each such conditional law involves only links of that closed box. Formula (1) itself vanishes on pairs whose link-tail sets are more than $(l+2)a$ apart. Factorization by $1-t$ as in (3), including the two anchor-to-link distances, now gives the safe site range
\[
 R=(2k+3)(l+2)a
\]
for the matrix $B$ formed from $P_l$ with filter (6). Both $B$ and its complement remain positive semidefinite.

In the Dirichlet form of $F_u$ the weighted sum on each fluctuating box is $H_b=\sum_{p\in b}^{*}u(x_p)s_p$, where the star retains only plaquettes meeting hidden links and $b$ now indexes a box. Its expected conditional variance is bounded by $\mathbb E_\mu H_b^2\le(\sum_{p\in b}^{*}|u(x_p)|^2)(\sum_{p\in b}^{*}\mathbb E_\mu s_p^2)$. The second factor is at most $C l^4\beta^{-2}$ by (CA.2). The starred sets are disjoint and there are six plaquettes per anchor. Summing proves
\[
 \langle Y_u,(1-P_l)Y_u\rangle
 \le C l^4\beta^{-2}\sum_x|u(x)|^2,\qquad
 \|B\|_{\ell^2\to\ell^2}\le C k^2 l^4\beta^{-2}. \tag{16}
\]
Thus the proof of (9), with blocks of physical diameter comparable to the new $R$, gives
\[
 \left|\sum_{x,y}B_{xy} f(x)g(y)-Q_B(f,g)\right|
 \le C |D|\|f\|_*\|g\|_*\,\beta^{-2}
             \epsilon(k+1)^7(l+2)^9. \tag{17}
\]
Indeed the three costs are the number $O(|D|\epsilon^{-4})$ of relevant sites, the operator bound in (16), and the degree-five Taylor cost $O((R/\ell_0)^5)$. The constant is independent of $l,k,T,K$ whenever $R$ is sufficiently small relative to $\ell_0$. Equation (8) defines $Q_B$ using this new $B$ and range.

Use one choice for every sufficiently deep compatible torus with $n=(T/\ell_0)L^K$ and $T/\ell_0$ integral:
\[
 l_a=L^{\lfloor K/18\rfloor},\qquad
 k=\lfloor\epsilon^{-1/14}\rfloor,\qquad
 \delta=(3\log(1/\epsilon)/k)^2,\qquad \epsilon=L^{-K}. \tag{18}
\]
Then $l_a\mid n$, $\delta\to0$, $R/\ell_0\to0$, and $\epsilon(k+1)^7(l_a+2)^9=O(1)$ since $7/14+9/18=1$. The fast part of $p(P_{l_a})$ obeys the same $4\epsilon^{12}$ spectral multiplier bound as before. Consequently (10) and (11) hold for this new operator and contact with the same orders of error. No choice in (18) depends on the torus or on a test. The computed contact itself still uses the actual finite-torus law.

It remains to bound how much diagonal covariance this single choice captures. Fix $l_*=L^j\ge2$ independently of $a$. For all sufficiently large $K$, $l_*\mid l_a$. Align the two tilings with the same offset. Every visible big-box link is visible in the subdivided tiling, since any big-box transverse cut is also a fine-box cut. Orthogonal projection onto the smaller visible sigma field decreases the squared projection norm. Averaging offsets modulo $l_a$ gives a uniform residue modulo $l_*$. It follows for *every* centered input $Y$ that
\[
 \langle Y,(1-P_{l_a})Y\rangle
  \ \ge\ \langle Y,(1-P_{l_*})Y\rangle . \tag{19}
\]
For fixed $l_*$, Annex O, equation (O.5) evaluates the right side for $Y=Y_f$ after scaling by $\beta^2a^4$. Each of its $l_*^4$ offsets has the same limit, by the same finite-box argument and translated Riemann sum. That limit is $d_A h_{l_*}\int f^2/(2l_*^4)$, with $h_l=(3l+1)(l-1)^3$. Apply (14) to $P_{l_a}$ and (17) to replace the diagonal $B$ pairing by $Q_B(f,f)$. Its scaled error is $O_f(a^4)$. Take the cutoff liminf **at fixed $j$**, then let $j\to\infty$ in the resulting lower bounds. This proves, for the single choice (18),
\[
 \liminf_{a\to0}\beta^2a^4 Q_B(f,f)
 \ \ge\ \frac{3d_A}{2}\int f(x)^2\,dx . \tag{20}
\]
This is a bound on the extracted Taylor contact for fixed real smooth tests along N2-F, on the aligned compatible tori. It uses no Laplace estimate uniform in a growing box. The factor $3d_A/2$ is the entire lower bound of Annex O.4. Whether it equals the leading coefficient of the complete covariance or of $Q_B$ remains open. The slow bilinear form and the difference to the prescribed torus-independent contact in (11) still require control.

The single-star moment input is source (CA.2) in Wilson energy normalization. The prescribed counterterm and full scalar criterion are in (CP.18), (CP.23), (CP.28) of Complete pressure analysis. For background on positivity of heat-bath chains in finite state spaces, see [Dyer, Greenhill and Ullrich](https://arxiv.org/abs/1301.4055). Equations (1)–(11) above use the conditional projections directly on the compact Wilson configuration space.

## 8. Spatial Wilson susceptibilities from reflection of closed cubes

Write $C_x=x+[0,a]^4$ for a closed unit lattice cube and label the six coordinate planes by $\alpha$. Set
\[
 H_x^\alpha=\tfrac14\sum_{\text{four }\alpha\text{-faces }p\text{ of }C_x}s_p,\quad
 H_x=\sum_\alpha H_x^\alpha,\quad S_\alpha=\sum_x H_x^\alpha .
\]
Each $\alpha$-plaquette belongs to four incident cubes. Thus $S_\alpha$ is its actual orientation sum and $\sum_x H_x=S$. This representative uses the elementary Wilson plaquettes at their reflected cube placements. The lower-vertex observable $e_x$ has a different placement.

On an even periodic lattice, for arbitrary real arrays $v_x\in\mathbb R^6$ and real $t$ the Wilson law satisfies
\[
 \log\mu_\beta \exp\!\left(t\sum_x v_x\cdot H_x^\bullet\right)
 \le V^{-1}\sum_x\log\mu_\beta\exp(t v_x\cdot S_\bullet). \tag{21}
\]
Here $V=n^4$ and bullets indicate the six-vectors. To verify this use the nonnegative base-block factor $\exp(t v_x\cdot H_0^\bullet)$ in the closed-unit-cube chessboard inequality. Reflection in a cube face permutes its four plaquettes of each fixed plane, with reversal of orientation immaterial for the real trace. Hence its transported copy is literally $\exp(t v_x\cdot H_y^\bullet)$ at the target cube $y$. The full dissemination of one label is $\exp(t v_x\cdot S_\bullet)$. The closed support is legitimate: cutting through site planes gives products on the two closed halves with the common boundary links integrated once in (CA.11); the maximizing-coloring proof of (CA.14) then applies verbatim. It requires an even number of cubes per direction and allows shared boundary variables. The closed-cube geometry and multiplicity are also stated in Annex A, §3. This proof uses the actual source-zero homogeneous Wilson law for every real $\beta>0$.

Both sides of (21) vanish at zero and their first derivatives agree by translation invariance. Their difference is nonnegative, so its second derivative at zero is nonnegative. With $\Gamma_{\alpha\gamma}=\operatorname{Cov}(S_\alpha,S_\gamma)/V$ and $\chi=\operatorname{Var}(S)/V$ this yields the exact matrix bounds
\[
 \operatorname{Var}\!\left(\sum_x v_x\cdot H_x^\bullet\right)
 \le\sum_xv_x^\top\Gamma v_x,\qquad
 C^H:=\big[\operatorname{Cov}(H_x,H_y)\big]_{x,y}\ \le\ \chi I . \tag{22}
\]
In particular every scalar cube Fourier susceptibility is at most its zero-momentum value at the same coupling. The matrix order follows for arbitrary real arrays, including changing signs. Translation covariance ensures that constants attain equality.

**Actual fixed-coupling separated inequality.** Let $B$ be the covariance form $\langle Y_f,(1-P_l)Y_g\rangle$ for the cube source $Y_f=\sum_xf_x(H_x-\mu H_x)$ and one tiling update of §7, or for any single fixed aligned tiling with its corresponding conditional projection. The same argument works for the finite-range filtered $B$ of §7. Then $0\le R=C^H-B\le A=\chi I-B$. Take two arrays with disjoint supports and separated sufficiently that $B(f,g)=0$ (for the averaged single update a distance exceeding $(l+4)a$ in sup norm suffices). Then $A(f,g)=0$ and
\[
 |\operatorname{Cov}(Y_f,Y_g)|\le\tfrac12
 \sqrt{\big[\chi\sum_xf_x^2-B(f,f)\big]
       \big[\chi\sum_xg_x^2-B(g,g)\big]}. \tag{23}
\]
To see the factor $1/2$, restrict to the span of the two arrays. In the seminorm of $A$, $f,g$ are orthogonal. The form $R-A/2$ has operator norm at most $1/2$ there, by $0\le R\le A$. Null directions follow directly by Cauchy–Schwarz for $R$. This proves (23) including the use of the complete interacting measure. The bracket in (23) can be bounded from above by subtracting any established lower bound for that same diagonal box variance. Getting fixed physical units requires a quantitative upper bound on the resulting deficits.

**Averaged leading local covariance.** Consider even $n\to\infty$, a fixed physical torus $T$ with $a=T/n$, and the logarithmic coupling windows of Annex O.9. For the following statement also require $\sup_n\log(1+B_n)/V<\infty$. Write $\mathbb A_n$ for the normalized integral in $d\log\beta$ on the window. For fixed real $C^1$ periodic tests define $\mathcal H_f=\sum_x f(x)H_x$. Then
\[
 \mathbb A_n\left|a^4\beta^2
       \operatorname{Cov}_\beta(\mathcal H_f,\mathcal H_g)
             -A_0\int fg\right|\longrightarrow0,\qquad A_0=3d_A/2 .
 \tag{24}
\]
This is a leading quadratic contact statement in logarithmic mean. It makes no claim of a Gaussian distribution or an unscaled separated bound.

Here are the ingredients for (24). Closed-cube dissemination at coefficient $\kappa\beta$, with $\kappa$ small so the shifted bare coefficient is at least $\beta/2$, bounds $\mu_\beta e^{\kappa\beta s_p}$ uniformly: use a cube containing $p$, then (21) with the nonzero weight on just that cube and the recursive forest ratio (CA.9c). This gives $\mu_\beta s_p^2\le C\beta^{-2}$ uniformly on the windows. The coefficient of $s_p$ in $\mathcal H_f$ is the average of $f$ over its four incident cube origins. For a fixed $l$-box the coefficients of its fluctuating plaquettes differ from $f$ at its base by at most $C_l a\|\nabla f\|_\infty$. The fixed-box conditional-variance proof in Annex O.5 applies with this change. In detail, fix $l$ before the limits. Its flattened box energy has scaled conditional variance $d_A h_l/2+o_l(1)$ after averaging the exterior, uniformly as the window lower endpoint tends to infinity; exceptional boundaries have probability $C_l e^{-c_l\beta}$ by the preceding local tail. The energy second moment bounds the root-mean-square error for freezing test weights on that box by $C_l a/\beta$. Sum conditionally independent box variances and reveal any leftover strips. The fixed physical test and the Riemann sum give
\[
 \liminf_n\inf_{\beta\in[b_n,B_n]}a^4\beta^2
   \operatorname{Var}_\beta(\mathcal H_f)
 \ge \frac{d_A h_l}{2l^4}\int f^2 .
\]
Now send $l$ to infinity. Conversely (22) gives $a^4\beta^2\operatorname{Var}\mathcal H_f\le(\beta^2\chi)a^4\sum f_x^2$. Annex O.9 makes the positive part above $A_0\int f^2$ tend to zero in logarithmic mean; the lower estimate gives uniform convergence of the negative part to zero. Polarize at $f+g,f-g$ and use the triangle inequality. This proves (24). For separated tests it bounds the absolute covariance in the displayed scaling, not just the signed mean over translations.

**Placement at the literal lower vertex.** For a plaquette with plane $\alpha=(i,j)$ and base $y$, let $\rho,\sigma$ be its two complementary axes. The coefficient produced at this plaquette by the oriented cube weights $v_{x,\alpha}$ is exactly $(A_\rho A_\sigma v_{\cdot,\alpha})(y)$, where $(A_i u)(y)=(u(y)+u(y-ae_i))/2$. Set
\[
 U_i=\sum_{r=0}^4 (I-A_i)^r,\qquad
 v_{\cdot,\alpha}=U_\rho U_\sigma f.
\]
Since $A_iU_i=I-(I-A_i)^5$, the coefficient differs from $f(y)$ by at most $C a^5\|f\|_{C^5}$ uniformly in all planes. This uses the fifth finite difference in each single coordinate; the second difference operator in a product can be bounded in sup norm without extra derivatives. These weights have a fixed fine-lattice collar and $\|v_{\cdot,\alpha}-f\|_\infty\le C a\|f\|_{C^1}$. Consequently the centered error in representing the literal $F_f$ by $\sum v_x\cdot H_x^\bullet$ has $L^2(\mu)$ norm at most $C_f a/\beta$ for fixed supported smooth tests under the preceding moment bound, or along the N2-F cofinal geometry. This is an error in the **linear insertion**. Errors in covariances additionally multiply the norm of the other insertion.

Axis permutation symmetry makes the all-ones vector an eigenvector of $\Gamma$, with eigenvalue $\chi/6$. Write $\Gamma_\perp$ for its restriction to the orthogonal five-dimensional subspace. As a result, when $a^4\beta^2$ is used to scale the covariance, the extra upper-bound cost of the non-scalar weights from (22) is at most $C_f a^2\beta^2\|\Gamma_\perp\|$. The scalar contribution differs from $\beta^2\chi\,a^4\sum f^2$ by $O_f(a\beta^2\chi)$. For example, at a chosen sequence of couplings where $\beta^2\chi\to A_0$ and $a^2\beta^2\|\Gamma_\perp\|\to0$, the original lower-vertex two-point form obeys $a^4\beta^2\operatorname{Cov}(F_f,F_g)\to A_0\int fg$ by (22), the root-mean-square approximation, the fixed-box lower estimate, and polarization. This conditional statement does not assume the tensor orientation response equals the scalar susceptibility.

For the cube representative (23) is a same-coupling upper bound, and (24) concerns localized smooth marks in the actual law under a coupling average. Neither yields bounded disjoint continuum smearings at a prescribed bare coupling: even a vanishing error after multiplication by $a^4\beta^2$ can diverge in physical units. Matching the prescribed source contact and controlling that stronger remainder remain necessary.

### 8.1 An exact nonconstant class for the original placement

Let $q=(t,t,t,t)$ be a lattice Fourier momentum in radians per site and let $\widehat C^e,\widehat C^H$ denote the covariance eigenvalues for the lower-vertex and cube representatives. On this line all six placement factors $A_\rho A_\sigma$ are the same complex number $[(1+e^{it})/2]^2$ up to conjugation under changing Fourier convention. Thus, for $\cos(t/2)\ne0$,
\[
 \widehat C^e(q)=\frac{\widehat C^H(q)}{\cos^4(t/2)}
 \le \frac{\chi}{\cos^4(t/2)} . \tag{25}
\]
This is a fixed-coupling comparison for the original plaquette source at nonzero momentum. More generally, for a periodic scalar profile depending only on the sum of the four site coordinates, the operators $U_i$ agree on that profile; $v_{\cdot,\alpha}$ in §8 is one common scalar array for all six planes. The orientation susceptibility drops out for this restricted family. Nonzero tests of this type have slab support on a torus.

### 8.2 One choice of susceptibility and geometry

Choose a fixed admissible block factor $L$, fix $n_m=2L^m$, and apply Annex O.9 on $[m^{1/4},m^{1/2}]$ to choose a single $\beta_m$ there with $\beta_m^2\chi_{n_m}(\beta_m)\to A_0$. The choice involves the exact homogeneous susceptibility alone. It is independent of every test. For any $a_m\to0$ with $T_m=n_m a_m\to\infty$, fixed compact smooth tests on the bulk then satisfy
\[
 a_m^4\beta_m^2\,\operatorname{Cov}_{n_m,\beta_m}
     (\mathcal H_f,\mathcal H_g)\ \longrightarrow\ A_0\int_{\mathbb R^4}fg . \tag{26}
\]
The fixed-box proof for the lower bound can use $l=L^j$ at fixed $j$, which divides all sufficiently large $n_m$. Only boxes near the supports enter, and the local energy moment is uniform on the window by (CA.9c) and closed-cube dissemination. Equation (22) gives the upper bound for each diagonal, and polarization gives (26). Therefore (26) holds on that *same sequence* for every fixed pair of tests. In particular the left side tends to zero for disjoint supports, at the displayed leading-contact scaling only.

On the same sequence, for any lattice body-diagonal momenta $q_m=(t_m,t_m,t_m,t_m)$ with $t_m\to0$, one likewise has $\beta_m^2\widehat C^e(q_m)\to A_0$. To check the lower bound uniformly in the spatial extent, use the normalized complex plane wave on sites, or sum the two real variance inequalities for its unnormalized sine and cosine and divide by $V$. The pair's weights change by $O_l(|t_m|)$ on any fixed box and their squares at the box origins sum to one. Freezing as in Annex O.5 gives the lower limit $d_Ah_l/(2l^4)$, first at fixed $l=L^j$ and then as $j\to\infty$. The upper bound is (25). The argument for $H$ itself applies to all lattice momenta tending to zero. This result contains genuinely nonconstant literal modes and requires no control of the five anisotropic homogeneous responses for those modes.

To interpret this selected Wilson sequence on a renormalization trajectory, an additional identification is necessary. Under the causal weak continuation, matched extraction and signed-window bounds of Annex N §§13 and 15, start the recursion at $x_0=\beta_m/(2N)$ and stop when the coupling coordinate first crosses its fixed weak threshold. These inputs give $K_m\asymp \beta_m$ with endpoints in a fixed compact weak interval. Thus $a_m=\ell_0L^{-K_m}$ gives $T_m/\ell_0=2L^{m-K_m}\to\infty$, and its terminal exponent eventually exceeds $K_m$ and every fixed additional buffer exponent. This provides the claimed ample divisibility when the stated native periods are centered powers of $L$ and the matching hypotheses hold. A subsequence can have a common limiting endpoint. The argument does not choose an exactly prescribed endpoint at every depth, does not establish N2-F, and does not satisfy the separate small-terminal-volume premise $V_{K_m}=o(K_m)$. No such running-coordinate identification was used to prove (26) as a Wilson covariance statement.

### 8.3 The Annex E vertex scalar on a common sequence

The scalar used in Annex E (1.5) assigns the *average over the four vertices of each plaquette* to its source in (1.7). This placement admits a stronger conclusion than the lower-vertex input in §8. Select $\beta_m$ in §8.2 so that also $\beta_m\mu(S)/V\to A_0$. To verify simultaneous choice, the signed logarithmic mean of $\beta\mu(S)/V=-\beta\psi'_n(\beta)$ tends to $A_0$ by the same forest endpoints used in Annex O.10. Its negative deviation below $A_0$ tends uniformly to zero in these windows: in a fixed hidden box the centered excess $\beta(A-\min A)$ has nonnegative mean tending to $d_Ah_l/2$ on good boundaries; omit the bad boundaries, minima and other nonnegative action terms. Sum, then let fixed $l=L^j$ tend to infinity. Thus the absolute deviation of the mean energy density also tends to zero in logarithmic mean. Apply Markov's inequality to the sum of the two absolute deviations to choose a single sequence for both mean and variance.

For bounded Lipschitz fixed compact scalar tests $u_\alpha$, one has, under these selected Wilson measures,
\[
 \beta a^4\sum_\alpha\sum_{p\parallel\alpha}
             u_\alpha(x_p)s_p
 \ \longrightarrow\ \frac{A_0}{6}\sum_\alpha\int u_\alpha
 \quad\text{in }L^2 . \tag{27}
\]
Here $x_p$ may be the face center or any fixed placement within its lattice cell. We give an argument using conditional matrix variances. Work first with one plane $\alpha$ and $u\ge0$. At fixed $l$, condition on all visible links of the tiling. Fix the interior forest gauge as in Annex O.5; the trace defining each $s_p$ is invariant, and for each plaquette touching the hidden links we use its holonomy matrix $U_p$ in this gauge. Under its box conditional law the exact identity is
\[
 \mathbb E(s_p\mid\mathcal E)=
 \tfrac12\mathbb E(\|U_p-\mathbb E(U_p\mid\mathcal E)\|_{\rm HS}^2
                                   \mid\mathcal E)
       +\tfrac12\|\mathbb E(U_p\mid\mathcal E)-I\|_{\rm HS}^2 . \tag{28}
\]
Because only a lower bound is needed, one may choose the boundary gauge bringing good exterior data into the fixed near-flat chart. A change of base vertex frame conjugates the plaquette matrix and preserves both norms. Existence of such a frame for each good exterior suffices for the pointwise conditional inequality; the observable on its left is gauge invariant.

On that chart at fixed $l$, the conditional variance of the matrix $U_p$, multiplied by $\beta$, tends to the squared Hilbert–Schmidt size of its linearized fluctuation under the minimizing-Hessian Gaussian. Indeed write $U_p=U_{p,*}+\beta^{-1/2}D U_{p,*}y+O_l(\beta^{-1}|y|^2)$ in the rescaled coordinates. The fixed-box moment and chart-tail bounds justify this in $L^2$, uniformly over a small good chart. At flat data the sum of the half variances in (28) over all fluctuating plaquettes is $d_Ah_l/2$ in these Gaussian units: it is the expectation of the full quadratic action. Each plane contributes exactly $d_Ah_l/12$ by symmetry of the flat closed box, its boundary, and the measure on physical fluctuations. The gauge choice introduces no anisotropy in this conclusion: changing interior forest adds a vertex gradient to the linearized field and leaves the plaquette curls invariant; the induced Gaussian on curls is unchanged by the gauge-coordinate change with constant linear Jacobian. The plane sum varies continuously with near-flat boundary data, so it has this limit as the allowed distance to flat tends to zero after the weak-coupling limit.

Use (28) on the good boxes and drop the remaining nonnegative terms. Replacing $u$ by its value at the box anchor costs $O_{l,u}(a)$ in the expected absolute value of the scaled insertion by the local first-moment bound. The fraction of bad boxes on the support tends to zero in expectation at every fixed tolerance by the finite-collar good-boundary estimate. Conditional independence bounds the variance of the scaled sum minus its conditional mean by $C_{l,u}a^4$: the unscaled second moment per box is $O_{l,u}(\beta^{-2})$ and there are $O_{l,u}(a^{-4})$ contributing boxes. Visible-only plaquettes are conditional constants. Consequently the scaled nonnegative orientation sum has lower limit in probability at least $d_Ah_l\int u/(12l^4)$ after sending the tolerance to zero. Then let $l=L^j\to\infty$. Its actual expectation tends to $A_0\int u/6$ by translation/axis-permutation symmetry and the joint mean selection. The random variables have uniformly bounded moments of any fixed order by the closed-cube local energy bound and the $L^p$ triangle inequality. Their negative deviation from the limiting constant therefore tends to zero in $L^1$; the exact limiting expectation forces the positive deviation to do the same. Interpolation gives $L^2$ convergence. Splitting a signed test into its Lipschitz positive and negative parts and summing the six fixed planes gives (27).

For a plaquette in plane $(i,j)$ with complementary axes $\rho,\sigma$, average a smooth test over its vertices or over the centers of its four incident cubes. Taylor expand at the plaquette center. Both averages have the same constant and linear terms. Their difference is
\[
 \frac{a^2}{8}(\partial_i^2+\partial_j^2-\partial_\rho^2-\partial_\sigma^2) f
              +O_f(a^3).
\]
The error, after inserting it with the prefactor $a^2\beta$ in the sum over plaquettes, has $L^2$ norm $O_f(a)$ by the local second moments. By (27) the centered insertion of the displayed leading term times $a^2\beta$ tends to zero in $L^2$. Cube-center testing instead of cube-origin testing in (26) preserves that theorem, by (22) for the translated difference of the tests. Cauchy–Schwarz and polarization therefore prove
\[
 a^4\beta^2\operatorname{Cov}\!\left(a^4\sum_x f(x)w_a(x),
                                      a^4\sum_y g(y)w_a(y)\right)
       \longrightarrow A_0\int fg                                      \tag{29}
\]
on the single selected sequence, for the actual vertex-averaged Annex E source and all fixed smooth compact tests. The coefficients of the second-order derivatives sum to zero across the six planes, although centering alone already suffices for this variance result. The lower-vertex source has a first-order placement difference; (27) alone supplies no rate that removes it. At separated supports, (29) gives a vanishing *scaled* covariance. Quantitative control in unscaled physical units and the prescribed contact comparison are still outstanding.

## 9. The joint curvature-energy law at fixed lattice separations

Consider the joint-mean selection of §8.3, or any sequence $n,\beta\to\infty$ satisfying $\beta\mu(S)/V\to A_0$, the single-plaquette exponential moment bound uniformly, and divisibility by every fixed $l=L^j$ eventually. The following microscopic result needs no physical scale $a$. On the oriented positive edges of $\mathbb Z^4$ take the lattice curl $d$ into the six oriented plaquettes per site. Give both spaces their counting $\ell^2$ metric and let $P_\infty$ be the orthogonal projection in plaquette space onto the closure of the curls of finitely supported edge arrays. Let $G_p$ be the centered Gaussian anti-Hermitian Lie-algebra field with covariance $P_\infty(p,q)$ in each independent color, using the real Hilbert–Schmidt metric on $\mathfrak{su}(N)$. The Gaussian field exists on the countable index set by its consistent finite covariance matrices.

For every fixed finite list of plaquettes in lattice coordinates, including repetitions, the *actual* Wilson observables obey
\[
   (\beta s_p)_p\ \Longrightarrow\
     (\tfrac12\|G_p\|_{\rm HS}^2)_p
       \quad\text{with convergence of all fixed joint moments}. \tag{30}
\]
All limits in this assertion are taken with the displacements measured in fine lattice units held fixed.

**Proof.** Independently choose a uniform translate of the side-$l$ tiling in §7. For a plaquette touching a hidden link, use the interior forest gauge of §8.3 and write $\bar U_p=\mathbb E(U_p\mid\mathcal E)$ in that frame. At each good exterior a further boundary gauge puts the visible field into the fixed near-flat chart. One may choose such frames locally on the compact good set, choosing the first admissible chart in a finite cover. The change of frame after forest gauge acts at a plaquette base by a deterministic conjugation for fixed boundary data. All squared norms in (28) are invariant.

The sum of nonnegative terms
\[
 D_{l,n}=\frac{\beta}{2V}
 \mathbb E_z\sum_{p\ {\rm fluctuating}}
      \mathbb E\|U_p-\bar U_p\|_{\rm HS}^2
\]
tends to $A_l=d_Ah_l/(2l^4)$ for each fixed $l$. On good boundary data this is the linearized matrix-variance calculation of (28), summed over plaquettes and followed by shrinking the tolerance to flat. On bad boxes, Jensen and $\frac12\mathbb E(\|U_p-\bar U_p\|^2\mid\mathcal E)\le\mathbb E(s_p\mid\mathcal E)$ give uniform integrability in the required scaling from the local energy moments. The complementary sum
\[
 \frac{\beta}{2V}\mathbb E_z\sum_{p\ {\rm fluctuating}}
          \mathbb E\|\bar U_p-I\|_{\rm HS}^2
   +\frac{\beta}{V}\mathbb E_z\sum_{p\ {\rm visible}}\mathbb E s_p
       =\frac{\beta}{V}\mathbb E S-D_{l,n} \tag{31}
\]
has limit $A_0-A_l$. Here visible means that all four of the plaquette's links are visible. The averaged quantities are translation invariant when the same forest template is translated along with the grid. Nonnegativity and translation averaging bound each fixed root's expected squared scaled mean displacement, counted when fluctuating, by $2(A_0-A_l)+o_l(1)$. Axis invariance of the forest is unnecessary.

For the finite target list, with displacement diameter $b$, the probability that the entire list is in one box at distance at least $r$ from its boundary is at least $1-C(b+r+1)/l$ if this is positive. At fixed $l$, in a common good box frame, the conditional centered vectors $\sqrt\beta(U_p-\bar U_p)$ jointly approach the linearized Gaussian curl variables in that box as the weak-coupling limit is taken and the boundary tolerance goes to zero. To verify this, expand each plaquette matrix to first order at the minimizing connection; the $L^2$ Taylor remainder after multiplication by $\sqrt\beta$ is $O_l(\beta^{-1/2})$ using the fixed-box chart and fourth moment. The rescaled coordinates converge jointly in moments to a Gaussian with the inverse minimizing action Hessian, and at the shrinking boundary tolerance both the linear derivatives and the Hessian approach their flat values. The finitely many possible root locations at fixed $l$ cause no loss of uniformity.

At flat data the Wilson quadratic form is $\|dA\|^2/2$ per independent color. Its induced centered Gaussian on the plaquette curls has covariance $P_{\rm box}$, the orthogonal projection onto the range of the hidden-edge curl map with the boundary edges zero. Indeed the density on that image, after dividing out the kernel of gradients or choosing the forest, is a constant times the standard Gaussian density on the image. Extending hidden edge potentials by zero adds no exterior plaquette curl because all incident plaquettes belong to the closed box. If a radius-$r$ cube containing the target is deep inside the box, the three curl ranges are nested and $P_r\le P_{\rm box}\le P_\infty$ as positive operators, where $P_r$ is the corresponding fixed inner-cube projection. The increasing projections $P_r$ converge strongly to $P_\infty$ by density of the finite-support curls. Cauchy–Schwarz for the positive difference bounds each target entry of $P_\infty-P_{\rm box}$ by the corresponding diagonal errors for $P_\infty-P_r$. Hence the joint Gaussian law of the fixed target tends to the claimed limit uniformly in these deep box placements.

Adding back the conditional mean to form $\sqrt\beta(U_p-I)$ costs $O_b((A_0-A_l)^{1/2})$ in expectation of the norm, apart from the discarded visible/boundary placements. For the energies, use $|\|v+h\|^2-\|v\|^2|\le2\|v\|\|h\|+\|h\|^2$ and uniform second moments. For bounded continuous tests of the finite list the discarded placements cost at most twice the test bound times their probability. First take the weak-coupling limit at fixed $l,r$ and shrink the boundary tolerance, then take $l\to\infty$, and finally $r\to\infty$. This proves the joint weak convergence of the gauge-invariant energies. The uniform local exponential moments imply uniform integrability of every fixed product and give the moment statement in (30).

The argument covers marks made from finitely many *based* plaquettes in common frames, such as the vertex clover. Changing the chosen base corner changes neither the action nor the flat derivative of a positively oriented curl: the conjugating path is identity at flat and derivatives of its conjugation of identity vanish. For negative orientations the sign reverses. For each corner convention separately the proof of (31) thus gives the same vanishing local scaled-mean estimate; finitely many are permitted simultaneously. In the single good box choose frames for all matrices consistently, and apply continuous polynomial contraction there. In particular $\sqrt\beta C_{\mu\nu}$ at a vertex has, in this common calculation, limiting Hermitian curl $(4i)^{-1}\sum_{\sigma,\tau}\sigma\tau\,G_{\sigma\mu,\tau\nu}$ with the corresponding signed oriented curls based there. The **gauge-invariant** products $\beta\operatorname{Tr}(C_A C_B)$ jointly converge in moments at fixed vertices to the corresponding products of Gaussian clover curls. Their uniform integrability follows from $\|\sqrt\beta C_A\|^2\le C\sum_{p\text{ incident}}\beta s_p$. This identifies physical trace products. It does not assert that untransported matrices at different bases have a gauge-independent joint law.

For oriented plaquette energies, Gaussian fourth moments give the explicit microscopic covariance
\[
 \lim\beta^2\operatorname{Cov}(s_p,s_q)
       =\frac{d_A}{2}|P_\infty(p,q)|^2 . \tag{32}
\]
For the lower-vertex scalar the sum over the six plaquettes at each end gives a nonnegative limiting kernel on $\mathbb Z^4$ of total mass $A_0$. Indeed by the projection identity its row sum is $(d_A/2)\sum_{p\text{ at }0} P_\infty(p,p)=3d_A/2$. In Fourier variables the curl is exterior multiplication by the vector $(e^{it_j}-1)_j$, hence has rank three at every nonzero momentum. Its projection has trace three almost everywhere; axis symmetry gives $P_\infty(p,p)=1/2$. The same sum holds for the cube scalar, since the spatial sums of the averaging weights of each plane are one. The limiting signed or positive kernel at fixed displacement must be distinguished from any uniform tail bound for the finite-cutoff interacting kernels.

### 9.1 Tightness of squared covariance tails for the cube representative

Assume in addition $\beta^2\chi=O(1)$, as holds on the sequence of §8.2. For each fixed $l$, let $R_l$ be the covariance kernel of the conditional means of $H_x$ given all visible links, averaged over tiling offsets. Then
\[
   \lim_{l=L^j\to\infty}\limsup_m\beta_m^2 (R_l)_{00}=0. \tag{33}
\]
Indeed for one root plaquette the first term of (28), multiplied by $\beta$, converges in the same iterated limits in probability to $d_A P_\infty(p,p)/2=d_A/4$: discard the rare boundary placements, then use the fixed-box Gaussian calculation and projection comparison above. On visible-only placements set this first term to zero. The remaining nonnegative conditional mean is small in $L^1$ by (31). The entire scaled conditional mean has uniformly bounded higher moments by conditional Jensen and the local energy estimates. Thus it converges in $L^2$ to $d_A/4$ in this iterated sense. Sum the four incident faces per orientation with their factor $1/4$ to obtain convergence of the cube conditional mean to a constant. This yields (33).

The single-update covariance decomposition gives $0\le R_l\le C^H\le\chi I$. Its difference from $C^H$ vanishes outside distance $l+4$ in fine lattice units. Therefore
\[
 \lim_{M\to\infty}\limsup_m\sum_{d_{\infty,n_m}(0,z)>M}
     |\beta_m^2 C^H_{0z}|^2=0,\qquad
 \beta_m^2 C^H_{0,\cdot}\longrightarrow K^H
                    \ \text{strongly in }\ell^2(\mathbb Z^4). \tag{34}
\]
For the first assertion choose an allowed fixed $l$ and $M\ge l+4$. The squared tail is bounded by $(\beta^4R_l^2)_{00}\le (\beta^2\chi)\beta^2(R_l)_{00}$. Now use (33). For the second, identify the torus displacements with a centered fundamental cube, extend the array by zero, and use (30) on finite displacements together with this uniform squared-tail bound. Here $K^H$ is the cube-placement average of (32).

There is also a signed smooth-annulus conclusion at every growing intermediate scale. Let $r_m\to\infty$ with $r_m/n_m\to0$ and let $\varphi$ be a smooth compactly supported function on $\mathbb R^4$. Then
\[
   \sum_z\beta_m^2 C^H_{0z}\,\varphi(z/r_m)
       \ \longrightarrow\ A_0\varphi(0). \tag{35}
\]
Indeed the rescaled cube Fourier susceptibilities are uniformly bounded by (22), and for **every** sequence of torus momenta tending to zero they tend to $A_0$ by the fixed-box plane-wave lower bound in §8.2. Fourier inversion on the torus now applies. More explicitly the Fourier coefficients of the periodized function $z\mapsto\varphi(z/r_m)$ are the alias sum $r_m^4 n_m^{-4}\sum_{h\in\mathbb Z^4}\widehat\varphi(r_m(q+2\pi h))$, with the convention $\widehat\varphi(k)=\int e^{-ikt}\varphi(t)\,dt$. The total absolute weight is uniformly bounded and the weight outside $|q|\le B/r_m$ tends uniformly to zero as $B\to\infty$ by rapid decay and $r_m/n_m\to0$. The sum of all weights is $\varphi(0)$ for large $m$. This proves (35), including its vanishing for annular smooth tests. Neither (34) nor (35) gives an absolute $\ell^1$ tail estimate for all finite-cutoff covariance entries or a physical decay rate.

## 10. An explicit growing microscopic window

On the jointly selected compatible sequence, (32) admits a uniform error $O((\log\beta)^{-1/2})$ for each pair of plaquettes with shortest displacement of sup norm at most $n/3$. The selection in §§8.2–8.3 can be made with the quantitative tolerances below. The proof uses a box of side comparable to $\log\beta$, retaining the normalized compact Wilson integration. All constants in this section may depend on $N,L$.

### 10.1 Elementary estimates on one compact box

Let $b=m^{1/4}$, $B=m^{1/2}$, $n=2L^m$, and choose the largest power $l$ of $L$ at most $\log b$. Uniformly for $b\le\beta\le B$ and sufficiently large $m$, $c\log\beta\le l\le\log\beta$. On a closed side-$l$ box join a spanning tree of its boundary graph to the interior forest of §7. This gives a full spanning tree: each interior component attaches to one boundary vertex. Fix the boundary tree using visible gauge transformations and the interior forest in the conditional Haar integral. The resulting conditional law has product Haar reference measure on $h_l$ free links, as in Annex O.5.

In full tree gauge any remaining link is a tree-based loop with at most $C l^4$ steps. The word of any closed lattice path of length $J$ in the box can be commuted into coordinate order with at most $J^2$ elementary square interchanges, then cancelled. Interchanging two adjacent steps in distinct axes stays inside the box: the fourth square vertex takes one coordinate from each of the other vertices and lies in the same coordinate rectangle. Cancelling adjacent inverse steps also stays in the box. Each interchange changes the holonomy by a conjugate of a unit plaquette (or its inverse), possibly after cyclic change of base. Thus unitarity and the product triangle inequality bound every tree-gauge link deviation by $Cl^8\max_p\|U_p-I\|_{\rm HS}$ over all box faces. The linear additive version gives $\max|v_b|\le C l^8\max |(dv)_p|$ for a zero-boundary, zero-forest tangent field. In particular the flat action Hessian $G$ satisfies
\[
       c l^{-20} I\le G\le C I . \tag{36}
\]
The lower estimate counts $O(l^4)$ coordinates in the squared Euclidean link norm. The upper estimate follows from bounded-degree incidence.

By the closed-cube energy moment, all faces of the sampled box have $\|U_p-I\|_{\rm HS}\le\beta^{-1/4}$ except on an event of probability $C l^4e^{-c\sqrt\beta}$. On this event the tree bound proves a **visible-only** condition: in the boundary tree gauge all fixed box boundary links are within $\zeta=C l^8\beta^{-1/4}$ of identity. The implication uses a possible full tree completion only to show the boundary estimate; the resulting boundary gauge on its vertices depends solely on its tree links. Thus this same probability bounds the bad boundary event, regardless of the as-yet unintegrated interior.

Write $A$ for the actual box energy summing the fluctuating plaquettes. For good boundary data the trial configuration with every free link identity gives $A_*\le C l^4\zeta^2$ at a minimum. Conversely the tree estimate gives $\max_b\|U_b-I\|\le C l^8(\sqrt A+\zeta)$ for all configurations with this boundary: the visible-only faces have link products within $C\zeta$ of identity. Consequently every minimizer is within $C l^{10}\zeta$ of identity. Put $r=c_0 l^{-24}$ and use exponential coordinates at identity in every free link. On the product chart $|u_b|<2r$ the Hessian in Euclidean link coordinates differs from $G$ by $C(r+\zeta)$ in operator norm. Each row has a bounded number of nonzero link blocks (two variables must occur in a common plaquette), each having a uniformly bounded derivative in its own finite set of arguments. In view of (36) the Hessian there is at least $c l^{-20}I$. This convex chart contains every minimizer in its inner half. Off the product chart of radius $r$, the tree estimate gives $A-A_*\ge c l^{-64}$ at large $\beta$, since $r^2/l^{16}$ is of that order whereas $l^4\zeta^2=o(l^{-64})$. Hence the box minimum is unique. At that minimum $u_*$, its Hessian $G_*$ satisfies $\|G_*-G\|\le C l^{10}\zeta$ by the same sparse estimate and $\|G_*^{-1}-G^{-1}\|\le C l^{50}\zeta$.

For precision the Gaussian approximation needed below holds with absolute error $O(\beta^{-c_*})$ for some fixed $c_*>0$ for the finitely many moment types used below, uniformly at good boundary data, even in this growing dimension. Here are details of the truncation. Write $D=d_A h_l=O(l^4)$, $y=\sqrt\beta(u-u_*)$. On $|y|\le\beta^{1/32}$, Taylor expansion gives
\[
 \left|\beta(A-A_*)-\tfrac12 y^\top G_* y\right|
       \le C l^4\beta^{-1/2}|y|^3.
\]
The product Haar density, relative to its value at $u_*$, has log bounded by $C l^4\beta^{-1/2}|y|$ there (smooth positive single-link chart densities). Thus the two unnormalized densities differ by a relative $O(\beta^{-1/3})$ on this ball for all sufficiently large $\beta$. For $|y|>\beta^{1/32}$ inside the radius-$r$ product chart the exact excess action is at least $c l^{-20}|y|^2$ in rescaled units. The ratio of this tail to the inner integral is bounded by $\exp[-c\beta^{1/16}l^{-20}+C D\log(2+l)]$, by Gaussian integration and the lower bound from $y\in[-1,1]^D$. The density and action integral on this latter cube is at least $e^{-CD}$ after removing $\exp(-\beta A_*)$ and $\beta^{-D/2}$. Uniform upper bounds on the product chart density cost at most $e^{CD}$. Off the radius-$r$ chart compact Haar mass at most one and the gap give a relative bound $\exp[-c\beta l^{-64}+(D/2)\log\beta+CD]$. These tails remain negligible under any fixed power of the bounded plaquette variables times $\sqrt\beta$, or of $\beta(A-A_*)$ (the latter is bounded by $C\beta l^4$). For the Gaussian the $y$-moments of fixed order are polynomial in $l$ by (36). These estimates justify relative normalization and fixed polynomial moment comparisons, with the absolute error asserted above after allowing those polynomial factors. For example one may decrease $c_*$ below $1/16$ to cover the Hessian perturbation and the finite-degree Taylor remainders in all the uses below.

Applied to $\beta(A-A_*)$ through its second moment this gives the flat Gaussian counterparts to absolute error $O(\beta^{-c_*})$, including in the variance after another possible decrease of $c_*$ to absorb a polynomial-in-$l$ first moment. The Gaussian mean and variance of its quadratic energy are both $d_Ah_l/2$. Applied to $\sqrt\beta(U_p-\bar U_p)$ the constant term of the matrix cancels. Expand at $u_*$ with error $O(\beta^{-1/2}|y|^2)$ on the chart; the plaquette is a product of four smooth link functions. Its derivative differs from the flat derivative by at most $C l^{10}\zeta$. The Gaussian covariance of these derivatives differs from that for $G^{-1}$ by at most $C l^{50}\zeta$ times an additional fixed polynomial in $l$, which is $O(\beta^{-c_*})$. Gaussian moments and these bounds give absolute errors $O(\beta^{-c_*})$ for the joint moments through degree four of any one or two such centered plaquette matrices and their conjugates, uniformly in their relative positions in the box. For different boxes the conditional law factors. On bad exteriors all unconditional contributions needed here are negligible by their exponentially small probability, conditional Jensen, the local energy moments (or the trivial polynomial bound in $\beta,l$ on compact energies), and Hölder. This proves the required uniform estimates without a dimension-independent compact Laplace theorem.

### 10.2 Selecting the error rate and comparing varying plaquette pairs

Use the above tiling at each $\beta$ in the window. Good box excess means and variances from §10.1 give
\[
 \frac{\beta\mu S}{V}\ge A_l-O(\beta^{-c_*}),\qquad
 \frac{\beta^2\operatorname{Var} S}{V}\ge A_l-O(\beta^{-c_*})
\]
by summing nonnegative conditional excess energies and independent conditional variances. Since $A_0-A_l=O(1/l)$, both lower deficits relative to $A_0$ are $O(1/\log b)$. Integrating the two derivatives of the forest pressure as in Annex O.9–O.10 gives signed logarithmic means $A_0+O(1/\log b)$ on $[b,B]$: endpoint errors are $O(1+\log(1+B)/V)$ and $\log(B/b)=\log b$. Combining with the lower bounds makes the normalized *absolute* errors $O(1/\log b)$. We can select one common point at which
\[
 \left|\beta\mu S/V-A_0\right|+
 \left|\beta^2\operatorname{Var}S/V-A_0\right|\le C/\log\beta . \tag{37}
\]
If the maximal-function selection used for exponential moments in Annex O is also required, the same rate is available. Extend the absolute susceptibility error by zero outside the log window and apply the weak $(1,1)$ inequality at threshold $C'/\log b$. Its excluded measure is a small fraction of the window length if $C'$ is chosen large. Apply Markov's inequality to the mean-energy error with the same threshold, and choose the common point in the middle half of the window. This requires no new trajectory matching beyond §8.2.

At the selected point, (31) and §10.1 imply for any fixed root
\[
 \mathbb E_{z,\mu}|\sqrt\beta(\bar U_p-I)|^2
          {\bf1}_{p\ {\rm fluctuating}}\le C/\log\beta .
\]
On a visible-only root use $\sqrt\beta(U_p-I)$ as the conditional-mean displacement; its squared expectation, with this event, satisfies the same bound by (31). This convention gives zero centered fluctuation on visible-only roots. In either case, the full scaled matrix, its conditional mean displacement and its conditional centered fluctuation have uniformly bounded $L^6$ norms under the joint law of offsets and configurations by the energy estimate and conditional Jensen. Replacing a full matrix by its centered version in a joint product of degree at most four therefore costs at most $C(\log\beta)^{-1/2}$ per factor: use Hölder with $L^2$ for the replaced mean and $L^6$ for each of at most three remaining factors. Scalar energies use matrix squared norms and retain their original gauge-invariant meanings. By §10.1 the resulting centered moments are given, up to $O(\beta^{-c_*})$, by the flat independent-box Gaussian moments. Only the one or two participating boxes need be good. Their translated finite-volume construction agrees locally with the infinite periodic tiling on a pair of roots at shortest displacement at most $n/3$, since $l\ll n$.

To compare to the free lattice covariance without an unspecified projection convergence rate, form the infinite direct sum $P_{z,l}$ of the independent-box curl projections at offset $z$, extended by zero on exterior faces. Its range is contained in the closure defining $P_\infty$: finite sums of finite-box curls give a dense subset of that direct sum. Thus $0\le P_\infty-P_{z,l}\le I$. Its offset-averaged sum of diagonal entries at one site is $3-h_l/l^4=O(1/l)$, using the flat rank-three symbol and the dimension of the hidden physical curl space. Each plane's deficit is nonnegative. Positive-matrix Cauchy–Schwarz, then offset Cauchy–Schwarz, give
\[
  \mathbb E_z |(P_\infty-P_{z,l})(p,q)|\le C/l \tag{38}
\]
for any two roots, uniformly in their locations, including roots in different boxes. All entries of both projections have modulus at most one, so Wick second and fourth moments vary by at most $C/l$ after offset averaging. This also controls the offset variation of diagonal factors in an uncentered fourth moment. Subtracting the actual means afterwards yields
\[
 \sup_{d_{\infty,n}(p,q)\le n/3}
 \left|\,\beta^2\operatorname{Cov}(s_p,s_q)
            -\tfrac{d_A}{2}|P_\infty(p,q)|^2\,\right|
       \le C(\log\beta)^{-1/2}. \tag{39}
\]
Here $P_\infty(p,q)$ uses the shortest relative lift. The same estimate holds for finite linear combinations of such energies at bounded nearby offsets in the distance range with the corresponding fixed margin. For length-four invariant products of the local clover matrices in paired traces, discard offsets on which either fixed vertex stencil is cut between boxes. Their offset fraction is $O(1/l)$; the unconditional gauge-invariant Wilson product has a uniform absolute moment independent of the offset, and the comparison Gaussian products have uniform moments as well. On each remaining offset use one common forest frame per vertex stencil, the same frame when both lie in the same box. Cyclic base choices are handled as in §9 (apply (31) to each needed base convention). Constants may depend on that fixed stencil. This does not bound the covariance by the right order at arbitrarily large $r$; (39) is an **absolute** error.

In particular, using the standard lattice curl projection estimate $|P_\infty(p,q)|\le C(1+r)^{-4}$ with $r$ the fine lattice displacement, (39) gives a uniform Wilson bound $C(1+r)^{-8}$ for the rescaled plaquette covariance whenever $r\le(\log\beta)^\kappa$ with any fixed $0<\kappa<1/16$. On that entire window its error relative to the envelope $(1+r)^{-8}$ tends to zero. One way to obtain the projection estimate is a smooth dyadic partition of its Fourier symbol away from its only singularity at zero. On a frequency annulus of radius $t$ its derivatives of order $j$ are $O_j(t^{-j})$ since its numerator and denominator vanish to order two, with the denominator comparable to $|k|^2$. Integration by parts gives $C_M t^4(1+t r)^{-M}$ per annulus. Sum with $M>4$, treating the remaining smooth symbol by repeated integration by parts. Consequently the physical two-point kernel of the bare scalar satisfies the ultraviolet annular bound of (CP.25), with right side $C\beta^{-2}h^{-4}$, for $a\le h$ and $2h/a$ inside this explicit cutoff window (allowing a fixed placement margin). A fixed positive physical separation is outside the window along the stopped trajectory. The annular estimate on the intervening scales and the prescribed contact estimate remain open.

## 11. A prescribed-coupling microscopic window from free and pinned box pressure

The preceding selection can be removed for the microscopic mean and covariance results (30), (32), (39). Here is one quantitative version for compatible growing tori. Fix $\epsilon_*=10^{-6}$, let $\beta\to\infty$, and assume that $l=L^{\lfloor\epsilon_*\log_L\beta\rfloor}$ divides the dimensionless torus side $n$, with $n\ge3l$ (and even $n$ for the local energy bound as above). These arithmetic conditions hold eventually on the stated compatible trajectory with $a=L^{-K}\ell_0$ and $\beta=O(1+K)$. The estimates below treat the Wilson coefficient as given; they do not identify a renormalization trajectory.

**Polynomial box size.** The proof of §10.1 remains valid with this $l$ in place of $\log\beta$, with all the required absolute errors $O(\beta^{-1/32})$. To check the rates, for a nearby coefficient $t\beta$ with $1/2\le t\le2$ keep $l$ fixed. All estimates below are unchanged up to constants. The dimension satisfies $D\le C_N l^4$. The good-boundary minimizer has sup distance $O(l^{18}\beta^{-1/4})\ll l^{-24}$, and the gap outside the chart remains $cl^{-64}$. The two tail exponents have leading negative terms of orders $\beta^{1/16}l^{-20}$ and $\beta l^{-64}$, whereas the positive loss is $O(D\log\beta)$. Both tails still beat all fixed powers of $\beta$. The local exponent error is at most $Cl^4\beta^{-13/32}$ on the truncated $y$-ball; the Haar log-density error is smaller. The centered-minimizer Hessian inverse differs from the flat one by $Cl^{58}\beta^{-1/4}$, and plaquette derivatives differ by $Cl^{18}\beta^{-1/4}$. For the finitely many moment comparisons one needs the centered Gaussian $y$-moment bound $(\mathbb E|y|^j)^{1/j}\le C_j l^{12}$ from (36) and $D\le Cl^4$. For instance squared quadratic-energy and fourth linear-plaquette moments are bounded using $C l^{8}(1+|y|^8)$; the same polynomial majorizes Taylor-quadratic remainder insertions after removing their explicit $\beta^{-1/2}$ factor on the truncated ball (the energy cubic term has coefficient at most $Cl^4$). The resulting moment factors are at most $C l^{104}$, the factors for squaring a first energy moment to get the variance are at most another fixed $Cl^{8}$ when the moment error is already small, and multiplying by $Cl^{60}$ for coefficient comparisons is harmless. Even a loss $Cl^{500}$ times $\beta^{-1/8}$ is $O(\beta^{-1/32})$. This checks the fourth-moment Gaussian comparison, the normalized integral approximation, and the mean/variance of the quadratic energy. For free or identically pinned boxes the same estimates apply with minimizer exactly identity. A free open box only requires tree gauge and the identical square-filling proof of (36), with no visible boundary variables.

**Box bracketing.** Partition the torus vertices into disjoint arrays of $l^4$ sites. Each is an open cubical complex of side $l-1$ fine *edges*. This comparison uses those vertex-disjoint boxes; the conditional updates in (31) continue to use side-$l$ edge boxes sharing boundaries. Gauge-fix an intra-box spanning tree consisting of a boundary spanning tree and an interior forest attached to that boundary. Tree integration is an exact Haar change of variables on the whole graph, also for interbox links by conditional left/right Haar invariance. Different box roots can be kept independent. Dropping all plaquette actions that cross from one vertex array to another gives an upper bound by a product of free open-box integrals. For a lower bound pin every interbox link and every remaining boundary edge of each box to the identity ball of radius $\beta^{-2}$. There are at most $C V/l$ such independent Haar variables so that the log probability is at least $-C(V/l)\log\beta$. Every cross-box plaquette has just pinned links, including tangential edges in the array boundaries or tree identities. Its action is $O(\beta^{-4})$. Inside the arrays replacing the boundary pins by identities changes $\beta$ times the sum of all action terms by at most $CV\beta^{-1}/l$, using bounded single-link Lipschitz constant of the plaquette action and the bounded incidence count. The remaining factors are independent Dirichlet box integrals. All of these bounds apply with $t\beta$ for $1/2\le t\le2$, keeping the same array and using radius $\beta^{-2}$.

For a free array let $h^F=4(l-1)l^3-l^4+1$ be the number of free tree-gauge link variables. Its flat Hessian $G^F$ has (36) and the unique flat tree-gauge minimizer. Its Dirichlet counterpart is obtained simply by setting the remaining boundary coordinates to zero. Thus $G^D$ is a principal compression of $G^F$ of codimension $O_N(l^3)$ in real Lie coordinates. The determinant ratio is a Schur complement determinant whose eigenvalues lie between $c l^{-20}$ and $C$ (its inverse is a principal compression of $(G^F)^{-1}$). The logs of the two Gaussian determinants consequently differ by at most $C l^3\log(2+l)$. Haar chart and Gaussian normalization constants per link are fixed constants, giving $O(l^3)$ additional discrepancy. The per-site errors of the two Laplace approximations are bounded by $C\beta^{-1/32}$. It follows with a constant $c_l$ independent of $t$ from the free Gaussian determinant that
\[
 \left|\psi_n(t\beta)+A_l^F\log(t\beta)-c_l\right|
 \le C\{\log\beta/l+\beta^{-1/32}\},\quad
 A_l^F=d_Ah^F/(2l^4)=A_0+O(l^{-1}) . \tag{40}
\]
Here $c_l$ may depend on $l$ and $N$, and $\psi_n=V^{-1}\log Z_n$. The needed cancellation occurs in pressure *differences* at the same box side.

By convexity bound $\psi'_n(\beta)$ by the two secants at $(1\pm h)\beta$, where $h=\beta^{-\epsilon_*/3}$. Using (40) and $\log(1\pm h)=\pm h+O(h^2)$ gives the actual prescribed-coupling estimate
\[
 \left|\beta\mu_{n,\beta}S/V-A_0\right|\le C\beta^{-\epsilon_*/3}. \tag{41}
\]
No control of the pointwise second derivative by secants is used.

Return to the side-$l$ edge boxes of (31). The conditional estimates of §10.1 in their polynomial-size version give $D_{l,n}=A_l+O(\beta^{-1/32})$. Together with (41) and $A_0-A_l=O(l^{-1})$, (31) bounds the squared conditional-mean displacement per root by $C\beta^{-\epsilon_*/3}$. The $L^2$–$L^6$ replacement, independent Gaussian box moment comparison and (38) now prove at this given coupling
\[
 \sup_{d_{\infty,n}(p,q)\le n/3}
  \left|\beta^2\operatorname{Cov}(s_p,s_q)
                -\frac{d_A}{2}|P_\infty(p,q)|^2\right|
       \le C\beta^{-\epsilon_*/6}. \tag{42}
\]
The stated local energy moments hold uniformly on this geometry because $\log(1+\beta)/V$ is bounded; the polynomial lower bound on $n$ suffices asymptotically. For $R_\beta=\beta^{\epsilon_*/100}$, multiplying (42) by $(1+r)^8$ for $r\le R_\beta$ still leaves a vanishing error. The bare Wilson CP.25 annular bound therefore holds for $2h/a$ up to this *explicit* $R_\beta$ with a fixed stencil margin, at the given coupling. The exponent is deliberately conservative. The participating box sizes, determinant estimates and energy saturation do not yield control out to a fixed positive physical separation along $a=L^{-K}\ell_0$, $\beta=O(1+K)$.

In particular (30) and the stated clover trace-product limits hold on this prescribed-coupling geometry, since their fixed-order convergence needs only the mean limit (41), the local moments and fixed-box comparisons. For the quantitative displayed pair error only moments through degree four are compared uniformly on the growing boxes. Formula (41) concerns a first derivative; (22) and (23) still involve the actual full pointwise susceptibility, which (40) does not determine. The white-noise contact-scale covariance results on a susceptibility-selected sequence and the second-moment tail conclusion (34) retain their respective additional hypotheses.

## 12. Positive time-slab spectra and the physical-separation criterion

Consider one time axis and a real spatial array $h$. For each time slab $t$ let $X_h(t)=\sum_{\mathbf x}h_{\mathbf x}(H_{(t,\mathbf x)}-\mu H_{(t,\mathbf x)})$ and $J_h(t)=\mu[X_h(0)X_h(t)]$. On the finite Wilson torus one has
\[
 J_h(t)=\int_{[0,\infty]}
       (e^{-(t-1)E}+e^{-(n-t-1)E})\,d\nu_h(E)\quad(1\le t\le n-1),
 \qquad \nu_h\ge0 . \tag{43}
\]
For clarity this statement is about slabs, with a one-step displacement in each exponential. Equal-time variance is considered separately. A general strictly local transfer insertion need not have the required endpoint symmetry; the closed cube's four face weights have it.

Indeed the one-step pure gauge Wilson transfer $T$ is positive and self-adjoint on the gauge-invariant Hilbert space of a spatial slice. In temporal gauge its time-like factors before gauge projection are tensor products of convolution by the positive-type central function $\exp(\beta\operatorname{ReTr}U)$, whose character coefficients are nonnegative by expanding the exponential of the fundamental and conjugate characters. Splitting the spatial action in half gives a real positive multiplication on either end, and integrating temporal links implements the global product of local gauge projectors. These operations preserve operator positivity. The kernels on a finite slice are bounded and Hilbert–Schmidt. The operator $K_h$ made by inserting the centered one-slab observable in that same kernel is self-adjoint by reflection exchanging the endpoints and reversing the temporal links. The trace of $T^n$ gives the partition function in these units. For the transfer construction see [Lüscher, *Construction of a selfadjoint, strictly positive transfer matrix for Euclidean lattice gauge theories*](https://doi.org/10.1007/BF01614090).

In an eigenbasis of $T$ with eigenvalues $\lambda_i$, expand
\[
 J_h(t)=\operatorname{Tr}(K_h T^{t-1}K_h T^{n-t-1})/\operatorname{Tr}(T^n).
\]
An explicit positive measure in (43) puts weight $\lambda_i^{n-2}|(K_h)_{ij}|^2/\operatorname{Tr}(T^n)$ at $E=\log(\lambda_i/\lambda_j)$ for each ordered pair with $\lambda_i>\lambda_j>0$. Include half of the same weight on **all ordered pairs** with $\lambda_i=\lambda_j>0$ at zero. If one works on a space with null modes, $\lambda_i>0=\lambda_j$ contributes the same weight at infinity, only at the endpoint lags $1,n-1$ (set $e^{-0\cdot\infty}=1$); pairs both zero contribute nothing for $n\ge4$. This verifies (43) without requiring a zero ground-state degeneracy or an infinite-time limit. The parameter $E$ is a finite-temperature eigenvalue difference in lattice units.

For a normalized spatial constant $h=n^{-3/2}$ the nonnegative kernel is $J_h(t)=\sum_{\mathbf x} C^H_{0,(t,\mathbf x)}$. At zero, $J_h(0)\ge0$ as well. On the susceptibility-selected sequence its scaled total mass tends to $A_0$, and its Fourier transforms at *all* sequences of temporal momenta tending to zero tend to the same $A_0$ by §8.2. The one-dimensional measures $\beta^2 J_h(t)$ are therefore tight in lattice-distance units. To see this directly, average $1-\cos(qt)$ for all discrete positive $q\le C/M$ with a sufficiently large numerical $C$. For $M\le d_{\mathbb Z/n}(0,t)\le n/2$ the average is bounded below by a positive constant whenever $n/M$ is sufficiently large, by the finite geometric-series bound. Thus the tail is bounded by the largest difference of the zero and near-zero Fourier transforms on this range. Send first $n\to\infty$, then $M\to\infty$. Nonnegativity here is for the spatially integrated slice covariance. Cancellation may still occur among the terms in a slice.

**A finite-difference criterion.** Write $\widehat J_h(q)=\sum_t e^{iqt}J_h(t)$ and
\[
 D_h(q)=\tfrac32\widehat J_h(0)-2\widehat J_h(q)
                         +\tfrac12\widehat J_h(2q)
       =\sum_t J_h(t)(1-\cos(qt))^2\ge0 . \tag{44}
\]
The identity automatically cancels the equal-time contact and the quadratic term of a momentum polynomial. Suppose for given separated physical times and every spatial profile needed in the test that throughout $|q|\le C/R$, with $R$ proportional to their separation in lattice units, one can bound $D_h(q)\le M_a\|h\|_2^2 R^{-4}$. Assume $n/R$ sufficiently large. The average of $(1-\cos(qt))^2$ is bounded below for $d_{\mathbb Z/n}(0,t)\ge R/2$ by Jensen and the same geometric series after increasing $C$. Hence
\[
 \sum_{d(0,t)\ge R/2}J_h(t)\le C M_a\|h\|_2^2 R^{-4},
 \qquad
 \sup_{d(0,t)\ge R}J_h(t)\le C M_a\|h\|_2^2 R^{-5}. \tag{45}
\]
The last step uses the monotone decrease of each symmetrized exponential in (43) up to $n/2$, also covering a zero-energy atom. For different real profiles $h,k$, the transfer trace and Hilbert–Schmidt Cauchy–Schwarz give $|J_{h,k}(t)|\le[J_h(t)J_k(t)]^{1/2}$. A bounded physical spatial profile has $\|h\|_2^2=O(a^{-3})$ at each time and the two time sums cost $O(a^{-2})$ for fixed supports. Thus (45) with $R\asymp a^{-1}$ gives an $O(M_a)$ physical separated covariance. Compact disjoint supports can be partitioned into finitely many pairs separated in some coordinate; use this test along the corresponding axis. This is an explicit sufficient **input** at physical frequencies for the symmetric cube representative. The present estimates do not supply the displayed fourth-order rate there. Chessboard alone gives a total spectral mass-in-time bound $\sum_t J_h(t)\le\chi\|h\|_2^2$, by (22) applied to the same $h$ repeated at every time and stationarity.

For comparison, a massive positive transfer channel can evade all current microscopic error rates. This is a check on the inference from spectral information, not an assertion about Wilson gauge theory. On a fixed physical four-torus, augment a law by an independent standard nearest-neighbor real Gaussian scalar with inverse covariance $-\Delta_{\rm lat}+a^2 I$, and include the nonnegative local term $c_a(\phi_x+1)^2$ in its **actual** bare-$\beta$ score, with $c_a=a^2/(\log(1/a))^2$. The additional density is proportional to $\exp[-\beta c_a\sum_x(\phi_x+1)^2]$. At $\beta\asymp\log(1/a)$ its covariance is $G=(-\Delta_{\rm lat}+a^2+2\beta c_a)^{-1}$ and $1+\mathbb E\phi_x=a^2/(a^2+2\beta c_a)$. The centered score covariance equals $c_a^2(4(1+\mathbb E\phi_x)^2G_{xy}+2G_{xy}^2)$, nonnegative entrywise as well as reflection positive for the scalar site field. Its scaled zero-mode contribution is $O(a^2/(\log(1/a))^2)$ since $G_{xx}=O(1)$ and $\sum_y G_{xy}=(a^2+2\beta c_a)^{-1}$. The diagonal microscopic contribution in $\beta^2$ units is $O(a^4/(\log(1/a))^2)$. Yet on two nonnegative nonzero, physically separated smooth bumps the linear $G$ term contributes order $a^{-2}/(\log(1/a))^4$. For example $a^6\sum_{x,y}f(x)G_{xy}g(y)$ converges to the positive massive continuum Green form by discrete Fourier inversion on the fixed physical torus (smooth Fourier coefficients control the tails). These statements concern a different local model with a genuine single-pole channel. They isolate the missing infrared spectral weight bound without assuming that such a pole is present in the Wilson scalar.

The conditional box covariance already meets the order-four momentum test. For the translation-averaged $B$ of (16), its temporal symbol at each spatial momentum is a trigonometric polynomial of degree at most $r=C(k+1)(l+2)$ by finite propagation. It has modulus at most $C\beta^{-2}k^2l^4$ on the torus momentum grid by (16); for the cube placement the same proof of (16) applies since each plaquette coefficient is an average over four neighboring cubes. The ordinary Bernstein inequality for the derivative of a trigonometric polynomial and distance $\pi/n$ to the nearest grid point give a continuous sup bound at most twice the grid bound when $\pi r/n<1/2$. The symbol for a fixed real spatial $h$ summed against $|\widehat h|^2$ is even in temporal momentum: reversing time alone permutes the plaquettes of the scalar cube, the random-offset tiling is invariant under this reflection, and translations identify the reflected cube grid. Apply the fourth-derivative Bernstein bound to this even polynomial; the second-difference combination in (44) kills the constant and quadratic Taylor terms. Thus
\[
 |D_h^{B}(q)|\le C\beta^{-2}(k+1)^6(l+2)^8
                         |q|^4\|h\|_2^2 . \tag{46}
\]
For the unfiltered single-update form take $p(t)=t$, directly using (16)'s first bound and $r=C(l+2)$. In particular on the prescribed side $l\asymp\beta^{\epsilon_*}$ of §11 it is $o(|q|^4\|h\|_2^2)$. To apply (45) it suffices to prove the desired **upper** bound for the remaining signed fourth momentum difference of the covariance of the true conditional means. No separate transfer positivity of that difference is assumed; (44)–(45) apply to the full Wilson covariance. The test concerns physical frequencies $|q|=O(a)$, which are not resolved by the polynomial microscopic window of (42).

### 12.1 A single nearby slice asymptotically captures the microscopic boundary score

For the cube $H_j$ at lattice time slab $[j,j+1]$ let $\mathcal B_0$ reveal spatial links on time plane zero, and $\mathcal B$ reveal those on both periodic site-reflection planes $0,n/2$. At finite cutoff,
$\|\mathbb E(H_j\mid\mathcal B)-\mu H_j\|_2^2=C^H(2j+1,0)$ as in Annex O.36. On the prescribed sequence of §11, for $j\to\infty$ with $j\ll\beta^{\epsilon_*/100}$, one can recover this norm asymptotically from $\mathcal B_0$ alone:
\[
 \frac{\|\mathbb E(H_j\mid\mathcal B_0)-\mu H_j\|_2^2}
 {C^H(2j+1,0)}\longrightarrow 1 . \tag{47}
\]
This statement concerns the microscopic range of (42).

Here are the Gaussian boundary computation and the approximation needed for (47). In the continuum limit of the reference lattice curl, use spatial momentum $k\in\mathbb R^3$, $k\ne0$, at positive time distance from the boundary. The transverse spatial potential has covariance
$P_T(k)e^{-|k||t-s|}/(2|k|)$ per independent color, where $P_T=I-kk^\top/|k|^2$. This follows either by integrating the free symbol in time momentum, or by decomposing the Maxwell action as
$\tfrac12\int (|\partial_t A_T|^2+|k|^2|A_T|^2+|E_L|^2)\,dt$: the longitudinal electric component $E_L$ is independent white noise. For each $k$ the transverse Gaussian is Markov in $t$, since its covariance factorizes across zero after division by its equal-time covariance. The tangential spatial curls determine $A_T(0)$ on this transverse subspace through the inverse spatial curl. The point $k=0$ has zero measure. Equivalently the boundary magnetic field has transverse covariance $|k|P_T(k)/2$. At positive unit height the conditional curvature means are the Poisson extensions of this boundary field. Their Fourier multipliers on the transverse magnetic field are bounded by $C e^{-|k|}$, including the angular inverse-curl factor in the normal electric components. Hence they are well-defined Gaussian variables of finite variance.

For a quadratic scalar insertion, its centered conditional mean is
$\tfrac12\sum_A(:\!\|\mathbb E(G_A(1,0)\mid\mathcal B_0)\|^2\!:)$. The colons subtract the expectation of each squared conditional mean. This identity can be justified by first smearing bulk curvatures in a small spacetime neighborhood of $(1,0)$, applying Gaussian conditioning to smooth random variables, and then shrinking the smear. The Poisson multipliers converge in the boundary Gaussian $L^2$ norm because the smear stays away from time zero. The conditional variance of the centered Gaussian quadratic is deterministic and cancels in the centered conditional mean. Reflection into negative time gives independent halves on this same boundary. Thus the variance of this boundary score is the reflected continuum energy covariance at displacement $2$, namely $3d_A/(2^8\pi^4)$ with the Annex O normalization. There is no boundary-independent white electric contribution to that reflected covariance.

Smooth compact spatial test combinations of the tangential curvatures are dense for each of the above linear Poisson functionals. In Fourier variables the separating norm is bounded by the scalar weight $C|k|$; first approximate by smooth rapidly decreasing multipliers away from the origin and then truncate their spatial inverse transforms. Convergence in weighted $L^2$ follows, for example, by convergence of the truncations in ordinary $H^1$ for a Schwartz spatial kernel. Centered color contractions of the squares converge in Gaussian $L^2$ by fourth moments. For any tolerance this gives one finite sum of compact-profile centered squared boundary fields, denoted $B$, for which the covariance-to-norm ratio approximates the full score norm to that tolerance. The profiles and their support may depend on the tolerance.

Lift each linear functional with profile $h$ to a lattice matrix at one root of plane zero. Use $j^{-1}\sum_{z\in\mathbb Z^3}h(z/j)\sqrt\beta\,C_A(0,z)$ for a tangential clover, transporting the matrices to the root along deterministic coordinate paths on that slice of length $O_h(j)$. Use Hermitian traceless components in a common normalization, and take the corresponding centered color traces of squared sums to obtain $B_j$. Such traces, without any choice of color axis, are measurable gauge-invariant boundary observables. The normalization $j^{-1}$ is the three-dimensional Riemann sum times the curvature dimension factor $j^2$.

For completeness the approximation estimates are uniform in this growing support. A linear functional has sum of absolute weights at most $C_h j^2$. On offsets for which all its paths and the bulk stencil if present belong to one side-$l$ box, choose its common near-flat forest gauge. Discard other offsets, of fraction $O_h(j/l)$, at cost $O_h(j^9/l)$ after the largest fourth-moment coefficient sum below; bounded local moments and unitarity control all individual trace products, independently of the offset. On the good chart and the $\beta^{1/32}$ fluctuation ball of §10.1, each path product differs from identity by at most $C_h j(l^{18}\beta^{-1/4}+\beta^{-15/32})$ by telescoping unitary factors. Exceptional data and chart tails are covered by the earlier moment and exponential tail estimates. This permits deletion of the transports in that chart with vanishing total error: the largest amplification is $O_h(j^8)$. For any four remaining matrix factors, deletion of conditional mean shifts costs $O(\beta^{-\epsilon_*/6})$ in joint expectation as in (42), uniformly over their positions; restricting to the geometric good offsets preserves this estimate by Hölder. The Gaussian box-to-infinite-lattice covariance replacement at four positions costs $O(1/l)$ by (38) and Wick. Both $j^8\beta^{-\epsilon_*/6}$ and $j^9/l$ vanish on the stated range. These arguments control $\operatorname{Var}(B_j)$ and $j^4\operatorname{Cov}(\beta H_j,B_j)$, since the latter combines the $j^4$ prefactor with a coefficient sum $O_h(j^4)$.

In the free lattice expression, rescaling $z/j$ gives precisely the boundary magnetic tests above. For instance the equal-time tangential $12$ covariance multiplier is $(|\widehat k_1|^2+|\widehat k_2|^2)/(|\widehat k|\sqrt{4+|\widehat k|^2})$ in plaquette midpoint coordinates, with $\widehat k_i=2\sin(k_i/2)$ and the bounded clover averages added when needed. Tensor entries follow from the same spatial curls. Thus on momenta $k=\xi/j$ the rescaled multiplier is bounded by $C|\xi|$ and converges to the specified continuum multiplier. Smooth profiles suppress aliases by repeated summation by parts. For the cross covariances with the unit-height bulk, the temporal Fourier integral supplies the factor $e^{-j\omega(k)}$, $2\cosh\omega=2+|\widehat k|^2$, times the corresponding bounded angular multiplier and the equal-time magnetic density. Equivalently the leading continuum cross kernel follows from the lattice curl large-distance asymptotic of Annex O; all boundary sites in this sum are separated in time by $j$. Wick's formula then gives convergence of the two lifted quadratic quantities to the variance and covariance with $B$ in the continuum boundary calculation.

By Hilbert-space duality, $\|\mathbb E(H_j\mid\mathcal B_0)-\mu H_j\|_2$ is at least the absolute covariance with $B_j$ divided by its nonzero norm. Its upper bound is the two-plane score norm by the tower property. Divide these inequalities by the latter norm, whose squared value times $\beta^2 j^8$ tends to $3d_A/(2^8\pi^4)$ by Annex O.37. Taking the limit at each fixed tolerance and then sending the tolerance to zero gives (47). Outside the controlled microscopic interval a collection of lower-bound witnesses does not bound any orthogonal component, and the same infinite Gaussian boundary product is not justified for the nonlinear macroscopic field.

### 12.2 Where successive slab projections lose the required power

For an actual nested construction fix the source location and condition on the exterior $\mathcal E_R$ of a centered slab of radius $R$. Its two boundaries determine the conditional mean by the local Wilson factorization. For $R'<R$ the sigma fields satisfy $\mathcal E_R\subset\mathcal E_{R'}$ and the tower property holds. These are nested exterior revelations; the two opposing planes of a single reflection in (O.36) slide when the source-to-near-plane distance changes. They are not themselves a nested sequence. For $R\ll n$, a bound on the centered-slab exterior score is sufficient for a reflected pair of slabs at comparable separation because the reflecting planes can both be chosen in this exterior.

Let an approximate score on $\mathcal E_R$ be a finite combination of boundary Poisson predictors and $e_R$ be the $L^2$-orthogonal prediction error. Projecting to $\mathcal E_{LR}$ only gives
\[
   \beta (LR)^4\|\mathbb E(e_R\mid\mathcal E_{LR})\|_2
             \le L^4\,\beta R^4\|e_R\|_2 . \tag{48}
\]
A uniform improvement by $L^{-4}$ for the conditional norm on the entire orthogonal complement of finitely many predictors fails on the actual finite Wilson probability space. A nontrivial full plaquette in the further exterior has infinitely many linearly independent square-integrable class functions (the full link law has strictly positive smooth density). Choose a nonzero linear combination orthogonal to the constants and the predictors at both radii. It belongs to both nested exterior sigma fields, so conditioning leaves its norm unchanged. This tests a proposed operator-norm inference; it does not identify the specific microscopic mark with that adversarial function.

Consequently a scale iteration must estimate the residual for the *transported Wilson insertion* or restrict its support/spectrum sufficiently to exclude retained exterior functions. Positivity and the single-scale relative approximation (47) by themselves give the first normalized loss (48). In Annex N §§5 and 9 the displayed connected bounds concern selected fluctuations and conditional covariances, with covariance of surviving exterior means explicitly kept. In the constrained boundary calculation, the extra tree decay attaches to a fresh connected fluctuation; the copied old coefficient need not touch that new fluctuation. A bare coarse plaquette estimate at a running coupling would also have to be related to the actual conditional transported source, including its additional boundary and vacuum scores. No all-history bound on this residual to physical radii follows from the current inputs.

For the 21-component vertex observable of Annex E a corresponding local statement includes its full score **law**. At distance $j$ from the reflecting site plane, multiply its two-plane conditional score for $\beta a^4\widetilde q$ by $j^4$. On the same microscopic window it converges in distribution to $c(W-d_AI_6)$, where $W$ is the Gram matrix of six independent standard real vectors in $\mathbb R^{d_A}$ and $c=1/(16\pi^2)$. Indeed at a separation of two rescaled time units the continuum curl projection has three diagonal time–space entries $-c$ and three tangential entries $+c$. Reflection multiplies the time–space components by $-1$, so the six conditional linear means have covariance $cI_6$ per color. The covariance of centered quadratic scores paired with real symmetric test matrices $H,K$ is therefore $2d_Ac^2\operatorname{tr}(HK)$. For this **reflected** comparison a coefficient matrix across the plane transforms as $S K S$, where $S$ acts by the indicated signs on two-forms. The zero-spatial-momentum quadratic Hodge-star cancellation in Annex O.13 is a different summation and creates no null direction in this pointwise Gram. All signed clover offsets stay bounded, so their common leading field strength enters these scores. The reflected quadratic covariance of the trace-completion discrepancy $2w_a-t_a$ has zero leading coefficient: in its signed stencil the two terms have the same diagonal Gram at this separation. Equation (42) times $j^8$ has vanishing error; positivity of the corresponding reflected squared conditional norm proves that this discrepancy vanishes in the scaled score. This reasoning uses actual vertex-site reflections and $2j$ separations, with the cube $2j+1$ convention used only for (47).

To justify distributional convergence, approximate the six continuum conditional means simultaneously by finitely many compact-profile boundary linear functionals as in §12.1. In a common good-box gauge the characteristic functions of the lifted linear sums converge jointly to their Gaussian counterparts. In more detail, the summed conditional-mean displacements cost $O_h(j^2\beta^{-\epsilon_*/6})$ in $L^2$, the path and Taylor factors cost $o_h(1)$ in $L^1$ (bounded local moments as above), and the good-box full-coordinate density approximation in §10.1 is in total variation, valid for bounded characteristic tests in growing dimension. The conditional centered *linear* Gaussian covariance depends on the offset. Bound its difference from the uniform lattice counterpart in expectation by $C_h j^4/l$ using (38) and the deterministic weight sum. The rare offsets cut between paths contribute $O_h(j/l)$ to a bounded characteristic test. Thus quadratic color contractions of a fixed family converge jointly in law by continuous mapping. For the actual conditional scores use the joint versions of the second-moment and cross-covariance comparison of §12.1 for each symmetric contraction. The exact reflected norm and this common family of approximate predictors give an $L^2$ approximation with error tending to zero as the fixed approximation tolerance is decreased. This proves the stated law and its covariance. Fourth-moment comparison for the underlying matrices alone would not imply a distributional theorem for the scores. No convergence of all higher score moments or fixed-physical-scale Wishart law is claimed.

### 12.3 Separated smooth vertex sources on the near-prescribed selection

Let $f,g$ be fixed smooth compact scalar profiles with supports a positive physical distance apart. Write $A_f=a^2\beta F_f^H$ for the centered closed-cube insertion and $D_f=a^2\beta(F_f^w-F_f^H)$ for the centered placement difference in the Annex E four-vertex convention. Suppose the selected coupling satisfies $|\beta^2\chi-A_0|=O(\beta^{-\epsilon_*})$ and use the prescribed mean estimate (O.30). On the weak-stop geometry $a$ decreases faster than any inverse power of $\beta$. Then
\[
    |\operatorname{Cov}(A_f+D_f,A_g+D_g)|
                   \le C_{f,g}\beta^{-\epsilon_*}. \tag{49}
\]

In the box estimates of §10 choose $l=L^{\lfloor 2\epsilon_*\log_L\beta\rfloor}$, where $\epsilon_*=10^{-6}$. The polynomial chart, Hessian, tail and fourth-moment errors of §10 still fit $O(\beta^{-1/32})$ with this exponent. The uniform per-root squared conditional mean budget from (O.30) and (31) is $O(1/l+\beta^{-1/2000}\sqrt{\log\beta})=O(\beta^{-2\epsilon_*})$. The replacement of any one of four factors by its centered version in (42) therefore costs $O(\beta^{-\epsilon_*})$ by Hölder with exponents $2,6,6,6$. The clover and plaquette moments used here are uniform by Annex A. In particular, all six orientation pairs of individual plaquette energies have absolute covariance error $O(\beta^{-\epsilon_*})$ in $\beta^2$ units, uniformly over pairs on the test support.

Both the transverse two-coordinate stencil in the cube smearing and the tangential two-coordinate stencil in vertex smearing average symmetrically about the same plaquette center. Consequently $D_f=\beta a^4\sum_p h_{p,a}(s_p-\mu s_p)$ with uniformly bounded weights supported on an $O(a)$ enlargement of the original support. This exact bounded-weight representation uses the second derivative bound; it does not require replacing $h_{p,a}$ by a limiting Hessian profile. The uniform absolute covariance error gives $O_f(\beta^{-\epsilon_*})$ in its variance by summing absolute weights. The Gaussian energy kernel is summable over relative positions by the projection row identity $\sum_q|P_\infty(p,q)|^2=P_\infty(p,p)$. Its contribution is $O_f(a^4)$. Thus $\operatorname{Var}D_f=O_f(a^4+\beta^{-\epsilon_*})$.

Condition on the translated box skeleton and include its independent uniform offset in the conditioning sigma field $\mathcal E$. The conditional variance loss for $A_f$ satisfies $\operatorname{Var}\mathbb E[A_f\mid\mathcal E]=O_f(\beta^{-\epsilon_*})$. Indeed the chessboard upper is $\beta^2\chi a^4\sum_c f_c^2$, while the conditional lower on these boxes is $(d_Ah_l/2l^4)\int f^2$ up to $O_f(\beta^{-1/32}+a l^3)$ by the box energy variance and smooth weight freezing. For sufficiently small $a$, no conditional box intersects the enlarged supports of both sources. Their conditional covariance therefore vanishes for every offset. The full covariance in (49) equals the covariance of the two exterior means. For each such mean its variance is bounded by $2\operatorname{Var}\mathbb E[A_f\mid\mathcal E]+2\operatorname{Var}D_f$, which proves (49). The result controls the contact-normalized covariance on the susceptibility selection. A finite physical covariance bound would require $O(a^4\beta^2)$ on the right of (49).

## 13. Connected real terminal kernels with component-owned sources

Freeze the real exterior and the geometry of one successful terminal erasure. Keep the original integration coordinates and any component-local history labels summed by LFR II (1.71). Suppose the physical density jets of two sources belong to distinct component variables $i,j$. For example, the two sources can lie on two captured first-step islands with disjoint owned determining collars in the constrained readout, §8. There (C.17) identifies the actual first regular density jet as a bounded real function of the owned old coordinates. Adding intermediate source-free kernels preserves this equality when those coordinates are protected throughout. A distinct-owner mixed density jet at this stage is the product of those two tests. Strictly raw tests in the respective original component coordinates also qualify.

Write $I(Y)$ for the indices whose component variables enter the native interaction on support $Y$. From (1.71)–(1.72) absorb all one-owner interactions into the individual positive unnormalized measures $m_i\nu_i$, with $\nu_i(1)=1$. Any exterior-only factor is retained once. Zero masses give zero unnormalized insertions. For positive masses let $K(F)$ be the original fixed-exterior unnormalized terminal functional. With $V_Y$ from (1.68), this has the form
\[
 K(F)=m_{\rm ext}\left(\prod_i m_i\right) (\otimes_i\nu_i)
          \left[F\exp\sum_{|I(Y)|\ge2}V_Y\right].
\]
If internal histories are summed, $V_Y$ is evaluated on them inside the integral as prescribed by (1.72). The source-free Wilson reference in LFR I (1.100) is included in the unnormalized measures.

For exactly two owners put $W=\sum_{I(Y)=\{1,2\}}V_Y$. For real $W$ the total variation distance between the probability proportional to $e^W d\nu_1d\nu_2$ and $\nu_1\otimes\nu_2$ is at most $\min(1,e^{2\|W\|_\infty}-1)$. Their bounded-test covariances consequently differ by at most $C\|F_1\|_\infty\|F_2\|_\infty\min(1,\|W\|_\infty)$. The product covariance vanishes. Multiplying by $K(1)^2$ gives a bound on the unnormalized mixed difference $K(F_1F_2)K(1)-K(F_1)K(F_2)$. This formulation is valid however small the original mass is.

Here is a uniform sufficient hypothesis for any finite number of components. Distances are in coarse $M$-cube units, with each owner contracted to a point and travel in the exterior charged ordinary lattice distance. Let $d(i,j)$ be this graph pseudometric and let $v_Y=\|V_Y\|_\infty$. For some $m>0$ assume
\[
 \delta=\sup_i\sum_{Y:i\in I(Y),\,|I(Y)|\ge2}
     (|I(Y)|-1)e^{m\operatorname{diam}_d I(Y)}v_Y
\]
is a sufficiently small numerical constant. Then
\[
 |K(F_iF_j)K(1)-K(F_i)K(F_j)|
 \le C K(1)^2\|F_i\|_\infty\|F_j\|_\infty e^{-m d(i,j)} .
 \tag{50}
\]
Indeed changing one coordinate $t$ changes the one-site conditional log density at $r$ by oscillation at most $4\sum_{Y:t,r\in I(Y)} v_Y$. Thus its variation distance changes by at most $c_{rt}=C\sum_{Y:t,r\in I(Y)}v_Y$ for $r\ne t$, $c_{rr}=0$. The weighted row sum of $c$ is at most $C\delta<1$. Tilt at $j$ by $e^{uF_j}$ for real $u$. Couple the random single-component resamplings in the tilted and original laws by maximally coupling the two one-site conditionals, starting at their respective invariant product-space Gibbs laws. In a time average of the resulting couplings, the mismatch probability at $r$ is bounded by $\sum_t c_{rt}$ times the corresponding mismatch probabilities (summed coordinate by coordinate), plus $C|u|\|F_j\|_\infty\mathbf1_{r=j}$ and an endpoint term tending to zero. The last assertion follows by telescoping the mismatch after each uniformly chosen coordinate update; the marginals stay invariant at every update. Applying the nonnegative Neumann series for $c$ and the weighted row bound gives mismatch at $i$ at most $C|u|\|F_j\|_\infty e^{-m d(i,j)}$ in the limiting time average. Differentiate at zero and multiply by the original mass squared to get (50).

The geometry matters when checking this hypothesis from (1.68). For connected mixed $Y$ there is an exterior $M$-cube incident to each component in its support, with fixed convention-dependent collars allowed. The relative tree in (1.67) is an embedded tree meeting every exterior cube of $Y$. It pays for distances between these ports and bounds the contracted diameter up to fixed collar constants. Starting at an exterior port of owner $i$, encode a discrete tree cover by a lattice walk of length $O(1+d_{k,Z}(Y))$, obtained by doubling the tree and adding its incident cubes. There are at most exponentially many such covers in that length. Given the cover, the selected exterior cubes and the touched fixed components are determined up to an exponential number of choices, since each cube has boundedly many incident components. The number of owners is also bounded by a constant times the cover size. Use the spare tree exponent after this entropy, as in the native resummations (1.92)–(1.94). Denote by $P_i$ the number of exterior ports at $i$ and by $s$ the minimum uncontracted exterior gap between distinct components. An individual mixed tree has length at least $s-O(1)$ up to lattice constants: any connected support joining two distinct components contains an exterior crossing between some consecutive pair. Thus the preceding row bound is at most $C\alpha\sup_i P_i e^{-c s}$, with $\alpha$ from (1.68). In the two-component calculation $\|W\|_\infty\le C\alpha\min(P_1,P_2)e^{-c d(1,2)}$ by the same count.

LFR I p.177 places each eligible erased component in a cube of side $100MR_k$, so $P_i=O((1+R_k)^4)$, or $O((1+R_k)^3)$ for aligned rectangular faces. A gap $s\ge C_0\log(2+R_k)$ with $C_0$ large enough and the native small $\alpha$ is sufficient uniformly in the number of components and the cutoff. The weighted-row criterion also applies to any particular denser geometry for which it can be checked directly. Pure per-port smallness by itself does not bound a component row when $P_i$ grows. If an unnormalized upper envelope is wanted, $K(1)\le m_{\rm ext}(\prod_i m_i)\exp(\sum_Y v_Y)$ for the residual mixed interactions; the exponent is bounded by $C\alpha\sum_iP_i$ with these rooted counts. Exterior and historical masses still multiply this expression.

The exterior and geometry are held fixed in (50). Side-by-side integration of (50) cannot remove the covariance of exterior conditional means when forming the covariance of the full Wilson measure. For the noncaptured case (C.20), on real positive histories satisfying its buffers, replacing each of two physical crossing sources by its local real surrogate in the source-dependent unnormalized density costs $O(e^{-cR_1})$ times the source-zero mass per root, including the mixed derivative on a smaller fixed disk. This follows by applying the several-root logarithmic estimate there and the positive real kernel to its density error. The two disjoint buffered neighborhoods must each be in its own owner, so no retained short source carrier meets both. Equation (50) for the surrogates then bounds the mixed determinant with this additional error times $K(1)^2$. For general global pre-erasure tests from (C.24), even a two-component determinant still needs an estimate of the change of each transported test when the other component is replaced. The product reference kernel kills the covariance only of tests depending on disjoint coordinates. A bound on the total variation of the global pullback controls the supremum of the test and does not supply this replacement estimate.

For the **unnormalized** determinant there is a stronger conclusion with a historical prefactor, on every geometry with the unmarked per-port summability above. On a fixed physical real fiber let $b_Y=\inf V_Y$ and expand each mixed weight into the inactive constant $e^{b_Y}$ and the nonnegative active factor $e^{V_Y}-e^{b_Y}$. If it is only the combined exponential that has been identified as real positive on the support, replace every mixed $V_Y$ by its real part; this leaves that exponential unchanged. Conditional on all component variables the activation labels in different $Y$ are independent, and $Y$ is active with probability at most $1-e^{-\operatorname{osc} V_Y}$. In two independent copies use separate uniforms for all these activations. Their union is dominated by independent hyperedges of probabilities $p_Y=1-e^{-2\operatorname{osc}V_Y}$.

The identity $2\operatorname{Cov}(F_i,F_j)=\mathbb E[(F_i-F_i')(F_j-F_j')]$ uses the full normalized two-copy law. On the event that the union cluster of $i$ misses $j$, swap the two replicas' component variables on that cluster and interchange their activation labels for hyperedges inside it. All cross-boundary hyperedges have both replicas inactive and contribute identical constants. The transformation preserves the joint law and reverses the sign of the integrand. Thus its absolute expectation is bounded by $\operatorname{osc}F_i\operatorname{osc}F_j$ times the independent connection probability. If a connection occurs, the sum of contracted diameters $\ell_Y$ of all occupied hyperedges is at least $d(i,j)$. Applying the exponential Markov inequality and the per-port sum gives
\[
 \mathbb P(i\leftrightarrow j)\le e^{-m d(i,j)}
     \prod_Y[1+p_Y(e^{m\ell_Y}-1)]
 \le \exp[-m d(i,j)+C\alpha\sum_t P_t].
 \tag{51}
\]
There is no maximum row restriction in (51). Multiplying the resulting covariance bound by the true $K(1)^2$ gives the unnormalized determinant. Each $P_t$ is bounded by a fixed constant times the terminal volume of component $t$ in $M$-cube units, so the cost can be absorbed on its actual aggregate historical ledger when all these components are charged. This estimate can be weak as a bound on the normalized covariance in a dense large history. Uniform constants without the historical prefactor follow under the row assumption of (50).

The total prefactor can also be reduced to $\prod_t C(1+\alpha P_t)$. Each connection admits a simple alternating path through distinct owner vertices and distinct hyperedges. In its independent union bound each path has weight $\prod_Y p_Y$. Set $a_t=2\max(1,\sum_{Y:t\in I(Y)}(|I(Y)|-1)p_Ye^{m\ell_Y})$. Multiply each transition out of $t$ by $e^{m\ell_Y}/a_t$. Summing these new weights over next hyperedges and new endpoints costs at most $1/2$ per step. The original simple path pays at most $e^{-m d(i,j)}\prod_t a_t$ to reverse the substitution, since it leaves each owner at most once. Dropping simplicity only after this extraction and summing the geometric series proves the claimed prefactor. This bound also leaves all unmarked component masses in place.

The native metric can be restored for the unnormalized bound. Lift a simple quotient path between the two owners to the ordinary $k$-scale $M$-cube graph by joining each entrance to its exit inside the corresponding connected component. Each owner is used at most once, and the cost including the two original anchors and their fixed incident collars is bounded by $C\sum_i|X_i|_k$. LFR I p.177 identifies $Z_k=Z$ at erasure, and (MR.4) includes $j=k$. Its volume comparison with LFR II p.380 gives $\sum_i|X_i|_k\le C\sum_i M^4R_k^4d'_k(X_i)\le C\sum_i H_i$. Collars and port counts obey the same bound. In the unnormalized two-copy integral, allocate this extra fixed historical coefficient before each replica's own old-history sum, using (MR.8)–(MR.9) with that coefficient on the corresponding real mass. This recovers $e^{-m\operatorname{dist}_{k,M}(p,q)}$ with the historically reserved mass majorants. The distance is measured in $M L^k a$ units even when the original anchors are finer. The history summations here are the local labels inside a fixed current owner geometry; an unrestricted sum over exterior geometries still carries its own connected subtraction.

For clarity, the precise residual to be estimated for a leaking source can be stated on the real fiber. Let $F_a,F_b,F_{ab}$ be the first and mixed *density* jets of the global normalized preliminary test (C.24) at zero. After reinstating the physical fixed-exterior terminal law $\pi=K/K(1)$, its mixed normalized logarithmic derivative is exactly
\[
 \pi(F_{ab}-F_aF_b)+\operatorname{Cov}_{\pi}(F_a,F_b).
\]
For components at separation $D$ take neighborhoods of radius $D/4$ around the two anchors in the contracted graph. A sufficient new estimate is that each $F_a$ has a replacement on its corresponding neighborhood with supremum error $C e^{-mD}$, and $\|F_{ab}-F_aF_b\|_\infty\le C e^{-mD}$, all allowing a fixed historical exponential before integration. The two-replica proof works unchanged for these neighborhood functions by swapping the union of every cluster hitting the first neighborhood when none reach the second. The residual interaction needs only a bound on its absolute mean if supremum control is unavailable. At a single real preliminary step the new mixed density defect is the conditional mean of the incoming defect plus the covariance of the incoming first jets after actual field substitution. This is the first source-specific quantity left unbounded by (C.23). Bounds on each absolute numerator separately discard this covariance's cancellation.

The replicated argument also gives every connected order on this real fiber. For $u\ge2$ bounded local marks $f_1,\ldots,f_u$ use $u$ independent activated replicas of the full law and $\zeta=e^{2\pi i/u}$. Put $Y_i=\sum_{b=0}^{u-1}\zeta^b f_i(\sigma^b)$. The logarithm of the joint formal moment generating function of the $Y_i$ is the sum of logs for the individual replicas. Homogeneous degrees $1,\ldots,u-1$ cancel, and the squarefree coefficient of degree $u$ equals $u\kappa(f_1,\ldots,f_u)$. Exponentiating does not change this coefficient, giving $\mathbb E\prod_iY_i=u\kappa(f_1,\ldots,f_u)$. If the union of active hyperedges disconnects the marked owners, cyclically permute replica coordinates on the union cluster of the first mark. This permutes active labels there and preserves the law by the same inactive-constant argument. If this cluster contains $v$ marks, $1\le v<u$, the product is multiplied by $\zeta^{v}$ or its inverse. The exchange on each fixed union graph thus gives zero conditional contribution.

For marks sharing a captured island, include the actual integrated fine configuration in that owner's variables, drawing it from $I_D/d_D$ given the owned real data in (C.17). This keeps $d_D$ in the original mass. Each $f_i$ then reads its physical Wilson plaquette. Replacing these variables by their separate conditional means could lose mixed moments on the same island. Mixed interactions $V_Y$ still act only on the old coarse variables. Multiple strict raw marks also permit this replica exchange.

The union is dominated by independent hyperedges with probabilities at most $u\operatorname{osc}V_Y$. Let $\tau_Y$ be the length of a tree spanning all incident owners in the contracted metric, bounded by $C(1+d_{k,Z}(Y))$ by the port construction. On the marked connection event, the sum of occupied $\tau_Y$ bounds the minimal contracted tree length $\tau$ joining all marked owners. The exponential moment of that sum is bounded by $\exp(Cu\alpha\sum_iP_i)$ by per-port counting at a fixed sufficiently small exponent $m>0$. With $|Y_i|\le u\|f_i\|_\infty$ this yields
\[
  K(1)^u |\kappa(f_1,\ldots,f_u)|
  \le e^u u!\left(\prod_{i=1}^u\|f_i\|_\infty\right)
        K(1)^u\exp[-m\tau+Cu\alpha\sum_iP_i]. \tag{52}
\]
One can restore the ordinary $k$-scale tree between all anchors by including all traversed owners with their connected coarse volumes and fixed-width collars once. Each replica then pays at most a fixed coefficient times its actual historical ledger, uniformly in $u$. Equation (52) applies before integrating the common exterior. Geometry mixing and transported nonlocal source jets require separate estimates.

A generating-function form covers component-local **analytic density factors** directly, without resolving their internal conditional moments. Label the $u$ scalar differentiation parameters by their owners, with sets $I_c$. Assume $F_c(t_{I_c};\sigma_c)$ is component-local and holomorphic in an admitted source disk, $F_c(0)=1$. Define $G(t)=K(\prod_c F_c(t_{I_c}))/K(1)$. The same formal logarithm identity gives
\[
 u[t_1\cdots t_u]\log G(t)
 = [t_1\cdots t_u]\mathbb E\prod_{b=0}^{u-1}\prod_c
                     F_c(\zeta^b t_{I_c};\sigma_c^b).
\]
On each disconnected union graph, cycling replicas in the first marked cluster rotates all its source variables by $\zeta$ or its inverse. Its squarefree coefficient consequently cancels even if the local factors have nontrivial mixed jets. On the connected event take Cauchy radii $r/u$ to remain within a common physical source disk $r$ when several labels name the same actual coupling. The inverse radii cost $(u/r)^u\le(e/r)^u u!$. For factors bounded by $\exp(C H_c(\sigma_c))$ on this disk, integrate their absolute majorants on this event. A possibly variable $H_c$ is paid by multiplying the unnormalized positive single-component measure in the bound by $\exp(CH_c)$ in **each** replica. Activations have precisely the same uniform conditional thresholds under this positive dominating measure, with the same unsourced $V_Y$. Thus the connected-event estimate (51) and the ledger still apply. In particular no smallness or nonvanishing of a *sourced* component normalization is used. Component ownership of the density factors is essential to the cluster rotation.

### 13.1 A finite replacement at one real preliminary step

There is a direct off-owner estimate for the *field evaluation* inside a successful (C.24). Hold its incoming determining background fixed. Write $B_A+B_B$ for the two disjoint real rescaled fluctuation arrays before the nonlinear constraint correction and suppose an incoming carrier $X$ of an analytic old activity misses the explicit real $A_j$ coordinates in component $B$. Keep $B_A$ arbitrary within its cutoff. For $0\le t\le1$ replace $B_B$ by $tB_B$ in the successful free-coordinate chart. LFR I (1.53)–(1.60) uses product small-fluctuation cutoffs here. Take the common smaller chart so that the entire segment and the local block corrections stay within the admitted field domains. The old real $A_j$ on $X$ is fixed along the segment.

CMP102 Proposition 9, (182),(190), bounds the functional derivative of the minimum map with respect to the change of its determining constraints, at every admitted small $B$, with an exponential in the distance from the varied cell. This is stronger than using the norm estimate (1.45) of LFR I on the union of two supports. CMP109 (3.6)–(3.9) explicitly uses the derivative along an interpolating field. In the preliminary change, $C$ and the unit-block correction $hD$ of CMP109 §2 use the fixed neighboring block corridors. More generally CMP102 Proposition 3 gives (73) when the exponentially localized linearizing chart there is used. Composing with those kernels preserves a smaller exponential. The projected curvatures and their finite covariant differences obey the same estimate by (190); the physical current is their local Wilson expression. A simultaneous real gauge transformation of the old and new data leaves the native gauge-invariant old activity unchanged. One can use the block axial representative at each site, as in the gauge-invariant application (3.6).

Integrating the directional derivative in $t$ now bounds the off-owner change of this analytic activity. In native chart units it is bounded by its outer sup norm times its inverse Cauchy margin, a fixed scale-conversion factor, and the sum of $C e^{-c d(x,y)}|g_jB_B(y)|$ over $x$ in the determining footprint of $X$ and $y$ in the other owner's fluctuating region (allow the fixed block corridors). Spatial distances here are on the native mixed lattice of (190). The bound is also valid at fixed nonzero $B_A$. It applies before the paired integral and does not differentiate a real old fluctuation argument. In particular, for a four-term action difference comparing both arrays with each set to zero, the smaller of the two single-owner oscillation bounds can be used. For a summand local in both real-coordinate sets, a genuine cross term must span their gap.

Extending this direct calculation to the final terminal variables requires more. The physical configurations are the actual minima $U(B_k^{(n)},V^{(n)})$ in LFR I (1.18). This permits re-basing the derivative at the actual regular minimum while smoothly changing its **determining constraints**. Newly reinstated constraints are products of the block average of the next minimum and the rescaled fluctuation from (1.53). One would need a common-metric convolution bound for this entire reconstruction, including the unmarked conditional weights and any changing determining sets. In particular the rough old variables $V''$ in (1.50) of LFR II need not lie on one small-data interpolation between two terminal histories. The paper handles these variables by splitting the minimum across a boundary in (1.52)–(1.58) and performing the carrier localization (1.61)–(1.66). Those estimates apply to an activity with an admitted *localized* field domain. A torus-wide supremum test from (C.24) alone supplies no such carrier. The one-step derivative estimate therefore gives one of the terms in a replacement calculation, leaving the conditioned measure and the rough terminal-field replacement for the general transported source.

### 13.2 The actual one-step change of the real conditional measure

Fix a positive real successful fiber of (1.25), its full new determining data and geometry, and two widely separated active components with their complete axial corridors. Hold all other active coordinates fixed in their admitted cutoffs, if present. Write $x,y$ for the pairs of current fluctuation arrays $(A_j,B_j)$ in the two components. In the following statement their separation $D$ is the least current $k$-scale $M$-cube distance between their full supports. Restrict to the physical smaller regularity charts of §13.1, with their margins, on the native weak corridor. Endpoint corners and connecting interpolation in the free determining fluctuations are in those charts. Let $q(x,y)$ be the positive part of the actual (1.60) density on its product cutoff support, with its reference measure fixed. Write
\[
 W(x,y)=\log q(x,y)-\log q(x,0)-\log q(0,y)+\log q(0,0).
\]
For a family with a persistent source component from the first layer through $k$, write $H$ for its total actual historical ledger (including all currently relevant components). Then, uniformly on the successful fiber,
\[
       |W(x,y)|\le C e^{CH-cD}. \tag{53}
\]
The constants can be chosen independently of the torus and cutoff. In particular when the right hand side is small the actual conditional law of these two components differs in total variation by at most $C e^{CH-cD}$ from the product with real weights $q(x,0)q(0,y)/q(0,0)$. For larger right hand sides the probability bound follows directly from variation distance at most one. The product comparison uses the true reference measures on the two free-coordinate sets.

To verify the density comparison, use the equality **before** the Taylor separation of Gaussian and interaction in (1.60). At the gauge-fixed (1.25), the native $T^{(j)}$ factors by region, by B119 (2.19)–(2.22). Immediately after (2.21) the old $A_j$ quadratic is restricted to the same connected component; cross-component quadratic terms have already gone into the old effective $B$ action. The reverse/forward Faddeev–Popov changes in LFR I pp.182–187 introduce block-tree gauge conditions on the active region. Work on their resulting gauge-fixed density, where they give the block-local gauge weights (1.5)–(1.6). The residual block averages are solved by eliminating $b_0(c)$ in each corridor as in CMP109 §2. At fixed new background $v$, $V_j=\exp(i[g_jCB_j-h\widetilde D(g_jCB_j)])M_j(v)$ is local in its free fluctuation coordinates: paths for a coarse bond use only its two adjacent blocks, and among the eliminated corridor bonds only $b_0(c)$ enters that coarse-bond constraint. Hence its nonlinear coarea determinant splits by coarse bond; Haar densities and the block gauge weights are also local. The older $A_j$ coordinates remain the native real free variables. No shared zero-mode delta is being discarded. If two supports intersect these fixed-width determining corridors, include the corridors in the supports defining $D$.

The successful branch equality (1.29) and the subsequent (1.53)–(1.60) leave the external factor $\chi_k^{(n+1)}$ independent of the integrating variables. The (1.9) cutoff is a product of old-$A_j$ constraints and (1.55) acts on each component's small real $B_j$ field, with the local corridor map included if the unscaled coordinates are used. The other small selectors are redundant on this branch by (1.29), (1.54)–(1.59). Thus one can keep sharp indicators in the product reference measures and take logarithms only of strictly positive smooth densities on their support. Variables that are subsequently changed in the failed branch are outside this calculation. Constants $z^{(j)}$, $E_0^{(j)}$ and the extracted action evaluated at $A_j=0$ in (1.60) are independent of $x,y$ on this fiber or are factors of the reference measure. In particular the comparison neither differentiates a sharp cutoff nor estimates a normalizing mass from below.

The remaining nonproduct exponential is exactly the old effective action at its reconstructed minimum. In (1.25) it is the original $A_k^{(n)}$, containing the weighted Wilson action, $E_k,R_k,B_k$ and earlier source-free preliminary $C_k^{(i)}$ as in (1.61); the old explicit fields in its boundary terms remain included. Expanding that same real density is what produces $\mathbb P^{(j)}(g_j,A_j,B_j)$, the new $B_j$ precision, the weighted Wilson difference and the other terms in (1.60). The bound is on their combined four-corner difference. It does not require a second Gaussian approximation of the original measure.

Here are details of the spatial summation. Each localized old term on a carrier $X$ at scale $i\le k$ has outer bound $b_X\le C e^{-\kappa d_i(X)}$ times its native dimension or coupling factors; see B119 (2.25)–(2.31), (2.40)–(2.42) and LFR I (1.63),(1.70). The Wilson term can be taken plaquette by plaquette with coefficient bounded by a fixed power of the smallest inverse coupling on the history. Vacuum constants drop out. For quantities $h_X$ of this type, set $r_U=\operatorname{dist}_{k,M}(X,S_U)$ to owner $U$, with incident stencils included. For either owner, changing only its fluctuations at fixed other owner has oscillation bounded by
\[
    |\Delta_U h_X|\le C\,b_X \exp(Ck+C|\log g_{\min}|)\,
                    (1+|S_U|_k)^C (1+d_i(X))^C e^{-c r_U}.
\]
If the real old $A_j$ arguments in $X$ meet this owner, use $2b_X$ instead; then $r_U=0$. Otherwise these real arguments remain fixed. Apply (190) of CMP102 along the small constraint segment of §13.1 and Cauchy to the old analytic field arguments on $X$. The native mixed separation in (190) bounds ordinary coarsest-scale separation up to fixed constants. Coordinate conversions, summation of cutoff bonds in a coarsest cell, block gauge restoration and the finite derivatives in the field chart cost at most fixed powers of $L^k$ and inverse coupling. In particular the inverse of the geometric $2^{-k}$ margin in the B119 boundary chart has that size. LFR II p.373, at (1.61), explicitly states that the axial restoring map at a site is analytic in the regular field on that site’s determining block alone and cites (106) of the averaging paper. Its real block-path products have unitary factors. See also CMP109 pp.265–266 at (2.3)–(2.5). The gauge can be fixed during the small off-owner comparison, keeping the old real argument fixed. On the near region where this Cauchy comparison would exit the smaller chart, the same inequality follows using $2b_X$ and the stated exponential prefactor. The number of fine coordinates or auxiliary center labels in $X$ per $i$-cell is at most exponential in $k$; its number of $i$-cells is bounded by a fixed power of $1+d_i(X)$. This coarse accounting is deliberately used only as a prefactor.

Bound the four-corner difference of $h_X$ by twice the smaller of its two single-owner oscillation bounds. Since $D\le r_1+r_2+C(1+d_i(X))$, one can spend a small portion of $\kappa d_i(X)+c(r_1+r_2)/2$ on $c'D$. Keep a positive exponential in $r_1$ for spatial summation and the native tree entropy allowance for $X$. Equivalently root $X$ at an $i$-cube realizing $r_1$; the native anchored exponential sum is bounded as in CMP116 (1.26), while summing possible roots against $e^{-c' r_1}$ costs at most $C L^{4k}(1+|S_1|_k)$ on a four-dimensional torus of any side. Sum over scales and finitely many types. The resulting prefactor has log at most $C(k+|\log g_{\min}|+\log(2+\sum|S_U|_k))$. The assumed persistent history has at least one charged nonempty layer at every preceding scale, and (MR.4) covers this cost including the original weak-coupling logarithm and the present volumes. Earlier $C_k^{(i)}$ contribute at most the finite $N$ scale multiplicity and the native overlap allowance of LFR I pp.191–192. This proves (53). The sharper mixed tree bound for individual *new sourced activities* is unnecessary for this real one-step measure estimate.

For bounded incoming source functions with owner-local replacements $f_1(x),f_2(y)$, (53) bounds the covariance under this actual conditional step by $C\|f_1\|_\infty\|f_2\|_\infty\min(1,e^{CH-cD})$, plus the two uniform replacement errors paired with the other respective norms. Any incoming mixed density defect remains a separate conditional mean. On a positive real fiber these estimates apply at fixed field values in every other component. They do not address how that single-owner reference kernel changes when the next coarser base itself changes, or what happens when two compared terminal histories have different determining sets or sharp selector outcomes.

### 13.3 A first moderate branch change with its actual event weight

The last decomposition (1.55) at a real preliminary step admits a comparison across its two alternatives. Fix the parent fiber **before** that split: the prescribed exterior selector $\chi_k^{(n+1)}$ is one, $\chi'_j$ of (1.27) is one on both components, and the additional old-$A_j$ condition in (1.28) has succeeded. Include the external last-step factor mentioned below (1.29) if $j+1=k$. LFR I pp.182–187 proves (1.29) under these hypotheses, before using (1.55). In particular the old determining-field regularity selector $\chi_k^{(n)}$ is one. The only active hard restrictions are now (1.9) for old $A_j$ and the primitive (1.27) for the newly fluctuating starred group links. The positive block gauge weights stay inside the integral. Equations (1.53)–(1.54) give $|V_j(V^{(j)})^{-1}-1|<3\delta'_j$ and $|B'_j|<6\delta'_j$ on this parent fiber. The later failure of (1.55) leaves this bound intact.

For the four-corner estimate choose the parent comparison point on the starred free bonds to be $V_Z^{(j)}$ of (1.26), keeping the actual determining and blocking data fixed and setting the old $A_j$ to zero. Join a free bond to that point by $V_j(t)=\exp(t\log(V_j(V_Z^{(j)})^{-1}))V_Z^{(j)}$, $0\le t\le1$. The small principal logarithm exists. Each eigenphase on the first factor shrinks in absolute value, so $\|V_j(t)(V_Z^{(j)})^{-1}-1\|$ never exceeds its endpoint norm. Thus (1.27) holds throughout, including for an endpoint in the full complement of (1.55). Determine each eliminated corridor bond from the same group block constraint and its local analytic solve. The native regularity proof (1.29) and the logarithmic chart (1.54) apply throughout this path. The current star array $B_j$ in (1.55) is the array of free coordinates after eliminating the group deltas and scaling; (1.55) is a component event in these same coordinates. The different coordinate switch (1.59) for a failed component lies **after** the comparison. Both corners may therefore be estimated by (53) on this parent fiber, with $V_Z^{(j)}$ as the comparison point instead of $B_j=0$.

Let $E$ be the entire event $1-\chi'^{(j)}$ at the second owner, or its complementary event, and let $K$ now denote this unnormalized parent integral. Other success requirements local to individual components may be kept fixed in the product reference measures. For a bounded observable $f$ supported on the first owner's variables, the conditional marginal there at any given second-owner value has likelihood ratio between $e^{-2\|W\|_\infty}$ and $e^{2\|W\|_\infty}$ relative to the same first-owner corner measure. The mixture using the original conditional weights on $E$ has the same property. Comparing with the full mixture yields
\[
 |K(f\mathbf1_E)K(1)-K(f)K(\mathbf1_E)|
 \le C\operatorname{osc}(f)\min\{1,e^{CH-cD}\}
                  K(1)K(\mathbf1_E).\tag{54}
\]
It also bounds the difference between two event-conditioned unnormalized readouts, multiplying by the respective two event masses. Zero event mass gives the identity directly. For a near-owner observable whose evaluated source has an off-owner supremum replacement error, add twice that error inside the corresponding marginal comparison using the same masses. Equation (54) controls the law up to the first (1.55) failure. The subsequent simplification of the determining set and new coarse action are separate operations.

There is no such uniformly small conditional probability for a selector already fixed by the common exterior. LFR I p.182 explicitly places $\chi_k^{(n+1)}$ outside the $(A_j,V_j)$ integration. At the initial Wilson decomposition B119 (1.1), for example, choose one distant fixed link in an embedded $SU(2)$ torus and all other links of its test cube equal to identity. Its angle can be varied across the threshold $\|U_p-I\|=\epsilon_0$ while leaving all links near the source untouched. The branch indicator on this frozen block takes the two deterministic values. Neither (54) nor small unconditioned probability estimates give a uniform small relative probability on arbitrary such fixed exterior fibers.

On the failed (1.55) branch the actual coordinate change leading to (1.59) also preserves (54) and the existing pointwise source-replacement errors. Fix the parent determining data. The switch is a bijection on the branch in the failed owner's real coordinates and the identity on the other owner's coordinates. Push forward its positive unnormalized measure, including the Jacobian and the event indicator, and compose each mark with the inverse coordinate change. A pointwise error bound composed with this map has precisely the same bound. An owner-local surrogate remains owner-local in the integration variables at this fixed parent. In particular the common-parent comparison at any positive branch mass remains valid after the exact switch, or after summing all subsequently revealed data back onto that parent.

For a physical free link the pointwise formula is particularly simple. If $B'$ is its new real coordinate and $0\le\gamma(B')\le1$ the B119 (1.22) switch, LFR I (1.58) gives
\[
 V_j(b)=e^{ig_jB'(b)}e^{i(1-\gamma(B'(b)))H_Z^{(j)}(b)}V_Z^{(j)}(b).
\]
Thus the regional background is exact on fully switched bonds. On partially switched bonds a bounded-length real Wilson trace changes by at most $C_N\sum_{b}\|H_Z^{(j)}(b)\|$ on replacing its middle factors by identity, by telescoping the unitary products (also for inverse occurrences). This is $O(\delta'_j e^{-R_j})$ per bond by (1.57)–(1.58). No comparable continuity follows just from boundedness for a merely measurable function of an old real fluctuation. In that case keep the composed test exactly. The distinguished-bond reconstruction must also be transported whenever the mark uses such a bond. The transformation can depend on the common outer determining field; the fixed-parent preservation above does not identify sources on two different later exterior fibers.

## 14. Momentum and angular control of the full Wilson cube covariance

Use the selected compatible tori of (O.57); put $e=\beta^{-\epsilon_*}$ and $F(q)=\beta^2\widehat C(q)$, where $C$ is the full centered closed-cube energy covariance and $q$ belongs to the four-dimensional torus dual with coordinates in $[-\pi,\pi)$. Fourier inversion uses normalized counting measure on this dual. The chessboard estimate gives $0\le F(q)\le F(0)=\beta^2\chi=A_0+O(e)$.

### 14.1 A lower Fourier bound at every momentum

Let $F_{G,n}$ be the multiplier of the flat Gaussian cube energy on the same periodic torus. Then
\[
 F(q)\ge F_{G,n}(q)-Ce,\qquad 0\le F(0)-F(q)\le C(e+|q|^2).
 \tag{55}
\]
The first inequality needs the small-box estimates at prescribed coupling only; the second uses the susceptibility selection. Here are details allowing weights that oscillate from cell to cell. In each compatible side-$l$ box, $l\asymp\beta^{\epsilon_*}$, assign the plane wave at cube centers, transferring it to plaquette weights $w_p$ by the actual cube face average, so $|w_p|\le1$. Each fluctuating plaquette belongs to one box. In the good forest chart let $y=\sqrt\beta(u-u_*)$. On $|y|\le\beta^{1/32}$ the normalized true density is at least $1-O(\beta^{-1/10})$ times the normalized *flat* centered Gaussian density. Indeed §10.1 compares to the Gaussian with precision $G_*$; changing to $G$ costs $O(l^{18}\beta^{-1/4}|y|^2)$ in the exponent and $O(l^{42}\beta^{-1/4})$ in log determinant, using (36). Both tails beyond this ball are superpolynomially small at this $l$.

Taylor-expand the true $\beta\sum_p w_p s_p$ about the good minimum. After subtracting an affine polynomial in $y$, its uniform difference on this ball from $Q_w(y)=\tfrac12\langle dy,M_wdy\rangle$ is at most $C(l^{18}\beta^{-1/4}|y|^2+l^4\beta^{-1/2}|y|^3)=O(\beta^{-1/8})$. Here $M_w$ is diagonal in plaquette indices, with the color identity. For the quadratic difference the sparse Hessian row bound of §10.1 applies with weights of modulus at most one; for the cubic remainder it suffices to sum the per-plaquette bound. All affine coefficients, including the possibly large deterministic linear term, are allowed in taking an infimum for a lower bound on the true variance. In truncated flat Gaussian $L^2$, the squared distance of $Q_w$ from affine polynomials is its variance, since the truncation ball and measure are even. The norm perturbation is $O(\beta^{-1/8})$, and the full Gaussian variance is $O(l^4)$ by Wick and the bounded multiplier. The Gaussian tails of the quadratic and its centered square are negligible uniformly by §10. Thus the true conditional variance on a good box bounds the corresponding flat quadratic variance from below, with error at most $C l^4\beta^{-1/10}$. This Hilbert-space argument applies to complex weights by taking the squared modulus norm. Bad boxes can be discarded in this lower bound: their probability is superpolynomially small per box and the comparison flat variance is uniformly $O(l^4)$. The conditional independent boxes' variances add, and the exterior variance is nonnegative.

If $P_l$ denotes the direct sum of the boxes' embedded curl projections and $P_n$ the full toroidal flat curl projection, then $P_l\le P_n$ and $n^{-4}\operatorname{rank}(P_n-P_l)=O(1/l)$. The ranks per color are $3(n^4-1)$ and $n^4 h_l/l^4$ respectively. The full flat plane-wave variance in a color is $\tfrac12\|P_n M_w P_n\|_{\rm HS}^2$; the box sum uses $P_l$ in its place. Relative to the orthogonal decomposition into $P_l$ and $P_n-P_l$, each of the three extra Hilbert–Schmidt blocks has squared norm at most $\operatorname{rank}(P_n-P_l)\|M_w\|^2$. Dividing by $n^4$ proves the first part of (55). This avoids summing pointwise microscopic errors over a full box.

For the flat energy, its nonnegative spatial kernel has uniformly bounded second moment. One direct check is to take a single lattice momentum step $\eta=2\pi/n$ in the multiplier of $P_n$, set to zero at zero momentum. Away from a distance $2\eta$ from zero the squared difference is bounded by $C\eta^2/|q|^2$ from the nearest-neighbor curl symbol. Inside this distance $O(1)$ grid points contribute $O(n^{-4})$ after normalization. The four-dimensional sum therefore gives a normalized squared difference $O(\eta^2)$. Parseval and $|e^{2\pi i x_j/n}-1|\ge4|x_j|/n$ in periodic representative distances imply a uniform bound for $\sum_x |x|^2\|P_n(x)\|_{\rm HS}^2$. Fixed cube offsets preserve the bound. Consequently $F_{G,n}(0)-F_{G,n}(q)\le C|q|^2$, and $F_{G,n}(0)=A_0(1-n^{-4})$ by rank. This gives (55).

### 14.2 Scalar transition weights at nonzero momenta

For fixed spatial momentum $p$, let $K_t(p)=\sum_z\beta^2C(t,z)e^{-ipz}$, $1\le t\le n/2$. Reflection positivity makes this quantity nonnegative and nonincreasing in $t$ by the paired thermal spectrum, as in (O.34). Complex plane waves can equivalently be realized by their real and imaginary parts; this adds the two real nonnegative quadratic forms, and spatial inversion identifies opposite momenta. In particular (O.57) follows from $\sum_{s=0}^{n-1}K_s(p)=F(0,p)\le C$. The stronger estimate (55) implies
\[
 K_t(p)\le {C\over t}\,[e+|p|^2+t^{-2}],\qquad
 \beta^2\nu_p([0,u])\le C(u+n^{-1})[e+|p|^2+(u+n^{-1})^2].
 \tag{56}
\]
Here $\nu_p$ is the per-momentum transition measure in the normalization of the corresponding unit spatial plane wave. For $t$ beyond a fixed constant choose a nonzero lattice frequency $\omega\asymp t^{-1}$ so that a positive fraction of the integers $s\in[t/2,t]$ obeys $1-\cos(\omega s)\ge c$. For example take the dual grid point nearest $\pi/t$; it lies between $\pi/(2t)$ and $3\pi/(2t)$ for $t\le n/2$. Then $ct K_t(p)\le F(0,p)-F(\omega,p)\le C(e+|p|^2+\omega^2)$. The finite set of small $t$ uses the uniform total bound. Testing the paired spectrum at $t$ comparable to $\min(n/2,1/u)$ gives the second estimate, including $u=0$; null endpoint modes do not contribute at low energy. For the joint momentum-energy measure of a spatial point insertion, integrate the per-momentum estimate against normalized spatial dual counting measure. A frequency ball of radius $r^{-1}$ about $p_0$ has mass bounded by
\[
 C(r^{-1}+n^{-1})^3(u+n^{-1})
       [e+(|p_0|+r^{-1})^2+(u+n^{-1})^2].
\]
This is control of transition *differences* in finite-volume thermal transfer. It gives no positive physical spectral threshold.

### 14.3 Pointwise directional and absolute angular bounds

Let $r_i=1+|x_i|$ in periodic representative coordinates and $R=\max_i|x_i|$. Then
\[
 \beta^2|C(x)|\le {C\over\prod_i r_i},\qquad
 \beta^2|C(x)|\le {C\over\prod_i r_i}
              \left(e+\sum_i r_i^{-2}\right)\quad (x\ne0).
 \tag{57}
\]
In particular, if all four coordinates are comparable to $R$, the improved bound is $C R^{-4}(e+R^{-2})$. The mean of the **absolute** covariance in $\beta^2$ units over the actual sup-norm lattice sphere of radius $R$ is at most $C R^{-4}\log^3(2+R)$ by summing the product bound over its faces. A dyadic annular mean obeys the same estimate. The proof does not assume a sign for the individual correlations.

Freeze the other three real grid momenta and vary one coordinate $q$. Hypercubic symmetry permits taking that direction as time. By the transition spectrum, the multiplier on this line equals its value at $\pi$ plus a positive mixture of functions
\[
 \phi_\rho(q)=\frac{(1-\rho)^2(1+\cos q)}
                       {2(1-2\rho\cos q+\rho^2)},\qquad 0\le\rho<1,
\]
and a possible nonnegative spike at $q=0$. Indeed the paired forward/backward kernel summed over $t=1,\ldots,n-1$ has nonconstant part proportional to $(\cos q-\rho)/(1-2\rho\cos q+\rho^2)$, and subtracting its value at $\pi$ and normalizing at zero gives the displayed factor. The equal-eigenvalue sector gives the spike and a constant; an adjacent null-mode endpoint gives $\rho=0$. The total weight is bounded by $F(0,p)-F(\pi,p)\le C$. Each $\phi_\rho$ is holomorphic and uniformly bounded on the complex disk of radius $c\operatorname{dist}(q,2\pi\mathbb Z)$ about a nonzero real $q$, with fixed small $c$. For $\rho\le1/2$ this follows directly by keeping the disk a fixed distance from its nearest pole. For $\rho\ge1/2$ factor the denominator as $(1-\rho e^{iz})(1-\rho e^{-iz})$; in the stated disk each factor has modulus at least $c'[(1-\rho)+\operatorname{dist}(q,2\pi\mathbb Z)]$, for example by the sine formula or by the triangle estimate on a sufficiently smaller disk around the real point. Consequently away from zero a one-coordinate real interpolation of the grid values obeys $|\partial_q^N F|\le C_N\operatorname{dist}(q,2\pi\mathbb Z)^{-N}$. Only one coordinate at a time is interpolated.

For fixed $N$, take a smooth periodic dyadic partition in each coordinate with a bottom interval containing the origin of width comparable to $C_N/r_i$ (use the whole circle if this is large) and subsequent bands of widths $Q_i\asymp C_N2^{s_i}/r_i$, $s_i\ge1$, capped at a fixed circle scale. The top band is smooth across $\pi$. On a product box whose maximum index is $k\ge1$, integrate by parts $N$ times in a coordinate attaining $k$, using finite differences on the exact dual lattice. The cutoff times the conditional interpolation in this high band has $N$th derivative at most $C_N Q_i^{-N}$ and support of length $O(Q_i)$; set it identically zero around the possible spike. Normalized sums of its $N$th differences cost $C_N Q_i(nQ_i)^{-N}$, since enlarging the support by $2\pi N/n$ changes its length by only a fixed factor. The Fourier denominator is at least $(4|x_i|/n)^N$. The other three coordinate sums contribute their support fractions $O(Q_j)$ by absolute value. Thus every product box contributes at most $C_N(\prod_i Q_i)2^{-Nk}$, with the trivial bottom bound for $k=0$. There are $O((k+1)^3)$ boxes at this index and $\prod Q_i\le C_N 2^{4k}/\prod r_i$. Summation gives the first bound in (57).

For $x\ne0$ invert the defect $G(q)=F(0)-F(q)$ instead, with the harmless change of sign. On a fixed coordinate line it equals its nonnegative value at coordinate zero plus the equal-eigenvalue weight times $\mathbf1_{q_i\ne0}$ and the positive mixture of $1-\phi_\rho(q_i)$. For real $q_i\ne0$, on the same complex disk about $q_i$ one has
\[
 |1-\phi_\rho(z)|\le C[1-\phi_\rho(q_i)].
\]
Indeed $1-\phi_\rho(z)=(1+\rho)^2(1-\cos z)/(2(1-2\rho\cos z+\rho^2))$, whose numerator and reciprocal denominator are each bounded by fixed multiples of their real counterparts on that disk. Cauchy on the mixture now bounds each order-$N$ derivative by $C_N|q_i|^{-N}G(q)$, using periodic distances. On a high band the real interpolated $G$ is at most $C(e+\sum_iQ_i^2)$: it increases in the absolute value of the interpolated coordinate, so apply (55) at the next grid point, capped by $\pi$. Band widths already exceed the spacing. Therefore, for the defect, the previous box estimate gains the full factor $e+\sum_iQ_i^2$, without interpolation loss. Summing over $k$ gives the second bound in (57) for any fixed $N>6$. No joint analyticity of the four momentum variables is required. A coordinate-axis point retains only the inverse first power in (57); the all-direction physical dimension-eight bound remains open.

### 14.4 The diagonal plane on the ordinary periodic torus

On an even cubic torus the isometry $\theta_k(x_1,x_2)=(x_2+k,x_1-k)$ fixes only the slice $d=x_1-x_2=k$ pointwise. On the opposite seam $d=k+n/2$ it acts by a translation by $(n/2,n/2)$. For a $34$ plaquette $p$ in that seam and $n\ge4$ set $F=s_p-s_{\theta_kp}$. This is a bounded gauge-invariant observable of the closed half, $\theta_k F=-F$, and the true Wilson law has $\mathbb E(F^2)>0$ by its strictly positive density on all link configurations. The diagonal reflection form on this half algebra therefore takes a negative value. The character expansion of each crossing $12$ plaquette at the reflecting slice does not change this seam calculation. The corresponding general proof with an actual reflecting boundary is in [Kazakov and Zheng, §3.2](https://doi.org/10.1007/JHEP03(2025)099).

On the alternative period lattice generated by $n(e_1-e_2),n(e_1+e_2),n e_3,n e_4$, opposite diagonal seams are pointwise fixed. A thermodynamic-limit argument for the *cubic* law would require an identification of the two-cube expectations obtained from these two period lattices. A sufficient hypothesis at fixed coupling is uniqueness of the translation-invariant energy two-point function among the relevant Gibbs limits. At each weak-coupling selection window, Fatou's lemma on the uniform integrated susceptibility error allows choosing a fixed coupling with an arbitrarily large subsequence of good compatible cubic volumes. If the stated matching hypothesis is available on a full-measure subset of those windows, first use it at that coupling, then approximate the resulting state's two-cube values on the whole finite target lattice radius to arbitrarily small accuracy by choosing a sufficiently large good cubic volume. Iterating would avoid demanding a thermodynamic-limit rate for fixed coupling. Differentiability of the pressure in scalar coupling fixes the one-point energy and does not by itself give the required matching of the two-point functions. No diagonal reflection theorem for the selected finite cubic laws follows by this argument.

Spatial wavelet decomposition alone also leaves the unresolved axis column. Its total positive time-transition weight is the sum of the weights of all spatial frequency bins. The bound (56) decreases in bins near zero momentum, whereas a fixed nonzero-momentum bin still has an inverse-time upper bound. A stronger estimate on low transition energies in these latter bins, or an independent comparison that transfers diagonal-plane positivity, is needed for this route.

## 15. The scalar score on a fixed nested box skeleton

Take one fixed side-$l$ tiling with an even number of boxes per coordinate. Let $X_B=\sum_{c\subset B}H_c$ sum the microscopic **closed-cube** energies over all cubes in a box. Plaquettes in the interior carry weight one. A plaquette lying on one or two transverse boundary hyperplanes has respectively the symmetric one-half or one-quarter ownership. Its four links lie in the visible boundary subcomplex. All partly hidden plaquettes have weight one and belong to exactly one box. Thus $\sum_B X_B=S$ exactly, and $X_B$ consists of the Dirichlet interior action plus a visible term. With $\mathcal E_l$ generated by the skeleton, set
\[
    Y_B=\mathbb E(X_B\mid\mathcal E_l),\qquad
    \chi_l^\partial=n^{-4}\operatorname{Var}\mathbb E(S\mid\mathcal E_l).
\]
Given the skeleton, the interiors are independent and $Y_B$ is a function only of the boundary of its closed box. It is the actual conditional energy, or the negative logarithmic coupling derivative of that box integral including its visible fraction. Reflection in a block face maps it to the same scalar function in the reflected box. The marginal skeleton measure inherits reflection positivity on its real subalgebra for these aligned reflections. Applying the native chessboard inequality on the coarse grid to the box-local functions $e^{s_B Y_B}$ and differentiating at zero gives
\[
    \operatorname{Var}\sum_B f_B Y_B\le l^4\chi_l^\partial\sum_B |f_B|^2.
    \tag{58}
\]
The same result holds for every translated choice with its correspondingly translated reflection planes. Treating the offset as part of a joint random state need not yield a reflection-positive algebra for a fixed plane: a function of the offset antisymmetric under the plane's permutation of offsets can have a strictly negative reflected square.

Conditional independence gives a stronger equality at distinct boxes. The covariance matrix of the $X_B$ is that of the $Y_B$ plus the scalar diagonal $d_l I$, where $d_l=\mathbb E\operatorname{Var}(X_B\mid\mathcal E_l)$ by translation invariance. In particular $l^{-4}d_l=\chi-\chi_l^\partial$. For every coarse momentum $P$,
\[
  0\le \sum_{q:lq=P} w_l(q)[\chi-\widehat C(q)]
       \le\chi_l^\partial,\qquad
  w_l(q)=\prod_{i=1}^4\left|{\sin(l q_i/2)\over l\sin(q_i/2)}\right|^2 .
 \tag{59}
\]
The factors are defined by continuity. This follows by Fourier transformation of the diagonal innovation identity: the normalized multiplier of $X_B$ is $\sum_{lq=P}w_l(q)\widehat C(q)$, with $\sum_{lq=P}w_l(q)=1$. At $P=0$ only the constant primary alias remains. The lower inequality also follows from the microscopic chessboard bound. In particular $\chi-\widehat C(q)\le(\pi/2)^8\chi_l^\partial$ when all $|q_i|\le\pi/l$. These identities are finite-volume and hold at any bare coupling.

For different temporal coarse slabs, every projected block covariance is exactly the actual block-sum covariance. Its Fourier transform in the coarse spatial sites is a nonnegative sum of the original paired transition exponentials with $\rho$ replaced by $\rho^l$, since each of the $l^2$ microscopic time differences between separated slabs is positive. Reverse time has the same weights by reflection of the whole block. The possible endpoint contact mode is confined to adjacent slabs. Projection changes only zero coarse displacement, hence only a constant in the four-dimensional Fourier multiplier. Thus the transfer decay and the first product bound in (57) apply on the coarse grid to $l^{-4}\operatorname{Cov}(Y_B,Y_{B'})$, with prefactor $C\chi_l^\partial$. They also apply to the true $X_B$ at distinct boxes. This is a statement about the sums of the physical plaquette sources over full boxes.

On aligned nested tilings, $\mathcal E_{Ll}\subset\mathcal E_l$, and the sum of all $Y_B$ within a superbox projects to its corresponding $Y_{B'}$ by the tower law. The associated conditional innovations in distinct superboxes are again independent given the coarser skeleton. Hence $\chi_{Ll}^\partial\le\chi_l^\partial$ exactly. At the selected coupling and for compatible $l$ in the growing weak box window, the full interior action is stationary at its minimizing free variables, so the conditional fourth-moment Laplace calculation gives $\beta^2d_l/l^4=d_A h_l/(2l^4)+O(\beta^{-1/32})$ uniformly. Bad boxes are absorbed by the per-box moment and probability bounds. Therefore
\[
  \beta^2\chi_l^\partial
   = {4d_A\over l}-{3d_A\over l^2}+{d_A\over2l^4}
       +O(\beta^{-\epsilon_*}).
\]
In particular the relative factor tends to $1/L$ along consecutive weak scales with $1\ll l\ll\beta^{\epsilon_*}$. For macroscopic scales, nestedness only carries the previous upper bound forward. To derive another fixed relative gain, one needs a lower bound on the conditional variance released by *this transported boundary score* at the next scale. Ordinary reflection positivity supplies the nonnegative difference and the upper (58); it does not estimate this release.

A fixed microscopic cube inside each coarse box is also a local boundary function after projection, but dissemination produces its reflected placements throughout the tiling. Its constant coarse mode samples those placements instead of all microscopic cubes with equal weight. The susceptibility of that sampled sum is not $\chi_l^\partial$. Thus (58) has not established a relative suppression for a single point score. Even for symmetric true block sums, uniform iteration to the physical scale would require further control of boundary effective actions or their Fisher information and the subtracted noncontact part.

### 15.1 Exact Wilson boundary responses and the remaining flux estimate

Let $\eta$ be the visible skeleton links. Take a collar $\mathcal C$ of $O(V/l)$ closed unit cubes containing all cubes incident on any plaquette that touches a visible link. Write $D=\sum_{c\in\mathcal C}H_c$ and $B=S-D$. Under the positive two-parameter measure with density proportional to $e^{-\beta B-tD}$, at $t=0$ the marginal of $\eta$ is product Haar. At $t=\beta$ it is the actual boundary law $p$. The original chessboard estimate gives $\operatorname{Var}_{p} E[D\mid\eta]\le\chi |\mathcal C|$. For the remaining term let $B_i,D_i$ denote the owned parts of each box, with visible plaquette shares included as boundary constants. With $\eta,\eta'$ independent samples from $p$, differentiation at fixed boundary followed by integration in $t$ gives
\[
  2\operatorname{Var}_{p} E[B\mid\eta]
   =E_{p\otimes p}\left|\sum_i\int_0^\beta
     \left[\operatorname{Cov}_{\beta,t;\eta_{\partial i}}(B_i,D_i)-
       \operatorname{Cov}_{\beta,t;\eta'_{\partial i}}(B_i,D_i)\right]dt\right|^2 .
   \tag{60}
\]
All covariances under the time integral are individual Dirichlet-box covariances. The box bulk mean at $t=0$ is independent of its boundary. Equation (60) uses the homogeneous physical endpoint law for both boundary draws. A pressure difference bounded by the number of collar plaquettes controls the size of an integral of free energies. Equation (60) requires its boundary-dependent bulk derivative in squared mean.

There is also an exact divergence representation with no cutoff. On the full finite torus put $L_b=-\Delta_b+\beta\nabla_bS\cdot\nabla_b$ and solve $\sum_b L_bu=\beta(S-ES)$ with $Eu=0$. A smooth solution exists by ellipticity on the connected compact product group and invariance of the Wilson measure. Integrating each hidden divergence conditionally on all its other links gives
\[
 \beta^2 V\chi_l^\partial
  =\left\| E\left[\sum_{b\text{ visible}} L_bu\mid\eta\right]\right\|_2^2 .
 \tag{61}
\]
A bound $\|\sum_{b\text{ visible}}L_bu\|_2^2\le C V/l$ uniform in $\beta,n,l$ would suffice. The explicit one-link force estimate treats $L_bS$. The vector field in (61) depends on the inverse of the full Wilson generator applied to the centered energy.

For comparison, on a single weak Dirichlet chart take coordinates $y$ centered at a stationary connection, $S=m+Q(y)/2+R(y)$ with $Q$ homogeneous quadratic, and density $J(y)\,dy$ before the Boltzmann weight. For a cutoff $\phi$ compactly supported in this chart, extend its integrands by zero. For conditional expectation at fixed boundary, with $d$ the number of real free coordinates, Haar integration gives exactly
\[
 \beta E[\phi S]= (\beta m+d/2)E\phi+
 E[\beta\phi(R-y\cdot\nabla R/2)
     +\phi y\cdot\nabla\log J/2+y\cdot\nabla\phi/2].
 \tag{62}
\]
This follows by integrating the divergence of $y\phi J e^{-\beta S}$. To recover the original conditional mean one adds $\beta E[(1-\phi)S]$. Even in the purely quadratic case, $m$ is a boundary-dependent harmonic extension energy. The growing weak boxes of §10 control the error to (62) in their stated range. For a physical-size box the centered boundary dependence of the minimum, the residual integral and its rough complement still requires a surface-order estimate on the true endpoint law.

A weaker sufficient dynamical condition uses just the scalar energy. Put $f=\beta(S-ES)$ and $L=\sum_bL_b$. For distinct links, commuting derivatives on their product factors and integrating twice gives
\[
  \langle L_bu,L_cu\rangle
   = E\|\nabla_b\nabla_c u\|^2
      +\beta E\operatorname{Hess}_{bc}S(\nabla_bu,\nabla_cu).
\]
The mixed Hessian has bounded norm and vanishes unless the two links share a plaquette. Consequently the sum over ordered pairs of the negative parts of these scalar products is at most $C\beta\langle f,L^{-1}f\rangle$. Diagonal pairs have nonnegative scalar products. Average the squared norm of the sum in (61) before conditioning over lattice isometries translating and rotating the mask. The norm is invariant, and the probability of retaining either fixed pair together is at most the one-link density $\alpha_l=O(l^{-1})$. Bounding the contribution of every positive scalar product by this inclusion probability and dropping the negative ones proves
\[
 \beta^2\chi_l^\partial
   \le \alpha_l\left[\beta^2\chi+
       {C\beta\over V}\langle f,L^{-1}f\rangle\right]. \tag{63}
\]
Thus an integrated equilibrium Langevin autocorrelation bound for this scalar score, uniform per unit volume in time scaled by $\beta$, suffices in any box range. In the flat Gaussian transverse model the inverse-generator term after this normalization is a constant times $V^{-1}\sum_{p\ne0}|\widehat p|^{-2}$ and stays bounded in four dimensions. For the Wilson endpoint the missing quantity is the inverse-generator quadratic form of the actual energy. The static variance controls the equal-time integrand alone.

### 15.2 A uniform regularized inverse-generator estimate on the original Wilson law

Put $A=L/\beta$, $f=\beta(S-ES)$, and $e=\beta^{-\epsilon_*}$. On the susceptibility selection of §10, for the original link generator on the entire torus,
\[
 V^{-1}\langle f,(A+e)^{-1}f\rangle\le C,\qquad
 V^{-1}\langle f,{\bf1}_{[0,u]}(A) f\rangle\le C(u+e).
 \tag{64}
\]
The first bound controls the inverse moment on $[e,\infty)$ uniformly. Here is a construction of a genuine compact-group divergence that accounts for the leading energy in this estimate.

Use one fixed aligned tiling of side $l\asymp e^{-1}$ as in §10. In a good box of fixed boundary, write $x=u-u_*$ for the difference of the free link logarithms in the relative tree gauge of (36). Choose a smooth radial cutoff $\phi(x)$ equal to one for $|\sqrt\beta x|\le\beta^{1/32}/2$ and zero for $|\sqrt\beta x|\ge\beta^{1/32}$. Set $X=\phi x/2$ in these coordinates, and
\[
 g_i=\beta X\cdot\partial S_i-J^{-1}\operatorname{div}(JX).
\]
Use $g_i=0$ on a bad boundary or outside the chart. The scalar $g_i$ is gauge invariant: the residual common frame acts by conjugation on all logs, the minimizer is unique in this gauge and the metric, radial cutoff and Haar density are invariant. $E[g_i\mid\eta]=0$ by compact support in the conditional integral. No derivative of the good-boundary indicator occurs. Relative-tree gauge integration can be performed with the eliminated vertex frames distributed by product Haar. For gauge-invariant tests these frames do not enter.

On the inner ball, $g_i=\beta(S_i-S_{i,*})-d_Ah_l/2+O(\beta^{-c})$ uniformly for some $c>\epsilon_*$. Indeed stationarity makes the first radial derivative times $1/2$ agree with the quadratic Taylor term. The third-order error is bounded by $Cl^4\beta^{-1/2}|\sqrt\beta x|^3$. The log Haar density gradient contributes at most $Cl^4|x|$. The derivative of the cutoff has $|x\cdot\partial\phi|\le C$. The complement of the inner ball on good exteriors has superpolynomially small conditional mass by (36) and the chart tail estimates, including the annulus where the cutoff varies. Multiplication by the compact polynomial bounds for the energy and the cutoff score preserves this tail. Bad exteriors have superpolynomially small marginal probability, and the energy is bounded by $C\beta l^4$ per box. Consequently for $g=\sum_i g_i$ the independent centered conditional remainder has variance $o(e V)$. The variance of the remaining boundary mean of $f$ is $O(eV)$ by §15. Orthogonality to the centered conditional remainder proves
\[
 \|f-g\|_2^2\le CeV.\tag{65}
\]

To bound the cost of $g$ in the original metric, first consider the flat relative cubical complex on the box. Relative one-forms vanish on boundary edges, and allowable vertex gradients $d_0 h$ have $h=0$ on boundary vertices. Let $P$ denote orthogonal projection off these gradients, and $T$ the isometric zero extension of free off-tree bond coordinates to relative one-forms. The map $PT$ is an isomorphism onto the orthogonal complement of gradients. Indeed any form can be put uniquely into relative tree gauge by subtracting a gradient, since the forest is rooted on the boundary. For flat tree Hessian $G=(d_1 T)^*(d_1 T)$, the random variable $PT y$, $y\sim N(0,G^{-1})$, therefore has covariance $(d_1^*d_1)^{-1}$ on this complement. A constant metric normalization only changes fixed factors. Its trace is $O(l^4)$, uniformly in $l$. For details, the full relative one-form Hodge Laplacian is $d_1^*d_1+d_0d_0^*$. In direction $j$ its tensor-product eigenbasis consists of one-dimensional edge Neumann modes indexed by $k_j=0,\ldots,l-1$, and vertex Dirichlet modes $k_i=1,\ldots,l-1$ for $i\ne j$. These are the eigenbases of $DD^*$ and $D^*D$ for the one-dimensional incidence matrix from internal vertices to all edges. Tensor-product differentials anticommute across axes in the Hodge sum. The eigenvalues are $4\sum_i\sin^2(\pi k_i/(2l))$; none vanish. Summing their inverses is bounded by $Cl^2\sum_{1\le |k|\le 2l}|k|^{-2}\le Cl^4$, including the fixed color multiplicity. Restricting to co-closed forms can only decrease the trace.

In the true inner chart the pushforward of $X$ to link tangents, in left logarithmic velocity, equals $T X+O(\max_b|u_b|\,|X|)$ in Euclidean link norm. Let $h$ solve $d_0h=(1-P)TX$, with a consistent sign convention. The Dirichlet vertex Laplacian has first eigenvalue at least $cl^{-2}$, hence $|h|\le Cl|X|$. Subtract the actual infinitesimal gauge transformation generated by this same $h$. Its difference from the flat gradient has norm at most $C\max_b\|U_b-I\|\,|h|$, by bounded lattice degree and unitarity. Both the actual and flat transformations vanish on visible boundary links, since $h$ is zero at boundary vertices. On support of $X$ all links in this common frame are within $C(l^{18}\beta^{-1/4}+\beta^{-1/2+1/32})$ of identity by §10. It follows that the corrected physical link vector $X_{\rm phys}$ has squared conditional norm bounded, on good boundaries, by
\[
 E|X_{\rm phys}|^2\le C E|PTX|^2+
 C l^2(l^{18}\beta^{-1/4}+\beta^{-1/2+1/32})^2 E|X|^2
 \le C l^4/\beta .
\]
For the last step use the uniform upper Gaussian density comparison on the cutoff ball from §§10,14, the trace estimate for $PTy$, and $\operatorname{tr}G^{-1}\le Cl^{24}$ from (36). The estimate is unaffected by conjugating back through the unitary tree gauge. This subtraction is used in pairing with derivatives of gauge-invariant tests, and requires no Jacobian for the subtracting field.

For any smooth gauge-invariant test $v$, integration by parts and the fact that $v$ has zero derivative along every gauge orbit give $\langle g,v\rangle=E\sum_i X_{i,\rm phys}\cdot\nabla v$. The physical vectors have disjoint hidden-link supports. Cauchy–Schwarz now gives $|\langle g,v\rangle|^2\le (CV/\beta)\langle v,Lv\rangle$. Arbitrary smooth tests may be averaged over vertex gauge transformations: the action and metric are invariant, the numerator stays fixed, and the Dirichlet form decreases by convexity. Density and the variational formula give $\langle g,A^{-1}g\rangle\le CV$. Combining (65) with $\|(A+e)^{-1}\|\le1/e$ proves (64).

For the linear transverse Gaussian torus around the trivial flat connection, the energy excludes all exact vertex gradients and harmonic constant one-forms. On each real transverse mode of positive curl eigenvalue $\lambda$, the centered normalized quadratic energy has variance $1/2$ and eigenvalue $2\lambda$ under $A$. Thus its inverse moment per mode is $1/(4\lambda)$, giving a finite per-volume sum in dimension four. In the actual compact model, invariance of $S$ and $L$ under vertex gauges and flat center twists excludes all nonsinglet gauge sectors and nontrivial center-character sectors from the energy spectral measure, exactly. Center-neutral functions of torus holonomies remain eligible, including conjugacy-invariant neutral Polyakov loop combinations. The Gaussian omission of harmonic modes does not establish independence of their nonlinear counterparts. Bound (64) permits a residual weight of order $eV$ at scales arbitrarily far below $e$, and does not bound its inverse moment; both the spectral cutoff and the susceptibility selection matter.

### 15.3 Positive moments of the actual energy Langevin spectrum

Let $\nu_\beta(ds)=V^{-1}\langle f,E_A(ds)f\rangle$, $\omega(p)=4\sum_i\sin^2(p_i/2)$, and let $dp$ denote normalized Haar measure on the Brillouin torus. With the Wilson action $N-\operatorname{ReTr}U_p$ and metric $-\operatorname{Tr}$, put
\[
    \nu_G=(3d_A/2)\,(2\omega)_*(dp).
\]
As $\beta,n\to\infty$ along the compatible weak-coupling sequence on which the local curvature limit of §§9–10 holds,
\[
  s\,\nu_\beta(ds)\ \Longrightarrow\ s\,\nu_G(ds).
  \tag{66}
\]
This statement needs the local prescribed-coupling results and does not require saturation of the zero-momentum susceptibility. Under saturation the total masses converge to $3d_A/2$ and $\nu_\beta\Rightarrow\nu_G$ as well.

Indeed, for every integer $m\ge1$ the $m$th moment is the sum per site of $\sum_{b,a} E[D_{ba}f\,D_{ba}A^{m-1}f]$, where $a$ indexes an orthonormal Lie basis and $D_{ba}=\beta^{-1/2}\partial_{ba}$ is a scaled left link derivative. The generator is $\sum_{b,a}[-D_{ba}^2+(D_{ba}\beta S)D_{ba}]$. Expand $f$ first into its local plaquette sum. Each application enlarges a local support by at most one plaquette star. After the two final derivatives only overlapping neighborhoods within a fixed radius depending on $m$ contribute. Translation invariance reduces the expectation to finitely many local terms independently of $n$. The integrations by parts are on the compact product with smooth densities.

The resulting expectation is a polynomial in finite ordered derivative jets of $\beta s_p$. Evaluate after differentiating in the independent physical links. All color indices in the final expression are contracted in invariant pairs, so each configuration can be put in one common finite-patch tree gauge for the evaluation. The link deviations in this frame on a fixed contractible patch tend to zero in every fixed $L^p$ by the elementary finite tree filling and the plaquette moment bound. Outside the logarithm chart the probabilities are superpolynomially small. At order zero $\beta s_p$ tends to half the squared Gaussian curl. A first jet is the incident generator contracted against the appropriate transported $\sqrt\beta$ skew plaquette, with the orientation sign, since every traceless anti-Hermitian generator has zero real trace against the identity. Every transport over a fixed path changes this leading contraction by $o(1)$ in moments within the common frame. The possible real trace from the Hermitian part vanishes identically. At order two the limiting tensor is the Euclidean color metric times the two incidence signs, also for repeated source links. This follows by setting all links to the identity in the bounded two-generator word. Each ordered jet of order $k\ge3$ has deterministic norm at most $C_k\beta^{1-k/2}$ by unitarity. The joint local curvature moment result applies to the contracted first jets: equivalently use the common good box frame of §§9–10, in which fixed transport paths converge to identity, then use invariance of the color contraction. The energy moment bound supplies uniform integrability of all finite polynomial products. The limiting generator moments therefore coincide with those of the flat transverse Gaussian energy. On its finite torus each real positive transverse direction contributes mass $1/2$ at $2\omega(p)$; at nonzero momentum the transverse multiplicity is $3d_A$. The Riemann limit yields $\int s^m d\nu_G$. All the positive moments thus converge. Applied to the finite measures $s\nu_\beta$, the moment argument gives tightness, uniform integrability for each moment, and uniqueness since the limit moments have compactly supported representing measure. This proves (66). It gives ordinary vague convergence on $(0,\infty)$ even if a susceptibility upper bound at the prescribed couplings is unavailable.

There is a sharp consequence on the susceptibility selection. For any $\tau\downarrow0$ with $e/\tau\to0$,
\[
   \lim V^{-1}\langle f,(A+\tau)^{-1} f\rangle
      =\frac{3d_A}{4}\int\frac{dp}{\omega(p)} . \tag{67}
\]
For the upper bound retain the leading factor $1/4$ in $X=\phi x/2$ in §15.2. The Gaussian density comparison is $1+o(1)$ uniformly on the support and the actual gauge correction has squared mean $o(l^4/\beta)$. The expected cost per box is thus at most $(4\beta)^{-1}\operatorname{tr}_{\rm coclosed}(d_1^*d_1)^{-1}+o(l^4/\beta)$. This trace is the relative one-form Hodge trace minus the internal vertex Dirichlet inverse trace, since $d_0$ identifies the latter spectrum with the exact one-form subspace. The sine/cosine eigenvalue arrays above give the limit of the difference divided by $l^4$ as $3d_A\int dp/\omega(p)$. For the singularity at zero, the sum over $|k|\le \delta l$ divided by $l^4$ is $O(\delta^2+l^{-2})$ by the same shell count. Cauchy–Schwarz in the regularized inverse norm and (65) make the residual contribution to the norm $O(\sqrt{Ve/\tau})$. For the lower bound apply (66) to compact spectral intervals strictly inside $(0,\infty)$, and then exhaust this interval by nonnegative continuous cutoff functions. They recover the entire finite Gaussian inverse integral. Equation (67) does not estimate an inverse weighted contribution at arbitrarily small positive $s$ on the individual tori.

### 15.4 The ultralow energy projected onto visible plaquette energies

For all sufficiently large prescribed $\beta$ on compatible tori and every family of real coefficients on individual unoriented plaquettes,
\[
   \operatorname{Var}\!\left(\beta\sum_p h_p s_p\right)
       \ge c\sum_p h_p^2 .\tag{68}
\]
Here the plaquettes may have different coefficients in each of the six planes, including zero coefficients on every hidden plaquette. To see this choose one fixed admissible box size $b=L^j\ge 6$ dividing $n$ and average translations of this tiling. At each fixed offset decompose the variance by conditioning on its boundary links. In one good box the argument of §14.1 projects off all affine polynomials to lower bound the variance by the flat quadratic variance up to $o_\beta(1)\sum_{p\in B}h_p^2$. For precision normalize the vector of weights on the fluctuating plaquettes in this box to unit Euclidean norm. At fixed $b$ their number is fixed; the finitely many Taylor bounds and Gaussian comparison on the weak ball are uniform on this unit sphere. Multiply back by the squared norm. The visible-only plaquettes are constants. The same homogeneity bounds the loss on discarding the bad exteriors after averaging, since their probability tends to zero uniformly. All estimates use the original compact Wilson conditional law.

In the flat relative complex let $d$ be curl on **all** relative links and $P$ the orthogonal projection onto its range on the fluctuating plaquettes. The quadratic energy variance is $(d_A/2)\|P M_h P\|_{\rm HS}^2$ and $\|d^*M_h d\|_{\rm HS}\le \|d\|^2\|P M_h P\|_{\rm HS}$. For every plaquette whose chosen pair of opposite parallel links $b_1,b_2$ both belong to the interior, the entry $(d^*M_h d)_{b_1 b_2}$ is exactly $\pm h_p$: these links determine just this one plaquette. Distinct such plaquettes determine distinct pairs. This uses the full relative complex; removing coordinates in a tree gauge preserves its curl range. The operator norm of $d$ is bounded by the lattice incidence degree. Consequently every plaquette deep in this box supplies $c h_p^2$ to the lower bound. Averaging offsets puts each plaquette deep inside some box with a fixed positive probability. Summing the errors counts each fluctuating plaquette once per offset, and yields (68).

For any deterministic set $D$ of visible plaquettes let $\Pi_D$ be orthogonal projection onto the span of their centered energies. Let $f_I={\bf1}_I(A)f$ for a Borel set of normalized Langevin frequencies. Lattice symmetries commute with the generator and preserve $f_I$. Hence
\[
 \langle f_I,\beta(s_p-E s_p)\rangle
    =\frac{1}{6V}\langle f_I,f\rangle
    =\frac{\nu_\beta(I)}6
\]
for every plaquette. Duality with (68) gives, at the actual physical coupling,
\[
   V^{-1}\|\Pi_D f_I\|^2\le C\frac{|D|}{V}\nu_\beta(I)^2 .\tag{69}
\]
In particular on the selected sequence, for *every* compatible macroscopic box size $l$, the full span of its visible plaquette energies sees at most $C(e+u)^2/l$ of the normalized squared energy score below frequency $u$. Its projection of the full energy has squared norm per site at most $C/l$. The estimates hold at once for all linear combinations of individual visible plaquettes. The full conditional mean on the skeleton can also involve nonlinear functions and holonomies along loops formed by many visible links. Equation (69) leaves the projection onto the orthogonal complement of this linear span within the boundary algebra unestimated.

There is a separate exact nonlinear class on a sparse pack $W$ of visible links with every incident plaquette visible. Such a link can run tangentially along the intersection of two distinct cutting planes: any plaquette containing it lies in at least one of those planes. Take no two links of $W$ in a common plaquette. Given the whole skeleton except $W$, the conditional laws on $W$ are the product of the original one-link laws, independent of hidden links. Write $P_b$ for conditional integration at $b$ and $S_b$ for the sum of its six incident plaquette energies. With $Q_\eta$ denoting conditional expectation on the named links, 
\[
 (Q_\eta-Q_{\eta\setminus W})f
   =\beta\sum_{b\in W}(S_b-P_b S_b),\qquad
 \|(Q_\eta-Q_{\eta\setminus W})f\|_2^2\le C|W| . \tag{70}
\]
Indeed all the remaining action is independent of these links under the conditional product, including its hidden conditional mean. The squared norm adds the conditional variances, each uniformly bounded in expectation by the local Wilson energy second moment after scaling. This controls arbitrary nonlinear tests in the orthogonal difference of the two boundary algebras.

At a link $b$ in the interior of a single flat face the same proof cannot be obtained by exposing a finite true collar and using the original one-link centering there. Fix the other visible links and consider an integrable function $h(U_b)$ centered under the original full one-link conditional for almost every compatible hidden exterior. A normal plaquette contains an opposite parallel tangential link off the skeleton that belongs to no other plaquette incident to $b$. Varying it moves its staple $V$ over $SU(N)$ with all other staples fixed. Since the joint physical density is strictly positive, the centering means $\int h(U)e^{\beta\operatorname{ReTr}(UA)} e^{\beta\operatorname{ReTr}(UV)}dU=0$ for Haar-almost every $V$, hence for every $V$ by continuity. Here $A$ is the fixed remaining staple sum. The central convolution kernel $e^{\beta\operatorname{ReTr}U}$ has a strictly positive Fourier coefficient at every irreducible representation: expand the exponential in products of fundamental and dual characters; multiplicities are nonnegative and every irreducible occurs in some such tensor power. Fourier inversion in the uniqueness sense forces $h(U)e^{\beta\operatorname{ReTr}(UA)}=0$ almost everywhere. Thus this uniformly centered single-link class on an ordinary face is trivial. Conditioning only on the actual visible links integrates the unknown normal staple and defines a different centering; control of its temperature response is still required.

A quantitative version does give an infinite-dimensional nonlinear class on ordinary faces. Let $W$ be any pack of $M\ge1$ visible links with no common plaquettes. For fixed other visible links, suppose the function $h$ has zero Haar integral against every polynomial of total degree at most $K$ on the product $SU(N)^W$, counting entries and conjugate entries as degree one. Apply this condition for almost every exterior of the pack in the skeleton. Functions are normalized in the actual $L^2$ norm. Given *all* links outside the pack, the conditional law on $W$ has density proportional to $e^x$, $x=\beta\sum_{b\in W}\operatorname{ReTr}(U_b A_b)$, with $|x|\le 6N\beta M=:B$. The degree-$K$ Taylor polynomial approximates this density with uniform relative error at most $e^{2B}B^{K+1}/(K+1)!$. Thus for any $0<\delta\le1/2$ it suffices to take $K\ge C_N(1+\beta M+\log(1/\delta))$ to bound that error by $\delta$. The polynomial's integral against $h$ vanishes even for the realized hidden staple values. Dividing by the actual partition function and taking conditional Cauchy–Schwarz consequently gives
\[
  \|E[h\mid W^c]\|_2\le\delta\|h\|_2 .
\]
Here $W^c$ contains all other links in the *full lattice*. This argument does not compare the exponentially different normalization constants of the pack to Haar. Since $(I-E[\cdot\mid W^c])f$ is exactly the sum of the independent one-link conditional energy innovations, its squared norm is $O(M)$. Orthogonal decomposition then gives
\[
  |\langle f,h\rangle|\le (C\sqrt M+\delta\|f\|_2)\|h\|_2 .\tag{71}
\]
On the susceptibility selection taking $\delta=\min(1/2,\sqrt{M/V})$ yields a surface-size $O(M)$ squared norm on this high-degree subspace, including ordinary face packs of size comparable to $V/l$. One can instead take a rectangular tensor cutoff of degree $C_N(1+\beta+\log(M/\delta))$ per link by multiplying relative approximants of accuracy $O(\delta/M)$. The unestimated complement still contains smooth functions of entire macroscopic Wilson loops. The reduction to finite fiber degree gives no bound on that growing family.

More precisely, if $p_W$ denotes the actual conditional skeleton density given the remaining visible links, the physical orthogonal complement of the Haar-annihilating test space is fiberwise $p_W^{-1}$ times the polynomial space. The density is positive on the compact product. Thus (71) leaves a score multiplied by its conditional density to be approximated by low-degree polynomials. It does not assert an unweighted polynomial projection in the physical inner product.

The full skeleton $W=\eta$ admits the same conclusion, with no independence assumption. Use the collar $D$ of (60), consisting of $m=O(V/l)$ cube energies. When conditioning on all hidden links $W^c$, $S-D$ is fixed. Therefore $\|(I-E[\cdot\mid W^c])f\|_2^2\le\beta^2\operatorname{Var}D\le\beta^2\chi m$ by the true scalar chessboard inequality. The conditional exponent $-\beta D$ is a polynomial in the entire set of visible matrix entries of degree at most four with absolute value bounded by $C_N\beta m$. Applying the relative Taylor approximation to this polynomial proves (71) with $C\sqrt M$ replaced by $\beta\sqrt{\chi m}$ and global Haar annihilation up to degree $4C_N(1+\beta m+\log(1/\delta))$. With $\delta=l^{-1/2}$ at large $l$ the squared norm bound is $O(V/l)$ on the susceptibility selection. Multiplying the approximants of the individual plaquette weights instead gives an alternative simultaneous degree cutoff $C_N(1+\beta+\log(m/\delta))$ in each visible link, since a link occurs in a bounded number of plaquettes. Here the remaining finite-dimensional comparison is against true boundary-marginal inverse-density times polynomials on the *whole* skeleton. Its dimension can grow rapidly with the physical box and the torus.

## 16. Partial preliminary integrations with successful physical tags

On the actual all-success geometry of LFR I (1.53)–(1.60), divide the new free bonds into a retained set of owners $T$ and an erased set $E$. Suppose the two sets have the ordinary terminal $MR_k$ gap up to fixed $M$-collars. On the $j$-unit lattice the gap is at least $c ML^{k-j}R_k$. Here $b_T,B_E$ are the *scaled* independent Lie-algebra variables of the whole original successful parent. At fixed represented background the new Gaussian precision $K=C^*\Delta^{(j)}C$ has uniform exponentially decaying entries and a uniform positive lower bound, as stated in CMP99 p.428 after (3.158). Write $r_j$ for the actual free-coordinate radius in (1.55) and use the conservative bound $|b_T|_\infty\le p_j=O(\delta'_j/g_j)$ at weak coupling. The printed (1.55) writes $|B_j(b)|<\delta'_j$ after the scaling on the preceding page. Retain its actual indicator and measure every width in that same coordinate. One then has
\[
   |(K_{ET}b_T)(e)|\le C p_j\exp[-c ML^{k-j}R_k],\qquad e\in E .
   \tag{72}
\]
Indeed summing the distance kernel on the entire $j$-unit lattice in four dimensions costs a fixed constant after a slight loss of rate. It costs no factor for the number or volume of the tagged components. The same conclusion holds for $K_{EE}^{-1}K_{ET}b_T$ by restricting to the free coordinates, the uniform gap, and exponential resolvent decay. Exact real Gaussian disintegration retains the tag marginal with Schur precision $K_{TT}-K_{TE}K_{EE}^{-1}K_{ET}>0$. If the erasure uses hard balls in $B_E$, leave the linear term in the exponent with the original balls and all marginal constants. The completion of the square does not justify translating the balls away. On the native complex fluctuation disk, the linear source has a cutoff-power bound times the same exponential per incident erased bond. Its walk decomposition carries an actual path between the two sets, permitting a smaller gap exponent with a remaining carrier decay. In particular the linear source itself is small in the single preliminary-step fluctuation expansion. B119 p.259 explicitly places only a single-component old-$A_j$ quadratic in (2.21); its other terms belong to the old $B$ activities.

For physical raw tags, (1.26),(1.53),(1.58) give a different issue. The regional center $V_Z^{(j)}$ uses the regional data in (1.19),(1.20). If those are fixed for the tagged owner, let $c_T=(ig_j)^{-1}\log[V_T(V_Z^{(j)})^{-1}]$ on the original primitive chart. There
\[
 b_T=(ig_j)^{-1}\log\{e^{ig_jc_T}e^{-iH_Z^{(j)}}\},\qquad
 |b_T-c_T|\le C(\epsilon_j/g_j)e^{-R_j}.
\]
The bound uses (1.57),(1.58) and bounded differential of the logarithm on the physical small chart. The *new* cutoff (1.55) is still on $b_T$. LFR I (1.29) removes an older selector, while (1.59) is an exact change only on a failed sheet.

A one-sided real replacement is possible after integrating the tagged fibers back on their original joint mass. Suppose for each relevant tagged free bond a center available from the intended local data differs from the full physical center by at most $g_j t_j$ on the common parent. Use its ball with radius decreased by $Ct_j$ in scaled coordinates. On that parent it lies inside the true success ball, and the discrepancy on the original success branch requires a true free coordinate in an inner annulus of thickness $C't_j$. At fixed later data and other current free coordinates, assume the smooth log density on this success ball has gradient norm at most $D_j$; for the admitted common smaller charts these are the smooth log terms estimated in the companion note §16, at fixed real historical variables. Radial integration in fixed color dimension $d$ bounds the annular probability by $C t_j(D_j+d/r_j)$. To see this compare the density for $r_j/2<r<r_j$ at nearby radii separated by at most $\min(r_j/4,1/(1+D_j))$, or use the integrated log-slope bound for the radial density with logarithmic derivative bounded by $D_j+2(d-1)/r_j$. For the case of larger thickness use the trivial probability bound; constants can be chosen using $\min(r_j/4,(D_j+d/r_j)^{-1})$ instead to cover also small $D_j$ without an additive constant. A union bound in the original triangular density (C.42) costs only the sum of these probabilities. In each summand all earlier normalized preliminary steps integrate back to one. Thus the unnormalized error for any bounded mark carries its supremum times the *actual* branch mass times this sum, at fixed final conditioning. There is no new branch denominator. This argument supplies an integrated bound and gives no pointwise control after fixing the value of $V_T$ at a moving cutoff face.

At a new preliminary step a copied activity supported entirely in $T$ may depend on the new erased fields through the full minimizing background. Its explicit support need not itself contain the crossing path of (72). A separate local represented-field expansion or a reapplication of the native mixed domain theorem to an admitted spectator representation is needed. In particular the original group variable held fixed at $T$ cannot simply be compared by principal log to arbitrary independent $(U,J)$ on the native gauge-invariant space: endpoint gauges can move a flat coarse link away from that fixed matrix. A covariant parameter $c_T$ and a small analytic extension of the correction $H_Z^{(j)}$ with its jointly compatible regional data would suffice for the smooth substitution. The physical collar formula (1.56) identifies the desired extension's forcing. Combining (72) and the annulus estimate alone does not construct that extension or make an arbitrary successful hard selector a pointwise holomorphic exterior test.

**A second erased integration on deep real tags.** Fix the physical data beyond $h+1$ on one common successful geometry, including the tagged raw records at the later scales and the next real old $A$'s. The regional center $M^h(U_{k,Z}^{(1)})$ on the tagged owner uses its raw determining records and terminal collar by (1.19),(1.20),(1.26). Restrict its free raw $h$-links to have regional logarithms of size less than $r_h-C\epsilon_h g_h^{-1}e^{-R_h}$ in the scaled units of their original test. Equations (1.57),(1.58) and the small logarithm then imply that the *actual* previous success indicator is one for every physical erased $(h+1)$-innovation on the shared admitted parent. The omitted successful mass is bounded by the annulus estimate above with the actual normalized kernels. For a positive fraction claim the prefactor in that estimate must actually be small. A ledger bound with $e^{Ck}$ by itself need not be small compared with $e^{-R_h}$.

For these interior raw tags there is also an explicit complex cylinder in the *new integrated fluctuations*, at a fixed later admitted real background. Hold $b_{h+1,T}$ fixed, and put $z=B_{h+1,E}$ in the native perturbation map $\Phi_{h+1}$. Define $V_c(z)=M^h\Phi_{h+1}(v_{h+2};b_{h+1,T},z)$ and let $c^0=(ig_h)^{-1}\log[V_T V_c(0)^{-1}]$ at the tagged $h$-bond. The required old fluctuation on this cylinder is
\[
 b_{h,T}(z)=(ig_h)^{-1}\log\{e^{ig_h c^0}V_c(0)V_c(z)^{-1}\}. \tag{73}
\]
The baseline $z=0$ and the physical real integration cube are on the stipulated common parent. In the complex cylinder restrict $g_{h+1}|z|$ to the admitted small fluctuation disk, of size $O(\epsilon_{h+1})$. CMP102 Proposition 9, (181)–(190), controls the change from $z=0$ by integrating its exponentially decaying derivative on the complex segment. The input forcing from $C$ and the constraint solve is on the erased bond corridors, with fixed block enlargement; see CMP99 p.428 and LFR I immediately after (1.54). The derivative remains valid with the other, nonzero, admitted determining fluctuations. At an output of scale $h$ its field factor is $(L^h\eta)^{-1}$ in (190), which cancels the factor in the axial restoration and average from LFR I (1.35)–(1.37). The source cell measure cancels the source kernel density $(L^{h+1}\eta)^{-4}$. Even if the remaining $h+1$ cell sum is counted in coarse units, each terminal cell contains at most $C L^{4(k-h-1)}$ such cells. The distance from the tagged output and its averaging stencil to $E$ is at least $cMR_k$ in terminal units on this geometry. Summing the distance kernel gives a bound $C\epsilon_{h+1} L^{4(k-h-1)} e^{-cMR_k}$ for the dimensionless relative change of the coarse link. If this is $o(\epsilon_h)$, as for comparable weak scales with $k-h\le C R_k$ and the fixed $M$ sufficiently large relative to the constants in this bound, (73) stays in the previous fluctuation analyticity disk. The physical radii $g_h r_h$ are smaller than this disk by the native logarithmic cutoff margin. This calculation concerns fluctuation perturbations about this one background; it does not compare arbitrary independent exterior currents or disconnected regular gauges.

In the partial density, changing variables for a retained free link from $b_{h,T}(z)$ to its regional real coordinate carries the ratio of the two exponential-chart Haar Jacobians. At a fixed future, the group map between their exponentials is right multiplication, so this ratio follows from right invariance, and extends analytically without zeros on the small complex cylinder. A bounded measurable function of the raw tag is held fixed. A physical marked coefficient which additionally reads a regular field must have its admitted mixed analytic representation as in the companion note. On the deep real tags the earlier E integral of this smooth density, over its original E cutoff balls, is therefore holomorphic in the new erased fluctuation cylinder by ordinary bounded finite-dimensional integration; use the previous true source-zero $Q_h$ wherever (C.36) uses it. Its physical values undergo the actual second erased integration. This supplies a restricted two-level operation. It neither identifies its output with LFR I (1.63) on an arbitrary independent exterior chart nor controls the pointwise receiver on the omitted raw cutoff faces.

The literal radius in this comparison is quantitatively adequate. Page 183 states $\delta'_i=g_i A_1(\log g_i^{-2})^{p_1}$ with $p_1<p_0$. Put $x_i=\log g_i^{-2}$, use the printed scaled radius $r_i=\delta'_i$ and $R_i\ge x_i^r$, $r>1$. For $t_i=C\epsilon_i g_i^{-1}e^{-R_i}$ and even the crude $\epsilon_i\le C'$, one has $t_i/r_i\le (CC'/A_1)x_i^{-p_1}e^{x_i-R_i}$. In particular $x_i^r\ge2x_i+2\log(100CC'/A_1)$ and $x_i\ge1$ suffice for $t_i/r_i\le e^{-R_i/2}/100$. This uses only a sufficiently weak ceiling at both $i=h,h+1$. It does not predict a vanishing margin error as $k$ grows at fixed endpoint coupling.

The local estimate of the radial log slope uses the *preintegration* logarithm rather than a ratio of partition functions. The Gaussian row contributes $O(p_i)$, and each independent $B_b$ has a positive analytic-disk margin in the smooth interactions (the actual hard indicator is kept outside). Subtract the action at $B=0$ holding the explicit historical real $A_i$ fixed. The discrepancy from the printed subtraction at $A_i=0$ is constant with respect to the varied bond. In the CMP116 (1.41)–(1.43) bounded-plus-quadratic family only carriers reading $b$ can contribute. CMP116 p.16 after (2.19) sums all carriers containing a fixed bond with spare decay. B119 pp.276–277 implements this expansion on (3.43), including the old $B$ and spatial Wilson terms. On the complex one-bond disk, a carrier quadratic costs at most its kernel bound times a cutoff polynomial and the number of its fluctuation sites; the latter is at most $C M^4 L^{4(k-i)}(1+\text{carrier tree length})$ for an $i$-scale array on the present mixed grids. Cauchy controls also possible fluctuation dependence of the quadratic coefficient. The bounded part dispenses with this site factor. LFR I pp.191–192 treats the extra overlap of the previously produced (1.61) contributions on the unmarked parent; there are none at $h$ and just one at $h+1$. Thus the resulting rooted original-law allowance has the form $\operatorname{poly}(1+p_i,g_i^{-1},1+N)L^{C(k-i)}$, with no product of Gaussian normalizations per touched owner. The first line of (1.57) pays this allowance and the count of bonds in a bounded number of tagged owners by its actual exponent $-10\delta M\sum_{a=i+1}^{k-1}R_a-\delta MR_k$ on the comparable weak corridor. Alternatively for a bounded number of all eligible owners, the absolute sum of the logarithmic terms from (C.23) costs at most another $C(1+N)(1+s_i)$ in the slope estimate, with $s_i\le C R_k^4 L^{4(k-i)}$; this factor is paid in the same manner. An estimate exponential in $s_i$ would not have this property. These original-law slope bounds need not hold after conditioning on an arbitrary point of the earlier raw-tag fibers.

## 17. An explicit local Wilson divergence for the exterior score of a scalar mark

Fix a closed cube $x$, write $H_x=\sum_p a_p s_p$ with its original face weights, and let $F=\beta(H_x-EH_x)$. Let $I$ contain the links of a box around $x$ with room for a stencil of radius $r\ge2$ and a fixed collar, and set $\mathcal E=\sigma(U_b:b\notin I)$. All normalizations use action $s_p=N-\operatorname{ReTr}U_p$ and metric $\langle X,Y\rangle=-\operatorname{Tr}(XY)$ on the traceless anti-Hermitian Lie algebra. On the prescribed-coupling compatible tori of §11, for $r$ smaller than $n/8$ with the indicated collar, the construction below gives a genuine polynomial vector field $X$, supported in $I$, such that
\[
  \|E[F\mid\mathcal E]\|_2^2\le \|F-k_X\|_2^2
     \le C\{r^{-8}+r^7\beta^{-\epsilon_*/6}\},\qquad
  k_X=-\operatorname{div}X+\beta X\cdot\nabla S .             \tag{74}
\]
The stated comparison holds in the range $r\le\beta^{\epsilon_*/100}$ at sufficiently large $\beta$. There the right side is $O(r^{-8})$, uniformly in $n$. More generally for each fixed $r$ its limiting residual is given below. Conditioning on any subalgebra of $\mathcal E$ can only decrease the left side. This includes multiple slices or an entire skeleton outside the stencil. Estimate (74) concerns a *point* score and does not bound the norm of the sum of such projected scores without controlling their mutual covariances.

Use the infinite-lattice exterior derivative $d$ on one-forms and its curl projection $P$. For a face $p$ choose $v_p=\eta_r d^*\Delta^{-1}e_p$ where $\Delta$ is the componentwise positive lattice Laplacian on two-forms, $e_p$ is its standard plaquette basis vector and $\eta_r$ on links is one through radius $r/3$, zero beyond $2r/3$, with neighboring differences $O(1/r)$. Put $w_p=dv_p$. All supports embed in the given finite torus without wrapping. The Fourier symbol gives $dd^*\Delta^{-1}=P$ away from zero. The Green-gradient kernel is $O((1+s)^{-3})$ at distance $s$, and its curl $O((1+s)^{-4})$ by dyadic integration of the symbols as in §10.2 (one inverse power of frequency for the Green gradient). Consequently
\[
 \|v_p\|_1\le Cr,\quad \|w_p\|_1\le C\log(2+r),\quad
 \|P e_p-w_p\|_2^2\le C r^{-4}.                                \tag{75}
\]
The last estimate sums the squared discarded curl outside $r/3$ and the squared cutoff-difference term $O(r^{-8})$ per site in the transition annulus.

Choose a base vertex $o$ near the insertion and fixed coordinate paths of length at most $Cr$ between $o$ and the bases of the required bonds/plaquettes, inside the box. Parallel transport all quantities using the original unitary links. Write $Y_q$ for the transported $\sqrt\beta\,\Pi_{\mathfrak g}(U_q-I)$ in the frame at $o$, where $\Pi_{\mathfrak g}$ is the real orthogonal traceless anti-Hermitian projection. Let $\xi_p=\sum_q w_p(q)Y_q$. If $T_{b\leftarrow o}$ transports the Lie algebra at $o$ to the initial vertex of positively directed $b$, set the *left* velocity on that bond equal to
\[
 X_b=\beta^{-1/2}\sum_p a_p v_p(b)\operatorname{Ad}_{T_{b\leftarrow o}}
                                  (Y_p-\xi_p/2).
                                                                    \tag{76}
\]
Thus a variation at $b$ is $U_b\mapsto\exp(tX_b)U_b$. Under vertex gauges $X_b$ transforms in the adjoint at that vertex. Group inverses are adjoints on $SU(N)$ so (76) is a genuine polynomial of matrix entries and their conjugates at fixed $r$. For any real orthonormal basis $T_a$, $\operatorname{div}X=\sum_{b,a}\partial_{ba}\langle X_b,T_a\rangle$, since the Haar-invariant elementary link velocities have zero divergence. Integrating the full compact group conditionally on the exterior gives $E[k_X\mid\mathcal E]=0$ exactly. No small-field event occurs in this identity.

In the infinite flat comparison let $y_q$ be the centered real Gaussian curls with covariance $P$ and independent colors. The action drift in (76) contributes $\sum_a\xi_p^a(y_p^a-\xi_p^a/2)$ per face before multiplying by $a_p$. Indeed varying a link infinitesimally changes a plaquette linearly with its signed incidence, yielding precisely $w_p=dv_p$. The divergence contributes the constant $d_A(w_p(p)-\|w_p\|_2^2/2)$, since the derivative of $y_q$ along the direction $v_p$ equals $w_p(q)$ in the chosen color. Thus the flat residual is $\tfrac12\sum_{p,a}a_p:(y_p^a-\xi_p^a)^2:$, where the colons subtract the Gaussian expectation. As $Pw_p=w_p$, its variance equals
\[
    \frac{d_A}{2}\sum_{p,p'}a_pa_{p'}
       \langle P e_p-w_p,P e_{p'}-w_{p'}\rangle^2 .
                                                                    \tag{77}
\]
This is $O(r^{-8})$ by (75). The same expression is the limit of $\|F-k_X\|_2^2$ at each fixed $r$ by the local prescribed-coupling moment law.

Here are details of the growing-stencil comparison in (74). Every first derivative of a path transport is a sum over *all occurrences* of the differentiated link, with inverse occurrences carrying the differentiated inverse and its sign. In left-invariant unit directions each summand has bounded norm by unitarity. This applies also when the path for the outer adjoint transport traverses the same bond as the inner path or the plaquette; the product rule retains all such terms. Differentiating the transports in $\operatorname{div}X$ therefore costs at most $Cr/\sqrt\beta$ times one rescaled plaquette norm per coefficient of (76). When the derivative instead hits $U_q$ in $Y_q$, its $\sqrt\beta$ cancels the factor $\beta^{-1/2}$ and at identity one obtains precisely the signed incidence times $T_a$, with no extra color normalization. The drift is computed by differentiating $-\operatorname{ReTr}U_q$; the identity and Hermitian parts have zero real contraction with $T_a$, leaving the scaled skew plaquette with the same incidence and transport convention. Finally $\beta s_p-\|Y_p\|^2/2$ is $O(\beta^{-1/2}(\sqrt\beta\|U_p-I\|)^3)$ in every fixed moment using the compact-group inequality $\|(1-\Pi_{\mathfrak g})(U-I)\|\le C_N\|U-I\|^2$, first near identity by Taylor and then on its compact complement.

To estimate products in the residual square, average over the independent offset of the side-$l$ weak boxes of §11. At most $C r/l$ of offsets cut the whole transport stencil. The unconditional summand is gauge invariant and its absolute moments on cut offsets are bounded by the uniform local plaquette moments, the path derivative bound, and (75), independently of that offset. Equivalently discard entire gauge-invariant sums using the coefficient bounds; no expectation of an unpaired color component in two unrelated frames is required. On the remaining offsets one common good box frame has all links on the cutoff ball within $\delta_*=C(l^{18}\beta^{-1/4}+\beta^{-1/2+1/32})$ of identity, with superpolynomially small exceptional probability. Replacing a path by identity in this frame costs $O(r\delta_*)$ times its finite product of bounded-moment scaled curls. Single plaquette derivative factors with two generator insertions have the same estimate by evaluation at identity. The remaining terms are polynomials of degree at most four in rescaled single-face matrices. Center their conditional displacements via the $L^2$–$L^6$ replacement from (41)–(42), with error $O(\beta^{-\epsilon_*/6})$ per product after offset averaging. This also bounds the restricted good-offset average since the squared mean-displacement bound is nonnegative. The uniform chart Gaussian covariance/moment comparison applies to at most four participating faces in one box using the same Hessian estimate, followed by Wick and (38). The same comparison for the scalar mean in $F$ uses the one-face bounds. With coarse constants, the absolute coefficient sum of the drift or divergence before squaring is at most $Cr^2\log(2+r)$, allowing one full extra path length without exploiting its $\beta^{-1/2}$ factor. Its square is at most $C r^6$. Multiplying by $C(r/l+r\delta_*+\beta^{-\epsilon_*/6})$ and absorbing the superpolynomial tails yields the conservative $C r^7\beta^{-\epsilon_*/6}$ in (74). Since $r^{15}\beta^{-\epsilon_*/6}=o(1)$ on the stated range, the Gaussian bound indeed controls the residual there.

At a fixed positive physical distance $R\asymp a^{-1}$ this certificate can still be used at its largest proved inner radius. It gives $O(\beta^{-8\epsilon_*/100})$ for the squared conditional point score on any remote exterior, on the prescribed trajectory. The $O(R^{-8})$ estimate at that physical lattice radius would require control of the actual residual across the intervening radii. The finite-stencil divergence identity alone has no such error rate.

## 18. Conditional damping of a genuine thin Wilson transport

Let $b$ be a link of the periodic Wilson lattice with distinct incident plaquettes, $\pi$ a fixed nontrivial irreducible unitary representation of $SU(N)$, and $\mu_b$ its one-link law given all other links. At every exterior,
\[
 \left\|\int\pi(U)\,d\mu_b(U)\right\|_{\rm op}
    \le 1-c_{N,\pi}/(1+\beta).                               \tag{78}
\]
Write its density $p(U)$ against Haar as proportional to $\exp(-\beta S_b(U))$. The elementary staple gives a uniform bound on the one-link Hessian and Laplacian of $S_b$. Haar integration by parts gives $\beta E_b|\nabla S_b|^2=E_b\Delta S_b\le C_N$. For $\beta\ge1$ choose $G=\{|\nabla S_b|\le C'_N/\sqrt\beta\}$ of conditional probability at least one half. For all $U\in G$ and $|X|\le r=c_N/\sqrt{1+\beta}$, the Hessian bound along the group geodesic shows $p(e^XU)\ge c'_N p(U)$. For $0\le\beta\le1$ the same statement holds on the entire group with new uniform constants by boundedness of the staple. Let $k_r$ be normalized Haar on the central symmetric geodesic ball of this radius. Pointwise translation of the density bound and averaging gives $\mu_b\ge c'_N k_r*(\mathbf1_G\mu_b)$. The Fourier average of $k_r$ is $\kappa_{r,\pi}$ times the identity by Schur's lemma; symmetry makes it real, and $1-|\kappa_{r,\pi}|^2\ge c_\pi r^2$ for small $r$. Indeed the quadratic Taylor term averaged over a ball is a positive constant times the Casimir of $\pi$, while odd terms integrate to zero and the smooth Haar density has its Euclidean leading term. The radius constant may be decreased for the finite set of representations in use. For each unit vector $v$, the variance of $\pi(U)v$ under $\mu_b$ is at least $c'_N\mu_b(G)(1-|\kappa_{r,\pi}|^2)$, by taking the conditional variance over the additional left multiplier first. This gives (78). Inverse orientations obey the same bound by taking adjoints.

Let a fixed thin transport involve a pack $W$ of $m$ distinct bonds, each traversed just once, with no two in a common plaquette. The complementary group factors along the path are held fixed under conditioning on $W^c$. Conditional independence and (78) then bound $\|E[\pi(U_{\rm path})\mid W^c]\|$ by $\exp[-c_{N,\pi}m/(1+\beta)]$. For a simple path a pack of size at least its length divided by 19 can be found by the bounded star conflict graph. The same argument applies to all nontrivial irreducibles in $\pi\otimes\bar\pi$ simultaneously. The trivial summand has multiplicity one and the conditional transport on it is exactly identity; all complementary path factors act by the same group representation so they preserve this summand. For any $W^c$-measurable matrix $M$ and $h=\operatorname{Tr}(M\pi(U_{\rm path}))$, comparison with the Haar second moment consequently gives
\[
 \left|E[|h|^2\mid W^c]-\|M\|_{\rm HS}^2/\dim\pi\right|
  \le C_\pi e^{-c_\pi m/(1+\beta)}\|M\|_{\rm HS}^2.
\]
For $m\ge C_{N,\pi}(1+\beta)$ the conditional second moment is at least $\|M\|_{\rm HS}^2/(2\dim\pi)$. Conditional first moments and Cauchy–Schwarz now imply for every complementary observable $F\in L^2(W^c)$,
\[
  |E[\bar F h]|\le C_\pi e^{-c_\pi m/(1+\beta)}\|F\|_2\,\|h\|_2. \tag{79}
\]
This controls normalized correlations of a bulk source with this entire class of thin boundary transports at physical path lengths. For example, adjoint transport between two based projected skew plaquettes admits the same first-moment estimate by excluding the endpoints and all their incident links from the chosen pack and using the endpoint curvature moments. Repeated traversal with a retained singlet, or a sum of many transports whose physical norm may be much smaller than the sum of the individual norms, requires separate estimates.

### 18.1 Boundary Wilson loops representing the interior score

Use a cubical relative-link box of side comparable to $r$, with the mark at distance at least $cr$ from every face, and fixed tangential boundary links. Let $P_I$ project onto the curl range of its relative one-forms, extended by zero on all other plaquettes. For each inserted plaquette $p$, now use $w_p=P_I e_p=d_I v_p$ in (76), with the co-closed solution $v_p=\Delta_{1,\rm rel}^{-1}d_I^* e_p$. Its zero extension is a relative one-form for the ambient lattice; its full curl is the displayed extension of $w_p$. The finite box normal equations give
\[
 j_p=d^*(e_p-w_p),\qquad j_p|_I=0,\qquad d_0^* j_p=0.           \tag{80}
\]
The surviving entries are tangential boundary links: no plaquette which reads an interior link crosses outside the closed box. Thus $j_p$ is a real divergence-free one-chain on the connected exterior boundary graph.

The componentwise Hodge calculus in §15.2 applies in every form degree. Double the side-$s$ relative interval to the periodic interval of length $2s$. Vertex coordinates extend oddly about the boundary sites and edge coordinates extend evenly with their reflected half-link positions. For a two-form use the edge extension on its two oriented axes and the vertex extension on the other two. These are exactly the tensor eigenbases of $DD^*$ and $D^*D$ used above; the one-dimensional incidence intertwines the extensions, including the orientation signs when passing to another form degree. Therefore $v_p$ and $w_p$ are restrictions of the periodic Green gradient and curl projection of at most 16 signed or reflected image sources. The source and its images are separated from boundary-incident faces by at least $cr-O(1)$. The periodic kernel bounds are $C(1+\mathrm{dist})^{-3}$ for the Green gradient and $C(1+\mathrm{dist})^{-4}$ for the curl projection on the doubled torus. One direct proof on the finite Fourier grid splits into smooth dyadic annuli down to width $1/s$. Periodic summation by parts on an annulus of width $a$ gives $C_N a^{4-m}(1+a\,\mathrm{dist})^{-N}$ for symbol order $-m$, $m=0,1$. The bottom grid annulus has boundedly many modes, contributing $Cs^{m-4}$ even without differencing, and the zero mode is omitted. The same proof covers the harmless phases at cell centers. Consequently
\[
 \|v_p\|_1\le Cr,\quad \|w_p\|_1\le C\log(2+r),\quad
 \|j_p\|_\infty\le Cr^{-4},\quad
 \|j_p\|_1\le C/r,\quad \|j_p\|_2^2\le Cr^{-5}.            \tag{81}
\]

Root a breadth-first spanning tree at $o_\partial$ on the cubical boundary. For each non-tree edge $e=(x,y)$ let $F_x,F_y$ be the tree products from that root, and $K_e=\Pi_{\mathfrak g}(F_x U_e F_y^{-1}-I)$. The notation $F_x U_e F_y^{-1}$ means the based holonomy of the tree path to $x$, then $e$, then the reversed tree path to $y$. Fundamental cycles of chords expand $j_p$ with coefficients $j_p(e)$: subtract those cycles and the remainder is a divergence-free flow on a finite tree, which is zero. Define the genuine boundary observable from
\[
  Z_p=\sqrt\beta\sum_{e\notin T} j_p(e)K_e,\qquad
  D_r=\tfrac12\sum_p a_p(\|Z_p\|^2-E\|Z_p\|^2).
                                                                    \tag{82}
\]
Every matrix in this definition is computed on the exterior. A fundamental loop has length $O(r)$, since the intrinsic graph diameter of the boundary is $O(r)$. Commuting neighboring coordinate steps and cancelling backtracks fills it by at most $Cr^2$ oriented elementary squares in the closed box, with conjugating paths of length $O(r)$ (prefixes of the intermediate words). This is for estimating moments only. For a product of unitary matrices the norm of the difference between its increment and the sum of the individual increments is at most the sum of products of their individual increment norms over pairs; telescope twice. The local plaquette moments thus bound, in $L^4$, the error of replacing each scaled skew loop by its sum of transported scaled skew plaquettes by $Cr^4/\sqrt\beta$. All loops together in each $Z_p$ have total absolute filling coefficients $O(r)$ and error $O(r^3/\sqrt\beta)$ by (81). In the flat comparison their filling cochain $u_\partial$ satisfies $d^*u_\partial=j_p=d^*(e_p-w_p)$, hence $P u_\partial=P(e_p-w_p)$. Frame transport is identity at leading order. The centered Gaussian square in (82) is therefore precisely the residual after (76). In the original Wilson comparison use the same good-offset tree frame and the same fourth-moment bounds as in (74), now with total filling weights $O(r)$ and one extra factor $O(r)$ for the path length. The expected square of the difference of the two residuals still has error at most $Cr^7\beta^{-\epsilon_*/6}$, using (81) for the vector and Cauchy–Schwarz for the $L^4$ loop-linearization error. The center of each squared term is its own actual expectation. This proves
\[
 \|E[F\mid\mathcal E]-D_r\|_2^2
   \le\|F-k_X-D_r\|_2^2\le Cr^7\beta^{-\epsilon_*/6},\qquad
               2\le r\le\beta^{\epsilon_*/100}.                       \tag{83}
\]
For fixed $r$, the limiting variance of the whole projected score equals (77) with $w_p=P_Ie_p$. Throughout this growing window the error in (83) is $o(r^{-8})$. The boundary conditions here condition on all exterior links, including the tangential edges of the box.

### 18.2 Fourth moment on physical-size boundaries

A separate argument bounds (82) at *all* box sizes embedded without periodic overlap, including $r\asymp a^{-1}$ on sufficiently large tori. For any four possibly repeated chords $e_1,\ldots,e_4$, and an invariant product of two color inner products of the four $K$'s, its expected absolute **value after expectation** is bounded by
\[
 C_N\sum_{\text{pairings}}\exp[-c_N(d(e_i,e_j)+d(e_k,e_l))/(1+\beta)] .
                                                                    \tag{84}
\]
Here $d$ is ambient lattice distance between chord endpoints up to additive constants. The estimate concerns the absolute value of the expectation of the contracted product; the expected absolute product need not decay.

In the tree keep only the root and the paths needed to connect the endpoints of the four chord occurrences. Split at the root, at the at most eight endpoints, and at the branch vertices. This gives boundedly many disjoint maximal segments. As a function of the holonomy of any such segment, the contraction is a matrix coefficient sum in tensor powers of at most eight fundamental or dual factors, with dimension bounded solely in terms of $N$. Expand on each segment into its finitely many irreducible isotypes. The trivial projection is exactly integration of that segment product against Haar. The coefficients of each expanded term are bounded in a fixed finite-dimensional tensor norm independently of all segment lengths: the number of factors and isotypes is fixed, and the chord matrices are unitary. On every nontrivial segment (78) thus yields a factor exponential in its number of purchased edges divided by $1+\beta$. Select a plaquette-independent pack of at least a fixed fraction of all edges of the nontrivial segments, which are edge-disjoint and exclude the non-tree chord edges. Condition on its complement; the bound multiplies over segments and occurrences in the *isotypic representation of each segment product*, not over repeated occurrences in the original expression.

For the cancellation underlying the length bound, delete all trivial segments and join the remaining tree pieces by all labeled chord edges. Before projecting on the nontrivial segments, integrating the deleted segment products against independent Haar randomizes one left root frame $R_C$ for each remaining tree piece $C$, independently, apart from the original root piece whose frame is fixed to identity. This follows by evaluating successive Haar connectors down the quotient tree. In terms of the remaining internal tree products $F_x^{\rm int}$ at each vertex, the based chord at $(x,y)$ becomes
\[
   (R_{C_x}F_x^{\rm int})\,U_e\,(R_{C_y}F_y^{\rm int})^{-1}.
\]
If a connected component of the graph after adding the chords has exactly one labeled chord occurrence, multiply all its $R_C$ on the left by a common $G$. Only that one $K_e$ is conjugated, and Haar averaging kills its traceless anti-Hermitian part. When that component includes the fixed root, rotate all the other components instead and use global conjugation invariance of the scalar contraction to obtain the same cancellation. If a chord is repeated it counts with all its occurrences. The subsequent projections in the remaining disjoint segment variables commute with the preceding Haar integrals and preserve this zero. Thus every surviving component containing chord labels contains at least two of them. With four labels this leaves two pairs or a connected quartet. In either case a traversal of a spanning tree, of doubled edge length at most twice the total nontrivial segment length plus a fixed chord allowance, produces a pairing whose distance sum is bounded by this traversal length. The spatial distances are no larger than the traversed lattice lengths. This proves (84).

For a fixed chord on the boundary, the sum of $\exp[-c d/(1+\beta)]$ over the other chords is $O((1+\beta)^3)$, by the finite number of three-dimensional faces of a box. Summing (84) with the real coefficients of (82) and applying the row-sum bound on each pair gives the actual Wilson estimate
\[
 E\|Z_p\|^4\le C_N\beta^2(1+\beta)^6\|j_p\|_2^4
         \le C_N\beta^2(1+\beta)^6 r^{-10},\qquad
 \|D_r\|_2^2\le C_N\beta^2(1+\beta)^6 r^{-10}.               \tag{85}
\]
Thus on physical boxes with $r/\beta^4\to\infty$ this particular boundary loop observable has variance $o(r^{-8})$. It is an actual Wilson observable evaluated at that radius. Identifying it with the full conditional energy score there would require extending (83) across the intervening radii. In particular two identical adjoint transports contracted into a singlet transmit $\langle\operatorname{Ad}_U Y,\operatorname{Ad}_U Y\rangle=\langle Y,Y\rangle$ unchanged. The one-link contraction cannot supply a uniform decay for this component of a general gauge-invariant score.

### 18.3 All nonlinear functions of coarse thin-link records

One can remove the restriction to a fixed representation in the mixing estimate. The symmetric central ball kernel $k_s$ on $SU(N)$ satisfies $1-|\kappa_{s,\pi}|^2\ge c_Ns^2$ for every nontrivial irreducible unitary $\pi$, uniformly at small $s$. For $|w|\le s/8$ average
$\|\pi(w)v-v\|\le\|\pi(wh)v-v\|+\|\pi(h)v-v\|$ over $h$ in the $s/8$-ball. Both arguments have densities at most $C_N k_{s/2}$ by the ratio of the ball volumes. For a unit vector this bounds the square by $C_N(1-\kappa_{s/2,\pi})$, uniformly in $w$. Every element of the compact connected group is a product of at most $C_N/s$ elements of that small ball. Telescoping their action on $v$ and averaging over the whole Haar group gives $2\le C_N s^{-2}(1-\kappa_{s/2,\pi})$. Finally $k_s*k_s\ge c_N k_{s/2}$ by the intersection of the two balls, so the claimed absolute gap follows by integrating the nonnegative squared displacement against this convolution. The same proof of (78) therefore yields one constant uniform in all nontrivial representations.

At its maximizer the smooth star density $p$ has zero gradient and a log Hessian bounded by $C_N\beta$ in absolute value. Integration over a ball of radius $c_N/\sqrt{1+\beta}$ therefore gives $\|p\|_\infty\le C_N(1+\beta)^{d_A/2}$ at every exterior. Conditional on the complement of a plaquette-independent pack of $m\ge2$ singly traversed path links, let $q$ be the density of the path holonomy with respect to Haar. The first and last factors each have $L^2$ norm at most $C_N(1+\beta)^{d_A/4}$. The intermediate convolutions are contractions by $1-c_N/(1+\beta)$ on the entire centered Haar $L^2$ by Peter–Weyl and (78). Interspersed fixed translations or inversions preserve the required norms. Taking the convolution of the first and last $L^2$ functions after the intermediate contractions bounds
\[
       \|q-1\|_\infty\le \delta_m
       = C_N(1+\beta)^{d_A/2} e^{-c_N(m-2)/(1+\beta)} .       \tag{86}
\]

For $M$ paths whose packs are mutually plaquette-independent, with each purchased bond exclusive to its own path, condition on their full common complement $\mathcal C$. The path holonomy variables are conditionally independent. If each path has at least $m$ purchased bonds and $M\delta_m\le 1/4$, their joint density against product Haar lies between $1-CM\delta_m$ and $1+CM\delta_m$, uniformly in the complement (with a fixed strictly positive lower bound). The actual marginal, obtained by averaging the same physical conditional density, has the same bounds. For a centered $F\in L^2(\mathcal C)$ the conditional projection onto all path records $G$ satisfies
\[
         \|E[F\mid G]\|_2\le C M\delta_m\|F\|_2 .              \tag{87}
\]
Indeed subtract one inside $E[Fq(G\mid\mathcal C)]$, then divide by the true marginal density. This proves (87) for the full nonlinear boundary algebra generated by these thin transports, including arbitrary joint neutral functions of winding loops, whenever its paths/packs satisfy these geometric hypotheses. For a cubical boundary grid at spacing $s$, reserve only middle sections of its straight coarse links, leaving a fixed endpoint buffer, and choose every other bond or a bounded coloring to achieve $m\ge c s$. A fixed physical box of fine side $O(e^{C\beta})$ has $\log M=O(\beta)$, so spacing $s\asymp\beta^3$ makes $M\delta_m$ exponentially small in $\beta^2$. The original bulk plaquette energy is complementary to these boundary packs. If $\eta$ denotes the complete boundary data, the exact orthogonal split $E[F\mid\eta]=E[F\mid G]+(E[F\mid\eta]-E[F\mid G])$ leaves the within-fiber fine boundary score in the second summand; (87) controls the first. Smoothed block variables which consult the purchased microscopic bonds outside the specified complete path products are outside this argument.

### 18.4 The actual nested-box release in the weak window

Take concentric cubical exteriors at radii $r$ and $2r$, with side-to-radius ratio fixed up to bounded cell displacements. Write $Q_r$ for conditional expectation onto the entire exterior, and take the same compactly supported scalar mark at the center. There is a fixed $b_N>0$, depending on the cubical radius convention and mark weights, such that
\[
   \|Q_r F\|_2^2=(b_N+o(1))r^{-8},
    \qquad
   \frac{\|Q_r F-Q_{2r}F\|_2^2}{\|Q_rF\|_2^2}
         \longrightarrow 1-2^{-8}                         \tag{88}
\]
for $r\to\infty$, $2r\le\beta^{\epsilon_*/100}$ on the prescribed sequence. The correction terms in (83) and the same moment comparison of (82) to its limiting Gaussian cochain are $o(r^{-8})$ in squared residual and in the variance comparison of the boundary square. The Gaussian expression (77) involves $\langle(P-P_I)e_p,(P-P_I)e_{p'}\rangle=(P-P_I)(p,p')$. Here $P_I$ is an orthogonal subprojection of $P$. It remains to identify the scaling of these fixed central entries.

For the original source's direct image the difference between the infinite and doubled periodic kernel at central sites has a definite limit after multiplication by the fourth power of the box side. On each identical plaquette orientation at equal base it is exactly $1/(2n'^4)$, where $n'$ is the doubled side, by hypercubic symmetry, trace of the rank-three multiplier at nonzero momentum and zero at momentum zero. Changing the displacement by any bounded number of sites affects this difference by $O(n'^{-5})$. Indeed a lattice first difference of $P$ is $O((1+|x|)^{-5})$, is absolutely summable, and its periodic kernel is its exact periodization, as follows from its continuous periodic symbol (assigned zero at zero). For differing plane orientations a coordinate reflection negates one component but not the other, up to bounded base displacements, so this direct-image difference is $O(n'^{-5})$ there. For each other image the rescaled displacement tends to a nonzero point of the doubled continuum torus. The scaled discrete periodic kernel tends there to the smooth-away-from-zero periodic continuum curl projection. To check convergence, use a smooth frequency cutoff at integer Fourier-mode radius $K$ on the unit continuum torus. The finite collection of low modes converges term by term from the sine symbol. The omitted dyadic annuli of the *scaled* far-separated kernel are bounded by $C_D\sum_{2^j\gtrsim K}2^{(4-D)j}$ using the periodic summation-by-parts argument in §18.1 with any $D>4$, uniformly in the doubled lattice size. This identifies a single limiting matrix for the cube and all bounded central displacements. Consequently $r^8$ times (77) has a finite limit. Its positivity follows independently from projecting onto the two true time cuts exterior to this box and the positive lower Gram of the corresponding scalar score in Annex O. The second part of (88) now follows by the exact tower identity $Q_{2r}Q_r=Q_{2r}$ and the variance difference formula. No ratio for a subsequent step outside this weak window follows from (88).

## 19. An entropy bound for the full nonlinear neutral exterior at physical distances

Consider the selected weak couplings of §§8,11 with the maximal pressure-response bound, including the near-prescribed selection using Annex O.20,O.30. Put $X_x=\beta(H_x-EH_x)$. For the exterior of a cubical box of radius $R$, on the compatible even torus with room for that box,
\[
    \|E[X_0\mid\text{exterior of radius }R]\|_2^2
       \le C\frac{\log(2+\beta)\,[1+\log(2+R)]}{R}.            \tag{89}
\]
The exterior may contain all fine link data, including neutral functions on every seam plaquette. At a physical radius $R\asymp a^{-1}$ this bound tends to zero exponentially in $\beta$ on a trajectory with $\log a^{-1}\asymp\beta$. It does not give $R^{-8}$.

Here are the finite-volume estimates. For any deterministic real array $t_x$ with $|t_x|\le t_0$ for a fixed small $t_0$,
\[
       \log E\exp\big(\sum_x t_x X_x\big)\le C\sum_x t_x^2.   \tag{90}
\]
Indeed the closed-cube Wilson chessboard comparison of §8 gives a sum of one-site pressure differences
$\lambda(t)=\psi_n(\beta(1-t))-\psi_n(\beta)+t\beta\psi_n'(\beta)$.
On the interval where the maximal logarithmic average of $s^2\psi_n''(s)$ at $s=\beta$ is bounded, integrating the second derivative twice gives $\lambda(t)\le Ct^2$. In the narrow near-prescribed selection this applies directly only for $|t|\le c h$, where $h\asymp\beta^{-1/4000}$ is the logarithmic window and the selected point lies in its middle half. For $ch\le |t|\le t_0$ use the prescribed first-derivative estimate of Annex O.30 throughout $[\beta/2,2\beta]$. Specifically $u(s)=-s\psi_n'(s)=A_0+O(\beta^{-1/2000}\sqrt{\log\beta})$ there using a common tile size. Integrating the first derivative gives $\lambda(t)\le C(t^2+\beta^{-1/2000}\sqrt{\log\beta}\,|t|)\le Ct^2$. The same reasoning applies on a broad maximal-function selection. A fixed-beta susceptibility bound only at one coupling is not sufficient to infer (90).

Take a box $B$ with side $s$ comparable to $R$ and its set of independent link variables $U_B$. Let $O$ be the complementary links. Choose the inner collar $\Gamma\subset B$ of bounded microscopic thickness containing every inner link in a plaquette meeting both sets. The Wilson action gives exact conditional independence of $U_{B\setminus\Gamma}$ and $O$ given $U_\Gamma$. Therefore the mutual information is
\[
 I(U_B;O)=I(U_\Gamma;O)\le C_N |\Gamma|\log(2+\beta)
                               \le C_N s^3\log(2+\beta).         \tag{91}
\]
For the bound in (91), each individual link given any subset of the other links has density bounded by $C_N(1+\beta)^{d_A/2}$ against Haar, by the maximum-point estimate of §18.3 and conditional averaging. Apply the chain rule inside the conditional distribution of $U_\Gamma$ given $O$. Its entropy relative to product Haar is at most the number of links times the logarithm of the displayed bound. Subtracting the nonnegative relative entropy of the unconditional marginal from the mean of this conditional entropy yields (91).

For the cubes $x$ fully inside $B$ put $m_x(O)=E[X_x\mid O]$. At each fixed exterior the entropy variational inequality against the *actual unrestricted marginal* of $U_B$, together with (90), bounds the conditional relative entropy below by $\sum_x(t_x m_x-Ct_x^2)$. The choice $t_x=\mathrm{sign}(m_x)\min(t_0,|m_x|/(2C))$ is legitimate since (90) holds simultaneously for every deterministic array. Averaging and invoking (91) gives $\sum_xE\min(m_x^2,|m_x|)\le C s^3\log(2+\beta)$. Also $E e^{c|m_x|}\le C'$ uniformly by conditional Jensen and the original one-cube exponential moment. For $T\ge1$, split at $|m_x|=T$. This gives
\[
     \sum_{x\text{ inside }B}\|m_x\|_2^2
        \le C T s^3\log(2+\beta)+C s^4 e^{-c'T}.                \tag{92}
\]
Choosing $T$ proportional to $1+\log(2+s)$ yields a surface-size trace bound up to logarithms.

Finally, the full radius-$R$ centered box about *every* interior $x$ contains $B$ after choosing $s\le cR$, with a fixed stencil margin. Its exterior is a subalgebra of $O$, so the corresponding projected variance is bounded above by $\|m_x\|_2^2$. Translation invariance makes that projected variance equal to the left side of (89) at every such site. There are order $s^4$ complete cubes. Dividing (92) by their count proves (89), including at physical radii beyond the weak-box expansion. The trace bound does not estimate the variance of the sum of all $m_x$ without their off-diagonal covariances.

### 19.1 Off-diagonal covariance for arbitrary fine sources in separated rectangles

Write $S$ for the covariance operator of the scaled closed-cube field $X$ and $A=\beta^2\chi_n$. On the selection of §19, $0\le S\le A I$, $A=O(1)$, and Annex O §45 gives the grid estimate $0\le A-S(q)\le C(\delta+\sum_i |e^{iq_i}-1|^2)$ with $\delta=\beta^{-\epsilon}$ on the stated compatible geometry. Let $B_1,B_2$ be boxes of complete source cubes, each side comparable to $R$, with gaps comparable to $R$ in **each** of the four coordinates. Require that both directed periodic gaps in each coordinate exceed $cR$. The upper comparability on the shorter gaps can be dropped. Suppose $R\gg1$ and take a fixed ratio of gap to side. Then the actual cross-covariance $K=1_{B_1}S1_{B_2}$ satisfies
\[
     \|K\|_{2\to2}\le C\{\delta+(1+\log R)^2/R\}.                 \tag{93}
\]
The bound covers every pair of unit lattice $\ell^2$ source arrays in these boxes, with arbitrary oscillation and concentration. If all links outside two slightly enlarged, disjoint interiors are revealed, conditional independence of these interiors makes $K$ exactly the cross-covariance of the two *conditional means*. No control of their covariance inside the same interior is used.

To prove (93), first use any one separated coordinate as time. On the transverse lattice let $G(t)$ be the operator obtained by taking the time-$t$ covariance column. At real integer separation with both transfer powers positive this is the actual kernel. The representation in (O.34), tested against a real spatial vector $h$ at both insertions, gives a positive weighted sum of the exponentials $e^{-(t-1)E}$ and $e^{-(n-t-1)E}$. Its analytic continuation away from the endpoints has magnitude at most the real-time value at $\operatorname{Re}t$, bounded by $CA\|h\|_2^2/R$ when both real gaps exceed $cR$. For noninteger real times use the neighboring integers separately for the increasing and decreasing exponentials and (O.57). The transverse convolution is symmetric on real integer times and in the continued transfer trace by transverse spatial inversion, which reflects both cube anchors with the same bounded origin shift. Equivalently use cosine and sine modes paired under momentum reversal. Polarization gives the operator norm bound $CA/R$ on the same complex domain for arbitrary transverse arrays. Equal-energy terms are constant and retained; null transfer states disappear at the interior times in use.

Split each normal interval into boundedly many subintervals, with their lengths at most a fixed small fraction of the normal gap. For an input time $s$, approximate $G(t-s)$ on any output subinterval by its operator Taylor polynomial of degree below $k$ about the midpoint. A disk of radius at least twice the half-width stays in the preceding domain, so the error is $CA2^{-k}/R$, uniformly in $s$. Restricting the transverse input/output supports is contractive. Summing the resulting time blocks in operator Schur norm costs $O(R)$. Thus if $P_i$ is the orthogonal projection on piecewise normal-coordinate polynomials of degree below $k$ on the actual integer output sites (transverse coefficients arbitrary), $\|(I-P_i)K\|\le CA2^{-k}$. The adjoint gives the same input assertion. In every separated coordinate the same proof applies independently. Telescoping the commuting output projections and the commuting input projections gives
\[
     \|K-P_{B_1}K P_{B_2}\|_{2\to2}\le CA2^{-k},
       \qquad \operatorname{rank}P_{B_j}\le Ck^4.                 \tag{94}
\]
Only a one-variable continuation was used at each application. With just one separated coordinate the corresponding directional statement still holds for all transverse arrays, with the projection unrestricted in those transverse coordinates.

For clarity, on an interval of length $D\asymp R$ a scalar polynomial $p$ of degree below $k$ has endpoint norm squared at most $C k^2 D^{-1}\|p\|_{L^2}^2$ by the normalized Legendre basis, and $\|p'\|_{L^2}\le Ck^2 D^{-1}\|p\|_{L^2}$ by the Legendre derivative expansion and Cauchy–Schwarz. In the first inequality the norm is in continuum coordinate units. The sum of squared samples differs from the continuum integral by at most $C k^2 D^{-1}\|p\|_{L^2}^2$ using the integral of $|(p^2)'|$ and the endpoint term. Hence for $k^2\ll R$ the discrete and continuum norms are comparable. The sum of squared internal mesh differences is bounded by the continuum derivative norm squared, by integration over each mesh interval. Jumps at subdivision endpoints and at the zero extension cost $Ck^2/R$ in squared-norm units. These inequalities also hold for Hilbert-valued coefficients by summing coordinates. Consequently every unit vector in a projected tensor space, extended by zero, has $\|\nabla f\|_2^2\le C(k^2/R+k^4/R^2)$. For $f,g$ projected in the two disjoint boxes the constant $AI$ has zero cross-pairing. Positivity of $AI-S$, its grid estimate above, and Cauchy–Schwarz give $|\langle f,Kg\rangle|\le C(\delta+k^2/R+k^4/R^2)$. Choose $k=\lceil2\log_2(2+R)\rceil$ in (94). This proves (93) for large $R$, with bounded sizes absorbed into constants.

For boxes separated in just one coordinate the same proof bounds the cross-covariance of two sources with prescribed small transverse discrete-gradient norms by adding those squared norms to the right side of (93). The normal projections commute with transverse differences after zero extension. In particular arbitrary normal-time profiles, including oscillatory profiles, are allowed for a smooth transverse smearing. For fully unrestricted transverse inputs, (94) still removes all high normal polynomial components. An estimate on surviving low normal components with rough transverse inputs, or the dimension-eight point law at a physical separation, does not follow from (93).
