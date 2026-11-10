# Constraints, finite jets and decorated components

## 4.1 Normalization, fixed maps and finite-cutoff identities

**Normalization obstruction (P).** At zero source the literal bare exponent in P2 is \(-\beta_a\sum_ps_p\), whereas the Wilson term written in N1-S(v) at scale zero would have coefficient \(x_0=\beta_a/(2N)\) multiplying the same \(s_p\). The prescribed bare initialization has no generated E/R/B activities: their sums start at \(j=1\), B119 (2.25), (2.30), (2.40), pp.259–261, and Theorem 1, p.262. The difference is not a constant function of the links. A vacuum-energy subtraction cannot correct it. Nor can the permitted bounded \(e_0\) absorb a coefficient difference proportional to \(x_0\), which grows with \(K\) by N2-F(iv). Comparing the identity configuration with a small one-link perturbation makes this last assertion immediate: the same nonzero plaquette increment would have two coefficients differing by an unbounded amount. In Balaban's normalized trace, the coefficient is instead (2.1). A consistent dictionary can repair the convention, but the repair must be stated. This is the existing ICR-N1-1, not a new dynamical obstruction to this approach.

If a running dictionary \(X_k=c x_k\) with \(c=2N^2\) is established, the recurrence converts exactly to

\[
X_{k+1}=X_k-cb_0\log L+\widetilde r_k(X_k),\qquad
\widetilde r_k(X)=c r_k(X/c),\qquad
|\widetilde r_k(X)|\le c^2C_r/X,
\quad |\widetilde r_k'(X)|\le c^2C_r/X^2.
\tag{4.1; P: conditional conversion, not an assumed running dictionary}
\]

The bare relation alone does not prove that running dictionary. We use the literal coefficient in each checked Gaussian calculation, and use N2-F for numerical consequences only in its own variable.

**Integral preservation (P).** Integrate (2.3) first in \(u'\). Its prefactor integrates to one, so \(\int P\rho=\int\rho\). The same is true coefficientwise for a finite source polynomial. Hence freezing a reference kernel at zero source is compatible with exact source differentiation. The resulting marked representation need not have the original finite-source normal form.

At finite cutoff the link space is compact and each Wilson or clover insertion is bounded. For any finite list of smooth tests the bare generating integral is an entire function of their complex coefficients, by dominated convergence on compact parameter sets. Its value at zero is positive; therefore its logarithmic derivatives at zero exist. This finite-cutoff fact provides no radius uniform in the cutoff and no uniform bound on those derivatives. Finite jets use only these derivatives and require no uniform source disc.

For a log jet \(\Phi=\xi\Phi_f+\zeta\Phi_g+\xi\zeta\Phi_{fg}\), expanding its finite exponential proves (2.5). Applying the fixed kernel proves the exact numerators. Writing \(Q=\sigma/\sigma(1)\) then gives

\[
D_f\log\sigma(e^\Phi)|_0=Q\Phi_f,\qquad
D_{fg}\log\sigma(e^\Phi)|_0
=Q\Phi_{fg}+\operatorname{Cov}_Q(\Phi_f,\Phi_g).
\tag{4.2; P}
\]

These identities apply to the complete incoming exponent. At the bare scalar scale \(\Phi_f=N\sum_pf_pa_p\) and \(\Phi_{fg}=0\); the latter is generally false after one integration. The same algebra transports the finite tensor marks, but it does not prove their required analytic or scale bounds.

## 4.2 The full B119 step, boundary jets and cutoff surfaces

#### 4.2.1 The measure that is actually differentiated

B119 (3.15), pp.267–268, and (3.23)–(3.25), p.270, retain all previous operations \(T_k\). The new conditional integral is inside \(T_{k+1}=T^{(k+1)}T_k\). Let \(A\) be its interior free fluctuation coordinate, \(a\) the retained exterior fluctuation, \(H=C^*\Delta^{(k)}C\), \(C_\Lambda=(H|_\Lambda)^{-1}\), and \(h_a=H_{\Lambda,\Lambda^c}a\). The complete zero-source interior weight has the form

\[
\begin{split}
d\sigma_{\mathrm{in}}(A;v,\omega)
={}&z_{\mathrm{in}}^{(k)}\chi^{(k)}(A)
\exp\{-\tfrac12\langle A,HA\rangle-\langle A,h_a\rangle
-\tfrac12\langle h_a,C_\Lambda h_a\rangle\\
&\qquad+P^{(k)}+\Delta E_k+\Delta R_k+\Delta B_k
+G_{\mathrm{geom}}+V_{\mathrm{loc}}^{(k)}\}\,dA.
\end{split}
\tag{4.3; L/P: full factor ledger; exact remainders defined below}
\]

Here \(v\) denotes every variable held fixed during this integration and \(\omega\) its selected geometry. The field arguments of the increments are the full frozen minimizing and constraint-straightening maps, starting with
\(U_k(\exp i[g_kCA-h\widetilde D(g_kCA)]V^{(k)})\), with the exterior field included. The term \(P^{(k)}\) contains the nonlinear Wilson and gauge remainder and the Haar/constraint Jacobians. The increments \(\Delta E_k,\Delta R_k,\Delta B_k\) are their values on this field minus their values on the extracted background. The cutoff-localization change contributes \(V_{\mathrm{loc}}^{(k)}\). The geometry term \(G_{\mathrm{geom}}\) is defined by subtracting the frozen uniform-coefficient Wilson expansion from the **full incoming exponent**.

This definition fixes the exact exponent independently of typography. Section 4.19 checks the definition of \(P^{(k)}\) in B109, proves the negative geometry increment (4.118), and records the incompatible positive increment printed in B119 (3.15). That finite sign question is resolved there. The full-exponent differentiation identities and absolute bounds below are unchanged.

The exterior operation has the Gaussian factor
\(\exp\{-\tfrac12\langle a,Ha\rangle+\tfrac12\langle h_a,C_\Lambda h_a\rangle\}\), as well as the exterior group integration, averaging delta functions, selectors and characteristic functions. Its second term cancels the compensating term in (4.3). Dropping either factor changes the original integral. Extracted background values remain inside the old and exterior integrations when they depend on their variables.

Let \(\widehat\Phi_I\) be the pullback of every complete incoming source coefficient by all these frozen maps. Set \(c_I(v,\omega)=\widehat\Phi_I(0,v,\omega)\), \(W_I=\widehat\Phi_I-c_I\). Then

\[
\begin{aligned}
I_f&=I_0c_f+\sigma_{\mathrm{in}}W_f,\\
I_{fg}&=I_0(c_{fg}+c_fc_g)+c_f\sigma_{\mathrm{in}}W_g
+c_g\sigma_{\mathrm{in}}W_f
+\sigma_{\mathrm{in}}(W_{fg}+W_fW_g),
\quad I_0=\sigma_{\mathrm{in}}1.
\end{aligned}
\tag{4.4; P}
\]

The coefficients include derivatives of the incoming Wilson coefficient, E/R/B activities, vacuum subtractions, and any source-bearing old factor not otherwise unrolled. Nothing is counted twice. Equation (4.4) follows by multiplying the finite exponential in §4.1. If the inner log coefficients are \(A_I^{\mathrm{in}}\), the later normalized integration gives

\[
A_{fg}^{\mathrm{all}}
=Q_{\mathrm{out}}A_{fg}^{\mathrm{in}}
+\operatorname{Cov}_{Q_{\mathrm{out}}}
 (A_f^{\mathrm{in}},A_g^{\mathrm{in}}).
\tag{4.5; P}
\]

The outer measure contains the inner mass \(I_0\). This is the law of total covariance, proved by substituting (4.4) into the outer integral. A function constant in \(A\) can still contribute to the second term of (4.5).

#### 4.2.2 Boundary interpolation

For \(Z_u=\int e^{V+uB}\,d\nu\), the fundamental theorem of calculus gives \(\log Z_1-\log Z_0=\int_0^1Q_uB\,du\). Differentiating a normalized expectation gives \(D_fQF=QF_f+\operatorname{Cov}(F,A_f)\). Differentiating once more proves (3.2), including its third cumulant. Thus two external marks require three distinguished vertices in this boundary calculation: the unmarked boundary interaction and the two source vertices. No third external source is introduced.

Use the actual multiscale analytic carrier norm of B119 (3.43), p.276, with marked and boundary anchors retained. Suppose uniformly in \(u\), on the common complex domain and under its decouplings, \(\|A_I\|\le a_I\), \(\|B_I\|\le b_I\), and the unmarked cluster majorant has a fixed strict margin admitting normalized auxiliary potentials. Then, at a smaller decay exponent,

\[
\begin{aligned}
\|D_f\Delta_B\|&\le C(b_f+b_0a_f),\\
\|D_{fg}\Delta_B\|&\le C(b_{fg}+b_fa_g+b_ga_f+b_0a_{fg}+b_0a_fa_g).
\end{aligned}
\tag{4.6; P under the stated analytic admission}
\]

To prove this, add one auxiliary parameter per distinguished vertex, with radius equal to a fixed part of the unused domination margin divided by its norm. The absolutely convergent connected series is analytic in these parameters. Its first, second and third coefficients are the expectation, covariance and third cumulant. Cauchy's formula bounds them by the corresponding products of vertex norms. A contributing connected cluster contains all distinguished vertices, so it retains every required anchor. A smaller carrier exponent pays the finite rooted convolutions. Integrate in \(u\). This proves the bound; it does not prove the incoming marked norms. The mechanism is the actual numerator/denominator cluster cancellation in B119 (3.44)–(3.47), pp.277–278, and B116 Lemma 3, (2.38)–(2.41), pp.20–21.

The frozen cutoff-localizing map \(T_H\), B119 (3.21)–(3.22), p.269, also acts on all old marked terms. Its source coefficient is \(\Phi_I\circ T_H-\Phi_I\). If \(\Phi_I\) is bounded by \(b_I\) on an analytic ball with margin \(\rho\), and the displacement and connecting segment remain within half that margin, Cauchy's directional derivative formula gives

\[
|\Phi_I(T_Hz)-\Phi_I(z)|\le 2b_I\|T_Hz-z\|/\rho.
\tag{4.7; P}
\]

The displacement has the boundary localization factor \(e^{-R_k}\). Its cost must be measured against the actual scale-dependent analytic margin, not a uniform radius invented for older layers.

#### 4.2.3 The signed cutoff-surface numerator

The exterior-fluctuation interpolation in B119 (3.28)–(3.29), pp.271–272, differentiates the cutoff after Gaussian integration by parts. To retain that term exactly, define

\[
I_u(s,t)=\int\chi(A)e^{-\frac12 AHA-u h\cdot A+V_u(A;s,t)}dA,\quad
\nu_u(F)=\int(h\cdot C_\Lambda\nabla\chi)F\,e^{-\frac12 AHA-u h\cdot A+V_u(A;0,0)}dA.
\tag{4.8; P: definitions}
\]

For a hard cutoff \(\nabla\chi\) is a signed boundary measure, obtained also by smooth approximation. It is never divided pointwise by \(\chi\). Let \(D_u=\partial_u-h\cdot C_\Lambda\nabla_A\), \(G_u=D_uV_u\), \(Z_u=I_u(0,0)\), \(q_u=\nu_u(1)/Z_u\). Gaussian integration by parts gives

\[
\log I_1-\log I_0-\tfrac12\langle h,C_\Lambda h\rangle
=\int_0^1\{Q_{u;s,t}G_u-q_u(s,t)\}\,du.
\tag{4.9; P}
\]

Indeed, integrating the constant vector field \(C_\Lambda h\) gives
\(h\cdot QA=q_u-u\langle h,C_\Lambda h\rangle+Q(hC_\Lambda\nabla V_u)\). Substitution in \(\partial_u\log I_u=Q(\partial_uV_u-h\cdot A)\) proves (4.9), including the Schur compensation.

Write \(\Psi_I=D_I V_u|_0\). The mixed derivative of its expectation is
\(QG_{fg}+\operatorname{Cov}(G_f,\Psi_g)+\operatorname{Cov}(G_g,\Psi_f)+\operatorname{Cov}(G_0,\Psi_{fg})+\kappa_3(G_0,\Psi_f,\Psi_g)\), with \(G_I=D_u\Psi_I\). The signed quotient contributes

\[
\begin{aligned}
D_fq_u={}&\nu_u(\Psi_f)/Z_u-q_uQ\Psi_f,\\
D_{fg}q_u={}&\nu_u(\Psi_{fg}+\Psi_f\Psi_g)/Z_u
-\nu_u(\Psi_f)Q\Psi_g/Z_u-\nu_u(\Psi_g)Q\Psi_f/Z_u\\
&-q_uQ(\Psi_{fg}+\Psi_f\Psi_g)
+2q_u(Q\Psi_f)(Q\Psi_g).
\end{aligned}
\tag{4.10; P}
\]

These are the quotient rule, and (4.9) gives them a minus sign. They are absent from an analysis of smooth potential derivatives alone.

Here is a precise sufficient analytic input. Suppose the localized surface quotient is bounded by \(\tau_{\mathrm{surf}}\), with its anchor, throughout a total auxiliary-potential norm budget \(\delta\). If complete vertices have sizes \(a_f,a_g,a_{fg}\), auxiliary parameters of radii \(\delta/(2a_f),\delta/(2a_g)\), and separately \(\delta/(2a_{fg})\), give

\[
\|D_fq\|\le 2\tau_{\mathrm{surf}}a_f/\delta,\qquad
\|D_{fg}q\|\le
2\tau_{\mathrm{surf}}a_{fg}/\delta
+4\tau_{\mathrm{surf}}a_fa_g/\delta^2.
\tag{4.11; P under the surface-majorant hypothesis}
\]

The field-differentiated vertices \(D_u\Psi_I\) need their actual Cauchy-margin bounds as well. B119 (3.37), p.274, explicitly retains a differentiated-cutoff numerator; p.277 treats its localized expectation. The unshifted regular sector has the usual Gaussian tail after a domination margin is reserved. For the exterior interpolation the conditional Gaussian mean is \(-uC_\Lambda h_a\). A tail estimate at threshold \(R\) requires a quantitative distance of this mean from the cutoff surface, or the actual generalized surface majorant. For example \(|m|\le(1-\delta_0)R\) in a coordinate with bounded variance gives an \(e^{-c\delta_0^2R^2}\) tail by the elementary Gaussian estimate. The required mean/threshold margin is not implied by the unshifted calculation. The complete marked verification of (4.11) in every mixed-scale sector remains open.

## 4.3 History-volume reserve and raw propagation through repeated R-operations

#### 4.3.1 The reserve that the published cancellation permits

The measure here is the actual post-cancellation component kernel of LFR II (1.71), pp.378–379. Its numerical history proof has a positive cost \(C\mathcal V\), with \(\mathcal V\) defined in (2.6). For every fixed \(s>0\), the same proof, with a sufficiently small fixed coupling ceiling, gives

\[
\sigma_{X,v}(e^{s\mathcal V})\le\varepsilon_k,
\qquad
\varepsilon_k=\exp\{-2(1+\beta_0)^{-1}p_0(g_{B,k})\},
\qquad
\sigma_{X,v}(\mathcal V^m)\le m!s^{-m}\varepsilon_k.
\tag{4.12; P in the checked LFR component setting}
\]

Here \(\beta_0\) is Balaban's history parameter, not the flow coefficient. To verify the first inequality, multiply each fixed history by \(e^{s\mathcal V}\). It is constant in all its field integrations and changes only \(C\) to \(C+s\). LFR II (1.81), p.385, bounds the accumulated future cost of a component by a fixed multiple of \(M^dL^{d+1}R_j^{d+2}(d_j'(Z)+1)\). Equation (1.82) supplies a seed cost proportional to \(A_1^2p_0(g_j)^2(d_j'(Z)+1)\). Equations (1.83)–(1.88), pp.385–387, sum shrinking, births and mergers with strict logarithmic-power margins, retaining the displayed final suppression. The strict power inequality on p.383 also pays the preparatory terms. Any fixed increase in \(C\) is absorbed by narrowing the coupling ceiling. All reference denominators and their Wilson cancellations remain unchanged. The last inequality in (4.12) follows from \(u^m\le m!s^{-m}e^{su}\).

This argument does not justify weakening a Wilson numerator with its reference denominator frozen. If \(xA(u)=C(v)+E(u,v)\), that proposed shortcut would introduce

\[
\frac{\int e^{-(1-\kappa)xA(u)}d\nu}{\int e^{-xA(u)}d\nu}
=e^{\kappa C(v)}
\frac{\int e^{-(1-\kappa)E(u,v)}d\nu}{\int e^{-E(u,v)}d\nu}.
\tag{4.13; P}
\]

The determinant ratio does not bound \(e^{\kappa C(v)}\). The cancellation of precisely this background action is visible in LFR II (1.10), p.358, and (1.30)–(1.32), p.364. No full-energy exponential moment is claimed here.

For still-explicit bare plaquettes in the actual counted old-history domains, including fixed collars, the scale-volume count gives \(\#\mathcal P(\omega)\le C\mathcal V\). Since \(0\le s_p\le2N\), their scalar payload has \(|F_f|\le C\|f\|_\infty\mathcal V\). This does not count all microscopic plaquettes in a current coarse box as though they were one old-scale block.

An admitted local vertex has a history envelope if its carrier norm (2.7) and the actual cutoff \(|B|\le P_j\) give
\(\sum_{Y:Y\cap Z_j\ne\varnothing}|W(Y,B)|\le C a_j(1+P_j^2)|Z_j|_j\), with \(\sup_ja_j(1+P_j^2)<\infty\). Sum the exponential carrier weights rooted at each block in \(Z_j\), then use (2.6). This proves the envelope for such a vertex. Establishing that hypothesis for every transported old jet is part of the marked induction.

#### 4.3.2 Finite jet norm and all affine orders

For the algebra in §2, multiplication only keeps disjoint label sets. Consequently

\[
\|\mathbf a\mathbf b\|_{\boldsymbol\tau}
\le\|\mathbf a\|_{\boldsymbol\tau}\|\mathbf b\|_{\boldsymbol\tau},
\qquad
\left\|\int\mathbf a\,d\sigma\right\|_{\boldsymbol\tau}
\le\int\|\mathbf a\|_{\boldsymbol\tau}d\sigma.
\tag{4.14; P}
\]

Indeed, expand the product coefficient as a sum over disjoint pairs and take absolute values. The product of the two norms contains every such term and additional nonnegative terms. The second inequality holds coefficientwise. Supremum norms of analytic coefficients obey the same inequalities.

For affine marks \(|F_i|\le a_i\mathcal V\),

\[
\left\|\sigma e^{\sum_i\xi_iF_i}\right\|_{\boldsymbol\tau}
\le\sigma\prod_i(1+\tau_i|F_i|)
\le\sigma e^{(\sum_i\tau_i a_i)\mathcal V}
\le\varepsilon_k
\quad\text{if }\sum_i\tau_i a_i\le s.
\tag{4.15; P}
\]

Choosing \(\tau_i=s/(2ma_i)\) proves (3.1), because \(m^m\le e^m m!\). A zero \(a_i\) removes that mark. Directly (4.12) even gives \(|\sigma\prod_iF_i|\le m!s^{-m}\varepsilon_k\prod_i a_i\); the radii in (4.15) also control all lower coefficients simultaneously and are useful for the polymer theorem.

For complete incoming two-jets, suppose
\(|A_f|\le b_f\mathcal V\), \(|A_g|\le b_g\mathcal V\), \(|A_{fg}|\le b_{fg}(\mathcal V+\mathcal V^2)\). Equations (2.5), (4.12) give

\[
\left\|\sigma e^{\xi A_f+\zeta A_g+\xi\zeta A_{fg}}\right\|_\tau
\le\varepsilon_k\left[1+\frac{\tau_fb_f+\tau_gb_g}{s}
+\tau_f\tau_g\left\{\frac{b_{fg}}s+\frac{2(b_{fg}+b_fb_g)}{s^2}\right\}\right].
\tag{4.16; P}
\]

This is a finite-jet bound. It does not assert an exponential moment of \(\mathcal V^2\) for an ordinary nonzero source. Under the admitted complex-background comparison \(|d\sigma_z/d\sigma_0|\le M\), the same raw bounds have the factor \(M\). No lower bound on \(\sigma_z1\) is used. LFR II (1.73), p.380, supplies this comparison in its own background domain; it is not an external-source nonvanishing theorem.

#### 4.3.3 Unrolling only the operations that are actually positive

Consider a finite tree of frozen positive integrations, history sums and products on component factors. Give its input factors primitive log jets \(F_{f,\ell},F_{g,\ell},C_{fg,\ell}\). Multiplication adds log jets in the commutative finite algebra, and Fubini unrolls the positive integrations. The complete raw result is exactly

\[
\mathbf t=\sigma_{\mathcal T}
[1+\xi F_f+\zeta F_g+\xi\zeta(C_{fg}+F_fF_g)],
\qquad F_i=\sum_\ell F_{i,\ell},\quad C_{fg}=\sum_\ell C_{fg,\ell}.
\tag{4.17; P}
\]

Source-free reference normalizers remain in the joint kernel. This identity can also be proved by induction on the tree using (4.14). No intermediate component is divided by its mass.

If nonnegative primitive budgets \(v_\ell\) satisfy
\(\sum_\ell v_\ell\le\mathcal V\),
\(|F_{i,\ell}|\le b_i v_\ell\), and
\(|C_{fg,\ell}|\le b_{fg}(v_\ell+v_\ell^2)\), then \(\sum v_\ell^2\le\mathcal V^2\). Thus (4.16) bounds (4.17) independently of the number of R nestings. This proves the raw composition assertion in Theorem 3.2.

The budgets are substantive input. One cannot undo all earlier small-field renormalization, count its microscopic insertions against a single current block, and invoke (4.17). Previously extracted regular and boundary jets must carry their proved renormalized budgets. Likewise, a background value that becomes variable in a later operation must enter the later payload. These are the exact limits of the depth-independent assertion.

#### 4.3.4 A sufficient all-order nonlinear primitive envelope

The raw method also handles nonlinear log jets without an ordinary exponential moment of \(V^2\). Suppose their symmetric multilinear operator norms satisfy
\(\|A_m(\omega)\|\le C^m(m!)^p V(\omega)^m\), with one fixed \(p\ge1\), and \(A_0=0\). The derivative of \(e^A\) is its set-partition sum. Since
\(\prod_{B\in\pi}|B|!\le m!\), and ordering blocks and then ordering their entries gives at most \(m!2^{m-1}\) permutations with cuts,

\[
\sum_{\pi\in\Pi_m}\prod_{B\in\pi}(|B|!)^p
\le(m!)^{p-1}\sum_{\pi\in\Pi_m}\prod_{B\in\pi}|B|!
\le(m!)^p2^{m-1}.
\tag{4.17a; P}
\]

It follows that \(\|(e^A)_m\|\le(2C)^m(m!)^pV^m\), and the single history reserve gives

\[
\|\sigma((e^A)_m)\|
\le\varepsilon(2C/s)^m(m!)^{p+1}.
\tag{4.17b; P under the displayed primitive envelope}
\]

Primitive sums preserve that envelope when their budgets sum to \(V\), because \(\sum_\ell v_\ell^m\le V^m\). This includes a second log coefficient bounded by \(V^2\). It is a single unrolled-stage implication. Repeatedly treating each integrated output as a new unrelated primitive would increase the factorial exponent and would not prove the invariant all-order RG bound.

## 4.4 The polymer logarithm with raw jet coefficients

Work first at finite volume, as on each lattice torus. Let \(\mathcal P\) be the actual polymer family, with symmetric incompatibility \(X\nsim Y\), including self-incompatibility. Activities \(\mathbf K(X)\) take values in the finite jet algebra with analytic coefficient norm. Let \(\ell(X)\) include the fixed joining cost so that the carrier cost of a connected union is at most the sum of its vertex costs. Suppose

\[
\sum_{Y\nsim X}\|\mathbf K(Y)\|_\tau
 e^{\kappa\ell(Y)+a(Y)}\le a(X)
\quad\text{for all }X,\qquad a(X)\ge0.
\tag{4.18; C: explicit cluster majorant}
\]

The partition function includes the compatible empty family, with value one. Its connected logarithm is

\[
\log\mathbf Z
=\sum_{n\ge1}\frac1{n!}
\sum_{X_1,\ldots,X_n}
\phi^T(X_1,\ldots,X_n)\prod_{j=1}^n\mathbf K(X_j)
=\sum_Z\mathbf R(Z),
\tag{4.19; P under (4.18)}
\]

where \(\phi^T\) is the connected-graph sum of products of \(-\mathbf1_{X_i\nsim X_j}\), and \(Z\) is the union carrier. In particular,

\[
\sum_{Z\ni b}e^{\kappa\ell(Z)}\|\mathbf R(Z)\|_\tau
\le\sum_{X\ni b}\|\mathbf K(X)\|_\tau
 e^{\kappa\ell(X)+a(X)}.
\tag{4.20; P}
\]

**Proof.** Submultiplicativity reduces the absolute series to scalar weights \(b(X)=\|\mathbf K(X)\|_\tau e^{\kappa\ell(X)}\). For hard-core incompatibility the absolute connected-graph coefficient is bounded by the sum over spanning trees of the incompatibility indicators. One proof orders vertices, assigns every connected graph its breadth-first tree with a fixed parent tie-break, and partitions connected graphs into intervals between that tree and its permitted extra edges. Summing the alternating signs on each interval has modulus at most one.

The rooted tree sum is bounded by the monotone iterates \(T_0(X)=1\),
\(T_{n+1}(X)=\exp\{\sum_{Y\nsim X}b(Y)T_n(Y)\}\). The exponential accounts for unordered children with their factorials. Hypothesis (4.18) implies inductively \(T_n(X)\le e^{a(X)}\). Passing to the limit bounds all rooted trees. A cluster whose union contains \(b\) has at least one vertex containing \(b\); choosing such a root only overcounts. The resulting factor changes \(1/n!\) to \(1/(n-1)!\), proving (4.20).

The identity between the compatible-family sum and the exponential of its connected graphs is a formal combinatorial identity. The absolute bound just proved permits evaluation, first on finite families and then by exhaustion whenever the total activity sum is finite. On an infinite lattice with only the rooted bound, the conclusion is convergence of local connected activities; a finite global logarithm is not asserted. The scalar body of this cluster partition function is nonzero, so the finite nilpotent logarithm is well defined. No individual activity or component mass is required to be nonzero. Uniform convergence on smaller analytic domains preserves analyticity. This proves (4.19)–(4.20).

If a coefficient with mark \(i\) vanishes unless its carrier contains that source anchor, every term in its mixed connected coefficient has a connected union containing all its anchors. Exponential carrier decay then pays their separation. A raw second coefficient can be disconnected; connectedness is imposed by the logarithm, not assumed prematurely.

**Application to LFR II (P with explicit marked inputs).** Equations (1.90)–(1.91), p.388, have exactly this empty-family-one structure. The activities contain products of the raw operations \(T'_k(X)\); (1.92) uses their unnormalized small masses. Assume their complete jets have the bound (4.16), and the actual localized interaction differences have an algebra norm strictly within the smallness margin of (1.93), uniformly on the prescribed background domain. The Mayer identity is valid in the finite algebra, with \(\|e^{\mathbf V}-1\|\le e^{\|\mathbf V\|}-1\). Repeat (1.92) with norms. Fixed numerical factors per component are absorbed by the suppression margins in (1.95)–(1.96), after a smaller fixed coupling ceiling if necessary. The carrier count in (1.97) gives (4.18). Equations (1.98)–(1.100), pp.389–390, therefore give

\[
\|\mathbf R^{(k)}(X)\|_\tau
\le C e^{-c'p_0(g_k)}e^{-\kappa'd_k(X)}
\tag{4.21; P for regular output carriers under the stated inputs}
\]

with \(\kappa'<\kappa\). This proves the erased-component clause of Theorem 3.2. The intermediate connectedness discounts distances inside surviving regions. Ordinary-distance decay in (4.21) applies to the selected regular carriers disjoint from those regions. Boundary carriers retain the modified norm until their surviving-component weight pays the missing distance.

There is also an order-uniform algebraic fact. For symmetric multilinear source jets \(J_m\), including their anchored operator norms, set

\[
\|J\|_{r,q}=\sum_{m\ge0}\frac{r^m}{(m!)^q}\|J_m\|,\qquad q\ge1.
\tag{4.22; P: factorially weighted jet norm}
\]

The Leibniz binomial in the product, after these weights, is multiplied by \(\binom{m}{k}^{1-q}\le1\). Thus this norm is submultiplicative. Positive kernels and the same polymer theorem act in this Banach algebra whenever the **input** bound and strict majorant hold in it. For \(q>1\) it is an algebra of formal derivative jets, not a claim that their ordinary source Taylor series converges. This proves that these algebraic operations need not increase the factorial order. Establishing one fixed \(q\) for the complete incoming hierarchy, its extractions and its surviving decorations is a remaining analytic task.

## 4.5 Surviving large-field components and weighted boundary decorations

LFR II (1.103)–(1.104), pp.391–392, factors each surviving mass \(t_i=T'_k(Y_i)1\) outside a boundary expression using normalized operations \(Q_i=T'_k(Y_i)/t_i\). Thus the erased-component theorem alone does not finish this sector.

**Why an ordinary marked boundary norm does not follow (P).** Let \(\sigma_n\) have two atoms of equal weight, total mass \(t_n=e^{-2sn}\), history size \(V=n\), and affine mark \(F=n\epsilon\), \(\epsilon=\pm1\). Then \(\sigma_n(e^{sV})=e^{-sn}\), but the second log derivative of \(\sigma_n(e^{zF})\) is \(n^2\). With a small source-free boundary factor \(H=e^{\alpha\epsilon}\),

\[
B(z)=\log Q_zH
=\log\cosh(\alpha+nz)-\log\cosh(nz),\quad
B'(0)=n\tanh\alpha,\quad B''(0)=-n^2\tanh^2\alpha.
\tag{4.23; P}
\]

Its unmarked value is \(O(\alpha^2)\), yet its marked derivatives are unbounded. The full raw expression is \(t(z)e^{B(z)}=e^{-2sn}\cosh(\alpha+nz)\), which retains its small weighted moments. This is a counterexample to an inference from the stated bounds, not to Yang–Mills theory.

**Complete two-mark bound (P).** Let \(t=\sigma1\), \(Q=\sigma/t\), and use log marks \(F,G,C\) with envelopes \(b_fV,b_gV,b_{fg}(V+V^2)\). Quotient differentiation gives

\[
D_f QH=Q(FH)-QF\,QH,
\quad
D_{fg}QH=Q((FG+C)H)-Q(FH)QG-Q(GH)QF
-Q(FG+C)QH+2QFQGQH.
\tag{4.24; P}
\]

For bounded source-independent \(H_1,\ldots,H_n\), Leibniz and Hölder imply

\[
\begin{split}
\left|D_{fg}\left[t(\xi,\zeta)\prod_{r=1}^nQ_{\xi,\zeta}H_r\right]_0\right|
\le\big[&(1+2n)b_{fg}\sigma(V+V^2)\\
&+(4n^2+6n+1)b_fb_g\sigma(V^2)\big]
\prod_r\|H_r\|_\infty.
\end{split}
\tag{4.25; P}
\]

For completeness, a second derivative on one normalized factor contributes at most \(2b_{fg}Q(V+V^2)+6b_fb_gQ(V^2)\). Derivatives on two distinct factors give \(4n(n-1)b_fb_g\sigma(V^2)\), since \((QV)^2\le QV^2\). The two prefactor cross terms contribute \(4nb_fb_g\sigma(V^2)\); its own derivative contributes the remaining raw terms. Summing proves (4.25). The first derivative has bound \((1+2n)b_f\sigma(V)\prod_r\|H_r\|_\infty\).

A strict cluster occurrence margin pays the polynomial \(n^2\). Marked boundary functions are handled by the same Leibniz rule and their admitted analytic carrier norms. Thus a convergent boundary expansion can carry the complete two-jet **with the associated raw masses retained**. It need not carry a uniformly bounded isolated \(D_{fg}B\). Under complex background continuation the relative bounds \(|d\sigma_z/d\sigma_0|\le M\), \(|t_z|\ge c t_0\) give the same statement with fixed \(M,c\)-dependent constants and the existing operator majorant per occurrence. LFR II (1.73)–(1.75) is the relevant domain-specific comparison.

**All-order affine refinement (P).** There is a useful extension when the marks are affine and the \(H_r\) themselves are source independent. Put \(F=\sum_i z_iF_i\), \(|F_i|\le a_iV\). For one component the exact expression is
\(t[Qe^F]^{1-n}\prod_{r=1}^nQ(e^F H_r)\). In its formal expansion, absolute values of the reciprocal coefficients are bounded by the coefficients of

\[
G_n(z)=e^{nz}(2-e^z)^{-(n-1)},\quad n\ge1,\qquad
G_n\bigl(1/[8(n+1)]\bigr)\le e.
\tag{4.26; P}
\]

To justify this majorant, expand the reciprocal in powers of \(Qe^F-1\). Every resulting product of conditional moments, of total degree \(m\), is bounded by \(Q(V^m)\) by Hölder. Replacing those moments by one leaves exactly the nonnegative scalar coefficient majorant in (4.26). Its bound follows from \(e^r-1\le2r\) and \(-\log(1-u)\le2u\) at the displayed small radius. Cauchy's coefficient estimate, or the nonnegative series bound at that radius, now gives

\[
\left|D_1\cdots D_m\left[t(\mathbf z)\prod_{r=1}^nQ_{\mathbf z}H_r\right]_0\right|
\le e\varepsilon(m!)^2
 [8(n+1)/s]^m\prod_i a_i\prod_r\|H_r\|_\infty.
\tag{4.27; P}
\]

There is no extra polarization factorial: the coefficient of \(z_1\cdots z_m\) in \(G_n(\sum a_i z_i)\) is \(m![z^m]G_n\prod a_i\). Equation (4.12) supplies the other factorial. The case \(n=0\) is the raw moment estimate.

For a charged occurrence majorant with \(\sum_\Gamma w_\Gamma\varepsilon_\Gamma e^{\delta(n_\Gamma+1)}\le B_*\), use \(u^m\le m!\delta^{-m}e^{\delta u}\) to sum (4.27). The resulting bound is

\[
eB_*(m!)^3[8/(s\delta)]^m\prod_i a_i.
\tag{4.28; P for the stated affine decorated series}
\]

For several independent component kernels at fixed exterior data, choose one replica per component as a single joint raw expectation. Only the repeated normalized occurrences cost: with \(n_j\) occurrences of component \(j\), put \(r=\sum_j(n_j-1)_+\). The same absolute moment argument has scalar majorant \(G_{r+1}\); passive components introduce no additional occurrence factor. The joint history budget and its moment bound must be the actual product-kernel budget.

This closes a stagewise all-order affine estimate. It does not prove that arbitrary incoming nonlinear log jets and their repeated extractions retain one factorial order through the complete RG. The norm (4.22) specifies the needed stronger input.

Spatial decay also needs its proper weight. The boundary connectedness discounts the interior of each surviving \(Y_i\). Its raw moment must pay the missing ordinary tree distance, using a proved inequality between that distance and its actual history budget. The unreduced old region and its operations remain in the representation. None is erased by the preceding estimates.
