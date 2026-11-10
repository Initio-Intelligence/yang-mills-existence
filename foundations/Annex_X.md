# A separated normalization prescription and rotational compatibility equations

**Annex X.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Finite normalization and continuum hypotheses

The finite construction gives seven separated physical-scale normalization conditions and explicit rotational compatibility equations. Applying them to the limiting hierarchy requires control of the generated contact terms and a common hierarchy estimate.

The seven-channel representation classification, clover fields, Wilson scalar repair, and positive-half-space square identity are retained results from Annex D and Annex E. The new finite construction gives explicit orthogonal projectors, seven separated reflection-positive normalization functionals at a fixed physical scale, a positive free reference value for each, the resulting normalization equations and determinant, and the three rotational compatibility defects expressed in those actual finite-cutoff data.

No numerical coefficient from a Gaussian benchmark is identified with an interacting RG coefficient. The actual nondegeneracy and logarithmic bounds along the cofinal sequence are still F-05. The vanishing of the rotational defects is not proved here.

### 1. Conventions and the twenty-one representatives

Work on the even-sided Wilson torus with gauge group \(SU(N)\), normalized Haar measure and action
\[
 d\mu_{a,T}(U)=Z_{a,T}^{-1}
 \exp\left[-\beta_a\sum_p s(U_p)\right]\prod_\ell dU_\ell,
 \qquad s(U)=N-\operatorname{Re}\operatorname{Tr}U.
 \tag{F.1}
\]
The normalization dictionary is fixed:
\[
 \beta_a=2Nx_{0,a},\qquad X_{B,a}=N\beta_a=2N^2x_{0,a}.
 \tag{F.2}
\]
Coordinates are \(0,1,2,3\), with time coordinate 0. Let
\[
 \mathcal I=(01,02,03,12,13,23),\qquad
 E=\operatorname{Sym}^2(\mathbb R^{\mathcal I}),
 \qquad \langle Q,Q'\rangle_E=\operatorname{Tr}(QQ').
 \tag{F.3}
\]
Thus \(E\) has dimension 21. Its orthonormal component basis consists of the six diagonal matrices and \((E_{AB}+E_{BA})/\sqrt2\) for \(A<B\). A symmetric matrix \(Q\) therefore has off-diagonal orthonormal coordinates \(\sqrt2 Q_{AB}\), rather than \(Q_{AB}\). This convention removes an otherwise easy factor-of-two ambiguity in finite Gram systems.

For signed orthogonal unit vectors \(u,v\), write \(P_{u,v}(x)\) for the oriented elementary plaquette rooted at \(x\). Put
\[
 C_{\mu\nu,a}(x)=\frac1{8i}
 \sum_{\sigma,\tau=\pm1}\sigma\tau\,
 \pi_0\bigl(P_{\sigma e_\mu,\tau e_\nu}(x)
             -P_{\sigma e_\mu,\tau e_\nu}(x)^\dagger\bigr),
 \qquad C_{\nu\mu,a}=-C_{\mu\nu,a},
 \tag{F.4}
\]
where \(\pi_0 H=H-\operatorname{Tr}(H)I/N\). Define
\[
 q_{AB,a}(x)=a^{-4}\operatorname{Tr}(C_{A,a}(x)C_{B,a}(x)),
 \qquad t_a=\sum_Aq_{AA,a},
 \tag{F.5}
\]
and retain the exact Wilson scalar through
\[
 w_a(x)=\frac1{4a^4}\sum_{\mu<\nu}\sum_{\sigma,\tau=\pm1}
 s(P_{\sigma e_\mu,\tau e_\nu}(x)),
 \qquad
 \widetilde q_a=q_a+\frac{I_6}{6}(2w_a-t_a).
 \tag{F.6}
\]
These are the retained scalar-repaired clover representatives. In particular,
\[
 \frac12\operatorname{Tr}\widetilde q_a=w_a,
 \qquad a^4\sum_xw_a(x)=\sum_ps(U_p).
 \tag{F.7}
\]
The 21 orthonormal components of \(\widetilde q\) are the field representatives in this prescription. Every component is real, gauge invariant, and supported on links with endpoints in \(x+[-a,a]^4\). Their exact signed-permutation action is
\[
 \widetilde q_a(x;gU)=D(g)\widetilde q_a(gx;U),
 \qquad D(g)Q=(\Lambda^2g)Q(\Lambda^2g)^t.
 \tag{F.8}
\]
Fine-lattice translations have no tensor factor. The scalar repair changes no nonscalar channel.

### 2. Explicit orthogonal projectors

Extend \(Q_{ij,kl}\) antisymmetrically in each index pair and symmetrically between pairs. All formulas below are linear on \(E\). Entries not specified in a projector are zero.

#### 2.1 The diagonal sector

Let
\[
 d_{ij}=Q_{ij,ij}=d_{ji},\qquad
 s=\sum_{i<j}d_{ij},\qquad
 r_i=\sum_{j\ne i}d_{ij}-\frac{s}{2}.
 \tag{F.9}
\]
Then \(\sum_i r_i=0\). Define
\[
 (P_SQ)_{ij,ij}=\frac{s}{6},\qquad
 (P_{T_d}Q)_{ij,ij}=\frac{r_i+r_j}{2},
 \tag{F.10}
\]
\[
 (P_{W_d}Q)_{ij,ij}=d_{ij}-\frac{s}{6}-\frac{r_i+r_j}{2}.
 \tag{F.11}
\]
The images have dimensions 1, 3 and 2. The factor \(1/2\) in \(P_{T_d}\) is essential: an input \(d_{ij}=u_i+u_j\), \(\sum_i u_i=0\), has \(r_i=2u_i\).

#### 2.2 The shared-index sector

For \(i<j\), let \(k<l\) be the complementary indices and put
\[
 x=Q_{ik,jk},\qquad y=Q_{il,jl}.
\]
Use the already specified pair antisymmetries to convert these entries back to the ordered-pair matrix. Set
\[
 P_{T_o}:(x,y)\longmapsto
 \left(\frac{x+y}{2},\frac{x+y}{2}\right),
\]
\[
 P_{W_s}:(x,y)\longmapsto
 \left(\frac{x-y}{2},\frac{y-x}{2}\right).
 \tag{F.12}
\]
Their image dimensions are 6 and 6. Every shared-index matrix entry belongs to exactly one such two-coordinate block, with the stipulated orientation signs.

#### 2.3 The disjoint-index sector

Let
\[
 p_1=Q_{01,23},\qquad p_2=-Q_{02,13},\qquad
 p_3=Q_{03,12},\qquad \bar p=\frac{p_1+p_2+p_3}{3}.
 \tag{F.13}
\]
Define
\[
 P_P:(p_1,p_2,p_3)\longmapsto(\bar p,\bar p,\bar p),
\]
\[
 P_{W_p}:(p_1,p_2,p_3)\longmapsto
 (p_1-\bar p,p_2-\bar p,p_3-\bar p).
 \tag{F.14}
\]
Their dimensions are 1 and 2. \(P_P\) is the pseudoscalar projector; the minus sign in \(p_2\) is part of the convention.

These seven maps obey
\[
 P_h^2=P_h=P_h^*,\qquad P_hP_k=0\ (h\ne k),
 \qquad\sum_hP_h=I_E,
 \tag{F.15}
\]
with
\[
 h=(S,T_d,W_d,T_o,W_s,P,W_p),\quad
 d_h=(1,3,2,6,6,1,2).
 \tag{F.16}
\]
Indeed, the three diagonal spaces are mutually orthogonal: the stress coefficients have zero sum and a diagonal Weyl coefficient has zero incident sum at each vertex. The latter property also proves stress/Weyl orthogonality. The other two decompositions are orthogonal sum/difference or mean/zero-sum decompositions in equal-weight coordinates. Their sum is the identity separately on the diagonal, shared-index and disjoint-index sectors. This proves (F.15) directly. Their equivariance and their correspondence to the seven irreducible signed-hypercubic channels are the retained classification.

The unit scalar vector is
\[
 e_S=I_6/\sqrt6.
 \tag{F.17}
\]
It spans the only identity-mixing direction. The invariant expectation is
\[
 \mathbb E\widetilde q_a(x)=m_{a,T}e_S,
 \qquad m_{a,T}=\mathbb E\langle e_S,\widetilde q_a(0)\rangle_E.
 \tag{F.18}
\]
Here the origin can be replaced by any lattice vertex. The equality follows from exact translation and hypercubic symmetry of the actual Wilson measure; no limiting theorem is used.

### 3. A separated normalization measurement at the physical scale

The prescription must not normalize using an ordinary same-support variance that may be dominated by contact divergences. The following measurements are genuine separated positive-half-space pairings.

Fix \(\mu>0\), \(\varepsilon=1/64\), and the explicit radial bump
\[
 \eta(z)=c_\eta
 \begin{cases}
 \exp[-1/(1-|z|^2)],& |z|<1,\\
 0,&|z|\ge1,
 \end{cases}
 \qquad \int_{\mathbb R^4}\eta(z)\,dz=1.
 \tag{F.19}
\]
Set
\[
 f_\mu(x)=\mu^4\varepsilon^{-4}
 \eta\left(\frac{\mu x-e_0}{\varepsilon}\right).
 \tag{F.20}
\]
Its support lies in a ball of radius \(\varepsilon/\mu\) centered at \(e_0/\mu\). Write \(r_0=\operatorname{diag}(-1,1,1,1)\) and \(\theta x=r_0x\). The two supports \(\operatorname{supp}f_\mu\) and \(\theta\operatorname{supp}f_\mu\) have distance at least \(2(1-\varepsilon)/\mu\).

Use tori with \(T>8/\mu\), and \(a<(1-\varepsilon)/(2\mu)\), so the positive field stencils fit strictly inside the positive half and neither lobe approaches a torus seam. Every admissible cofinal sequence eventually meets these inequalities. This uses only its eventual geometric embedding; it does not verify the separate RG geometry statement B-02.

For any real equivariant field \(A_a\), define its centered smeared vector
\[
 B_a(A)=a^4\sum_x f_\mu(x)
 \bigl(A_a(x)-\mathbb EA_a(x)\bigr)\in E.
 \tag{F.21}
\]
For an orthonormal basis \(e_{h,1},\ldots,e_{h,d_h}\) of \(P_hE\), put
\[
 \mathcal N_{h,a,T}(A)=\frac1{d_h}
 \sum_{i=1}^{d_h}
 \mathbb E\left[
 \overline{\langle e_{h,i},B_a(A;\theta U)\rangle_E}
 \langle e_{h,i},B_a(A;U)\rangle_E\right].
 \tag{F.22}
\]
This is independent of the chosen orthonormal basis. In terms of the connected two-point distribution it is
\[
 \mathcal N_{h,a,T}(A)=\frac{a^8}{d_h}
 \sum_{x,y}f_\mu(x)f_\mu(y)
 \mathbb E\left[
 \left\langle D(r_0)P_hA_a^c(\theta x),
 P_hA_a^c(y)\right\rangle_E\right].
 \tag{F.23}
\]
It is a finite normalization functional on the two-point distribution, with the fixed tensor contraction shown. Its two external source arguments stay a fixed physical distance apart. Point-local contact changes do not alter it.

#### Proposition F.1 — the actual normalization data are nonnegative

For the compact Wilson law and the stated cutoff margins,
\[
 0\le n_{h,a,T}:=\mathcal N_{h,a,T}(\widetilde q)<\infty.
 \tag{F.24}
\]
**Proof.** Each summand of (F.22) is the original Wilson site-reflection Gram form of a bounded positive-half-link function. The compactness of the finite link space gives finiteness. The exact site-reflection square formula proves nonnegativity. Summation and division by \(d_h\) preserve it. This uses the actual compact measure, not an auxiliary RG law. ∎

Strict positivity is not asserted merely from compactness or from reflection positivity. For example, at \(\beta=0\), a centered field supported strictly away from the boundary has zero conditional mean on the reflecting-plane links, so its site-reflection norm vanishes. The asymptotically free sequence has positive large \(\beta\), but excluding small or zero values of (F.24) on that sequence is still a real nondegeneracy task.

### 4. Explicit positive reference values

Fix generators \(T^a\) with \(\operatorname{Tr}(T^aT^b)=\delta^{ab}/2\). As a normalization benchmark only, take independent unit-coupling free Euclidean potentials with covariance \(\delta^{ab}\delta_{\mu\nu}/(4\pi^2|x-y|^2)\). Their curvature covariance at distinct points is
\[
 \mathbb E F_A^a(x)F_B^b(y)
 =\frac{\delta^{ab}}{\pi^2|x-y|^4}
 (\Lambda^2R_{x-y})_{AB},
 \qquad
 R_r=I_4-2\widehat r\widehat r^t.
 \tag{F.25}
\]
This follows by differentiating the displayed potential covariance. The quartic term in the wedge of \(I-2\widehat r\widehat r^t\) cancels, giving the familiar curl-curl expression directly.

Let \(Q^*_{AB}=:\!\operatorname{Tr}(F_AF_B)\!:\) in the benchmark. Wick contraction gives, for \(u,v\in E\),
\[
 \mathbb E\langle u,Q^*(x)\rangle_E
 \langle v,Q^*(y)\rangle_E
 =c_N|x-y|^{-8}\langle u,D(R_{x-y})v\rangle_E,
 \quad c_N=\frac{N^2-1}{2\pi^4}.
 \tag{F.26}
\]
Only distinct-point pairings are used, so no extension of this benchmark through coincidence sets is needed here.

Define the seven fixed reference numbers by the finite integrals
\[
 \lambda_h(\mu)=\frac{c_N}{d_h}
 \int f_\mu(x)f_\mu(y)|\theta x-y|^{-8}
 \operatorname{Tr}_E\left[
 P_hD(r_0)P_hD(R_{\theta x-y})P_h\right]dx\,dy.
 \tag{F.27}
\]
These are explicit real numbers determined by (F.10)–(F.20) and the fixed trace convention. In particular \(\lambda_h(\mu)=\mu^8\lambda_h(1)\). They are fully specified finite reference integrals, rather than unspecified matching coefficients; no numerical quadrature is required by this prescription.

#### Proposition F.2 — every reference value is strictly positive

For every channel,
\[
 \frac{c_N(1-8\varepsilon/(1-\varepsilon))}
 {[2(1+\varepsilon)]^8}\,\mu^8
 \le\lambda_h(\mu)
 \le\frac{c_N}{[2(1-\varepsilon)]^8}\,\mu^8.
 \tag{F.28}
\]
**Proof.** On the two supports,
\[
 2(1-\varepsilon)/\mu\le|\theta x-y|
 \le2(1+\varepsilon)/\mu.
\]
The sine of the angle of \(\theta x-y\) to the time axis is at most \(\varepsilon/(1-\varepsilon)\). Hence
\[
 \|R_{\theta x-y}-r_0\|\le 2\varepsilon/(1-\varepsilon).
\]
The tensor action \(D\) is a restriction of the fourth tensor power, so telescoping the four tensor factors gives
\[
 \|D(R_{\theta x-y})-D(r_0)\|
 \le8\varepsilon/(1-\varepsilon).
\]
The projector \(P_h\) commutes with \(D(r_0)\), and the latter is an orthogonal involution. At \(R=r_0\), the trace in (F.27) equals \(d_h\); its difference from \(d_h\) is at most \(d_h\) times the last norm bound. Its absolute value is at most \(d_h\), because it is the trace of a product of contractions on \(P_hE\). Integrating against the two probability densities proves (F.28). With \(\varepsilon=1/64\), the lower prefactor is positive. ∎

The free value fixes a convention for the finite normalization. It does not prove that the interacting data \(n_{h,a,T}\) have this asymptotic, nor that the induced fields have the desired interacting short-distance coefficients. Those are F-05 and U-01–U-03.

### 5. The finite system, identity coefficient and determinant

The proposed physical-scale conditions are
\[
 \mathbb E\Phi_a(x)=0,
 \qquad \mathcal N_{h,a,T}(\Phi)=\lambda_h(\mu)
 \quad(h=S,T_d,W_d,T_o,W_s,P,W_p),
 \tag{F.29}
\]
with positive channel orientation. Write
\[
 Z_{a,T,\mu}=\sum_hz_{h,a,T,\mu}P_h,
 \qquad
 \Phi_a=Z_{a,T,\mu}\widetilde q_a-c_{a,T,\mu}e_S.
 \tag{F.30}
\]
Because \(P_hZ=z_hP_h\) and the connected normalization functional removes constants,
\[
 \mathcal N_{h,a,T}(\Phi)=z_h^2n_{h,a,T},
 \qquad c=z_Sm_{a,T}.
 \tag{F.31}
\]
Consequently, on the explicitly checkable domain
\[
 \boxed{n_{h,a,T}>0\quad\text{for all seven channels},}
 \tag{F.32}
\]
the unique solution with \(z_h>0\) is
\[
 \boxed{
 z_{h,a,T,\mu}=\sqrt{\lambda_h(\mu)/n_{h,a,T}},
 \qquad c_{a,T,\mu}=z_{S,a,T,\mu}m_{a,T}.}
 \tag{F.33}
\]
The seven measurements therefore separate the seven channel coefficients, and the mean separates the identity coefficient. The determinant of the eight-variable normalization Jacobian, ordering the seven two-point equations before the scalar mean equation, is
\[
 \boxed{-2^7\prod_h z_h n_{h,a,T}\ne0.}
 \tag{F.34}
\]
Changing the order of equations changes only its sign. This is the promised explicit finite nondegeneracy test.

This completes **F-01 as stated**: it asks for a concrete prescription and checkable nondegeneracy, leaving actual invertibility and its cutoff control to F-05. The explicit tests require only eventual embedding along B-02, not a new geometric hypothesis.

#### A total finite-cutoff definition, without hiding nondegeneracy

If a coefficient must be defined at every cutoff obeying the geometric margins of Section 3 before (F.32) is established, one may use the following explicitly marked totalization:
\[
 z_h^{\mathrm{tot}}=
 \begin{cases}
 \sqrt{\lambda_h/n_h},&n_h>0,\\
 1,&n_h=0,
 \end{cases}
 \qquad c^{\mathrm{tot}}=z_S^{\mathrm{tot}}m.
 \tag{F.35}
\]
Every coefficient in (F.35) is a finite real number determined by the actual compact law, so this defines an actual cutoff field rather than an arbitrary-coefficient placeholder. If \(n_h=0\), it deliberately does **not** claim to satisfy that channel's nonzero condition in (F.29). F-05 must show that the totalization agrees with (F.33) on the required tail of the cofinal sequence and has the prescribed logarithmic budgets. The fallback is bookkeeping for the cutoff construction, not a solution of a singular normalization system.

The coefficients in either prescription are constant in spacetime. Translating the normalization lobe and its reflecting plane together by a fine-lattice translation leaves the data unchanged by the change of link variables. Applying a signed permutation to the lobe, reflection and channel basis together likewise leaves the data unchanged. Thus using a particular time axis and origin in (F.20) does not insert an uncontrolled spatially varying coefficient.

### 6. Wick and reflection conventions for this prescription

In the real Euclidean component basis, a component with \(n_0\) occurrences of the time index obeys the reflection sign \((-1)^{n_0}\), where \(n_0\in\{0,1,2\}\). All projectors commute with the time reflection, and all coefficients in (F.33) or (F.35) are real. Therefore the normalized fields satisfy exactly
\[
 \overline{\Phi_a(x;\theta U)}=D(r_0)\Phi_a(\theta x;U).
 \tag{F.36}
\]
For the Hermitian Wick component convention set
\[
 W_{\alpha\alpha}=i^{n_0(\alpha)},\qquad
 \widehat\Phi_a=W\Phi_a.
 \tag{F.37}
\]
Then \(\overline W D(r_0)=W\), so the antilinear reflection on \(\widehat\Phi\) has no remaining component sign. Other tensor transformations are \(\widehat D(g)=WD(g)W^{-1}\). The identity vector also changes to \(We_S\); it must not be silently kept as the real Euclidean scalar vector after the Wick basis change.

Use either this Wick convention everywhere or the real Euclidean convention with \(D(r_0)\) everywhere. They are equivalent descriptions of the same cutoff Gram forms.

### 7. R-01: the three conditions in the actual normalization data

The retained classification groups the seven projectors into four rotational types:
\[
 P_S,\quad P_P,\quad P_T=P_{T_d}+P_{T_o},\quad
 P_W=P_{W_d}+P_{W_s}+P_{W_p}.
 \tag{R.1}
\]
For the explicitly constructed normalization map (F.30), its commutation with the canonical \(O(4)\) tensor action is equivalent to the three scalar relations
\[
 z_{T_d}=z_{T_o},\qquad
 z_{W_d}=z_{W_s},\qquad z_{W_p}=z_{W_s}.
 \tag{R.2}
\]
The representation classification proving this equivalence is reused. The new concrete normalization conditions are obtained by substituting (F.33):
\[
 \boxed{
 \frac{n_{T_d,a,T}}{\lambda_{T_d}(\mu)}
 =\frac{n_{T_o,a,T}}{\lambda_{T_o}(\mu)},
 }
 \tag{R.3}
\]
\[
 \boxed{
 \frac{n_{W_d,a,T}}{\lambda_{W_d}(\mu)}
 =\frac{n_{W_s,a,T}}{\lambda_{W_s}(\mu)},\qquad
 \frac{n_{W_p,a,T}}{\lambda_{W_p}(\mu)}
 =\frac{n_{W_s,a,T}}{\lambda_{W_s}(\mu)}.
 }
 \tag{R.4}
\]
All quantities are now specified compact Wilson integrals or the fixed positive integrals (F.27). The equivalent logarithmic defects are
\[
 d_T=\frac12\log\frac{n_{T_o}/\lambda_{T_o}}
                              {n_{T_d}/\lambda_{T_d}},
\]
\[
 d_{W_d}=\frac12\log\frac{n_{W_s}/\lambda_{W_s}}
                                 {n_{W_d}/\lambda_{W_d}},\qquad
 d_{W_p}=\frac12\log\frac{n_{W_s}/\lambda_{W_s}}
                                 {n_{W_p}/\lambda_{W_p}}.
 \tag{R.5}
\]
They are \(\log(z_{T_d}/z_{T_o})\), \(\log(z_{W_d}/z_{W_s})\), and \(\log(z_{W_p}/z_{W_s})\), respectively.

There is also an explicit finite metric for this defect. The Hilbert–Schmidt orthogonal projection of \(Z\) onto the four-channel rotational commutant is
\[
 \overline Z=z_SP_S+z_PP_P+\bar z_TP_T+\bar z_WP_W,
\]
\[
 \bar z_T=\frac{3z_{T_d}+6z_{T_o}}9,
 \qquad
 \bar z_W=\frac{2z_{W_d}+6z_{W_s}+2z_{W_p}}{10}.
 \tag{R.6}
\]
The exact squared distance is
\[
 \boxed{\begin{aligned}
 \|Z-\overline Z\|_{\mathrm{HS}}^2
 ={}&2(z_{T_d}-z_{T_o})^2
 +\frac65(z_{W_d}-z_{W_s})^2\\
 &+\frac25(z_{W_d}-z_{W_p})^2
 +\frac65(z_{W_s}-z_{W_p})^2.
 \end{aligned}}
 \tag{R.7}
\]
This follows from the weighted-variance identity
\(\sum_i d_i(z_i-\bar z)^2=(\sum_i d_i)^{-1}\sum_{i<j}d_id_j(z_i-z_j)^2\).

If an actual one-step matrix is later proved to be
\[
 M_j=I+u_j\sum_h\gamma_hP_h+\mathcal E_j,
\]
its first-order rotational compatibility relations are correspondingly
\[
 \gamma_{T_d}=\gamma_{T_o},\quad
 \gamma_{W_d}=\gamma_{W_s},\quad
 \gamma_{W_p}=\gamma_{W_s}.
 \tag{R.8}
\]
This writes the conditions without assigning values to the uncomputed actual coefficients in F-03.

Equations (R.3)–(R.7) complete the finite construction required by **R-01** for the prescription in this note. They do not assert that the data satisfy them. Nor is exact rotational commutation of a finite-cutoff bare-to-normalized map a necessary substitute for covariance of the limiting hierarchy: anisotropic cutoff representatives can require compensating finite coefficients. R-02 through R-05 still concern the actual hierarchy's action, observable and contact defects. No rotation-restoration estimate is inferred from this finite construction.

### 8. The actual cutoff positivity and translation verification obtained here

The totalization (F.35), with the scalar identity coefficient shown there, is an actual finite-cutoff function of the Wilson measure. Define its ordinary full moment hierarchy by
\[
 S^{\mathrm{tot}}_{m,a,T}(F)=a^{4m}\sum_{X,\boldsymbol\alpha}
 F_{\boldsymbol\alpha}(X)
 \mathbb E\prod_{i=1}^m\Phi^{\mathrm{tot}}_{\alpha_i,a}(x_i).
 \tag{P.1}
\]
These finite sums are always defined. The same statements hold for the exactly normalized prescription on (F.32).

#### Proposition P.1 — concrete cutoff instance

The hierarchy (P.1) has permutation symmetry, exact fine-lattice translation symmetry, hypercubic tensor covariance, and reflection positivity on every fixed positive-time test algebra once its stencil margin fits. The Wick convention is exactly (F.37).

**Proof.** The coefficients are real and independent of position; their mixing matrix is the displayed sum of the equivariant projectors; their identity direction is \(e_S\). Thus (F.8) and (F.36) hold with these actual coefficients. For a finite positive-time polynomial test vector, the corresponding polynomial in \(\Phi^{\mathrm{tot}}\) is a bounded positive-half-link function at each cutoff. The Wilson square formula gives its nonnegative Gram form. Commutativity gives permutation symmetry, and changing all link variables by a fine-lattice translation proves exact translation covariance of the finite sums. No bound on \(Z\) is needed for these finite-cutoff statements. ∎

The proposition also verifies any explicitly chosen point-local real equivariant source substitution that has been constructed for this hierarchy and splits across separated half-spaces. In particular the concrete choice \(R[j]=j\), \(C[j]=0\) defines a compatible all-order external source jet and needs no contact coefficients. This observation must be used with its exact scope: it does not identify all contact terms generated by the marked RG induction with that zero-contact representative, or bound their finite-stencil and normalization remainders.

Exact positive transports may be used to evaluate (P.1). If the **whole product** is transported, its integral is unchanged, and an auxiliary skeleton cannot break the original fine-translation identity. If the product of the separately transported marks is used instead, the matching discrepancy must be retained. Its vanishing requires the actual matching and coefficient budgets; the unnormalized mesoscopic theorem alone does not establish them for (F.35).

### 9. Why P-01 and P-02 remain open under their stated mathematical requirements

#### P-01: the missing actual contact realization

The finite one-field coefficients in this note are actual real coefficients, so no arbitrary-coefficient placeholder is needed for this cutoff prescription. Nevertheless P-01 asks for the constructed field/source substitutions of the target hierarchy, including its required contacts, and explicitly depends on F-05, F-06 and S-06.

The following have not been proved here:

1. That (F.32) holds on a cofinal tail and that (F.33) is the normalization produced and controlled by the actual marked induction.
2. That every local extraction generated by that induction has the required point-jet or shrinking-stencil realization, compatible in source degree and with the stipulated spatial-order bounds.
3. That the complete contact/normalization approximation error vanishes in the common joint-test norm for the same hierarchy.

Proposition P.1 therefore completes a useful concrete cutoff verification, **not the P-01 statement**. Calling the external contact coefficients zero does not prove the missing equality between that chosen representative and the exact transported marked hierarchy.

#### P-02: the missing common continuity and matching budget

Exact fine-lattice translation symmetry and permutation symmetry are proved for (P.1). For a continuum shift \(b\), however, the passage using fine shifts \(b_a\to b\) still needs a uniform estimate of the form
\[
 |S_{m,a,T}(\tau_bF-\tau_{b_a}F)|
 \le C^{m+1}(m!)^p\nu_{qm}(\tau_bF-\tau_{b_a}F),
 \tag{P.2}
\]
for the actual normalized hierarchy, with the common parameters supplied by S-05/S-06. No such estimate is proved by cutoff symmetry. If an approximate skeleton representation is used, its corresponding translation defect also requires the matching budget just described.

Passing from (P.2) to continuum translation covariance requires the stated common seminorm estimate.
