# Reflected susceptibilities and physical normalization

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

**Gaussian calibration hypothesis (GC).** For the signed Gaussian increments of the actual stationary source section in its thermodynamic normalization, assume $\sum_{k<n}d_k^G=d_Bn+\vartheta_n$ with $d_B>0$ and $\sup_n|\vartheta_n|\le B_G$. The coupling and stopping conclusions use this calibration and the specified source readout and replay. A physical continuum limit also requires the stated uniform normalization and full-law hierarchy estimates.

**Finite-cutoff scope.** Nonzero reflected measurements at each cutoff allow finite normalization. Uniform bounds for the seven normalizing factors along one physical sequence and passage of the full normalized hierarchy have separate hypotheses.

## Result and exact status

The actual scalar identity coefficient in the stated F01 prescription is
controlled by the actual channel multiplier. It is not an additional
uncontrolled parameter. On the stopped Wilson sequence of PE,
\[
 c_N\le \beta_a a^4 m_{a,T}\le C_N,
 \qquad
 c_N\,\frac{z_S}{\beta_a}
 \le a^4c_{a,T,\mu}
 \le C_N\,\frac{z_S}{\beta_a}.
 \tag{PN.1}
\]
The upper constant may depend on the fixed trajectory and geometric
constants; neither constant depends on the ultraviolet depth or total
volume. Here \(m\) is the exact scalar mean and \(c=z_Sm\) is precisely
the identity coefficient of Annex X, rather than a new subtraction.

Consequently the coefficient budget used in CS and ER satisfies
\[
 B_a:=\frac{\|Z_{a,T,\mu}\|_{\rm op}}{\beta_a}
 \le b_a:=B_a+a^4|c_{a,T,\mu}|
 \le C B_a.
 \tag{PN.2}
\]
The proof below uses the original compact Wilson law, an exact
Schwinger--Dyson identity, and the checked Wilson partition-ratio bound.
No Gaussian replacement, source-conditioned density, or assumed
susceptibility estimate is used.

This closes the identity-coefficient part of the normalization budget
once the channel multipliers are controlled. It does **not** prove the
missing logarithmic bounds for those multipliers, the actual F03/F04
mixing estimates, or the prescribed B05 endpoint. F05 as a whole remains
open. Sections 6--8 identify its remaining numerical data precisely and
prove how the prescribed finite normalization supplies nondegeneracy
whenever a common hierarchy limit has been obtained.

The subsequent finite reflected witnesses proves
the separate qualitative finite-cutoff positivity needed to use
this prescription. Its Corollary FN.5 supplies all seven \(n_h>0\)
on one actual PE sequence with the original slow-volume geometry.
It therefore removes exact zero-channel and determinant
singularities on that sequence; the logarithmic upper and lower
bounds remain open.

Statements labeled P are proved here. Statements labeled C are proved
implications with an explicitly stated remaining actual-model input.
The final table records the unproved inputs.

## 1. Frozen physical prescription

Use the original four-dimensional periodic Wilson measure on an
even cubic \(n^4\) lattice, \(n\ge2\), with fine physical spacing \(a\):
\[
 d\mu_{\beta,n}(U)=Z_n(\beta)^{-1}
 e^{-\beta S(U)}\,dU,\qquad
 S=\sum_p s_p,\qquad
 s_p=N-\operatorname{ReTr}U_p,\qquad G=SU(N).
 \tag{PN.3}
\]
There are \(V=n^4\) vertices and \(6V\) plaquettes. Haar measure is
normalized. The coefficient \(\beta\) is the **bare Wilson coefficient**,
not the terminal effective inverse coupling. In the
source units, PE uses \(\beta_{W,n}=Y_{0,n}/N\), consistently with
Annex X's \(\beta=2Nx_0\) and \(Y_0=2N^2x_0\).

The tensor space is
\[
 E=\operatorname{Sym}^2(\Lambda^2\mathbb R^4),\qquad \dim E=21,
 \qquad e_S=I_6/\sqrt6.
 \tag{PN.4}
\]
Retain exactly the clover and Wilson-scalar repair of Annex X
(F.4)--(F.7). Only the following exact identities are needed here:
\[
 \frac12\operatorname{Tr}\widetilde q_a(x)=w_a(x),\qquad
 w_a(x)=\frac1{4a^4}
 \sum_{\mu<\nu}\sum_{\sigma,\tau=\pm1}
             s(P_{\sigma e_\mu,\tau e_\nu}(x)),
 \tag{PN.5}
\]
\[
 \mathbb E\widetilde q_a(x)=m_{a,T}e_S,\qquad
 m_{a,T}=\frac{2}{\sqrt6}\mathbb E w_a(0).
 \tag{PN.6}
\]
Translation and hypercubic invariance make all the plaquette means in
(PN.5) identical. There are 24 summands, so
\[
 \mathbb E w_a(0)=6a^{-4}\mathbb E s_p,\qquad
 \boxed{\ \beta a^4m_{a,T}=2\sqrt6\,\beta\mathbb E s_p.\ }
 \tag{PN.7}
\]

Let \(P_h\), \(h=(S,T_d,W_d,T_o,W_s,P,W_p)\), be the seven fixed
orthogonal hypercubic projectors, with dimensions
\[
 (d_h)=(1,3,2,6,6,1,2).
 \tag{PN.8}
\]
The fixed separated reflected measurements and their positive
reference values are those of Annex X (F.19)--(F.28):
\[
 n_{h,a,T}=\mathcal N_{h,a,T}(\widetilde q_a)\ge0,
 \qquad \lambda_h(\mu)>0.
 \tag{PN.9}
\]
At a cutoff where all seven \(n_h\) are positive, the actual prescribed
solution is
\[
 Z=\sum_hz_hP_h,\qquad
 z_h=\sqrt{\lambda_h/n_h}>0,\qquad
 c=z_Sm,\qquad
 \Phi_a=Z\widetilde q_a-ce_S.
 \tag{PN.10}
\]
Its mean is exactly zero and its seven reflected measurements are
exactly \(\lambda_h\). No change of this prescription is made below.

The stated F05 normalization condition asks for actual mixing products, the inverse
matrices, the finite normalization determinant and logarithmic
coefficient budgets. Its predecessor F01 is a finite construction;
nonnegativity of \(n_h\) alone is not quantitative invertibility.

## 2. An exact lower Wilson-energy bound

### Theorem PN.1 (P): uniform lower energy from one-link integration

Equip \(\mathfrak{su}(N)\) with the metric
\(\langle X,Y\rangle=-\operatorname{Tr}(XY)\), and put
\[
 d=N^2-1,\qquad c_F=d/N.
 \tag{PN.11}
\]
For every \(\beta>0\), every finite cubic torus as above, and every
plaquette \(p\),
\[
 \boxed{\quad
 \beta\,\mathbb E_{\beta,n}s_p
 \ge \frac{c_FN\,\beta}{12\beta+c_F}.
 \quad}
 \tag{PN.12}
\]
In particular, for \(\beta\ge1\), the right side is at least
\(c_FN/(12+c_F)>0\), uniformly in volume.

**Proof.** Let \(X_1,\ldots,X_d\) be an orthonormal basis of the
Lie algebra, and let \(\Delta=\sum_\alpha D_{X_\alpha}^2\) be the
nonpositive group Laplacian. Adjoint invariance makes
\(\sum_\alpha X_\alpha^2\) a scalar matrix. Taking its trace gives
\[
 \sum_\alpha X_\alpha^2=-c_F I.
 \tag{PN.13}
\]
For \(s(U)=N-\operatorname{ReTr}U\),
\[
 \Delta s=c_F(N-s).
 \tag{PN.14}
\]
Also \(\operatorname{ReTr}X_\alpha=0\). Bessel's inequality in the
real Hilbert--Schmidt space, together with
\(\|U-I\|_{HS}^2=2s(U)\), gives
\[
 |\nabla s(U)|^2
 =\sum_\alpha\bigl(\operatorname{ReTr}
                         [X_\alpha(U-I)]\bigr)^2
 \le 2s(U).
 \tag{PN.15}
\]
Left and right translations and inversion preserve these statements
for a plaquette viewed as a function of any one of its links.

Fix a positive link \(b\) and all the other raw Wilson links. Exactly
six plaquettes contain \(b\). Their sum
\[
 A_b(U_b)=\sum_{p\ni b}s_p(U_b)
 \tag{PN.16}
\]
is the entire \(U_b\)-dependent action. Its true conditional law is
proportional to \(e^{-\beta A_b(U_b)}\,dU_b\). Equations
(PN.14)--(PN.15) give, pointwise,
\[
 \Delta_bA_b=c_F(6N-A_b),\qquad
 |\nabla_bA_b|^2
 \le6\sum_{p\ni b}|\nabla_bs_p|^2\le12A_b.
 \tag{PN.17}
\]
There is no boundary term on the compact group. Integration by parts
under this **normalized conditional law** yields
\[
 c_F\bigl(6N-\mathbb E[A_b\mid U_{b^c}]\bigr)
 =\beta\,\mathbb E[|\nabla_bA_b|^2\mid U_{b^c}]
 \le12\beta\,\mathbb E[A_b\mid U_{b^c}].
 \tag{PN.18}
\]
Thus
\[
 \mathbb E[A_b\mid U_{b^c}]
 \ge\frac{6c_FN}{12\beta+c_F}.
 \tag{PN.19}
\]
Average the actual exterior marginal. Translation and hypercubic
symmetry give \(\mathbb EA_b=6\mathbb Es_p\), proving (PN.12).
\(\square\)

The conditional assertion (PN.19) is valid for the literal one-link
Wilson conditional law. An additional selector depending on \(U_b\)
would change that law and is not included. No such selector is present
when deriving the full-law mean used in (PN.7).

## 3. The matching upper energy bound on the actual sequence

### Theorem PN.2 (P): first-moment upper bound with its finite-volume term

For each fixed \(0<s<1\), the checked partition-ratio estimate gives
\[
 \beta\mathbb E_{\beta,n}s_p
 \le C_{N,s}
       +\frac{d}{3sV}\log(1+\beta).
 \tag{PN.20}
\]
In particular this is uniformly bounded on the actual stopped
sequence of PE.

**Proof.** The exact compact bounds CA.3, CA.6 and CA.9a in
the Wilson energy normalization give
\[
 c_N(1+\beta)^{-d/2}\le z(\beta)
       \le C_N(1+\beta)^{-d/2},
 \tag{PN.21}
\]
\[
 Z_n(\beta)\ge e^{-C_NV}
       (1+\beta)^{-d(3V+1)/2},\qquad
 Z_n(\beta)\le z(\beta)^{3V-3}.
 \tag{PN.22}
\]
The lower bound comes from an exact spanning-tree gauge and a
product identity neighborhood in the \(3V+1\) remaining group
variables. The upper bound integrates the recursive open plaquette
forest in CA.9a--CA.9b; it is not a product assumption for the
full action. Comparing the two at \(\beta\) and \((1-s)\beta\)
gives
\[
 \log\frac{Z_n((1-s)\beta)}{Z_n(\beta)}
 \le C_{N,s}V+2d\log(1+\beta).
 \tag{PN.23}
\]
The normalization remains in this ratio. Since
\[
 \mathbb E_{\beta,n}e^{s\beta S}
       =\frac{Z_n((1-s)\beta)}{Z_n(\beta)},
 \qquad
 \mathbb ES=6V\mathbb Es_p,
 \tag{PN.24}
\]
Jensen's inequality proves (PN.20).

For the actual PE sequence,
\[
 \beta_{W,n}\le C(1+K_n'),\qquad
 T_n/a_n=2L^{H_n+K_n'},\qquad
 V_n=(T_n/a_n)^4.
 \tag{PN.25}
\]
Therefore \(\log(1+\beta_{W,n})/V_n\) is bounded, and tends to zero
as the ultraviolet depth grows. The finitely many initial members
can be absorbed into the same constant. This uses PE.17 and
PE.21, not an unidentified physical normalization of the coupling.
\(\square\)

The proof of this first-moment bound does not require the more
substantial local chessboard estimate. That estimate, CA.16--CA.18,
is used only for the higher moments in Section 5.

## 4. The identity coefficient is now controlled

### Theorem PN.3 (P): the actual F01 scalar counterterm budget

On the stopped sequence, use the precise finite F01 prescription
where it is nonsingular. There are fixed \(0<c_m\le C_m<\infty\)
such that
\[
 c_m\le e_a:=\beta_a a^4m_{a,T}\le C_m.
 \tag{PN.26}
\]
Consequently
\[
 a^4c_{a,T,\mu}
   =e_a\,\frac{z_{S,a,T,\mu}}{\beta_a}>0,
 \tag{PN.27}
\]
and (PN.1)--(PN.2) follow.

**Proof.** Combine the exact scalar identity (PN.7) with
Theorems PN.1--PN.2. Orthogonality of the seven projectors and
positivity of their multipliers give
\(\|Z\|_{\rm op}=\max_hz_h\). Hence
\[
 B_a\le b_a
 =B_a+e_a z_S/\beta_a
 \le(1+C_m)B_a.
 \tag{PN.28}
\]
All these quantities refer to the same Wilson law and the same
finite physical prescription. \(\square\)

In particular, a proved channel budget
\[
 \frac{\|Z_a\|_{\rm op}}{\beta_a}
       \le C[1+\log(\ell_0/a)]^\gamma
 \tag{PN.29}
\]
would imply the **same logarithmic power** for \(b_a\), and
\[
 |c_a|\le C a^{-4}[1+\log(\ell_0/a)]^\gamma.
 \tag{PN.30}
\]
There is no further logarithmic loss in the identity term.
Channel-specific upper and lower powers for \(z_S/\beta_a\)
transfer directly to \(a^4c_a\) through (PN.27).

The bare identity coefficient is naturally of order \(a^{-4}\)
times its scalar channel budget. A bounded dimensionless
\(a^4c_a\) is not a bounded unscaled \(c_a\).

The same estimates hold for the explicit totalization F.35 wherever
that bookkeeping definition is used, because it still sets
\(c=z_Sm\). At a zero measurement, however, the totalization does
not solve that channel's physical normalization equation. This
observation supplies no missing nondegeneracy assertion.

## 5. Consequences for the actual transported source

### Corollary PN.4 (P): one coefficient budget suffices in CS and ER

For the actual normalized cutoff fields of (PN.10), the compact
Wilson local-energy reserve gives
\[
 \|\Phi_{\alpha,a}(x)\|_{L^p(\mu_a)}
       \le C B_a\,a^{-4}p,\qquad p\ge1.
 \tag{PN.31}
\]
Thus \(b_a\) may be replaced by a fixed constant times \(B_a\)
in the source collar and ancient-history estimates CS.17,
CS.19, CS.22 and ER.4--ER.6.

**Proof.** The finite clover identities give the pointwise bound
\[
 |\widetilde q_{\alpha,a}(x)|
       \le C_Na^{-4}\sum_{p\in\mathcal P_x}s_p,
 \tag{PN.32}
\]
where \(\mathcal P_x\) is the fixed finite stencil. It follows from
\(\|U_p-I\|_{HS}^2=2s_p\), the finite clover sum, and
Hilbert--Schmidt Cauchy--Schwarz; the scalar repair adds only
the same finite energy sum.

CA.16--CA.18 on the PE geometry imply
\[
 \|\beta_a\widetilde q_{\alpha,a}(x)\|_p
       \le C_Na^{-4}p.
 \tag{PN.33}
\]
Those estimates apply because their proof only needs the compatible
fixed reflection blocks and the bounded partition-ratio density.
Both are supplied by PE.21 and (PN.23)--(PN.25). They do not require
the unproved physical endpoint matching.

Now
\[
 \Phi_a
 =Z_a\bigl(\widetilde q_a-m_ae_S\bigr)
 \tag{PN.34}
\]
exactly. Minkowski's inequality and the finite number of components
give (PN.31). This is the same original microscopic field in every
source-free conditional kernel. Conditional expectation remains an
\(L^p\) contraction, so the CS arguments apply without another
identity budget. \(\square\)

The full one-point Schwinger function of these fields is identically
zero at every cutoff. Their conditional first moments at retained
cuts can be nonzero. Equation (PN.34) does not discard those outer
means or the higher source vertices of CS.10--CS.11.

## 6. What the remaining finite normalization problem actually is

Introduce the dimensionless physical data
\[
 D_{h,a}:=\beta_a^2n_{h,a,T},\qquad
 t_{h,a}:=z_{h,a,T,\mu}/\beta_a,\qquad
 \widehat c_a:=a^4c_a.
 \tag{PN.35}
\]
The exact finite system is now
\[
 t_h^2D_h=\lambda_h,\qquad
 \widehat c=e_at_S,\qquad
 c_m\le e_a\le C_m.
 \tag{PN.36}
\]

### Proposition PN.5 (P): budget and determinant equivalences

Whenever \(D_h>0\) for all seven channels,
\[
 t_h=\sqrt{\lambda_h/D_h},\qquad
 B_a=\max_h\sqrt{\lambda_h/D_h}.
 \tag{PN.37}
\]
For any positive prescribed scale function \(L_a\), the following
are equivalent up to fixed constants:
\[
 b_a\le C L_a
 \quad\Longleftrightarrow\quad
 B_a\le C' L_a
 \quad\Longleftrightarrow\quad
 D_{h,a}\ge c\,\lambda_h L_a^{-2}
       \quad\hbox{for every }h.
 \tag{PN.38}
\]
Also
\[
 \|\beta_aZ_a^{-1}\|_{\rm op}
       =\max_h\sqrt{D_{h,a}/\lambda_h}.
 \tag{PN.39}
\]
Thus logarithmic upper and lower bounds on the seven \(D_h\)
give the corresponding logarithmic bounds on the scaled
normalization and its inverse. A polynomial version of the lower
bound, with \(L_a=a^{-\gamma}\), is precisely the coefficient
budget required for ER.2, with no separate scalar-identity input.

The Jacobian of (PN.36) in \((t_h,\widehat c)\), with the
seven measurement equations first, has determinant
\[
 \det J=-2^7\prod_h t_hD_h
       =-2^7\prod_h\sqrt{\lambda_hD_h}.
 \tag{PN.40}
\]
Its inverse has the explicit action
\[
 \delta t_h=\frac{t_h}{2\lambda_h}\,\delta F_h,\qquad
 \delta\widehat c=e_a\delta t_S-\delta F_0,
 \tag{PN.41}
\]
where \(\delta F_h\) and \(\delta F_0\) are changes in the
equation values with the data held fixed. In particular its
norm is at most \(C(1+\max_ht_h)\). The scalar mean introduces
no additional ill-conditioning.

**Proof.** Equations (PN.37)--(PN.39) follow from the exact
orthogonal diagonalization and (PN.28). The last row of the
Jacobian has \(e_a\) in the scalar-channel column and \(-1\)
in its last column. The first seven rows are diagonal with
entries \(2t_hD_h=2\lambda_h/t_h\). This proves
(PN.40)--(PN.41). \(\square\)

This proposition does not supply the lower bounds in (PN.38).
The existing raw compact estimate gives only
\[
 D_{h,a}\le C_{\mu,N}a^{-8},
 \tag{PN.42}
\]
by Cauchy--Schwarz and (PN.33) on the fixed normalization lobe.
That upper bound is useful for finite-cutoff control but is
weaker than the logarithmic upper bound required for the inverse
budget. In particular, an upper moment bound on a microscopic
field cannot be substituted for a lower separated reflected norm.

## 7. An additional microscopic nondegeneracy estimate

### Proposition PN.6 (P): conditional small-ball bound

For \(\beta\ge1\), any plaquette \(p\), any one of its links \(b\),
and the true conditional law with all other raw links fixed,
there are constants \(C_N,u_N>0\), independent of the exterior,
such that
\[
 \mathbb P_{\beta,n}
   \{\beta s_p\le u\mid U_{b^c}\}
       \le C_Nu^{d/2},
 \qquad 0<u\le u_N.
 \tag{PN.43}
\]
Consequently, for every \(0<q<d/2\),
\[
 \mathbb E_{\beta,n}
       [(\beta s_p)^{-q}\mid U_{b^c}]\le C_{N,q}.
 \tag{PN.44}
\]

**Proof.** The conditional potential can be written
\(A_b(V)=6N-\operatorname{ReTr}(VM)\), where \(M\) is the
sum of six unitary staples, after the orientation conventions
are absorbed. Thus \(\|M\|_{\rm op}\le6\). Let \(V_0\) minimize
\(A_b\). Its first derivative vanishes, and for a unit
Lie-algebra direction \(X\),
\[
 \left|\frac{d^2}{dt^2}A_b(V_0e^{tX})\right|\le6.
 \tag{PN.45}
\]
On a fixed identity chart this implies
\(A_b(V_0e^X)\le A_b(V_0)+3\|X\|^2\).
The Haar Jacobian is bounded below there. Integrating a ball
of radius \(c\beta^{-1/2}\) gives the conditional partition bound
\[
 \int_Ge^{-\beta A_b(V)}\,dV
       \ge c_N\beta^{-d/2}e^{-\beta A_b(V_0)}.
 \tag{PN.46}
\]
The conditional Haar density is therefore at most
\(C_N\beta^{d/2}\), uniformly in the staples.

For fixed exterior, the plaquette holonomy as a function of
\(V\) is a left/right translate of \(V\) or \(V^{-1}\), so its
Haar distribution is Haar. The exact identity
\(s(U)=\|U-I\|_{HS}^2/2\), the nondegenerate identity chart
and compactness give
\[
 \operatorname{Haar}\{U:s(U)\le v\}\le C_Nv^{d/2}
 \quad(0<v\le v_N).
 \tag{PN.47}
\]
Multiply this by the conditional density bound, with
\(v=u/\beta\), to obtain (PN.43). Choose \(u_N\le v_N\).

Finally split the tail integral for \((\beta s_p)^{-q}\)
at a fixed small \(u_N\). The small-\(u\) part is bounded by
a constant times
\(\int_0^{u_N}u^{d/2-q-1}\,du\), which is finite precisely
for \(q<d/2\); the remainder is bounded by \(u_N^{-q}\).
This proves (PN.44). \(\square\)

This is microscopic energy nondegeneracy, not the separated
reflected norm of a centered composite. The latter is the
square of a conditional mean on the reflection-plane links.
Centered local fluctuations can have positive variance and
still have zero such conditional mean. Therefore neither
(PN.12) nor (PN.43) proves the missing lower \(D_h\) bound.

## 8. What exact physical normalization gives in a common limit

### Theorem PN.7 (C): the prescribed nondegeneracy survives hierarchy convergence

Suppose that along one cofinal sequence:

1. all seven \(n_{h,a,T}\) are positive and the exact F01
   prescription (PN.10) is used;
2. the mixed full Schwinger functions of these same fields
   converge on compact coincidence-flat joint tests, on one
   common subsequence.

Hypothesis 1 is now supplied on the slow-volume stopped sequence
of Corollary FN.5 in finite reflected witnesses.
Hypothesis 2 remains the physical hierarchy input; bounded-probe
kernel compactness alone does not establish it.

Then the limiting one-point functions vanish and the limiting
separated reflected channel measurements satisfy
\[
 \mathcal N_h(S_2)=\lambda_h(\mu)>0.
 \tag{PN.48}
\]
In particular no hypercubic channel disappears from the limiting
field hierarchy. More precisely, after averaging the reflected
Gram matrices over the finite signed hypercubic symmetry group,
the Gram matrix on \(E\) is
\[
 \overline G=\sum_h\lambda_h(\mu)P_h,
 \qquad
 \langle u,\overline Gu\rangle
       \ge\lambda_{\min}(\mu)\|u\|^2.
 \tag{PN.49}
\]
Thus every nonzero tensor direction has a nonzero separated
field measurement in the finite symmetry orbit of the fixed
physical normalization probe.

**Proof.** The normalization lobe and its reflection stay a
fixed positive physical distance apart. Each tensor contraction
in F.22 is therefore a compact smooth joint test vanishing in
an entire neighborhood of the coincidence diagonal. It belongs
to the common test space in hypothesis 2. Its finite-cutoff
measurement equals \(\lambda_h\) exactly by (PN.10), so its
limit has that value. The one-point assertion follows from
the exact cutoff centering.

Let \(G\) be the \(21\times21\) reflected Gram matrix at the
fixed lobe and plane. It is positive semidefinite by the
original Wilson reflection positivity and passage of this
finite family of joint tests. Its channel traces obey
\(\operatorname{Tr}(P_hG)=d_h\lambda_h\).
Average \(D(g)^*GD(g)\) over the finite signed hypercubic
group. This positive selfadjoint average commutes with every
\(D(g)\). The seven sectors are the fixed inequivalent real
irreducible sectors of F01. The eigenspaces of a commuting
selfadjoint operator are invariant, so it is scalar on each
sector, and its off-sector blocks vanish. The preserved
channel traces identify the scalar as \(\lambda_h\), proving
(PN.49).

Equivalently, this average is taken over the physically rotated
and reflected probe geometries. Their covariance follows from
the exact finite hypercubic tensor law, which passes to the
same limiting hierarchy. If a nonzero tensor direction vanished
as a field distribution, all its symmetry-related measurements
would vanish, contradicting (PN.49). This argument requires
no full continuous-rotation restoration. \(\square\)

The theorem proves passage of the specified nondegeneracy,
not hypothesis 1 or hypothesis 2. A free curvature-bilinear
hierarchy can also satisfy these positive measurements.
They do not establish the interacting ultraviolet coefficient,
a nonzero physical coupling in a specified continuum scheme,
or the complete Yang--Mills identification.

## 9. The narrow remaining reflected-susceptibility input

The exact site-reflection square formula identifies
\[
 n_{h,a,T}
 =\frac1{d_h}\sum_{i=1}^{d_h}
 \left\|\mathbb E\!\left[
    \langle e_{h,i},B_a(\widetilde q_a)\rangle
             \mid U_{\partial}\right]\right\|_2^2,
 \tag{PN.50}
\]
where \(U_\partial\) are the shared links on the two
site-reflection planes. All conditional and exterior measures
in this formula are the actual normalized Wilson measures.
It follows from the same complete source and its actual
centering, as in the reflected normalization convention.

For a vector of centered plane-measurable witnesses \(W\), the
Hilbert-space projection inequality gives a useful sufficient
lower bound. If
\[
 V_W=\mathbb E[WW^*]>0,\qquad
 C_{hW}=\mathbb E[
       \beta_a P_h B_a(\widetilde q_a)\,W^*],
 \tag{PN.51}
\]
then
\[
 D_{h,a}\ge\frac1{d_h}
       \operatorname{Tr}
       (C_{hW}V_W^{-1}C_{hW}^*).
 \tag{PN.52}
\]
This follows by orthogonally projecting the conditional
mean in (PN.50) onto the span of \(W\); its squared norm is
the displayed matrix expression. It is valid with the
Moore--Penrose inverse after restriction to the actual
positive covariance range.

Equation (PN.52) is a sufficient test, not a computed Wilson
lower bound. Using a Gaussian covariance in place of the
actual \(C_{hW}\), or a current-scale stencil in place of
the transported microscopic \(B_a(\widetilde q_a)\), would
change the problem. The matrix must be estimated through
the exact full source transport, including its outer
conditional means.

## Remaining conditions

| Obligation | Status after this note |
|---|---|
| Actual scalar mean in the F01 identity direction | P: two-sided bound (PN.26), uniformly on the PE sequence. |
| Independent identity-coefficient budget | P: reduced exactly to the scalar channel multiplier, with no extra logarithmic exponent; (PN.27)--(PN.30). |
| Separate identity assumption in CS/ER's coefficient budget | P: eliminated through (PN.2) and PN.4. |
| Microscopic Wilson energy small-ball nondegeneracy | P: conditional (PN.43)--(PN.44); its distinct scope is explicit. |
| Finite normalization and inverse-Jacobian algebra | P: exact formulas (PN.36)--(PN.41); quantitative data bounds remain required. |
| Strict positivity of all seven actual measurements on one slow-volume PE sequence | P in subsequent Corollary FN.5: the actual finite normalization and determinant are nonsingular on that sequence. |
| Nondegeneracy of a common physically normalized hierarchy limit | C: proved under the two explicit hypotheses of PN.7. |
| Uniform logarithmic upper/lower bounds for the seven positive reflected data | O: these remain the quantitative actual-model normalization estimates. |
| Actual seven one-step mixing coefficients and summable matrix remainder | O: F03/F04 are not established by the source-free C05 estimate. |
| Prescribed physical B05 endpoint and full state compatibility | O: the stopped emergent positive endpoint alone does not establish them. |
| ER.7 for the recent separated full microscopic hierarchy | O: the source estimate remains necessary; only its identity-budget input is simplified here. |
