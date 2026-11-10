# Actual normalized successful-component energy and rank moments

This note combines two estimates for the Wilson law: the complete positive mixed posterior in HS20 and the old energy/rank reserve in NR20. It turns the conditional deletion consequence into a normalized theorem for **successful components in the joint law**. It does not condition on the presence of a component, control fixed residual-component energies, or claim a full M-03 carrier representation.

### 1. Fixed actual posterior and a common exponential store

Fix an admitted real retained datum \(v\). Use exactly the posterior

\[
 \pi_v(dC,d\eta_Y,d\eta_C)
  =Z_v^{-1}\mathbf1_{\{C\ {\rm admissible}\}}e^{H_C}
       \prod_i\nu_{Y_i}(d\eta_{Y_i})
       \prod_{X\in C}M_X(v,d\eta_X)
 \tag{NM20.1}
\]

of HS20.4. Each residual base includes all its required old and descriptor-dependent reference factors. Each successful \(M_X\) is unnormalized. Its internal histories are summed inside it, and the cross action retains their dependence. There is no signed activity probability and no replacement reference used in place of the old law.

Let \(\mathcal F_X^\natural\) be NR20.15's common positive native envelope, and \(D_X\) the actual surviving Gaussian coordinate rank in NR20.9a. Put

\[
       B_X=\mathcal F_X^\natural+D_X\ge1 .
 \tag{NM20.2}
\]

The ordinary birth-scale native free squares are bounded by a fixed multiple of this energy, by NR20.1a, with the exact coordinate qualification there. No raw old plaquette energy is added to the definition.

Choose the fractional-energy reserve parameter \(\theta_0>0\) in NR20.1 and a fixed rank parameter \(u_0>0\) in NR20.9a. Fix once and for all

\[
        0<t\le\tfrac12\min\{\theta_0,u_0\}.
 \tag{NM20.3}
\]

The same common source ceiling can then be used for all source orders. Equations NR20.9a and NR20.14–NR20.16 give

\[
          M_X(v,e^{tB_X})\le C_0e^{-P_k},
       \qquad P_k=P_0(g_k),
 \tag{NM20.4}
\]

uniformly in \(X,v\) and old depth. Indeed the common-envelope bound is
\(\mathcal F_X^\natural\le1+\mathcal F_{X,0}+\delta_Q\), and the density comparison contributes at most \(e^{\delta_\sigma}\). The remaining insertion has coefficients \(t\le\theta_0\) and \(t\le u_0\), so the actual reserve applies. \(C_0\) is fixed. This calculation uses a positive real reference; analytic native directions enter only through total variation and the positive envelope.

The source-specific component deletion and interaction bound HS20.1/HS20.7 give

\[
 H_{C\cup\{X\}}-H_C\le\lambda_R
 \tag{NM20.5}
\]

whenever insertion is allowed, with \(\lambda_R\) uniformly small at the common ceiling. Reduce that ceiling so that

\[
        \lambda_R+\log C_0\le P_k/2
 \tag{NM20.6}
\]

at every admitted scale.

### 2. A normalized exponential theorem

#### Theorem NM20.1 — pinned successful energy and rank

For every compatible finite family \(\mathcal D\) of candidate successful components,

\[
 \boxed{
 \mathbb E_{\pi_v}\!\left[
   \mathbf1_{\{\mathcal D\subset C\}}
       \exp\!\left(t\sum_{X\in\mathcal D}B_X\right)\right]
       \le e^{-P_k|\mathcal D|/2}. }
 \tag{NM20.7}
\]

If the prescribed family is incompatible, the left side is zero. The bound is uniform in all remaining source-admitted data and internal old depth. It is a statement about the full normalized posterior (NM20.1).

**Proof.** In the numerator of (NM20.1), restrict to \(C\supset\mathcal D\) and write \(C=E\cup\mathcal D\). HS20.1 says that deletion leaves an admissible \(E\), the same retained datum and exactly the same remaining component measures. In particular it leaves the residual bases unchanged.

Successive deletion, or insertion in the reverse order, gives
\[
             H_{E\cup\mathcal D}-H_E
                         \le|\mathcal D|\lambda_R .
\]
This inequality holds uniformly in all old states, including the residual states still integrated. Therefore the deleted integrations factor, and the restricted numerator is at most
\[
 e^{|\mathcal D|\lambda_R}
       \prod_{X\in\mathcal D}M_X(e^{tB_X})
   \sum_{\substack{E\ {\rm admissible}\\E\sim\mathcal D}}
        \int e^{H_E}\prod_i d\nu_{Y_i}
                         \prod_{X\in E}dM_X .
\]
Positivity bounds the remaining restricted sum by the **same full partition function** \(Z_v\). Divide by it and apply (NM20.4)–(NM20.6). No \(m_X^{-1}\) is introduced. ∎

#### Corollary NM20.2 — every polynomial grade

For nonnegative integers \(m_X\), and also for a single total power \(m\ge0\),

\[
 \mathbb E_{\pi_v}\!\left[
  \mathbf1_{\{\mathcal D\subset C\}}
        \prod_{X\in\mathcal D}B_X^{m_X}\right]
 \le e^{-P_k|\mathcal D|/2}
                  \prod_{X\in\mathcal D}t^{-m_X}m_X!,
 \tag{NM20.8}
\]

\[
 \mathbb E_{\pi_v}\!\left[
  \mathbf1_{\{\mathcal D\subset C\}}
        \left(\sum_{X\in\mathcal D}B_X\right)^m\right]
 \le e^{-P_k|\mathcal D|/2}t^{-m}m! .
 \tag{NM20.9}
\]

For \(m=0\), interpret the total-power expression as the occupation indicator. For a real power \(q\ge1\), replace the integer-power factor \(t^{-m}m!\) by \((q/(et))^q\).

**Proof.** Apply \(x^m\le m!t^{-m}e^{tx}\) to each factor or to the total sum and use (NM20.7). ∎

The estimates are pointwise in the actual admitted \(v\). Integrating over its true outer marginal preserves them. They are not an estimate for \(\pi_v(\cdot\mid\mathcal D\subset C)\): that division would remove the occupation probability.

### 3. Anchored geometry cost and finite marked numerators

For every fixed physical component weight \(\kappa>0\), the source bound on eligible component size and the shape count in HS20.9 imply

\[
 \sup_b\sum_{X\ni b}
      e^{\kappa(|X^+|+\mathsf t(X^+))}
 \mathbb E_{\pi_v}\!\left[
       \mathbf1_{\{X\in C\}}B_X^m\right]
        \le C^{m+1}m!\,e^{-P_k/4}
 \tag{NM20.10}
\]

at one common ceiling. Both the number of shapes through \(b\) and the footprint weight are bounded by \(\exp[C_\kappa R_k^d]\), and \(P_k\gg R_k^d\); this proves the displayed estimate from (NM20.8). The internal histories have already been summed in \(M_X\) and are not counted again.

This is a weighted **positive energy majorant** in the actual normalized law. It does not state that the resulting function of \(v\) has carrier \(X^+\). Its dependence through the full posterior can require additional connecting carriers; constructing and paying those actual carriers remains a separate marked-localization task.

The same reserve controls every finite unnormalized marked numerator inside the normalized law. For a compatible fixed \(\mathcal D\), suppose the degree-\(d\) incoming log-jet coefficients obey

\[
 |A_B|\le K^{d+1}(d!)^s b^d r(v)^d
          \left(\sum_{X\in\mathcal D}B_X\right)^d,
 \qquad d=|B|,\quad s\ge1 .
 \tag{NM20.11}
\]

Define the finite formal numerator
\[
 N_{\mathcal D}(t)
   =\pi_v\!\left[
      \mathbf1_{\{\mathcal D\subset C\}}
                \exp\!\left(\sum_{B\ne\varnothing}t_BA_B\right)
           \right].
 \tag{NM20.12}
\]

The labeled partition identity and (NM20.9) give

\[
 |\partial_I N_{\mathcal D}(0)|
   \le e^{-P_k|\mathcal D|/2}
           C^m(m!)^{s+1}b^m r(v)^m,
       \qquad |I|=m .
 \tag{NM20.13}
\]

For completeness, a partition with block sizes \(d_1,\ldots,d_\ell\) has total energy degree \(m\), so its integral costs \(t^{-m}m!\) by (NM20.9). The ordered-size identity bounds
\[
 \sum_{\pi\in\Pi_m}\prod_{B\in\pi}(|B|!)^s
                  \le C^m(m!)^s,\qquad s\ge1.
\]
Absorb the fixed \(K^{m+\ell}\), \(t^{-m}\) and the number of compositions into \(C^m\). This proves (NM20.13), with every higher incoming vertex retained. The bounds are compatible under finite-order truncation.

No logarithm of \(N_{\mathcal D}\) is taken: normalizing this pinned numerator by its constant term would again divide out the rare occupation. The complete unpinned reset logarithmic jet is separately the exact HS20.29 formula.

### 4. Exact limits of the result

The actual normalized estimate now covers the successful-component energy/rank class. Fixed residual \(Y\) components have no absent state in (NM20.1), so this deletion argument supplies no rare mass for their individually normalized energies. It also does not control all raw old plaquette energies, arbitrary raw retained shifts, moving selector boundaries or all separate kernel-current records. Its geometry-weighted positive majorant is not an M-03 carrier expansion of a transported scalar or tensor.

The same deletion argument without the rank variable gives RA20.1. M-04, M-06 and H-04 require stronger marked estimates.
