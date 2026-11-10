# Local tensor sources and the normalized boundary score

**Catalogue item:** F-03, computation of the seven actual first mixing coefficients.\
**Result:** an explicit localized tensor Ward identity, its exact normalized Gaussian boundary-score term, and a checked finite model showing why the uniform-source cancellation cannot be applied to a local row without its divergence remainder. **F-03 is not completed.**

## 1 Scope and inherited inputs

[The actual tensor coefficient and its gauge, source, and regulator identities](../lattice_theory/observable_i.md) already computes the seven coefficients of the whole-lattice covariant regular mean. T9.33 there and N9.19--N9.26 of [Bounded finite parts and the actual regular mean metric](../lattice_theory/observable_iii.md) identify its constrained Gaussian trace, including classical stable feedback, the actual physical quotient, finite parts and cutoff terms. In the F-01 ordering

$$\left( S,T_{d},W_{d},T_{o},W_{s},P,W_{p} \right),$$

its inherited universal vector in $u_{j} = Y_{j}^{- 1}$ units is

$$\gamma = \left( 0, - d_{B}, - \frac{18}{11}d_{B}, - d_{B}, - \frac{18}{11}d_{B},0, - \frac{18}{11}d_{B} \right),\quad\quad d_{B} = \frac{22N^{2}\log L}{24\pi^{2}}.$$

(LS20.1)

The raw mean coefficient also contains the bounded finite-part difference $\mathcal{F}_{j} - \mathcal{F}_{j + 1}$⁠. These inherited coefficients and that difference are not newly computed here. A common fixed field normalization at both endpoints conjugates the mean matrix and leaves its seven scalar entries unchanged; different endpoint normalizations do not.

The unresolved identification in F-03 concerns the actual retained-background conditional output and its inherited stable part. A uniform-source trace does not alone give its local response, its separately recorded current, or its geometric dependence. The calculation below identifies one precise term in that gap. It applies to an arbitrary frozen finite determining geometry. It neither assumes its hypercubic invariance nor treats an independent current as a physical constrained minimum.

## 2 The finite lattice derivative

Use current lattice units in this section. Let $a = \left( a_{\ell} \right)$ be a real Cartan-valued link perturbation on a finite periodic lattice. Pick a Cartan generator $H$ and normalize its invariant inner product to one; the general normalization multiplies every bilinear below by $\langle H,H\rangle$⁠.

Let $\mathsf{C}$ be the linearized clover curl from real link cochains to the six oriented curvature components. Its entries are the signed sum of the four elementary plaquette curls in F-01, divided by four. All sums use the same link and site counting convention. Write $\mathsf{C}^{*}$ for its adjoint. For a constant two-form $f$⁠, periodic summation of a discrete curl gives

$$\mathsf{C}^{*}f = 0.$$

(LS20.2)

Take $J \in E = {Sym}^{2}\left( {\mathbb{R}}^{6} \right)$ and a real site weight $\psi$⁠. Use $sf$ as a formal constant-curvature test, with $s$ its amplitude. This is not a claim that an arbitrary continuous $s$ gives a periodic compact-link field: periodic flux is quantized. An application to actual periodic backgrounds must use compatible quantized fluxes and the fixed-depth cover/local-germ limit of T9. The finite cochain identities below require only the formal curvature coefficient and periodic fluctuation cochains; no flux integer is differentiated.

The quadratic curvature germ of the scalar-repaired F-01 insertion, with the convenient one-half source convention, is

$$\mathcal{O}_{J,\psi}(sf,\tau a) = \frac{1}{2}\sum_{x}^{}\psi_{x}\left( sf + \tau\mathsf{C}a(x) \right)^{\mathsf{T}}J\left( sf + \tau\mathsf{C}a(x) \right) + \mathcal{R}_{J,\psi}^{sc}(\tau a).$$

(LS20.3)

Here, writing $(da)_{A,p}(x)$ for the consistently oriented curl on the four plaquettes of clover $A$⁠,

$$\mathcal{R}_{J,\psi}^{sc}(\tau a) = \frac{TrJ}{12}\tau^{2}\sum_{x,A}^{}\psi_{x}\left\lbrack \frac{1}{4}\sum_{p = 1}^{4}(da)_{A,p}(x)^{2} - \left( \mathsf{C}a \right)_{A}(x)^{2} \right\rbrack.$$

(LS20.3a)

Equation (LS20.3) specifies the quadratic Taylor germ, rather than identifying the nonlinear compact insertion with a quadratic polynomial at arbitrary fields. The scalar repair is generally nonzero in its $\tau^{2}$ term: the mean of four squared plaquette curls is different from the square of their mean. Its coefficient at $s\tau$ does vanish. To check this, expand a plaquette as $I + i\, sf_{A} + O\left( s^{2} \right)$⁠. The derivative of its Wilson action at order $s\tau$⁠, averaged over the four oriented plaquettes, equals the derivative of one-half the corresponding clover square. Thus the repair $2w - Trq$ has no additional coefficient at that mixed order. An off-Cartan perturbation has zero linear color trace against the Cartan background.

The actual smeared F-01 component $\sum_{x}^{}\psi_{x}\langle J,\widetilde{q}(x)\rangle_{E}$ is twice this convenient half-source insertion. Its absolute derivative and score terms are therefore twice those displayed below. Its relative multiplicative coefficient is unchanged, because the classical coefficient is doubled as well.

The first fluctuation derivative in (LS20.3) is

$$\left. \ \partial_{\tau}\mathcal{O}_{J,\psi} \right|_{\tau = 0} = s\langle\mathsf{C}^{*}(\psi Jf),a\rangle.$$

(LS20.4)

This identity holds for all 21 tensor directions. If the actual constrained fluctuation inclusion at the flat background is $a = Ez$⁠, the corresponding vector in the free coordinates is

$$\ell_{J,\psi,f} = E^{*}\mathsf{C}^{*}(\psi Jf).$$

(LS20.5)

No inverse of an unconstrained zero mode appears in this formula.

### Proposition LS20 A The local source is a divergence

For each link $\ell$⁠, choose any site $x_{\ell}$ in its fixed clover stencil. Then

$$\lbrack\mathsf{C}^{*}(\psi Jf)\rbrack_{\ell} = \sum_{x,A}^{}\mathsf{C}_{xA,\ell}\left( \psi_{x} - \psi_{x_{\ell}} \right)(Jf)_{A}.$$

(LS20.6)

Consequently, with a fixed stencil constant $c_{cl}$⁠,

$$\parallel \mathsf{C}^{*}(\psi Jf) \parallel_{\infty} \leq c_{cl} \parallel J \parallel \,|f|\,{osc}_{cl}(\psi),$$

(LS20.7)

where ${osc}_{cl}(\psi)$ is the largest difference of the site weights within one such stencil. If $\psi_{x} = \varphi(hx)$ for a differentiable physical test,

$${osc}_{cl}(\psi) \leq c_{st}h \parallel \nabla\varphi \parallel_{\infty}.$$

(LS20.8)

**Proof.** Subtract $\psi_{x_{\ell}}$ from the weight in the adjoint sum. Its constant part vanishes by (LS20.2), separately for each constant curvature component. Each link belongs to a fixed number of clover stencils, with fixed coefficients. Taking absolute values proves (LS20.7). The mean-value theorem on the bounded physical stencil gives (LS20.8). $▫$

Thus the uniform-source cancellation is exact already before estimating the propagator: $\ell_{J,1,f} = 0$⁠. For a local or smoothly varying source it produces a discrete divergence, with an explicit first spatial difference. This is a statement about the insertion, not an assertion that the conditional law is translation invariant.

## 3 Exact normalized boundary score contribution

At one finite frozen chart let $z$ be a centered Gaussian with positive precision $K$⁠, covariance $C = K^{- 1}$⁠, and the actual linear constraint inclusion $E$⁠. Let $V_{\tau}(z)$ denote an additional log-density term, and $F_{\tau}(z)$ an insertion, both twice differentiable near zero with enough Gaussian integrability to differentiate. Suppose $V_{0} = 0$ and $F_{0}$ is independent of $z$⁠. Define

$$\langle F_{\tau}\rangle_{\tau} = \frac{{\mathbb{E}}_{C}\left\lbrack F_{\tau}e^{V_{\tau}} \right\rbrack}{{\mathbb{E}}_{C}\left\lbrack e^{V_{\tau}} \right\rbrack}.$$

(LS20.9)

Differentiating numerator and denominator twice, without dropping the denominator, gives

$$\left. \ \frac{d^{2}}{d\tau^{2}}\langle F_{\tau}\rangle_{\tau} \right|_{0} = {\mathbb{E}}_{C}F''_{0} + 2\,{Cov}_{C}\left( F'_{0},V'_{0} \right).$$

(LS20.10)

All terms involving $F_{0}V''_{0}$ and $F_{0}\left( V'_{0} \right)^{2}$ cancel because $F_{0}$ is constant in the integrated variable. This formula is an exact finite-dimensional derivative identity. An unbounded-volume Taylor remainder is not inferred from it.

For an actual action contribution $W$⁠, the log-density contains $- W$⁠. Its linearized score on a constant-curvature test can be written

$$V'_{0}(z) = - s\,\langle b_{f},Ez\rangle + O\left( s^{2} \right),\quad\quad F'_{0}(z) = s\,\langle\mathsf{C}^{*}(\psi Jf),Ez\rangle + O\left( s^{2} \right).$$

(LS20.11)

When the indicated terms are the respective linear-in-$s$ parts and their constant parts vanish, their contribution to the $\tau^{2}s^{2}$ coefficient is exactly

$$\boxed{- \left\langle \mathsf{C}^{*}(\psi Jf),\, G\, b_{f} \right\rangle,\quad\quad G = ECE^{*}.}$$

(LS20.12)

For a weighted quadratic Wilson action $\frac{1}{2}\sum_{x}^{}w_{x}\left| \text{curvature}(x) \right|^{2}$⁠, the vector $b_{f}$ is the adjoint of that action's plaquette curl applied to $wf$⁠. If the same clover quadratic discretization is used, it is $\mathsf{C}^{*}(wf)$⁠. The distinction between the Wilson plaquette curl and the clover curl must be retained when evaluating the actual finite-lattice integral; their equality is not assumed.

The source-to-current map $E$⁠, the Gaussian precision $K$⁠, and every scale factor remain in $G$⁠. Replacing $G$ by the unconstrained free propagator would change the formula.

If $\parallel G \parallel_{1 \rightarrow 1} \leq c_{G}$⁠, Proposition LS20 A yields

$$\left| \langle\mathsf{C}^{*}(\psi Jf),Gb_{f}\rangle \right| \leq c_{cl}c_{G}\, \parallel J \parallel \,|f|\,{osc}_{cl}(\psi) \parallel b_{f} \parallel_{1}.$$

(LS20.13)

This is a useful local response estimate whenever the actual $G$ and score satisfy its displayed norms. It exposes the boundary-score mass $\parallel b_{f} \parallel_{1}$⁠, instead of replacing it by a volume-independent constant. An anchored version follows by using the corresponding weighted row or column norm and retaining the score carrier.

### What is and is not eliminated

For $\psi = 1$⁠, (LS20.12) vanishes for every $b_{f}$⁠, including a nonconstant boundary weight. This extends the use of uniform-source stationarity to this particular score term without requiring a separately covariant old action. The stationary uniform-source argument itself is already present in T9; the new calculation supplies its localized divergence and its exact score pairing.

For a point source or a cell indicator, ${osc}_{cl}(\psi)$ is generally of order one. There is no small factor from (LS20.13). A smooth test gives the physical $h$ in (LS20.8), but the remaining propagator and score-carrier norms must still be bounded. A pointwise carrier-current estimate in M-03 is stronger than this smeared divergence estimate.

If a fixed retained old field produces a nonzero $s^{0}$ score, or the input has additional inherited vertices, their mixed Taylor terms must be kept as well. Equations (LS20.11)--(LS20.12) isolate only the stated linear-by-linear contribution. They do not assert that it is the entire coefficient of a general retained-history jet.

## 4 An exact two cell calculation

The following computation checks the sign, denominator, and distinction between local and uniform sources. It is a constrained Cartan quadratic model, not a claim that a two-cell Gaussian is the full nonabelian Wilson measure.

Let $z$ have standard Gaussian reference law, let $\lambda > 0$⁠, and put

$$b_{1} = s + \frac{\tau z}{\sqrt{2}},\quad\quad b_{2} = s - \frac{\tau z}{\sqrt{2}}.$$

(LS20.14)

The fluctuation leaves $b_{1} + b_{2} = 2s$ fixed. Tilt the reference law by $\exp\left\lbrack - \lambda b_{1}^{2}/2 + \lambda s^{2}/2 \right\rbrack$⁠, so that the added log density is zero at $\tau = 0$⁠, as in (LS20.9). The constant recentering cancels in normalization. With $d = 1 + \lambda\tau^{2}/2$⁠, completing the square gives

$${\mathbb{E}}_{\tau}z = - \frac{\lambda\tau s}{\sqrt{2}\, d},\quad\quad{Var}_{\tau}z = d^{- 1}.$$

(LS20.15)

For the local insertion $F_{loc} = b_{1}^{2}/2$⁠, its exact normalized expectation is

$${\mathbb{E}}_{\tau}F_{loc} = \frac{s^{2}}{2d^{2}} + \frac{\tau^{2}}{4d}.$$

(LS20.16)

Thus its critical scalar factor relative to the classical $s^{2}/2$ is

$$M_{loc}(\tau) = d^{- 2} = 1 - \lambda\tau^{2} + O\left( \tau^{4} \right).$$

(LS20.17)

The $- \lambda\tau^{2}s^{2}/2$ term is exactly (LS20.12), using $v = (1, - 1)/\sqrt{2}$⁠, $\psi = (1,0)$⁠, and $w = (1,0)$⁠.

For the uniform insertion $F_{sum} = \left( b_{1}^{2} + b_{2}^{2} \right)/2$⁠, direct substitution gives

$${\mathbb{E}}_{\tau}F_{sum} = s^{2} + \frac{\tau^{2}}{2d} + \frac{\lambda^{2}\tau^{4}s^{2}}{4d^{2}}.$$

(LS20.18)

There is no order-$\tau^{2}s^{2}$ correction. Its uniform-source fluctuation derivative is zero. Equations (LS20.16) and (LS20.18) come from the same positive normalized law; the discrepancy is entirely the location of the insertion. This is why an exact uniform Ward cancellation does not remove the separate local score from a transported point row.

No conclusion about the size of an actual Yang--Mills boundary remainder follows from this example. The example verifies an algebraic obstruction to dropping that remainder without proof.

## 5 Remaining uniform estimate

The original F-03 statement asks for seven coefficients of the actual regular transported one-field outputs in the fixed normalization. A completion still requires the following identifications on the admitted retained-background class.

1.  The actual input row and its inherited stable part must be matched to the source used in the critical projection. The classical source Hessian alone does not identify an arbitrary already transported jet.
2.  The local divergence and every other proper/exterior score must either be included in a controlled remainder or shown to give the required negligible critical contribution. Formula (LS20.13) states the propagator and score norms needed for this contribution.
3.  The conditioned geometry must be carried through the coefficient projection. At one fixed non-invariant exterior, the conditional map need not commute with the seven projectors. Averaging that exterior with arbitrary new weights would change the target law.
4.  The inherited bounded finite-part difference must be retained, or removed by an explicitly permitted change of intermediate coordinates. It is not an $O\left( u_{j}^{2} \right)$ error merely because its endpoints are bounded.

Catalogue item C-05 concerns a common boundary continuation and the carrier sums needed in item 2. Even a successful native contour theorem would not, by itself, identify all inherited marked vertices or prove all direct/current records in M-03. No dependency is marked complete by substituting the homogeneous calculation for these checks.

**Status:** F-03 remains open. The new contribution is the explicit local tensor divergence, the exact normalized score pairing, and its finite positive-law verification. The previously established seven mean coefficients in (LS20.1) are cited as inputs and are not counted again.

## References

- Annex X, F.3--F.17: fixed 21-component clover family, scalar repair, and projectors.
- Annex Y, M.3--M.12: separate retained differences and kernel currents, with the current-scale carrier norm.
- [The actual tensor coefficient and its gauge, source, and regulator identities](../lattice_theory/observable_i.md), §9, T9.31--T9.34, and [Bounded finite parts and the actual regular mean metric](../lattice_theory/observable_iii.md), §§6--7, N9.19--N9.26: inherited stationary uniform source trace and finite parts.
- Observable normalization analysis, Section 5: exact outstanding F-03 identification and normalization conventions.
- Theorem CB, and Theorem MG: admitted all-age coupling trajectory and common physical matching. They supply the numerical coupling convention in (LS20.1), not the missing marked identification.
