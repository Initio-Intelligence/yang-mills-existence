# A two-step transfer bound and the Wilson pseudoscalar

Fix SU(N), a finite cubic spatial lattice of even side n≥4, Wilson coefficient β=2Nx₀, and the original compact transfer operator T=AKA on the gauge-invariant Hilbert space of spatial links. Here A=exp(−V_s/2), K is the tensor product of the normalized central one-link convolution kernels, λ=||T|| and P=T/λ=exp(−aH). Work initially with finite β>0. All comparison constants below are uniform under sup log(1+β)/n<∞. This is the compact reserve geometry of Annex A; no assumption on F-05 or the interacting RG mark is made.

## A rectangular Wilson reserve with no temporal aspect-ratio cost

The elementary Wilson proof of Annex A (2.1)–(3.4) works on even periodic rectangles of sides n₁,…,n_d≥4. In its notation, for V=∏n_i one has q_P=(d−1)V+1 and q_P−q_F=V∑n_i⁻¹, by counting wrapping links. The spanning-tree restriction on the periodic box gives the identical lower bound c^{q_P}(1+β)^{-D q_P/2}, D=N²−1. On the open box use the same axial forest in the last coordinate, a spatial spanning tree at its first slice, and its recursively selected first-slice plaquettes. Integrating each remaining chain from its upper end gives z(β) per free variable, exactly q_F factors. The local Haar estimate for z is unchanged. Hence the per-site comparison Z(β/2)/Z(β) costs at most C_{N,d}(1+β)^{(D/2)∑1/n_i} after the V-th root. The site-reflection chessboard inequality is iterated one coordinate at a time with even block count in each coordinate. Each closed unit cube disseminates to all V translates/reflections, and every plaquette is counted M_d=2^{d−2} times. It follows at 0≤η≤1/(2M_d) that

    E exp(ηβ Σ_{p∈X} s_p) ≤ [C_{N,d}(1+β)^{(D/2)∑1/n_i}]^{b(X)}.    (1)

Here b(X) is the unit-cube cover number and a plaquette in X is counted once. No comparison of normalized expectations after deleting plaquettes is used. For sides n,n,n,2q and 2q≥n the bracket is ≤K=C_{N,4} exp(2D sup log(1+β)/n), independently of q. These are auxiliary compact Wilson trace integrals for one fixed spatial graph. The source-free multiscale theorem is used on no rectangle. Annex A, original matched count and reserve

## Arbitrary vectors and the temporal stencil

For a finite set of plaquettes X on two adjacent time intervals, closed under reflection about their common time slice, define B as the transfer over these intervals with exp(ηβ∑_{p∈X}s_p) inserted. Retain the original magnetic half weights at the two endpoints and the full weight at the middle. The temporal-gauge representation integrates the middle spatial links. B is a continuous compact self-adjoint kernel: reflection interchanges the two endpoints and leaves its real weight unchanged. Its kernel is pointwise nonnegative, and gauge invariance makes it an operator on the physical Hilbert space. Repeating the normalized transfer trace gives exactly

    Tr_phys B^q / Tr_phys T^{2q}
      = E_{n,n,n,2q} exp(ηβ Σ_{j<q} Σ_{p∈X+2j} s_p).                (2)

The one-link convolution normalizations cancel. The projectors onto the physical subspace insert the original temporal links (or the periodic seam gauge average); all stencil weights are invariant under their native gauge change. Centered clover stencils have a fixed multiplicity bound b₀ under these repetitions, including endpoint faces. Choose η≤1/(8b₀) and apply (1) to the union, coverable by q times a fixed b_X. The ratio in (2) is at most K^{q b_X}. Along even q, Tr B^q=∑|b_i|^q, independently of whether every spectral value is positive. At fixed spatial cutoff, both kernels are Hilbert–Schmidt; the q-th root limits give ||B|| and λ² respectively. There is no surviving finite-dimensional trace factor and no uniform vacuum-projection rate is needed.

Let M_f be the same two-step operator for a real or complex gauge-invariant insertion f, divided by λ². For any physical unit vectors its matrix element in absolute value is bounded by the positive majorant evaluated on their absolute values, which are again physical. In particular, if |f|≤C_X ∑_{p∈X}s_p, then

    ||M_f|| ≤ C_X K^{b_X}/(eηβ).                                    (3)

Use xe^{-ηβx}≤1/(eηβ). More generally an analytic family with pointwise modulus bounded by the same exponential can be integrated on a fixed complex disk. Centering at its ground or periodic Wilson mean subtracts that scalar times P²; the ground mean is bounded by (3), and the periodic mean on the cubic reserve class obeys the same order by (1). Arbitrary outer heat contractions preserve (3). This is one common Wilson time direction and a bound on a finite-support spacetime slab. It does not identify M_f with equal-time multiplication for temporal insertions.

For the actual based clovers, ||C_A||²_HS≤C∑_{p∈A}s_p by unitarity, the four-term average and Hilbert–Schmidt contraction of the traceless projection. Hence every Tr(C_A C_B) and the Wilson scalar trace repair satisfy the premise of (3) with fixed stencil. For the genuine bare pseudoscalar the ground and periodic means vanish by a spatial reflection. The off-diagonal magnetic seed also has a vanishing mean by a coordinate reflection, as do its genuine projected temporal partners with that parity. After the seven real F.33 coefficients, restoration of dimension four gives the rigorous upper bound C a⁻⁴ max_h|z_h|/β for each of these two centered seeds. Spatial or positive-time slab translations can be summed with the lattice L¹ norm of the test; their absolute weights add. This covers actual temporal admixtures and removes the logarithmic loss of the bare Annex Q majorant. The engineering factor remains.

## A signed identity for the actual pseudoscalar

Use temporal gauge on an open two-step slab and independent outgoing spatial bonds at its central time. Write B₁=C₂₃, B₂=C₃₁, B₃=C₁₂, all at x, and p=Σ_i Tr(C₀ᵢ B_i) in the precise X convention. On smooth functions of the central spatial configuration u let L_{x,κi,H} differentiate the outgoing bond U_{κi}(x) in exp(i tH)U_{κi}(x). For κ=− this varies the corresponding independent positive i-link by right multiplication exp(−i tH). Set D_B=∑_{i,κ=±} κ L_{x,κi,B_i(x)}. B_i uses only bonds in the complementary plane, so is independent of the bond it differentiates. The vector field is divergence free for Haar product, transforms covariantly at x and preserves gauge-invariant smooth functions. It is smooth and complete on the finite compact link manifold. Its skew realization generates a measure-preserving unitary flow.

For either neighbor configuration v the temporally oriented plaquette through the outgoing central bond is v_{κi}(x)u_{κi}(x)^{-1}, with the orientation of the time displacement accounted for by the sign σ in X (F.4). Direct differentiation of the central convolution density gives

    L_{x,κi,B_i(x)} log K(u,v)
      = β Tr[B_i(x) (v_{κi}u_{κi}^{−1}−(v_{κi}u_{κi}^{−1})†)/(2i)].

The trace kills the identity part. Thus βp is one quarter of D_B log K(u,v_+)−D_B log K(u,v_−). For two endpoint vectors put l=KAψ and r=KAφ. In the exact matrix element the central integral is one quarter of ∫A²[conj(l) D_B r−conj(D_B l)r] dHaar. Replacing Al and Ar by Tψ and Tφ cancels both D_B A terms pointwise. Haar integration by parts gives the exact identity on the closed finite-cutoff Hilbert space, initially on smooth vectors,

    β M_p = ½ P D_B P.                                                 (4)

P maps into smooth functions at fixed β and finite spatial size; (3) gives the bounded extension, and the adjoint identity makes M_p skew. The fixed Minkowski pseudoscalar Wick phase makes it self-adjoint up to its specified real normalization. In particular the Euclidean forward/backward clover here is a signed insertion, even though the positive majorant in (2) used both time intervals. This expression uses the actual magnetic central field and the original compact electric transfer; there is no polar change of the Hamiltonian.

## A uniform relative energy gain for the time-odd channel

In (4) the earlier endpoint is the bra and the later endpoint is the ket. Transform the physical Hilbert space by its strictly positive normalized ground state Ω. The transfer P then acts as a reversible Markov operator on π=Ω² dHaar and the bilinear insertion is E[conj(f(X))p g(Y)] on the stationary two-step chain, including its central variables. This is just conjugation by Ω: the two-step path has endpoint factors Ω(X)Ω(Y) and normalization λ⁻². Positivity and uniqueness of the top eigenvector of the strictly positive compact Wilson kernel imply its gauge invariance. The same statements therefore apply to the invariant endpoint Hilbert space. On reversing the two steps the based real p changes sign, with its spatial B at the same center. Write

    D(f)=〈f,(I−P²)f〉=½ E|f(X)−f(Y)|².

The exponential majorant (2) and β|p|≤C_X βΣ s give, for u≥1 and h=p 1_{β|p|≤u},

    ‖M_{p−h}‖ ≤ C β⁻¹ exp(−c u),       ‖M_{h²}‖ ≤ C β⁻².              (5)

Indeed in each inequality dominate the absolute integrand by a constant times exp(ηβΣ s), retaining the displayed tail by using half the exponent. For normalized f put δ_f=√D(f). Reversibility and |h|≤u/β imply

    E[h² |f(X)|²] = Re〈f,M_{h²} f〉 + ½ E[h²|f(X)−f(Y)|²]
                    ≤ C β⁻²(1+u²δ_f²).

The earlier endpoint can equally be the later endpoint in this identity. Twice the pairing with M_h equals the expectation of h times conj(f(X))g(Y)−conj(f(Y))g(X). Subtract and add conj(f(Y))g(Y), then use Cauchy–Schwarz, the last estimate and (5). The resulting bound times β is C(δ_f+δ_g+uδ_fδ_g+exp(−cu)). For δ=δ_f+δ_g in (0,1), choose u=max(1,c⁻¹log(1/δ)); then uδ²≤Cδ. For δ≥1 apply (3), and for δ=0 let u grow without bound. Homogeneity restores the vector norms and yields the finite-Wilson form estimate

    |〈f,M_p g〉| ≤ C β⁻¹ (‖f‖√D(g)+‖g‖√D(f)).                         (6)

These constants have the rectangular-reserve and stencil dependence of (2). In the original representation P=e^(−aH). Spectral calculus gives ‖(I−P²)^(1/2)e^(−tH)‖≤C min(1,√(a/t)) and ‖(I−P²)^(1/2)(1+H)^(-1/2)‖≤√(2a). Thus

    ‖e^(−tH) M_p e^(−sH)‖ ≤ C β⁻¹ min(1, √(a/t)+√(a/s)),
    ‖(1+H)^(-1/2) M_p (1+H)^(-1/2)‖ ≤ C β⁻¹ √a.                      (7)

The pseudoscalar ground mean is zero. Its actual F.33 insertion carries the additional factor a⁻⁴|z_odd| and its fixed convention constant. At fixed physical heat times (7) retains a⁻⁷ᐟ²|z_odd|/β. The argument supplies no corresponding reversal cancellation for a time-even insertion. A uniform engineered bound, the required continuum field domain, and the E-03/E-04 conclusions remain open.

For the spatial smearing of Annex Q (5.1)–(5.3), the engineered two-sided graph bound is explicitly
\[
 \left\|(1+H)^{-1/2} z_{\rm odd}a^{-4}
       a^3\sum_{x\in a\mathbb Z^3\cap\Lambda} g(x)M_{p(x)}
       (1+H)^{-1/2}\right\|
 \le C\frac{|z_{\rm odd}|}{\beta a^{7/2}}
       \left(a^3\sum_{x\in a\mathbb Z^3\cap\Lambda}|g(x)|\right).
\]
Here the torus is represented by one central spatial box. The final parenthesis is at most \(C\sup_x(1+|x|)^4|g(x)|\) for \(a\le1\), by a three-dimensional summable weight. Periodizing a Schwartz test obeys the same estimate after the triangle inequality. The spatial cell factor pays for the number of sites occupied by the test. No further power of \(a\) follows from this summation.
