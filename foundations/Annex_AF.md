# Boundary normalization, current Hessian rows and collar sums

**Annex AF.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 0. Results and hypotheses

This annex proves three analytic reductions and locates a more useful actual source domain for the boundary fluctuation expansion. It does not complete C-05. The missing application is a uniform estimate for the complete actual boundary pullback, including every inherited fluctuation, relocation, independent-current and retained-variable argument, in the current coordinates used by the marked induction.

The new reductions are:

1. a retained-data-dependent boundary constant cancels exactly from a normalized regular conditional law, including all its normalized retained derivatives; the factor remains in the outer marginal;
2. a simultaneous complex polydisc gives a weighted Hessian row bound without the unnecessary number-of-coordinates factor obtained by summing separate pairwise Cauchy estimates;
3. an actual collar factor of the form \(e^{-c R L^a}\) pays dyadic radius losses \(2^{am}\), polynomial carrier multiplicity, and source-order-dependent polynomial age losses within one fixed factorial exponent.

The third statement is deliberately different from the insufficient logarithmic-age suppression diagnosed in Annex Z. Its stronger decay must be established for the actual differentiated terms before using the theorem.

### 1. Primary source conditions

See CMP119, pp. 254, 259, 261–262 and 276–277.

- Formula (2.1) interlaces the domains as \(\Omega_1\supset\Lambda_1\supset\Omega_2\supset\Lambda_2\supset\cdots\). Formula (2.3) names \(Z_j=\Lambda_j^c\).
- The primitive E activities on p.259 use the regular space from the earlier small-field construction. The separate multiscale conditions (2.34)-(2.39), p.261, are introduced for boundary terms. A statement that every primitive E activity itself has the full B-domain definition would conflate these two inputs.
- The B expansion (2.40)-(2.42) retains old fields and history data and has primitive bound \(B_0 e^{-\kappa d_j(X)}\). The source selects this full-tree bound. The weaker component-resummed alternative with \(d_j(X\setminus Z_j)\), discussed on p.262, must not silently replace it in a spatial estimate.
- The localized boundary fluctuation expansion on p.276 is analytic on the explicit product space (3.43), whose current fluctuation factor is \(\sup|A|<C_1p_1(g_k)\) on the displayed free-bond set. Its background factor is the stated enlarged multiscale complex space. This is stronger information than bare membership in an unspecified open set.
- Page 277 assigns an additional \(O(\varepsilon_k)\) to localized B fluctuation terms and explains how minimizing-field decay pays the shrinking dyadic analytic reserve. It also retains the heterogeneous-action and boundary-relocation terms. Extracting a single complete, current-coordinate derivative majorant from all these statements still requires the original indices, resummations, maps and radius costs.

The precise representation in (3.43) concerns the localized action/fluctuation expressions at this stage of the construction. It does not justify assigning its native current radius to every independently transported history observable. It also does not identify the native background coordinates with arbitrary retained variables without a pullback estimate.

The earlier effective-action paper, CMP109, equations (3.9), (3.14)-(3.17), supplies the far-field decay and the native differentiated-insertion contour used by the source argument.

### 2. Remove only the conditional boundary constant

Let \(v\) denote retained data, let \(A\) range over the fixed regular product domain \(D\) of C-07, and let

\[
 r_v(dA)=\mathbf1_D(A)\exp\{L(A,v)+B(A,v)\}\,dA,
 \qquad Z(v)=r_v(1)>0.
 \tag{BD.1}
\]

All other action terms remain in \(L\); \(B\) can be the complete boundary contribution. Fix a reference \(A_*(v)\in D\) for which the displayed quantities exist, and define

\[
 b_*(v)=B(A_*(v),v),\qquad
 \widetilde B(A,v)=B(A,v)-b_*(v),\qquad
 \widetilde r_v=e^{-b_*(v)}r_v.
 \tag{BD.2}
\]

#### Proposition BD.1 -- exact conditional cancellation

The normalized law \(q_v=r_v/Z(v)\) equals \(\widetilde r_v/\widetilde r_v(1)\). For every integrable marked numerator \(F(A,v)\), its conditional expectation is unchanged. Whenever retained derivatives of these equal expressions exist, all orders of their normalized retained derivatives agree as well.

For an outer measure \(\eta(dv)\), the unnormalized retained marginal is

\[
 Z(v)\eta(dv)
 =e^{b_*(v)}\widetilde r_v(1)\eta(dv).
 \tag{BD.3}
\]

Thus this operation does not delete \(b_*\) from the full law.

**Proof.** Both numerator and denominator of every conditional expectation acquire the same nonzero scalar factor \(e^{-b_*(v)}\), so it cancels. Differentiation preserves the resulting exact equality whenever the chosen derivatives are justified. Equivalently, in a finite source-jet algebra, an invertible scalar series cancels algebraically, without an analytic convergence assumption. Formula (BD.3) follows by integrating (BD.2). \(\square\)

In a smooth fixed chart the normalized score is

\[
 \partial_a(L+B)-q_v\partial_a(L+B)
 =\partial_a(L+\widetilde B)
       -q_v\partial_a(L+\widetilde B).
 \tag{BD.4}
\]

This observation allows conditional estimates to be phrased in terms of the actual boundary fluctuation difference. Retained-only factors remain in the outer history law, and their cumulants are still part of H-03/H-05. If the live geometry changes across an interface, this smooth-chart identity does not remove the two-sided interface current from Annex AA. No global positivity or phase property is inferred from this cancellation.

### 3. A simultaneous contour gives a sharper Hessian budget

Let \(f\) be holomorphic and bounded in modulus by \(M\) on the polydisc

\[
 \mathcal P(z,r)=
 \{z+\zeta:|\zeta_j|<r_j\text{ for every }j\in I\},
 \qquad r_j>0.
 \tag{BD.5}
\]

The coordinates here are scalar complex coordinates. A fixed finite Lie-algebra block dimension changes only the constants, as explained below.

#### Theorem BD.2 -- one anchored row without a carrier-volume loss

For every \(i\in I\),

\[
 \sum_{j\in I}r_j
       |\partial_i\partial_j f(z)|
 \le \frac{4M}{r_i}.
 \tag{BD.6}
\]

Consequently, for positive coordinate weights \(\omega_i\) and any nonnegative spatial weights \(w_{ij}\),

\[
 \sum_j\frac{w_{ij}}{\omega_i\omega_j}
       |\partial_i\partial_j f(z)|
 \le
 \frac{4M}{\omega_i r_i}
       \max_j\frac{w_{ij}}{\omega_jr_j}.
 \tag{BD.7}
\]

**Proof.** Choose phases \(u_j\) with \(|u_j|=1\) so that every nonzero number \(u_j\partial_i\partial_jf(z)\) is real and nonnegative. For \(|t|,|s|<1\), the function

\[
 F(t,s)=f\!\left(z+\tfrac12r_it e_i
                      +\tfrac12s\sum_jr_ju_je_j\right)
 \tag{BD.8}
\]

lies in (BD.5), including when the two variations affect coordinate \(i\). The two-variable Cauchy estimate gives \(|\partial_t\partial_sF(0,0)|\le M\). Its derivative is

\[
 \partial_t\partial_sF(0,0)
 =\tfrac14r_i\sum_jr_ju_j\partial_i\partial_jf(z).
\]

The choice of phases proves (BD.6); multiplying by the maximum displayed in (BD.7) proves the second claim. Boundary radii are obtained as limits from smaller discs. \(\square\)

This is stronger than summing the separate estimate \(2M/(r_ir_j)\) over \(j\). It uses a **simultaneous** contour: a collection of two-coordinate discs does not suffice for (BD.8).

For Lie-algebra blocks choose a fixed scalar basis and its norm-equivalence constants. Apply (BD.6) to each output component and each input component, reducing each scalar radius by the fixed amount needed to remain inside the block ball. Summing over the fixed number of components yields

\[
 \sum_j\frac{w_{ij}}{\omega_i\omega_j}
       \|D_iD_jf(z)\|_{\rm op}
 \le
 \frac{C_GM}{\omega_ir_i}
       \max_j\frac{w_{ij}}{\omega_jr_j}.
 \tag{BD.9}
\]

Here \(C_G\) depends on the fixed gauge group and chosen block norms, not on the number of bonds, carrier size or torus volume.

#### Application to a native boundary vertex

For a localized vertex \(b_{k,Y}(A;U,J,\mathbf A_{\rm old})\) on the source domain (3.43), keep its native background arguments in that domain. Suppose its source bound on that domain is \(M_{k,Y}\). At a real current field with

\[
 \sup_{i\in I_Y}|A_i|\le P_k<R_k^{A},
 \quad R_k^{A}=C_1p_1(g_k),
 \quad \rho_k=R_k^{A}-P_k>0,
 \tag{BD.10}
\]

the actual translated current polydisc has radius \(\rho_k\). Formula (BD.9), with \(w_{il}=e^{\gamma d(i,l)}\), gives

\[
 \sum_l e^{\gamma d(i,l)}
       \|D_iD_l b_{k,Y}(A)\|_{\rm op}
 \le C_GM_{k,Y}\rho_k^{-2}
       e^{\gamma\operatorname{diam}(I_Y)}.
 \tag{BD.11}
\]

The same source domain gives all finite current-direction derivatives by multivariable Cauchy, with the usual \(m^m\le e^m m!\) factor. This does not imply a dimension-free absolute sum of every order-\(m\) tensor coefficient. The row argument works because all but one index form a linear functional after fixing the first index. General higher-order absolute coefficient sums require their own localization or tensor norm.

The still-required normalization check in (BD.10) is explicit. The literal cutoff symbol in CMP119 (3.16) and the preceding rescaling must be reconciled before declaring a lower bound for \(\rho_k\) on the entire actual support. Using \(P_k=\delta_k\) in one formula and \(P_k=\delta_k/g_k\) in another would be invalid.

The source comparison makes this issue more specific. CMP119 after (3.4), p.265, defines the unprimed cutoff using \(p_0(g_k)\). The smaller polynomial introduced for a **primed** preparation selector in LFR I is a different quantity. The printed \(p_1(g_k)\) in CMP119 (3.43) has not been identified here with either quantity by a verified dictionary. One must not import the sharper primed-selector radius for the full original cutoff. If one were to identify the native radius with \(C\ell^{p_1}\) and the normalized original cutoff with \(A\ell^{p_0}\), where \(p_1<p_0\) and \(\ell=\log g^{-2}\), then

\[
 \frac{C\ell^{p_1}}{A\ell^{p_0}}
 =\frac CA\ell^{-(p_0-p_1)}\longrightarrow0.
 \tag{BD.10a}
\]

No fixed enlargement of \(C\) would produce a uniform margin in that identification. This is a test of the proposed identification, not a claim that the source construction has been disproved. The alternatives are a correct polynomial dictionary or a new quantitative admission argument using the underlying fluctuation theorem. Annex AD records the sharper remaining comparison.

### 4. Carrier sums and the complete current Hessian

Suppose a current-scale expansion has actual vertices \(b_{k,Y}\), all with the current radius \(\rho_k\), such that

\[
 M_{k,Y}\le K_k e^{-\kappa n(Y)},\qquad
 \operatorname{diam}(I_Y)\le c_d n(Y),
 \tag{BD.12}
\]

and, for every fixed current bond \(i\), at most \(C_D A_D^n\) of the carriers containing \(i\) have integer size \(n\ge1\). If

\[
 \delta=\kappa-c_d\gamma-\log A_D>0,
 \tag{BD.13}
\]

then (BD.11) proves

\[
 \sup_i\sum_l e^{\gamma d(i,l)}
 \left\|D_iD_l\sum_Yb_{k,Y}\right\|_{\rm op}
 \le
 \frac{C_GC_DK_k}{\rho_k^2}
       \frac{e^{-\delta}}{1-e^{-\delta}}.
 \tag{BD.14}
\]

**Proof.** Sum (BD.11), first over carriers at fixed size and then over \(n\). The scalar series is geometric by (BD.13). All constants are independent of the total number of bonds. \(\square\)

For nearest-neighbor connected cell carriers a crude exponential counting constant follows by recording a depth-first traversal of a spanning tree, with a number of possible steps bounded by the fixed lattice degree. More general source domains must be counted in their actual cell convention. One cannot assign this counting constant to an arbitrary collection of resummed or component-contracted carriers without checking that convention.

For the B-origin fluctuation terms the source's additional \(O(\varepsilon_k)\) is potentially the factor \(K_k\) in (BD.12). This identification must include the complete sum over old terms and the actual localization constants. The heterogeneous-action and relocation contributions require the same check; the displayed inequality does not assert that their constants already equal those of a single primitive B vertex.

For a pullback not already included in the native expansion, one still has

\[
 D^2(b\circ\Phi)
 =D^2b(\Phi)[D\Phi,D\Phi]+Db(\Phi)D^2\Phi.
 \tag{BD.15}
\]

The second term remains. A direct native estimate (BD.11) is useful precisely when the source has already performed that pullback and supplied its joint norm; it cannot be transported to a different coordinate system by changing its name.

### 5. What a genuine collar gain pays at every source order

#### Lemma BD.3 -- elementary scaled collar geometry

Let the physical cell sizes be \(h_j=L^ja\), with \(L>1\). Suppose a current support point \(x\) lies at physical distance at least \(bRh_k\) from \(Z_k\), and \(Z_j\subset Z_k\) for \(j\le k\). Every connected tree meeting both \(x\) and \(Z_j\) has length in \(j\)-scale units at least

\[
 bR\frac{h_k}{h_j}=bR L^{k-j}.
 \tag{BD.16}
\]

**Proof.** A connected tree joining the two sets has physical length at least their distance. Nested bad regions give \(\operatorname{dist}(x,Z_j)\ge\operatorname{dist}(x,Z_k)\). Divide by \(h_j\). The same proof applies with the torus metric whenever the stated collar exists. \(\square\)

The interlacing of source domains supplies the nesting. The current collar and the tree connecting the *actual differentiated influence* to the old boundary must still be identified in the localized expression. A native vertex's nominal label is not such a tree when an unlocalized minimizing-field map remains attached to it. Derivatives of a localization or preparation factor must retain their own connecting paths.

#### Theorem BD.4 -- dyadic radius losses with a collar factor

Fix \(L>1\), \(c>0\), \(d,\sigma,\eta\ge0\), \(A\ge1\), and \(p\ge0\). Put \(\beta=\log 2/\log L\). Suppose nonnegative terms, for integers \(a\ge0,m\ge1\) and \(R\ge1\), satisfy

\[
 T_{a,m}(R)
 \le A^{m+1}(m!)^p\rho^{-m}
       2^{am}L^{da}(1+a)^{\sigma m+\eta}
       e^{-cRL^a},\qquad \rho>0.
 \tag{BD.17}
\]

For every \(\epsilon>0\) there is a constant \(C_\epsilon\), depending only on the fixed displayed parameters and \(\epsilon\), such that

\[
 \sum_{a\ge0}T_{a,m}(R)
 \le C_\epsilon^{m+1}
       (m!)^{p+\beta+\epsilon}\rho^{-m}e^{-cR/2}.
 \tag{BD.18}
\]

If \(\sigma=0\), one may take \(\epsilon=0\).

**Proof.** If \(\sigma>0\), the elementary exponential-versus-polynomial bound gives

\[
 (1+a)^\sigma\le K_\epsilon L^{\epsilon a}
 \quad(a\ge0).
 \tag{BD.19}
\]

If \(\sigma=0\), use \(K_0=1\) and no additional power. Similarly \((1+a)^\eta\le K L^a\). With \(b=\beta+\epsilon\), or \(b=\beta\) when \(\sigma=0\), it suffices to bound

\[
 \sum_{a\ge0}(L^a)^{s}e^{-cRL^a},
 \qquad s=d+1+bm.
 \tag{BD.20}
\]

Split the exponential into factors of relative weights \(1/2,1/4,1/4\). Since \(L^a\ge1\), the first factor is at most \(e^{-cR/2}\). For the second factor,

\[
 \sup_{x\ge0}x^se^{-cRx/4}
 =\left(\frac{4s}{ecR}\right)^s
 \le \left(\frac{4s}{ec}\right)^s.
 \tag{BD.21}
\]

The sum of the remaining factors is bounded by

\[
 \sum_{a\ge0}e^{-cL^a/4}
 \le \frac{e^{-c/4}}{1-e^{-c(L-1)/4}},
 \tag{BD.22}
\]

because \(L^a\ge1+a(L-1)\). Finally, for fixed \(d,b>0\),

\[
 s^s\le C^{m+1}(m!)^b.
 \tag{BD.23}
\]

To verify this last step, write \(s=bm+D\), with fixed \(D=d+1\). The factor \((1+D/(bm))^{bm+D}\) is uniformly bounded up to a fixed constant; the remaining factor is a constant to the power \(m\), times \(m^{bm+D}\). Use \(m!\ge(m/e)^m\) and absorb the fixed power \(m^D\) into another constant to the power \(m\). Combining these bounds proves (BD.18). \(\square\)

Thus a verified dyadic radius loss does not by itself destroy the fixed OS factorial budget when it is paired with this stronger physical collar decay. The theorem retains the common current radius \(\rho^{-m}\); it has not proved that this radius has the required physical scaling. It also does not supply (BD.17) for every boundary response. Source-order growth of the preparation maps and carrier multiplicity must be included in the parameters before applying it.

### 6. Application conditions

The current proof obligation for C-05 can now be stated more economically, without discarding any term:

1. identify the complete native boundary fluctuation expansion in the actual free current variable, resolving its normalization and giving a positive uniform reserve in (BD.10);
2. prove the fully resummed anchored majorant (BD.12), or a directly sufficient weighted sum, for B-origin, heterogeneous-action and relocation terms together;
3. verify the pullbacks of all independently extended current and retained-data derivatives, including both terms of (BD.15);
4. retain outer boundary factors and live-history interface currents in the full law, where Proposition BD.1 does not eliminate them.

The first source domain is now explicit, and the analytic and summation implications needed after these checks are proved. Their actual joint hypotheses have not all been verified. **C-05 therefore remains open under its unchanged hypotheses.**

### 7. References

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, Communications in Mathematical Physics **119** (1988), 243-285. pp.254, 259, 261-262, 276-277; equations (2.1), (2.28), (2.34)-(2.42), (3.43).
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. I. Generation of Effective Actions in a Small Field Approximation and a Coupling Constant Renormalization in Four Dimensions*, Communications in Mathematical Physics **109** (1987), 249-301, equations (3.9), (3.14)-(3.17). DOI: https://doi.org/10.1007/BF01215223.

All new propositions above are proved in this note. Source-specific estimates are imported only in the scopes described in Section 1. No inaccessible announced Yang-Mills proof is used.

### Supplement AF.1: Weighted layer geometry and the actual local averaging response


#### 1. The metric is specified in the primary source

The weighted distance used in CMP99 and CMP102 is the distance defined in CMP96, p.231, **(2.46)**. The reference to (2.36) in CMP99's discussion after (3.41) is an indexing error: (2.36) in CMP96 is not the metric definition. See CMP96, pp. 224 and 231–234.

Write \(h_r=L^r\eta\), let \(\Omega_0\supset\cdots\supset\Omega_K\) be the admitted determining geometry, and put
\(A_r=\Omega_r\setminus\Omega_{r+1}\), with \(\Omega_{K+1}=\varnothing\). In CMP96 (2.2) the separation condition is

\[
 \operatorname{dist}(\Omega_r^c,\Omega_{r+1})>RMh_r.
 \tag{BM.1}
\]

The fixed \(RM\) here is the separation parameter of the admitted propagator geometry. It is not an old-scale Euclidean tree distance and need not be identified with a running \(R_r\).

For determining-block centers \(y,y'\), the actual metric is

\[
 d_\Omega(y,y')
 =\inf_\Gamma\sum_{r=0}^K h_r^{-1}|\Gamma\cap A_r|,
 \tag{BM.2}
\]

with the source's admissible paths and block-center convention. The source extends the metric to fine points by assigning their determining-block centers. The conclusions below allow the resulting fixed endpoint offsets. The actual complete construction invokes the propagator/minimizer results only on their admitted determining geometries; (BM.1) is retained as that primary hypothesis. This does not assert that every arbitrary interlaced family satisfies it.

#### 2. Layer separation and the row bound

##### Lemma BM.1 — weighted age separation

If \(y\) belongs to layer \(n\) and \(y'\) belongs to layer \(k\), then

\[
 d_\Omega(y,y')\ge RM(|k-n|-1)_+.
 \tag{BM.3}
\]

**Proof.** Decompose an admissible path at the interfaces \(\Sigma_r=\partial\Omega_r\), exactly as in CMP96 (2.47)–(2.48). A passage between successive distinct interfaces \(\Sigma_r\) and \(\Sigma_{r+1}\) lies in layer \(r\). Its length is at least the separation in (BM.1); dividing by \(h_r\) gives at least \(RM\), as displayed in source (2.57). A path between layers \(n\) and \(k\) has at least \((|k-n|-1)_+\) such complete passages. Repeated exits, re-entries and detours add nonnegative length. Taking the infimum proves (BM.3). \(\square\)

For any fixed kernel rate \(\delta>0\), split an endpoint exponential into two halves and use Lemma 2.1 of CMP96 for the remaining row sum. With \(RM\) satisfying that lemma's fixed-parameter requirement,

\[
 \sup_{y\in A_n}\sum_{y'\in\Gamma_k}
       e^{-\delta d_\Omega(y,y')}
 \le C_{\rm row}(\delta/2)
       e^{-\frac12\delta RM(|k-n|-1)_+}.
 \tag{BM.4}
\]

The sum is over determining-block centers, in the source convention. Formula (2.58) proves the uniform row sum by counting interface passages and spatial lattice steps; (2.59) pays that counting. In the source normalization it suffices to require, for the appropriate fixed \(0<a<1\),

\[
 \tfrac14a\delta_0RM
 >2d\log c_0(a/2)+\gamma+1.
 \tag{BM.5}
\]

The proof then retains a prescribed fixed age rate \(\gamma\). Alternatively, (BM.4) retains the rate \(\delta RM/2\) once its row condition is met. There is no intrinsic limit at the rate one displayed in the source's convenient final choice. One can fix
\(\gamma>4\log L+\log2+2\) if a subsequent activity sum needs the extra four-dimensional count. For the normalized single-map row alone, \(\gamma>\log2\) is sufficient.

The source permits the fixed geometric parameters to be chosen sufficiently large. The propagator rate can be fixed positively before this enlargement; CMP99's random-walk construction retains a fixed rate below that of its local propagators. The small-coupling ceiling can subsequently be reduced to meet the remaining fixed-parameter requirements. No choice here depends on observable order or total depth.

#### 3. Normalized minimizing-map outputs

CMP102 (190) bounds the derivative of the actual relative minimizing map in five output norms. On output layer \(n\), their scale factors are

\[
 h_n^{-1},\quad h_n^{-2},\quad
 h_n^{-2-\beta},\quad h_n^{-3},\quad h_n^{-3},
 \tag{BM.6}
\]

and on an input layer \(k\) the kernel contains the factor \(h_k^{-d}\). The input integration/summation measure is \(h_k^d\); these factors cancel. After multiplying by the output normalization in (BM.6), the remaining kernel is bounded by a fixed multiple of \(e^{-\delta d_\Omega}\). Consequently, for input \(B\) supported on layer \(k\),

\[
 \|D\mathcal H(B_0)[B]\|_{{\rm norm},n}
 \le C_H\|B\|_\infty
       e^{-\gamma(|k-n|-1)_+}.
 \tag{BM.7}
\]

Here \(B_0\) is any actual admitted background input in the smaller absolute map domain, and \(\|\cdot\|_{{\rm norm},n}\) denotes the physically normalized output norms supplied by (190). The corresponding covariant Laplacian/projection combinations used in CMP109 (3.14) are controlled by the stated propagator identities and their kernel bounds; they are not obtained by dilating a projection defined on another determining geometry. The bound is uniform in the admitted remaining history. It does not require \(B_0=0\).

The normalized row estimate has **no** factor \(L^{d(k-n)}\). The cancellation of input cell volume and the source's weighted row sum are the reasons. If a later sum over activity carriers contributes such a factor, it must be charged separately; (BM.5) allows a fixed larger rate for that purpose.

##### Preparation parameters

The same argument can retain a fixed positive spatial rate after the actual complex preparation. CMP116 (1.7) contains both a walk-localization exponential and an endpoint exponential. The estimate (1.11) uses the former to pay the complex decouplings. Taking \(M\) so that the displayed \(\delta_1M\) condition has a strict factor-of-two reserve leaves an endpoint rate \(\delta_*>0\), with the fixed norm loss \(e^{16\kappa_1}\). All source output norms are included in (1.7).

For completeness, the nonlinear step can be made in the weighted norm

\[
 \|A\|_{w,S}=\sup_y e^{\delta_*d_\Omega(y,S)}
                |A(y)|_{\rm normalized},
 \tag{BM.8}
\]

and the corresponding derivative/Hölder norms. The triangle inequality makes each prepared propagator bounded in this norm after reserving part of its endpoint exponential for the row sum. The actual nonlinear terms in CMP116 (1.3)–(1.4) and (1.17) are local analytic operations and the displayed propagator compositions. In a difference of two nonlinear expressions, place the weight on the one differing factor and bound the other factors in the ordinary small norm. The local operations have bounded weighted diameter on their proper-scale blocks, giving only a fixed factor \(e^{\delta_*D_{\rm loc}}\). Their weighted Lipschitz constant is therefore bounded by

\[
 C_{\rm nl}e^{\delta_*D_{\rm loc}}K_w^{r}\epsilon,
 \tag{BM.9}
\]

for a fixed finite \(r\), where \(K_w\) is the prepared weighted propagator norm and \(\epsilon\) is the source's ordinary map-input ceiling. The analytic nonlinear remainders entering the contraction start at degree at least two. The explicitly linear source terms, including the \(G\Delta^{(2)}H_0B\) forcing in CMP102 (180), are retained separately and obey the same weighted propagator estimate with their source coefficient bounds; they are not falsely declared quadratic. Reduce that fixed ceiling until (BM.9) is at most \(1/2\). The actual contraction proof then holds in the weighted norm, and its resolvent costs at most two. This proves the analogue of (BM.7) for the actual prepared nonlinear map, with a fixed changed constant and rate. It does not presume that a bound in an unweighted norm automatically implies spatial decay.

The local constraint map \(g_kCz-hD(g_kCz)\) enlarges the support of a current variation by only its source proper-scale stencil. If that stencil stays in the same deepest determining layer, (BM.7) applies directly. A fixed adjacent-layer enlargement changes \((k-n-1)_+\) to \((k-n-c_0)_+\), with a fixed integer \(c_0\). The actual current collar admits such an enlargement; this support check cannot be replaced by merely naming a current carrier.

For a current variation on its actual deep support, the resulting bound is

\[
 \|\delta\mathcal H_k\|_{{\rm norm},n}
 \le C_{\rm prep}g_k\|\delta z\|_\infty
             e^{-\gamma(k-n-c_0)_+}.
 \tag{BM.10}
\]

Integrating the derivative along an admitted current segment gives the same bound for the finite difference from a reference current field. In particular, it is appropriate for the exact boundary fluctuation difference of BD.1; no source-free boundary constant is removed from the outer marginal.

#### 4. The basic current and the dyadic reserve

Let \(u_n\) be the right side of (BM.10). The exact local-current estimate LC.17 gives, in physically normalized layer units,

\[
 \|\delta J\|_{{\rm norm},n}
 \le C\bigl[u_n+\alpha_{0,n}u_n+u_n^2+u_n^3\bigr].
 \tag{BM.11}
\]

The terms \(\Delta A\) and \(PA\) use the normalized second-order output bounds. For example \(h_n^3b_n|A|\le C\alpha_{0,n}u_n\), and \(h_n^3|A||\nabla A|\le u_n^2\). Thus no power of the fine spacing is hidden in (BM.11). The plaquette and relative-first-difference clauses have the same linear bound with higher powers of \(u_n\) absorbed at a fixed small ceiling. This covers the **basic** field/current clauses on the original geometry, including the independent-current extension used in the local source formula.

For an old boundary activity of birth scale \(j\le k\), the coefficient gap between its domain and the current \(k+1\) domain in CMP119 (2.34)–(2.39) is

\[
 \beta\bigl(2^{-(j-n)}-2^{-(k+1-n)}\bigr)\alpha_{i,n}
 \ge\frac\beta2\,2^{-(j-n)}\alpha_{i,n},
 \qquad n\le j.
 \tag{BM.12}
\]

Using \(\alpha_{0,k}/\alpha_{0,n}\le C_{\rm AF}\sqrt{1+k-n}\), the ratio of (BM.10) at \(\|\delta z\|\le CP_k\) to the right side of (BM.12) is at most

\[
 C\ell_k^{p_0-q}\,
       2^{j-n}\sqrt{1+k-n}\,
       e^{-\gamma(k-n-c_0)_+}.
 \tag{BM.13}
\]

For fixed \(\gamma>\log2\), its age supremum is finite. One fixed small-coupling ceiling therefore gives a strict common current contour for these original-geometry output clauses, before any source differentiation. This is the valid use of exponential age suppression. An order-\(m\) derivative is not first charged \(2^{m(k-n)}\) and then incorrectly paid by one fixed exponential rate.

#### 5. A separate current collar, when its anchor is present

The current construction in CMP119 (3.2)–(3.5) separates the current forcing support from \(Z_k\) by a physical collar of width at least \(c_{\rm col}MR_{k+1}h_k\), after the fixed stencil enlargement. Let an old boundary carrier \(X\) of scale \(j\le k\) meet \(Z_j\subset Z_k\), and let \(x\in X\) be the point at which its argument responds to the current forcing \(S\). Because every weight in (BM.2) is at least \(h_k^{-1}\), while source \(d_j(X)\) is the old tree length divided by the block side \(M\), and \(h_j\le h_k\),

\[
 d_\Omega(x,S)+C_{\rm tree}M d_j(X)
 \ge c_{\rm col}MR_{k+1}-C_{\rm end}M.
 \tag{BM.14}
\]

**Proof.** Choose a boundary anchor \(y\in X\cap Z_j\). The first distance bounds \(\operatorname{dist}_{\rm phys}(x,S)/h_k\), up to the fixed endpoint convention. The carrier tree bounds \(\operatorname{dist}_{\rm phys}(x,y)/h_k\) by \(C_{\rm tree}M L^{j-k}(d_j(X)+1)\), hence by \(C_{\rm tree}M(d_j(X)+1)\). This factor \(M\) follows from the tree-distance normalization in CMP109, immediately before (0.24). The physical triangle inequality bounds their sum below by the stated separation of \(S\) and \(Z_k\), divided by \(h_k\). \(\square\)

Splitting the endpoint and carrier exponentials into fixed fractions therefore retains an additional factor \(e^{-c_{\rm eff}R_{k+1}}\), with \(c_{\rm eff}\) proportional to \(\min\{\delta M,\kappa\}\) up to fixed geometric constants, while leaving a positive age rate and a positive carrier decay rate. Equivalently one may write \(e^{-cMR_{k+1}}\) only with \(c\) allowed to depend on \(M^{-1}\). Fixed \(RM\) can be enlarged after this splitting so that the remaining age rate still satisfies the desired inequality in (BM.5). This does not substitute an ordinary old-scale tree distance for \(d_\Omega\), and it does not claim a collar factor for an arbitrary output point with no boundary anchor.

#### 6. The exact part not proved here

The full B domain also contains the reconstructed pair

\[
 U_{p,X}(M^\bullet(U))
 =U\bigl(B_p(X)\cup\{\Gamma_i\}_{i<p},M^\bullet(U)\bigr),
 \qquad J_{p,X}(M^\bullet(U)).
 \tag{BM.15}
\]

The current restriction in CMP119 (2.37) has the exact weight

\[
 \alpha_{0,n}L^{n-\min\{p,n\}}
                   (L^nL^{-p})^{-3}.
 \tag{BM.16}
\]

For \(n>p\), this is proportional to \(\alpha_{0,n}L^{-2(n-p)}\). A generic relative-potential input estimate gives only one improved scale power and is not enough. The reconstruction must preserve the smoother layer's curvature/difference input, giving the two-power bound, on the changed determining geometry and with the independent-current extension retained.

Two further checks are therefore not consequences of (BM.3) alone:

1. the compatible determining-set union in (BM.15) must preserve or dominate the original weighted geometry in the kernel compositions actually used, or its geometry must be estimated directly;
2. the reconstructed pair must obey (BM.16), and the corresponding curvature bound (2.35), with the same layerwise exponential response and preparation reserve.

The source's localized determining set in (2.14) and the reconstruction union in (2.35) are not silently identified. A purely formal mesh-cap argument which discards overlapping fine constraints is not used. The normalized row theorem proves the original minimizing-map response and resolves the previous metric ambiguity; it does not by itself complete this reconstructed tuple or the separate relocation/value-majorant estimates of C-05.

#### 7. Local two-power averaging gain

The local nonlinear averaging part of the \(n>p\) difficulty can be settled without assuming a property of the changed minimizing geometry.

##### Lemma BM.2 — an actual local averaging response

Let \(h_p\le h_n\), and let a cube of physical side \(C_bh_p\) contain all bonds used in one fixed family of the actual \(p\)-scale averages. Write \(\eta\) for the underlying fine spacing. Suppose on this cube that \(U_0\) is a compact-group field multiplied by a complex relative field of size at most \(C a/h_n\), its plaquette curvature is bounded by
\[
 \|dU_0-I\|\le C a\eta^2h_n^{-2},
 \tag{BM.17}
\]
and \(U_1=e^{i\eta A}U_0\) with
\[
 \|A\|\le u h_n^{-1},\qquad
 \|\nabla_{U_0}A\|\le u h_n^{-2},\qquad
 0<u\le c_a a.
 \tag{BM.18}
\]
Here \(a\) is below one fixed small ceiling and \(c_a>0\) is a sufficiently small fixed number. Let \(g_t\) be the ordered axial gauge on this cube, anchored at a fixed point, for
\(U_t=e^{i\eta tA}U_0\). In the resulting gauged determining coordinates, the actual nonlinear average has logarithm \(B_p^g(t)\), and
\[
 \|B_p^g(1)-B_p^g(0)\|
 \le C_{\rm av}u(h_p/h_n)^2.
 \tag{BM.19}
\]
All constants depend on the fixed block geometry and group but not on the number of fine bonds, \(p,n\), or total depth.

**Proof.** Take \(R=c\,a/u\), choosing \(c_a\) so that \(R\ge4\). On the complex disc \(|t|<R\), the elementary plaquette expansion gives
\[
 \|dU_t-I\|\le C a\eta^2h_n^{-2}.
\]
Indeed its terms are the original curvature, the covariant curl of \(tA\), and products bounded by \(|tA|^2\), with higher analytic terms paid by the fixed small ceiling. The link and inverse-link norms are bounded by \(\exp(C\eta a/h_n)\); a compact-group part costs no norm.

The axial paths have at most \(C h_p/\eta\) links. The exact path-interchange proof of (R14.23) therefore yields
\[
 \|U_t^{g_t}-I\|
 \le C a\eta h_p h_n^{-2}
       \exp(Ca h_p/h_n).
\]
The exponential is bounded by a fixed constant. The principal logarithm is consequently defined, and \(U_t^{g_t}=e^{i\eta A_t^g}\) with
\[
 \|A_t^g\|\le C a h_ph_n^{-2}.
 \tag{BM.20}
\]
These gauges and logarithms are holomorphic throughout the disc.

Use the actual relative-average bound proved from CMP99, p.406 after (3.78), and the fixed final averaging step, as recorded in (E14.39)–(E14.41). It gives
\[
 \|B_p^g(t)\|\le C h_p\|A_t^g\|
       \le C a(h_p/h_n)^2
 \tag{BM.21}
\]
on \(|t|<R\). This is the unmodified nonlinear average, not an identification with its linearization or with a different \(Q'_p\). Cauchy on a disc of radius at least \(R/2\) around each \(t\in[0,1]\), followed by integration over that segment, gives
\[
 \|B_p^g(1)-B_p^g(0)\|
 \le C R^{-1}a(h_p/h_n)^2
 \le C u(h_p/h_n)^2.
\]
This proves (BM.19). If \(u=0\), the conclusion is immediate. \(\square\)

The corresponding value gain is already visible in CMP109, p.263, immediately after (1.16): the actual averaged plaquette bound contains the square of the averaging length. Lemma BM.2 makes its response version explicit and retains complex parallel-transport costs. An axial gauge anchored at an output point equals the identity there, so it does not change a current evaluated at that point; it still changes the surrounding determining data and must be retained in any subsequent reconstruction.

In a basic \(n\)-regular layer chart one may take \(a=C\max\{\alpha_{0,n},\alpha_{1,n}\}\) and \(u\) from (BM.10), provided the required averaging cube and its fixed margin are in that chart. The reserve (BM.13) makes \(u/a\) small. Equation (BM.19) then supplies precisely the two scale powers needed for the **local determining input** when \(n>p\).

It remains necessary to control the full \(p\)-reconstructed output, whose determining data outside this local cube also contribute. That requires the actual joined determining geometry in (BM.15), its normalized kernel composition, and the independently extended current. Lemma BM.2 does not replace those checks by an unproved minimizer-consistency assertion under refinement or under a change of underlying lattice.

#### 8. The single remaining reconstruction-transfer statement

Here is a quantitative formulation of the surviving reconstruction issue, rather than a further generic sufficient contour theorem. Denote the **actual** prepared current connection in CMP109 (3.6)–(3.13), with the full multiscale construction of CMP119 pp.275–277, by
\(\mathcal V_{k,s}(z;U,J)\). Its comparison value at \(z=0\) is the prescribed unperturbed connection. Keep the independently varied external \(J\) and the complex preparations \(s\) in that actual formula. Form the prescribed reconstructed pair
\[
 \mathcal T_{p,X;k,s}(z;U,J)
 =
 \left(
 U_{p,X}(M^\bullet(\mathcal V_{k,s}(z;U,J))),
 J_{p,X}(M^\bullet(\mathcal V_{k,s}(z;U,J)))
 \right)
 \tag{BM.22}
\]
using exactly the determining data and gauge conventions in CMP119 (2.35)–(2.37). Define its two normalization weights by
\[
 w_F(n,p)=L^{-2p}(L^nL^{-p})^{-2},\qquad
 w_J(n,p)=L^{n-\min\{p,n\}}(L^nL^{-p})^{-3}.
 \tag{BM.23}
\]

**Remaining statement.** On the actual current contour
\(\|z\|_\infty<2P_k\), \(|s(\Delta)|<e^{\kappa_1}\), and the prescribed joint background/independent-current domain, prove that every pair (BM.22) is holomorphic on a common fixed-fraction reserve and that its finite response obeys
\[
 \sup_{x\in X\cap A_n}
 \max\left\{
 \frac{\|\delta[dU_{p,X}](x)\|}{w_F(n,p)},
 \frac{\|\delta J_{p,X}(x)\|}{w_J(n,p)}
 \right\}
 \le
 C_{\rm rec}g_k\|z\|_\infty
 e^{-\Gamma(k-n-c_0)_+},
 \quad p\le j\le k,\quad n\le j.
 \tag{BM.24}
\]
The deltas compare \(z\) with zero using the source's fixed comparison gauges; \(C_{\rm rec},c_0,\Gamma\) must be independent of \(p,j,k,X\), volume and remaining admitted history. A fixed \(\Gamma>\log2\) suffices for the domain gap; a larger fixed reserve such as the one in (BM.5) also pays the subsequent carrier sums. The argument must first define the maps on their absolute domains and then prove this smaller-domain inclusion, so it cannot assume the desired B contour to apply Cauchy.

The weighted-age proof and Lemma BM.2 supply, respectively, the original-map response and the local smoother-input gain needed by (BM.24). They do not yet prove that estimate for the full joined reconstruction.

The exact source-geometry issue is as follows. CMP119 (2.14) defines a localized joining operation by retaining the original determining set away from a proper-scale boundary collar and using the localized determining set in that collar. LFR II p.373 explicitly confirms this same-lattice localization property, including the at-most \(2M_1\) boundary width. Its notation uses the local determining set first, so argument order is not a reliable way to read the operation. A possible proof of (BM.24) would identify (BM.15) with the actual localization of the original determining geometry truncated at level \(p\), with the same averaged boundary data. That would permit a pointwise mesh comparison and normalized kernel composition.

This identification has **not** been verified here. In particular, the boundary data inserted in (BM.15) are \(M^\bullet(U)\); localizing a separately constructed global \(p\)-minimizer would insert its own \(M^\bullet(U_p)\). These data are not identified by a general minimality principle. The change of the underlying reconstructed lattice and the fine boundary collars also have to respect the current weight \(w_J(n,p)\). An ordinary union of overlapping coarse and fine constraints, a formal intersection of layer sets, or a same-lattice identity from LFR II does not by itself prove the required statement.

Thus C-05 remains open at the precise full reconstruction-transfer estimate (BM.24), followed by its application to all of the actual B contributions. The preceding metric ambiguity and the local two-power averaging loss have been resolved; they are not listed again as missing inputs.

#### 9. Source references

- Balaban, CMP96 (1984), 223–250, (2.2), (2.46)–(2.59), Lemma 2.1. pp. 224 and 231–234.
- Balaban, CMP99 (1985), 389–434, (3.41), Theorems 3.1 and 3.10 and the random-walk kernel bounds.
- Balaban, CMP102 (1985), 277–309, Proposition 9 and (190).
- Balaban, CMP116 (1988), 1–22, (1.3)–(1.7), (1.11)–(1.21). article.
- Balaban, CMP119 (1988), 243–285, (2.34)–(2.39), (3.2)–(3.5), (3.20), pp.276–277.

The direct metric, normalized-row, weighted-preparation, anchored-collar and local averaging-response deductions are proved above with their exact scopes. The full joined reconstruction-transfer estimate (BM.24) remains explicit.

### Supplement AF.2: Complete boundary terms and value sums


#### 1. Exact scope

This argument concerns the **current-dependent boundary perturbation** in the actual conditional integral of CMP119 (3.25), with all older fluctuation coordinates and history geometry retained as parameters. The present conditional Gaussian quadratic form, its cross force and its Schur-complement scalar remain in the exact Gaussian split of C-01. A boundary perturbation value at the reference current field is separated only by the exact conditional cancellation of Proposition BD.1. That scalar remains in the outer marginal.

The actual common multiscale B contour and the required complete map-output kernel bounds are being proved separately. The value-summation deduction below states their precise uses. Merely knowing that a contour exists does not sum an unweighted collection of old B bounds.

The primary primitive boundary bound is the full-tree bound

\[
 |B^{(j)}(X,U,J,\mathbf A,\{S\})|
 \le B_0 e^{-\kappa d_j(X)}.
 \tag{BV.1}
\]

This is CMP119 (2.40)–(2.42), pp.261–262. The source explicitly chooses it instead of the optional component-resummed bound with \(d_j(X\setminus Z_j)\). The latter would not justify the connector argument below.

#### 2. The actual sectors are exhaustive

CMP119, pp. 267–277, separates the following contributions.

| Sector in the conditional action | Exact source location and operation |
|---|---|
| Classical nonlinear fluctuation, constraint substitution, Haar and coarea terms | The full formula (3.15), pp.267–268, uses the actual constrained field \(g_kCA-hD(g_kCA)\). Page 276 applies the actual localized small-field construction, including \(P^{(k)}\), with its multiscale operators. The relevant classical quadratic form remains in the source Gaussian precision. |
| Inherited E and R contributions assigned to B | Page 276 repeats CMP109 Sections 3–4 on a layer of scale \(n\), replacing the old unit parameter by \(L^{-n}\), and then localizes with the full multiscale random-walk expansions. Terms whose localization crosses the current regular boundary are assigned to B. R is treated in the same way except that its coupling subtraction is absent. |
| Inherited B fluctuation differences | The end of p.276 applies CMP109 (3.6)–(3.7), then localizes. These carriers intersect the current regular integration region. Page 277 states the primitive boundary decay bound with an additional \(O(\varepsilon_k)\), and explains that minimizing-field decay pays the shrinking dyadic domains. |
| Heterogeneous Wilson coefficient | The last term in the braces of (3.15)/(3.27) is localized by the multiscale partition of unity in the plaquette sum. Page 277 puts it in B because the coefficient difference is supported in \(Z_k\), and explicitly suppresses its large coefficient using decay of the minimizing map. Its coefficient is the localized recursion (2.24), not simply one homogeneous \(g_j^{-2}\) throughout a transition collar. |
| Relocation and its Jacobian | Pages 251–252, (1.21)–(1.24), give the first-step operation. Pages 269–270 repeat it with \(H^{(k)}\), and define \(V^{(k)}(S_{k+1},A_k,H^{(k)})\). Every previous action term contributes, along with the exponentiated Jacobian. Page 277 retains these terms and their additional localization in \(S_{k+1}\). |
| Gaussian cross-component terms already placed in B | Page 258 after (2.21) keeps only within-component quadratic terms in the operation \(T^{(j)}\); the other quadratic terms are included in B. They are therefore among the inherited B terms in (BV.1), not omitted Gaussian terms. |

The last row concerns **older terms already assigned to B by the source**. It is distinct from splitting the present Gaussian form between the currently integrated field \(z\) and retained field \(v\). The latter has a cross term \(z^{\mathsf T}H_{IO}v\). Its current Hessian is zero, but its force \(H_{IO}v\) need not be small. It remains in the exact conditional Gaussian mean and in C-08; it is not included in the small perturbation prefactor below. A calculation involving only the nonlinear Wilson remainder and a determinant would not cover the complete action.

The relocation cutoff in (1.22), denoted \(g(A')\) in the source, is \(C^\infty\), not claimed analytic in the older real coordinates \(A'\). These coordinates remain parameters in the native B theorem. Dependence on the small relocation field \(H\), and on the native complex \(U,J\) arguments, is analytic. Arbitrary derivatives in old coordinates, changing selectors or history interfaces are not supplied by a native current contour.

#### 3. The localized heterogeneous coefficient has a safe age bound

Write \(w_j=g_j^{-2}>0\), and let \(w_j(x)\) be the coefficient in CMP119 (2.24). The exact homogeneous and localized recursions give

\[
 \beta_l=w_{l-1}-w_l,\qquad
 w_k(x)-w_k=\sum_{l=1}^k\beta_l(1-\phi_l(x)).
 \tag{BV.2}
\]

Let \(n\) be such that \(\phi_l(x)=1\) for \(l\le n\). This may be the earliest active cutoff index at the point; identifying it with a geometric layer requires the source partition and cutoff support, not a change of notation. Assume the fixed cutoff bound \(|1-\phi_l|\le C_\phi\).

The checked source AF comparison yields

\[
 w_l\le C_{\rm AF}'(1+k-l)w_k.
 \tag{BV.3}
\]

It follows, without assuming the sign of \(\beta_l\), that

\[
\begin{split}
 |w_k(x)-w_k|
 &\le C_\phi\sum_{l=n+1}^k(w_{l-1}+w_l)\\
 &\le C_\phi C_{\rm AF}''(1+k-n)^2g_k^{-2}.
\end{split}
\tag{BV.4}
\]

Thus transition collars cost at most a quadratic age factor and the explicit \(g_k^{-2}\). The constant-stratum estimate can be sharper, but is not needed for a summation with an exponential age reserve. The small physical current collar must pay the running \(g_k^{-2}\); a fixed number \(e^{-cMR_{\min}}\) cannot do so.

The geometric cutoff radius is \(R_k\ge\ell_k^r\), \(\ell_k=\log g_k^{-2}\), by CMP119 (2.5), p.255. For a fixed admitted choice \(r>1\) and every fixed \(s,N\),

\[
 g_k^{-s}\ell_k^N e^{-cR_k}\longrightarrow0.
 \tag{BV.5}
\]

This follows directly by taking logarithms:
\(s\ell_k/2+N\log\ell_k-c\ell_k^r\to-\infty\).
The source's description of \(H^{(k)}=O(\varepsilon_ke^{-R_k})\) on p.269 as smaller than every positive coupling power uses exactly this type of reserve.

#### 4. One connector covers both possible locations of an old B carrier

Let \(i\) be a current input anchor, and let \(y\) be an attachment point of a localized minimizing-map variation to a primitive carrier \(X\), with \(X\cap Z_j\ne\varnothing\). Let \(d_\Omega\) be the actual weighted distance of CMP96 (2.46), not the Euclidean distance in old units. Its weight on a layer of physical mesh \(h_n\) is \(h_n^{-1}\).

There are two cases.

1. If \(y\notin\Lambda_j\), every path from the current region to \(y\) already exits \(\Lambda_j\). Thus the minimizing-map path supplies the needed connection by itself.
2. If \(y\in\Lambda_j\), choose a path in a full tree for \(X\), from \(y\) toward \(X\cap Z_j\), and stop at its first exit from \(\Lambda_j\). Before this exit it lies in \(\Lambda_j\subset\Omega_j\). Every distance weight there is at most \(h_j^{-1}\). Convert the segment to an admissible block-center path by the fixed source block rounding: replacing each visited block segment by its prescribed center connections costs at most a fixed multiple of its weighted length plus a fixed cost per visited block. All visited blocks have scale at least \(h_j\), so their number is bounded by a fixed multiple of the old \(j\)-grid length plus an endpoint constant. The resulting weighted length is at most \(C_M(d_j(X)+1)\), with \(C_M=CM\) in the source's \(M\)-cell convention. There is no factor growing with old age.

In both cases,

\[
 d_\Omega(i,\partial_{\rm in}\Lambda_j)
 \le d_\Omega(i,y)+C_Md_j(X)+C_{\rm edge}.
 \tag{BV.6}
\]

The fixed edge term accommodates the first-exit convention. It has no age or volume dependence. Outputs outside the entire active domain have no current variation. Attachments in an earlier active layer \(n<j\) need not be incorrectly declared zero: the minimizing path to them carries the stronger age \(k-n\).

Suppose an actual localized kernel/tree contribution has the available decay

\[
 e^{-c_Hd_\Omega(i,y)-\kappa d_j(X)}.
 \tag{BV.7}
\]

Split each exponent into four fixed shares. With

\[
 \mu=\frac14\min\{c_H,\kappa/C_M\}>0,
 \tag{BV.8}
\]

the first share gives the connector bound
\(C e^{-\mu d_\Omega(i,\partial_{\rm in}\Lambda_j)}\), used to pay the current collar. The second share pays the age: for the innermost restriction \(n=j\), use the same connector and the layer-crossing lower bound; for an earlier-layer restriction \(n<j\), use the endpoint \(y\) in that layer and the stronger \(k-n\) lower bound on the H path itself. The third shares are reserved for the normalized kernel/carrier row sums, and the fourth shares for final current-carrier localization. In particular the age \(k-n\) is not inferred from a path that merely reaches \(\partial\Lambda_j\). No exponent is spent twice.

The separate geometry/kernel proof must supply these actual lower bounds in the weighted metric, with its fixed adjacent-step conventions. The distinct shares just described give the simultaneous factor

\[
 e^{-c_{\rm col}MR_k}e^{-\Gamma(k-j)}
 \tag{BV.9}
\]

at reduced fixed constants. For earlier-layer restrictions use \(k-n\), by the separate H-endpoint argument. Equivalently one may first use that the maximum of collar and age lower bounds is at least half their sum, with correspondingly smaller constants. The effective rate must be chosen after the reduction (BV.8); increasing the fixed admissible \(R_{\min}\) can pay the entropy and scaling losses in CMP96 (2.58)–(2.59). An ordinary old-scale tree length is not substituted into \(d_\Omega\).

#### 5. The resulting scalar age sum

This section gives a quantitative implication once the complete map/domain proof supplies (BV.7)–(BV.9), all relevant normalized kernel row sums, and the source localization on the common contour. It exposes the costs required of that proof.

For an inherited B activity of index \(j\) and one of its output-layer restrictions \(n\le j\), the dyadic source radius costs \(2^{j-n}/\alpha_{*,n}\). The checked running comparison gives

\[
 \frac{g_kP_k}{\alpha_{*,n}}
 \le C\sqrt{1+k-n}\,\ell_k^{p_0-q}.
 \tag{BV.10}
\]

Retaining the conservative old-cell factor \(L^{4(k-n)}\), the sum over \(n\le j\le k\) is bounded by

\[
\begin{split}
 &C B_0\ell_k^{p_0-q}e^{-c_{\rm col}MR_k}\\
 &\qquad\times
 \sum_{a\ge0}(1+a)^{3/2}
 \exp[-(\Gamma-4\log L-\log2)a].
\end{split}
\tag{BV.11}
\]

The factor \(1+a\) includes the number of admissible \(j\) at fixed \(a=k-n\). If the normalized source row/column estimate removes an old-cell factor, the bound improves; (BV.11) does not require that improvement. The integration measures and scale-normalized outputs must be those of the actual kernel theorem. An unnormalized sum over every fine bond is not used as that row sum.

Choose

\[
 \Gamma>4\log L+\log2+\delta,\qquad\delta>0.
 \tag{BV.12}
\]

Then (BV.11) is uniform in cutoff depth. Any additional *fixed* polynomial age factors from the heterogeneous coefficient (BV.4), finite kernel moments or fixed-order classical expansion can be included by replacing \(3/2\) by one fixed exponent \(b\). The numerical sum
\[
 S_{b,\delta}=\sum_{a\ge0}(1+a)^b e^{-\delta a}<\infty
 \tag{BV.13}
\]
remains uniform.

For E- and R-origin boundary terms, p.276 first performs the same regular calculation on the appropriate layer \(n\). The inner \(j\le n\) sum is therefore controlled by the already established E and R majorants on their admitted layer domains. Carriers crossing the **newest** boundary of \(\Lambda_{k+1}\) may touch the current support. No old-\(Z_k\) collar factor is available or claimed for them: the already finite regular E/R value majorant is used directly, on the common B background contour supplied by the admission proof. For a genuinely older layer \(n<k\), the remaining remote current-to-layer dependence uses the connector just described. These activities remain B at the final scale under the actual source classification.

The heterogeneous term retains the extra coefficient (BV.4); its \(g_k^{-2}\) is paid only with the actual current-collar factor (BV.5). The relocation terms retain the analytic \(H^{(k)}\) and their source bound \(O(\varepsilon_ke^{-R_k})\), including all previous-action and Jacobian contributions. Their stated arbitrarily high positive power of \(g_k\) remains uniform only on the native contour and with the older cutoff arguments fixed.

Finally reserve enough of the source's *full current-carrier* decay to perform the anchored \(M\)-cell sum. The carrier count and spatial weight must use the source's face-connected \(M\)-cube convention. If
\[
 \sup_{\mathcal C_k}|\widetilde B_{k,Y}|
 \le K_{B,k}e^{-\kappa_Bd_k(Y)}
 \tag{BV.14}
\]
is the fully localized majorant obtained above, then for a sufficiently small fixed spatial \(\gamma>0\), and with the required entropy reserve,
\[
 \sup_i\sum_{Y:\,i\in I_Y}
 e^{\gamma\operatorname{diam}(I_Y)}
 \sup_{\mathcal C_k}|\widetilde B_{k,Y}|
 \le C_{\rm car}K_{B,k}.
 \tag{BV.15}
\]
The fixed localization prefactors, kernel moments, Lie-algebra dimension and powers of \(M\) belong in \(C_{\rm car}\). They may not contain total volume, hidden distance to the current region, or an unsummed old-scale index.

On a common current-coordinate polydisc of radius \(c_GP_k\), BD.2 then gives the complete conditional boundary Hessian row bound
\[
 \sup_i\sum_l e^{\gamma d(i,l)}
 \|D_iD_l\widetilde B_k\|_{\rm op}
 \le C_GC_{\rm car}K_{B,k}P_k^{-2}.
 \tag{BV.16}
\]
Higher current derivatives are taken after the normally convergent age/carrier sum. Native external derivative radii must be those proved by the complete B-domain admission theorem; this deduction does not assign them unverified regular-E radii.

For a concrete sufficient prefactor, put \(\delta_k=g_kP_k\), \(\theta_k=\ell_k^{p_0-q}\le1\), and retain the standard cubic classical bound and bounded Haar/coarea remainder from CMP116 Lemmas 1–2, transferred exactly as specified on CMP119 p.276. Once the complete map and connector estimates just stated hold, a conservative sector majorant is

\[
\begin{split}
K_{B,k}\le C_{\rm src}(1+S_{b,\delta})\bigl[
 &\mathfrak K_E+C_Rg_k^{\kappa_0-11}+B_0\theta_k\\
 &+g_k^{-2}\delta_k^3+\delta_k
 +g_k^{-2}\delta_ke^{-c_{\rm col}MR_k}
 +g_k^\nu\bigr],
\end{split}
\tag{BV.17}
\]

where \(\nu>0\) is any one fixed relocation power allowed by the source, and \(b\) contains the fixed age-polynomial costs, including (BV.4). The first two terms use the complete layerwise E/R majorants and claim no extra collar factor for newly boundary-crossing carriers. For their remote older-layer part, the additional current-fluctuation ratio is at most one after the chosen coupling ceiling. The third is (BV.11), with its helpful collar suppressed from the bound. The fourth and fifth are the current classical cubic and measure remainders. The sixth retains the heterogeneous coefficient until its actual current collar pays it. The last is the source relocation/Jacobian bound, with its full fixed-parameter constant. The present exact Gaussian cross force is not part of \(K_{B,k}\). All fixed preparation and localization constants belong in \(C_{\rm src}\).

This displayed prefactor is an application consequence of the specified actual sector estimates. It is not obtained from a bound on one representative Wilson term alone. In particular the heterogeneous and relocation rows of the source formulas remain necessary to use it.

Equations (BV.5) and (BV.17) yield
\[
 K_{B,k}P_k^{-2}\longrightarrow0
 \quad\hbox{as }g_k\downarrow0,
 \tag{BV.18}
\]
uniformly in depth and volume after the fixed source choices. For example the classical contribution is
\(g_k^{-2}\delta_k^3P_k^{-2}=g_kP_k\to0\);
the unenhanced E term is \(\mathfrak K_EP_k^{-2}\to0\).
Thus a source \(O(\varepsilon_k)\) improvement for every individual B row is stronger than needed for the small conditional Hessian conclusion. The current collar is nevertheless indispensable for the explicit running \(g_k^{-2}\) coefficient in the heterogeneous row.

#### 6. Exact remaining application checks

There is no extra algebraic sector missing from the ledger in Section 2. The actual open checks in applying (BV.11)–(BV.16) are quantitative:

- all required output restrictions of the actual B pullback must obey the common-contour layerwise kernel estimate, including the reconstructed current, independent current and relocation;
- the current collar and age rate must be retained after the exponent split (BV.8), with the normalized row sums and fixed entropy costs, not just in one pointwise kernel entry;
- the heterogeneous coefficient must use its actual localized recursion and its earliest active cutoff layer, including transition collars;
- the actual localization must preserve enough full-tree/current-carrier decay after the anchor connector is paid;
- old real cutoff arguments and outer retained-only factors must not be mistaken for analytic native variables already controlled by this theorem.

Once those checks are supplied, the displayed sums are finite with no remaining unexplained old-age or volume factor. This note does not itself declare C-05 complete before they are verified.

#### 7. The exact reconstructed-data issue still preventing C-05 completion

The published construction distinguishes two operations which must not be equated without checking their data.

CMP119 (2.14), p.257, defines a localized determining set by

\[
 \mathbf B\cup\mathbf B_j(\Omega)
 =
 (\mathbf B\cap\Omega^{-2})
 \cup
 \bigl(\mathbf B_j(\Omega)\cap
          (\Omega\setminus\Omega^{-2})\bigr).
 \tag{BV.19}
\]

The original determining set is preserved in the interior. The specifically constructed local determining set supplies the boundary collar. The notation denotes this prescribed construction, not an unqualified union of arbitrary overlapping fine and coarse constraints.

LFR II, p.373, (1.161)/(1.61), explicitly uses the identity

\[
 U_k^0=
 U\bigl(\mathbf B_k''(Y_1),M^\bullet(U_k^0)\bigr),
 \qquad
 \mathbf B_k''(Y_1)=\mathbf B(Y_1)\cup\mathbf B_k''.
 \tag{BV.20}
\]

Its neighboring (1.62) uses the corresponding identity for \(U_1\). The fields and gauge transformations in these formulas are retained explicitly. This is localization of an already constructed minimizing field on the same underlying lattice with the specified determining data.

The B-domain reconstruction in CMP119 p.261 is instead defined by

\[
 U_{p,X}(M^\bullet(U))
 =
 U\bigl(\mathbf B_p(X)\cup\{\Gamma_i\}_{i<p},
             M^\bullet(U)\bigr),
 \tag{BV.21}
\]

with the additional curvature and current bounds (2.35), (2.37) in their \(p,n\) scale convention. In particular the \(n>p\) current bound requires the two-power improvement
\(\alpha_{0,n}L^{-2(n-p)}\).

Equation (BV.20) does not identify (BV.21) with a simple average of the original finer minimizing field. Nor does localizing a separately constructed global \(p\)-minimizer automatically identify its new boundary data \(M^\bullet(U_p)\) with the required \(M^\bullet(U)\). Such a claim would change either the determining data or the underlying minimization problem.

The newly proved weighted-age row bound on the original admitted determining geometry, and the local two-power averaging lemma in Supplement AF.1, therefore do not alone settle the full joined \(p\)-reconstruction. One still needs a direct theorem for its actual compatible determining geometry and data, or an exact source identity whose hypotheses and data match (BV.21), followed by the normalized kernel composition and independent-current output estimate. This is the concrete remaining C-05 domain step. No counterexample to the source construction is asserted.


#### Primary record

- CMP119 (1988), 243–285: (1.21)–(1.24), (2.21)–(2.24), (2.40)–(2.42), (3.15), (3.23)–(3.29), and pp.269–270, 275–277.
- CMP96 (1984), 223–250: weighted distance (2.46), transition estimate (2.57), entropy estimate (2.58)–(2.59), and Lemma 2.1. The actual kernel admission proof must retain its source norm and integration conventions.
- CMP109 (1987), 249–301, and CMP116 (1988), 1–22: the localization and layer-transfer uses stated explicitly in CMP119 pp.276–277. The fixed source localization constants remain scoped inputs, as in the completed regular E/R contour proofs.

### Supplement AF.3: Final boundary application conditions


Theorem E14.3 removes the regular E contour obstruction. The subsequent Supplement AF.1 proof resolves the weighted-age geometry, normalized prepared response on the original determining geometry, and the local two-power averaging response. The connector and scalar summations in Supplement AF.2 also pass their stated application checks. These results do not yet discharge the complete boundary statement C-05. The surviving step is the actual joined \(p\)-reconstruction and its global outputs on the full source tuple, followed by verification that the complete localized boundary action meets the displayed carrier/application bounds.


#### 1. What the new result supplies

E14.39–E14.44 use the actual nonlinear relative average, a fixed absolute domain for the internal maps, the zero insertion, and the full source derivative output norms. They admit the entire relative insertion segment before testing the smaller running primitive E radius. E14.49–E14.53 then provide a simultaneous native current/background/independent-current/preparation contour and a summable regular E prefactor. The near- and far-age summations can therefore be differentiated on that contour without an old-age-dependent Cauchy radius.

The theorem retains the actual source E/B assignment. It expressly does not assert the corresponding multiscale B-domain inclusion. Native background directions in it also do not stand for arbitrary raw retained or selector variations.

#### 2. The actual boundary margins have an additional layer index

CMP119 gives the formulas on pp.254–256, 261–262 and 276–277; the construction of the current collar is on pp.264–269. In CMP119 (2.34)–(2.39), the restrictions on layer

\[
 \Omega_n\setminus\Omega_{n+1},\qquad n<j,
\]

and on the innermost region \(\Omega_j\), include the coefficient

\[
 \vartheta_{j,n}=1-\beta\bigl(1-2^{-(j-n)}\bigr).
 \tag{BA.1}
\]

It multiplies the relevant running radius and the displayed physical scale weights. The restrictions include the original plaquette and independently extended current, the reconstructed-field and reconstructed-current quantities, and the complex relative field and its first derivative. These are not merely the regular E restrictions at index \(j\).

In particular, the published text of p.261 gives the reconstructed curvature and current weights, respectively, as

\[
 L^{-2p}(L^nL^{-p})^{-2},\qquad
 L^{n-\min\{p,n\}}(L^nL^{-p})^{-3}.
 \tag{BA.1a}
\]

The additional reconstruction index \(p\) belongs to the tuple and cannot be dropped. The second weight equals \(L^{3(p-n)}\) for \(n\le p\), and \(L^{-2(n-p)}\) for \(n>p\). The latter improvement involves the curvature/difference regularity of the actual coarse determining field; a bound on its undifferentiated relative-potential supremum is not that estimate.

When a center meets the corresponding later \((k+1)\)-domain restriction, the algebraic reserve in an old \(j\)-domain, with \(n\le j\le k\), is

\[
 \vartheta_{j,n}-\vartheta_{k+1,n}
 =\beta\left(2^{-(j-n)}-2^{-(k+1-n)}\right)
 \ge(\beta/2)\,2^{-(j-n)}.
 \tag{BA.2}
\]

This is a reserve statement for those exact source restrictions, not a proof that an arbitrary center or pullback meets them. It quantifies the additional application required by the source explanation on p.277. For each restriction, the reserve must be multiplied by that restriction's own \(\alpha_{0,n}\) or \(\alpha_{1,n}\) and its physical normalization. A single unspecified old radius cannot replace them all.

The product domain (3.43), p.276, is genuinely useful: it already applies to the localized boundary fluctuation expressions after their source substitutions. Its displayed current radius is \(C_1p_1(g_k)\). The identification needed to compare that printed polynomial with the full normalized real support \(P_k=\delta_k/g_k\) remains unverified. E14.3 bypassed that identification for the E component through its underlying maps; the corresponding B-domain argument must also be supplied before making that bypass for B.

#### 3. An ordinary old-scale collar and a multiscale kernel have different metrics

The geometric collar is real. CMP119 pp.264–265 surrounds the old bad region \(Z_k\) by several layers of current-size cubes before defining \(\Omega_{k+1}\); p.269 takes a further interior set for the regular integration. This is stronger information than interlacing alone.

Consequently BD.3 applies to an ordinary connected tree, measured in old \(j\)-scale units, joining the current region to \(Z_j\subset Z_k\): its length is at least a fixed collar constant times \(R_kL^{k-j}\), with the source's fixed adjacent-step conventions absorbed into that constant. The full primitive B bound (2.42), chosen by the source rather than its weaker component-resummed alternative, can pay this length when that connection lies in the primitive carrier itself.

There is a second way a B vertex can depend on a current variable. A small old carrier close to \(Z_j\) can receive a remote current dependence through the minimizing-field pullback. For that dependence the relevant exponential in CMP102 (190) is

\[
 \exp\{-c\,d_{\Omega}(y,y')\},
 \tag{BA.3}
\]

where \(d_{\Omega}\) is the source's weighted multiscale distance. CMP99 p.397 explicitly identifies this weighted distance and refers to its earlier definition. It is not automatically the Euclidean distance divided by the old mesh. A route through a coarser layer has a different distance weight. Thus BD.3 does not by itself justify substituting \(R_kL^{k-j}\) into (BA.3).

This distinction matters in precisely the application at issue. The primitive-tree weight controls a carrier which reaches the current region; the minimizing kernel controls the additional connection for a carrier which does not. A complete anchored estimate must combine the two with their actual metrics and their actual localization/preparation factors. It may prove more decay than a separate estimate, but that combined bound is not the ordinary-tree statement BD.3.

##### 3.1 The weighted-age geometry

CMP96 gives the formulas on printed pp.224, 231 and 233. Formula (2.2) requires separation of successive nested regions by more than \(RM\) in the local scale. Formula (2.46) defines the actual path metric by adding the length spent in each determining layer, weighted by the inverse local mesh. The surface decomposition (2.47)–(2.48), followed by (2.57), charges more than \(RM\) for every complete layer transition. A path from level \(n\) to level \(k\) therefore has at least \((|k-n|-1)_+\) such transitions.

The source row-sum proof (2.58) also retains this information after summing its spatial and path indices. To display it without changing the source metric, let \(0<a<1\), let \(\delta_0>0\) be the kernel decay rate, and use the source's finite number \(c_0(a/2)\). The row restricted to an input layer differing by \(s\) is bounded by

\[
 c_0(a/2)^d
 \sum_{m\ge(s-1)_+}
 \exp\!\left[-m\left(
 \frac{a\delta_0RM}{2}-2d\log c_0(a/2)
 \right)\right].
 \tag{BA.3a}
\]

Thus, for any fixed \(\gamma>0\), strengthening the source parameter condition to

\[
 \frac{a\delta_0RM}{4}
 >2d\log c_0(a/2)+\gamma+1
 \tag{BA.3b}
\]

gives a bound \(C_\gamma e^{-\gamma s}\) for that row, with a fixed \(C_\gamma\). This follows directly by summing the geometric series in (BA.3a), with its missing first transition absorbed in the fixed constant. The source's normalized integration measures and physical output weights must still accompany an application to a particular operator. The strengthened parameter choice must also be checked jointly with the other retained source choices; it is not an unconditional certificate for J0.

This settles the metric and base-row-summation part. Sections 3–4 of Supplement AF.1 further retain it under the actual original-geometry nonlinear preparation, with weighted contraction and the source current-output formula. None of these statements replaces \(d_\Omega\) by old-scale Euclidean distance or proves a factor \(e^{-cR_kL^{k-j}}\) for every multiscale kernel. Applying them to the changed \(p\)-reconstructed B outputs, with their actual \(p,n\) weights in (BA.1a), is the remaining operator step.

The source's assertion on p.277 that minimizing decay pays the shrinking domains is retained as a scoped source input. The verified age estimate and prepared original-geometry response now quantify that payment for the basic field/current clauses. Turning it into the whole reconstructed tuple still requires the changed-geometry application. The source regular contour theorem does not replace it.

##### 3.2 The local two-power input response is also proved

Lemma BM.2 in Supplement AF.1 settles the local determining-input issue for \(n>p\), with an explicit local cube margin. For \(U_t=e^{i\eta tA}U_0\), whose physically normalized variation has size \(u\) in the field and first-difference norms, take a complex parameter disc of radius proportional to \(a/u\), where \(a\) is the admitted local background ceiling. The actual plaquette expansion stays within curvature size \(Ca\eta^2h_n^{-2}\) on that disc. The ordered axial gauge gives a potential of size \(Ca h_ph_n^{-2}\), with bounded complex parallel-transport factors. The actual nonlinear average then has size \(Ca(h_p/h_n)^2\). Cauchy and integration over the real parameter segment yield

\[
 \|B_p^g(1)-B_p^g(0)\|
 \le C u(h_p/h_n)^2.
 \tag{BA.3c}
\]

The local-input estimate does not imply that the global reconstructed minimum depends only on that cube. Its other determining variables, its joined geometry, and the reconstructed independent-current output remain to be controlled. No exact consistency of minimizers under a change of lattice has been assumed.

#### 4. A precise sufficient remaining kernel test

The stronger superexponential old-age bound in BD.4 is one sufficient route, not the only possible one. There is another route that avoids paying \(2^{am}\) separately at derivative order \(m\).

For each source output restriction on layer \(n\), measure its increment in the physical normalization appearing in (2.34)–(2.39). Let \(\mathcal K_{n,k}\) denote a common bound for the corresponding normalized row sums of the **actual complete** current-to-output derivative, including the prepared minimizing map, independently extended current outputs, and the required boundary relocation. The necessary row sum includes its source integration measure; it is not an unnormalized sum over all fine bonds. Suppose, on a previously admitted fixed absolute map domain, that these bounds imply

\[
 \|\Delta\Phi_{n,k}\|_n
 \le C g_kP_k\,\mathcal K_{n,k}
 \quad\hbox{for }\|z\|_\infty<2P_k,
 \tag{BA.4}
\]

jointly with the proposed external native variables and preparation parameters. A sufficient B-domain admission test, for each of its output restrictions, is

\[
 \frac{C g_kP_k\,\mathcal K_{n,k}}{\alpha_{*,n}}
 \le \frac\beta8\,2^{-(j-n)},
 \qquad n\le j\le k,
 \tag{BA.5}
\]

where \(\alpha_{*,n}\) is that restriction's own radius. Equations (BA.2) and (BA.5) then leave a strict reserve. The whole source segment and all output restrictions must satisfy the test; bounding only the first plaquette variation is insufficient.

The source geometry and base-kernel calculation above now provide the candidate age rate. The needed full-output conclusion is

\[
 \mathcal K_{n,k}\le C_H e^{-\gamma(k-n)}.
 \tag{BA.6}
\]

Its application to the entire reconstructed tuple and preparation map is **not proved here**. A stronger factor involving \(\sum_rR_r\) is unnecessary for the following implication. With one fixed \(q>p_0\), equal logarithmic exponents for the two running radii, their fixed source-admissible ratio, and the common admitted coupling ceiling for that fixed exponent as in E14.3, the already checked AF comparison gives

\[
 \frac{g_kP_k}{\alpha_{*,n}}
 \le C_*\sqrt{1+k-n}\,\ell_k^{p_0-q}.
 \tag{BA.7}
\]

For fixed \(\gamma>\log2\), the right-hand side of (BA.7) multiplied by (BA.6) and \(2^{j-n}\) is uniformly bounded in \(n,j,k\); the fixed small-coupling ceiling could then make it meet (BA.5). This implication uses \(j-n\le k-n\), and a strict exponential in \(k-n\) dominates its square-root factor. It does not silently extend the verified base-kernel row bound to an unchecked reconstructed output. A larger fixed reserve, for example \(\gamma>4\log L+\log2+1\), also pays a conservative four-dimensional old-cell count in a subsequent value estimate.

Once such a **single common contour** and a summable complete boundary value/carrier majorant have been established, arbitrary current derivatives can be taken after the old-age sum, as in E14.3. The Cauchy factor would then be \(m!(cP_k)^{-m}\), with no additional \(2^{am}\) from differentiation. This avoids requiring a stronger metric estimate solely to repair an artifact of differentiating too early.

#### 5. What remains for C-05

After the contour, the remaining steps are:

1. Prove (BA.5), or an equivalent direct simultaneous B-domain inclusion, for the complete actual pullback. The weighted-age geometry, original-geometry preparation, and local two-power determining input are verified. The exact joined \(p\)-reconstruction geometry and the global reconstructed curvature/current outputs, with every weight in (BA.1a), remain to be established.
2. Verify the complete anchored current-carrier majorant for that admitted pullback, retaining old B terms, E/R terms assigned to B, the heterogeneous-action difference supported in \(Z_k\), and relocation terms supported in \(S_{k+1}\). Supplement AF.2 supplies the exhaustive source formulas, the combined primitive-tree/minimizer connector, four separate exponent reserves, the double old-index summation, and a sufficient sector prefactor. The full-map and localization hypotheses are required here. BD.2 then gives the required weighted Hessian row without a spurious carrier-volume factor. Newest-boundary E/R terms do not require an unavailable old-\(Z_k\) collar; the current Gaussian exterior force stays in its exact Gaussian/Schur split.
3. Check that the resulting budget fits the complete coercivity margin and retain the stated native external derivatives. The additional arbitrary retained/selector pullbacks and history interface currents must not be declared controlled by a native-domain theorem.

The conditional subtraction of BD.1 remains exact and useful, but its discarded-in-the-conditional-law scalar still belongs to the outer marginal. It cannot supply the missing spatial or current estimate.

**Boundary-domain hypothesis.** Application of the boundary induction to the Wilson law requires CL. See [the boundary induction](../boundary/boundary_induction.md). The weighted distance itself is known and checked, the relevant original-geometry row and preparation bounds are proved, the local two-power response is proved, and the final scalar/carrier deductions are explicit. The surviving actual-model application is the joined \(p\)-reconstruction, its global outputs, and the complete localized boundary bound on that admitted contour. Arbitrary retained-coordinate and selector-current estimates have not been folded into a native-domain completion claim.

#### References

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243–285: especially (2.34)–(2.42), pp.261–262, and (3.43) with the discussion on pp.276–277. Geometric construction at pp.254–256 and pp.264–269.
- T. Balaban, *The Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*, CMP 102 (1985), 277–309: Proposition 9 and (182)–(190). The estimate uses its actual derivative kernel and retains its weighted distance.
- T. Balaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP 99 (1985), 389–434: definition/reference to the weighted distance preceding the propagator theorems.
- T. Balaban, *Propagators and Renormalization Transformations for Lattice Gauge Theories II*, CMP 96 (1984), 223–250: pp.224, 231 and 233, especially (2.2), (2.46)–(2.48), and (2.57)–(2.59). This supplies the verified age geometry and row sum of Section 3.1.


---
