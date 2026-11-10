# Conditional restoration with the cutoff normalizer retained

This note proves a finite-dimensional energy estimate for variables restored
from an actual conditional integral. The theorem does not assume that a
cutoff-completion probability is bounded below. Its first-Wilson application
uses the Hessian bounds already proved in RMg. The full multiscale residual
application additionally needs a common positive refinement and its actual
energy identity.

## 1. A convex-domain exponential moment

Let C be a bounded convex product of norm balls containing zero in its
interior, in n real scalar coordinates. A general bounded convex domain
containing zero also suffices. Let K be a positive definite real matrix.
Let V be twice differentiable on a neighborhood of C and suppose
\[
 \nabla^2 V(b)\succeq aK,\qquad a>0,\qquad
 h=-\nabla V(0).
 \tag{CR.1}
\]
Write q(db)=Z^{-1}1_C(b)e^{-V(b)}db. Then, for
\(0\le\theta\le a/4\),
\[
 \log q\!\left(e^{\theta b^{\mathsf T}Kb}\right)
 \le \theta\left(\frac{4n}{a}
       +\frac{4\|h\|_{K^{-1}}^2}{a^2}\right).
 \tag{CR.2}
\]
All normalization is the actual conditional normalization Z.

**Proof.** First suppose the boundary is piecewise smooth. Because C is
convex and contains zero, its outward unit normal satisfies
\(b\cdot n_C(b)\ge0\) almost everywhere. The divergence theorem gives
\[
 0\le \int_{\partial C}b\cdot n_C\,e^{-V}\,dS
    = nZ-\int_C b\cdot\nabla V\,e^{-V}\,db .
\]
Integrating the Hessian lower bound along the segment from zero to b gives
\[
 b\cdot\nabla V(b)\ge a\,b^{\mathsf T}Kb-h\cdot b.
\]
Consequently, with \(X=q(b^{\mathsf T}Kb)\),
\[
 aX\le n+\|h\|_{K^{-1}}\sqrt X
      \le n+\frac a2 X+\frac{\|h\|_{K^{-1}}^2}{2a}.
\]
Thus
\[
 q(b^{\mathsf T}Kb)\le
       \frac{2n}{a}+\frac{\|h\|_{K^{-1}}^2}{a^2}.     \tag{CR.3}
\]
The potential \(V_\theta=V-\theta b^{\mathsf T}Kb\) has the same
gradient at zero and Hessian at least \((a-2\theta)K\).
For \(0\le\theta\le a/4\), apply (CR.3) with \(a-2\theta\ge a/2\).
Integrating the identity
\(\partial_\theta\log q(e^{\theta b^{\mathsf T}Kb})
=q_\theta(b^{\mathsf T}Kb)\) proves (CR.2).
Approximation by smooth convex domains or convex barriers gives the same
result for the product norm balls, including their corners. The integrals
converge on a common bounded set. QED.

The n in this estimate counts the coordinates actually restored. It does
not count an unrelated exterior region.

## 2. Exact Gaussian restoration and the retained Schur energy

Split the coordinates of one positive Gaussian form into restored b and
retained u:
\[
 K_{\rm full}=
 \begin{pmatrix}K_{BB}&K_{BO}\\K_{OB}&K_{OO}\end{pmatrix},
 \qquad mI\preceq K_{\rm full}\preceq MI.
 \tag{CR.4}
\]
For fixed u, retain the actual product cutoff in b. The conditional
potential is
\[
 V_u(b)=\tfrac12 b^{\mathsf T}K_{BB}b+
               b^{\mathsf T}K_{BO}u .
\]
The conditional mean before truncation is
\(m_B(u)=-K_{BB}^{-1}K_{BO}u\).
The untruncated retained Schur form is
\[
 S_O=K_{OO}-K_{OB}K_{BB}^{-1}K_{BO}.
\]
Even though the actual marginal in u also contains a cutoff completion
factor, the following matrix bound is unchanged:
\[
 \|K_{BO}u\|_{K_{BB}^{-1}}^2
 \le \frac{M^2}{m^2}\,u^{\mathsf T}S_Ou.             \tag{CR.5}
\]
Indeed the left side is at most \(M^2m^{-1}\|u\|^2\),
and \(S_O\succeq mI\). Applying CR.2 with \(a=1\) yields
\[
 q_u\!\left(e^{\theta b^{\mathsf T}K_{BB}b}\right)
 \le \exp\!\left[
       4\theta n_B+
       C_{m,M}\theta\,u^{\mathsf T}S_Ou\right],
 \quad 0\le\theta\le\tfrac14.                       \tag{CR.6}
\]
The same argument bounds the conditional innovation
\(b-m_B(u)\) after a fixed reduction of theta, since
\[
 \|b-m_B(u)\|_{K_{BB}}^2
 \le2\|b\|_{K_{BB}}^2+
        2\|K_{BO}u\|_{K_{BB}^{-1}}^2.
\]

CR.6 is not obtained by dropping the cutoff normalizer. It remains true
when its value is extremely small or depends on u.

## 3. Stability under the proved first-step interaction

Suppose the conditional potential is instead
\[
 V_u(b)=\tfrac12 b^{\mathsf T}K_{BB}b+
       b^{\mathsf T}K_{BO}u-W(b,u),
\]
and, on the same cutoff,
\[
 \|\nabla_b^2W\|\le\delta,\qquad
 \delta\le m/2,\qquad
 \|\nabla_bW(0,u)\|^2\le \rho^2 n_B.                \tag{CR.7}
\]
Then \(\nabla^2V_u\succeq \frac12 K_{BB}\), and
\[
 \|-\nabla_bV_u(0)\|_{K_{BB}^{-1}}^2
 \le C_{m,M}u^{\mathsf T}S_Ou+C_m\rho^2 n_B.
\]
Equation CR.2 therefore gives
\[
 q_u\!\left(e^{\theta b^{\mathsf T}K_{BB}b}\right)
 \le \exp\{C\theta[(1+\rho^2)n_B+
                         u^{\mathsf T}S_Ou]\},
 \qquad 0\le\theta\le\theta_*(m,M).                 \tag{CR.8}
\]

For the actual first globally P/Q-regular Wilson chart, RMg gives
\(\delta=O(gP+g^2)\) and
\(\rho=O(gP^2+g^2P)\), uniformly in the admitted held variables
on the encompassing fixed product chart. W here includes its complete
Haar, coarea and constraint-Jacobian contributions. Thus CR.8 applies to
a subset of variables conditionally restored in that chart, with the
same actual density and its cutoff. This is an admitted-domain assertion;
it does not yet supply every shifted ambient version or discrete
history current.

## 4. Transfer an existing retained reserve

Let pi be any actual retained law, and suppose
\[
 \pi(e^{tE_{\rm ret}})\le e^A,\qquad
 E_{\rm ret}\ge u^{\mathsf T}S_Ou,\qquad t>0.
 \tag{CR.9}
\]
Then the joint law pi(du)q_u(db) obeys, for a fixed sufficiently small
theta depending only on t and the constants above,
\[
 (\pi q)\exp\{\theta[E_{\rm ret}+b^{\mathsf T}K_{BB}b]\}
 \le \exp\{A+C\theta(1+\rho^2)n_B\}.               \tag{CR.10}
\]
This follows by applying CR.8 first and choosing
\((1+C)\theta\le t\). It retains the original joint normalization.

The same statement can be expressed for an unnormalized positive mass M.
If \(M(e^{tE_{\rm ret}})\le U\), the restored mass of the displayed
exponential is at most \(U\exp(C\theta(1+\rho^2)n_B)\).
No lower bound on M1 is needed for this upper estimate. A matched lower
bound can subsequently normalize it.

## 5. Why one common energy is needed across many levels

It is not legitimate to apply CR.10 at N levels and silently ignore the
successive reductions of theta. A naive iteration can cost a factor
\((1+C)^N\), which is too large for the desired uniform estimate.

For one finite Gaussian joint law, however, all Schur disintegrations are
factorizations of the **same** positive quadratic energy. Completing
squares in any order gives the exact identity
\[
 \tfrac12 z^{\mathsf T}K_{\rm full}z
 =\tfrac12 u^{\mathsf T}S_Ou+
  \tfrac12(b-m_B(u))^{\mathsf T}K_{BB}(b-m_B(u)).
 \tag{CR.11}
\]
A common refinement must be defined before using this identity. Keeping
the joint positive energy then lets either history's partial Schur form
be bounded by that one energy, without multiplying an operator constant
at each depth. Hard cutoffs contribute their actual completion factors
to the marginal laws; they do not invalidate the pointwise quadratic
identity.

The analogous nonlinear residual assertion requires more information:
the actual changes of variables and gauges, all Jacobians, the complete
positive action/energy ledger, and a comparison of the two histories'
literal tests with that common energy. The source's preparation failure
estimates may provide this comparison once the common refinement has
been constructed. They do not do so merely because two separate
coordinate lists have small rank.

This note therefore closes the conditional moment calculation and one
regular-chart application. It records the multiscale matching obligation
explicitly and does not claim the complete two-history theorem.
