# Actual heterogeneous precision and conditional law estimates

The estimates below concern the stated law. For all-history application, see [the composed-response criterion](../continuum/partial_gauge_transport.md).

## 1 Hessian and reconstruction identities

CMP 99, p. 428, (3.156)–(3.158) gives the identity of $\mathsf{C}$ on free bonds, and the explicitly stated uniform gap. CMP 119, p. 268, (3.15) identifies the actual inherited B argument is the genuine minimum $U_{k}( \cdot )$ at every real current $z$⁠, with the coarse fluctuation inside that map. 

**CMP99, pp.391--392, (3.7)--(3.12).** The physical Hessian contains the curvature-dependent contribution as well as the covariant curl-square. It is not the free Maxwell Hessian. The Lie-algebra scalar product uses normalized fundamental trace, $tr1 = 1$⁠.

**CMP99, pp.393--396, (3.16), (3.35)--(3.36).** The operators depend on the actual nested domains. The regularity conditions are imposed on local two-layer cubes in their own meshes. They allow nonconstant fields and different layer geometries. They do not require regularity outside the specified active domain.

**CMP99, p.399 after Theorem 3.2; Theorem 3.4.** Constants are independent of the sequence of domains satisfying the source geometry assumptions. The propagator estimates have analytic continuation in the native background neighborhood (3.37), with the actual mesh weights retained.

**CMP99, pp.423--426, Theorems 3.12--3.13.** The added background-current/constraint terms are retained in the propagators; their regularity and decay use both (3.35) and (3.36). The covariant-Laplacian exception in those theorems is not used below.

**CMP99, pp.427--428, (3.155)--(3.158) and following paragraph.** The unit-lattice constrained precision is $\mathsf{C}^{*}\Delta^{(k)}\mathsf{C}$⁠. The map $\mathsf{C}$ solves exceptional-bond constraints and is the identity on the independent free bonds. The source explicitly states a positive lower bound $\gamma_{0}$ independent of $k$ and $U$ for arbitrary $U$ satisfying (3.35)--(3.36), once $M\alpha_{0}$ is sufficiently small; it also states uniform exponential decay of this precision.

**CMP99, p.432, Theorem 3.15, (3.187).** The actual unit-lattice covariance has an exponential kernel bound with constants independent of the admitted depth/background. The inverse of a newly chosen principal block is not identified with a restriction of a full inverse; the direct argument below handles principal restrictions.

**CMP102, pp.277--279, (1), (7)--(10), Theorem 1.** Admitted determining data give a genuine minimizing orbit with the layered local regularity needed in CMP99. This is the real background used in the conditional expansion.

**CMP102, pp.308--309, (190), Proposition 9.** The minimizing map is analytic on the native regular background domain and has the stated mesh-weighted response bounds. An arbitrary raw fine-link polydisc is not substituted for this native domain.

**CMP119, pp.267--270, (3.15)--(3.25); Annex W (3.8), (3.11), (3.15).** These identify the actual precision and complete perturbation, including the physical sign of the heterogeneous action, and retain the present interior/exterior Gaussian cross term.

The precision gap here is a gap of a **conditioned RG fluctuation form in current lattice units**. It is not a physical Yang--Mills Hamiltonian mass-gap theorem and gives no E-05 thermal trace estimate by itself.

### Trace normalization

Use the Euclidean Hessian of the exact physical exponent in C-01 throughout. If free coordinates are orthonormal for the source product $tr(XY)$⁠, the source gap is directly $\gamma_{0}$⁠. If they are instead unscaled Hilbert--Schmidt coordinates with $Tr\left( T_{a}T_{b} \right) = \delta_{ab}$⁠, the quadratic potential Hessian carries the fixed factor $1/N$⁠: the corresponding gap is $\gamma_{0}/N$⁠. All precision and perturbation constants must undergo the same fixed conversion. Nothing depends on cutoff or age in this conversion.

## 2 Exact admissible class and law

Fix the source parameters $L,M,R_{\min}$ and small regularity ceilings. At an admitted finite stage $k$⁠, retain the live geometry, graphs, determining data, coupling labels and older fluctuation/history parameters. Let $v$ denote those data. The background $U_{k + 1}(v)$ is the genuine real constrained minimum, with CMP99 (3.35)--(3.36) satisfied at the source's fixed margins. A new C-05 theorem must keep those actual domains; a formal cap that does not reproduce all determining constraints is not enough.

Let $I$ be the current regular free-bond coordinates and $O$ the current retained exterior free-bond coordinates. Write $y = \left( y_{o} \right)_{o \in O}$ for the latter. These are current unit-lattice variables. Earlier-layer fields are retained parameters in $v$ and in the complete action; they are not silently added as an unweighted cloud of current free variables.

The completed C-07 support theorem gives the exact source-normal-form regular marginal on

$$D = \prod_{i \in I}^{}D_{i},$$

(CQ20.1)

where each $D_{i}$ is the actual symmetric convex free-bond norm ball. These radii are fixed while the retained field values vary in one admitted chart. Use the established C-02/C-03/C-04 normalization, with actual current support contained in $\parallel z \parallel_{\infty} \leq P_{k}$⁠, $P_{k} = A_{1}\left( \log g_{k}^{- 2} \right)^{p_{0}}$⁠. No alternative interpretation of the printed source cutoff is introduced.

Let $\mathcal{K}$ be the full current precision identified in C-01 and put

$$Q = \mathcal{K}_{II},\quad\quad b = - \mathcal{K}_{IO}y.$$

(CQ20.2)

Then the actual law is

$$d\nu_{s,b,v}(z) = Z_{s,b,v}^{- 1}\mathbf{1}_{D}(z)\exp\left\lbrack - \frac{1}{2}z^{T}Qz + b^{T}z + sW(z;v) \right\rbrack\, dz,\quad\quad 0 \leq s \leq 1.$$

(CQ20.3)

At $s = 1$ this is the full regular conditional law. The interpolation is an analytic device on its same support. The source-normal-form projection of the **whole incoming jet** remains necessary if a mark originated on the finer positive history space.

Decompose the actual logarithmic perturbation once as

$$W = W^{ER} + W^{B,full}.$$

(CQ20.4)

The first term is exactly the regular E/R family of DS.1. The second contains every remaining term in CM.6: nonlinear classical and gauge remainders, Haar/constraint factors, inherited B, E/R terms assigned to B by the source, the heterogeneous Wilson difference with its physical negative-action sign, and complete relocation with its Jacobian. Any variable-dependent old-operation factor present in the chosen exact representation is also included. Present Gaussian cross force $b$ and its outer Schur scalar are kept in (CQ20.2) and the outer law; older cross-component terms already assigned to B remain in $W^{B,full}$⁠.

## 3 The exact named boundary input

### Input B20 complete current coordinate remainder budget

The following is the required output of the C-05 boundary application, not an assumption that C-05 is already complete.

For every datum in the class of §2, every real point of $D$⁠, and the **same** current contour of radius $r_{z} = c_{G}P_{k}$⁠, suppose the full remainder in (CQ20.4) has the source-localized or proved quasilocal representation yielding

$$\sup_{i}\left| \partial_{i}W^{B,full}(0;v) \right| \leq \frac{C_{B,1}K_{B,k}}{P_{k}},$$

(B20.1)

$$\sup_{i}\sum_{j}^{}e^{\gamma_{B}d(i,j)}\sup_{z \in D} \parallel \partial_{i}\partial_{j}W^{B,full}(z;v) \parallel \leq \frac{C_{B,2}K_{B,k}}{P_{k}^{2}}.$$

(B20.2)

The same native background/current/preparation radii and all their source map margins must be retained in the accompanying derivative estimates. They need not equal the regular-E radii and cannot be assigned those radii by notation. The representation must reproduce the actual conditional action, not just its value at a physical center.

A sufficient explicit prefactor is the **complete** BV.17 one:

$$\begin{matrix}
K_{B,k} \leq C_{src}\left( 1 + S_{b_{0},\delta} \right)\lbrack{\mathfrak{K}}_{E} + C_{R}g_{k}^{\kappa_{0} - 11} + B_{0}\ell_{k}^{p_{0} - q} \\
 + g_{k}P_{k}^{3} + g_{k}P_{k} + g_{k}^{- 1}P_{k}e^{- c_{col}MR_{k}} + g_{k}^{\nu}\rbrack,
\end{matrix}$$

(B20.3)

where $\ell_{k} = \log g_{k}^{- 2}$⁠, $q > p_{0}$⁠, $\kappa_{0} \geq 12$⁠, $R_{k} \geq \ell_{k}^{r}$ with $r > 1$⁠, $\nu > 0$ is one fixed permitted relocation power, and $S_{b_{0},\delta} = \sum_{a \geq 0}^{}(1 + a)^{b_{0}}e^{- \delta a} < \infty$⁠. All constants and exponents are fixed before reducing the common coupling ceiling. There is no hidden volume, old-age sum, or distance factor in them.

The full anchored carrier bound BV.15 plus a verified simultaneous polydisc gives (B20.1) and a Hessian row at each common real point by first Cauchy and BD.2. **That simultaneous row does not by itself prove (B20.2): the supremum in (B20.2) is inside the sum.** For exactly localized current carriers, the polynomial carrier-cardinality argument immediately below proves the stronger bound from the same exponential reserve, with a larger fixed constant. If the new cap produces quasilocal rather than finitely supported functions, its first- and second-response rows must instead prove these same final current-coordinate bounds, or its actual localized decomposition must supply them. Invoking finite-carrier Cauchy for an undecomposed quasilocal composition would not verify B20.

### A further consequence of the proposed prefactor

Besides $K_{B,k}/P_{k}^{2} \rightarrow 0$⁠, the prefactor actually gives

$$K_{B,k}/P_{k} \rightarrow 0\quad\quad\left( g_{k} \downarrow 0 \right).$$

(CQ20.5)

Indeed its separate terms after division by $P_{k}$ are bounded by fixed multiples of

$$\frac{{\mathfrak{K}}_{E} + C_{R}g_{k}^{\kappa_{0} - 11}}{P_{k}},\quad B_{0}A_{1}^{- 1}\ell_{k}^{- q},\quad g_{k}P_{k}^{2},\quad g_{k},\quad g_{k}^{- 1}e^{- c_{col}MR_{k}},\quad g_{k}^{\nu}/P_{k}.$$

Every term tends to zero; the fifth uses $R_{k} \geq \ell_{k}^{r}$⁠, $r > 1$⁠. This proves a small **zero-field force** from B20, not merely a small Hessian.

C-04 already supplies, in these same current coordinates, the pointwise simultaneous Hessian row and zero-field gradient bounds

$$\varepsilon_{ER,k} = \frac{4D_{\mathfrak{g}}{\widehat{K}}_{k}\mathcal{S}_{\gamma_{ER}}}{c_{G}^{2}P_{k}^{2}} \rightarrow 0,\quad\quad d_{ER,k} \leq C_{G,1}{\widehat{K}}_{k}\mathcal{S}_{0}/P_{k} \rightarrow 0.$$

(CQ20.6)

### Lemma CQ20 A the stronger absolute Hessian majorant from actual carriers

The fixed nonnegative matrix in CM.10 has a supremum over $z$ in **each entry**. To verify it without interchanging a supremum and a sum, let $n(Y)$ be the actual integer tree length in DS.2a--DS.4. A tree with $n$ edges has $n + 1$ vertices and meets at most $2^{4}(n + 1)$ current $M$-cubes. A cube contains at most $2d(M + 1)^{d}$ oriented nearest-neighbor bond types with $d = 4$⁠. Hence the number of current free-bond blocks on its carrier satisfies

$$\left| I_{Y} \right| \leq q_{d,M}\left( n(Y) + 1 \right),\quad\quad q_{d,M} = 2^{d + 1}d(M + 1)^{d},\quad d = 4.$$

(CQ20.6a)

A fixed enlargement in the source's equivalent cube convention only enlarges this one fixed constant. This count concerns current unit-lattice blocks; it does not count all fine degrees of freedom or archived variables in the original multiscale construction.

For the common translated scalar-coordinate polydisc of radius $r_{z} = c_{G}P_{k}$⁠, ordinary two-coordinate Cauchy gives, uniformly over its real centers,

$$\sup_{z \in D}\left| \partial_{ia}\partial_{jb}V_{k,Y}(z) \right| \leq 2{\widehat{K}}_{k}e^{- \widehat{\kappa}n(Y)}r_{z}^{- 2}.$$

(CQ20.6b)

The factor 2 covers a repeated scalar coordinate. Bound a block operator norm by the sum of its $D_{\mathfrak{g}}^{2}$ entry moduli and sum the nonnegative bounds. With

$$q_{\gamma} = A_{d}e^{- \left( \widehat{\kappa} - \gamma M \right)} < 1,\quad\quad\mathcal{S}_{\gamma}^{\lbrack 1\rbrack} = \frac{q_{d,M}B_{d}e^{\gamma Mc_{d}}}{\left( 1 - q_{\gamma} \right)^{2}},$$

(CQ20.6c)

the actual regular E/R Hessian has the stronger estimate

$$\begin{matrix}
\sup_{i}\sum_{j}^{}e^{\gamma d(i,j)}\sup_{z \in D} \parallel \partial_{i}\partial_{j}W_{k}^{ER}(z) \parallel \leq {\overline{\varepsilon}}_{ER,k}(\gamma) \\
{: =}\frac{2D_{\mathfrak{g}}^{2}{\widehat{K}}_{k}\mathcal{S}_{\gamma}^{\lbrack 1\rbrack}}{c_{G}^{2}P_{k}^{2}} \rightarrow 0.
\end{matrix}$$

(CQ20.6d)

**Proof.** Exact current-carrier locality makes a derivative zero unless both indices belong to $I_{Y}$⁠. Triangle inequality permits replacing the supremum of the complete Hessian entry by the sum of the uniform per-carrier bounds (CQ20.6b). For a fixed output block $i$⁠, sum first over the at most $q_{d,M}(n + 1)$ input blocks of a carrier, then over its at most $B_{d}A_{d}^{n}$ possible rooted carriers; use $d(i,j) \leq M\left( n + c_{d} \right)$⁠. The remaining sum is $\sum_{n \geq 0}^{}(n + 1)q_{\gamma}^{n} = \left( 1 - q_{\gamma} \right)^{- 2}$⁠, giving (CQ20.6d). The fixed source choices give bounded ${\widehat{K}}_{k}$ and $P_{k} \rightarrow \infty$⁠. The last limit is therefore uniform. ∎

The same proof verifies B20.2 from a complete finite-carrier B decomposition with its own admitted decay, radius and constants. It costs the fixed cardinality factor (CQ20.6a) and uses its residual exponential reserve. Unlike the dimension-free pointwise BD.2 bound, this stronger estimate intentionally pays that polynomial factor. No correction to the accepted C-04 pointwise theorem is required.

For any fixed $\gamma \leq \min\left( \gamma_{B},\gamma_{ER} \right)$⁠, define the actual absolute majorant

$$A_{ij} = \sup_{z \in D} \parallel \partial_{i}\partial_{j}W(z;v) \parallel ,\quad\quad d_{i} = \left| \partial_{i}W(0;v) \right|,$$

and bounds

$$\parallel A \parallel_{\gamma} \leq \varepsilon_{k}: = {\overline{\varepsilon}}_{ER,k}(\gamma) + C_{B,2}K_{B,k}/P_{k}^{2},\quad\quad d_{i} \leq d_{k}^{*}: = d_{ER,k} + C_{B,1}K_{B,k}/P_{k}.$$

(CQ20.7)

Thus B20 would provide both $\varepsilon_{k} \rightarrow 0$ and $d_{k}^{*} \rightarrow 0$ uniformly in the admitted retained data. This does not assume monotonicity of the coupling trajectory: use the supremum of these elementary majorants over $0 < g \leq g_{*}$ and then choose a single sufficiently small $g_{*}$⁠.

## 4 Direct actual precision theorem

From the checked CMP99 statement, after the fixed trace conversion, there are $\lambda_{*} > 0$⁠, $C_{K} < \infty$ and $\mu_{K} > 0$ such that

$$\mathcal{K} \geq \lambda_{*}I,\quad\quad \parallel \mathcal{K}_{ij} \parallel \leq C_{K}e^{- \mu_{K}d(i,j)}$$

(CQ20.8)

on the real admitted class, uniformly in stage, volume and permitted layer geometry. Here $d$ is a fixed current-unit bond metric; changing from the source's norm to this metric costs only fixed dimension-dependent constants.

Let

$$S_{a} = \sup_{i}\sum_{j}^{}e^{- ad(i,j)},\quad\quad R_{a} = \sup_{i}\sum_{j}^{}d(i,j)e^{- ad(i,j)}.$$

(CQ20.9)

These are finite with volume-independent bounds: the current free coordinates form a subset of a fixed finite number of bond types per site of a four-dimensional unit lattice. A periodic displacement can be chosen in one fundamental box and its sum bounded by the corresponding infinite-lattice exponential sum. The number of older retained/history variables is not counted in (CQ20.9).

Choose once

$$0 < \gamma \leq \min\left\{ \gamma_{B},\gamma_{ER},\mu_{K}/2,\ \frac{\lambda_{*}}{4C_{K}\max\left( 1,R_{\mu_{K}/2} \right)} \right\}.$$

(CQ20.10)

If B20 has not yet supplied $\gamma_{B}$⁠, the purely quadratic theorem holds with that entry omitted; the common value is fixed when the boundary theorem is instantiated.

### Theorem CQ20 1 principal block weighted inverse

For the actual $Q = \mathcal{K}_{II}$⁠,

$$Q \geq \lambda_{*}I,\quad\quad \parallel \left( Q^{- 1} \right)_{ij} \parallel \leq \frac{4}{3\lambda_{*}}e^{- \gamma d(i,j)}.$$

(CQ20.11)

In particular, for $0 < a < \gamma$⁠,

$$\parallel \,\left| Q^{- 1} \right|\, \parallel_{a} \leq \frac{4}{3\lambda_{*}}S_{\gamma - a}.$$

(CQ20.12)

**Proof.** A principal restriction has the same lower bound by extending a test vector by zero. For a fixed center $x$⁠, put $M_{i} = e^{\gamma d(i,x)}$⁠. The weighted conjugation defect has row and column Schur bounds at most

$$a_{K}(\gamma): = \sup_{i}\sum_{j}^{} \parallel \mathcal{K}_{ij} \parallel \left( e^{\gamma d(i,j)} - 1 \right) \leq \gamma C_{K}R_{\mu_{K}/2} \leq \lambda_{*}/4.$$

(CQ20.13)

The middle inequality uses $e^{\gamma r} - 1 \leq \gamma re^{\gamma r}$ and $\gamma \leq \mu_{K}/2$⁠. It holds on every principal block. Hence $MQM^{- 1} = Q + E_{x}$⁠, $\parallel E_{x} \parallel \leq \lambda_{*}/4$⁠, and its inverse has norm at most $4/\left( 3\lambda_{*} \right)$ by a convergent resolvent series. Choose $x = j$ and read the $(i,j)$ block of the inverse to obtain (CQ20.11); summing gives (CQ20.12). ∎

This is a genuine direct consequence of the actual primary-source precision bound. It does not infer the inverse of a principal restriction from a submatrix of a full covariance.

## 5 Concrete C 06 application gate

### Theorem CQ20 2 complete law coercivity and weighted covariance conditional only on B20

Assume B20 has been proved on §2's actual class. Reduce the common source coupling ceiling until

$$\boxed{\quad\varepsilon_{k} \leq \varepsilon_{*}{: =}\min\left\{ \frac{\lambda_{*}}{4},\frac{\lambda_{*}}{4S_{\gamma/2}} \right\}\quad\text{at every admitted step.}\quad}$$

(CQ20.14)

Then all the laws (CQ20.3), including every real linear tilt, have Hessian at least $\lambda_{*}/2$ on their true product support. They satisfy

$$\left| {Cov}_{\nu_{s}}(f,g) \right| \leq \sum_{i,j}^{}G_{ij} \parallel \nabla_{i}f \parallel_{L^{2}\left( \nu_{s} \right)} \parallel \nabla_{j}g \parallel_{L^{2}\left( \nu_{s} \right)},\quad\quad G_{ij} = \frac{2}{\lambda_{*}}e^{- \gamma d(i,j)}.$$

(CQ20.15)

The same constants give CM.9 for a coordinate block. For $a = \gamma/2$⁠,

$$\parallel GA \parallel_{a} \leq \frac{1}{2},\quad\quad \parallel (I - GA)^{- 1}G \parallel_{a} \leq \frac{4}{\lambda_{*}}S_{\gamma/2}.$$

(CQ20.16)

**Proof.** The complete potential is $V_{s}(z) = \frac{1}{2}z^{T}Qz - b^{T}z - sW(z)$⁠. The absolute Hessian majorant is symmetric, so its unweighted row bound controls its operator norm. Hence $\nabla^{2}V_{s} \geq \left( \lambda_{*} - \varepsilon_{k} \right)I \geq 3\lambda_{*}I/4$⁠, and a further linear tilt changes no Hessian.

For a spatially weighted Neumann estimate, the precision conjugation costs at most $a_{K}(\gamma) \leq \lambda_{*}/4$⁠, and the complete perturbation costs at most $\parallel A \parallel_{\gamma} \leq \lambda_{*}/4$⁠. Thus the numerical margin is at least $\lambda_{*}/2$⁠. The product-domain boundary is exactly the one proved in C-07: block-scalar weights preserve its tangency condition, and its second-fundamental-form term has the favorable nonnegative sign.

More explicitly, the differentiated Neumann operator on vector fields is $\mathcal{L}^{(1)} = L \otimes I + \nabla^{2}V_{s}$ with that convex-product boundary form. Multiplication by $M_{i} = e^{\gamma d(i,x)}$ commutes with the scalar differential part and preserves the boundary domain. Its inverse has weighted operator norm at most $2/\lambda_{*}$⁠. Choosing the center at one block gives $\parallel \left( \mathcal{L}^{(1)} \right)_{ij}^{- 1} \parallel_{L^{2} \rightarrow L^{2}} \leq \left( 2/\lambda_{*} \right)e^{- \gamma d(i,j)}$⁠. The differentiated Neumann equation and $Cov(f,g) = \langle\nabla f,\left( \mathcal{L}^{(1)} \right)^{- 1}\nabla g\rangle$ give (CQ20.15) by summing block pairs. Smooth convex approximations and Sobolev density pass this to the literal source norm balls, exactly as in C-07; no cutoff derivative is discarded.

Finally $\parallel G \parallel_{a} \leq \left( 2/\lambda_{*} \right)S_{\gamma/2}$⁠, and (CQ20.14) implies $\parallel GA \parallel_{a} \leq 1/2$⁠. The positive Neumann series and weighted row-norm submultiplicativity prove (CQ20.16). ∎

This supplies both distinct numerical conditions in Annex AB: the covariance/coercivity margin and the force-resolvent margin CM.12. One is not silently substituted for the other.

All native external derivative estimates retain the actual source radii. CMP99's regular-background analytic continuation and CMP102 Proposition 9 supply the quadratic native chart; C-04 and B20 supply the interaction slots on their common admitted chart. Cauchy differentiation in a direction with native radius $\rho$ costs that $\rho^{- 1}$⁠, not one. No arbitrary raw fine-link direction or history-interface derivative has been added to the C-06 conclusion.

## 6 Exact retained force and mean envelopes

Let

$$H = (I - GA)^{- 1}G,\quad\quad h_{a} = \frac{4}{\lambda_{*}}S_{\gamma/2},\quad\quad\sigma = \sqrt{2D_{\max}/\lambda_{*}},\quad\quad a = \gamma/2.$$

Under CQ20.2, CM.1 now applies with its covariance hypotheses verified, giving

$$M_{i}: = \sup_{0 \leq s \leq 1}\left| \nu_{s}z_{i} \right| \leq \sum_{j \in I}^{}H_{ij}\left( \left| b_{j} \right| + d_{j} + \sigma\sum_{l}^{}A_{jl} \right).$$

(CQ20.17)

The exterior force itself has the actual bound

$$\left| b_{j} \right| \leq C_{K}\sum_{o \in O}^{}e^{- \mu_{K}d(j,o)}\left| y_{o} \right|.$$

(CQ20.18)

Combining the two kernels gives the explicit local envelope

$$\boxed{M_{i} \leq h_{a}C_{K}\sum_{o \in O}^{}e^{- ad(i,o)}\left| y_{o} \right| + h_{a}\left( d_{k}^{*} + \sigma\varepsilon_{k} \right).}$$

(CQ20.19)

**Proof.** For each fixed $i,o$⁠, the triangle inequality gives

$$\begin{matrix}
e^{ad(i,o)}\sum_{j}^{}H_{ij} \parallel \mathcal{K}_{jo} \parallel \leq \sum_{j}^{}H_{ij}e^{ad(i,j)} \parallel \mathcal{K}_{jo} \parallel e^{ad(j,o)} \\
 \leq C_{K} \parallel H \parallel_{a} \leq C_{K}h_{a}.
\end{matrix}$$

Insert (CQ20.18) into (CQ20.17), use $d_{j} \leq d_{k}^{*}$ and $\sum_{l}^{}A_{jl} \leq \varepsilon_{k}$⁠, and sum. ∎

The unrestricted Gaussian conditional mean is $- Q^{- 1}\mathcal{K}_{IO}y$ and has the analogous bound from CQ20.11. The mean of the **truncated** Gaussian on $D$ need not equal that vector. Equation (CQ20.19) concerns the actual selected conditional laws, including truncation and interaction.

For all $p \geq 1$⁠,

$$\parallel z_{i} - \nu_{s}z_{i} \parallel_{L^{p}\left( \nu_{s} \right)} \leq C\sqrt{p/\lambda_{*}}.$$

(CQ20.20)

Indeed every real linear tilt has the same Hessian lower bound, so the logarithmic moment-generating function of a centered block component has second derivative at most $2/\lambda_{*}$⁠. Integrating twice, applying exponential Markov, and integrating the tail proves (CQ20.20). The fixed block dimension is the only additional constant.

These are volume-uniform **conditional** estimates with the retained field dependence exposed. They do not bound its outer distribution or its cumulants; H-04/H-05 retain that work. A collar estimate such as CM.41 further requires the actual numerical mean margin. If a separately verified exterior bound is $\left| y_{o} \right| \leq Y_{k}$ and $d(i,O) \geq R$⁠, then

$$\sum_{o \in O}^{}e^{- ad(i,o)}\left| y_{o} \right| \leq Y_{k}e^{- aR/2}S_{a/2}.$$

(CQ20.21)

This makes a deep-interior margin check explicit. It does not assert such a distance or exterior ceiling at every boundary site. Neither convexity nor product support alone gives the margin.

## 7 The remaining C 08 clauses

Even if B20 is proved and CQ20.2 thereby instantiated, the Annex AB §6 list still requires the actual projected marks

$$\overline{F}(z;v) = {\mathbb{E}}\left\lbrack F^{aug} \mid z,v \right\rbrack$$

and the full projected incoming jet to satisfy field and gradient envelopes such as CM.21--CM.22, with fixed factorial source-order growth and actual retained-coordinate dependence. C-07 proves this projection is exact; it does not prove those envelopes.

A uniform convex marginal does not regularize arbitrary conditional marks. If a hard old label is determined by retained links and is erased while those links remain, its projected mark can still be the hard selector. The explicit P0 example in [the history-kernel note](native_history_kernel.md), Section 5, demonstrates this at a finite cutoff. It is not a claim about every native R operation; it shows why a generic "conditional expectation smooths the mark" inference is invalid.

Once actual envelopes are proved, CQ20.19--CQ20.20 insert directly into CM.24; the bilinear covariance bound CQ20.15 and the established cut-cumulant argument give the fixed $(m!)^{2}$ bound and the order-dependent decay range in CM.25. At present those actual mark hypotheses are not verified by the quadratic theorem, by C-04, or by a native boundary contour alone. Their direct derivatives, kernel currents, full footprints, higher incoming vertices and retained force factors must all be retained in the stated requirement.
