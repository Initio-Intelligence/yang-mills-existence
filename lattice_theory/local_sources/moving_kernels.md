# Cutoff surfaces, extensive cumulants and moving kernels

## 4.12 A volume-independent Gaussian cutoff-surface theorem

This subsection closes a normalization estimate for a complete centered Gaussian layer. It also shows why the corresponding estimate for an arbitrarily retained large-field exterior is false. The distinction matters in applying the cutoff identity of §4.2.

#### 4.12.1 The normalized radial boundary bound

Let \((X,Y)\) be a centered nondegenerate finite-dimensional Gaussian vector, with \(X\in\mathbb R^d\), \(\operatorname{Cov}(X)=\Sigma\le \sigma^2 I\). The dimension of \(Y\) is arbitrary. Let \(D=-D\) be a convex measurable set in the \(Y\)-space. We may additionally multiply the joint Gaussian density by \(e^{-W(X,Y)}\), where \(W\) is even, convex, and finite enough that the integrals below exist. Set \(Z(R)=\int 1_{\{|X|<R\}}1_D(Y)e^{-W(X,Y)}\,d\gamma\), and assume \(Z(R)>0\). A positive boundary integral is defined by the radial derivative, or by monotone smooth approximations to the indicator.

**Proposition 4.12.1 (P).** For \(R>0\) at which the derivative exists,

\[
\begin{split}
0\le \frac{RZ'(R)}{Z(R)}
&\le H_d(R/\sigma),\\
H_d(z)&:=
\left[\int_0^1 t^{d-1}
       \exp\!\left(\frac{z^2}{2}(1-t^2)\right)\,dt\right]^{-1},\\
H_d(z)&\le d e^{1/2}z^d e^{-z^2/2}\quad(z\ge1).
\end{split}
\tag{4.66; P}
\]

The constants have no dependence on the number of other Gaussian coordinates, the correlations between the coordinates, or the smallness of \(Z(R)\). For nonsingular Gaussian density and ordinary ball or box constraints, differentiation under the radial integral supplies the derivative for every positive \(R\) for which the weighted density is continuous; the almost-everywhere statement is sufficient in the general convex case.

**Proof.** Write the conditional Gaussian law as \(Y=M X+\eta\), where \(\eta\) is centered Gaussian and independent of \(X\). Define
\(q(x)=\int 1_D(Mx+\eta)e^{-W(x,Mx+\eta)}\,d\gamma_\eta\).
The integrand is jointly log-concave in \((x,\eta)\): its negative logarithm is a sum of a positive quadratic form, a convex function, and the indicator potential of a convex set. Integration in \(\eta\) preserves log-concavity. Central symmetry also gives \(q(-x)=q(x)\). It follows that \(q(r\omega)\ge q(R\omega)\) for \(0\le r\le R\), along every unit vector \(\omega\).

For completeness, the marginalization fact needed here follows from the integral log-concavity inequality. In one dimension, normalize positive smooth integrands \(f,g\) to mass one and let \(T\) be their increasing transport, so \(T'=f/(g\circ T)\). If \(h((1-t)x+ty)\ge f(x)^{1-t}g(y)^t\), change variables \(z=(1-t)x+tT(x)\), and use
\((1-t)+tT'\ge(T')^t\).
The resulting lower bound for \(\int h\) is \(\int f=1\). Restoring the two masses gives the general inequality. Integrating one coordinate at a time proves it in every finite dimension. Gaussian regularization and monotone convex approximations extend it to the Gaussian times convex-indicator functions used above. Applying the inequality to the two sections of a jointly log-concave function proves log-concavity of its marginal. This is the classical marginalization result stated in Prékopa, *Acta Sci. Math.* 34 (1973), Theorem 6, printed p.342; the argument here gives the needed case directly.

In polar coordinates the unnormalized \(X\)-density on a ray is a constant times
\(r^{d-1}e^{-a_\omega r^2/2}q(r\omega)\), with
\(a_\omega=\omega^T\Sigma^{-1}\omega\ge \sigma^{-2}\).
Its integral from zero to \(R\) is at least
\(q(R\omega)\int_0^R r^{d-1}e^{-a_\omega r^2/2}\,dr\).
Consequently the boundary flux on this ray, divided by its interior mass and multiplied by \(R\), is at most
\(H_d(R\sqrt{a_\omega})\).
The displayed integral defining \(H_d\) shows that it decreases in \(z\). Thus each ray has ratio at most \(H_d(R/\sigma)\); integrating the raywise numerator inequality proves the first bound. For \(z\ge1\), restrict the defining integral to \(0\le t\le z^{-1}\). It is at least
\(e^{(z^2-1)/2}/(d z^d)\), proving the final bound. ∎

The same argument applies when every other coordinate block is restricted to a centered ball, because their product is symmetric and convex. For a scalar cutoff, \(d=1\). For a Lie-algebra link ball, \(d=\dim\mathfrak{su}(N)\), a fixed number. If a different fixed norm is used, the radial argument is made in its star-shaped polar coordinates; the corresponding fixed norm-equivalence constants alter the exponent and prefactor, not their volume independence.

#### 4.12.2 Marked surface quotients and recombination of the exterior Gaussian

Let \(\mu_R\) be the positive interior-cutoff measure in the proposition and \(\nu_R=R\partial_R\mu_R\) its positive radial boundary measure. Put \(\tau=\nu_R1/\mu_R1\). For bounded functions \(W_i\), with \(\|W_i\|_\infty\le a_i\), define
\(F(z)=\nu_R(e^{\sum_i z_iW_i})/\mu_R(e^{\sum_i z_iW_i})\).
This is a complex analytic ratio near zero. With \(\eta_0=\log(3/2)\), throughout \(\sum_i|z_i|a_i\le\eta_0\) its denominator has absolute value at least \(\frac12\mu_R1\), and its numerator at most \(\frac32\nu_R1\). Cauchy's formula therefore gives

\[
\left|\partial_{z_1}\cdots\partial_{z_m}F(0)\right|
 \le 3\tau\left(\frac{m}{\eta_0}\right)^m\prod_i a_i
 \le 3\tau\,m!\left(\frac{e}{\eta_0}\right)^m\prod_i a_i .
\tag{4.67; P}
\]

This estimate is for derivatives of the quotient itself; it includes all derivatives of its normalizer. For a complete exponent
\(zW_f+wW_g+zwW_{fg}\), the chain rule in three auxiliary variables instead yields
\(|F_{fg}(0)|\le3\tau(4a_fa_g/\eta_0^2+a_{fg}/\eta_0)\).
Zero norms are handled by continuity. A bounded real background perturbation whose oscillation is at most \(2B\) increases the unmarked surface ratio by at most \(e^{2B}\). Here \(B\) must be the actual oscillation after cancellation of irrelevant common factors; a bound proportional to the total torus volume would not be useful.

The Gaussian recombination underlying this application is exact. In block coordinates let
\(H=\left(\begin{smallmatrix}H_I&B\\B^*&H_E\end{smallmatrix}\right)>0\),
\(C_I=H_I^{-1}\), and \(h=By\). The complete inner and outer factors satisfy

\[
\begin{split}
&\exp\{-\tfrac12 x^TH_Ix-x^Th-\tfrac12 h^TC_Ih\}
 \exp\{-\tfrac12 y^TH_Ey+\tfrac12 h^TC_Ih\}\\
&\hspace{30mm}
=\exp\{-\tfrac12(x,y)^TH(x,y)\}.
\end{split}
\tag{4.68; P; B119 (3.23), (3.25), p.270 for its occurrence}
\]

The inner conditional mean is \(-C_Ih\), which need not be small. Equation (4.68) nevertheless restores a centered Gaussian after the exterior is integrated. A cross-term interpolation \(B\mapsto tB\), \(0\le t\le1\), retains positivity: its precision is the convex combination of \(H\) and \(\operatorname{diag}(H_I,H_E)\). If the original precision has a lower bound \(cI\), the same lower bound holds throughout this interpolation. More generally the proposition only needs the actual distinguished marginal covariance bound.

For the unmarked, centered Gaussian cutoff term of B119 (3.32), p.273, and the second integral of (3.37), p.274, the cutoff is a product of centered link-ball indicators. The needed current-core covariance estimate is the one checked in §4.6. Thus (4.66) supplies a direct local bound for this Gaussian normalized surface term, with the actual rescaled cutoff radius and covariance normalization inserted. The scale interpolation \(\chi(tX)\) has radius \(R/t\); its derivative contributes \(-R t^{-2}Z'(R/t)/Z(R/t)\). The exponential bound is integrable down to \(t=0\). Section 4.19 now fixes this free-coordinate radius as \(R_k^{\rm fl}=\delta_k/g_k\) and proves its exact surface Jacobians. Nonlinear group cutoffs retain the full pullback (4.121).

This closes the centered Gaussian quotient estimate. Formula (4.67) closes its bounded local marked perturbation version. It does not assert that a full nonlinear Wilson fluctuation potential is even and convex, or that the complete marked boundary potential has the required bounded oscillation. Those are separate applications of the proved estimate, not its hypotheses being silently dropped.

#### 4.12.3 A retained large-field selector can destroy this bound

There is a simple Gaussian counterexample to a stronger statement that would be tempting in the full RG. Let \(X,Y\) be standard centered Gaussian variables with correlation \(0<\rho<1\). Keep the large-field selector \(|Y|\ge M\), and set
\(Z_M(R)=\mathbb P(|X|<R,\ |Y|\ge M)\).
For fixed \(R>0\),

\[
\frac{RZ_M'(R)}{Z_M(R)}\longrightarrow\infty
\quad\text{as }M\longrightarrow\infty .
\tag{4.69; P}
\]

To prove this without an asymptotic expansion, first use the selector \(Y\ge M\). Its marginal \(X\)-density is
\(f_M(x)=\varphi(x)\,\overline\Phi((M-\rho x)/\sqrt{1-\rho^2})\).
For \(|x|\le R\) and \(M>\rho R\), the elementary Gaussian Mills inequality
\(\varphi(z)/\overline\Phi(z)\ge z\), \(z>0\), gives
\((\log f_M)'(x)\ge k_M:=-R+\rho(M-\rho R)/(1-\rho^2)\).
For \(k_M>0\), integration yields
\(\int_{-R}^R f_M(x)\,dx\le f_M(R)/k_M\).
The radial boundary numerator is at least \(R f_M(R)\), so the ratio is at least \(Rk_M\). The selector \(|Y|\ge M\) replaces \(f_M(x)\) by \(f_M(x)+f_M(-x)\); both its interior integral and its boundary integral are twice the corresponding one-sided quantities. The same lower bound applies.

This counterexample has a symmetric but nonconvex retained selector, exactly the property that invalidates the radial monotonicity argument. It does not refute a raw weighted large-field estimate: the probability of the retained event is very small. It proves that the surviving weight cannot be discarded before normalizing. In particular, an argument that cites only a small unshifted Gaussian tail for every fixed large-field exterior would be incorrect even in this two-variable model.

## 4.13 Fixed factorial order under cumulants and extensive raw primitives

Two algebraic estimates sharpen the all-order bookkeeping. They remove avoidable factorial losses, while leaving the analytic question of admitting the complete incoming coefficients explicit.

**Proposition 4.13.1 (P).** Let \(p\ge1\). Suppose the full coefficients for every nonempty labelled subset \(I\) satisfy
\(|M_I|\le C^{|I|}(|I|!)^p\prod_{i\in I}a_i\), with \(M_\varnothing=1\).
Then their connected coefficients satisfy
\(|K_I|\le(2C)^{|I|}(|I|!)^p\prod_{i\in I}a_i\).
The converse implication, from connected coefficients to full coefficients with a changed exponential constant, holds with the same factorial exponent \(p\).

**Proof.** Use the finite partition identities for moments and cumulants. If \(m=|I|\), retain one power of the block factorials and use
\(\prod_{B\in\pi}(|B|!)^{p-1}\le(m!)^{p-1}\).
The remaining sums are

\[
\begin{split}
\sum_{\pi\vdash[m]}(|\pi|-1)!\prod_{B\in\pi}|B|!
 &= (m-1)!(2^m-1),\\
\sum_{\pi\vdash[m]}\prod_{B\in\pi}|B|!
 &=m!\sum_{\ell=1}^m
       \frac1{\ell!}\binom{m-1}{\ell-1}
 \le 2^{m-1}m!.
\end{split}
\tag{4.70; P}
\]

For the first identity, the exponential generating function is
\(-\log(1-z/(1-z))=\log(1-z)-\log(1-2z)\).
For the second, fix \(\ell\), order the blocks, choose their positive sizes, and order the entries in each block. Dividing by \(\ell!\) gives the displayed composition count. Substitution proves both assertions. The argument is an identity of finite jets and needs no analytic source disk. ∎

Thus the extra factorial power allowed in the earlier rough full/connected conversion is unnecessary. This sharpening concerns that conversion; it is not a claim that every RG operation is now bounded in a common all-order norm.

There is a stronger raw integration result when logarithmic primitives are extensive in one common history budget. Let \(\sigma\) be a positive finite measure, let \(V\ge0\), and suppose \(\sigma(e^{sV})\le\varepsilon\), with \(s>0\). In a square-free source algebra take a zero-constant-term logarithmic primitive \(A\), with labelled coefficients satisfying
\(|A_I|\le C^{|I|}(|I|!)^p V\prod_{i\in I}a_i\), \(p\ge1\).
The linear power of \(V\) is part of this hypothesis.

**Proposition 4.13.2 (P).** Its integrated raw exponential obeys

\[
\left|\sigma\!\left([\exp A]_I\right)\right|
 \le \varepsilon\,C^m(m!)^p
          s^{-1}(1+s^{-1})^{m-1}\prod_{i\in I}a_i,
 \qquad m=|I|\ge1.
\tag{4.71; P}
\]

In particular the factorial exponent does not increase.

**Proof.** A partition with \(\ell\) blocks contributes at most
\(C^m\prod_{B\in\pi}(|B|!)^p V^\ell\prod_i a_i\).
The exponential reserve gives \(\sigma(V^\ell)\le\varepsilon\ell!s^{-\ell}\). For a fixed \(\ell\), ordering the blocks as above gives

\[
\sum_{\substack{\pi\vdash[m]\\|\pi|=\ell}}
 \ell!\prod_{B\in\pi}(|B|!)^p
 =m!\!\!\sum_{\substack{n_1+\cdots+n_\ell=m\\n_j\ge1}}
          \prod_{j=1}^{\ell}(n_j!)^{p-1}
 \le(m!)^p\binom{m-1}{\ell-1}.
\tag{4.72; P}
\]

Summing \(s^{-\ell}\binom{m-1}{\ell-1}\) over \(\ell\) proves (4.71). ∎

This hypothesis is preserved when primitive contributions have budgets \(v_\lambda\) with \(\sum_\lambda v_\lambda\le V\) and the same coefficient constants: summing the logarithmic primitives still gives a linear \(V\) bound. Accordingly, the theorem can be applied once to a globally unrolled extensive primitive, independently of its number of contributing stages.

The linear budget cannot be inferred for the logarithm of every normalized surviving component. In the explicit example of §4.5, the second logarithmic derivative is of order \(n^2\) while the carrier budget is \(n\). Such a component must retain its raw weight, or be treated using a proved connected-local decomposition. Equation (4.71) identifies a sufficient invariant structure that avoids accumulating factorial losses; proving that structure for all regular, boundary and surviving sectors is still part of R1/R3.

## 4.14 Normalization of optional positive histories and the physical-cell budget

This subsection proves a normalized estimate for a class of positive history ensembles. Unlike a bound on an individual rare component, its conclusion includes the complete optional partition function in the denominator. The deletion hypothesis is essential.

#### 4.14.1 An insertion inequality with the denominator retained

Fix retained variables \(v\). Let \(\mathcal P\) be a finite or countable family of carriers, with positive finite component measures \(\sigma_X(v,d\eta_X)\). Allowed finite families \(\Gamma\) must be hereditary under deletion: every subfamily, including the empty family, is allowed. Let \(B_\Gamma(v,\eta_\Gamma)\) be a real interaction, with \(B_\varnothing=0\). Suppose, for every allowed disjoint union \(S\cup\Gamma\),

\[
B_{S\cup\Gamma}(v,\eta_S,\eta_\Gamma)
       -B_\Gamma(v,\eta_\Gamma)
 \le\sum_{X\in S}b_X,\qquad b_X\ge0 .
\tag{4.73; C: explicit deletion-cost hypothesis for the application}
\]

The abstract theorem below is valid whenever this displayed hypothesis holds. Define
\(W(v)=\sum_{\Gamma\ {\rm allowed}}\int e^{B_\Gamma}\prod_{X\in\Gamma}d\sigma_X\),
assume \(W(v)<\infty\), and let \(\mathbb P_v\) be the normalized corresponding probability. The empty family gives \(W(v)\ge1\).

**Proposition 4.14.1 (P).** For distinct carriers \(X_1,\ldots,X_r\) and nonnegative payloads \(F_i\),

\[
\mathbb E_v\!\left[
  1_{\{X_1,\ldots,X_r\subset\Gamma\}}\prod_{i=1}^rF_i(\eta_{X_i})
 \right]
 \le\prod_{i=1}^r e^{b_{X_i}}\sigma_{X_i}(v,F_i).
\tag{4.74; P}
\]

**Proof.** For a compatible selected set \(S\), write each numerator family uniquely as \(S\cup\Gamma'\). Apply (4.73) and integrate the selected component variables. The residual partition sum is over allowed families compatible with \(S\), so positivity bounds it by the very same \(W(v)\) in the denominator. They cancel. Incompatible selected families have zero numerator. Monotone finite approximations prove the countable version. No component mass has been divided out. ∎

Let \(D\) be a finite union of physical cells and
\(V_D=\sum_{X\in\Gamma:\,X\cap D\ne\varnothing}V_X\), \(V_X\ge0\).
Expand the finite product for \(e^{sV_D}\), use (4.74) for its selected factors, and drop exclusion restrictions in the positive majorant. This proves

\[
\mathbb E_v e^{sV_D}\le
 \exp U_D(s),\qquad
U_D(s):=\sum_{X:\,X\cap D\ne\varnothing}
          e^{b_X}\sup_v\sigma_X(v,e^{sV_X}-1).
\tag{4.75; P}
\]

A bound \(U_D(s)\le A|D|\) is therefore sufficient for local normalized exponential moments, uniformly in the total torus and under any further positive integration of \(v\). The latter claim follows because the estimate is pointwise in \(v\); the outer measure may contain \(W(v)\) and any other positive factors.

Suppose each of \(m\) affine marks is supported in at most \(q_0\) physical cells and obeys \(|F_i|\le a_i V_{D_i}\). With \(D=\bigcup_iD_i\), use \(V_D^m\le m!s^{-m}e^{sV_D}\). Then
\(|\mathbb E\prod_iF_i|\le m![e^{Aq_0}/s]^m\prod_i a_i\).
Proposition 4.13.1 gives the same factorial exponent for the connected hierarchy. Bounded deterministic terminal contributions can be included by using \(1+V_D\).

The application to a particular RG history ensemble requires both deletion closure and (4.73), as well as the rooted reserve in (4.75). An extensive absolute estimate on \(B_\Gamma\) is not a deletion-cost estimate: terms unaffected by deletion must cancel before the cost is charged. Fixed mandatory exterior components may be included in \(v\); the theorem then controls only the optional components, not source marks inside the mandatory ones.

#### 4.14.2 The ultraviolet anchor count and the dimension-four weight

A raw component reserve at one scale does not by itself prove the physical-cell bound in (4.75). At generation \(j\), a cell of side \(\ell_0\) contains order \((\ell_0/h_j)^4\) anchors. At \(j=0\), N2-F gives \(x_0\) of order \(K\). A component majorant of size \(\epsilon_0=\exp[-c(\log K)^r]\), for a fixed finite \(r\), yields the per-cell majorant \(L^{4K}\epsilon_0\), which diverges. This says that such an upper estimate is insufficient; it does not assert that actual component masses saturate it.

There is a precise weighted remedy. Assume a common positive multiscale ensemble satisfying (4.74), and the scale-wise rooted estimates

\[
\sum_{\substack{X\ {\rm at\ generation}\ j\\X\cap D\ne\varnothing}}
 e^{b_X}\sup_v\sigma_X(v,e^{sV_X}-1)
 \le C|D|(\ell_0/h_j)^4\epsilon_j .
\tag{4.76; C: explicit rooted reserve to verify}
\]

Set \(w_j=(h_j/\ell_0)^4\le1\) and
\(\widetilde V_D=\sum_{X\in\Gamma:\,X\cap D\ne\varnothing}w_{j(X)}V_X\).
Convexity gives \(e^{swV}-1\le w(e^{sV}-1)\) for \(0\le w\le1\). Applying (4.75) with these weighted budgets proves

\[
\mathbb E e^{s\widetilde V_D}
 \le\exp\!\left(C|D|\sum_j\epsilon_j\right).
\tag{4.77; P from the stated rooted hypotheses}
\]

The dimension-four weight cancels the anchor count exactly. If
\(x_j\ge x_*+b_-(K-j)\) and
\(\epsilon_j\le C\exp[-c_1(\log x_j)^r]\) with \(r>1\), the sum is uniformly finite: for any fixed \(q>1\), that exponential is eventually at most \(x_j^{-q}\), and the arithmetic-tail series converges.

This gives a concrete use for the dimension-four field extraction. It does not give that weight to a bare source insertion for free. Vacuum terms and collision contacts must first be subtracted, and the actual remaining payload must satisfy the weighted envelope. Current-scale erased-component estimates are not automatically a single deletion-hereditary multiscale ensemble. LFR II's sum over erasable components, (1.72), p.379, is performed at fixed surviving components; (1.103)–(1.104), pp.391–392, still retains their selectors, constraints and old integrations. Thus the optional theorem has not completed R2 for mandatory survivors.

#### 4.14.3 A finite-energy comparison and a filling obstruction

There is a useful exact benchmark at the terminal scale. For an ordinary Wilson measure with fixed coefficient \(\beta_*>0\), let \(D\) now be a finite set of independent links and \(P(D)\) the plaquettes meeting those links. Given arbitrary exterior links \(v\), its conditional density \(f_D\) relative to product normalized Haar measure satisfies

\[
e^{-2N\beta_*|P(D)|}\le f_D(u\mid v)
       \le e^{2N\beta_*|P(D)|},\qquad |P(D)|\le6|D|.
\tag{4.78; P}
\]

Indeed the exterior-only action cancels, and the remaining action lies between zero and \(2N\beta_*|P(D)|\). Normalizing its exponential proves the bounds. Since \(\beta_*=2N/g_*^2\) is fixed, this comparison has no ultraviolet dependence. Applying it on a microscopic physical cell would instead cost order \(a^{-4}\) links and would not solve the problem.

More generally, a genuine coarse Gibbs representation with
\(\sup_b\sum_{X\ni b}\operatorname{osc}\Phi_X\le B\)
has conditional densities between \(e^{-B|D|}\) and \(e^{B|D|}\). Only potentials meeting \(D\) remain in the conditional action, and their total oscillation is at most \(B|D|\). This proof is independent of torus size. It remains to establish such a representation or a suitable alternative comparison for the **complete** Balaban terminal marginal, after compulsory old histories are included. The pointwise total-volume bound of B119 Corollary 3, (2.50), p.264, does not supply it.

Finally, finite energy does not imply that arbitrary exterior data admit an all-small-plaquette filling. Take a rectangular lattice disk of \(M\) plaquettes and fix its boundary holonomy to
\(H=\operatorname{diag}(-1,-1,1,\ldots,1)\in SU(N)\).
Its operator-norm distance from the identity is two. Peeling the disk one plaquette at a time expresses \(H\) as an ordered product of conjugates of the plaquette holonomies or their inverses. The inequality
\(\|AB-I\|\le\|A-I\|+\|B-I\|\) for unitaries therefore proves

\[
2=\|H-I\|\le\sum_{p\ {\rm in\ disk}}\|U_p-I\|
             \le M\epsilon .
\tag{4.79; P}
\]

If \(M\epsilon<2\), the proposed all-small filling is impossible. A valid local normalization construction must allow a controlled defect, a larger patch, an appropriate exterior decomposition, or another reference configuration. Its cost must be proved with the same exterior data. The obstruction does not rule out these alternatives; it rules out replacing their proof by an unconditional small-field filling assertion.

The admitted shell used by Balaban is more restrictive. LFR I, p.193, explicitly constructs a regular extension on the selector \(\chi_{k,\Lambda}\); Proposition 1, pp.194–195, then constructs its minimizing reference. The arbitrary-boundary example above does not refute that admitted extension. LFR II (1.10)–(1.11), p.358, already supplies the reference denominator after factoring the background Wilson energy and the explicit coupling/Haar constants; its residual logarithm is bounded by \(C\log M\,|\Lambda|\). The missing comparison is between that reference branch and the **complete terminal history ensemble with the same exterior**, including rejected selectors and unreduced old operations. A possible repair keeps a fixed number of terminal bad generations instead of insisting on an empty history; its geometry, constraints, Jacobian and multiplicity costs still need proof.

#### 4.14.4 Normalized moments from a local mass-deficit estimate

There is a weaker alternative to a pointwise lower comparison for every exterior configuration. It allows unfavorable exteriors, provided their complete normalized distribution controls the deficit of the local mass.

Let \(\sigma\) be a positive kernel with \(t=\sigma1>0\) and a proved raw reserve \(\sigma(e^{sV})\le\varepsilon\), \(V\ge0\), \(s>0\). Put \(Q=\sigma/t\) and \(A=\log(\varepsilon/t)\ge0\). Here \(A\) is a logarithmic mass deficit; it is not asserted to be a relative entropy.

**Proposition 4.14.2 (P).** For \(0<\theta<1\) and integers \(m\ge1\),

\[
\begin{split}
Q(V\ge u)&\le \min\{1,e^{A-su}\},\\
Q(e^{\theta sV})&\le e^{\theta A},\\
Q(V^m)&\le m!s^{-m}\sum_{k=0}^{m}\frac{A^k}{k!},
\qquad QV\le A/s .
\end{split}
\tag{4.80; P}
\]

**Proof.** The first bound is Markov's inequality and the fact that \(Q\) is a probability. For the second, concavity of \(z^\theta\) gives \(Q(e^{\theta sV})\le[Q(e^{sV})]^\theta\le e^{\theta A}\). The analogous integral
\(QV^m=m\int_0^\infty u^{m-1}Q(V>u)\,du\)
gives the third estimate, using the elementary integer incomplete-gamma formula. The sharper first-moment bound follows from Jensen:
\(e^{sQV}\le Qe^{sV}\le e^A\). ∎

Apply this to a **complete active-patch kernel** \(\sigma_D(v,d\omega)\), with raw reserve \(\varepsilon_D(v)\), mass \(t_D(v)\), and budget \(V_D\). Let \(\mathbb P_D\) be its actual outer marginal, proportional to \(t_D(v)\) times all remaining positive factors. Exteriors with \(t_D=0\) have zero marginal measure. If

\[
\mathbb E_{\mathbb P_D}
 \exp\!\left[\theta\log\frac{\varepsilon_D(v)}{t_D(v)}\right]
 \le e^{C|D|},
\tag{4.81; O: sufficient complete-patch mass-deficit estimate}
\]

then (4.80) and conditional expectation give
\(\mathbb E_{\rm full}e^{\theta sV_D}\le e^{C|D|}\).
Consequently complete affine mark payloads bounded by \(a_iV_D\), supported in at most \(q_0m\) active cells, have full normalized moments bounded by \(C_1^m m!\prod_i a_i\), with the same factorial order for cumulants. The nonlinear extensive version follows from Proposition 4.13.2 with the normalized reserve.

If the remaining outer measure is \(d\lambda(v)\), condition (4.81) is exactly the fractional integral comparison \(\int\varepsilon_D^\theta t_D^{1-\theta}\,d\lambda\le e^{C|D|}\int t_D\,d\lambda\). This is a proved reduction to (4.81), not a proof of (4.81) for Yang–Mills. The kernel must include every compulsory old integration and decoration carrying the active derivatives; substituting an isolated component kernel would not control the full observable. Unlike a uniform lower bound for \(t_D/\varepsilon_D\), (4.81) needs only a fractional inverse-mass moment under the actual outer law. It is therefore a concrete, potentially weaker R2 target. Neither a total-volume pressure bound nor the raw reserve alone implies it.

## 4.15 Scalar transport, moving reference kernels, and what N2-F does not supply

#### 4.15.1 Numerical tangents and their identification with the source-free family

For a selected set of N2-F functions write \(F_k(x)=x-b+r_k(x)\), \(b=b_0\log L\). On the sufficiently high trajectory of §4.9, \(F_k'\) lies between \(1/2\) and \(3/2\). There is a bare-shift interval \(|s|\le\delta\), independent of the ultraviolet depth, on which their numerical iterates are defined, stay close to the unperturbed trajectory, and obey

\[
x_j^{\rm num}(s)=F_{j-1}\circ\cdots\circ F_0(x_0+s),
\quad |x_j^{\rm num}(s)-x_j|\le C_*|s|,
\quad C_*^{-1}\le\partial_s x_j^{\rm num}(s)\le C_* .
\tag{4.82; P from the selected N2-F functions}
\]

Here the terminal coordinate is chosen inside the allowed range with a fixed positive margin, as permitted by the existential target. To prove (4.82), apply the mean value theorem while the two trajectories stay within distance one. The resulting factors are \(1+r_k'(\xi_k)\), with \(\xi_k\ge x_k-1\). The integral comparison gives
\(\sum_{k<j}(x_k-1)^{-2}\le[b_-(x_j-1)]^{-1}\).
Taking \(\delta\le(2C_*)^{-1}\) improves the distance bound from one to one half, completing a first-exit proof. Differentiating the finite composition and using \(|\log(1+a)|\le2|a|\), \(|a|\le1/2\), gives the two derivative bounds.

Identifying these iterates with the coefficients of the actual nearby source-free family requires a compatibility statement. The quantifier order in N2-F does not expressly say that one collection of functions \(r_{K,k}\) serves all terminal targets. Their being \(C^1\) extensions for each trajectory alone would not say this. The precise common-family statement is **ICR-N1-3** in [Lattice conventions and hypotheses](../lattice_conventions.md), §4; it is not an additional assumed interface.

Under that compatibility statement, the numerical family in (4.82) is the actual family: its terminal value remains admitted, N2-F supplies a trajectory to that target, and strict monotonicity of the common maps makes the high-range preimage unique. Since a constant scalar source \(t\) changes the bare coordinate by \(-ct\), \(c=1/(2N)\), this proves

\[
\mathfrak x_j^{\rm ad}(t)
 =F_{j-1}\circ\cdots\circ F_0(x_0-ct),\qquad
\partial_t\mathfrak x_j^{\rm ad}(0)
 =-c\prod_{\ell<j}(1+r_\ell'(x_\ell)),\qquad
|\mathfrak x_j^{\rm ad}(t)-x_j+ct|
 \le C|t|/(x_j-1).
\tag{4.83; C: actual-family identification requires ICR-N1-3 or its proof}
\]

The last bound follows by integrating the estimate that the derivative product differs from one by at most \(C/(x_j-1)\). These are source-adapted coefficients, obtained by reapplying the entire source-free construction at the shifted bare coupling. They are not automatically the coefficients of a representation whose reference kernels and selectors are all frozen.

There is a concrete reason for this distinction. B119 (0.1), p.243, defines the physical block transformation by averaging against \(\delta(\overline U V^{-1})\); its kernel has no coupling parameter. The representations of that map use coupling-dependent cutoffs, coordinates and reference replacements. Moreover B109, final paragraph on p.298, expressly records dependence of its beta coefficient on earlier couplings. A derivative along the coherent family is different from a derivative with respect to arbitrary independently varied irrelevant activities.

#### 4.15.2 Exact reference-kernel derivatives and an actual LFR bound

Fix a geometry, exterior data \(v\), a gauge constraint and an integration domain \(d\mu_v(u)\). For a positive differentiable reference \(h_{\mathbf t}\), set
\(H_{\mathbf t}=\int h_{\mathbf t}\,d\mu_v\),
\(q_{\mathbf t}=h_{\mathbf t}/H_{\mathbf t}\), and
\(P_{\mathbf t}\psi=q_{\mathbf t}\int\psi\,d\mu_v\).
Derivatives are taken on this fixed domain with a valid integrable majorant. Let \(Q=q_0d\mu_v\),
\(a_f=\partial_f\log h|_0\), \(a_{fg}=\partial_{fg}\log h|_0\), and \(\bar a_f=a_f-Qa_f\). Direct differentiation gives

\[
\frac{q_f}{q}=\bar a_f,\qquad
\frac{q_{fg}}q
 =a_{fg}-Qa_{fg}+\bar a_f\bar a_g
                 -\operatorname{Cov}_Q(a_f,a_g).
\tag{4.84; P}
\]

Each derivative has zero conditional integral. Let the nonnegative budget \(V=V(v,\mathrm{geometry})\) be fixed during the \(u\)-integration. If
\(\operatorname{osc}a_f\le b_fV\),
\(\operatorname{osc}a_g\le b_gV\), and
\(\operatorname{osc}a_{fg}\le b_{fg}V\), then

\[
|P_f\psi|\le b_fV\,P_0|\psi|,\qquad
|P_{fg}\psi|
 \le(b_{fg}V+2b_fb_gV^2)P_0|\psi|.
\tag{4.85; P}
\]

Indeed centering costs no more than the oscillation, and the covariance is bounded by the product of the two oscillations. This estimate never divides by the value of an individual characteristic function or by an uncontrolled rare-component mass.

The source-free LFR reference permits a direct application. LFR I (1.100), p.201, has the pure-Wilson reference
\(h_X=\delta_G\chi(\Lambda)\exp[-X\mathcal A]\), where
\(\mathcal A=A(\zeta,U_{k,Z}(V'V_\Lambda))\) and \(X=g_{B,k}^{-2}\).
Old \(E,R,B\)-terms belong to the other factor of that operation. The cutoff in (1.101) is
\(|(1/i)\log V'(b)|<M_0\epsilon_k\).
All its geometry, cutoffs and minimizing maps are held fixed in the following statement. The fixed factor \(\delta_G\chi\) is absorbed into \(d\mu_v\) before taking a logarithm; the reference density being differentiated is the strictly positive \(e^{-X\mathcal A}\).

On the admitted **current-scale regular reference support**,

\[
\operatorname{osc}_{V'}\mathcal A
 \le C\epsilon_k^2|Z|_k,\qquad
\left|\partial_t\log q_{X(t)}\right|
 \le C|X'(t)|\epsilon_k^2|Z|_k .
\tag{4.86; P in the checked current-scale reference domain}
\]

Here \(|Z|_k\) is current-scale volume. To verify the input, LFR I Proposition 1 and (1.78)–(1.80), pp.194–195, give the regular filling \(V_\Lambda\) and its fine minimizing field. On the fixed cutoff, multiplying the four perturbed coarse links bounds the plaquette of \(V'V_\Lambda\) by \(C\epsilon_k\), with construction constants included. For sufficiently small fixed coupling this is admitted by B102 Theorem 1, (8), p.279. Its regular space, defined in (2), p.278, gives
\(\|U(\partial p)-1\|\le C\eta^2\epsilon_k\) on the current-scale portion. For a real unitary plaquette,
\(1-N^{-1}\operatorname{ReTr}P=(2N)^{-1}\|P-I\|_{\rm HS}^2\).
Thus each plaquette contributes at most \(C\eta^4\epsilon_k^2\); the at most \(C\eta^{-4}|Z|_k\) plaquettes cancel this fine-scale factor. Since \(0\le\zeta\le1\), this bounds the energy and its oscillation. Differentiating the normalized reference gives
\(-X'(t)(\mathcal A-Q_t\mathcal A)\), proving (4.86).

A globally multiplying positive coefficient does not move the minimizing orbit. For deliberately affine reference coefficients in two formal source parameters, (4.84) also yields
\(|q_{fg}/q|\le2C^2|u_fu_g|\epsilon_k^4|Z|_k^2\).
This is an allowed reference-jet choice, not a claim that N2-F has a bounded second derivative.

On an unrolled history whose component volumes are charged to \(\mathcal V\), bounded first slopes give total first score \(O(\mathcal V)\) and total mixed raw derivative \(O(\mathcal V^2)\). The actual reserve (4.12) therefore bounds their total variation by \(C_f\varepsilon/s\) and \(C_{fg}\varepsilon/s^2\), respectively. This closes the fixed-geometry reference-coefficient contribution on the stated domain. If old layers remain inside the reference energy support, their own regularity and volume factors must be summed; the current-scale estimate is not silently substituted for them. Derivatives of moving selectors, integer geometry, cutoff surfaces and complex localizers remain separate.

Finally, for integral-preserving operators \(P_{j,t}\), the exact telescoping identity for the difference of \(\prod_jP_{j,t}\) and \(\prod_jP_{j,0}\), or its differentiated Duhamel formula, shows that the total integral of all kernel-motion terms vanishes after the complete later composition. This does **not** make their Wilson projection zero. On the two-point space \(u=0,1\), the normalized reference \(q_t(u)\propto e^{-(X+\lambda t)u}\) preserves mass while its logarithmic field coefficient changes by \(-\lambda\). Nonzero projected corrections must be bounded; they cannot be removed using mass conservation alone.

#### 4.15.3 Even entire common-family N2 data can have unbounded second response

**Proposition 4.15.1 (P).** All numerical clauses of N2-F are compatible with a single entire common-family remainder for which the second derivative of the \(K\)-step map grows faster than any prescribed sequence. First we give a simpler smooth construction, then its entire refinement.

**Proof.** Choose \(A>\max(4\gamma^{-2},2)\), set \(x_n=A+nb\), \(n\ge1\), and choose arbitrary \(M_n\ge1\). Let \(\chi\ge0\) be smooth, supported in \((-1,1)\), and equal to one near zero. For a sufficiently small fixed \(\epsilon>0\), put

\[
w_n=\min\{\epsilon/(M_nx_n^2),\,b/8,\,x_n/4\},\qquad
r(x)=\sum_{n\ge1}\frac{M_n}{2}(x-x_n)^2
                \chi((x-x_n)/w_n).
\tag{4.87; P}
\]

The supports are disjoint and locally finite. Differentiation and a smaller \(\epsilon\) give
\(0\le r(x)\le\min(C_r/x,b/4)\),
\(|r'(x)|\le\min(C_r/x^2,1/2)\), while
\(r(x_n)=r'(x_n)=0\), \(r''(x_n)=M_n\).
Set every \(r_k=r\). Then \(F=x-b+r(x)\) is strictly increasing, unbounded above, and its downward drift is between \(3b/4\) and \(b\). For every terminal \(Y=g_*^{-2}\ge4\gamma^{-2}\), the inverse iterates exist uniquely, depend smoothly on \(Y\), and have every coordinate at least \(Y\). They therefore give the admitted small couplings and continuous bare-coupling choice. Also
\(x_0=Y+bK-\sum_{j<K}r(x_j)=bK+O(\log(K+1))\), since
\(x_j\ge Y+(3b/4)(K-j)\). This checks all the specified numerical value, endpoint, continuity and derivative properties.

At terminal \(Y=A\), the exact orbit is \(x_j=A+b(K-j)\). Differentiating its finite composition twice gives

\[
(F^K)'(A+Kb)=1,\qquad
(F^K)''(A+Kb)=\sum_{n=1}^K M_n .
\tag{4.88; P}
\]

The second equality follows inductively from the chain rule, since each sampled first derivative equals one. For a scalar bare shift, it is multiplied by \(c^2\). Taking \(M_n\) arbitrarily large proves the claim. ∎

**Entire refinement (P).** Set \(\lambda=\pi/b\), \(c_n=M_n/(2\lambda^2)\), and
\(0<w_n\le\min\{b/8,1,\epsilon2^{-n}/[M_n(1+x_n)^2]\}\). Replace (4.87) by

\[
r(z)=\sin^2\!\bigl(\lambda(z-A)\bigr)
       \sum_{n\ge1}c_n
           \exp\!\left[-\left(\frac{z-x_n}{w_n}\right)^2\right].
\tag{4.88a; P}
\]

This series converges uniformly on each compact subset of \(\mathbb C\). Indeed for \(|\operatorname{Re}z|,|\operatorname{Im}z|\le R\) and sufficiently large \(n\),
\(\operatorname{Re}(z-x_n)^2\ge x_n^2/4\).
The chosen upper bound on \(w_n\) makes
\(c_n\exp[-x_n^2/(4w_n^2)]\) summable even for arbitrarily large \(M_n\). Thus \(r\) is entire and real nonnegative on the real axis.

Write \(t=(x-x_n)/w_n\). Periodicity gives
\(|\sin(\lambda(x-A))|\le\lambda|x-x_n|\).
For the \(n\)-th summand,
\(|r_n'(x)|\le C M_n w_n(|t|+|t|^3)e^{-t^2}\).
Using \(x^2\le2x_n^2+2w_n^2t^2\) yields
\(\sup_{x\ge\gamma^{-2}}x^2|r_n'(x)|\le C\epsilon2^{-n}\).
The same argument bounds \(x^2|r_n(x)|\) by \(C\epsilon2^{-n}w_n\).
After summation and a sufficiently small \(\epsilon\), all value, derivative and drift bounds used above hold.

At every lattice center, including \(A\),
\(r(x_n)=r'(x_n)=0\), whereas
\(r''(x_n)=\sum_m M_m
 \exp[-((x_n-x_m)/w_m)^2]\ge M_n\).
The exact orbit and first derivative in (4.88) are unchanged, and now
\((F^K)''(A+Kb)\ge\sum_{n=1}^K M_n\).
This proves the stronger proposition.

These are counterexamples to an inference from N2-F, not to Yang–Mills existence. They satisfy even the common-family reading. Neither its \(C^1\) estimate nor unquantified holomorphic extension supplies the desired two-scalar estimate. A quantitative uniform complex bound, or a bound on the actual marked second forcing, must do that work.

#### 4.15.4 Nonzero scheme corrections can be controlled along a coherent full-state curve

The useful first-order structure involves the whole effective action. Let \(C^1\) maps \(\Gamma_k=(p_k,q_k)\) on \(\mathbb R\times\mathcal B_k\), and \(C^1\) curves \(m_k\), obey

\[
\Gamma_k(x,m_k(x))
   =(F_k(x),m_{k+1}(F_k(x))).
\tag{4.89; C: coherent full-state curve to construct}
\]

This includes a specified Banach topology for all regular, boundary and history coordinates; N2-F supplies no such topology or curve. Linearize at the reference trajectory. For a perturbation \((u_k,z_k)\), let \(w_k=z_k-m'_k(x_k)u_k\). With errors \(e_k=(e_k^x,e_k^z)\), differentiating (4.89) once proves

\[
\begin{split}
u_{k+1}&=a_ku_k+\ell_kw_k+e_k^x,\\
w_{k+1}&=D_kw_k+\eta_k,\qquad
\eta_k=e_k^z-m'_{k+1}(x_{k+1})e_k^x,\\
a_k&=F_k'(x_k),\quad \ell_k=D_zp_k,\quad
D_k=D_zq_k-m'_{k+1}(x_{k+1})D_zp_k .
\end{split}
\tag{4.90; P from (4.89)}
\]

Indeed the tangent part of each differentiated coordinate equals its derivative along the curve; subtracting \(m'_{k+1}u_{k+1}\) cancels that part exactly. No second derivative is used.

Assume \(x_k\) decreases, all partial products of \(a_k\) and their inverses are at most \(C_A\), \(\|\ell_k\|\le C_\ell(1+x_k)^p\), \(p\ge0\), and
\(\|D_{k-1}\cdots D_j\|\le C_Dq^{k-j}\), \(0<q<1\), \(C_D\ge1\).
Suppose \(w_0=0\) and
\(|e_k^x|+\|\eta_k\|\le\varepsilon_k(|u_k|+\|w_k\|)\).
Set
\(\mathcal E=\sum_{k<K}(1+x_k)^p\varepsilon_k\),
\(B=1+C_\ell C_D/(1-q)\), and \(C_0=C_D+C_AB\).
If \(\mathcal E\le(2C_0)^{-1}\), then

\[
\begin{split}
\sup_k(|u_k|+\|w_k\|)&\le2C_A|u_0|,\\
\sup_k\left|u_k-\Bigl(\prod_{j<k}a_j\Bigr)u_0\right|
 &\le2C_A^2B\,\mathcal E\,|u_0|,\\
\sup_k\|w_k\|&\le2C_AC_D\,\mathcal E\,|u_0|.
\end{split}
\tag{4.91; P under the displayed quantitative hypotheses}
\]

For a direct proof, variation of constants bounds
\(\|w_k\|\le C_D\sum_{j<k}q^{k-j-1}\varepsilon_j
(|u_j|+\|w_j\|)\).
If \(M_n=\max_{k\le n}|u_k|+\max_{k\le n}\|w_k\|\), its maximum is at most \(C_D\mathcal E M_n\). In the scalar variation formula, the contribution \(\sum_\ell\|\ell_\ell w_\ell\|\) is at most
\(C_\ell C_D M_n\sum_j\varepsilon_j(1+x_j)^p/(1-q)\),
because \(x_\ell\le x_j\) when \(\ell>j\). Thus
\(M_n\le C_A|u_0|+C_0\mathcal E M_n\).
Absorption proves the first bound, and substitution proves the others.

Fixed shrinking-radius losses do not prevent such summability on the N2 high-range trajectory, which has \(x_k-x_{k+1}\ge b_->0\). If
\(\rho_k\asymp x_k^{-1/2}(\log x_k)^q\), then

\[
\sum_{k<K}g_k^\kappa\rho_k^{-m}
 \le C\sum_{k<K}x_k^{-(\kappa-m)/2}(\log x_k)^{-qm}<\infty
 \quad\text{uniformly in }K\quad\text{if }\kappa>m+2.
\tag{4.92; P}
\]

The bound tends to zero with a sufficiently high terminal coordinate. Extra fixed polynomial losses are paid by a larger \(\kappa\). Thus a quantitatively small local scheme correction need not have zero Wilson projection. The missing YM statements are admission of all such corrections, construction of (4.89), and contraction in the same complete norm. The proved stability theorem specifies what suffices; it does not assume these statements follow from source-free pressure stability.

## 4.16 Extraction and localization on the full regular complex image

The physical-background proof of §4.7 is not by itself an analytic norm estimate. This subsection supplies the missing operator estimate for **already admitted regular marked activities**, using the reconstructed complex images of B109 and the joint localization domains of B116. It does not claim that every exceptional large-field image has the same regularity.

#### 4.16.1 The analytic operator theorem

First split the full determining-lattice cochain \(\mathbf B\) into its inner and outer parts, \(\mathbf B_{\rm in}=\chi\mathbf B\) and \(\mathbf B_{\rm out}=(1-\chi)\mathbf B\), as in B109 (4.1), p.281. Terms with an outer factor are estimated as multilinear operators by (4.5), p.282, before any endpoint-coordinate sum. Only the all-core terms are then written on the old unit lattice \(T_1^{(j)}\); this is exactly the order stated in the paragraph immediately following (4.5). In (4.93), \(B\) and \(K_{n,X}\) denote the retained core field and its core-endpoint kernels.

For a small carrier choose a contractible lifted reconstruction chart containing its entire carrier \(X\), with
\(\operatorname{dist}_{\rm old}(X,\operatorname{supp}(1-\chi))\ge c/\theta\) and
\(\operatorname{dist}_{\rm old}(X,\partial\mathcal C)\ge c/\theta\), and nested cutoffs leaving the same buffer for the Ward gauges. Take \(\chi\) with first and second differences bounded by \(C\theta\) and \(C\theta^2\). Declare the small-carrier class by \(1+D\le c_0/\theta\), with \(c_0\) smaller than the fixed chart buffer constants. Chart radius \(c/\theta\) alone does not imply the required carrier-to-boundary distance. The declared large carriers and winding carriers are handled by exponential carrier tails. If a padded admitted chart is unavailable for another geometric reason, its availability remains a separate input.

Write the full reconstructed functional as \(G_X(U_j(\mathbf B),J_j(\mathbf B))\). Its core Taylor coefficients inherit Ward identities for gauges supported inside \(\chi=1\). The activity takes values in the Banach space of multilinear source functionals. The complex tube and endpoint-moment hypotheses below are in that Banach norm. In addition to the core estimates in (4.93), retain the full outer envelope \(\|\mathbf B_{\rm out}\|_{\rm det}\le CM_{\rm out}\). For the stated bound (4.94) assume \(M_{\rm out}\le CM\); otherwise retain the explicit outer error below. Let \(0<r\le1\) and \(0<M\le M_0<1\), with \(M_0\) sufficiently small for the exact plaquette logarithms.

The zero base sets **all** determining data, including the outer annuli, to the identity. For these data the identity is a feasible zero-action minimizer; B102 Theorem 1 and its axial-gauge uniqueness therefore give \(U_j(\square_0,1)=1\), with zero current. Constant color conjugation fixes this base and acts on every tangent direction. Its invariant linear functional vanishes because \(\mathfrak{sl}_N\) is spanned by commutators. Thus \(D\widetilde\Phi_X(0)=0\) exactly, also in the source Banach norm by duality. This is the cancellation in B109 (4.13)–(4.14), p.284. A different expansion holding nonzero outer data fixed would need a boundary-response term and is not used here.

Here are the precise norm hypotheses. The full composite \(\widetilde\Phi_X\) is bounded by \(a_X\) on complex tubes in the full determining norm about \(\tau\mathbf B\), \(0\le\tau\le1\). Choose \(r\) as a common lower analytic margin for the determining tube and the image activity domain, after their fixed reconstruction constants, and reserve a fixed smaller common tube for the Cauchy derivatives. Its degree-two through degree-four derivative kernels at zero have localized endpoint moments. Uniformly on the complete complex reconstruction/localization image, assume

\[
\begin{gathered}
\sum_{b_1,\ldots,b_n}\|K_{n,X}(b_1,\ldots,b_n)\|
       \prod_{\ell=1}^n(1+d(b_\ell,z))^{12}
 \le C_n a_Xr^{-n}P_n(D),\quad 2\le n\le4,\\
\|B\|_\infty\le M\theta,\qquad
\|\partial B\|_\infty\le M\theta^2,\qquad
\|\partial^2B\|_\infty\le M\theta^{2+\alpha}.
\end{gathered}
\tag{4.93; C: input norms; checked reconstruction scope below}
\]

Here \(D\) is the carrier diameter or tree size and \(P_n\) a fixed polynomial. The finite color-index sum is included. The corresponding exponential endpoint tails are included in the admitted-map hypotheses. More precisely, with \(d_*=\operatorname{dist}_{\rm old}(X,\operatorname{supp}(1-\chi))\), the localized first response on the common tube obeys

\[
\|D\widetilde\Phi_X(C)[h_{\rm out}]\|_{\rm src}
 \le C a_X r^{-1}P(D)e^{-c d_*}
              \|h_{\rm out}\|_{\rm det}.
\tag{4.93r; C: admitted map response and common activity/determining margin}
\]

For the regular map, the localized minimizing-field response in B102 Proposition 9, including (190), and the activity-domain Cauchy estimate give this bound. Taking a common lower margin is essential: with separate margins the initial factor would be \(r_{\rm activity}^{-1}\), and four further derivatives would cost \(r_{\rm det}^{-4}\). The single \(r^{-5}\) notation is used only after the specified choice of common margin. These assumptions describe the operator theorem; the incoming marked amplitudes \(a_X\) still have to be established by the full induction.

The outer terms have the distinct operator estimate
\[
\left\|D^n\widetilde\Phi_X(0)
  [\mathbf B_{\rm in}^{\otimes m},
   \mathbf B_{\rm out}^{\otimes(n-m)}]\right\|_{\rm src}
\le C_n a_Xr^{-n}P_n(D)e^{-c/\theta}
       (M\theta)^m M_{\rm out}^{\,n-m},
\quad 2\le n\le4,\quad m<n.
\tag{4.93a; P from the admitted map and input activity norm}
\]
The same estimate applies to the fifth Taylor remainder along its admitted complex tube. One proves it from the localized minimizing-map response in the paragraph before B109 (4.5), followed by the activity Cauchy bound. For the fifth remainder, take one outer-supported variation and apply Cauchy in the other four directions on a fixed smaller common tube; the uniform separation factor persists. B109 p.280 explicitly requires this inside/outside treatment after (3.54), because its \(O(\theta)\) bound for \(B\) is asserted only in the inner box.

No outer direction is expanded into fine-coordinate deltas. Thus (4.93a) carries no fine-mesh counting factor. The total discarded outer contribution is bounded by
\[
Ca_XP(D)e^{-c'/\theta}
 \sum_{n=2}^{5}\sum_{m=0}^{n-1}
 r^{-n}(M\theta)^mM_{\rm out}^{\,n-m}.
\tag{4.93b; P}
\]
For \(M_{\rm out}\le CM\), this is bounded by the right side of (4.94), since
\(\theta^m e^{-c'/\theta}\le C_{\alpha,m}\theta^{4+\alpha}\) for the finitely many \(0\le m\le4\). If that outer envelope is not known, (4.93b) remains an additional term; it is not dropped. The cochain-operator and core-kernel estimates are uniform in the source arguments, so the source-operator supremum is retained without a support-cardinality loss.

**The actual regular-map outer envelope (P, with the stated fixed stencil collar).** The outer bound can be obtained from the full weighted minimizing-field estimate, rather than guessed from the core. Write \(M_b\) for Balaban's fixed geometric block size. B109 (3.26), p.275, gives
\(\|V-1\|\le C M_b\alpha_0\) on the full determining set after its generalized axial gauge. Take identity reference \(V_0=1\) in B102 Proposition 9, p.309. Its explicit retention of (19), p.281, gives the complex Landau field on every nested domain:

\[
\sup_{\Omega_q}|H|\le C\varepsilon_{\rm det}/h_q,
\qquad
\varepsilon_{\rm det}=C M_b\alpha_0.
\tag{4.93c; L: B102 (19), (173), Proposition 9, in physical units}
\]

Choose the fixed domain collars with \(R M_1>C_{\rm av}L\). The \(q\)-th averaging stencil has radius at most \(C_{\rm av}h_q\), by B98 Proposition 4, p.38, whereas the preceding domain supplies a collar \(R M_1h_{q-1}\), by B102 (1), p.277. Hence the stencil is contained in \(\Omega_{q-1}\); \(q=0\) needs no averaging. Its minimizing field satisfies
\(h_q\sup|H|\le C\varepsilon_{\rm det}h_q/h_{q-1}=CL\varepsilon_{\rm det}\).
The auxiliary field \(A\) in B109 (3.31), p.276, has size at most \(\alpha_2\) in current units throughout the chart, and every determining bond is at most current size. The small complex matrix-product logarithm therefore has the same scaled bound
\(C(\alpha_2+\varepsilon_{\rm det})\).

Rescale each averaging stencil to unit size. B109 immediately after (0.12), p.254, carries the B98 estimates to its Euclidean-symmetric averaging convention. B98 (131) and Proposition 4, p.38, with identity reference field, bound its iterated averaged logarithm by that same quantity, uniformly in the number of fine links and averaging steps. This proves

\[
\|\mathbf B\|_{\rm det}+\|\mathbf B_{\rm out}\|_{\rm det}
 \le C(\alpha_2+M_b\alpha_0),\qquad
\|B_{\rm in}\|_\infty
 \le C(\alpha_2+M_b\alpha_0)\theta .
\tag{4.93d; P}
\]

For the second inequality the stronger unweighted interior bound B109 (3.27)–(3.32), pp.275–277, holds on the complete core averaging stencil; its old bond has current physical length \(\theta\). This supplies the additional \(\theta\), which is not asserted for the outer field. There is no sum over layers or individual fine endpoints in the argument.

Set \(M=C_0(\alpha_2+M_b\alpha_0)\), with \(C_0\) large enough and the fixed analytic domains small enough. Then \(M_{\rm out}\le CM\) holds on these regular maps, and (4.93b) is absorbed into (4.94). This verifies the map envelope on the published small analytic domains with the stated collar choice. It does not enlarge them or establish marked activity admission there. Any further assignment of these domains to prescribed running radii has to obey the other inductive requirements as well.

**Buffered charts on a cofinal torus family (P).** In the fundamental local case, B109 (3.5), p.271, places the entire carrier inside the second enlarged current cube. The variational chart is the fifth enlargement, constructed on p.273. The cutoff in (3.21), p.274, is one on the third enlargement and zero outside the fourth; the stated carrier-to-transition distance is \(M_b/\theta\). A Ward cutoff can turn off strictly between the second and third enlargements, inside \(\chi=1\), leaving a further fixed buffer to the fifth-enlargement boundary. Its old-coordinate differences are bounded by \(C\theta\) and \(C\theta^2\).

These charts fit uniformly along a cofinal family with \(T\) a multiple of \(2M_b\ell_0\) and \(T\ge C_{\rm geom}\ell_0\). Indeed the current cover cube has side \(2M_bh_k\); five enlargements add fixed layers of width \(M_bh_k\), so a fixed enclosing cube of side at most \(16M_bh_k\) suffices. Taking \(C_{\rm geom}\ge64M_b\), enlarged for any further fixed collars, makes that cube injectively lift at every \(h_k\le\ell_0\). The grids align because \(\ell_0/h_k\) is an integral power of \(L\). This proves the needed chart geometry on that cofinal family. It does not cover every compatible short torus.

Outside the fundamental class, B109 (3.5)–(3.9), p.271, gives a distant-or-large split. A carrier meeting the fluctuation neighborhood and reaching beyond the second enlargement has \(D\ge c/\theta\). A disjoint distant carrier instead gains \(e^{-c/\theta}\) from the **differentiated** minimizing map, with its actual common-radius Cauchy factor. Distance alone does not make an undifferentiated activity small. These two discarded classes are estimated by their appropriate exponential tails before summing the regular localized step.

**Proposition 4.16.1 (P).** On a padded small-carrier chart with the preceding admitted-map hypotheses, and with \(M_{\rm out}\le CM\), there is a linear extraction
\(\mathcal L_X\Phi=\Phi(0)+\sum_{\alpha,\beta}c_X^{\alpha\beta}
\operatorname{Tr}(\mathcal F_\alpha\mathcal F_\beta)\),
where \(\alpha,\beta\) are independent oriented two-form indices,
\(\mathcal F_{\mu\nu}=i^{-1}\log P_{\mu\nu}(B;z)\), and \(c_X\) is symmetric, such that

\[
|c_X|\le Ca_Xr^{-2}P(D),\qquad
\|\Phi_X-\mathcal L_X\Phi_X\|
 \le C_\alpha a_XP(D)\theta^{4+\alpha}
                   \sum_{n=2}^5(M/r)^n .
\tag{4.94; P on the full specified complex image}
\]

No translation or hypercubic invariance of the individual marked carrier is required.

**Proof.** First split each field-Taylor direction into inner and outer parts. Equations (4.93a)–(4.93b) control all terms containing an outer part. Cauchy's formula bounds the retained all-core fifth-order remainder by \(Ca_Xr^{-5}(M\theta)^5\). Only the retained degree-two through degree-four coefficients are now expressed as unit-lattice kernels and summed using (4.93). Their linear differential vanishes by constant color conjugation.

Write \(b_\mu=B_\mu(z)\), \(M_{\mu\nu}=(\partial_\nu B_\mu)(z)\), and
\(B_\mu(x)=b_\mu+M_{\mu\nu}(x_\nu-z_\nu)+E_\mu(x)\).
Discrete telescoping and (4.93) give
\(|E_\mu(x)|\le CM\theta^{2+\alpha}(1+|x-z|)^2\).
The quadratic Hessian annihilates the constant cochain, since that cochain is the gradient of the affine site polynomial. Thus replacing \(B\) by its affine jet costs \(Ca_Xr^{-2}M^2\theta^{4+\alpha}P(D)\) at quadratic order, rather than an inadequate third-order scale power. At cubic and quartic orders, the endpoint-moment bounds give errors bounded respectively by
\(Ca_Xr^{-3}M^3\theta^{4+\alpha}P(D)\) and
\(Ca_Xr^{-4}M^4\theta^{5+\alpha}P(D)\).

The remaining weighted-degree-at-most-four expression has a short exact gauge calculation. Give \(b\) weight one and the spatial derivative matrix weight two. In the formal field
\(B_\mu(t,x)=t b_\mu+t^2M_{\mu\nu}(x_\nu-z_\nu)\),
the gauge \(u_t(x)=\exp[it(x-z)\cdot b]\) removes the constant term. Its order-two coefficient is
\(M'_{\mu\nu}=M_{\mu\nu}+\frac i2[b_\nu,b_\mu]\).
Let \(S=(M'+M'^{\mathsf T})/2\). The site polynomial

\[
\phi(x)=\tfrac12\sum_{\mu,\nu}S_{\mu\nu}r_\mu r_\nu
              -\tfrac12\sum_\mu S_{\mu\mu}r_\mu,\qquad r=x-z,
\quad
\partial_\mu\phi=\sum_\nu S_{\mu\nu}r_\nu
\tag{4.95; P: exact forward-difference identity}
\]

gives a second gauge \(e^{it^2\phi}\) removing the symmetric first jet. The transformed field starts as
\(t^2A_\mu^F=-\frac12t^2\sum_\nu F_{\mu\nu}r_\nu\), with
\(F_{\mu\nu}=M_{\nu\mu}-M_{\mu\nu}+i[b_\mu,b_\nu]\).
Since the linear differential is zero, its entire contribution through weighted degree four is
\(\frac12D^2\Phi_X(0)[A^F,A^F]\).
Invariant bilinear forms on the simple color algebra are multiples of the trace pairing, so this is precisely a symmetric curvature-pair tensor. The second endpoint moment bounds its coefficient by \(Ca_Xr^{-2}P(D)\). Terms of higher weighted degree have at least five powers of \(\theta\), and are bounded with the respective \(r^{-n}M^n\) factors, \(2\le n\le4\). Replacing the leading curvature \(F\) by the exact plaquette logarithm costs another \(Ca_Xr^{-2}M^2\theta^{4+\alpha}P(D)\), by the same finite-product expansion and (4.93). The fifth Taylor remainder has \(\theta^5\le\theta^{4+\alpha}\). This proves (4.94).

For the core Ward calculation choose the polynomial-gauge cutoff equal to one on a neighborhood of the entire carrier \(X\), with its transition at distance at least \(c/\theta\) from \(X\), still inside the old-unit core \(\chi=1\). Exact polynomial Ward identities hold for the infinite/free-boundary kernel; on the finite buffered chart the cutoff identities differ from them only in terms with a distant core endpoint. Their exponential endpoint bound through degree four, the corresponding \(r^{-n}\), and the fixed polynomial coordinate moments give
\(Ca_XP(D)e^{-c'/\theta}\sum_{n=2}^{4}r^{-n}M^n\theta^n P(\theta^{-1})\), which is absorbed by (4.94). This also justifies the annihilation of the affine constant cochain used above, up to that explicitly controlled finite-chart error.

For carriers in the declared large class, or winding carriers of comparable size,
\(e^{-\kappa D}1_{\{1+D\ge c_0/\theta\}}\le C_q\theta^q e^{-\kappa'D}\).
Set their field projection to zero. Use their actual vacuum-subtracted bound \(2a_X\), or \(Ca_X(M_{\rm tot}/r)^2\) when a full determining-field envelope \(M_{\rm tot}\) and the common tube are available. The carrier tail supplies the whole missing scale power; no \(O(M\theta)\) bound is assumed for these unsplit large-carrier fields. No holonomy is gauged away.

The displayed small-carrier bound (4.94) includes the outer term only when its stated envelope holds. For an unsplit large carrier the \(2a_X\) alternative carries no small \(M/r\) prefactor. It is kept as a separate carrier-tail contribution unless the full-field envelope or a numerical lower radius-ratio comparison supplies that prefactor. All operations are bounded in the source Banach norm. ∎

The hypothesis that the field lies on a regular reconstructed image is necessary. For example take commuting links in a Cartan subgroup, with curvature \(\theta^2H\) on one local plaquette and zero at a different anchor. A small local gauge-invariant plaquette activity is \(O(\theta^4)\) on this configuration, while the anchor curvature subtraction vanishes. Its finite differences are not of order \(\theta^{2+\alpha}\). Thus smallness and gauge invariance alone do not yield (4.94) on an arbitrary ambient link-field domain.

#### 4.16.2 Exact conversion to the Wilson and clover representatives

The tensor representative in (4.94) can be changed on the same complex field without a new radius loss. Let \(A_{\mu\nu}=i^{-1}\log P_{\mu\nu}(B;z)\). Use holomorphic extensions of the real observables: \(s^{\rm hol}(P)=N-\frac12\operatorname{Tr}(P+P^{-1})\),
\(\widehat F^{\rm hol}=\frac18\mathsf P_{\rm tr}\sum_{\rm clover}(P-P^{-1})\), and \(Q^{\rm hol}_{\alpha\beta}=\operatorname{Tr}(\widehat F^{\rm hol}_\alpha\widehat F^{\rm hol}_\beta)\). On unitary links these agree with P2. The trace projection is
\(\mathsf P_{\rm tr}A=A-N^{-1}(\operatorname{Tr}A)I\); the anti-Hermitian condition is automatic on the real slice. One must not apply a literal complex conjugation to define the holomorphic extension.

On the domain (4.93),

\[
\begin{split}
\widehat F^{\rm hol}_\alpha&=iA_\alpha+O(M\theta^{2+\alpha}),\\
Q^{\rm hol}_{\alpha\beta}
 &=-\operatorname{Tr}(A_\alpha A_\beta)
                    +O(M^2\theta^{4+\alpha}),\\
s^{\rm hol}(e^{iA_\alpha})
 &=\tfrac12\operatorname{Tr}A_\alpha^2
                    +O(M^4\theta^8).
\end{split}
\tag{4.96; P, uniformly on the same complex image}
\]

To prove the first two bounds, write each consistently oriented clover plaquette based at \(z\) as a conjugate of a neighboring forward plaquette by a path of at most two links. The finite-product/Baker–Campbell–Hausdorff expansion gives
\(A_{\mu\nu}(y)=\partial_\mu B_\nu(y)-\partial_\nu B_\mu(y)
+i[B_\mu(y),B_\nu(y)]+O((M^2+M^3)\theta^3)\).
Changing \(y\) by at most two lattice steps costs
\(CM\theta^{2+\alpha}+C(M^2+M^3)\theta^3\).
Conjugation by the connecting path costs \(CM^2\theta^3\).
Since \(M,\theta\le1\) and \(\alpha<1\), all these errors are at most \(CM\theta^{2+\alpha}\). Each logarithm is traceless in the small \(SL(N,\mathbb C)\) chart. Expanding \(P-P^{-1}=2i\sin A\) in all four plaquettes gives the factor \(iA_\alpha\) exactly. Multiplication and the bound \(\|A_\alpha\|\le CM\theta^2\) prove the clover formula. The scalar formula is the exact cosine Taylor expansion; odd powers cancel.

Consequently the tensor term \(\sum c_X^{\alpha\beta}\operatorname{Tr}A_\alpha A_\beta\) may be replaced by \(-\sum c_X^{\alpha\beta}Q^{\rm hol}_{\alpha\beta}\), at an additional error at most
\(Ca_XP(D)(M/r)^2\theta^{4+\alpha}\).
For a diagonal scalar term, the replacement is
\(c\operatorname{Tr}A_\alpha^2\mapsto2c\,s^{\rm hol}(P_\alpha)
=2Nc\,a_{\rm Balaban}^{\rm hol}(P_\alpha)\).
These sums use \(\mu<\nu\) and \(\rho<\sigma\), with both ordered independent pairs allowed. If the P2 tensor summation is written over all ordered \(\mu,\nu,\rho,\sigma\), the corresponding displayed source coefficient is divided by four. This is a basis conversion, not an assertion of a bounded running tensor mixing matrix.

Thus same-image Wilson/clover conversion is proved. Identifying the old reconstructed curvature with the prescribed current-step variable, and identifying its complete scalar coefficient with N2's running coordinate, remain separate cross-scale tasks. B119 (3.65)–(3.67), p.283, performs the source-free scalar matching; it does not by itself give the complete sourced matching.

#### 4.16.3 Localization retains the analytic gain

Suppose the complete reconstruction has a simultaneous complex interpolation disk \(|t|<T\) and localization polydisc \(|s_e|<R\), \(R>1\), on which all the hypotheses of Proposition 4.16.1 hold uniformly: (4.93), (4.93r), the full common tubes and activity margin, the outer envelope and the chart buffers. Write
\(\mathscr R_X(t,s)=\Phi_X(B(t,s))-(\mathcal L_X\Phi_X)(B(t,s))\),
using either representative of §4.16.2. For a set \(F\) of distinct localization variables, joint Cauchy estimates at \(t=0\), \(s_e\in[0,1]\), give

\[
\left\|\partial_t\prod_{e\in F}\partial_{s_e}\mathscr R_X\right\|
 \le
 \frac{C_\alpha a_XP(D)}{T}\theta^{4+\alpha}
 \sum_{n=2}^5(M/r)^n
 \left(\frac{R}{(R-1)^2}\right)^{|F|}.
\tag{4.97; P}
\]

Indeed use the bound (4.94) on the full product contour. A single localization derivative contributes the contour-length/denominator factor \(R/(R-1)^2\); the interpolation derivative contributes \(T^{-1}\). Distinct variables introduce no \(|F|!\). Real interpolation integrations have measure one. Source anchors are retained, because extraction and localization act linearly on the field activity, not by deleting its source restrictions.

These product domains are present in the published regular construction. B109 (3.24)–(3.32), pp.275–277, reconstructs from independent complex \(U,J\); Lemma 4, (3.53), p.280, admits complex perturbations into the old activity domain. B109 (4.1)–(4.5), pp.281–282, first separates the determining field into inner and outer directions. The mixed/fine outer directions are controlled by (4.5) as cochain multilinear operators, with their actual inverse-radius factors. The paragraph following (4.5) then identifies the retained all-core field with a function on \(T_1^{(j)}\). Only at this point does the finite chain-rule estimate give unit-lattice endpoint kernels whose exponential decay yields the polynomial moments in (4.93). The tree estimate discussed on p.286 supplies a sharper version. The same chain-rule/Cauchy argument is valid in the source Banach norm for an admitted marked activity. Equations (4.16)–(4.18), p.285, supply the regularity powers on the retained core. None of these statements counts fine outer endpoints as old unit sites. The common-tube outer-response estimate, the actual outer envelope and the buffered-chart condition must accompany this use. The joint Cauchy operation also applies to the explicit error (4.93b), whether or not it can already be absorbed into (4.94).

B116 (1.11), p.5, admits all \(|s_e|\le e^{\kappa_1}\) simultaneously with a norm bound independent of their number. Its fixed-point estimates (1.12)–(1.21), pp.5–7, retain those regularity norms. Its (1.22), p.7, gives
\(T^{-1}\le8B_0C_1e^{16\kappa_1}\alpha_2^{-1}\epsilon_1\);
(1.23) is the joint Cauchy formula and (1.25) retains the final independent-variable domain. With \(R=e^{\kappa_1}\) sufficiently large, the last factor of (4.97) supplies the localization-cube decay. The references in later papers to “(6.9) [I]” use combined/preprint numbering; the published localization formulas are B116 §1, not a nonexistent §6 of B109.

This proves the regular operator extension to admitted marked inputs. LFR II (1.65), p.375, supplies an inclusion of its localized image into mixed-scale activity domains. Domain inclusion alone does not supply every layerwise regularity and endpoint estimate in (4.93); that exceptional-sector verification remains open.

#### 4.16.4 Radius-normalized regular memory and variable sources

Keep the size of the current field in every old Cauchy ratio. If
\(r_j\asymp\rho_j\), \(M_k\le C\rho_k\), and the admitted interpolation has
\(T_{j,k}^{-1}\le C\epsilon_k/\rho_j\), put
\(\delta_k=\epsilon_k/\rho_k\), \(\theta=L^{j-k}\).
Equation (4.97), followed by the \(C\theta^{-4}\) old-anchor count and the reserved carrier/localizer decay, gives the rooted regular remainder bound

\[
C\delta_k\sum_{j\le k}L^{-\alpha(k-j)}
        \left[\sum_{n=3}^{6}(\rho_k/\rho_j)^n\right]a_j .
\tag{4.98; P under the specified radius and regular-image hypotheses}
\]

The counting is local: fix the current root block, sum old carriers through an old anchor using the spare exponential, sum its old anchors, then sum the connected current localizer carriers. No sum over the entire torus volume is needed.

If \(\rho_j\asymp x_j^{-1/2}(\log x_j)^q\) with common fixed \(q>0\), and
\(b_-\le x_j-x_{j+1}\le b_+\), then for fixed \(n\) and \(0<\alpha'<\alpha\),

\[
(\rho_k/\rho_j)^n
 \le C_n\left(1+\frac{b_+(k-j)}{x_k}\right)^{n/2},
\quad
L^{-\alpha(k-j)}(\rho_k/\rho_j)^n
 \le C_{\alpha,\alpha',n}L^{-\alpha'(k-j)}.
\tag{4.99; P}
\]

The logarithmic ratio is at most one; the remaining polynomial is absorbed by the spare exponential. There is also a positive lower bound \(\rho_k/\rho_j\ge c_*>0\) for \(x_j\ge x_k\ge X_*>1\): \(f_q(x)=x^{-1/2}(\log x)^q\) increases up to \(e^{2q}\) and decreases thereafter, so
\(f_q(x_k)/f_q(x_j)\ge\min\{1,f_q(X_*)/f_q(e^{2q})\}\), with the decreasing case used if \(X_*\ge e^{2q}\). For \(q=0\) it is simply decreasing. The fixed comparison constants in the radii preserve a positive lower bound.

When \(M_k\) is the **chosen domain envelope** comparable to \(\rho_k\), this proves \(M_k/r_j\ge c>0\). The crude \(2a_X\) large-carrier estimate can therefore take the same radius-weighted form after its exponential tail supplies \(\theta^{4+\alpha}\). An old-radius outer envelope is also at most \(CM_k\). Neither claim holds for an arbitrarily small measured field amplitude at fixed radius. These comparisons justify inclusion of the large and distant classes in (4.98), under its matched-domain hypotheses. Thus, for the regular linear recurrence
\(a_{k+1}\le f_{k+1}+C\delta\sum_{j\le k}q_*^{k-j}a_j\),
\(q_*<1\), \(C\delta<1-q_*\), taking finite maxima and absorbing gives
\(\sup a_k\le\max(a_0,\sup f_k)/(1-C\delta/(1-q_*))\).
The same proof works after dividing by a nondecreasing forcing weight. This closes that regular irrelevant linear system. Establishing its forcing and smallness for the same fixed full-construction parameter ledger remains necessary; the common-radius choice is not a silent change of N2-F's scheme.

There is also a full-complex-norm source-freezing estimate, with an essential source-norm qualification. On the generation-\(j\) collar set
\(\|f\|_{C^5,h_j}=\sum_{|\alpha|\le5}h_j^{|\alpha|}\sup|\partial^\alpha f|\).
Assume the \(m\)-linear activity has operator norm \(a_je^{-\kappa D}\) for these **generation-scaled** source norms, uniformly on its field domain. This admission is explicit; it is not inferred from an operator bound using the fixed physical \(C^5,\ell_0\) norm.

Define
\(D_{5,\ell_0}(f)=\sum_{1\le|\alpha|\le5}\ell_0^{|\alpha|}\sup|\partial^\alpha f|\).
For a collar of radius \(Ch_j(1+D)\) about \(z\), the mean value theorem for the zero-order term, and \(h_j\le\ell_0\) for every derivative term, give
\(\|f-f(z)\|_{C^5,h_j}\le C(1+D)(h_j/\ell_0)D_{5,\ell_0}(f)\).
Let \(\Delta_{\rm src}G=G[f_1,\ldots,f_m]-\prod_i f_i(z)G[1,\ldots,1]\).
Telescoping in the \(m\) slots bounds its old activity norm by this difference norm in one slot and the norms of the other slots. The single factor \(1+D\) is paid by the reserved carrier decay; no factor is raised to the number of marks.

Apply (4.94), retaining both the tensor projection and the remainder but subtracting the vacuum value. Since the exact curvature is \(O(M_k\theta^2)\), this proves

\[
\begin{split}
\|\Delta_{\rm src}G(B)-\Delta_{\rm src}G(0)\|
 \le{}& C a_je^{-\kappa'D}\frac{h_j}{\ell_0}\theta^4
       \sum_{n=2}^5(M_k/r_j)^n\\
 &{}\times\sum_i D_{5,\ell_0}(f_i)
                 \prod_{\ell\ne i}\|f_\ell\|_{C^5,\ell_0}.
\end{split}
\tag{4.100; P under the stated generation-scaled source norm}
\]

For an activity bounded in the multilinear **supremum** source norm, the sharper version replaces
\((h_j/\ell_0)D_{5,\ell_0}(f_i)\) by
\(h_j\|\nabla f_i\|_\infty\) and the other factors by \(\|f_\ell\|_\infty\). A general fixed-\(C^5\) operator bound alone gives neither freezing assertion, because its derivative seminorms do not become small on a short collar. Source contact distributions may require the scaled-derivative formulation.

The same joint Cauchy argument preserves the proved gain under localization. Old-anchor counting removes \(\theta^4\), and
\(h_j/\ell_0=(h_k/\ell_0)\theta\le\theta\).
Fixed radius powers are absorbed as in (4.99), giving a summable old-age factor. With the displayed sum over source labels retained, the operator constant is independent of their number; the admitted multilinear norm carries their order dependence. The vacuum source contact still requires §4.8's Taylor subtraction. The constant-source marginal, full all-order input bounds and exceptional large-field sectors are not supplied by this theorem.

## 4.17 Quantitative complex coupling control and a complete frozen regular block

This subsection gives a positive alternative to the counterexample in §4.15.3. It proves that a fixed complex coupling tube with only a polynomial bound, combined with N2-F's real first-derivative estimate, suffices for all constant-scalar coupling jets. That quantitative tube for the actual coherent RG curve remains to be proved. We then establish a related tube and the complete second derivative for a frozen positive regular block, including its affine reference motion. These two families are not identified without proof.

#### 4.17.1 A polynomial tube improves the complex derivative

Let a family \(r_j\) be holomorphic on the union of \(D(x,4R)\), \(x\ge x_*>1\), with \(R>0\) fixed. Suppose, uniformly in \(j\) and ultraviolet depth,

\[
|r_j(z)|\le C_0(1+x)^A\quad(z\in D(x,4R)),\qquad
|r'_j(x)|\le C_rx^{-2},\qquad A\ge0 .
\tag{4.101; C: quantitative tube for the actual family to establish}
\]

**Proposition 4.17.1 (P).** For each \(1<p<2\) there are fixed \(\eta>0,X_*,C_p\), independent of \(j\), such that
\(|r'_j(z)|\le C_p(\operatorname{Re}z)^{-p}\) for
\(\operatorname{Re}z\ge X_*\), \(|\operatorname{Im}z|\le\eta\).
One may take \(\eta=R(2-p)/[3(A+2)]\), after increasing the threshold.

**Proof.** Fix a large \(x\). On the rectangle
\(x-R<t<x+R,\ 0<y<R\), Cauchy's estimate on disks of radius \(R\) bounds
\(|r'_j|\) by \(M_x=C_Mx^A\), while its bottom edge has
\(|r'_j|\le m_x=4C_rx^{-2}\). Choose \(C_M\) with \(M_x\ge m_x\). If \(C_r=0\), the identity theorem finishes the proof; otherwise use logarithms.

The harmonic measure \(\omega\) of the three non-bottom sides is bounded by the positive harmonic barrier

\[
B(t,y)=\frac yR+
 \frac R4\,\frac{y}{(t-x+R)^2+y^2}
 +\frac R4\,\frac{y}{(t-x-R)^2+y^2}.
\tag{4.102; P}
\]

It is zero on the bottom except at its endpoints and at least one on the top. On either vertical side, \(y/R+R/(4y)\ge1\). The maximum principle gives \(\omega\le B\); the exceptional endpoints have harmonic measure zero. In the middle half, \(B\le3y/R\). Apply the two-constants principle to the subharmonic \(\log|r'_j|\):
\(|r'_j(t+iy)|\le m_x^{1-\omega}M_x^\omega\).
For \(y\le\eta\), the exponent of \(x\) is at most
\(-2+(A+2)(2-p)/(A+2)=-p\).
The lower rectangle gives the same estimate below the real axis. Centering a rectangle at every sufficiently large real part proves the assertion. Zeros of \(r'_j\) present no problem for the subharmonic inequality. ∎

Cauchy's estimate on a circle of radius \(\eta/2\) now gives

\[
|r_j^{(m)}(x)|\le C'_p(m-1)!(2/\eta)^{m-1}x^{-p},
\qquad m\ge1 .
\tag{4.103; P from (4.101)}
\]

In particular the second derivative is summable along a positively drifting weak-coupling trajectory. A direct Cauchy estimate on the polynomial bound alone would not give this decay; the real first-derivative estimate is used essentially. The entire counterexample (4.88a) violates the uniform polynomial tube, so there is no contradiction.

#### 4.17.2 One fixed source disk controls every scalar coupling derivative

Let \(x_{j+1}=F_j(x_j)=x_j-b+r_j(x_j)\), with
\(x_j-x_{j+1}\ge b_->0\), and assume (4.101). Choose the terminal lower threshold \(X_1\) sufficiently high that the disks of radius
\(d=\min(1,\eta/2)\) around the trajectory lie in the smaller strip. Put
\(D_p=2^pC_p\),
\(C_F=\exp[D_p/(b_-(p-1)X_1^{p-1})]\),
\(\sigma=d/(2C_F)\), and \(C_H=C_FD_p/[b_-(p-1)]\).

For \(z_0(s)=x_0+s\), \(z_{j+1}(s)=F_j(z_j(s))\), one has

\[
\begin{split}
|z_j(s)-x_j|&\le C_F|s|,\qquad |s|<\sigma,\\
|z_j(s)-x_j-s|&\le C_H|s|x_j^{1-p},\\
|z_j^{(m)}(0)|&\le m!C_H\sigma^{1-m}x_j^{1-p},
\qquad m\ge2 .
\end{split}
\tag{4.104; P under (4.101)}
\]

Indeed, while \(|z_j-x_j|\le d\), integration of \(r'_j\) along the complex segment gives
\(|z_{j+1}-x_{j+1}|\le(1+D_px_j^{-p})|z_j-x_j|\).
The real drift implies
\(\sum_{\ell<j}x_\ell^{-p}\le x_j^{1-p}/[b_-(p-1)]\), by integrating \(u^{-p}\) over the drift intervals. Iteration gives a deviation at most \(d/2\), closing the first-exit argument and proving holomorphy on the common disk. Telescope the remainder increments to obtain the second bound. The analytic function
\([z_j(s)-x_j-s]/s\), with its removable value at zero, has the stated uniform bound. Its Cauchy coefficient estimate proves the third line.

For a constant scalar source the physical bare shift is \(s=-t/(2N)\). If these \(F_j\) are the actual common-family coefficient maps for one coherent recipe, (4.104) supplies the corresponding source derivatives, with a factor \((2N)^{-m}\). This identification, and the quantitative tube for that complete family, are still C/O. N2-F alone has not been strengthened. A fixed-width polynomial tube is sufficient; a complex \(O(x^{-1})\) bound is not required.

#### 4.17.3 An elementary zero-free reference disk

There is a direct coefficient-analyticity theorem for a fixed positive reference. Let
\(q_X=e^{-X\mathcal A}/H(X)\) with fixed positive measure, and suppose the integrated real energy has essential oscillation \(D\), uniformly in admitted exterior variables. Put \(\alpha=2\log(3/2)\). Then

\[
H(X+z)\ne0,\qquad
\left|\frac{q_{X+z}}{q_X}\right|\le3
\quad(|z|\le\alpha/D),\qquad
\frac{|\partial_X^m q_X|}{q_X}
 \le3m!(D/\alpha)^m .
\tag{4.105; P}
\]

If \(D=0\), the normalized reference is constant. Otherwise center the energy at the midpoint \(a_0\) of a range interval of length \(D\). For \(B=\mathcal A-a_0\),
\(H(X+z)/H(X)=e^{-a_0z}Q_Xe^{-zB}\), and
\(|Q_Xe^{-zB}-1|\le e^{|z|D/2}-1\le1/2\).
This proves nonvanishing and the density ratio; Cauchy proves the derivatives. The logarithm of the centered partition ratio is bounded by \(\log2\), giving
\(|\partial_X^m\log H|\le m!\log2(D/\alpha)^m\) for \(m\ge2\).
The exact formulas are
\(\partial_X\log q_X=-(\mathcal A-Q_X\mathcal A)\) and
\(\partial_X^2\log q_X=-\operatorname{Var}_{Q_X}\mathcal A\), with variance at most \(D^2/4\). For the last assertion use
\(Q[(\mathcal A-a)(a+D-\mathcal A)]\ge0\).
No inverse unnormalized reference mass is used.

For the current-scale regular support in §4.15, B119 (2.4)–(2.5), p.255, gives
\(\epsilon_k=g_{B,k}A_0(\log X)^{p_0}\) and
\(R_k\le L(\log X)^r\), \(X=g_{B,k}^{-2}\).
LFR I p.177 restricts the selected original component to a cube of side \(100MR_k\). Consequently the coarse current-scale oscillation estimate yields
\(D\le CX^{-1}(\log X)^{2p_0+4r}\).
For this restricted support, (4.105) gives any prescribed fixed coefficient disk once the coupling ceiling is small enough. The stronger integrated reference estimate in §4.18 centers away the outer background and uses the actual fixed-size reset core \(\Lambda\); it should not be confused with counting all of \(Z\) as reference integration variables.

#### 4.17.4 Complete fresh and affine-reference derivatives on a positive regular block

A useful bound survives arbitrary source-independent positive reweighting. Let

\[
W_{s,t}=w\,e^{-sB_f-tB_g}
  \prod_{\nu=1}^J q_{\nu,X_\nu+s\lambda_{\nu f}
                                  +t\lambda_{\nu g}},
\quad w\ge0,\quad Z(s,t)=\int W_{s,t},
\quad \Pi=W_{0,0}/Z(0,0).
\tag{4.106; P: definition on fixed integration coordinates}
\]

Assume \(0<Z(0,0)<\infty\), fixed geometry and cutoffs, and conditional reference energy oscillations \(D_\nu\) uniformly in their real conditioning variables. These variables are fixed coordinates when differentiating the source. Define
\(S_f=-B_f-\sum_\nu\lambda_{\nu f}(\mathcal A_\nu-Q_\nu\mathcal A_\nu)\),
and similarly \(S_g\), and
\(T_{fg}=-\sum_\nu\lambda_{\nu f}\lambda_{\nu g}
\operatorname{Var}_{Q_\nu}\mathcal A_\nu\).
Put
\(b_f=\|B_f\|_\infty+\sum_\nu|\lambda_{\nu f}|D_\nu\), similarly \(b_g\), and
\(d_{fg}=\frac14\sum_\nu|\lambda_{\nu f}\lambda_{\nu g}|D_\nu^2\).
Exact differentiation gives

\[
\frac{W_{fg}}{W_0}=T_{fg}+S_fS_g,\qquad
\partial_{fg}\log Z=\Pi T_{fg}+\operatorname{Cov}_\Pi(S_f,S_g),
\qquad
\left|\frac{W_{fg}}{W_0}\right|,
\ |\partial_{fg}\log Z|
 \le d_{fg}+b_fb_g .
\tag{4.107; P}
\]

The bound follows from the pointwise score bounds and
\(|\operatorname{Cov}_\Pi(S_f,S_g)|\le
(\Pi S_f^2\,\Pi S_g^2)^{1/2}\le b_fb_g\).
It includes the derivative of each reference normalizer, every fresh/reference cross term, and every cross term between references. The arbitrary positive factor \(w\), including additional real selectors, is retained.

On an unexpanded regular block where **every contributing plaquette on the full integration domain** satisfies
\(\|U(\partial p)-1\|\le C\eta^2\epsilon_k\), the plaquette identity in §4.15 gives
\(\|B_f\|_\infty\le C\|f\|_\infty\epsilon_k^2V_0\).
Assume for each of the finitely many references that
\(|\lambda_{\nu f}|\le C\|f\|\),
\(|\lambda_{\nu g}|\le C\|g\|\), and
\(D_\nu\le C\epsilon_k^2V_\nu\) on that same current-scale support. Then, with \(V=V_0+\sum_\nu V_\nu\),

\[
|\partial_{fg}\log Z|,\quad |W_{fg}|/W_0
 \le C\|f\|\|g\|\epsilon_k^4 V^2.
\tag{4.108; P on this restricted positive regular domain}
\]

For one \(O(MR_k)\) carrier with bounded reference multiplicity this is
\(CX^{-2}(\log X)^{4p_0+8r}\|f\|\|g\|\), a summable numerical scale dependence along a positive lower-drift trajectory. Indeed the sum is bounded by a constant times
\(\int_{X_K}^\infty u^{-2}(\log u)^qdu
\le CX_K^{-1}(1+\log X_K)^q\).
This does not count all microscopic carriers in a physical source cell or perform their complex field projection.

For completeness the frozen positive block also has a fixed complex source disk. In one direction let the fresh energy have oscillation \(D_B\), set
\(C_{\rm block}=D_B/2+2\sum_\nu|\lambda_\nu|D_\nu\), and
\(r_{\rm block}=\log(3/2)/C_{\rm block}\).
For each reference, the proof of (4.105) gives
\(|\log(q_{X+s\lambda}/q_X)|\le2|s\lambda|D\) on the smaller disk. After centering the fresh energy by its range midpoint \(a_B\), the logarithm of the relative block weight is bounded by \(|s|C_{\rm block}\). Thus its exponential lies within \(1/2\) of one. Integrating against \(\Pi\) preserves that disk, so \(Z(s)\ne0\), the centered logarithm is at most \(\log2\), and Cauchy gives \(m!\log2\,r_{\rm block}^{-m}\) for derivatives of order \(m\ge2\). The complete normalized density ratio is at most three. If \(C_{\rm block}=0\), only a deterministic vacuum factor remains.

The limitations are concrete. The enlarged B116 fluctuation cutoff is \(g_k|B|<\epsilon_1\), with fixed \(\epsilon_1\); the whole extended contour cannot be assigned the smaller \(\eta^2\epsilon_k\) plaquette bound. The earlier quadratic-envelope and marked-cluster estimates, with their actual input norms, are needed there. These are real-exterior block estimates; a Wilson-field projection requires a joint complex-field bound and may still cost \(\rho_k^{-2}\). Finally, if the old weight moves with the source, let
\(a_f^{\rm in}=\partial_f\log w|_0\) and
\(a_{fg}^{\rm in}=\partial_{fg}\log w|_0\) where the logarithm exists. At zeros use its raw product-rule jets instead. The connected formula acquires
\(\Pi a_{fg}^{\rm in}\) and the covariance of
\(a_f^{\rm in}+S_f\) with \(a_g^{\rm in}+S_g\).
Those incoming and cross terms are mandatory. The frozen block has not supplied their full induction or the coherent-family tube (4.101).

## 4.18 All-order R-reference motion and the remaining normalization obstruction

The exact pure-Wilson R-reference permits a stronger integrated estimate than its energy oscillation. Its fluctuating integration region has bounded current-scale size. Centering removes the possibly large surrounding background energy. This closes an all-order reference-coefficient module and a chronological composition theorem, while identifying why neither is the compulsory-history normalization theorem.

#### 4.18.1 Gaussian scaling and the actual reference energy

Let \(E\subset\mathbb R^d\) be star-shaped about zero and \(Q\) a positive quadratic form. For the probability proportional to
\(1_Ee^{-Q(B)}w(B)dB\), assume \(0<m\le w\le M\), and put
\(B_0=\log(M/m)\). If \(\Xi=Q+R\), \(|R|\le R_0\), and
\(D=1+d+B_0+R_0\), then

\[
\mathbb E e^{\theta Q}\le e^{B_0}(1-\theta)^{-d/2}
\quad(0\le\theta<1),\qquad
\mathbb E\exp\!\left(\frac{|\Xi-\mathbb E\Xi|}{8D}\right)\le4 .
\tag{4.109; P}
\]

For the first inequality bound the numerator weight by \(M\), the denominator weight by \(m\), and substitute \(C=\sqrt{1-\theta}\,B\). The transformed domain lies inside \(E\), and the Jacobian is \((1-\theta)^{-d/2}\). No lower determinant estimate is needed. At \(\theta=1/2\), the resulting tail bound shows that \(|\Xi|\) is stochastically bounded by \(2D\) plus an exponential variable of rate \(1/2\). In particular \(\mathbb E|\Xi|\le4D\), and
\(\mathbb E e^{|\Xi|/(8D)}\le e^{1/4}/(1-1/(4D))\).
Centering multiplies this by at most \(e^{1/2}\), proving the second inequality.

Now take the actual reference of LFR I (1.100), with fixed real exterior, geometry, gauge graph, cutoff and minimizing maps. Write
\(\mathcal A(V')=A(\zeta_0,U_{k,Z}(V'V_\Lambda))\) and \(X=g_{B,k}^{-2}\).
At this base point use \(V'=\exp(ig_{B,k}B)\). The axial free coordinates form a Euclidean space, and (1.101) makes their domain a product of centered link balls. The exact expansion LFR II (1.2), pp.356–357, gives
\(X[\mathcal A(V')-\mathcal A(1)]=Q(B)+R(B)\).
Its (1.9), p.358, gives \(Q\ge c_M\|B\|^2\). The linear term is bounded by one in (1.6), and the scaled cubic term is bounded by
\(Cg_{B,k}^{1-\beta}|\Lambda|\), with the fixed \(\beta<1\) used there. Hence \(|R|\le C_M\) on the admitted weak-coupling range. The exponential-coordinate Haar Jacobian is positive with bounded logarithmic oscillation on the small chart.

Crucially, this reference integrates over \(\Lambda\), **not the whole original component \(Z\)**. LFR I (1.73), p.192, and LFR II p.358 place \(\Lambda\) inside a current-scale cube of side \(100M\). Its number of free real coordinates is at most \(d_M\), independent of ultraviolet depth. The possibly larger \(Z\) contributes to the background energy that cancels in the normalized reference. The explicit Haar constant and coupling powers cancel as well. Thus (4.109) applies to \(w=\sigma(g_{B,k}B)e^{-R}\) and gives

\[
Q_X\exp\!\left[
 \frac{X|\mathcal A-Q_X\mathcal A|}{8D_M}\right]\le4,\qquad
Q_X|\mathcal A-Q_X\mathcal A|^m
 \le4m!(8D_M/X)^m .
\tag{4.110; P for the actual frozen real R-reference}
\]

This estimate includes the reference's full energy dependence through its bounded reset core, after the constant background has canceled. It is not a bound for an unreduced \(T_k''\) operation or for all of \(Z\). For a different integration region the same proof retains its actual \(D=1+d+B_0+R_0\); it does not hide growing dimension in \(D_M\).

#### 4.18.2 All coefficient jets and square-summable composition

The group-coordinate domain and the chart \(B=g_{B,k}^{-1}\log V'\) are now frozen at the base \(X\); no cutoff or coordinate derivative is taken. Set \(Y=\mathcal A-Q_X\mathcal A\). The exact likelihood ratio is
\(q_{X+z}/q_X=e^{-zY}/Q_Xe^{-zY}\).
Since \(Q_XY=0\), (4.110) and
\(|e^w-1-w|\le\frac12|w|^2e^{|w|}\)
give, for \(|z|D/X\le c\),

\[
\begin{split}
\left|\log Q_Xe^{-zY}\right|&\le C|z|^2D^2/X^2,\\
Q_X\left|q_{X+z}/q_X\right|^2
 &\le \exp(C|z|^2D^2/X^2),\\
\left\|(\partial_X^m q_X)/q_X\right\|_{L^2(q_X)}
 &\le m!(CD/X)^m,\qquad
\int\partial_X^m q_X=0\quad(m\ge1).
\end{split}
\tag{4.111; P}
\]

For the first line choose the disk so that the centered moment-generating function lies within \(1/4\) of one and use its analytic logarithm. For the second line apply the same centered estimate to \(2\operatorname{Re}z\) in the numerator and to \(z\) in the denominator. Cauchy's formula in \(L^2(q_X)\), on a fixed fraction of the disk \(cX/D\), proves the third line; its total-variation version follows by Cauchy–Schwarz. An affine coefficient \(X+uz\) replaces \(D/X\) by \(|u|D/X\). Nonlinear coefficient curves need their actual higher derivatives.

There is an efficient composition theorem. Consider a chronological chain of normalized positive conditional references, with source-independent Markov steps allowed between them. Suppose the conditional version of the second line of (4.111) holds uniformly in the past, with predictable costs
\(b_j=u_j^2D_j^2/X_j^2\), and suppose
\(\sum_jb_j\le B\) on every path. On the common coefficient disk let
\(\ell_j(z)=dQ_{j,z}/dQ_{j,0}\) and \(L_n(z)=\prod_{j\le n}\ell_j(z)\). Then

\[
\mathbb E_0L_n(z)=1,\qquad
\mathbb E_0|L_n(z)|^2\le e^{C|z|^2B},\qquad
\|L_n^{(m)}(0)\|_2\le m!(C_1\sqrt B)^m .
\tag{4.112; P for the stated chronological chain}
\]

When \(B=0\), the likelihood is constant. Otherwise use a circle of radius \(c_1/\sqrt B\), with \(c_1\) small enough for every conditional disk. Normalization proves the first equality. The process
\(|L_n(z)|^2\exp[-C|z|^2\sum_{j\le n}b_j]\)
is a positive supermartingale under the base law, so its expectation is at most one. The pathwise bound on the sum proves the second inequality. Finite products are analytic; their locally uniform \(L^2\) bounds give Banach-valued analyticity, by testing against the dual and applying Morera and Fubini. Cauchy proves the final bound. Forgetting latent variables is conditional expectation and contracts \(L^2\), so the final retained relative density has the same derivative estimates.

For one bounded-core R-reference at each scale, bounded slopes and the matched positive-drift trajectory give
\(\sum_jb_j\le C\sum_jX_j^{-2}<\infty\).
More generally \(D_j\le C(1+\log X_j)^q\) is still summable with \(X_j^{-2}\). This is a depth-independent all-order reference-motion result.

The chain must remain unconditioned on future compulsory large-field flags. Such conditioning changes its conditional laws and can remove the centered estimate used above. Section 4.21 proves the complete positive lift in which all future flags are summed, so that no such conditioning is introduced; it also proves the stronger exact cancellation against original payloads. All components in a physical source patch must also be counted in \(\sum_jb_j\); one lineage per scale is not a count of all fine-scale components. An arbitrary final positive reweighting is not a source-independent Markov step. The oscillation bound (4.105), when available, survives such reweighting; the sharper integrated energy bound does not automatically do so.

#### 4.18.3 A restricted joint complex-background estimate

For a complex exterior the positive probability argument is replaced by a coercive comparison and the actual analytic denominator. In the same fixed chart write
\(X[\mathcal A_U(V')-\mathcal A_U(1)]=Q_U(B)+R_U(B)\), and let \(Q_0\) be the real flat-background comparison form on the same free coordinates. Work on a smaller admitted domain where

\[
|Q_U-Q_0|\le\tfrac14 Q_0,\qquad
|R_U|\le C_M,\qquad Q_0\ge c_M\|B\|^2 .
\tag{4.113; C/L: explicitly restricted complex domain}
\]

The perturbative comparison on LFR II p.357 and its extension described on p.358 bound the quadratic error by
\(C_M[R_k(\alpha_{0,k}+\alpha_{1,k})+e^{-R_k}]\|B\|^2\).
Impose its smallness relative to \(c_M\); this is a domain restriction, not a claim about every enlarged complex domain. This restriction is compatible with the actual published radii: B119 (2.5), p.255, and (2.28), p.259, give, with \(t=\log g_{B,k}^{-2}\),
\(R_k\le Lt^r\) and
\(\alpha_{i,k}=C_i g_{B,k}t^{q_i}\).
Hence
\(R_k(\alpha_{0,k}+\alpha_{1,k})
\le Lg_{B,k}(C_0t^{r+q_0}+C_1t^{r+q_1})\to0\).
Also \(e^{-R_k}\to0\). A sufficiently weak common coupling range therefore meets the quadratic comparison inside those radii, without enlarging them. The complex linear remainder is bounded by
\(C_Mg_{B,k}^{-1}p_0(g_{B,k})(\alpha_{0,k}+\alpha_{1,k})e^{-R_k}\),
which is a fixed polynomial in \(t\) times \(e^{-R_k}\); it is uniformly bounded. The other remainder bounds are the fixed-core estimates already used above. After removing the displayed background and Haar/coupling factors, LFR II (1.10)–(1.11), p.358, identifies the coordinate denominator as \(e^{-I(U_0)}\), with \(|I(U_0)|\le C_M\). Its modulus therefore has a uniform positive lower bound. This is nonvanishing of a complex integral, not positivity of a complex measure.

The absolute normalized numerator is at most \(C_Me^{-3Q_0/4}\), while
\(|X(\mathcal A_U-\mathcal A_U(1))|\le5Q_0/4+C_M\).
Multiplying by a sufficiently small exponential of that energy leaves an integrable Gaussian in at most \(d_M\) coordinates. Its first moment permits centering at \(Q_{X,U}\mathcal A_U\) as well. Consequently

\[
\int |q_{X,U}|\,
 e^{c_M X|\mathcal A_U-Q_{X,U}\mathcal A_U|}
 \le C_M,\qquad
\int|\partial_X^m q_{X,U}|
 \le m!(C_M/X)^m,\qquad m\ge1 .
\tag{4.114; P on (4.113) and the quoted nonvanishing denominator bound}
\]

For the derivative estimate use the same exact exponential-tilt quotient, now with a normalized complex integral. Its centered first moment is still zero. The total-variation exponential bound keeps the denominator within \(1/4\) of one on a coefficient disk of radius \(c_MX\), and bounds the quotient in total variation there. Banach-valued Cauchy gives the assertion. The real chronological \(L^2\) theorem has not thereby become a theorem for complex path probabilities. Equation (4.114) concerns one reference kernel on its specified joint domain.

#### 4.18.4 What an exact R reset preserves

Let \(\sigma_v(d\omega)\) be the old positive conditional measure at fixed exterior \(v\), and let \(q_v(u)du\) be the normalized new reference. Retain the old variables as latent labels, as required for raw source derivatives. The exact replacement is
\(d\widehat\sigma_v(u,\omega)=q_v(u)du\,d\sigma_v(\omega)\).
For every integrable old raw coefficient \(F_I\), of either sign, and every nonnegative old budget \(V\),

\[
\widehat\sigma_v(1)=\sigma_v(1),\qquad
\widehat\sigma_v(e^{sV})=\sigma_v(e^{sV}),\qquad
\widehat\sigma_v(F_I)=\sigma_v(F_I).
\tag{4.115; P; actual operation LFR I (1.100)–(1.102)}
\]

Integrate \(q_v\) first; Tonelli proves the positive identities and integrability proves the signed one. Repeating this argument backwards proves the same identities for any finite chain of normalized resets preserving the exterior.

In particular the old logarithmic mass deficit
\(\log[\sigma_v(e^{sV})/\sigma_v(1)]\)
does not decrease merely because the new field is regular. Neither does its integrated fractional moment under an unchanged exterior law. Take an old two-atom measure of mass \(e^{-2sn}\), budget \(V=n\), and mark \(F=n\xi\), \(\xi=\pm1\). Even if the new reference is supported entirely on perfectly regular fields, the normalized old second moment remains \(n^2\).

There is nevertheless a true new-flag suppression estimate on a flat admitted shell. The fixed-core coercivity, bounded remainder and denominator yield
\(q_X(B)\le C_Me^{-c_M\|B\|^2}\), so
\(Q_X(\|B\|_\infty\ge r)\le C_Me^{-c_Mr^2}\).
With flat determining data the minimizing reference is flat. Products of four links and B102 Theorem 1, (8), p.279, show that
\(\|B\|_\infty\le c_M\epsilon_k/g_{B,k}\)
implies the localized new regularity test. Thus the new bad-flag probability is at most
\(C_M\exp[-c_M(\epsilon_k/g_{B,k})^2]\).
A nonflat shell requires a separately proved strict cutoff margin. This bounds the fraction of the fixed old branch carried by that new flag, and the flagged total variation of a fixed old coefficient. It does not bound the old coefficient divided by its mass, as (4.115) makes explicit.

#### 4.18.5 Why global interpolation does not settle the local fractional comparison

A counterexample isolates the missing local comparison. Fix \(a>c>s>0\), \(s<1\), and \(N\) compact single-cell probability spaces with a regular subset of measure \(e^{-a}\) in each cell. Let \(G_N\) be the event that all cells are regular. For an ultraviolet label \(K\), define
\(\rho_{K,N}=1_{G_N}+e^{-K-cN}1_{G_N^c}\) and
\(V_{K,N}=(K+N)1_{G_N^c}\).
The empty history is allowed on \(G_N\); elsewhere a volume-spanning component is compulsory. Throughout \(0\le\theta\le1\),

\[
\begin{split}
Z_{K,N}(\theta)
 &=e^{-aN}+e^{-(1-\theta s)K-(c-\theta s)N}(1-e^{-aN}),\\
e^{-aN}&\le Z_{K,N}(\theta)\le1,\\
\sigma_{\rm bad}(e^{sV})
 &\le e^{-(1-s)K-(c-s)N}.
\end{split}
\tag{4.116; P}
\]

Thus global stability holds uniformly even for the whole interpolation, and the bad component has an arbitrarily strong fixed exponential volume reserve by increasing \(c\) and then \(a\). Choose a cofinal sequence \(N_K\) with \((a-c)N_K\ge2K\); compatible fourth-power volumes can be used. Its bad-sector probability tends to one, since the regular mass divided by the bad mass is at most \(e^{-K}/(1-e^{-aN_K})\). Therefore
\(Z_{K,N_K}(\theta)/Z_{K,N_K}(0)\ge
(1-o(1))e^{\theta s(K+N_K)}\to\infty\) for every fixed \(\theta>0\).

Taking conditional mass \(t=\rho_{K,N}\) and exact reserve \(\varepsilon=t e^{sV}\) makes that ratio precisely
\(\int\varepsilon^\theta t^{1-\theta}/\int t\).
An active mark anchored in one designated cell can be carried by the compulsory spanning component: take a sign label \(\xi=\pm1\) in that cell and \(F=K\xi\,1_{G_N^c}\), so \(|F|\le V\); its normalized second moment grows as \(K^2\). This is an example within the abstract history/envelope bounds, not a Wilson-theory counterexample or an assertion about a strictly local bare observable. It deliberately lacks the needed common-exterior deletion or repair property.

Hölder only gives
\(\int\varepsilon^\theta t^{1-\theta}\le
(\int\varepsilon)^\theta(\int t)^{1-\theta}\).
Global stability then permits a cost proportional to total torus volume. The example proves that it cannot be replaced by the number of active source cells using those assumptions alone. The actual R2 target remains (4.81), for the **complete** active-patch kernel, or a stronger proved local comparison. A successful finite-depth repair must compare with another allowed branch in that same denominator or use a controlled common-exterior change of variables; normalizing the new R-reference alone has already preserved the old mass.
