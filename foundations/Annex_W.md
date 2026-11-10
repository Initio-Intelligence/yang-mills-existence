# Source-free identities, complete conditional density and normalized histories

**Annex W.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md). Identifying the calibrated Gaussian marginal with the Wilson trajectory also requires GC, including the bounded error uniform in depth.


### 0. Result and scope

This chapter gives the source formulas and a finite-cutoff construction for B-01, C-01, and H-01, subject to the published source-free construction's stated admissibility hypotheses. It is not a proof that the actual Wilson coupling trajectory satisfies those hypotheses. B-02 remains open as a whole: its geometric part can be made explicit, but its requested coupling-ceiling verification is not supplied by geometric arithmetic.

The distinction between an exposed source input and a new analytic estimate is essential. The localized reference density below is the actual one in Balaban's LFR I (1.100), not the schematic full density of its introduction. All history probabilities come from nonnegative primitive integrals. Individual cluster activities and their absolute values are never treated as probabilities.

The conditional-density identity is written directly from the physical exponent in CMP119 (2.23). This avoids an unresolved sign comparison with the decomposed expression (3.15). All variables and Jacobians are retained; no estimate from a homogeneous conditional law is imported for the complete law by this rewriting.

The finite conditional construction applies to the Wilson measure under CL. Its uniform coupling ceiling is a separate hypothesis.

### 1. Conventions and primary scope

Fix \(SU(N)\), \(N\ge2\), with normalized Haar measure on each positively oriented link. For a periodic four-dimensional lattice, write

\[
s_p(U)=N-\operatorname{Re}\operatorname{Tr}U_p,
\qquad
A(U)=\sum_p\left(1-\frac1N\operatorname{Re}\operatorname{Tr}U_p\right).
\tag{1.1}
\]

The actual Wilson law and the source's initial density are

\[
d\mu_W(U)=Z_W^{-1}e^{-\beta_W\sum_p s_p(U)}dH(U),
\qquad
\rho_0(U)=e^{-g_0^{-2}A(U)-\mathcal E_0}.
\tag{1.2}
\]

Here

\[
\boxed{\beta_W=2Nx_0,\qquad g_0^{-2}=X_{B,0}=N\beta_W=2N^2x_0.}
\tag{1.3}
\]

The symbol \(\beta_W\) is deliberately distinct from the small domain parameter called \(\beta\) in the Balaban papers, and from the functions \(\beta_j\) in the coupling recursion. In particular,

\[
\mathscr Z:=\int\rho_0\,dH=e^{-\mathcal E_0}Z_W.
\tag{1.4}
\]

The initial scalar \(\mathcal E_0\) cancels from normalized expectations. Later history-dependent vacuum constants do not separately cancel from history probabilities.

The following published formulas fix the conventions.

- **CMP119:** *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243–285, pp. 251–252, 257–263 and 267–270.
- **LFR I:** *Large Field Renormalization. I. The Basic Step of the R Operation*, CMP 122 (1989), 175–202. The localized quotient and its normalization appear on p. 201.
- **LFR II:** *Large Field Renormalization. II. Localization, Exponentiation, and Bounds for the R Operation*, CMP 122 (1989), 355–392, Theorem 1 on p.355 retains a small-effective-coupling hypothesis. The reference-denominator calculation is (1.2)–(1.11), pp.356–358.
- **CMP109:** *Renormalization Group Approach to Lattice Gauge Field Theories. I*, CMP 109 (1987), 249–301, DOI <https://doi.org/10.1007/BF01215223>. Its p.251 gives the torus geometry, p.252 the normalized trace, and pp.267–268 the constraint-linearization and elimination conventions.

LFR II Theorem 1 assumes \(0<g_j\le\gamma\) for sufficiently small \(\gamma\), along the source-defined effective trajectory. Its discussion expressly does not provide the second-order calculation proposed to remove that assumption. Neither this note nor the numerical recurrence theorem B-04 supplies that missing application. The underlying averaging, variational, propagator, and cluster-expansion theorems remain scoped source inputs, rather than newly reproved results.

### 2. B-01: the actual positive integral construction

#### 2.1 Blocking and gauge normalization

For the source averaging map \(\mathcal M_j\), the complete blocking operator is

\[
(T_j\rho)(V)=\int dH(U)\,
\delta_G(\mathcal M_j(U)V^{-1})\rho(U).
\tag{2.1}
\]

This is CMP119 (0.1), with the index and averaging map displayed. The group delta is normalized against Haar measure, so

\[
\int dH(V)(T_j\rho)(V)=\int dH(U)\rho(U).
\tag{2.2}
\]

Equivalently, the forward blocking kernel is the Dirac probability at \(\mathcal M_j(U)\). The delta notation is not an extra signed density. All formulas containing gauge deltas may be read as finite positive measures on the constrained variables. Absolute continuity with respect to unrestricted link Haar measure is not assumed for an intermediate gauge-fixed output.

The smoothed axial gauge factor of CMP119 (1.5)–(1.7) uses the one-variable normalization

\[
z_j=\int_G \mathbf1_{\{|W-1|<\varepsilon_j\}}
\exp[-g_j^{-2}(1-\operatorname{Re}\operatorname{tr}W)]\,dH(W).
\tag{2.3}
\]

Each noncentral site of a block contributes the corresponding normalized factor. The contour variable transforms by the endpoint gauge transformations, so Haar invariance makes its gauge integral exactly \(z_j\). The source's factor \(z_j^{-(L^4-1)|\Gamma|}\) is therefore required. It is retained before passing to conditional or history probabilities.

The tree-gauge alternative uses normalized Haar deltas on the chosen tree. It is an exact gauge disintegration, not a replacement of an integral by its value at a gauge-fixed field. If the gauge orientation is averaged, use the probability average over signed coordinate permutations; in four dimensions each of the \(2^4 4!=384\) choices has weight \(1/384\). Section 6 records the source notation issue which makes it preferable to write this probability explicitly.

#### 2.2 Selector and history inventory

At finite cutoff the primitive history records the labels introduced by the following decompositions, with all complement branches kept.

| Operation | Source | Actual label and retained restriction |
|---|---|---|
| Initial plaquette split | CMP119 (1.1) | \(P_0\), from the good/bad plaquette test on the \(LM_2R_0\) cubes. |
| Coarse-field split | CMP119 (1.4); general step (3.2) | \(P_{j+1}\), testing the local minimizing background determined by the coarse field. |
| Approximate-fluctuation split | CMP119 (1.8); general step (3.3) | \(Q_{j+1}\), before the normalized free fluctuation variable has been introduced. |
| Current free-field split | CMP119 (1.18); general step (3.16) | \(R_{j+1}\), with both good and bad free-field restrictions. The literal current-coordinate cutoff is retained; see Section 6. |
| Enlarged geometric domains | CMP119 (1.10), (1.20), (2.1)–(2.3), (3.5), (3.20) | \(\Omega_j,\Lambda_j,S_j\), obtained from the preceding labels and their specified cube layers. Small eligible complements are replaced by their specified rectangular hulls. |
| Preparatory R tests | LFR I (1.24)–(1.29), (1.64)–(1.73) | The success/failure of each preliminary integration test and the remaining selected components. A failed component is retained in the nonreplaced sector. |
| Exterior extension test | LFR I (1.75) | \(\chi_{k,\Lambda}\), a condition on the exterior data admitting a regular extension; it is not a condition on a newly sampled reference field. |
| Preparatory fluctuation and final boundary tests | LFR I (1.82), (1.88)–(1.89) | \(\chi'\), boundary half-threshold labels, and the corresponding excluded components. |
| Gauge choices | CMP119 (1.5)–(1.7); LFR I (1.100) | Axial/tree graphs and their explicitly normalized finite averages. |
| Replacement components | LFR I (1.99)–(1.100) | Disjoint selected components \(X_i\), their cores \(\Lambda_i\), and their local determining sets. |

Each elementary indicator insertion has the form \(1=\chi+(1-\chi)\), or the corresponding finite product expansion. Thus a primitive branch has a nonnegative weight. Resummation over labels which produce the same geometry produces sums of such weights. It does not turn a polymer activity into a branch probability.

The geometric labels determine the determining set of CMP119 (2.2), the retained fields of (2.10), and the minimizing background \(U_k=U_{\mathcal B_k}(V)\) of (2.12). All minima, selectors and coordinate maps remain fixed at zero external source for marked calculations.

#### 2.3 The source inductive integral and its terms

Use bold symbols for the three activity classes and \(\mathcal E_k\) for the scalar vacuum term. CMP119 (2.18)–(2.23) reads

\[
\rho_k(V_k)
=\sum_{\{\Omega_j\},\{\Lambda_j\}}
\chi_k(\Omega_k)\,
\mathcal T_k(\{\Omega_j\},\{\Lambda_j\})
\exp\mathcal A_k(w_k,U_k),
\tag{2.4}
\]

\[
\mathcal A_k(w_k,U_k)
=-A(w_k,U_k)+\mathbf E_k(U_k)+\mathbf R_k(U_k)
+\mathbf B_k(U_k,\mathbf a)-\mathcal E_k.
\tag{2.5}
\]

Here \(A(w,U)=\sum_p w(x(p))(1-\operatorname{Re}\operatorname{tr}U_p)\), \(w_k(x)=g_k(x)^{-2}\), and \(\mathbf a\) denotes the retained earlier fluctuation fields. The sum over \(S_j\) is inside \(\mathcal T_k\), as specified in the source.

For disjoint large-field components \(X_i\), the operations factor and commute; within one component their scale order is fixed:

\[
\mathcal T_k\Big(\bigcup_iX_i\Big)=\prod_i\mathcal T_k(X_i),
\qquad
\mathcal T_k(X)=\mathcal T^{(k-1)}(Z_k\cap X)\cdots
\mathcal T^{(0)}(Z_1\cap X).
\tag{2.6}
\]

Before an R modification, the elementary retained operation of CMP119 (2.21) has the following explicit content:

\[
\begin{aligned}
\mathcal T^{(j)}(Z_{j+1}\cap X)
={}&\int dV_j\big|_{\Omega_{j+1}^{c}\cap X}
\delta_G(\overline V_jV_{j+1}^{-1})\zeta(\Omega_{j+1}^{c})\\
&\cdot\int da_j\big|_{Z_{j+1}\cap\Omega_{j+1}\cap X}
\chi(Z_{j+1}\cap\Omega_{j+1}\cap X)\\
&\cdot\exp\left[-\frac12\langle a_j,K_ja_j\rangle
+\frac12\langle a_j,K_jC^{(j)}(\Lambda_{j+1})K_ja_j\rangle\right].
\end{aligned}
\tag{2.7}
\]

The quadratic form is \(K_j=C_j^*\Delta^{(j)}C_j\), with the component restrictions in the source. Cross-component quadratic terms are assigned to \(\mathbf B\); they are not included a second time in (2.7). The function \(\zeta\) is the resummed product of the specified outer characteristic and normalized gauge factors. The R operation changes the selector/domain content and adds the localized reference integrals below. The recursive primitive description gives every resulting case; it does not require pretending that all histories have the unchanged form of one homogeneous Gaussian fiber.

The three activity classes in (2.5) are distinct:

\[
\begin{aligned}
\mathbf E_k(U)
=\sum_{j=1}^k\bigl[&\mathbf E^{(j)}(\Lambda_j,g_{j-1},U)
-\mathbf E^{(j)}(\Lambda_j,g_{j-1},1)\\
&-\beta_j(g_{j-1})A(\phi_j,U)\bigr],
\end{aligned}
\tag{2.8}
\]

\[
\mathbf R_k(U)=\sum_{j=1}^k
\left[\mathbf R^{(j)}(\Lambda_j,U)-\mathbf R^{(j)}(\Lambda_j,1)\right],
\tag{2.9}
\]

\[
\mathbf B_k(U,\mathbf a)
=\sum_{j=1}^k\sum_X
\mathbf B^{(j)}(X,U,\mathbf a,\{S_i\cap X\}).
\tag{2.10}
\]

These are respectively CMP119 (2.25), (2.30), and (2.40)–(2.41). The E activities also have their point/carrier expansion (2.26)–(2.27). The B carriers meet the current old large-field boundary as specified in (2.41); they include boundary cross terms and changes of variables. The E term has coupling and vacuum subtraction, the R term has vacuum subtraction, and B has neither additional subtraction. No new counterterm is inserted by merely rewriting (2.8)–(2.10).

The source's local coupling identity is

\[
w_{j-1}(x)=w_j(x)+\beta_j(g_{j-1})\phi_j(x).
\tag{2.11}
\]

The scalar \(\mathcal E_k\) depends on the geometry history. The statement on CMP119 p.262 is why it must stay inside (2.4) and inside the normalized history weights below.

#### 2.4 The localized R kernel, rather than its introductory surrogate

Fix a selected component \(X\), its core \(\Lambda\), its retained exterior data \(v\), and a selected axial graph \(G\). Let \(V_\Lambda(v)\) be the source's constrained minimizing filling, and \(U_{k,X}\) its localized minimizing-background map. Let \(\zeta_X\) be exactly the localization function in LFR I (1.100). Define the positive reference measure

\[
\begin{aligned}
h_{k,X,G}(dV';v)
={}&dH(V')\big|_\Lambda\,\delta_G(V')
\mathbf1_{\{|(1/i)\log V'(b)|<M_0\varepsilon_k:\ b\in\Lambda\}}\\
&\cdot\exp\left[-g_k^{-2}A\bigl(\zeta_X,
U_{k,X}(V'V_\Lambda(v))\bigr)\right],\\
H_{k,X,G}(v)={}&\int h_{k,X,G}(dV';v),
\qquad K_{k,X,G}(dV'\mid v)=\frac{h_{k,X,G}(dV';v)}{H_{k,X,G}(v)}.
\end{aligned}
\tag{2.12}
\]

This is the numerator and denominator of the localized quotient of LFR I (1.100), with its cutoff (1.101). It is not the complete effective action evaluated at a fresh field. The exterior selector \(\chi_{k,\Lambda}(v)\), the preparatory selectors, earlier integrations, and the numerator action \(\mathcal A_k''\) remain in the old branch weight. They do not enter a different reference denominator.

On the active exterior set, LFR II (1.2)–(1.11) gives a finite, positive reference normalization. The kernel may be extended arbitrarily as a probability on unused null or inactive fibers; the inactive branch itself uses the identity operation.

For a branch whose old variables inside the replacement are \(u\), the operation is exactly

\[
(\mathcal R_{k,X,G}f)(dV',dv)
=K_{k,X,G}(dV'\mid v)\int f(du,dv).
\tag{2.13}
\]

For the disjoint selected components in (1.100), take the product of (2.12), retain the old-component numerator integrations appearing there, and then sum over the admissible component histories and normalized graph choices. Equation (2.13) is the quotient cancellation performed at each such component, with the actual localized reference specified by (2.12). It proves integral preservation by Tonelli:

\[
\int\mathcal R_{k,X,G}f=\int f,
\qquad
\int(R'_k\rho_k)=\int\rho_k.
\tag{2.14}
\]

The latter is LFR I (1.102). The localization and exponentiation in LFR II reorganize these same integrals. Their signed or complex analytic activities are a representation of the integral and are not an additional stochastic branching rule.

#### 2.5 Exact equality with the normalized Wilson law

At every finite cutoff in the admitted source-free domain, expose all primitive selectors, gauge choices, old integration variables, and fresh reference variables. Blocking is (2.1); gauge and selector insertion are normalized identities; coordinate changes have the Jacobians of Section 3; each replacement is (2.13). Consequently their composed positive integral map \(\mathcal P_{0:k}\) obeys

\[
\rho_k=\mathcal P_{0:k}\rho_0,
\qquad
\int\rho_k=\mathscr Z=e^{-\mathcal E_0}Z_W.
\tag{2.15}
\]

For any integrable microscopic mark \(F\), its transported numerator is
\(\mathcal P_{0:k}(\rho_0F)\). Hence

\[
\boxed{
\frac{\int\mathcal P_{0:k}(\rho_0F)}{\int\rho_k}
=\int F\,d\mu_W.
}
\tag{2.16}
\]

The same formula holds coefficientwise for a finite exponential source jet. It does not mean that the original mark may simply be multiplied into the final unmarked density.

### 3. C-01: one complete current-coordinate density

#### 3.1 Constraint elimination and its determinant

At a regular step, choose the same free link coordinates as the source. Let \(Q=(Q_E,Q_R)\) be the linearized averaging constraint, including the source's fixed scale factor when present, where the square block \(Q_E\) acts on the eliminated coordinates and is invertible in the admitted chart. Put

\[
Cz=\begin{pmatrix}-Q_E^{-1}Q_Rz\\z\end{pmatrix},
\qquad QC=0.
\tag{3.1}
\]

The exact Euclidean delta identity is

\[
\int dB\,\delta(QB)f(B)
=\frac1{|\det Q_E|}\int dz\,f(Cz).
\tag{3.2}
\]

It follows by integrating the eliminated variables. It is consistent with the coarea formula, since

\[
\frac{\sqrt{\det(C^*C)}}{\sqrt{\det(QQ^*)}}
=\frac1{|\det Q_E|}.
\tag{3.3}
\]

To verify (3.3), write \(C^*C=I+Q_R^*(Q_EQ_E^*)^{-1}Q_R\) and use the finite-dimensional determinant identity \(\det(I+AB)=\det(I+BA)\). Thus no additional factor \(\sqrt{\det C^*C}\) may be inserted after (3.2); that would count part of coarea twice. The source factor denoted \(z^{(k)}\) includes this linear constraint normalization and its stated convention-dependent constants.

Let \(D\) be the source's analytic linearizing function, with \(D(0)=D'(0)=0\), and let \(h\) be its right-inverse insertion operator. In the source's normalized free variable,

\[
\theta_{k,v}(z)=g_kCz-hD(g_kCz),
\qquad
V_k(z)=e^{i\theta_{k,v}(z)}V^{(k)}.
\tag{3.4}
\]

Here all operators and backgrounds depend on retained data \(v\). They are fixed when differentiating in the current free variable \(z\). The full configuration entering the old effective action is

\[
\Phi_{k,v}(z)=U_k(V_k(z)),
\qquad \Phi_{k,v}(0)=U_{k+1}(v).
\tag{3.5}
\]

Before the delta constraints are eliminated, the change \(B\mapsto B-hD(B)\) contributes the determinant \(\det(I-hD'(B))\). Write \(\sigma_{\mathrm{in},k}\) for the **total** Haar density in the chosen real coordinates on all current integration links. Thus it is already a product over those links, not a one-coordinate constant. After fixed normalization factors are separated, the remaining coordinate density is

\[
J_{k,v}(z)=
\frac{\sigma_{\mathrm{in},k}(\theta_{k,v}(z))}
{\sigma_{\mathrm{in},k}(0)}
\left|\det(I-hD'(g_kCz))\right|.
\tag{3.6}
\]

On an oriented real analytic chart the determinant has its continuously chosen positive sign; the absolute value in (3.6) states the real change-of-variable formula independently of that convention.

The fixed factor can be stated without guessing a power of a Haar normalization. Let \(m\) be the real dimension before linear-constraint elimination, let \(r\) be the real rank of \(Q\), and let \(\sigma_{\mathrm{con},k}(0)\) be the total Haar density at the identity in the real coordinates used for the group-valued constraints. Normalized group delta becomes \(\sigma_{\mathrm{con},k}(0)^{-1}\delta_{\mathbb R^r}\) in those coordinates. The scaling \(B=g_k b\) contributes \(g_k^m\), while its linear delta contributes \(g_k^{-r}\). Equation (3.2) then gives the fixed prefactor

\[
\mathfrak c_{k,v}
=g_k^{m-r}\,
\frac{\sigma_{\mathrm{in},k}(0)}
{\sigma_{\mathrm{con},k}(0)}
\frac1{|\det Q_E(v)|}.
\tag{3.6a}
\]

The normalized gauge factor from (2.3), and any separately imposed graph-constraint normalization, remain separate factors with their actual source conventions. Formula (3.6a) concerns precisely the current Haar measure, group averaging constraints, scaling, and linear elimination just described. In particular there is no factor \(\sigma_{\mathrm{in},k}(0)^{\dim z}\): that would raise an already multiplied Haar density to an unjustified power. All these fixed factors cancel only when conditioning on the same retained datum. They remain in its marginal and in the history normalizers.

#### 3.2 The physical action identity fixes every sign

Let \(G_k(z;v)\) be the actual axial gauge action generated by (2.3), evaluated on (3.4). It has \(G_k(0;v)=0\). Define the complete homogeneous classical difference

\[
\mathscr S_{k,v}(z)
=g_k^{-2}\left[A(\Phi_{k,v}(z))-A(U_{k+1}(v))+G_k(z;v)\right].
\tag{3.7}
\]

The stationary constrained background gives \(D\mathscr S_{k,v}(0)=0\). Define its actual constrained Hessian and exact nonlinear remainder by

\[
K_{k,v}=D^2\mathscr S_{k,v}(0),
\qquad
\mathscr V_{k,v}(z)=\mathscr S_{k,v}(z)-\tfrac12\langle z,K_{k,v}z\rangle.
\tag{3.8}
\]

In the source coordinates \(K_{k,v}=C^*\Delta^{(k)}C\), with the full background-current contribution already inside \(\Delta^{(k)}\). It is not obtained by discarding the nonlinear constraint before differentiating.

For any function \(F\) of the old background and retained old fields, write

\[
\Delta_zF=F(\Phi_{k,v}(z),\mathbf a)-F(U_{k+1}(v),\mathbf a).
\tag{3.9}
\]

For the physical coefficient \(w_k(x)=g_k(x)^{-2}\), the elementary identity

\[
-\Delta_z A(w_k,\cdot)
=-g_k^{-2}\Delta_z A(1,\cdot)
-\Delta_z A(w_k-g_k^{-2},\cdot)
\tag{3.10}
\]

determines the heterogeneous Wilson term. In particular the last sign is fixed by the original negative action, independently of any shorthand for a remainder.

After dividing by the value of the background exponential at \(z=0\), the complete unshifted current-coordinate exponent is therefore

\[
\boxed{
\begin{aligned}
\mathscr L_{k,v}(z)
={}&-\tfrac12\langle z,K_{k,v}z\rangle-\mathscr V_{k,v}(z)
+\log J_{k,v}(z)\\
&+\Delta_z\mathbf E_k+\Delta_z\mathbf R_k+\Delta_z\mathbf B_k
-\Delta_z A(w_k-g_k^{-2},\cdot).
\end{aligned}}
\tag{3.11}
\]

Equation (3.11) is an exact identity obtained from (2.5) and the change of variables. It is not a claim that its seven displayed contributions are small. The E differences include the already chosen local coupling counterterms of (2.8). The R differences include their actual local carriers. The B differences include all old boundary activities and their dependence on retained old fluctuations. None is discarded because it is absent from a homogeneous approximation.

**Older Gaussian factors.** On the C-01 coordinates used here, fixing an older fluctuation or selector can leave its Gaussian density dependent on the current field. For any such unintegrated factor, (3.11) includes the logarithm of its ratio at the current field to its value at zero. In a completed component the source integrates the entire boundary exponential. [Conditional density and older Gaussian factors](../boundary/conditional_density_inputs.md)

The factors of the older operation \(\mathcal T_k\) retained outside the current integral in CMP119 (3.15) and (3.25) stay in the outer law. This separation is the one provided by the source's supported operations, not a claim of independence for an arbitrary choice of a block. If a different coordinate selection makes one of those factors depend on the free variable, its exact logarithmic ratio must be retained in (3.11); there is no permission to freeze it merely by notation.

#### 3.3 Boundary relocation, including its full Jacobian

The boundary localization of CMP119 (1.22) and (3.22) uses a map supported on the specified set \(S_{k+1}\). With a cutoff \(\vartheta_b\) taking values in \([0,1]\), the linkwise formula is

\[
\mathcal F_{H,b}(t_b)
=\frac1{ig_k}\log\left(e^{ig_kt_b}e^{-i\vartheta_b(t_b)H_b}\right).
\tag{3.12}
\]

The cutoff equals the source's smooth interpolant on the appropriate bad-fluctuation boundary links and is identically one on the other shifted links. The background difference \(H\) is exactly (3.22), obtained from the two source minimizing fields with the specified determining sets. On unshifted coordinates \(\mathcal F_H\) is the identity. All these choices are frozen at zero source.

The exact new boundary contribution can be written without losing a Taylor remainder:

\[
\mathscr B_{\partial,k,v}(t)
=\mathscr L_{k,v}(\mathcal F_H(t))-\mathscr L_{k,v}(t)
+\log|\det D\mathcal F_H(t)|.
\tag{3.13}
\]

This is a complete definition of the source's boundary-change contribution before its subsequent localized expansion. It includes the change of every old term and the full Jacobian. In particular one may either use the pulled-back \(\mathscr L\) and the Jacobian, or use \(\mathscr L+\mathscr B_\partial\); using both would count the change twice.

Let \(\mathcal D_{k,v}\) be the intersection of the transformed real selector domains specified by the chosen primitive history. It includes the current good-field tests, the retained large-field tests, the exterior extension test where relevant, and every surviving preparatory test. The exact normalized law is

\[
\boxed{
d\nu_{k,v}(t)
=\frac{\mathbf1_{\mathcal D_{k,v}}(t)
\exp[\mathscr L_{k,v}(t)+\mathscr B_{\partial,k,v}(t)]\,dt}
{\displaystyle\int_{\mathcal D_{k,v}}
\exp[\mathscr L_{k,v}(s)+\mathscr B_{\partial,k,v}(s)]\,ds}.
}
\tag{3.14}
\]

Only active positive-mass fibers are used. An R-reference fiber uses (2.12) instead; an arbitrary inherited coarse fiber is not substituted for that reference law.

#### 3.4 Conditioning on the interior: the Schur complement is not a second action

To identify the quadratic terms in CMP119 (3.23)–(3.25), write \(t=(A,y)\), where \(A\) is free in \(\Lambda_{k+1}\) and \(y\) is the retained current fluctuation outside it. Put \(C_\Lambda=K_{\Lambda\Lambda}^{-1}\), extended by zero outside \(\Lambda\). Then

\[
\begin{aligned}
-\tfrac12\langle A+y,K(A+y)\rangle
={}&\left[-\tfrac12\langle y,Ky\rangle
+\tfrac12\langle y,KC_\Lambda Ky\rangle\right]\\
&+\left[-\tfrac12\langle A,KA\rangle-\langle A,Ky\rangle
-\tfrac12\langle y,KC_\Lambda Ky\rangle\right].
\end{aligned}
\tag{3.15}
\]

The first bracket is the retained Gaussian factor in the new \(\mathcal T^{(k)}\). The second is the inner Gaussian exponent, equivalently the completed square around \(-C_\Lambda Ky\). Their sum is the original quadratic form. This proves the bookkeeping identity and shows exactly where the retained mean occurs. Dropping the cross term would change the conditional law.

The normalized conditional law of \(A\) follows by fixing \(y\) in (3.14). All nonlinear terms in (3.11) and (3.13) are evaluated at the same pair \((A,y)\). Constants independent of \(A\) cancel in this conditional normalization, but they remain in the marginal law of \(y\) and in history weights.

#### 3.5 Terms and domains

| Contribution | Exact place in the current law | Allocation |
|---|---|---|
| Full constrained homogeneous Hessian | \(-\langle z,Kz\rangle/2\) | Retain the source background-current contribution and constraint curvature. |
| All higher classical/gauge terms | \(-\mathscr V\) | Defined as the exact difference in (3.8); no nonlinear term omitted. |
| Heterogeneous Wilson coefficient | \(-\Delta A(w_k-g_k^{-2},\cdot)\) | Sign follows from (2.5), not from a shorthand \(P\). |
| Haar density | \(\log[\sigma_{\mathrm{in},k}(\theta)/\sigma_{\mathrm{in},k}(0)]\) inside \(\log J\) | Insert once; the total input/constraint constants occur in (3.6a). |
| Nonlinear constraint-linearization Jacobian | \(\log|\det(I-hD')|\) inside \(\log J\) | Insert once before elimination, as in the source change of variables. |
| Linear constraint coarea | \(|\det Q_E|^{-1}\), together with fixed scale factors | Outer factor for fixed \(v\); keep in marginal/history normalizers. |
| Inherited E activities and their local subtraction | \(\Delta\mathbf E_k\), expanded by (2.8) | Do not add the same coupling subtraction again. |
| Inherited R activities | \(\Delta\mathbf R_k\), expanded by (2.9) | R analytic sizes are not normalized probabilities. |
| Inherited boundary activities | \(\Delta\mathbf B_k\), expanded by (2.10) | Keep old fluctuation and boundary-data dependence. |
| Boundary-coordinate change | \(\mathscr B_\partial\) | Either use (3.13), or pull back all terms and include its Jacobian. |
| Current and historical selectors | \(\mathbf1_{\mathcal D_{k,v}}\) | Keep actual real support; differentiating a moving support is a separate estimate. |
| Retained Gaussian/mean terms | The two brackets of (3.15) | Preserve cross terms and outer Schur complement. |
| History-dependent vacuum scalar | Outer \(e^{-\mathcal E_k(h)}\) | Cancels within a fixed conditional fiber, not between histories. |
| Fresh replacement normalization | \(H_{k,X,G}(v)\) in (2.12) | Use the localized reference action and its own graph/cutoff. |

This closes an identification problem. It does not give the current-coordinate complex tubes, derivative-carrier bounds, selector boundary estimates, or full conditional moment and decay estimate required by C-02 through C-08.

### 4. H-01: exact normalized history and reset laws

#### 4.1 Primitive path construction

For a fixed finite construction, start with \(U_0\sim\mu_W\). At each chronological operation:

1. expose the next finite selector label according to its actual partition of unity;
2. expose any gauge choice using its normalized gauge or finite graph probability;
3. apply the deterministic blocking or coordinate map, retaining old variables as latent variables;
4. for each active R replacement, sample from the actual kernel (2.12).

The resulting finite path law is the product of \(\mu_W\) and these probability kernels. All compact field spaces, their admitted finite-dimensional coordinate charts, and the finite label spaces are standard measurable spaces; regular conditional laws can be used on their completed probability spaces. The original Wilson field remains a coordinate of this construction, with exactly its original marginal.

Let \(h\) denote the exposed history through scale \(k\), including primitive selector and graph labels before any resummation. Let \(r_{k,h}(dV_k)\) denote its unnormalized output measure. Expanding only primitive positive integrals in (2.4) defines these measures, and

\[
r_{k,h}\ge0,
\qquad
\rho_k(dV_k)=\sum_h r_{k,h}(dV_k),
\qquad
Z_{k,h}=\int r_{k,h}(dV_k),
\qquad
\sum_hZ_{k,h}=\mathscr Z.
\tag{4.1}
\]

If some retained labels are continuous, the same formulas use the corresponding disintegration rather than a finite sum.

The exact normalized laws are

\[
\boxed{
\mathbb P(H_k=h,dV_k)=\frac{r_{k,h}(dV_k)}{\mathscr Z},
\quad
\mathbb P(H_k=h)=\frac{Z_{k,h}}{\mathscr Z},
\quad
\mathbb P(H_k=h\mid V_k)=\frac{dr_{k,h}}{d\rho_k}(V_k).
}
\tag{4.2}
\]

The Radon–Nikodym derivative exists since \(r_{k,h}\le\rho_k\). When both measures are represented against a common reference measure it is the familiar quotient \(r_{k,h}(V_k)/\rho_k(V_k)\). This formulation also covers singular gauge-fixed outputs without a false Haar-density assumption. All formulas are on nonzero-mass sets; arbitrary versions on null sets make no difference. They give the law of a retained history as an exact integral of the actual normalized Wilson construction. The denominator is not replaced by the mass of a convenient reference Gaussian.

**Vacuum-normalization warning.** The common factor \(e^{-\mathcal E_0}\) cancels from (4.2). The factors \(e^{-\mathcal E_k(h)}\) generally depend on the history and are part of \(r_{k,h}\). Removing them from individual branch weights would usually change both probabilities in (4.2).

#### 4.2 Old and fresh conditional laws at a replacement

For an old normalized branch density \(\rho(du,dv)/\mathscr Z\), the exact old–fresh coupling is

\[
d\Pi(u,u',v)=\frac{\rho(du,dv)}{\mathscr Z}
\frac{h_{k,X,G}(du';v)}{H_{k,X,G}(v)}.
\tag{4.3}
\]

Its new marginal is the R quotient (2.13). Its old conditional law, given the augmented output \((u',v)\), is

\[
\Pi(du\mid u',v)=\frac{\rho(du,v)}{\int\rho(d\widetilde u,v)}.
\tag{4.4}
\]

The fresh reference factor cancels from this conditional law. Thus the transported observable is

\[
(QF)(u',v)
=\frac{\int F(u,v)\rho(du,v)}{\int\rho(du,v)}.
\tag{4.5}
\]

The retained data \(v\) must include the history, graph and exterior data deciding which kernel was applied. Conditioning later on an omitted rare event would give a different kernel; (4.5) is not permission to ignore that event's normalizer.

The fresh denominator \(H_{k,X,G}\), the old conditional denominator \(\int\rho(du,v)\), and the history normalizer \(\rho_k(V_k)\) in (4.2) are different objects. Keeping all three separate prevents the incorrect transfer of a fresh-reference estimate to an inherited conditional history.

#### 4.3 Resetting an auxiliary history label

Let the actual joint law at a reset be

\[
d\mu(x,h)=d\bar\mu(x)\,\pi(dh\mid x),
\tag{4.6}
\]

where \(\pi\) is obtained from (4.2) or its corresponding conditional version. The exact reset joint law is

\[
d\Pi_{\mathrm{reset}}(x,h,h')
=d\bar\mu(x)\,\pi(dh\mid x)\,\pi(dh'\mid x).
\tag{4.7}
\]

Both old and new marginals equal (4.6). If the mark is \(F(x,h)\), the transported new mark is

\[
\widetilde F(x,h')=\int F(x,h)\pi(dh\mid x).
\tag{4.8}
\]

For a full finite source jet \(G(x,h;t)\), apply (4.8) to the entire truncated polynomial:

\[
\widetilde G(x,h';t)=\int G(x,h;t)\pi(dh\mid x).
\tag{4.9}
\]

Every integrated coefficient is preserved. If \(G=e^\Psi\), taking the finite formal logarithm after averaging generates all conditional covariance and higher cumulant responses. Averaging only each one-field coefficient and then multiplying would omit those responses.

Equations (4.1)–(4.9), with the actual primitive selectors and reference kernel (2.12), are the normalized-history construction required for marked expectations. They establish no smallness of a bad-history probability. H-02 through H-05 retain that analytic task.

### 5. B-02: explicit geometric progress and the remaining obstruction

#### 5.1 Compatible cubic tori

CMP109 p.251 takes an odd block integer with a lower restriction at 11, torus half-side a power of that integer, and nested center lattices with spacing a negative power. We use an admitted odd \(L\ge13\), so the endpoint ambiguity in the printed text is immaterial. These are cubic tori. No rectangular extension is required for the following construction.

Fix an admitted odd \(L\) and fixed block constants supplied by the source hypotheses. The elementary numerical choices \(L=13\), \(L_0=2\), and domain parameter \(\beta_{\mathrm{dom}}=1/8\) satisfy the displayed restrictions \(L\ge11\), \(2\le L_0<L/2\), \(L_0^2\le L/3\), and \(0<\beta_{\mathrm{dom}}<1/4\). This checks these numerical restrictions only; it is not a claim that every other source parameter or coupling condition is thereby verified.

Write the source radii at a finite cutoff as

\[
R_{j,n}=L^{r_{j,n}},
\qquad
R_{j,n}\ge[\log g_{j,n}^{-2}]^r,
\qquad 0\le j\le K_n,
\tag{5.1}
\]

with the source's least-power choice and fixed \(r\ge2\). Choose an integer \(m_*\) large enough for all the fixed block exponents and finite halo multipliers being used. An explicit adaptive sequence is

\[
K_n=n,
\qquad
M_n=n+m_*+2+\max_{0\le j\le n}r_{j,n},
\qquad
a_n=L^{-n}\ell_0,
\quad T_n=2L^{M_n}\ell_0.
\tag{5.2}
\]

Every source grid whose size is a fixed power of \(L\) times \(R_{j,n}\) at one of the first \(n\) scales divides the period when \(m_*\) includes its fixed exponent. Its finite surrounding layers fit inside the period for sufficiently large \(m_*\). The extra factor \(L^n\) gives an arbitrarily large separation from any fixed support and from these fixed multiples. Any further primary geometric condition involving a different scale-dependent family must be inserted into the maximum before claiming the complete B-02 test.

The number of microscopic sites per direction is

\[
N_n=T_n/a_n=2L^{M_n+n},
\tag{5.3}
\]

which is even. In the source's original coordinates, reflection of the center lattice through time zero sends \(a_n(j+1/2)\) to \(a_n(-j-1+1/2)\). This proves lattice invariance, but the original coordinate plane is a **bond plane**. It does not by itself verify the site-reflection convention used by the chosen field architecture.

The conventions agree after one fixed translation: move the coordinate origin to the coarsest center \(\ell_0/2\) in each coordinate. At stopped scale \(j\), put \(h=L^{j-K_n}\ell_0\). Since \(L\) is odd,

\[
h(\mathbb Z+\tfrac12)-\tfrac{\ell_0}{2}
=h\left(\mathbb Z+\frac{1-L^{K_n-j}}2\right)
=h\mathbb Z.
\tag{5.3a}
\]

Moreover \(T_n/(2h)=L^{M_n+K_n-j}\) is an integer. Thus the planes with translated time coordinates \(0\) and \(T_n/2\) are **site planes at every stopped scale**. This exact coordinate dictionary permits the site-reflection convention of the field construction to be used on the same cubic sequence; it is stronger than mere reflection invariance of the unshifted center grid. Since \(T_n\to\infty\), every fixed compact support eventually embeds with a fixed positive boundary margin.

The choice also pays the elementary geometric condition used in the compact reserve. Indeed \(\beta_{W,0,n}=g_{0,n}^{-2}/N\), while \(N_n\) dominates \(R_{0,n}\). Thus, for weak couplings bounded above by a fixed small number,

\[
\sup_n\frac{\log(1+\beta_{W,0,n})}{N_n}<\infty.
\tag{5.4}
\]

For large \(\log g_{0,n}^{-2}\), its numerator grows linearly in that logarithm and \(R_{0,n}\) grows at least as its power \(r\ge2\); the remaining finite range is bounded. This does not use asymptotic freedom to prove a coupling recursion.

#### 5.2 Why the complete statement remains open

The B-02 statement asks for **every** actual minimum-size, coarse-grid, reflection-plane, and coupling-ceiling condition. Equations (5.2)–(5.4) settle a useful geometric subproblem. They do not establish

\[
0<g_{j,n}\le\gamma
\quad\text{for every }0\le j\le K_n
\tag{5.5}
\]

for the actual Wilson-normalized trajectory required by the source-free theorem. Nor does naming an admitted \(L\) replace a final exhaustive constants ledger. The actual trajectory and its source identification belong to B-03 and B-05. The stated application requires the trajectory and its uniform coupling ceiling.

### 6. Literal-source comparisons and their handling

#### 6.1 Graph-average normalization

On LFR I p.201 the display (1.100) places \(1/N_i\) before a graph sum, while the following prose writes \(N_i=1/(2^dd!)\) for the signed-coordinate averaging choice. Read literally, those two uses of \(N_i\) conflict. This note uses the unambiguous normalized averaging measure: each signed-coordinate choice has mass \(1/(2^dd!)\). This agrees with the word “average” and with the integral normalization (1.102). The notation clash is not interpreted as a failure of the R mechanism.

#### 6.2 The heterogeneous action sign

CMP119 (2.23) has \(-A(w_k,U)\). The displayed curly bracket in (3.15), on p.268, has

\[
+A(w_k-g_k^{-2},\Phi(z))-A(w_k-g_k^{-2},U_{k+1}).
\tag{6.1}
\]

The direct physical-action decomposition (3.10) has the opposite sign. CMP109's prose after (2.12) identifies \(P^{(k)}\) with the homogeneous action and measure contribution. This is therefore recorded as an **unresolved cross-paper sign/convention comparison**, not as a proved misprint.

The current-density identity (3.11) does not rely on resolving that comparison: it is derived directly from the physical exponent (2.5). Before importing a bound stated for the source's shorthand \(P^{(k)}\) into this exact density, the correspondence must be checked. This is part of the remaining conditional-law estimates, not an extra unstated premise of (3.11).

#### 6.3 The printed free-field cutoff

CMP119 p.267 states the scaling \(A'_k=g_kA_k\); its (3.16) on p.268 prints a good-field test \(|A_k|<\delta_k\). The initial-step expression (1.18) instead displays \(|A|<g_0^{-1}\delta_0\). This note does not silently identify the two radii. Any literal cutoff gives an exact partition of unity when its complement is kept, so the normalized identities above remain valid. Which current normalized radius is intended by a subsequently quoted analytic bound must be checked before that bound is used. The real domain \(\mathcal D_{k,v}\) in (3.14) is the actual selected domain, not an enlarged Gaussian domain chosen for convenience.

#### 6.4 No hidden source imports

The published source-free construction assumes small effective couplings. A Wilson application must verify this hypothesis on its normalized trajectory.

Every remaining application condition is assigned to an existing open statement:

| Remaining condition | Catalogue statement retaining it |
|---|---|
| Derive the actual effective coupling recurrence and its quantitative remainder. | **B-03** |
| Identify that trajectory with the physical Wilson coefficient and verify all source-free coupling hypotheses. | **B-05** |
| Exhaust all source parameter/minimum-size conditions and verify the ceilings along one complete cofinal sequence. | **B-02** |
| Admit the complete E contribution, with the correct current coordinates, classical term and heterogeneous correction, on a common contour. | **C-02** |
| Admit the actual R activities and their current-coordinate marginal transfer. | **C-03** |
| Bound the resulting actual E/R derivative carriers and the constants needed to compare any imported shorthand \(P^{(k)}\) with (3.11). | **C-04** |
| Bound old boundary activities and the full boundary-coordinate contribution (3.13). | **C-05** |
| Control heterogeneous determining sets, backgrounds and nonconstant coefficients in (3.11). | **C-06** |
| Fix the actual current cutoff convention for the estimates, retain its real support, and treat selectors and their boundaries. | **C-07** |
| Prove the complete conditional moment and spatial decay theorem for (3.14), rather than a homogeneous surrogate. | **C-08** |
| Identify and bound inherited or unreplaced bad events under (4.2). | **H-02** |
| Localize all responses generated by (4.9). | **H-03** |
| Sum marked bad-history contributions with their actual normalizers. | **H-04** |
| Control the outer retained-mean covariance and higher cumulants. | **H-05** |
