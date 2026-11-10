# Posterior means and normalized history interfaces

**Current status:** H8/H9/R9 extend the clean and controlled-prefix sectors, and RB9 supplies the strict-regular Q/R sector. The exact posterior covariance identities below remain necessary for combining sectors. The full normalized majorant has not yet been established.

**Status:** This module proves regular \(R\)-potential perturbations of the actual normalized rooted operation, asynchronous protected-core entry, a one-operation support attachment estimate, and an exact posterior good/bad covariance estimate. It additionally proves normalized initial-birth rarity on the original Wilson measure and a sharp \(r^{-8}\) scale-summed bound for clean descendants of those initial births. It identifies the ordinary-metric reserve for unprocessed regions and the normalization estimate still needed for general histories. The complete mixed-history gate is not declared closed.

### 1. The actual positive law and the conditioning levels

Fix one frozen positive RG operation. Write its joint law as \(\Pi(d\omega,d\gamma,dV)\), where \(\omega\) contains old variables, \(\gamma\) is a carrier/history label, and \(V\) is the physical output. Its input and output marginals are normalized. The unmarked kernel, trajectory, cutoffs, geometry convention, and reset normalizers remain fixed when insertion labels are introduced.

Let

\[
w_\gamma(V)=\Pi(\gamma\mid V),\qquad
f_\gamma(V)=\mathbb E_\Pi[F\mid \gamma,V],\qquad
g_\gamma(V)=\mathbb E_\Pi[G\mid \gamma,V].
\tag{H7.1}
\]

These are conditional expectations on the disjoint union of the carrier-specific spaces; different reset geometries need not share an exterior coordinate. The exact conditional covariance is

\[
\operatorname{Cov}(F,G\mid V)
=\sum_\gamma w_\gamma(V)
\operatorname{Cov}(F,G\mid\gamma,V)
+\operatorname{Cov}_{w(V)}(f_\gamma,g_\gamma).
\tag{H7.2}
\]

An estimate for the first term on a fixed carrier is not yet an estimate for the second term. No history-dependent subtraction from the physical observable is performed below.

#### 1.1 The source already gives an exact way to remove old integral operations

LFR II, printed pp.391–392, (1.103)–(1.104), gives a useful alternative representation for a fixed family of remaining old large-field regions \(Y_1,\ldots,Y_r\). For the real positive operations, put

\[
z_i(V)=\mathcal T_k(Y_i)1,\qquad
\widehat{\mathcal T}_i=\frac{\mathcal T_k(Y_i)}{z_i(V)}.
\tag{H7.3}
\]

On nonzero support, \(\widehat{\mathcal T}_i1=1\). With the other variables held fixed, the relevant factor is exactly

\[
\left(\prod_i\mathcal T_k(Y_i)\right)e^{B}
=\left(\prod_i z_i\right)
\left(\prod_i\widehat{\mathcal T}_i\right)e^{B}.
\tag{H7.4}
\]

The normalized bracket has a connected boundary expansion. The source uses ordinary connectedness in that expansion but explains that its decay need not pay for the internal size of \(Y_i\): the \(Y_i\) are fixed, with no sum over those regions in that argument. The final expression retains \(z_i\) as scalar multipliers of the effective density. The remaining new-region operations in (1.104) have not all disappeared.

Frozen old sources can be inserted into the integrand of (H7.4) before the operations are performed. Distinct nilpotent labels retain all degree-one and degree-two coefficients exactly. The source normalization is thereby preserved; no source-dependent reset kernel is differentiated.

This representation removes old integration variables from the chosen \(Y_i\). It does not remove their old-source responses. Those responses occur in the normalized bracket and in the resulting functions of the exterior/current fields.

In particular, the rare multiplier \(\prod_i z_i\) is independent of the labels when the operations are frozen. It cancels from the logarithm of the *fixed-family conditional* generating function. It reappears only when that conditional coefficient is weighted by the actual outer density. One must retain this distinction when using its smallness.

### 2. A completed regular-\(R\) perturbation estimate

The part of \(R\) whose activities lie in the complete regular chart can be handled as a perturbation of the normalized rooted operation. This avoids a comparison between extensive partition functions.

Use the local potential norm and explicit rooted output norm in RX18. Let \(E\) be an admitted regular potential with fixed unused analytic reserve \(b_*>0\), and let \(R\) be a localized analytic potential on the same chart with

\[
\|R\|_{\mathrm{pot}}\le\varepsilon_R,\qquad
\varepsilon_R\le b_*/8.
\tag{H7.5}
\]

All coordinate maps, minimizing fields, forward kernels, fluctuation cutoffs, and integration contours are frozen. Only the factor \(e^R\) in the action density is varied. A different sign convention for the action changes the sign of the derivative below, not its bound.

For an actual admitted local insertion \(f_X\), define

\[
\mathcal M_z(f_X)
=
\frac{\int f_X\,e^{E+zR}\,d\nu_0}
     {\int e^{E+zR}\,d\nu_0}.
\tag{H7.6}
\]

The notation includes the retained exterior background. The background-dependent source-free factors in \(d\nu_0\) are not dropped.

#### Theorem H7-A: regular \(R\) is a small operator perturbation

On this carrier,

\[
\boxed{
\|\mathcal M_1(f_X)-\mathcal M_0(f_X)\|_{\mathrm{rooted}}
\le C\varepsilon_R\|f_X\|_{\mathrm{input}} .
}
\tag{H7.7}
\]

The norms retain the same root footprint, support weights, and complex-background margins as RX18. The estimate extends by summation to its admitted localized insertion class. It is an estimate for the actual normalized means.

**Proof.** Introduce an auxiliary insertion parameter \(t\), so that \(\mathcal M_z(f_X)\) is the coefficient of \(t\) in the logarithm of the source-deformed integral. For

\[
|z|\le R_z:=\frac{b_*}{2\varepsilon_R},
\tag{H7.8}
\]

the added local potential has norm at most \(b_*/2\). The RX18 source construction therefore gives the same explicit rooted expansion, holomorphic in \(z\), with

\[
\sup_{|z|\le R_z}
\|\mathcal M_z(f_X)\|_{\mathrm{rooted}}
\le C_0\|f_X\|_{\mathrm{input}}.
\tag{H7.9}
\]

Use the common coefficientwise localized expansion, not an uncontrolled choice of minimizing decompositions for each \(z\). Cauchy's formula can then be applied term by term and summed with the fixed rooted weights. Since \(R_z\ge4\), a circle of radius \(R_z/2\) around each real \(z\in[0,1]\) remains in the admitted disk. Consequently

\[
\|\partial_z\mathcal M_z(f_X)\|_{\mathrm{rooted}}
\le \frac{2C_0}{R_z}\|f_X\|_{\mathrm{input}}
\le C\varepsilon_R\|f_X\|_{\mathrm{input}}.
\tag{H7.10}
\]

Integrate from zero to one. For real \(z\), direct differentiation also gives the exact identity

\[
\partial_z\mathcal M_z(f_X)
=\operatorname{Cov}_{E+zR}(f_X,R).
\tag{H7.11}
\]

The normalized denominator supplies the second term in this covariance. There is no inverse global partition-function estimate. \(\square\)

This theorem has direct source support. CMP119, printed pp.270–271, (3.26)–(3.27), already separates recent \(R\)-terms through an interpolation parameter in the normalized fluctuation measure. The new estimate supplies a rooted *marked* operator bound for that interpolation, using the uniform source neighborhood proved in RX18.

For fresh regular \(R\)-activities, LFR II (1.100) gives the stronger smallness \(e^{-p_0(g_k)}\), and the ordinary activity decay supplies the norm in (H7.5), after reserving the input and output localization exponents. Thus their contribution to (H7.7) has this rare factor.

For accumulated \(R\)-terms, one must use their actual norm, rather than relabeling it \(e^{-p_0(g_k)}\). CMP119 (2.31) provides individual analytic bounds \(g_j^{\kappa_0}e^{-\kappa d_j(X)}\), with \(\kappa_0\) selectable sufficiently large. The paper absorbs sufficiently old translation-compatible \(R\)-terms into \(E_k\), retaining the recent terms separately in (3.26). Any conversion from birth-scale norms to the current norm must be included.

The source's real-field estimate (2.44) is an absolute value of a sum of vacuum-subtracted \(R\)-terms; it is not itself a bound on the absolute complex rooted norm used here. The individual analytic estimate (2.31), together with an actual chart conversion, is the correct input for (H7.5).

#### 2.1 A useful summation check for recent \(R\)-terms

Suppose the regular chart conversion of a birth-\(j\) term loses at most

\[
C L^{c(k-j)}x_j^a,\qquad x_j=g_j^{-2},
\tag{H7.12}
\]

with fixed \(a,c\), and retains the required localization reserve. For the source's recent terms, the split implies \(L^{k-j}\le CMR_j\). Since \(R_j\) is polylogarithmic in \(x_j\), the converted norm is at most \(C x_j^{-\kappa_0/2+a+\epsilon}\) for any fixed \(\epsilon>0\), after changing \(C\).

Using \(x_j\ge x_k+c_-(k-j)\), choose \(\kappa_0\) once so that \(\kappa_0/2-a-\epsilon>q+1\). Then

\[
\sum_{\text{recent }j}\varepsilon_{j\to k}
\le C_q x_k^{-q}.
\tag{H7.13}
\]

The proof may sum over all \(j\le k\) after the bound has been obtained for recent \(j\); a separate count of recent scales is unnecessary. This is a proved numerical implication of (H7.12), not an assertion that every multiscale boundary chart already satisfies (H7.12).

The same Cauchy argument as H7-A applies to a two-source connected coefficient *when its full two-root norm is known uniformly in the same complex potential neighborhood*. It preserves that norm's separation factor. A one-root estimate alone is not used to invent the required two-root theorem.

### 3. Asynchronous entry into protected old cores

The first-meeting argument does not require every seed to have the same microscopic birth scale. This matters for marks that first evolve regularly and then enter an unresolved component.

Let \(h_j=aL^j\le1\), and set \(T(h)=1+\log(1/h)\). In each selected history, mark \(i\) enters the retained old-variable class at scale \(b_i\), with the actual pointwise incoming bound

\[
|F_i|\le A_i h_{b_i}^{-4}T(h_{b_i})^s.
\tag{H7.14}
\]

The \(b_i\) may differ, and may be determined by the selected local history. The constants \(A_i\) and fixed \(s\) are uniform over those histories. After entry, the complete marked support remains in its unresolved ancestry until the chosen component operation; all roots end in the same final component \(X\). Its root remains in the ancestry or in its stated fixed protective collar. Every source selector is fixed independently of the subset of labels extracted.

#### Theorem H7-B: protected asynchronous entry

Fix \(\epsilon>0\). Under the same source budget reserve as PC-A, enlarged by a fixed amount depending on \(s,\epsilon\), the actual matched component operation obeys, for \(m\ge2\) and distinct roots,

\[
\boxed{
\left|\mathcal T'_k(X)\prod_iF_i\right|
\le C^{m+1}(m!)^{4+\epsilon}
\left(\prod_iA_i\right)
\delta^{-4m}T(\delta)^{sm}
\eta_k e^{-\kappa_*d_k(X)} .
}
\tag{H7.15}
\]

The threshold is independent of \(m\) and of the entry times. The one-root estimate is

\[
|\mathcal T'_k(X)F_i|
\le CA_i h_k^{-4}T(h_k)^s
\eta_k e^{-\kappa_*d_k(X)}.
\tag{H7.16}
\]

**Proof.** A root is active only after its entry. Charge its scale growth while its current component contains no other already-born root. Stop immediately before the first meeting with another already-born root. If it is born into a component already carrying a root, stop it at birth; no preceding age charge is assigned to it.

For a root charged from \(b\) through \(r\), factor its scale exactly:

\[
h_b^{-4}T(h_b)^s
=h_r^{-4}T(h_r)^s
\prod_{j=b+1}^{r}
\left[L^4\left(\frac{T(h_{j-1})}{T(h_j)}\right)^s\right].
\tag{H7.17}
\]

Since \(T(h_{j-1})/T(h_j)\le1+\log L\), the logarithmic charge per charged component-step is at most

\[
4\log L+s\log(1+\log L).
\tag{H7.18}
\]

Every such component-step carries at most one charged root. Components with several born roots carry no new charge, though they can receive newly born roots or later singletons. The source positive history budget therefore needs only one fixed enlargement.

Group stopped roots by their stopping component-step \((j,Z)\). At every such event the component contains at least two born roots, so its ordinary geometric reserve satisfies \(q_j(Z)\ge c\delta/h_j\). For an older root its remaining scale is \(h_{j-1}\); for a root born into the marked component it is \(h_j\). The difference costs at most \(L^4\) and one fixed logarithmic factor per root. With \(u=\delta/h_j\),

\[
h_r^{-4}T(h_r)^s
\le C\delta^{-4}T(\delta)^s
u^4(1+\log_+u)^s.
\tag{H7.19}
\]

Use \((1+\log_+u)^s\le C_{s,\epsilon}(1+u)^\epsilon\). A stopping event with \(n\) newly stopped roots is bounded by

\[
C^n\delta^{-4n}T(\delta)^{sn}
u^{4n}(1+u)^{\epsilon n}e^{-cu}
\le C^n(n!)^{4+\epsilon}
\delta^{-4n}T(\delta)^{sn}.
\tag{H7.20}
\]

Different stopping events are different component-steps, and the groups partition the labels. Thus their factorials multiply to at most \((m!)^{4+\epsilon}\). Apply the unchanged positive history majorant with the fixed charge (H7.18). For an initial-scale indexing event, using the first active output component costs one further fixed \(L^4\) factor per root, as in PC-C. The one-root proof charges from its own entry through \(k\). \(\square\)

The result starts from the actual incoming norm at \(b_i\). It does not pay the earlier regular age. If only a microscopic bound is available at entry, the missing amplification remains in \(A_i\).

A first-entry construction can keep the value of a mark from the last regular state as the old seed. It need not evaluate a regular analytic formula on a new large-field configuration outside that formula's domain. This avoids an unnecessary analytic continuation at the moment of entry. The boundedness of that old seed follows from the regular-state norm, while its subsequent positive transport uses the old variables.

After a successful reset and a later re-entry, this theorem can be restarted only after the returned mark has again been shown to possess the common incoming norm. The existence of that return, including its boundary dependence, is not supplied by (H7.15).

### 4. Partial-support insertions at one component operation

At a single frozen component operation, the full support of an incoming local mark need not lie inside the component in order to obtain the elementary operator estimate. Exterior variables can remain as parameters.

Let \(f_S(u_{\mathcal Y},b)\) have support \(S\), with \(b\) the unchanged exterior, and let \(\mathcal Y\) be disjoint component domains whose operations are applied. On the actual integration domain assume

\[
\sup|f_S|\le A_S,\qquad
\|\mathcal T_Y\|_+\le w(Y)
\le C\eta e^{-\kappa_{\rm LF}\ell(Y)}.
\tag{H7.21}
\]

The positive majorant may include the fixed \(e^{|\sigma|}\) factor used in the analytic continuation of LFR II (1.73). Then

\[
\left|\left(\prod_{Y\in\mathcal Y}\mathcal T_Y\right)f_S\right|
\le A_S\prod_{Y\in\mathcal Y}w(Y).
\tag{H7.22}
\]

The output support is contained in \(S\cup\bigcup_{Y\in\mathcal Y}Y\), with the source's fixed collars. If the input and kernel are holomorphic on the same exterior chart with a uniform bound, dominated integration gives holomorphy on that chart. This is a statement about the original positive/gauge-fixed kernel. A reversed Faddeev–Popov identity is not applied separately to a noninvariant localized piece.

#### Lemma H7-C: summing component attachments costs a stronger input weight

Suppose every component in \(\mathcal Y\) meets \(S\), and its weighted anchored sum obeys

\[
\sup_b\sum_{Y\ni b}w(Y)e^{\kappa\ell(Y)}
\le c_0\eta.
\tag{H7.23}
\]

Choose a length \(\ell\ge1\) that counts the root/support collar and is subadditive on connected unions. Assume the number of blocks in \(S\) is at most \(c_1\ell(S)\). Ignoring disjointness only enlarges the positive sum, so

\[
\begin{aligned}
\sum_{\substack{\mathcal Y\ne\varnothing\\Y\cap S\ne\varnothing}}
\prod_{Y\in\mathcal Y}w(Y)e^{\kappa\ell(Y)}
&\le
\exp\!\left(\sum_{Y:Y\cap S\ne\varnothing}
w(Y)e^{\kappa\ell(Y)}\right)-1\\
&\le C\eta\,\ell(S)e^{C\eta\ell(S)}.
\end{aligned}
\tag{H7.24}
\]

Here an unordered family is counted once; equivalently its ordered enumeration carries \(1/n!\). The fixed touching collar changes \(C\).

For any fixed stronger input weight \(\kappa+\gamma\), take \(\eta\) small enough that \(C\eta\le\gamma/2\). Equations (H7.22)–(H7.24) then imply

\[
\boxed{
\sum_S\sum_{\mathcal Y\ne\varnothing}
e^{\kappa\ell(S\cup\mathcal Y)}
\left|\left(\prod_{Y\in\mathcal Y}\mathcal T_Y\right)f_S\right|
\le C_\gamma\eta
\sum_S e^{(\kappa+\gamma)\ell(S)}A_S .
}
\tag{H7.25}
\]

This proves an actual one-operation support attachment bound. It includes a stencil or a localized tail that straddles a processed core boundary, provided its norm on the actual joint input domain is supplied. For two insertions, insert their product as one marked hyperedge on the union of the supports; all source labels remain distinct and no mark is assigned twice.

Additional unmarked Mayer links and subsequent connected normalization must still be included. On the carrier of CG with no remaining \(Y_i\), the same submultiplicative finite-source expansion performs that normalization. With remaining unprocessed \(Y_i\), (H7.25) remains an unnormalized operation/attachment estimate; it does not replace the normalization issue in Sections 6–7.

For a mark straddling a boundary during many subsequent scales, its exterior part also undergoes regular evolution. That mixed-boundary evolution needs a compatible chart and localization theorem. The one-operation estimate does not declare that long history closed.

### 5. Posterior history means can be controlled without sub-Gaussian tails

The earlier posterior–Herbst estimate required a sub-Gaussian bound for the old mark under the same complete law. A different estimate needs only a good-sector mean and a posterior-weighted bad second moment.

Let \(B\) be any measurable bad event in the joint input/carrier/output space. It may unite arbitrarily many histories and geometries. At a fixed output let

\[
p(V)=\Pi(B\mid V),\qquad q(V)=1-p(V),
\]

\[
m_G^F(V)=\mathbb E[F\mid V,B^c],\qquad
C_G(V)=\operatorname{Cov}(F,G\mid V,B^c).
\tag{H7.26}
\]

On the set \(q=0\), define \(m_G^F\) arbitrarily and set \(qC_G=0\). The bounds below require finiteness of the displayed marked second moments; if a right side is infinite, the inequality remains valid but uninformative. Real marks are written for clarity.

#### Theorem H7-D: exact good/bad covariance remainder

Set

\[
U_F=\mathbb E_\Pi\!\left[1_B|F-m_G^F(V)|^2\right],
\qquad
U_G=\mathbb E_\Pi\!\left[1_B|G-m_G^G(V)|^2\right].
\tag{H7.27}
\]

Then

\[
\boxed{
\mathbb E_{\mu'}\left|
\operatorname{Cov}(F,G\mid V)-q(V)C_G(V)
\right|
\le\sqrt{U_FU_G}.
}
\tag{H7.28}
\]

This includes the covariance of posterior history means between the good and bad sectors. It neither bounds nor divides by the probability of an individual history.

**Proof.** Write \(m_B^F=\mathbb E[F\mid V,B]\), and likewise for \(G\). The exact binary mixture identity is

\[
\operatorname{Cov}(F,G\mid V)
=qC_G+pC_B
+pq(m_B^F-m_G^F)(m_B^G-m_G^G).
\tag{H7.29}
\]

Define the centered, selected marks

\[
X_F=1_B(F-m_G^F(V)),\qquad X_G=1_B(G-m_G^G(V)).
\tag{H7.30}
\]

Expanding their conditional covariance gives the exact identity

\[
\operatorname{Cov}(F,G\mid V)-qC_G
=\operatorname{Cov}(X_F,X_G\mid V)
=pC_B+pq(m_B^F-m_G^F)(m_B^G-m_G^G).
\tag{H7.31}
\]

Conditional Cauchy–Schwarz bounds its absolute value by
\(\{\mathbb E[X_F^2\mid V]\mathbb E[X_G^2\mid V]\}^{1/2}\).
Outer Cauchy–Schwarz proves (H7.28). The limiting cases \(p=0\) or \(q=0\) obey the same identity; when \(q=0\), the chosen comparison values are constants given \(V\) and do not change conditional covariance. \(\square\)

The comparison mean \(m_G^F(V)\) is common across the bad histories at a given output. It is used inside an exact covariance identity; it is not subtracted from the physical observable. Its own variation in \(V\) remains part of the transported mean and terminal covariance.

#### Corollary H7-D1: use a deterministic common subtraction and a regular mean bound

Suppose \(c_F,c_G\) are deterministic common constants and

\[
|m_G^F(V)-c_F|\le K_F,\qquad
|m_G^G(V)-c_G|\le K_G.
\]

Let

\[
B_F=\mathbb E[1_B|F-c_F|^2],\quad
B_G=\mathbb E[1_B|G-c_G|^2],\quad p_*=\Pi(B).
\tag{H7.32}
\]

Then \(U_F\le2(B_F+K_F^2p_*)\), and

\[
\boxed{
\mathbb E\left|
\operatorname{Cov}(F,G\mid V)-qC_G
\right|
\le
2\sqrt{(B_F+K_F^2p_*)(B_G+K_G^2p_*)}.
}
\tag{H7.33}
\]

For physical bounds \(K_F\le A_Fh^{-4}\), \(K_G\le A_Gh^{-4}\), together with

\[
p_*\le C\eta,\qquad
B_F\le C A_F^2h^{-8}\eta,\qquad
B_G\le C A_G^2h^{-8}\eta,
\tag{H7.34}
\]

the entire bad-sector covariance remainder is at most \(CA_FA_Gh^{-8}\eta\). There is no square-root loss of the rare factor when both marked masses carry that factor.

Equation (H7.34) must hold under the actual normalized joint law. The source component numerator bound does not establish it by itself. The estimate also does not supply separation decay when the definition of \(B\) and the marked mass carry none.

#### 5.1 Exact elimination of additional history variables

Inside a single joint law, take a finite nested reveal filtration
\(\mathscr H_0\subset\cdots\subset\mathscr H_n\), with \(\mathscr H_0\) containing the physical output. Set

\[
M_j^F=\mathbb E[F\mid\mathscr H_j],\qquad
\Delta_j^F=M_j^F-M_{j-1}^F.
\]

Conditional martingale orthogonality gives

\[
\operatorname{Cov}(F,G\mid\mathscr H_0)
=\mathbb E[\operatorname{Cov}(F,G\mid\mathscr H_n)\mid\mathscr H_0]
+\sum_{j=1}^n
\mathbb E[\Delta_j^F\Delta_j^G\mid\mathscr H_0].
\tag{H7.35}
\]

For \(i<j\), the conditional expectation of \(\Delta_i^F\Delta_j^G\) given \(\mathscr H_0\) vanishes because \(\Delta_i^F\) is \(\mathscr H_{j-1}\)-measurable and \(\mathbb E[\Delta_j^G\mid\mathscr H_{j-1}]=0\). This proves the formula by expanding \(M_n-M_0\) and applying the conditional covariance identity once.

Bounded stopping times or stopping lines along a specified finite reveal order may group these increments. The factors \(1_{\{\sigma<j\le\tau\}}\) are predictable, so the same orthogonality applies. This permits a first-entry/last-reset bookkeeping without adding a separate entropy factor for every history label.

Discarding a carrier label therefore moves its covariance into an exact reveal increment. It does not erase it. Formula (H7.35) is internal to one joint operation; it does not assert nested sigma-algebras for the entire RG chain.

### 6. Restoring ordinary distance across collapsed regions

There is a direct geometric way to use the remaining large-field reserve.

Work in current block units. Let \(d_0\) be ordinary distance, and \(d_{\mathcal Y}\) the quotient distance obtained by giving each disjoint connected region \(Y\in\mathcal Y\) zero internal cost. Choose a shortest quotient path from \(x\) to \(y\), with a fixed tie-breaking rule. A simple path uses each contracted region at most once. Let \(\mathcal Y_{xy}\) denote its used regions.

Lifting the path to the original lattice and joining each entry and exit inside the ambient lattice proves

\[
d_0(x,y)
\le d_{\mathcal Y}(x,y)
+C_{\rm geo}\sum_{Y\in\mathcal Y_{xy}}\ell(Y).
\tag{H7.36}
\]

The length \(\ell(Y)\) may be the ordinary spanning-tree/block length with a fixed collar. It dominates the ambient diameter of \(Y\); no internal shortcut is counted as ordinary decay.

Consequently, for \(s>0\) and any nonnegative amplitude \(A\),

\[
A e^{-s d_{\mathcal Y}(x,y)}
\le e^{-s d_0(x,y)}
A\exp\!\left[sC_{\rm geo}
\sum_{Y\in\mathcal Y_{xy}}\ell(Y)\right].
\tag{H7.37}
\]

An actual normalized marked exponential moment,

\[
\mathbb E\!\left[
A\exp\!\left(sC_{\rm geo}\sum_{Y\in\mathcal Y_{xy}}\ell(Y)\right)
\right]\le M,
\tag{H7.38}
\]

would therefore give ordinary decay \(M e^{-s d_0(x,y)}\). The same proof applies termwise to an absolute connected expansion whose regular supports and used large-field regions form a lifted connected graph. Each distinct used region is paid once; repeated traversals are removed by the simple-path choice.

#### 6.1 The source supplies the unnormalized size reserve

LFR II, printed p.387 immediately after (1.89), explicitly extends its positive operation estimate to arbitrary large-field regions, with an additional ordinary spatial penalty \(-\kappa_{\rm LF}d_k(Y)\). This statement is stronger than the collapsed-metric estimate for the subsequent boundary activities.

The fixed-overhead argument of PC-A can reserve a chosen finite portion of this ordinary penalty and a geometric exponential moment. Thus the size cost in (H7.37) can be paid at the positive component-majorant level, together with a fixed degree-two engineering charge, without a new scale-dependent threshold.

The conclusion is an unnormalized operation estimate. To obtain (H7.38), the corresponding marked masses must be placed in the actual normalized outer law with an anchored relative partition estimate. That is the remaining analytic task; the metric conversion itself is proved.

### 7. The remaining normalized large-field estimate is explicit

The precise missing input can be stated as a marked local ratio bound. For a connected root-support configuration \(\mathcal C\), let \(\mathcal Y(\mathcal C)\) be its distinct unresolved components. First construct an exact covariance/reveal expansion or an absolute domination of it. Let \(N_{\mathcal C}^{(2)}\) be its positive degree-two old-mark majorant, with all posterior factors, matching reset normalizers, cutoff factors, exterior interactions, and history summations retained. The existence of this correctly normalized connected majorant is part of the required construction; it is not identified with a bare source component numerator by notation.

A sufficient estimate is

\[
\boxed{
\frac1Z\sum_{\mathcal C\ {\rm anchored}}
\int N_{\mathcal C}^{(2)}
\exp\!\left[
\lambda\ell_{\rm outside}(\mathcal C)
+\lambda C_{\rm geo}
\sum_{Y\in\mathcal Y(\mathcal C)}\ell(Y)
\right]
\le C h^{-8}\eta_k .
}
\tag{H7.39}
\]

The marked numerator is understood as a positive absolute majorant appropriate to the chosen covariance/reveal decomposition. A one-root second-moment version controls the quantities in (H7.34); a two-root connected version supplies the separation factor through (H7.36). Every quantity in (H7.39) uses the same full partition function and frozen positive law.

The source does provide:

- The positive component bounds, including ordinary component size.
- Analytic background bounds for the normalized component operations.
- The fixed-family boundary expansion (1.103)–(1.104).
- Source-free global stability.

The cited statements do not yet give (H7.39). In particular, CMP119, printed p.264, (2.50), bounds the full density above by an exponential of the total coarse volume and gives a lower bound on the complete regular-cutoff sector. On an output containing large fields that lower bound can vanish. Dividing a local numerator estimate by this global lower bound would introduce an extensive volume factor or yield no lower bound at all.

Even the elementary positive example with unnormalized weights

\[
w_{\rm bad}=\varepsilon,\qquad
w_{\rm good}=\varepsilon^2
\tag{H7.40}
\]

has a small bad weight but normalized bad probability \(1/(1+\varepsilon)\). This is a counterexample to that inference, not to the Yang–Mills estimate sought here.

A concrete way to finish (H7.39) is an anchored partition-ratio theorem: compare the partition integral with a specified connected marked large-field family present to the original partition integral, cancel the exterior vacuum factors locally, retain the matching Wilson/minimizer terms, and use the component size reserve for the inserted family and its boundary attachments. The comparison must cover the compulsory large-field geometry of the output; an empty-core comparison is unavailable when its cutoff vanishes.

An alternative is a single absolute connected expansion of the normalized history law in an enlarged boundary-source norm. In that construction the ordinary size penalties must be assigned to used large-field components before the collapsed metric is converted. Either strategy must also keep the old incoming mark in the same analytic class while its support straddles a boundary.

### 8. A normalized initial-birth theorem on the original Wilson measure

There is one source-specific sector in which normalization can be supplied directly, without an anchored exterior partition comparison. Work first with the original, pure Wilson measure

\[
d\mu_\beta(U)=Z_\beta^{-1}e^{-\beta A(U)}\prod_e dU_e,\qquad
\beta=g_0^{-2},
\quad
A(U)=\sum_p\bigl(N_c-\operatorname{Re}\operatorname{Tr}U(\partial p)\bigr).
\tag{H7.41}
\]

Normalized trace conventions change only constants. The compact matrix gauge group is fixed. For the Frobenius norm the plaquette action is exactly \(\frac12\|1-U(\partial p)\|_F^2\); any fixed equivalent matrix norm has the corresponding positive lower bound.

Use the literal source tori. CMP109, printed p.251, takes odd fixed \(L>11\), physical side lengths \(2L^{m_\mu}\), and lattice spacing \(L^{-n}\); hence the fine side lengths are \(2L^{m_\mu+n}\). Tile their vertices by cubes of fixed side \(B_{\rm tile}=L\). The number of tiles in each direction is \(2L^{m_\mu+n-1}\), which is even. Tile boundary reflections are fine-lattice bond-plane reflections. Thus the blocked chessboard inequality applies without changing the source tori. More generally any fixed integer tile side at least two with an even number of tiles in every direction suffices. No reflection positivity is assumed for an effective or reset law.

#### Theorem H7-E: normalized initial source-cube rarity

Let \(\mathcal B_0\) be the source partition into cubes of side \(B_0=LM_2R_0\). Let \(E_C\) be precisely the initial bad-cube event from CMP119 (1.1): a plaquette in its prescribed fixed neighborhood violates
\(\|1-U(\partial p)\|<\varepsilon_0\), where

\[
\varepsilon_0=g_0p_0(g_0),\qquad
p_0(g_0)=A_0(\log\beta)^{P},\quad P\ge5r,
\qquad R_0\le C(\log\beta)^r .
\tag{H7.42}
\]

For every finite specified family \(\mathcal S\subset\mathcal B_0\), uniformly in the torus and cutoff,

\[
\boxed{
\mu_\beta\!\left(\bigcap_{C\in\mathcal S}E_C\right)
\le \exp\{-c_b p_0(g_0)^2|\mathcal S|\}.
}
\tag{H7.43}
\]

The weak-coupling threshold and \(c_b>0\) are independent of \(\mathcal S\).

**Proof.** The all-link identity neighborhood gives an elementary extensive lower bound for the *same* partition function. Restrict every independent link to a ball of radius \(c\beta^{-1/2}\) around the identity. Haar volume of that ball is at least \(c_1\beta^{-\dim G/2}\), and unitarity bounds the defect of each plaquette by the sum of its four link defects. Consequently, for \(N\) lattice sites,

\[
Z_\beta\ge \exp\{-C N(1+\log\beta)\}.
\tag{H7.44}
\]

Fix one of the \(B_{\rm tile}^d\) phases of the disjoint vertex tiles
\(B_{\rm tile}z+u+\{0,\ldots,B_{\rm tile}-1\}^d\), where
\(u\in\{0,\ldots,B_{\rm tile}-1\}^d\). In a tile \(D\), let \(E_D\) mean that at least one plaquette wholly internal to \(D\) violates the threshold in an invariant matrix norm. If the source norm differs, use the Frobenius norm and threshold \(c\varepsilon_0\), with \(c>0\) chosen by finite-dimensional norm equivalence so that each source violation is included. This event is unchanged by the reflections that disseminate it to other tiles: inversion and conjugation do not change its norm.

Wilson reflection positivity and the block chessboard inequality give, for a specified set \(\mathcal T\) of these tiles,

\[
\mu_\beta\!\left(\bigcap_{D\in\mathcal T}E_D\right)
\le
\left(\frac{Z_{\rm all\ tiles\ bad}}{Z_\beta}\right)^{|\mathcal T|/N_{\rm tile}}.
\tag{H7.45}
\]

Here \(N_{\rm tile}=B_{\rm tile}^{-d}N\). The block version follows from the same reflection Cauchy–Schwarz argument using tile boundary planes: the fine Wilson measure is reflection positive at those planes, and the blocked periodic rectangle has even side lengths, precisely the hypothesis of the chessboard theorem. No power-of-two side-length assumption is needed. The completely disseminated event forces at least one bad internal plaquette per tile, and these plaquettes are distinct. Hence
\(Z_{\rm all\ tiles\ bad}\le \exp\{-c\beta\varepsilon_0^2N_{\rm tile}\}\).
Combining this with (H7.44) proves

\[
\mu_\beta\!\left(\bigcap_{D\in\mathcal T}E_D\right)
\le
\exp\{-|\mathcal T|[c p_0(g_0)^2-CB_{\rm tile}^d(1+\log\beta)]\}.
\tag{H7.46}
\]

Every microscopic plaquette is internal to a tile in at least one phase. Within a fixed phase, only \(O_d(B_{\rm tile}^d)\) plaquettes fit in one tile. Thus a family of \(n\) specified distinct bad plaquettes contains at least \(n/C_{d,L}\) plaquettes in distinct tiles of one phase. Its joint event is bounded by (H7.46), with a changed constant. Both the number of phases and this loss depend only on the fixed \(L,d\); the extra \(B_{\rm tile}^d\log\beta\) cost is absorbed by \(p_0(g_0)^2\).

For \(m=|\mathcal S|\), choose one violating plaquette for each source cube. A fixed plaquette belongs to the prescribed neighborhoods of at most a fixed number of source cubes; this remains true for the small enlargement in (1.1). Therefore every such choice contains at least \(m/C\) distinct plaquettes. There are at most \((CB_0^d)^m\) choices. The union bound now gives an exponent
\(-c p_0^2m+C m\log B_0+C m(1+\log\beta)\).
Since \(p_0^2\) grows faster than \(\log\beta\), while \(\log B_0=O(\log\log\beta)\), this proves (H7.43). \(\square\)

The external primary input is the Wilson-measure reflection positivity and chessboard theorem of Brydges, Fröhlich, and Seiler, *On the Construction of Quantized Gauge Fields I. General Results*, IHES/P/78/237 (1978), Theorems 2.8 and 2.10, printed pp.36 and 40. [Primary preprint](https://repo-archives.ihes.fr/FONDS_IHES/I_Prepublications/FROHLICH/1978-1980/P_78_237/P_78_237_web.pdf). The source-specific threshold and neighborhood are those of CMP119, printed p.246, (1.1); this is the original plaquette event, not the nonlinear next-stage selector (1.4).

#### 8.1 Passage to an arbitrary actual positive lift

Let \(\Pi\) be any actual positive joint history law with original marginal \(\mu_\beta\). No property of its conditional kernels beyond positivity and the correct marginal is needed here. If \(E\) is an initial event and \(\mathscr H\) is any retained sigma algebra, conditional Jensen gives

\[
\mathbb E_\Pi\!\left[
\Pi(E\mid\mathscr H)
\left|\mathbb E_\Pi[F\mid E,\mathscr H]\right|^2
\right]
\le \mathbb E_{\mu_\beta}[1_E|F|^2].
\tag{H7.47}
\]

The same statement holds for a history event \(C\) contained in \(E\), with \(1_C\) on the right before using \(1_C\le1_E\). Thus a bounded microscopic seed \(|F|\le A a^{-4}T(a)^s\) has normalized marked mass
\(A^2a^{-8}T(a)^{2s}e^{-c_bp_0^2m}\) on a specified \(m\)-cube initial-birth event. The actual posterior weight is essential in (H7.47).

This proves normalization at initial birth. Its bare \(a^{-8}\) factor alone is insufficient to control a mark that remains unresolved for arbitrarily many later scales. The clean geometry supplies the additional information needed for one restricted aged sector.

### 9. Normalized clean descendants of initial births

Call a descendant of an initial large-field component **clean until scale \(j\)** if its ancestry contains only the specified initial \(P_0\) bad cubes, has no subsequent large-field creation or failed preparation, has no merger with another component, and has not yet been successfully reset. In the first transformation, the other new selectors must also be absent in this component. Outside it, no restriction is imposed. This definition concerns a sector of the actual positive lift; it does not change its measure.

Let \(m\ge1\) be the number of initial bad source cubes in that component. These cubes form an animal in a fixed finite-range adjacency graph: the range accounts for the fixed covers and collars in the first transformation. The number of such animals through a specified source cube is at most \(A_{\rm an}^m\). This is an ordinary bounded-degree graph count, with constants independent of \(R_0\).

#### 9.1 The precise source geometry used

The following consequences use only the actual source construction.

1. The initial active region is obtained from its bad source cubes by fixed-range covers and layers. The optional rectangular fill is applied only to components contained in a cube of side \(100MR_1\). Thus its initial source size is at most \(Cm\). CMP119, printed p.251, (1.20) and the following paragraph, describes this fill; (2.3) retains the convention.
2. With no new large field, LFR II, printed pp.384–385, defines the successor operation \(S\) by the coarse cover and ten new layers and states \(Z_{n+1}=S(Z_n)\) in (1.83). Its estimate preceding (1.81) contracts the unthickened size by at least \(2^{-n}\). Once that size reaches zero, the descendant is contained in a cube of side \(64MR_n\). At most \(R_1\) further clean steps supply the clean window.
3. LFR I, printed p.177, defines \(Z\) as the union of all components satisfying the size and clean-window conditions (i), (ii). The operations on these components are performed in (1.99)–(1.100), pp.200–201. A preparation failure moves the component into the remaining class and is excluded by the definition of the clean sector. Therefore an unresolved clean descendant cannot continue past this eligibility window.

Consequently there are fixed constants \(C_0,C_1,\alpha>0\) such that, whenever this clean descendant is unresolved at scale \(j\),

\[
j\le K(m):=C_0+C_1R_0+\alpha\log(m+1).
\tag{H7.48}
\]

The fixed shift from initial plaquettes to the first active component is included in \(C_0\). This is a bound on a clean unresolved lifetime, not on arbitrary histories that keep acquiring new large fields. The source permits \(N\le R_k\); using the larger birth-scale window in (1.80) gives the displayed upper bound. CMP119 (2.5)–(2.7) give \(R_n\le C R_0\) for subsequent scales in this argument; strict monotonicity of the rounded \(R_n\) is unnecessary.

In physical coordinates, the same covers and layers also give

\[
\operatorname{diam}Z_j
\le C_{\rm geom}aR_0(m+L^j),\qquad h_j=aL^j.
\tag{H7.49}
\]

Indeed, the initial diameter is at most \(CaR_0m\), while the later collars contribute at most
\(C\sum_{n\le j}h_nR_n\le C h_jR_0\).
Taking a rectangular hull does not enlarge the coordinate diameter. A fixed mark-support collar can be included by increasing \(C_{\rm geom}\).

For a fixed root \(x\), a descendant containing \(x\) can originate from at most
\(C(m+L^j)^d\) choices of an initial source-cube anchor. This root-location entropy must be counted: the root need not have belonged to the initial bad region.

#### Theorem H7-F: normalized current-scale marked mass of the clean sector

Let \(C_j(x)\) denote the event that \(x\), with its prescribed fixed support collar, lies in a clean unresolved descendant at scale \(j\). For fixed \(s\ge0\) and a seed satisfying
\(|F_x|\le A_xa^{-4}T(a)^s\), one has

\[
\boxed{
\mathbb E_\Pi[1_{C_j(x)}|F_x|^2]
\le C_sA_x^2h_j^{-8}T(h_j)^{2s}
e^{-c_*p_0(g_0)^2}.
}
\tag{H7.50}
\]

The same bound holds for every posterior-weighted conditional second moment in (H7.47), with the clean event. Constants are independent of \(j\), the total number of RG scales, and the torus.

**Proof.** Set \(Q=p_0(g_0)^2\). Combining the animal count, anchor count, original normalized family bound, and the necessary survival condition gives

\[
\Pi(C_j(x))
\le C\sum_{m\ge1}
(m+L^j)^d A_{\rm an}^m
e^{-c_bQm}\,1_{\{j\le K(m)\}}.
\tag{H7.51}
\]

No number of later histories multiplies this bound: for each original configuration their conditional probabilities sum to at most one. On \(j\le K(m)\), every fixed exponential age factor obeys
\(e^{Dj}\le C_D e^{C_DR_0}(m+1)^{C_D}\).
Moreover
\(T(a)/T(h_j)\le(1+\log L)^j\).
Multiply (H7.51) by
\(L^{8j}[T(a)/T(h_j)]^{2s}\), and use the anchor factor
\((m+L^j)^d\le C(m+1)^dL^{dj}\).
The resulting sum is bounded by

\[
C_s e^{C_sR_0}
\sum_{m\ge1}(m+1)^{C_s}A_{\rm an}^m e^{-c_bQm}
\le C_se^{-c_*Q}.
\tag{H7.52}
\]

Here \(Q/R_0\to\infty\) by (H7.42), and the fixed exponents, animal entropy, and \(e^{C_sR_0}\) are absorbed by part of the \(Q\)-reserve. Multiplication by
\(A_x^2h_j^{-8}T(h_j)^{2s}\) proves (H7.50). The posterior version follows from (H7.47). \(\square\)

#### Theorem H7-G: the clean same-component sector has the sharp two-root exponent

For distinct roots at physical distance \(r\in(0,1]\), let \(C_j(x,y)\) require both root supports to lie in the same clean unresolved descendant. For bounded seeds of the preceding class,

\[
\boxed{
\sum_{j:\,h_j\le1}
\mathbb E_\Pi[1_{C_j(x,y)}|F_xF_y|]
\le C_s A_xA_y\,r^{-8}T(r)^{2s}
e^{-c_*p_0(g_0)^2}.
}
\tag{H7.53}
\]

The event-weighted absolute conditional covariance inside this sector obeys the same estimate with an additional factor at most two. The conditional sigma algebra may be any one used by the actual positive lift, provided the sector conditioning is retained in that displayed term.

**Proof.** Use the elementary seed bound and sum (H7.51) with the additional spanning condition
\(r\le C_{\rm geom}aR_0(m+L^j)\).
Split the scales at \(h_j=r/(2C_{\rm geom}R_0)\).

At the coarser scales, the proof of (H7.50), applied to the product bound, yields
\(C_sA_xA_yh_j^{-8}T(h_j)^{2s}e^{-c_*Q}\).
A geometric sum of \(h_j^{-8}\), followed by
\(T(h_j)\le T(r)+\log(2C_{\rm geom}R_0)\), bounds this part by
\[
C_s A_xA_y r^{-8}T(r)^{2s}
R_0^8[1+\log(CR_0)]^{2s}e^{-c_*Q}.
\]
The extra powers of \(R_0\) are absorbed by a smaller fixed portion of the rare reserve.

At the finer scales, the spanning condition forces
\[
m\ge c\,\frac r{aR_0},\qquad
L^j\le C m.
\tag{H7.54}
\]
The anchor count is therefore at most \(C m^d\), and the number of possible ages is at most \(K(m)\). Also
\[
a^{-8}\le C r^{-8}R_0^8m^8,\qquad
T(a)\le T(r)+\log(CR_0m).
\tag{H7.55}
\]
After extracting \(r^{-8}T(r)^{2s}\), the remaining sum has only fixed powers of \(m\) and \(R_0\), the factor \(K(m)\), and \(A_{\rm an}^me^{-c_bQm}\). It is bounded by \(C_se^{-c_*Q}\) as in (H7.52). This proves (H7.53).

Finally, condition on any retained sigma algebra \(\mathscr H\) and on \(C_j(x,y)\). If \(p_j=\Pi(C_j(x,y)\mid\mathscr H)\), then
\[
\mathbb E[p_j|\operatorname{Cov}(F_x,F_y\mid
\mathscr H,C_j(x,y))|]
\le
2 A_xA_y a^{-8}T(a)^{2s}\Pi(C_j(x,y)).
\tag{H7.56}
\]
This follows by bounding the conditional product and the product of conditional means separately. The preceding geometric argument bounds the sum of the right sides. \(\square\)

These are normalized estimates for actual restricted sectors and survive arbitrary positive lifting of the original Wilson law. They apply to clean descendants, including roots reached by growing collars; no history entropy or exterior partition reciprocal has been inserted.

They do not yet cover later-born components, a failed reset, a merger, or the complete conditional-mean covariance between this sector and all its complements. H7-D can incorporate its marked second moments when the relevant complementary good mean is controlled, but it cannot delete the remaining bad sectors. Theorems H7-F and H7-G are fixed two-mark results. Their proof uses a fixed age exponent and does not claim an order-uniform factorial hierarchy for arbitrarily many marks.

A possible extension is to prove that a particular frozen blocking kernel preserves reflection positivity at the required coarse reflection planes, then verify an energy cost for the disseminated *actual* coarse birth event. Positivity of the kernel alone does not imply either statement. The nonlinear minimizer and preparation-failure selectors have not been shown to satisfy that criterion.

### 10. What this completes for Gate 3

| Interface | Result of this module | Remaining scope |
|---|---|---|
| Regular \(R\)-potential forcing | H7-A bounds the actual normalized rooted operator difference by the local potential norm; fresh regular \(R\) terms retain their rare factor | Birth-to-current conversion for every historical/background chart must be verified |
| Entry after regular evolution | H7-B extends the protected-core theorem to asynchronous actual entry scales, with one order-independent threshold | Actual incoming norms must be supplied by the common regular induction |
| One-operation boundary overlap | H7-C bounds partial-support component attachments with a fixed stronger input weight | Long mixed-boundary evolution and its return chart remain open |
| Posterior history means | H7-D controls the whole binary bad-sector covariance remainder through normalized marked second moments and the good-sector mean | The normalized marked masses and their connected spatial weights must be proved |
| Elimination/revealing of history variables | H7.35 gives exact covariance increments, including stopped reveal intervals | Those increments still require bounds; discarding labels is not a cancellation |
| Collapsed-to-ordinary distance | H7.36–H7.38 prove the metric transfer, and the source has an ordinary unprocessed-component reserve | The actual normalized marked exponential moment H7.39 remains open |
| Initial physical large-field births | H7-E gives a normalized joint rarity bound for the actual \(P_0\) source events on the literal original Wilson source tori, using fixed \(L\)-site tiles | Later nonlinear birth and preparation-failure events are not original plaquette events |
| Clean initial descendants | H7-F pays the actual unresolved age and root-location entropy; H7-G gives a normalized scale-summed \(r^{-8}T(r)^{2s}\) same-component bound | Later births, failures, mergers, mixed-sector mean covariance, and an all-order hierarchy remain outside this restricted theorem |

Together these results replace several unnecessary demands—uniform lower bounds on individual carrier masses, a common birth scale for all seeds, and a full-law sub-Gaussian premise for posterior means—with explicit usable estimates. The original-Wilson argument supplies actual normalized rarity for one nonempty family of aged histories. The full history average and its terminal covariance remain to be proved.

#### Primary sources

The following source clauses are used:

- LFR II (1989), pp.379–380, (1.71)–(1.75): matched localized operation, positive analytic majorant, and normalized operation bound.
- LFR II, pp.383–387, (1.79)–(1.89), including the paragraph after (1.89): unresolved-age budget and ordinary size reserve for arbitrary remaining regions.
- LFR II, pp.388–392, (1.90)–(1.104): regular versus boundary activities, fixed-family normalized boundary expansion, and scalar old-region weights.
- CMP119 (1988), pp.260–264, (2.30)–(2.50): analytic \(R\)-activity bound, multiscale boundary chart, real vacuum-subtracted estimates, and global stability.
- CMP119, pp.270–271, (3.26)–(3.27): normalized interpolation of recent \(R\) and boundary terms, with older compatible \(R\)-terms absorbed into \(E_k\).
- CMP119, pp.245–246, (1.1), and pp.251, 255–256, (1.20), (2.3)–(2.7): the initial plaquette event, fixed-range covers and rectangular fill, and radius bounds.
- LFR I, pp.177 and 200–201, (i), (ii), (1.99)–(1.100), together with LFR II pp.384–385, (1.80)–(1.83): all eligible components are processed, and clean unresolved descendants have the stated finite eligibility horizon.
- Brydges–Fröhlich–Seiler (1978), Theorems 2.8 and 2.10, pp.36, 40: reflection positivity and chessboard on an even-sided periodic rectangle. The source tori in CMP109 p.251 have an even number of fixed \(L\)-site tiles in each direction. No effective-law reflection positivity was imported.
- Earlier companion results PC-A/PC-C, CG, and RX18: the previously proved source budget, connected normalization on the stated carrier, and explicit regular source neighborhood.

No independent probability law is assigned to signed cluster activities. No new cutoff is substituted for the source cutoff, and no history-dependent normalization or identity subtraction is introduced.

---
