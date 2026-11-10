# The first background curvature has a depth-uniform Gaussian root bound

This note settles the linear Gaussian version of the background term TM.23 without multiplying one-step prolongation estimates. It also states a finite-dimensional perturbative criterion sufficient to transfer the bound. The criterion for the **complete actual restored later law** is not claimed proved here. A bound on the oscillation of that law by D_late alone is insufficient for this marked conclusion.

## 1. Energy projection, with all gauge and terminal constraints retained

Work at a fixed finite lattice cutoff. Remove the null physical gauge directions, or take the corresponding quotient; compact gauge samplers are retained separately. On the resulting real physical space let

\[
 d\gamma(A)=Z^{-1}e^{-\frac12 A^{\mathsf T}KA}\,dA,
 \qquad K>0.
 \tag{GB.1}
\]

No volume-uniform lower spectral gap of the full massless K is needed below. The local curvature readout R_x is normalized in the same quadratic Wilson action, so

\[
 R_x^{\mathsf T}R_x\le c_x K,
 \qquad c_x\le C,
 \tag{GB.2}
\]

where R_x has fixed output rank, including the fixed microscopic scalar stencil and Lie-algebra multiplicity. This follows by retaining that stencil's positive terms in the full Wilson quadratic. Additional soft-gauge terms can only increase K. Pure null modes annihilated by the curvature can equivalently be handled with Moore–Penrose inverses.

For the literal source interpretation one may take K to be the Wilson quadratic on the physical quotient and keep the normalized soft-gauge samplers as independent additional variables. Their endpoint-covariant reparameterization is MT.13–MT.19. In that convention the physical conditional mean below is exactly the Wilson constrained minimum. One must not silently change that minimum by adding an arbitrary physical gauge penalty and then call its new conditional mean the old background.

Let Q be the actual linearized first coarse readout. The K-orthogonal minimum with the same first readout is P A, with

\[
 P=K^{-1}Q^{\mathsf T}(QK^{-1}Q^{\mathsf T})^{+}Q.
 \tag{GB.3}
\]

The plus sign means the inverse on the actual readout range. Thus P²=P, P is self-adjoint in the K inner product, and

\[
 PK^{-1}P^{\mathsf T}\le K^{-1}.
 \tag{GB.4}
\]

The final retained current constraint has the form T A=v with T=T'Q, because the literal chronological readout factors through the first average; see FR.1. The conditional Gaussian has mean m and covariance

\[
 m=K^{-1}T^{\mathsf T}(TK^{-1}T^{\mathsf T})^{+}v,
 \qquad
 C_T=K^{-1}-K^{-1}T^{\mathsf T}(TK^{-1}T^{\mathsf T})^{+}TK^{-1}.
 \tag{GB.5}
\]

Its mean lies in the range of P, so Pm=m. Conditional on T A=v, the first innovation (I−P)A and the later physical variable Y=P(A−m) remain independent: they are independent in the original Gaussian and the terminal constraint only reads the second variable.

By (GB.4) and C_T≤K^{-1},

\[
 \operatorname{Cov}(Y)=PC_TP^{\mathsf T}\le K^{-1},
 \qquad
 R_x\operatorname{Cov}(Y)R_x^{\mathsf T}\le CI.
 \tag{GB.6}
\]

The second inequality follows from (GB.2): the nonzero singular values of R_xK^{-1/2} are bounded by sqrt(C). It is independent of the number of subsequent averaging steps, the smallest mesh, and the total volume.

In particular the first background curvature is

\[
 R_x P A=R_xm+R_xY,
 \tag{GB.7}
\]

and its Gaussian local energy is bounded by C[1+||R_xm||²]. This is a statement about the **first background**, even though the terminal condition may be many scales later. It does not identify that background with the final field.

## 2. Any centered convex quiet mask preserves the root bound

Include all independent normalized Gaussian gauge samplers in the later vector if necessary. Let G be a centrally symmetric convex event in the joint later Gaussian variables. It may encode many good tests, on several native scales, and may have arbitrarily small positive probability. The convex-mask estimate CR.12 gives

\[
 \gamma(e^{t\ell Y}\mid G)
 \le \exp[\tfrac12t^2\ell\operatorname{Cov}(Y)\ell^{\mathsf T}]
 \tag{GB.8}
\]

for every scalar linear functional, with the covariance of the complete Gaussian vector when gauge coordinates are involved. Applying this to the fixed output coordinates of R_xY yields

\[
 \gamma(\|R_xm+R_xY\|^2\mid G)
 \le C[1+\|R_xm\|^2].
 \tag{GB.9}
\]

The probability of G is not divided into an absolute estimate. The same argument gives fixed-order or exponential local curvature moments with their usual fixed-rank Gaussian constants.

Suppose an affine good event H obeys centered sandwiches G^-⊂H⊂G^+, with the thresholds of G^- and G^+ differing by at most a fixed fraction. If the centered Gaussian tails give

\[
 \gamma(G^-\mid G^+)\ge1-\eta,
 \tag{GB.10}
\]

then positivity and (GB.9) give

\[
 \gamma(\|R_xm+R_xY\|^2\mid H)
 \le {C[1+\|R_xm\|^2]\over1-\eta}.
 \tag{GB.11}
\]

Thus small nonzero reference offsets can be retained by the same genuine tail estimate used for CE. They need not be declared zero. At a flat final retained field, m=0 in the Gaussian model, but Y still fluctuates and its first-background energy is O(1), not zero.

## 3. A positive later Schur tilt causes no new depth loss

Let E_L(Y)=Y^{\mathsf T}S_LY/2 be a finite-rank nonnegative later energy with

\[
 0\le S_L\le C K_Y,
 \qquad \operatorname{rank}S_L\le D,
 \tag{GB.12}
\]

on the allowed later physical quotient, where K_Y is the inverse of its covariance. For the exact Gaussian Schur decomposition, any retained sum of its positive innovation and Schur forms has this property with a fixed C. It is not justified by summing unrelated diagonal blocks with discarded cross terms.

For t below a fixed t_0, the tilted precision K_Y−tS_L is at least K_Y/2. Its curvature covariance remains bounded by twice the right side of (GB.6). The Gaussian convex-mask argument therefore still bounds the root under this tilted law. Moreover, writing E_L=||LY||²/2 with LCov(Y)L^T≤CI and applying the quadratic form of CR.12 gives

\[
 \gamma(e^{tE_L}\mid G)\le (1-Ct)^{-D/2}
 \le e^{CtD}.
 \tag{GB.13}
\]

Combining the exact tilted conditional identity with (GB.9),

\[
 \gamma(\|R_xm+R_xY\|^2e^{tE_L}\mid G)
 \le C[1+\|R_xm\|^2]e^{CtD}.
 \tag{GB.14}
\]

For t≤c/K with K≥D, this is bounded uniformly. Affine-mask sandwiches remain valid if their variance/tail bounds are checked for the tilted covariance, which differs by at most the fixed factor two. This closes the background term in the Gaussian counterpart of TM.23 and gives its n!K^n mixed moments. Together with TM's Gaussian first-innovation argument and unweighted mass dilution, the Gaussian first-birth family has the desired one-root mixed budget without an extra K factor.

If the current reference has native fine curvature bounded by CP L^{-2N}, as the source variational regularity gives deep inside the first-reset core, then ||R_xm||²≤CP²L^{-4N} and the deterministic term is also bounded. At a general root keep the actual deterministic reference curvature instead. This scaling estimate does not make the random first background equal to the final reference.

## 4. A precise perturbative transfer criterion

The following criterion shows what additional estimate would close the same marked background root in the actual finite restored chart. Let γ be the Gaussian law on that chart, with a centered convex enclosing product domain C and possibly a centered convex quiet mask G. Suppose the actual complete density on the same support is

\[
 d\mu_\theta=Z_\theta^{-1}e^{\theta W}\,d\gamma,
 \qquad 0\le\theta\le1,
\]

and, in the physical Gaussian energy metric,

\[
 \|K^{-1/2}(\nabla^2W)K^{-1/2}\|\le\epsilon<1/2,
 \qquad
 \sup\|K^{-1/2}\nabla W\|\le\rho.
 \tag{GB.15}
\]

On the convex support the Brascamp–Lieb covariance bound is at most 2K^{-1}. For a linear curvature component ℓY, differentiation in theta gives

\[
 |\partial_\theta\mu_\theta(\ell Y)|
   =|\operatorname{Cov}_{\mu_\theta}(\ell Y,W)|
   \le C\|\ell K^{-1/2}\|\rho.
 \tag{GB.16}
\]

The inequality uses the Brascamp–Lieb variance estimates for each factor and Cauchy–Schwarz; the **entire finite rank** is already included in rho. Since the reference mean is zero on centered C∩G, the actual curvature mean is O(rho), its variance is O(1), and

\[
 \mu_1(\|R_xm+R_xY\|^2)
 \le C[1+\|R_xm\|^2+\rho^2].
 \tag{GB.17}
\]

This criterion tolerates rho=O(1). A finite local vertex expansion with complete derivative rows O(g times fixed powers of R and P), and a polynomially conditioned common chart, would give rho=o(1) because the restored rank is only a fixed logarithmic power. The same estimates after the small later Schur tilt give the mixed version of (GB.17). Nonlinear selector sandwiches and nonlinear scalar readout errors must also be kept; WA supplies a primitive averaging Taylor bound but not this complete density hypothesis.

By contrast, an estimate osc W≤D_late does **not** imply (GB.15) or an O(1) curvature root. A weight e^{lambda z_1} on a unit Gaussian has oscillation O(lambda P) on a P-box and shifts its local mean by order lambda. A diverging coarse ledger therefore cannot be converted into a bounded marked local expectation without a derivative or local relative comparison argument.

## 5. Source scope

The all-depth projection identities above are exact for the linearized Wilson Gaussian with its actual physical quotient and chronological constraints. They do not use a false inverse implication from contraction of the forward averaging map. The source nonlinear first background is a conditional minimum, not exactly a Gaussian conditional mean. For the actual M04 application, either the complete later law must satisfy a criterion such as (GB.15), or an equivalent local marked marginal bound must be proved. The positive energy reserve ER is sufficient for rare quiet-mask failures; it is not by itself sufficient for the O(1) microscopic background root in TM.23.
