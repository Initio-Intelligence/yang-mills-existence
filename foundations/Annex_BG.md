# A spatial carrier criterion for marked conditional kernels

**Annex BG.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).

For the developments under their corresponding hypotheses, see [the history extensions](../history/README.md) and [the scalar matching analysis](../observable_transport/README.md).


The following is a concrete sufficient estimate for the remaining H-03 problem. It is **not proved**. It states the unknown in the existing M-03 quantities rather than replacing the estimate by a moment bound. The actual input records are the prepared records entering the R step; their earlier preparation is a separate obligation.

Fix the literal positive source-free R coupling, all retained exterior and residual-history data x, and the actual old conditional probability Q_x obtained after including its self action and all cross activities. Fix a source order m and a partition into incoming vertices F_1,...,F_l, of positive source grades d_1,...,d_l with sum m. Each incoming vertex carries its existing compatible triple (F_i,B_i,J_i) and its true padded dependency footprint. The conditional cumulant is

\[
 K_{\boldsymbol d}(x)=\kappa_{Q_x}(F_1,\ldots,F_l).
 \tag{KT19.1}
\]

For l=1 this denotes Q_x F_1. All higher incoming log-jet vertices are included by allowing every partition and every grade tuple; replacing them by only first-order marks would not meet the test.

### Required actual decomposition and estimate

Construct a compatible physical-carrier expansion

\[
 \mathbf K_{\boldsymbol d}
   =\sum_Z\bigl(K_Z,B_Z,J_Z^{\rm old}+J_Z^{\rm new}\bigr),
 \qquad \delta K_Z=B_Z+J_Z^{\rm old}+J_Z^{\rm new},
 \tag{KT19.2}
\]

in the exact current/retained coordinates of this R step. Here B_Z includes the direct coordinate pullback, J_Z^old transports the already present current records, and J_Z^new contains every change of the normalized old law, including selectors, domain/geometry labels and the denominator. It is not permissible to combine B and J before taking their separate norms.

For fixed positive kappa_out less than the available input decay reserve and some fixed C,q, prove

\[
 \sum_Z e^{\kappa_{\rm out}(|Z|+\mathsf t_h(Z))}
  \left[v_{h,m,Z}(K)+g_{h,m,Z}(B)
       +j_{h,m,Z}(J^{\rm old})+j_{h,m,Z}(J^{\rm new})\right]
 \le C^{m+l}(l!)^q
      \prod_{i=1}^{l}\|\mathbf F_i\|_{h,\kappa_{\rm in}}.
 \tag{KT19.3; open}
\]

The terms v,g,j and the input norm in this display are **exactly M-03 (M.11)–(M.12)**. In particular their value part includes

\[
 h^{4m}\mathfrak m_m(K_Z^\sharp;\mu_{\rm out})
 +\frac{h^{4m}}{m^m}
       \sup_x\frac{K_Z^\sharp(x)}{\widehat R_{h,Z}(x)^m},
 \tag{KT19.4}
\]

and their current parts use the grade m+1/2, the summed finite-difference envelope, and the corresponding shifted **output** native regulator. All ambient shifts in the specified M-03 versions are included; membership in an interior analytic chart is not a substitute for this quantifier. Constants may depend on the fixed source parameters and chosen input-class budget, but not on the cutoff, volume, number of older layers, actual remaining history or the position of the component.

The full jet is the sum of KT19.1 over its labeled partitions. The already recorded finite-jet partition algebra then gives its complete response; it does not remove any part of KT19.3. Subsequent all-scale inductive closure remains with the corresponding marked-induction estimates.

### What must enter the new-current record

For one retained direction tau with nonzero continuous displacement t, let M_x and M_(tau x) be the unnormalized kernels on the same padded hidden space, with masses Z_x and Z_(tau x). The mandatory new current at a first moment is

\[
 J_{\tau}^{\rm new}(F)(x)
 =\frac{1}{tZ_{\tau x}}
   \int\left(F_x-Q_xF_x\right)
                    d\left(M_{\tau x}-M_x\right).
 \tag{KT19.5}
\]

For a discrete replacement take t=1. The direct term is Q_(tau x)[(F_(tau x)-F_x)/t], preserving its B and old-J split. If M_x=chi_x r_x and the smooth part changes by exp(sigma), KT19.5 includes the selector measure (chi_(tau x)-chi_x) exp(sigma) r_x. For a cumulant apply these exact rules to every conditional moment in its finite partition formula. This specifies J^new without discarding support changes.

The marked chart problem is to realize KT19.2–KT19.5 for the actual preintegration map, including every old hidden variable. The native fixed-support tilt in LFR II (1.73)–(1.75) bounds one part of KT19.5. It does not identify all the raw/selector/geometry changes in that display with native analytic shifts.

### Precisely what is available and what remains

The pure fresh-coordinate directions in the correctly fixed-reference R quotient have J^new=0 exactly, as proved in MG19.1. The continuously integrated support after preparation is inside a fixed current-block core, so its connector cost is bounded. These facts remove two costs from KT19.3.

Still open are the actual retained-direction chart/pullback and selector terms in KT19.5, their pointwise comparison to the shifted output regulator in KT19.4, and their full dependency footprints in KT19.3. The source-native response endpoints include Gamma''_k intersect X-tilde, so the core volume alone does not pay that full footprint.

An explicitly adopted joint-history coupling can set additional fresh and output-descriptor currents to zero and preserve small component masses. If it is used, Q in KT19.1–KT19.5 must be its actual mixture posterior, including the descriptor-mean cumulants. The same norm estimate must still be proved. Changing the coupling does not, on its own, verify KT19.3.
