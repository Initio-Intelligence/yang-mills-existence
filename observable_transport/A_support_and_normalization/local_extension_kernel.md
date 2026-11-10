# First clean Wilson step: physical localization and a coercive local extension

This note develops a constructive first-step result after the inactive-fiber diagnostic. It does not claim the complete M-04 statement or an all-history theorem.

## 1. The useful first-step fact in the primary construction

The background about which the variational construction starts need not be the final nonlocal minimizer U_1(V). In CMP 102 (1985), 277–309, Section A, printed p.280, the author explicitly takes, for k=1,

    U_0=V_0,

where V_0 is the lift constructed in (11). In the one-step notation of CMP 119, p.246, (1.3), this is the local lift Q^f V: internal fine links are identity, and each fine link crossing a specified coarse face carries that coarse link matrix. This lift has the exact coarse average V. Its dependence on the raw retained links is local.

This matters for physical support. Localizing a function of U_1(V) in the variables U_1 does not automatically localize it in raw V. Starting the variational equations at U_0=Q^f V avoids that inference. The propagators and local vertices of those equations depend on a local raw-V lift. The decoupling of CMP 116, Section 1, then has genuine raw-V support at the first step.

No corresponding assertion is made for an arbitrary later background containing completed residual components.

## 2. Exact force and energy identities for the local lift

Write

    S(U)=sum_p [N-Re Tr U_p],

and let J_e(U_0) be the original Wilson first variation at a fine link e, in a fixed orthonormal Lie-algebra basis. Up to the fixed source trace normalization,

    |J_e(U_0)| <= C_N sum_{p incident to e} sqrt(s((U_0)_p)),
    s(P)=N-Re Tr P.                                      (2.1)

**Proof.** A link derivative of a plaquette trace is a trace with one traceless generator. Subtracting the identity from the remaining plaquette factor and applying Cauchy–Schwarz gives a constant times ||P-I||_HS=sqrt(2s(P)). A fine link meets a fixed number of plaquettes. Summing proves (2.1).

The gauge-fixing term has zero first variation at this lift in the axial representative used for the first-step construction: the internal contour variables at Q^f V are identity. If a different representative is used, its actual gauge force must be kept; it cannot simply be called part of J and discarded.

Every elementary fine plaquette of Q^f V is either identity or a transported coarse plaquette holonomy. Therefore, on a finite carrier Y enlarged by the fixed averaging stencil,

    beta sum_{e in Y}|J_e(Q^f V)|^2
       <= C(N,L) sum_{p' in foot(Y)} beta s(V_p').         (2.2)

The multiplicity is a fixed power of L and is independent of the volume and coupling. The source convention is beta g^2=1/N when its Wilson action uses normalized trace. Replacing that convention by another fixed normalization changes only C(N,L).

Equation (2.2) controls the actual force, not a separately introduced Gaussian force.

## 3. A root majorant before Gaussian integration

### 3.1 The source's local contraction data

The following are properties of the actual first-step variational/constraint construction used here.

1. The reference U_0=Q^f V is local in the coarse raw links.
2. The variational equations are built from local analytic nonlinearities and the propagators H, H_0 and G. CMP 102, (143), displays the force term -GJ and nonlinear terms vanishing at zero. CMP 116, pp.2–5, (1.2)–(1.12), carries out the decoupling of these propagators and the associated nonlinear equations.
3. On the enlarged decoupling polydisc |s_Delta|<=exp(kappa_1), the source's operator bounds are uniform; their constants may contain exp(C kappa_1). The geometric small-field ceiling can be chosen sufficiently small, after fixing these constants, that the nonlinear fixed-point map has Lipschitz constant at most 1/2 on its prescribed ball.
4. The fluctuation constraint correction has zero value and zero first nonlinear remainder at zero fluctuation. It therefore adds O(g|z|) to the reconstruction on g|z|<=delta, with delta fixed sufficiently small.

The third property requires the **enlarged** source domain, not just the physical endpoint at s=1. Its parameter order is the same one used to establish CMP 116 (1.11)–(1.21). The all-regular first-step fields have epsilon_1(g)->0 and g P(g)->0, so they eventually lie within this fixed geometric ceiling.

### Lemma 3.1 (force-resolved decoupled reconstruction)

On a connected decoupling component Y containing the root stencil, the background correction and full fluctuation reconstruction satisfy

    sup_s |A_bg(s;V)|_infty
       <= C max_{e in Y}|J_e(Q^f V)|,                    (3.1)

    sup_s |A_fl(s;z,V)|_infty <= C g max_{i in Y}|z_i|.   (3.2)

All functions in these formulas depend only on the raw V and z coordinates in the enlarged Y.

**Proof.** Write the decoupled background equation as A=T_s(J,A), with T_s(0,0)=0. Its force-linear part is bounded by C||J||_infty and its nonlinear part has Lipschitz constant at most 1/2. At its fixed point,

    ||A||_infty <= C||J||_infty+(1/2)||A||_infty,

which proves (3.1). The analytic constraint correction vanishes quadratically in its input; together with the bounded linear free-coordinate embedding, this gives (3.2). Source transformations between the linearized and nonlinear field add bounded maps with a quadratic remainder and preserve these inequalities after changing C.

When s is set to zero outside Y, each propagator vanishes between distinct components. The local nonlinear equations consequently separate, as proved in CMP 116 following (1.9). U_0 and J are local functions of V. Hence the fixed point in Y and the root reconstruction depend only on data in Y. This proves actual raw-coordinate support, rather than deducing support from a numerical estimate. QED.

### Lemma 3.2 (complex scalar energy on each decoupling component)

Let F_h be the primitive scalar of SR20.1, with exposed budget b. For real compact retained V, on every source decoupling polydisc and the admitted fluctuation domain,

    |F_h(U(s,z;V))|
      <= C b h^(-4) [1+E_Y(V)+sum_{i in Y}|z_i|^2],       (3.3)

where E_Y(V) is the sum of the actual retained coarse plaquette energies beta s(V_p') in the fixed footprint of Y. A finite sum of root stencils changes C and the footprint by a fixed amount.

**Proof.** Expand the holomorphic Wilson trace about the real compact lift U_0. Each first trace derivative has a traceless generator, so its linear term is bounded by C sqrt(s((U_0)_p)) times the total relative increment. Its second-order Taylor remainder is bounded by the square of that increment, uniformly on the fixed small physical tube. Thus

    beta |mathsf s(U_p)|
      <= C beta [s((U_0)_p)+|A_bg|^2+|A_fl|^2].

Apply (3.1)–(3.2), replace the maxima by the sums of squares on Y, use (2.2), and use beta g^2=1/N. Add the identity coefficient from the exposed budget. This proves (3.3). The estimate is a positive majorant of the modulus of the complex trace; it does not assume positivity of the complex Wilson action. QED.

The background-only version is

    sup_s beta |mathsf s(U_1,p(s;V))| <= C E_Y(V).         (3.4)

It is the physical energy comparison needed by an adaptive marked-source disk. In particular, a polylogarithmic bound on the maximum background amplitude need not be substituted for E_Y(V).

### 3.2 The supported scalar expansion

Apply exactly the component decoupling identity CMP 116 (1.10) to the primitive scalar root reconstructed through the first-step equations. Its terms are indexed by connected source-block sets Y containing the root. Setting all decoupling parameters outside Y to zero gives the actual supported function before differentiation.

For n new decoupling blocks, Cauchy's formula on the source polydisc gives a factor

    (exp(kappa_1)-1)^(-n).                               (3.5)

Combining (3.3) with (3.5) gives, for the corresponding pre-integration root coefficient f_Y,

    |f_Y(z,V)|
      <= C b h^(-4) exp(-nu n(Y))
             [1+E_Y(V)+sum_{i in Y}|z_i|^2],
    nu=log(exp(kappa_1)-1).                              (3.6)

The source's fixed collars and regroupings only change the fixed geometric constants and may consume a fixed fraction of nu. The physical carrier is the footprint of Y in current coarse units. Each source block has a fixed volume in these units. Thus, for a fixed C_geo,

    |foot(Y)|+t(foot(Y)) <= C_geo n(Y)+C_root.              (3.7)

Choose the M-03 rate small enough that the remaining source rate exceeds C_geo kappa plus the connected-block entropy. This is a strictly positive fixed interval of allowed kappa after the source block sizes have been fixed. A claim for arbitrary large kappa is not made.

The Gaussian insertion theorem in [actual kernel](actual_kernel.md), G1–G3, then pays the quadratic part of every such root by a trace O(|foot(Y)|), using the same Gaussian mass as the unmarked source expansion. This proves a genuine first-clean **pre-Gaussian** physical localization and energy bound. Completing the normalized root operator still requires the marked source-family and denominator-cluster summation with the same extensions; that step must not be replaced by merely bounding the conditional mean.

### 3.3 The continued law must retain the exact critical cancellation

The modified background U_1(s;V) is not generally a Wilson critical point when s differs from one. It would be incorrect to define the decoupled law by substituting that field into the full original action and then deleting its linear fluctuation term. The resulting residual force could be of size sqrt(beta) times a background curvature and would destroy the intended polynomial energy estimate.

The decoupled law used by CMP 116 is the analytic continuation of the **already critical-cancelled complete normal form**: the constrained Gaussian and its full W terms, with the independent background/current slots and propagators changed according to the source formulas. At s=1 it is the exact original conditional law. Away from s=1 it need not be the Wilson action of a new stationary background. The root observable may be evaluated on the correspondingly modified reconstruction to obtain its localized expansion; this does not license changing the source-free law or asserting stationarity of the modified background.

This distinction also governs the off-support extension below. It extends the complete normal-form coefficients and the reconstruction separately. They coincide with the original Wilson kernel on the physical active support; outside that support a positive source-free extension is sufficient.

### 3.4 The first-step raw pullback of the complete native unmarked family

The following source-fit check is used by the marked theorem LC.6 in [local coupling source](local_coupling_source.md). Its scope is the buffered native first-clean graph. It is not a claim about the Gram-clipped ambient coefficients in Section 4.

At this step, before any inherited effective vertex is present, the complete non-Gaussian normal form consists of the Wilson Taylor remainder, the soft-gauge remainder, and the logarithmic Haar/coarea and exceptional-coordinate Jacobian terms. These are local analytic functions of the background/current slots, the finite local constraint solve, and the source propagators. CMP119 p.249, after (1.14), gives the local exceptional-bond solve; the source's Gaussian and density retain its Jacobian. Their dependence on the final minimizing field is composed with the force-resolved construction in Lemma 3.1. Thus the local slot functions and every propagator can be decoupled before their raw-V variables are summed. The complete native Gaussian and W are continued in their already critical-cancelled form, as in Section 3.3.

There are two connected localization operations in this composition: the background/constraint fixed point, and the conditioning/covariance operation of CMP116 (2.5)–(2.9). Use a common fixed enlargement of their block partitions, or keep two labelled decoupler copies and include the union of their footprints in each carrier. Setting the decouplers outside a component to zero disconnects each fixed point and each native generalized walk. Because the reference Q^fV and all primitive slot functions are local, the resulting component depends only on its declared raw retained variables. The second operation does not reintroduce an independently variable global U_1. The fixed number of decoupler copies changes the localization constants and rate margin, rather than creating a volume-dependent loss.

The required analytic-domain admission is quantitative. On the enlarged component polydiscs, the complex relative correction to the real compact Q^fV is bounded by C exp(C kappa_1) gamma, where gamma is the chosen first-step geometric curvature ceiling; its first differences have the same bound with fixed L-dependent factors. The native independent current slot is bounded by that ceiling as well. Choose gamma after kappa_1 and the fixed source block sizes. The smaller basic domain criterion of CMP109 p.263, following (1.16), then admits these fields into the source's full local spaces: its first three regularity conditions with sufficiently smaller constants imply its reconstructed-field condition (iv). This is especially simple at the first step; it does not resolve the joined multiscale determining-domain question for later histories. A normalized one-coordinate raw retained disc has physical radius O(g), so it lies in the same fixed buffer once g is sufficiently small.

For the final Gaussian localization retain the **simultaneous native formulas** for the conditioned covariance, covariance square root, precision and Gamma in CMP116 (2.5)–(2.8). On each such local family the comparison in (2.15)–(2.26) can use the real compact local lift as its unitary reference and set the independent current to zero. Its positive reference precision follows from the first-step gap lemma below, with the current-dependent correction set to zero. The difference between the composed complex background and that real lift contributes O(gamma exp(C kappa_1)) to the source's alpha_0+alpha_1 error. The walk modification contributes O(exp(-cM)), just as in (2.16). The nonlinear action contributes the source's separate alpha_4 reserve. Hence the joint completed-square comparison has an error parameter of the form

    alpha_5 <= C exp(-cM)
                 + C gamma exp(C kappa_1)
                 + C alpha_4 + y_2.                    (3.8)

All four contributions can be made sufficiently small in the source's stated parameter order. The determinant comparison costs exp(C alpha_5 |Z|), as in (2.17), (2.25), not an uncontrolled exp(C|Z|) with a fixed large coefficient. It is important that the four Gaussian objects use the same native conditioning formulas; a separately chosen absolute expansion of their summed kernels would not establish this comparison.

On the unchanged first-step free cutoff |z|<=P(g), the actual Wilson remainder is bounded by C g P(g)^3 and the Haar remainder by C g^2 P(g)^2; bounded lower-degree Jacobian terms fit the first bound for P(g)>=1. Here P(g) is the actual polylogarithmic cutoff, gP(g) tends to zero, and beta g^2 is fixed. The complete coefficient budgets therefore meet the same strict unmarked smallness inequalities for sufficiently small g. The force term of the original Wilson action is canceled only by its exact native critical identity; it is not reintroduced through a new saddle in this estimate.

These checks justify the full source-free first-step raw pullback needed by LC.5: the local action species, the actual fixed cutoff, and the simultaneous positive-reference Gaussian comparison all have the native source bounds and genuine raw supports. They remain upstream of the marked calculation, which adds and estimates one new scalar source species. Outside the native domain, the Gram construction proves a different positive density. Its real covariance locality alone does not transport the simultaneous comparison (3.8). Section 5 below identifies the separate exact-marginal construction that supplies the ambient Gaussian bridge.

## 4. Local extension without loss of coercivity

Cutting off the full precision separately on each local support can destroy positivity. A factor extension avoids that problem.

### Theorem 4.1 (Gram-factor extension)

Suppose a fixed-coordinate regular precision K(v) obeys K>=lambda_0 I on its admitted domain. Let the full non-Gaussian potential have a local decomposition W=sum_X W_X with Hessian majorant norm at most epsilon<lambda_0. Choose sigma with epsilon<sigma<lambda_0 and set

    B(v)=(K(v)-sigma I)^(1/2).

Assume B has an absolutely convergent expansion into genuinely supported coefficients B_X, and that each W_X and B_X has a buffered local domain D_X^+ containing the restrictions of all active data. Let eta_X be a retained-only smooth cutoff, equal to one on those active restrictions, supported inside D_X^+, and between zero and one. Extend each coefficient by zero after multiplying by eta_X. Define

    B_ext=sum_X eta_X B_X,
    K_ext=sigma I+B_ext^T B_ext,
    W_ext=sum_X eta_X W_X.                               (4.1)

Then on every real ambient retained datum,

    Hess_z[ (1/2)z^T K_ext z-W_ext(z;v)]
      >=(sigma-epsilon)I.                               (4.2)

On the active data, the extended law agrees exactly with the original law. It is a positive normalized probability on the same free product support.

**Proof.** The Gram form gives K_ext>=sigma I without a commutation or diagonal-dominance assumption. Because eta_X depends only on retained variables, Hess_z(eta_X W_X)=eta_X Hess_z W_X. Its absolute majorant is therefore no larger than the original coefficientwise majorant. This proves (4.2). All cutoffs equal one on the active set, so B_ext=B, K_ext=K and W_ext=W there. Normalizing the finite positive integral gives the asserted probability. QED.

Every product in B_ext^T B_ext has the union of its two genuine supports, plus the common matrix index footprint. Hence the construction creates explicit carrier products, not a hidden global cutoff. Weighted summability follows from the usual overlapping-carrier product estimate once the coefficient sums are available.

The new retained derivative is explicit:

    D(eta_X B_X)=eta_X DB_X+(D eta_X)B_X,
    D(eta_X W_X)=eta_X DW_X+(D eta_X)W_X.                  (4.3)

At fixed source block size, a local cutoff with a fixed geometric collar has a controlled raw derivative. In the normalized coarse-link direction its size is O(g) times that derivative. Summing the directions belonging to X costs a polynomial in |X|, paid by a spare rate. This statement requires the cutoff's actual footprint; it does not permit treating a global regularity test as a local scalar.

### 4.1 Constructing local retained cutoffs

At the first step the primitive regularity tests are local coarse curvature and the specified local gauge/current tests. On a fixed local domain, a smooth cutoff between two separated real thresholds can be chosen gauge invariant by using the spectrum of the positive matrix (P-I)^*(P-I), or by compact gauge averaging an already supported cutoff. Compact gauge averaging changes neither the local footprint nor uniform derivative bounds. The cutoff is one on the inner test domain and zero before the boundary of the enlarged native domain.

This construction must use a quantitative inclusion of the inner domain in the enlarged chart. A mere assertion that a point belongs to an open chart is insufficient. The first-step local lift and the fixed geometric variational ceiling provide such a margin after the admitted coupling is made small. More complicated inherited chart conditions have not been treated here.

### 4.2 A necessary warning about a square-root path argument

A binomial series with ||A||_2<1 proves convergence of sum c_n A^n as an operator. It does **not** prove convergence of the sum of absolute path/carrier coefficients. In general || |A| || can exceed one, even though ||A||_2<1. Grouping A^n into its entire n-neighborhood pays a volume of order n^4 and does not solve this problem.

The useful source construction is the buffered local-resolvent expansion. CMP 116, pp.12–14, especially (2.7), explicitly obtains the square root of the covariance from resolvent random walks. The same positive-gap functional calculus can be used for the Gram factor, provided the local resolvents have the genuine raw-V support and absolute walk estimates. At the first step, starting at Q^f V and applying the nonlinear decoupling of Section 3 is the route to those supports. For later completed histories this input is not established merely by C-08's covariance bound.

### 4.3 A correct carrier-algebra construction of the Gram factor

Here is an explicit route that uses a binomial series only where it contracts in the **absolute carrier algebra**, rather than only in operator norm.

For an operator with a supported representation A_ij=sum_X A^X_ij, where X contains both matrix-coordinate footprints, use the two-sided row/column norm

    ||A||_nu,loc
      = max { sup_i sum_j sum_X exp[nu(|X|+t(X))]
                    sup_{v in D_X}|A^X_ij(v)|,
              sup_j sum_i sum_X exp[nu(|X|+t(X))]
                    sup_{v in D_X}|A^X_ij(v)| }.          (4.4)

Fixed local matrix components can be included in i,j; block operator norms give an equivalent convention with fixed factors. Products are submultiplicative: an X-term and a Y-term meeting through the intermediate matrix index have carrier X union Y, and its weight is at most the product of the two weights. Transposition or adjunction is an isometry, as needed for the Gram product and coefficientwise Hermitian pairing. This is a norm of the represented operator coefficients and does not use cancellation between different carriers.

#### Lemma 4.2 (the actual local-reference gap at the first step)

For the first-step precision at U_0=Q^f V, with the literal local constraint elimination and soft axial gauge retained, there are fixed gamma>0 and lambda>0 such that

    K_0(V)>=lambda I                                     (4.4a)

whenever all coarse plaquette curvature norms are below gamma. Constants depend on L,N and the fixed source conventions, not on the torus volume. The geometric torus must accommodate the fixed local patches; the source's compatible large tori do so.

**Proof of the flat gap.** At identity background the quadratic form is a fixed positive multiple of the curl-square plus the soft axial contour-square,

    ||d a||^2+||tau a||^2,

on the linear constraint Q a=0, with a=C_0 z. Here tau is the **average** of the shortest-contour linear sums specified by CMP 109 (0.8), (0.11), as used in CMP 119 (1.5); it is not silently replaced by a fixed tree gauge. The constraint-Hessian correction proportional to the Wilson first variation is zero at identity. All coefficients and the eliminated-coordinate embedding are periodic with one coarse cell and have finite range.

Consider its finite-dimensional Bloch matrix at any coarse quasi-momentum. A zero vector has d a=0 and tau a=0. Because the fine curl is zero, all shortest internal contour integrals from a fixed center to a fixed vertex agree; their average therefore equals each individual contour integral. Every internal block-edge integral equals the difference of those contour integrals from the block center. They vanish by tau a=0, so all internal block links vanish. Fine links crossing a given adjacent-block face have the same value, since their differences are sums around contractible fine plaquette loops. Every averaging path defining Q then has that same face value, because its internal portions are zero. Q a=0 sets the face value to zero. Thus a=0, including quasi-periodic and zero-momentum modes. Since C_0 is identity on the remaining free coordinates, z=0 as well.

Each Bloch matrix is therefore positive definite. It depends continuously on quasi-momentum in a compact torus, so its least eigenvalue has a positive minimum lambda_flat(L,N). Discrete momenta of every finite periodic torus are a subset of that compact parameter set. This proves a volume-independent flat gap. Fixed positive trace/gauge normalizations merely rescale lambda_flat.

**Passage to weak coarse curvature.** The local-reference precision is finite range: the source's nonlinear constraint linearization changes only b_0(c), and its linear elimination uses the two adjacent blocks; the Wilson, axial and current-dependent constraint Hessians have fixed local stencils. Its coefficient functions are analytic in those local compact background/current variables near the flat orbit. A fixed local coefficient bound K_* is available on a sufficiently small geometric regularity domain. Here K_* can be taken to mean the sum of the suprema of the individual finite-stencil entries, avoiding an interchange of supremum and sum.

Choose a partition of unity sum_Q chi_Q^2=1 on free-coordinate blocks with supports in cubes of side O(M), fixed overlap and Lipschitz constant C/M. Take M large enough that the finite-range matrix IMS error is less than lambda_flat/4. Explicitly,

    sum_Q chi_Q (K_0)_Q chi_Q-K_0

has entries -1/2 sum_Q(chi_Q(i)-chi_Q(j))^2 K_0(i,j), so its operator norm is at most C K_* r^2/M^2. This estimate is algebraic and does not assume positivity of K_0 in advance.

On each Q with its fixed coefficient halo, use a coarse axial gauge. If the coarse plaquette curvature is at most gamma, the gauged retained links on this fixed patch differ from identity by at most C(M)gamma. This follows by writing each non-tree link as a product of at most C(M) plaquettes; the compact product estimate is uniform. The block-constant fine lift of this coarse gauge preserves Q^f and acts orthogonally on the free coordinates, as in CMP 119 (1.17). Consequently the gauged principal precision differs from the flat principal precision by at most C(L,N,M)gamma in operator norm. This comparison includes the nonlinear constraint correction J_0 D'' because (2.1) gives J_0=O(gamma), and its remaining local derivatives are bounded. No stationarity of U_0 is assumed.

Choose gamma, after fixing M, so C(L,N,M)gamma<=lambda_flat/4. Every principal block then has lower bound 3lambda_flat/4. Summing the localized quadratic forms and subtracting the IMS error gives K_0>=lambda_flat/2. This proves (4.4a), with lambda=lambda_flat/2. The order M first, gamma second is essential. The actual all-regular epsilon_1(g) tends to zero, so it eventually obeys this fixed geometric condition. QED.

Let K_0(V) be the source's constrained quadratic-form extension evaluated at the local reference U_0=Q^f V, with the actual local independent-current values. It includes the soft-gauge quadratic term and the nonlinear-constraint quadratic correction. It does not include a logarithmic Haar/coarea term a second time: the latter and all higher Wilson terms belong to W. The free-coordinate embedding C is the same actual exceptional-bond elimination, with its background dependence retained.

Write

    K(V)=K_0(V)+E(V),

where K(V) is the actual precision at the minimizing background. The local analytic dependence of the quadratic coefficients on the background and current, together with (3.1) and the component Cauchy expansion, gives

    ||E||_nu,loc <= C a_1                                  (4.5)

on a geometric regularity domain with ceiling a_1, after consuming fixed localization slack. This coefficient difference vanishes when the background correction vanishes; it is not estimated by the sum of the two O(1) precision norms.

The source form of K_0 is finite range in raw V at the first step. CMP 119, p.249, after (1.14), states that the nonlinear linearizing transformation changes only the exceptional bonds b_0(c). The equation Q A'=0 expresses each exceptional value through the remaining bonds in the two adjacent blocks B(c_-) and B(c_+). Thus its free-coordinate embedding C(U_0) is local. The Wilson quadratic form, the one-block soft gauge form, and the constraint-Hessian correction are also local in U_0 and its actual local current. Since U_0=Q^f V is local, their composition K_0=C^* Delta C has a fixed raw-V range and footprint. A logarithmic Jacobian is not being included in Delta and again in W.

Given the native positive gap K_0>=mI and its bounded local coefficients, Theorem PR.1 in [physical carrier resolvent](physical_carrier_resolvent.md) therefore supplies represented kernels

    R_0(t)=(K_0+t I)^(-1),
    ||R_0(t)||_nu,loc <= B/(1+t),    t>=0.                (4.6)

The parameter t acts on the independent free coordinates. PR.1 constructs (4.6) directly from buffered principal-block inverses and an absolutely small commutator error. Its local matrix coefficients are exactly functions of their raw retained footprints. This removes the need to infer a uniform absolute carrier bound from the source's informal statement that a positive-mass resolvent has the same random-walk properties. A spectral norm bound alone would not imply (4.6).

A separate argument handles the all-t issue. On any fixed compact t interval, the positive extra term retains the local compression gap. For t>=2||K_0||_nu,loc, the series

    R_0(t)=t^(-1) sum_{n>=0}(-K_0/t)^n

converges in the absolute carrier algebra and has norm at most 2/t. The direct parametrix proof is stronger: it gives the same all-t bound at once.

Choose a_1 so that B||E||_nu,loc<1/4. Then

    (K+tI)^(-1)
      =sum_{n>=0}[-R_0(t)E]^n R_0(t),                   (4.7)

converges in that algebra, with bound (4/3)B/(1+t). The true covariance C=K^(-1) is its value at zero. Moreover

    C^(1/2)=(1/pi) integral_0^infty
                         t^(-1/2)(K+tI)^(-1) dt         (4.8)

converges absolutely coefficientwise because integral t^(-1/2)/(1+t) dt=pi. It therefore supplies a genuinely supported coefficient expansion of C^(1/2), rather than only its spatial matrix-element decay.

Now choose a fixed sigma>0 so small that

    sigma ||C||_nu,loc <1/4,

and take the admitted coupling small enough that the complete W-Hessian budget satisfies epsilon<sigma/2. Define

    T=(I-sigma C)^(1/2)
      = I+sum_{n>=1} binom(1/2,n)(-sigma C)^n.            (4.9)

This series **does** converge in the carrier algebra. Set

    B=K C^(1/2) T.                                      (4.10)

On real admitted data, the factors are commuting spectral functions of the same K, so B is exactly (K-sigma I)^(1/2). The carrier norm of B is bounded by the product of the finite norms in (4.8)–(4.10). This proves the coefficient expansion required by Theorem 4.1 from source-free precision/resolvent inputs.

First retained derivatives can be carried through (4.7)–(4.10) with the product rule. Differentiating a product of n covariance factors produces n terms and the summable scalar factor n r^(n-1), r<1/4. For local native coefficients, normalized retained derivatives follow by a one-coordinate Cauchy contour inside the fixed geometric buffer. Summing the directions on a carrier costs O(|X|); a spare rate absorbs that factor. The same applies to the explicit cutoff terms in (4.3).

This argument explains precisely why taking sigma small is useful: it gives contraction in the stronger algebra that remembers physical dependence, while the independently small first-step interaction budget allows epsilon<sigma/2. It is not an attempt to turn an arbitrary spectral contraction into an absolute polymer expansion.

### Source verification boundary for (4.5)–(4.6)

At the first clean step, U_0 is local and the actual free-coordinate quadratic form has the finite-range structure just identified. Lemma 4.2 supplies the local-reference gap from the literal flat constraint/gauge structure and its local analytic continuation. PR.1 then proves (4.6), and the component contraction proves the small supported difference (4.5). Their constants depend on the fixed source block sizes and geometric ceiling, not on total volume or the scalar mark.

There is no need to assume that every locally admissible field extends to a globally admissible one when defining the local inverse coefficients. A principal block A_Q has gap at least m on the actual active data. Include a local smooth spectral cutoff that is one for eigenvalues at least m and vanishes before the least eigenvalue reaches m/2. Its footprint is the block's exact coefficient footprint. This guarantees that every local inverse is evaluated on a genuine buffered positive domain. Its finite-dimensional derivative cost is retained just like the curvature cutoff cost. It does not assert positivity of an unrelated local operator outside that domain.

A full application must retain the exact domain/current convention of the source precision in these formulas. In particular, replacing its constrained quadratic form by an unconstrained curl operator, omitting its current-dependent constraint Hessian, or assigning a global raw footprint to a supposedly local reference would invalidate the construction. These are genuine source-free kernel obligations. No later completed-component version of (4.5)–(4.6) is claimed by this first-step argument.

### 4.4 Extending the reconstruction, not individual observable outputs

The density extension alone is insufficient. M-03 generates outputs recursively through a kernel and its coordinate reconstruction. A transported scalar cannot be assigned an unrelated extension after taking its conditional expectation.

At the first step, choose the fixed geometric ceiling sufficiently small that the exact relative microscopic link

    chi_e(z,V) (Q^f V)_e^(-1)

lies in a fixed neighborhood of identity on the entire admitted free cutoff, including the stated coordinate/gauge maps. A principal analytic logarithm then gives an exact Hermitian real-field correction

    chi_e(z,V)=exp(i Theta_e(z,V))(Q^f V)_e.

The same component decoupling of Section 3 gives Theta_e=sum_X Theta_e,X with genuine raw supports and, after fixed collars,

    |Theta_e,X|
      <= c_e,X [ (sum_{f in X}|J_f(Q^f V)|^2)^(1/2)
                    +g(sum_{i in X}|z_i|^2)^(1/2) ],     (4.11)

where the weighted sum of the coefficients c_e,X is finite. Each coefficient is Hermitian on real data: use the real fundamental-theorem-of-calculus localization formula, and use complex Cauchy only for its bound. Compact gauge transformations used in the original coordinate map must remain in chi. If a near-identity representative is obtained after a source gauge map, that map must be included or carried by its exact gauge averaging; gauge invariance of the scalar does not justify altering a general mark.

Use the same class of local retained cutoffs to define

    Theta_e,ext=sum_X eta_X Theta_e,X,
    chi_e,ext=exp(i Theta_e,ext)(Q^f V)_e.                (4.12)

The sum is Hermitian on real data, so chi_ext is a compact-link configuration. It equals the actual reconstruction on all active data. Consequently the extended old-state kernel is the pushforward of the positive extended z-law through chi_ext. Every microscopic mark is evaluated by its original global compact-link formula on that same old state. Positivity, the constant jet and products are therefore preserved; no marked output is extended independently.

For eta_X nonzero, its carrier data remain within the buffered native domain, and (4.11) retains its actual local force bound. When eta_X=0 the extended term is zero. Thus (4.11) remains an ambient majorant with the original local force J(Q^f V). The total correction is uniformly small because the supported coefficients are summable, the active local geometric threshold is small and gP(g) is small.

To expand the primitive scalar F(chi_ext), expand the local plaquette products of the exponentials in (4.12). The zeroth-order term is the coarse-lift scalar. The linear trace term contains the factor sqrt(s((Q^f V)_p)) by tracelessness. Every term of degree at least two contains two correction factors; use (4.11) on those two and the uniformly small bounded correction norm on the remaining factors. The power-series factorials and the overlapping-carrier product inequality give an absolutely supported expansion with the same energy grade as (3.6). In particular the pointwise root majorant still consists of genuine native coarse Wilson energy plus quadratic free-coordinate energy.

The direct current of this reconstruction is retained explicitly:

    DTheta_ext=sum_X[eta_X DTheta_X+(Deta_X)Theta_X].

A normalized coarse-link derivative of the local lift or force costs O(g). On a fixed geometric cutoff collar, Deta_X=O(g) per affected local test, with its actual carrier and a summed polynomial |X| loss. Thus the direct root estimate follows from the same shifted local energy majorant and the exact derivative of the compact plaquette. This is a reconstruction current calculation, not an assumption of total-variation differentiability of a moving point mass.

### 4.5 What the smooth cutoffs do and do not preserve analytically

The retained cutoffs are smooth, not holomorphic, in the raw retained field. They are independent of the integrated z variables. Hence they preserve the needed analyticity in the fluctuation variables. They also do not prevent analyticity in the **decoupling parameters**: at fixed retained V, the cutoff coefficient is a fixed real scalar, while the decoupling parameters enter the localized propagators and vertices in the specified analytic manner.

Retained derivatives are handled by the explicit product rule (4.3), not by pretending that a compactly supported cutoff is holomorphic. The native coefficient derivative is estimated on its genuine inner analytic domain; the extra cutoff derivative is estimated by its fixed collar. This distinction is needed when combining the extension with the marked Gaussian/cluster construction.

## 5. What a genuine one-step kernel input budget may contain

A useful induction hypothesis can concern the source-free kernel, without assuming the marked output that M-04 asks to prove. The following are legitimate kernel inputs:

1. A fixed free product support, complete positive density and an actual reconstruction map; the exact coarea, Haar and gauge factors are included once.
2. The positive-gap precision and its buffered local-resolvent/random-walk representation, with actual raw retained supports and summed first retained derivative bounds.
3. A local analytic decomposition of the complete non-Gaussian exponent with the small quadratic/Gaussian reserve used in CMP 116; its local retained cutoff extensions and their derivative costs are specified.
4. Local analytic constraint/variational vertices with their contraction margins on the **decoupling** polydiscs, not just on the physical integration contour.
5. The incoming scalar's exposed energy/analytic budget and its existing direct/current records before application of the kernel.
6. The actual outer native-energy moments needed by the averaged part of M-03.

None of these is the unknown absolute marked numerator sum SR20.23. They must nevertheless be proved for the actual source-free kernel. C-08's numerical covariance decay and conditional moments alone do not contain items 2–4.

For the first clean original Wilson step, items 1 and 4 have the source formulas and the local-lift explanation in Sections 1–3; the primitive scalar has the explicit bound (3.6). The first-step non-Gaussian terms consist of the Wilson nonlinear remainder and the exact Haar/coarea/gauge factors, without inherited E/B/R activities. The native marked summation is carried out in [local coupling source](local_coupling_source.md), Lemmas LC.5–LC.6, using the same complete denominator. At later steps, a full physical coefficient budget for inherited and completed-component terms remains an additional theorem.

### 5.1 The ambient Gaussian bridge through exact marginals

Theorem PR.2 of [physical carrier resolvent](physical_carrier_resolvent.md) strengthens the matrix input: a uniformly positive Hermitian precision with an absolute connected physical-carrier expansion has an inverse and inverse square root in that algebra at a smaller positive rate. In particular it applies to K_ext in (4.1), since the Gram form gives the gap and its coefficient products give a finite carrier norm. This proves real ambient Gaussian covariance locality. It does not assert that independently clipping its coefficients preserves the native complex conditioning family of CMP116.

The stronger construction is now proved in [ambient gaussian marginal](ambient_gaussian_marginal.md), GM.1–GM.21. For every Mayer/failed-cutoff support I, use its exact normalized Gaussian marginal with covariance C_II. Restrict the Gram coefficients to a buffered block union D by B^D=sum_{X subset D} B_X, so K^D=sigma I+(B^D)^T B^D stays positive. Apply the same PR.2 tag construction to every such restriction. A tag whose entire declared carrier is contained in D is identical to the unrestricted tag, including its local inverse cube halos. The difference C-C^D therefore has only carrier tags leaving D, with an exponentially small absolute tail at endpoints in I.

Attach external decouplers to this difference and use C^D_II as its positive local reference. Symmetric covariance tags make the same one analytic covariance define both its inverse and determinant. The small tail gives a uniformly positive real part of the precision and a determinant cost with a tunably small coefficient times |I|. The proof establishes exact factorization across disconnected components and equality with the independently calculated component families. It does not identify arbitrary coefficient masking with the inverse of a masked precision.

This supplies the source-free Gaussian input for the ambient clipped interaction without importing the native Gamma/covariance-square-root identities. The exact interaction and hard-cutoff expansion uses ordinary Gaussian marginals on the union of its actual supports. GM.22–GM.27 differentiate the same covariance, determinant and exponent using the complete retained coefficient budgets and the explicit cutoff product rule. Theorem GM.4 then combines these ingredients with the scalar source and the exact M.30 endpoint split to give a full-ambient **continuous-direction** theorem at this fixed first-clean geometry.

## 6. Status of this construction

**Proved here from the explicit first-step source equations:** the local lift force inequality, the force-resolved decoupled scalar majorant, the resulting genuine raw-V pre-integration root support, and the native source-free pullback check in Section 3.4. The local-reference gap and absolute resolvent complete the corresponding first-step precision input. This replaces the invalid shortcut from localization in U_1 to localization in V.

**Proved as a general construction:** local Gram-factor extension preserves positivity and complete integrated-variable coercivity, while retaining explicit extra currents.

**Native marked theorem now available:** [local coupling source](local_coupling_source.md), LC.6, combines these first-step inputs with its adaptive marked-source calculation and retains the exact separate M.30 endpoint records. It applies on the buffered native first-clean graph, with active endpoints and continuous directions. Its supremum is not the full ambient product supremum of M-03.

**Ambient continuous theorem now available:** [ambient gaussian marginal](ambient_gaussian_marginal.md), Theorem GM.4, uses the exact extended kernel and reconstruction and controls its individual supported value, direct and normalized-kernel records on the whole real retained product domain for this fixed geometry. The proof includes the explicit cutoff currents and uses the same complete conditional denominator.

**Still required before claiming a full first-clean augmented-state M-03 theorem:** control the replacements by another active history geometry. The continuous theorem does not regard these discrete currents as zero and does not assign them a differential estimate.

**Scalar/identity extraction on this domain:** [ambient gaussian marginal](ambient_gaussian_marginal.md), (GM.38)–(GM.40), applies the covariant finite-pulse projector to the actual transported coefficients and expresses the result in the fixed incoming F-01 basis. This is the algebraic extraction requested by M-04; a different downstream physical-renormalization coefficient prescription is a separate comparison.

**Still required for original M-04:** all allowed histories, residual-component normalization and physical support, and the complete current family including changes of active geometry.

There is also a discrete-history qualification. A bound on one fixed all-regular geometry and its continuous raw-link directions does not control the M-03 replacements of a history coordinate by a different active geometry. Those are not zero currents. The first-clean calculations above therefore cannot be labeled a full augmented-state M-03 theorem merely by freezing the history labels. They provide actual input to that theorem; the cross-sector operation must still be bounded.
