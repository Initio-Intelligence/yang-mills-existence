# Heterogeneous constrained precision and coercivity

**Composed-response hypothesis (CR).** Each complete boundary conclusion below assumes the displayed native-chart and spatial response estimates for the actual iterated reconstruction, with the prescribed earlier innovations and raw variables fixed, uniformly over the admitted histories. A sufficient estimate for the latent contribution is (A.8) in [Conditional-law estimates and the continuum application](../continuum/conditional_to_continuum.md), refined for the anchored exterior derivative in PG.18–PG.20. The two endpoint bounds concern the identical Wilson-subtracted primitive, its actual cutoff and its independently extended current. A direct minimizing-field derivative alone does not establish this hypothesis. The application to every required original Wilson history remains open. Complete boundary estimates and their C06/C08 applications in this chapter are conditional on CR and the other displayed source, AF, domain and support assumptions. Exact density identities and abstract inequalities retain their individually stated hypotheses.

In the projective density formulation, a sufficient comparison is
\[
 \sup_{\zeta,x,a}\left|
 \log\frac{W_\zeta(x,a)W_0(x,a_*)}
               {W_0(x,a)W_\zeta(x,a_*)}
 \right|\le\delta_r<\pi/2,
\]
on the stipulated chart with the required uniform rates and actual fixed support. The composed ordinary response is the unresolved input in its derivation. The exact partial-gauge transport and the surviving fixed-exterior derivative are given in the chapter [Gauge covariance of partial integrals and exterior scores](../continuum/partial_gauge_transport.md), equations PG.2–PG.6 and the subsequent anchored-score criterion.

**Status:** the C-06 implication is proved at the retained J0/C01 source-construction and AF scope, and its C05 interface is assumed through CR and the boundary-induction assembly with the two-age OR.19 replacement. This note checks that interface explicitly. It does not infer a small Hessian from the polynomial ordinary-action bound in SR.24.  
**Scope:** every finite cutoff, admissible volume, current scale, real retained datum, and admitted source history in the theorem group's fixed construction; one set of source parameters and one weak-coupling ceiling. No moving-selector derivative or physical-observable matching theorem is asserted.

## 1. The original obligation and the conclusion

The unchanged C-06 condition asks to extend the regular derivative and coercivity estimates to the heterogeneous retained backgrounds and layer geometries actually encountered, with explicit weighted norms and domain margins. Its declared predecessors are C04 and C05. Annex AI already proved that implication, including the actual constrained principal operator. The missing application was the complete boundary estimate on its real current support and common native chart.

The present note makes the new application explicit. In particular, there are **three different bounds**:

1. SR.24 is a polynomial bound on an ordinary preintegration difference on an enlarged ordinary analytic chart.
2. Radial Cauchy comparison turns that into a small projective variation of a literal stopped density, with fixed earlier raw variables. This gives a uniform normalized-kernel bound and positive-catalog transfer.
3. The current endpoint calculation CE4–CE22, using the positive capacity induction and the separate ordinary-sector estimates, gives a bounded current prefactor and the required first/second derivatives.

The first bound is not used as the third one. The scalar mass that cancels from a normalized insertion remains in the complete action and native-derivative decomposition.

### Theorem C6.7 (assuming CR)

Retain the J0/C01 source construction and its stipulated two-sided AF trajectory. Use C02, C03 and C04, together with the C05 conditional estimates FP.1–FP.26 with SR.24 replacing the old OR.19 derivation. Fix the source representation, complete internally resummed atoms, and native continuation as in those statements.

There are constants

\[
\lambda_0>0,\quad \gamma>0,\quad C<\infty,\quad g_*>0
\tag{C6.1}
\]

independent of cutoff depth, volume, history length and derivative order such that the actual current conditional potential on every admitted retained fiber satisfies

\[
D_z^2V_{k,v}(z)\ge\frac34\lambda_0 I
\tag{C6.2}
\]

throughout the entire actual real current support. Its pointwise inverse satisfies

\[
\left\|\bigl[D_z^2V_{k,v}(z)\bigr]^{-1}_{ij}\right\|_{\rm op}
\le\frac2{\lambda_0}e^{-\gamma\rho_k(i,j)}.
\tag{C6.3}
\]

The same conclusions hold under every real linear current tilt. The complete perturbation \(W\), after the exact principal quadratic and retained exterior linear force have been separated, has

\[
\sup_{v,z,i}\|D_iW(z;v)\|\le CP_k^{-1},
\tag{C6.4}
\]

and a symmetric nonnegative matrix

\[
A_{ij}(v)\ge\sup_z\|D_iD_jW(z;v)\|_{\rm op},\qquad
\sup_i\sum_j e^{\gamma\rho_k(i,j)/2}A_{ij}(v)
\le CP_k^{-2}.
\tag{C6.5}
\]

The supremum in (C6.5) may be taken over the admitted inner complex current chart. The source current and unsubtracted native local-jet estimates hold on the quantitative common domain in Section 8, with a fixed factorial exponent. The source-normal-form support and its later Neumann application are separate C07 statements; they are not inputs to the pointwise proof of (C6.2).

The constants may depend on the fixed group, block factors, localization parameters, source-profile exponents and the chosen positive rates. They do not depend on a particular retained history. The original construction/AF hypotheses are not proved by C6.7.

## 2. Coordinates, principal matrix, and actual heterogeneous admission

Fix a current scale \(k\), an admitted retained datum \(v\), and a history/chart branch. Let \(I\) be the current-unit independent free bonds in the regular inner region. Earlier-layer fields are retained parameters; they are not additional coordinates in this Hilbert space. With the fixed Lie-algebra norm,

\[
\|z\|_2^2=\sum_{i\in I}|z_i|^2,\qquad
P_k=A_1\ell_k^{p_0},\quad \ell_k=\log g_k^{-2}.
\tag{C6.6}
\]

The exact free-coordinate precision is

\[
K_{k,v}=C_{k,v}^{*}\Delta_v^{(k)}C_{k,v},\qquad
K_\Lambda=(K_{k,v})_{II}.
\tag{C6.7}
\]

The map \(C_{k,v}\) is formed on the full source fluctuation region before conditioning. Taking the principal block in (C6.7) does not re-solve the constraint on the smaller interior. In particular, a free bond whose constraint image contains a neighboring exceptional bond is still represented by the same \(C_{k,v}\).

The matrix \(\Delta_v^{(k)}\) includes the quadratic constraint-current term in CMP99 (3.156). Removing that term changes the principal form. CMP99 p.428, immediately after (3.158), gives a positive lower bound for \(C^*\Delta_k C\), independent of scale and the admitted background, and its uniform exponential locality. The statement is made for arbitrary backgrounds satisfying (3.35)–(3.36) with the prescribed smallness, not only for \(U=1\). Theorem 3.15/(3.187), p.432, supplies the associated actual constrained propagator and localized expansion.

Annex AI, HC.5–HC.10, checks the application to the present class. The regular region lies farther than the fixed propagator range from the bad complement once the running collar exceeds that fixed range. CMP102 Theorem 1, (9)–(10), supplies the second-order local-background bound required by CMP99 (3.36). A plaquette or first-gradient bound alone would not establish that admission. The exceptional linear-constraint block stays uniformly invertible on the fixed local chart.

Consequently, for fixed constants independent of the retained history,

\[
K_\Lambda\ge\lambda_0 I,\qquad
\|(K_\Lambda)_{ij}\|_{\rm op}\le K_0e^{-\delta_K\rho_k(i,j)}.
\tag{C6.8}
\]

These facts are principal Gaussian coefficient theorems, established before any interacting covariance theorem. Principal restriction preserves both bounds. There is no identity-background replacement.

For block matrices define

\[
\|A\|_\beta=\max\left\{
\sup_i\sum_j e^{\beta\rho_k(i,j)}\|A_{ij}\|_{\rm op},
\sup_j\sum_i e^{\beta\rho_k(i,j)}\|A_{ij}\|_{\rm op}
\right\}.
\tag{C6.9}
\]

On the current four-dimensional lattice,

\[
S_t:=\sup_i\sum_j e^{-t\rho_k(i,j)}<\infty,\qquad t>0,
\tag{C6.10}
\]

uniformly under restrictions and periodic volume changes. One may bound this by the number of bond orientations times a fixed multiple of \((1+2/(e^t-1))^4\). Shortest periodic representatives prove the same estimate on a torus. All counting here is in current units.

## 3. The OR.19 polynomial is used only for the ordinary phase

### 3.1 An explicit profile dictionary

Keep four separate exponents:

\[
\begin{split}
q_{\rm tar}&=q,\\
q_{\rm val}&=q_{\rm tar}+Q_1,\\
q_{\rm phase}&=q_{\rm val}+Q,\\
q_{\rm prim}&=q_{\rm phase}+D_{\rm prep}+2.
\end{split}
\tag{C6.11}
\]

The target native radius is \(g_n\ell_n^{q_{\rm tar}}\); the maintained value chart uses \(g_n\ell_n^{q_{\rm val}}\). The enlarged ordinary phase chart uses \(g_n\ell_n^{q_{\rm phase}}\), and the primitive chart leaves the further preparation reserve shown in (C6.11). Thus the base exponent in SR.12 is read as \(q_{\rm val}\) for this application. One must not compare the phase chart to a value chart whose existing \(Q_1\) enlargement has been omitted.

The exponents \(q_{\rm tar},Q_1,D_{\rm prep},D_E\) are fixed before \(Q\). Constants and fixed age-polynomial degrees may depend on the once-selected \(Q\). The fixed powers of \(\ell_r\) in the ordinary bound do not acquire an additional \(Q\)-dependence.

### Lemma C6.8: radial phase extraction

Suppose \(F(\zeta;a,x)\) is an ordinary preintegration difference, with the old raw tuple \(x\) and integrated tuple \(a\) fixed, and

\[
\sup_{\mathcal D^{++}}|F|\le C_Q\ell_r^D.
\tag{C6.12}
\]

Assume the actual source-profile comparison gives a radial analytic disk \(t\mapsto F(t\zeta;a,x)\), \(|t|<c\ell_r^{Q-D_{\rm map}}\), for every \(\zeta\in\mathcal D^+\), with the same bound. Then, for \(\ell_r\) sufficiently large,

\[
|F(\zeta;a,x)-F(0;a,x)|
\le C_Q'\ell_r^{D+D_{\rm map}-Q}.
\tag{C6.13}
\]

**Proof.** Write \(f(t)=F(t\zeta;a,x)=\sum_{m\ge0}a_mt^m\). Cauchy on a disk of radius \(R=c\ell_r^{Q-D_{\rm map}}\) gives \(|a_m|\le C_Q\ell_r^D R^{-m}\). For \(R\ge2\),

\[
|f(1)-f(0)|\le C_Q\ell_r^D\sum_{m\ge1}R^{-m}
=\frac{C_Q\ell_r^D}{R-1}
\le\frac{2C_Q}{c}\ell_r^{D+D_{\rm map}-Q}.
\]

There is a single complex variable \(t\); no factor counting raw coordinates, native slots, layers, or current sites appears. The old raw tuple is fixed before the estimate. \(\square\)

The radial disk is the ordinary source chart comparison used in SD.18–SD.27 and OR.20–OR.26. We retain the fixed external-composition loss \(D_{\rm map}\) in OR.22: the usable radial radius is \(c\ell_r^{Q-D_{\rm map}}\). This radius follows from (C6.11), the common fixed primitive margin, the actual external-map bound, and the AF comparison \(\ell_n\ge\ell_r-O(1)\) on the relevant earlier layers. The finite exponent \(D_{\rm map}\) is fixed before \(Q\). Localization variables retain their printed disks; this radial comparison varies the physical/native increment in the ordinary family. It does not enlarge an arbitrary inherited relative input.

SR.24 supplies (C6.12) with \(D=D_E\) for the complete ordinary \(E\) difference, including its literal Wilson subtraction, recent truncated-tensor error, and cutoff residual. The other ordinary sectors have the corresponding already displayed estimates. Set \(D_2\) equal to the maximum of the finite ordinary degrees plus their fixed external-composition losses \(D_{\rm map}\). In particular the ordinary E contribution has degree \(D_E+D_{\rm map}\). Choose once

\[
Q>D_2+2.
\tag{C6.14}
\]

The bound \(C_Q\) need not be uniform as \(Q\to\infty\): \(Q\) is now fixed, and the common weak ceiling is selected afterwards. Equations FP.8–FP.9 then give

\[
\delta_{{\rm ord},r}
\le Cg_r\ell_r^{D_1}
 +C_Q\ell_r^{D_2-Q}
 +Cg_r^{-u}\ell_r^{D_3}e^{-cR_r}
\longrightarrow0.
\tag{C6.15}
\]

The last limit uses \(R_r\ge c_R\ell_r^p\), \(p>1\). For every fixed \(u,D\), \(g_r^{-u}\ell_r^D e^{-cR_r}\) tends to zero as the common coupling ceiling tends to zero. None of (C6.12)–(C6.15) is a bound of order \(P_k^{-2}\) on the complete boundary Hessian.

## 4. Fixed-raw normalization and the positive induction

On the literal source support, after the actual changes of variables have fixed that support, write the complete unrolled density as

\[
W_\zeta(x,a)=W_0(x,a)e^{c_\zeta(x)+\sigma_\zeta(x,a)}.
\tag{C6.16}
\]

The ordinary contribution is (C6.15). The incoming relative part is bounded by FP.10/RL.11,

\[
K_r\le Cg_r^{-u}(1+\ell_r)^D A_{r-1},\qquad
|\sigma_\zeta|\le\delta_r:=\delta_{{\rm ord},r}+2K_r.
\tag{C6.17}
\]

Here \(A_{r-1}\) is the incoming chronological capacity. It is not the output of the step under consideration. The incoming relative action is evaluated once on the unrolled tuple. Intermediate \(C^{(n)}\) generated by the same attempt are the intermediate masses already canceled in the exact product of kernels and final mass; they are not counted again as independent incoming atoms. SD.2–SD.6e gives this identity before fixing any earlier raw variables.

For \(\delta_r\le\delta_*<\pi/4\), the actual normalized density obeys

\[
|p_\zeta(a\mid x)|\le M_*p_0(a\mid x),\qquad
M_*=e^{2\delta_*}\sec\delta_*.
\tag{C6.18}
\]

This is SD.7–SD.14, applied on each fixed raw fiber. Consequently, for nonnegative weights \(w_G\),

\[
\sum_Gw_G\sup_{\zeta\in\mathcal D^+}
 |\Pi_\zeta F_G|
\le M_*\int p_0(da\mid x)
 \sum_Gw_G\sup_{\zeta\in\mathcal D^+}|F_G|.
\tag{C6.19}
\]

The raw supremum is taken after this positive sum. The result is stronger than an operator bound at one parameter value and does not require convexity of an old selector fiber.

The mass remains

\[
\log Z_\zeta-\log Z_0
=c_\zeta+\log\mathbb E_0e^{\sigma_\zeta}.
\tag{C6.20}
\]

In particular, the current/native derivatives of \(c_\zeta\) do not disappear. They remain in the ordinary scalar/source sectors of Section 5. Every archived mass depending on a variable still integrated later stays inside that later density. Differentiation therefore gives the exact covariance term

\[
D\Pi F=\Pi(DF)+\Pi(F\,DH)-\Pi F\,\Pi(DH).
\tag{C6.21}
\]

The nonlinear normalized logarithm has its quadratic cumulant bound FP.17–FP.19; the once-paid linear transport and physical-root construction are FP.14–FP.19b and RL.44. These are necessary C05 inputs. A product of \(M_*\) over all past scales would not prove a uniform result.

With those positive source estimates, the actual recurrence is

\[
A_r\le e^{C\widehat\sigma_r+C d_rA_{r-1}}A_{r-1}+f_r,
\qquad A_{r_0-1}=0,
\tag{C6.22}
\]

and FP.21–FP.24 gives

\[
F_r:=\sum_{b\le r}f_b\le C_1e^{-c_1\ell_r^p},\qquad
C\sum_r\widehat\sigma_r+2C\sum_r d_rF_{r-1}\le\log2.
\tag{C6.23}
\]

Unfolding (C6.22) and using the inductive estimate \(A_{s-1}\le2F_{s-1}\) yields \(A_r\le2F_r\). Thus (C6.17) tends uniformly to zero before the step's output is estimated. The finite induction validates (C6.18) and the output capacity together. It uses no C06 coercivity or C08 covariance estimate.

The role of the two-age calculation is now precise: it supplies the ordinary phase estimate that validates the common positive domination in this already stated C05 induction. It does not replace the separate current-root estimates by a scalar bound.

## 5. The actual current prefactor remains bounded

Let

\[
\theta_k=\ell_k^{p_0-q_{\rm tar}},\qquad
\delta_k=Cg_kP_k,\qquad
D_k\le Cg_k\ell_k^{q_{\rm loc}},\qquad q_{\rm loc}=q_{\rm val}+D_{\rm loc}.
\tag{C6.24}
\]

Here \(D_{\rm loc}\ge0\) is a fixed local full-input conversion loss selected before \(Q\); the literal CE2 estimate permits \(D_{\rm loc}=0\). If a source-coordinate estimate retains an additional fixed logarithmic power, it is included explicitly in \(D_{\rm loc}\). This is a bound on the actual output, not an enlargement of the maintained value chart. It is distinct from the radial external-map loss \(D_{\rm map}\) in Section 3. The phase exponent \(q_{\rm phase}\) in (C6.11) is used for the independently controlled ordinary family; it does not become a history-dependent exponent in the positive relative induction.

The actual current-to-native tangent has the physical \(g_k\) factor and the full field, gradient and current weights. CE4–CE6 gives its first-current factor \(\theta_k/P_k\), with the genuine old port and current attachment joined by their paid carrier. The current root count is performed before collapsing any bounded protected core. The remaining current derivatives use the common current analytic contour. The physical graph and endpoint moments pay the weighted spatial sums. This yields CE21–CE22/FP.2–FP.3, rather than an inference from an unweighted value bound.

The separate positive sector estimate is

\[
\begin{split}
K_{B,k}\le C[&\mathfrak K_E+C_R'g_k^{\kappa_0-11}
 +(B_0+C_0)\theta_k
 +g_k^{-2}D_k^3+D_k\\
&+g_k^{-2}\delta_k(1+\log\ell_k)^{A_\phi}e^{-c_\phi R_k}
 +\theta_kP_k^2(1+\ell_k)^{A_G}e^{-c_GR_k}
 +\theta_k(A_k+\mathcal F_*)].
\end{split}
\tag{C6.25}
\]

This is CE19/FP.26, with the now-established running capacity from (C6.23). The terms are, in order: boundary-assigned \(E/R\), original ordinary \(B\) and pure-prefix \(C_0\), constrained classical and measure remainders, heterogeneous Wilson coefficient, actual old Gaussian/Schur responses, and the relative/failed families. A term that is in a disjoint local family below is removed from this positive sector sum before it is added there; no cancellation between protected internal pieces is undone.

Three points in (C6.25) are essential.

* The pure-prefix ordinary scalar and extracted mass derivatives have their source \(C_0\) sector and actual strip port. Section 3's projective cancellation does not set them to zero.
* The old Gaussian/Schur coefficient has its actual \(P_j^2\) cost. AF comparison converts this to \(P_k^2\) times an age polynomial; the true current collar gives the displayed exponential. One does not replace this interacting density by an untruncated Gaussian law.
* The heterogeneous coefficient retains \(g_k^{-2}\delta_k\), hence a possible \(g_k^{-1}\) loss. Its actual collar supplies \(e^{-c_\phi R_k}\). The smallness is not obtained by discarding the heterogeneous coefficient.

For completeness, each possibly large expression has a direct limit. For fixed \(s\),

\[
g_k\ell_k^s=e^{-\ell_k/2}\ell_k^s\longrightarrow0,
\tag{C6.26}
\]

and for fixed \(u,s,c>0\),

\[
g_k^{-u}\ell_k^s e^{-cR_k}
\le \exp\{u\ell_k/2+s\log\ell_k-cc_R\ell_k^p\}
\longrightarrow0.
\tag{C6.27}
\]

Thus \(g_k^{-2}D_k^3\le Cg_k\ell_k^{3q_{\rm loc}}\to0\), \(D_k\to0\), the heterogeneous term tends to zero, and the Gaussian term tends to zero despite \(P_k^2\). The capacity and failure budget are uniformly bounded; \(q_{\rm tar}>p_0\) makes their \(\theta_k\) factor small. With \(\kappa_0\ge12\), all terms except the fixed finite \(\mathfrak K_E\) tend to zero. Hence

\[
K_B^*:=\sup_{\text{admitted }k,v,\,g_k\le g_*}K_{B,k}<\infty,
\qquad K_{B,k}P_k^{-2}\longrightarrow0
\tag{C6.28}
\]

uniformly at a common sufficiently small ceiling.

This is the required bridge from the C05 argument under CR to a small Hessian. The polynomial \(\ell_r^{D_E}\) from SR.24 is nowhere inserted as \(K_{B,k}\).

## 6. First and second current derivatives, including the fixed matrix

The current chart supplied by FP.1 is \(|z_i|<2P_k\), in the source block norm, with fixed dimensional conversion constants. It contains a simultaneous increment polydisc of radius \(cP_k\) around every point of the full real support \(|z_i|\le P_k\). Old raw variables and history labels are fixed. No shrinkage of the real cutoff is used.

The positive current endpoint theorem CE21–CE22 gives, on an admitted inner chart,

\[
\sup_{v,z,i}\|D_iW_B\|\le C K_B^*P_k^{-1},
\tag{C6.29}
\]

\[
\sup_{v,z}\|D_z^2W_B\|_{\beta_B}
\le C K_B^*P_k^{-2}.
\tag{C6.30}
\]

For \(m\ge1\), the complete current bound is

\[
\sup_{v,z,i_1}\sum_{i_2,\ldots,i_m}
e^{\sigma\tau_k(i_1,\ldots,i_m)/m}
\|D_{i_1}\cdots D_{i_m}W_B\|
\le C^{m+1}(m!)^5K_B^*P_k^{-m}.
\tag{C6.31}
\]

For \(m=2\) a fixed reduction of \(\sigma\) supplies \(\beta_B>0\). The bound is for complete coarsened atoms with their physical footprint costs paid. It is not a norm on individual pieces of a canceled atom. C04 supplies the analogous regular \(E/R\) score and weighted Hessian, DS.9–DS.10, and the corresponding native joint jets.

The remaining local classical and measure terms are evaluated at the **full shifted current input** \(t=z+y\). Their exact analytic localization is supplied by CMP116 (1.37)–(1.40), p.10, and the paragraph immediately preceding Lemma 2. Equation (1.39) is cubic in the unscaled fluctuation after the full constrained quadratic is separated. The local measure logarithms have their local analytic loop expansion; an extensive determinant bound is not used.

On a fixed multiple of the actual current contour, \(g_k\|t\|_\infty\le D_k\to0\). The common native value chart may enlarge \(D_k\) by a fixed logarithmic power. The rooted local prefactor is therefore

\[
K_{{\rm loc},k}\le C\{g_k^{-2}D_k^3+D_k\}\longrightarrow0.
\tag{C6.32}
\]

The contour is uniform around every real support point and uses the actual retained exterior field. Native dependence of that shift is part of the complete analytic composition. Cauchy and the local carrier sum give

\[
\sup_{v,z,i}\|D_iW_{\rm loc}\|\le C K_{{\rm loc},k}/P_k,
\quad
\sup_{v,z}\|D_z^2W_{\rm loc}\|_{\beta_{\rm loc}}
\le C K_{{\rm loc},k}/P_k^2.
\tag{C6.33}
\]

Induced linear and quadratic terms from \(y\ne0\) remain in (C6.32)–(C6.33). A Taylor expansion about \(z=0,y=0\) followed by deletion of those terms would be invalid. For coercivity alone one may instead use the independent fixed absolute-map estimate HC.24,

\[
\|D_z^2W_{\rm loc}\|_\beta
\le C_{\rm cl}'\epsilon+C_{\rm meas}'g_k^2/\epsilon.
\tag{C6.34}
\]

Its parameter order is useful because \(\epsilon\) is fixed before the final \(g_*\). The stronger current-scale score estimate (C6.33) is retained for C08.

Assign the \(E/R\), boundary and local carrier families disjointly, and put \(W=W_{ER}+W_B+W_{\rm loc}\). With \(\beta\le\min(\beta_B,\beta_{ER},\beta_{\rm loc})\), (C6.29)–(C6.33) imply

\[
\sup_{v,z,i}|D_iW(z;v)|\le C/P_k,
\qquad
\sup_{v,z}\|D_z^2W(z;v)\|_\beta\le C/P_k^2.
\tag{C6.35}
\]

These are genuine first- and second-derivative bounds. The first is not deduced from the second.

### Lemma C6.9: a fixed Hessian majorant with an explicit rate loss

For fixed retained \(v\), define

\[
A_{ij}(v)=\sup_{z\in\mathcal U_{k,v}}\|D_iD_jW(z;v)\|_{\rm op},
\tag{C6.36}
\]

where \(\mathcal U_{k,v}\) is the same admitted inner complex chart as in (C6.35). Mixed-derivative symmetry makes this matrix symmetric. Each term of the nonnegative row in (C6.35) gives

\[
A_{ij}(v)\le CP_k^{-2}e^{-\beta\rho_k(i,j)}.
\tag{C6.37}
\]

Therefore

\[
\sup_i\sum_j e^{\beta\rho_k(i,j)/2}A_{ij}(v)
\le CP_k^{-2}S_{\beta/2}.
\tag{C6.38}
\]

The lattice constant is uniform by (C6.10). This proof takes an entrywise supremum only after obtaining each entry's decay, and pays a smaller spatial rate. It does not interchange \(\sup_z\sum_j\) with \(\sum_j\sup_z\) at the original rate. \(\square\)

Equations (C6.35) and (C6.38), in particular at \(z=0\), are the complete score and fixed-Hessian-matrix inputs required by C8A.5–C8A.10. The zero-current point is in the analytic domain even when an earlier selector fiber does not contain zero; no reference raw anchor is changed to zero here.

## 7. Exact conditional potential, force and matrix proof

The C01 normal form gives, up to a \(z\)-independent scalar,

\[
V_{k,v}(z)
=\frac12\langle z,K_\Lambda z\rangle
 +\langle z,K_{IO}y\rangle-W(z;v).
\tag{C6.39}
\]

The exterior \(y\) consists only of the actual retained current exterior coordinates, after their prescribed relocation. Older archived layers are parameters in \(v\), not extra entries of \(y\). The exterior Schur scalar, purely raw masses and native-dependent outer normalizations retain their original outer-law positions. A \(z\)-independent scalar has zero current Hessian but keeps all native derivatives in the unsubtracted native statement.

In (C6.39), the force \(b=-K_{IO}y\) is retained. The actual source support gives \(\|y\|_\infty\le C_yP_k\). If \(d_O(i)=\inf_{j\in O}\rho_k(i,j)\), then (C6.8) and (C6.10) give

\[
|b_i|\le CP_k e^{-\delta_K d_O(i)/2}S_{\delta_K/2}.
\tag{C6.40}
\]

The force can be of order \(P_k\) near the exterior. Its zero current Hessian does not imply a small mean. The C08 mean argument must use (C6.40) as a spatial force profile.

Let

\[
A_K=K_0\sup_i\sum_j\rho_k(i,j)e^{-\delta_K\rho_k(i,j)/2}<\infty.
\tag{C6.41}
\]

Choose a positive rate once so that

\[
\gamma\le\min\left\{\frac{\delta_K}2,\beta,
\frac{\lambda_0}{4A_K}\right\},
\tag{C6.42}
\]

omitting the last term if \(A_K=0\). Choose the absolute local radius \(\epsilon\) so that \(C_{\rm cl}'\epsilon\le\lambda_0/16\). Then reduce the common \(g_*\), while keeping every exponent and rate fixed, so that

\[
\varepsilon_B(g_k)\le\lambda_0/16,\quad
\varepsilon_{ER}(g_k)\le\lambda_0/16,\quad
C_{\rm meas}'g_k^2/\epsilon\le\lambda_0/16.
\tag{C6.43}
\]

The availability of this choice is (C6.28), C04, and the explicit local estimate. All prior source-admission and C05 inequalities are also preserved by a smaller common ceiling. Thus

\[
\eta_\gamma:=\sup_{v,z}\|D_z^2W\|_\gamma\le\lambda_0/4.
\tag{C6.44}
\]

At a real configuration, the Hessian is symmetric. The block Schur test gives \(\|D_z^2W\|_{2\to2}\le\eta_\gamma\). Since

\[
H(z):=D_z^2V(z)=K_\Lambda-D_z^2W(z),
\]

(C6.8) proves (C6.2).

For a real 1-Lipschitz \(f\), set \(D_f=\operatorname{diag}(e^{\gamma f_i})\). Entrywise,

\[
|e^{\gamma(f_i-f_j)}-1|
\le\gamma\rho_k(i,j)e^{\gamma\rho_k(i,j)}.
\]

The two Schur sums and (C6.8) imply

\[
\|D_fK_\Lambda D_f^{-1}-K_\Lambda\|_{2\to2}
\le\gamma A_K\le\lambda_0/4.
\tag{C6.45}
\]

The weighted perturbation has operator norm at most \(\eta_\gamma\). Consequently, for complex vectors \(u\),

\[
\operatorname{Re}\langle u,D_fH(z)D_f^{-1}u\rangle
\ge\frac12\lambda_0\|u\|_2^2.
\tag{C6.46}
\]

Its inverse has operator norm at most \(2/\lambda_0\). Taking \(f_i=\rho_k(i,j)\) for a fixed \(j\), and extracting the \(ij\) block, proves (C6.3). Summing at a smaller rate gives

\[
\|H(z)^{-1}\|_{\gamma/2}\le\frac{2S_{\gamma/2}}{\lambda_0}.
\tag{C6.47}
\]

Every real linear tilt changes \(V\) by a linear function. It changes neither this Hessian nor the support. This proves the coercivity and inverse conclusions of Theorem C6.7.

No support integration by parts has occurred. No identity of \(H(z)^{-1}\) with interacting covariance has been used. In particular the C06 proof has no circular dependence on the downstream C07 support/Neumann theorem.

## 8. The common native/current domain and derivative order

The C04 and repaired C05 current contours have radii which are fixed multiples of \(P_k\) around the entire real current support. The local classical, propagator and exceptional-coordinate maps have fixed absolute unscaled radii. Under the actual input \(g_kz\), their current-coordinate radii are of order \(g_k^{-1}\), not fixed constants in \(z\). Since \(g_kP_k\to0\), these absolute charts do not destroy the \(cP_k\) increment margin at the final ceiling.

Native field and current directions are measured in their original layer-weighted norms. With \(h_n=L^n\eta\), the field norm includes the \(h_n\), \(h_n^2\), and \(h_n^3\) field/gradient/second-order-current weights, and any specified Hölder term. Independent currents retain their own slot. The source C05 reconstructed-output constraints remain part of the domain; a first-gradient norm or an unrestricted old raw ball is not substituted.

In each direction's own normalization choose

\[
r_{\rm joint}=\frac12\min\{r_{ER},r_B,r_{\rm prop},
r_{\rm prop,J},r_C,r_{\rm loc}\}.
\tag{C6.48}
\]

Here the positive fixed propagator and exceptional-block reserves are the HC.26a radii; the C04/C05 reserves are their actual strong-native radii. The minimum is taken after converting each radius to that same slot normalization. This costs fixed constants, not a factor for each layer.

The full unsubtracted native C05 theorem FP.4 and CE24–CE30 keeps \(B_k(0,\xi)\), the current exterior relocation Jacobian in its prescribed convention, old Gaussian/Schur derivatives, and the scalar masses in (C6.20). C04 supplies DS.13–DS.16. The remaining local coefficients are analytic on the same intersection; HC.25 bounds their current derivatives by

\[
m!\,C g_k^{-2}\epsilon^3
\left(\frac{2c_{\mathfrak g}g_k}{\epsilon}\right)^m
e^{-\kappa' d_k(Y)}
\tag{C6.49}
\]

before the rooted carrier sum. The measure terms have the corresponding value prefactor and the same radii. Common Cauchy estimates for the complete analytic compositions retain all nonlinear map and constraint derivatives.

The current \(m\)-jet bound is (C6.31), with fixed factorial exponent five and the divided-tree weight. Native joint jets use the first direction's proper native cell count, FP.4, and fixed factorial growth. There is no claimed undivided-tree bound at every order and no derivative-order-dependent coupling ceiling.

This proves the derivative and domain part of the original C06 statement, as well as its current coercivity part. Differentiating a moving selector, changing a retained-data chart, or applying the result to a merely measurable raw test would be a different task and is not hidden in (C6.48).

## Mathematical dependencies
The following links refer to the accompanying boundary estimates.

1. [Ordinary stopped-density oscillation on mixed scales](ordinary_oscillation.md): SR.12–SR.15d, SR.23a–SR.24, and Section 9. The new ordinary-E bound and source-domain choices.
2. [Complete boundary activities and normalized component induction](boundary_induction.md): FP.1–FP.4, FP.8–FP.13, FP.14–FP.26. The two-age argument replaces the one-age OR.19 derivation.
3. [Stopped densities and projective comparison](stopped_densities.md): SD.2–SD.14. Literal unrolling, final mass, fixed raw fibers and common positive domination.
4. [Direct boundary score and Hessian tests](boundary_derivative_tests.md): DB.5–DB.17, DB.54–DB.63. Exact derivative identities and the distinction between scalar, pointwise-row and fixed-majorant bounds.
5. [Current endpoint estimates for boundary activities](current_endpoints.md): CE4–CE22, CE24–CE30. Genuine current response, Gaussian/Schur \(P_j^2\), complete sector budget and unsubtracted native supplement.
7. Bałaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP **99** (1985), 389–434: (3.35)–(3.38), Section E, (3.155)–(3.158), the paragraph following (3.158) on p.428, and Theorem 3.15/(3.187), p.432. The supplied primary text was checked directly for the actual free-coordinate lower bound and locality.
8. Bałaban, *The Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*, CMP **102** (1985), 277–309: Theorem 1/(9)–(10), and Proposition 9/(190), with the retained C02/PF admission dictionary.
9. Bałaban, *Renormalization Group Approach to Lattice Gauge Field Theories. II. Cluster Expansions*, CMP **116** (1988), 1–22: (1.15)–(1.21), (1.37)–(1.40), p.10, and the paragraph preceding Lemma 2 on p.11. The supplied primary text was checked for the full cubic classical localization and its other fluctuation-action terms.
10. Bałaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP **119** (1988), 243–285: (3.14)–(3.25), pp.268–270, and pp.275–277. Actual whole-current support before the interior/exterior split and the source localizations.

The proof is conditional on the same independently stated source construction and AF trajectory as the original C-series statements. It does not establish Yang–Mills existence, observable transport, or the missing construction of that trajectory.

## 11. Independent conditions of the integrated C-series and C08 application

**C05-to-C06 parameter check.** The integrated distinction between the ordinary phase bound and the final current prefactor is necessary and correctly retained. The fixed external-map loss from OR.22 is kept: the usable radial disk is \(c\ell_r^{Q-D_{\rm map}}\), and the phase exponent is \(D_E+D_{\rm map}-Q\). Equations C6.13–C6.15 retain this loss. The local full-input loss \(D_{\rm loc}\) is a separate fixed conversion in C6.24; neither loss changes the working value chart or depends on history depth. The source rate choices precede the final small physical weights and the common coupling ceiling.

**C08 probability argument.** The following conditions enter the application.

1. The weighted scalar covariance proof works on products of smooth convex factors with facewise boundary conditions. The spatial multiplier is scalar on each Lie-algebra block, hence preserves its tangency condition. Passing the scalar inequalities and their Sobolev norms to the literal balls avoids an unsupported claim about convergence of arbitrary vector-operator boundary domains.
2. The mean interpolation keeps the full force and normalizer. The estimate
   \(M^*\le\mathsf G(|b|+d)+\mathsf GA(M^*+\sigma\mathbf1)\)
   is a positive finite-dimensional inequality; the displayed weighted smallness of \(\mathsf GA\) justifies its resolvent. No extensive force norm or inverse-Hessian covariance identity is used.
3. The cumulant partition telescope is valid after centering the marks. For a fixed pair crossing the cut, merging that pair identifies the relevant coefficient sum with \(c_{m-1}\). There is no extra independent block count. Combining the \(m^2\) crossing-pair count with the displayed \(L^{2m}\) norms gives
   \(m^{m+1}(m-1)!\le e^m(m!)^2\).
   The rooted four-dimensional divided-tree sum adds factorial power five, so the final power seven is fixed.
4. The auxiliary-Gaussian regulator proof uses the joint linear moment-generating bound of the same conditional law; it does not replace that law by a Gaussian. Its determinant bound correctly retains the trace/rank cost and the uncentered version retains the mean cost. In the central quadratic-form formulation the matrix must be **symmetric positive semidefinite**, not merely entrywise nonnegative. The formulation with an arbitrary linear map \(T\) and the positive matrix \(TT^*\) in C8R.2 makes this explicit.
5. The nonlinear local field regulator follows from the actual derivative envelope, a weighted diagonal quadratic form with bounded trace, and the centered coordinate exponential estimate. Only the stated fixed finite stencils are covered.
6. The same-current exterior response keeps the coarse datum and \(K\) fixed by the exact nonlinear constraint identity. Its score includes the order-one principal cross term and the mixed \(W\) derivative. Centering removes only the deterministic score, not the covariance term. The source's real relocation is used at first derivative order; no analytic continuation of its smooth cutoff is asserted.

**Conditional implication.** C06 and C08 apply on the stated source chart provided the complete C05 estimates hold, including CR for the original composed field.
