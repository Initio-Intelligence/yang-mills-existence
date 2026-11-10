# Angular defect identities for the Wilson law

## Scope and fixed conventions

The target is the existing hierarchy in $V=\operatorname{Sym}^2(\Lambda^2\mathbb R^4)$, with all 21 labels, the seven reflected normalization coefficients, and the prescribed coincidence-flat tests. No averaged theory, replacement field or alternative continuum limit is introduced.

The existing rotation estimate applies to a selected family with vanishing terminal coupling. It does not supply the physical-sequence estimates required by R-02/R-03. Likewise, the conditional implication in Section 4 does not turn missing action and observable bounds into completed actual-model estimates.

At fixed finite cutoff let $\mathcal M=SU(N)^E$ be the product of independent positively oriented link groups, with normalized product Haar measure $dU$. Write $$d\mu_a(U)=Z_a^{-1}e^{-S_a(U)}dU,\qquad
 S_a(U)=b_a\sum_p\left(1-\frac1N\operatorname{Re}\operatorname{Tr}U_p\right).$$ Here $b_a>0$ is exactly the Wilson coefficient in this trace convention; it is not a newly chosen running coupling. Each unoriented elementary plaquette is counted once. The density is smooth and positive. At a fixed cutoff all smooth functions used below are integrable.

## R-02: an exact local identity on the full Wilson law

Choose an orthonormal anti-Hermitian basis $T_A$ of $\mathfrak{su}(N)$ and define the left derivatives $$L_b^Af(U)=\left.\frac d{dt}f(\ldots,e^{tT_A}U_b,\ldots)\right|_{t=0}.$$ Let $\mathcal V=\sum_{b,A}v_b^A(U)L_b^A$ be any smooth real vector field on $\mathcal M$. Its Haar divergence is $$\operatorname{div}\mathcal V=\sum_{b,A}L_b^Av_b^A.$$ Define the normalized-law score insertion $$\begin{equation}
\label{eq:score}
 W_{a,\mathcal V}=\mathcal V S_a-\operatorname{div}\mathcal V.
\end{equation}$$

**Theorem 1** (Full-law Ward identity). *For every smooth scalar observable $O$, $$\begin{equation}
\label{eq:ward}
 \mathbb E_{\mu_a}W_{a,\mathcal V}=0,\qquad
 \mathbb E_{\mu_a}(\mathcal V O)=\operatorname{Cov}_{\mu_a}(O,W_{a,\mathcal V}).
\end{equation}$$ For a smooth family $O_t$ and vector fields $\mathcal V_t$, $$\begin{equation}
\label{eq:split}
 \frac d{dt}\mathbb E_{\mu_a}O_t
 =\mathbb E_{\mu_a}(\dot O_t-\mathcal V_tO_t)
    +\operatorname{Cov}_{\mu_a}(O_t,W_{a,\mathcal V_t}).
\end{equation}$$ Both formulas are exact at arbitrary positive Wilson coupling and finite volume.*

*Proof.* Left-invariant derivatives have zero integral against Haar measure. Apply this to $v_b^A O e^{-S_a}$ and sum over $b,A$. The result is $$0=\mathbb E_{\mu_a}\bigl[\mathcal V O+O\operatorname{div}\mathcal V
                                      -O\mathcal V S_a\bigr].$$ Taking $O=1$ proves the zero-mean assertion; subtracting the mean of $O$ gives the covariance. Differentiate the fixed finite-volume expectation of $O_t$, then add and subtract $\mathbb E\mathcal V_tO_t$ to obtain [\[eq:split\]](#eq:split). ◻

## A concrete local vector field for an angular test

For a plane $(\alpha,\beta)$ choose a smooth compactly supported coordinate vector field $$\xi(x)=\chi(x)(x_\alpha e_\beta-x_\beta e_\alpha),$$ where $\chi=1$ on a physical region containing the compact test support and its fixed stencil margin. Embed its support away from the torus seam. This construction is for compact tests; passing to arbitrary Schwartz tails needs the common hierarchy bound still assigned to S-05.

For a matrix $Q\in SU(N)$ put $$\mathcal P(Q)=\tfrac12(Q-Q^\dagger)
                 -\frac{\operatorname{Tr}(Q-Q^\dagger)}{2N}I.$$ For $\nu\ne\mu$, $U_{\nu\mu}(x)$ is the oriented plaquette based at $x$. Define $$\begin{equation}
\label{eq:localV}
 v_{x,\mu}(U)=a^{-1}\sum_{\nu\ne\mu}\xi_\nu(x)\mathcal P(U_{\nu\mu}(x)),
 \qquad v_{x,\mu}=\sum_Av_{x,\mu}^AT_A.
\end{equation}$$ This is a globally smooth link vector field, and is covariant under gauge transformations at the starting point of each link. Thus it maps gauge-invariant observables to gauge-invariant observables. On a smooth classical connection, the leading expression is the usual $a\xi^\nu F_{\nu\mu}$ link variation, up to orientation convention. No smooth-field approximation is used in the exact identities here, and this observation is not an estimate under the Wilson measure.

The score has the exact carrier decomposition $$\begin{align}
 W_{a,\xi}&=\sum_b w_{a,b},\\
 w_{a,b}&=\sum_A v_b^A L_b^AS_a-\sum_A L_b^Av_b^A.\label{eq:carriers}
\end{align}$$ Only plaquettes incident to $b$ appear in $L_b^AS_a$, and $v_b$ uses plaquettes based at the initial site of $b$. Each $w_{a,b}$ therefore depends on a fixed number of neighboring links, independent of volume, coupling and RG depth. There are no omitted nonlocal terms in this microscopic formula.

Compactness gives the quantitative, but non-small, bound $$\begin{equation}
\label{eq:rough}
 |w_{a,b}|\le C_N(b_a+1)a^{-1}\sum_\nu|\xi_\nu(x_b)|.
\end{equation}$$ Indeed $\mathcal P(U_p)$ and its link derivatives are bounded by fixed group constants; each $L_b^AS_a$ is a sum over a fixed number of incident plaquettes and is bounded by $C_Nb_a$. Summing [\[eq:rough\]](#eq:rough) over links in a fixed physical region of volume $O(1)$ produces a bound of order $(b_a+1)a^{-5}$. It does not prove a vanishing angular defect. The zero mean in [\[eq:ward\]](#eq:ward) is essential and is not a small absolute-value bound.

## The precise angular defect split

Let $O_{m,a}(F;U)$ be the actual finite-cutoff product observable paired with a joint tensor test $F$, including the chosen normalization matrix and identity subtraction. Let $U_R$ rotate all external coordinates and tensor labels together, and write $D_{\alpha\beta}$ for its test generator. Define $$\begin{equation}
\label{eq:remainder}
 \mathcal R_{m,a,\xi}(F;U)
   =O_{m,a}(D_{\alpha\beta}F;U)-\mathcal V_\xi O_{m,a}(F;U).
\end{equation}$$ Then Theorem 1 proves $$\begin{equation}
\label{eq:angular}
 S_{m,a}(D_{\alpha\beta}F)
 =\mathbb E\mathcal R_{m,a,\xi}(F)
       +\sum_b\operatorname{Cov}(O_{m,a}(F),w_{a,b}).
\end{equation}$$ This displays local action-score carriers for the actual full law. It includes every tensor label and every finite source order by using that order's actual observable. The remainder is explicitly defined, rather than assumed small. It contains the discrepancy between continuous coordinate rotation and the link variation, tensor-label matching terms, and any cutoff effects in the chosen observable. The normalization data are fixed coefficients of the cutoff observable, so the link derivative does not differentiate those coefficients as if they were random link functions.

Equation [\[eq:angular\]](#eq:angular) is a starting identity for R-02/R-03. To complete R-02/R-03 one must bound its two contributions by the required vanishing rates on the physically matched sequence. A tautological definition of the remainder alone does not accomplish that task.

## What exact conditioning preserves

For any retained-data sigma algebra $\mathcal G$, the exact identity is $$\begin{equation}
\label{eq:conditional}
 \operatorname{Cov}(O,W)
 =\operatorname{Cov}(\mathbb E[O\mid\mathcal G],\mathbb E[W\mid\mathcal G])
     +\mathbb E\operatorname{Cov}(O,W\mid\mathcal G).
\end{equation}$$ It follows by expanding both products and using the tower property. Thus a source-free RG step may transfer the joint insertion exactly, but replacing it by a product of its separately conditional expectations drops the second term. Iteration retains the successive conditional covariance terms. Nonlocal tails generated by conditional transport and all retained-history contributions need estimates; microscopic locality does not establish those estimates. Working on the full compact link manifold avoids introducing artificial selector-boundary terms at the outset; an eventual selected-coordinate proof must preserve the same identity.

## R-03: an exact six-generator tensor diagnostic

Use the seven projectors of Annex X in the orthogonal Frobenius metric on symmetric $6\times6$ matrices: $$Z=z_SP_S+z_PP_P+z_{T_d}P_{T_d}+z_{T_o}P_{T_o}
          +z_{W_d}P_{W_d}+z_{W_s}P_{W_s}+z_{W_p}P_{W_p}.$$ All coefficients in this section are real, as in the stated field prescription. Let $J_{\mu\nu}$ be the generator on $V$ of a unit-speed rotation in the $(\mu,\nu)$ plane. The six generators use the ordinary angle in radians, with no rescaling.

**Theorem 2** (Exact angular commutator budget). *The following identity holds: $$\begin{equation}
\label{eq:Q}
 \sum_{\mu<\nu}\left\|[J_{\mu\nu},Z]\right\|_{\rm HS}^2
 =48\left[(z_{T_d}-z_{T_o})^2+(z_{W_d}-z_{W_s})^2
                              +(z_{W_p}-z_{W_s})^2\right].
\end{equation}$$ If $\delta_Z=\left\|Z-\bar Z\right\|_{\rm HS}$ is the distance in (R.7), then $$\begin{equation}
\label{eq:equiv}
 24\delta_Z^2\le\sum_{\mu<\nu}\left\|[J_{\mu\nu},Z]\right\|_{\rm HS}^2
                                  \le40\delta_Z^2.
\end{equation}$$*

*Proof.* Take the ordered wedge basis $e_i\wedge e_j$, $i<j$. If $L_{\mu\nu}$ is the skew $4\times4$ plane generator, its action on wedges is $$A(e_i\wedge e_j)=L_{\mu\nu}e_i\wedge e_j+e_i\wedge L_{\mu\nu}e_j.$$ Its induced action on a symmetric matrix $B$ is $J B=AB+BA^{\mathsf T}$. The norm on symmetric coordinate entries has weights 1 on diagonal entries and 2 off the diagonal. Inserting the seven orthogonal projectors gives, for each fixed plane, the following nonzero off-sector squared norms: $$\begin{array}{c|c}
\text{block}&\left\|P_hJ_{\mu\nu}P_l\right\|_{\rm HS}^2\\\hline
(T_o,T_d)&4\\
(W_s,W_d)&4\\
(W_p,W_s)&4
\end{array}$$ The reverse blocks have the same norms; all other off-sector blocks vanish. To check the table directly one can take the $(1,2)$ plane: $A$ rotates the pairs $(e_{13},e_{23})$ and $(e_{14},e_{24})$, fixing $e_{12},e_{34}$. Apply $AB+BA^{\mathsf T}$ to each projector range. The other planes are conjugate by signed coordinate permutations, which preserve the projectors. The accompanying rational-arithmetic certificate constructs precisely these matrices and verifies all cross-block coefficients, without floating-point tolerances.

Orthogonality of the projector blocks gives $$\left\|[J,Z]\right\|_{\rm HS}^2
   =\sum_{h,l}(z_h-z_l)^2\left\|P_hJP_l\right\|_{\rm HS}^2.$$ There are six planes and two directed blocks for each displayed pair, giving $6\cdot2\cdot4=48$.

Set $t=z_{T_d}-z_{T_o}$, $u=z_{W_d}-z_{W_s}$ and $v=z_{W_p}-z_{W_s}$. The existing distance formula becomes $$\delta_Z^2=2t^2+\frac85(u^2+v^2)-\frac45uv.$$ Writing the left side of [\[eq:Q\]](#eq:Q) as $Q_Z$, direct subtraction gives $$Q_Z-24\delta_Z^2=\frac{48}{5}(u+v)^2,\qquad
40\delta_Z^2-Q_Z=32t^2+16(u-v)^2.$$ These identities prove both bounds. The lower constant is attained when only $t$ is nonzero, and the upper constant when $t=0$ and $u=v\ne0$. ◻

This gives a quantitative test of the finite normalization map. In particular $\left\|[D(R),Z]\right\|_{\rm HS}\le2\delta_Z$ for every $R\in O(4)$, because $\bar Z$ commutes with that representation and the representation is orthogonal. The calculation does not prove that the measured Wilson normalization data satisfy $\delta_Z\to0$. Nor does commutation of $Z$ alone prove covariance of the normalized fields: cutoff representatives can have compensating anisotropies, as already noted in R-01. The quantities in [\[eq:Q\]](#eq:Q) must be combined with the actual field-transport defects.

## Exact contacts under angular differentiation

The statement already proves that point-local higher source vertices give distributions supported on partial diagonals and annihilate $\mathcal S_0$. The angular consequence is exact at each source order. Simultaneous rotations preserve every partial diagonal, and the orbital angular vector field is tangent to them. Hence $U_RF$ and $D_{\mu\nu}F$ are still flat on every partial diagonal whenever $F$ is. Therefore every such existing contact distribution $C_{m,a}$ obeys $$C_{m,a}(U_RF)=C_{m,a}(D_{\mu\nu}F)=0.$$ No bound on its cutoff-dependent coefficients is needed for this exact statement. This is a consequence of the statement's contact theorem, not a newly completed catalogue item. Contacts transported into finite stencils or nonlocal carriers are covered only after the corresponding matching remainder is bounded. One-field mixing and identity subtraction are not higher source contacts and do not disappear by this argument.

## R-04: uniformity along every fixed rotation 

For tensor tests use the maximum over components in a fixed orthonormal basis and the construction seminorm $$\nu_s(F)=\max_{|\alpha|\le s}\sup_X(1+|X|^2)^{s/2}
                                      |\partial^\alpha F(X)|.$$ Orthogonality on the full tensor product of dimension $21^m$ and the blockwise action on $m$ spacetime coordinates give the explicit estimate $$\begin{equation}
\label{eq:rotate}
 \nu_s(U_RF)\le21^{m/2}2^s\nu_s(F),\qquad R\in O(4).
\end{equation}$$ Indeed each row of a four-dimensional orthogonal matrix has absolute sum at most 2; each differentiated coordinate thus costs at most 2. A row of the tensor-product matrix has absolute sum at most $21^{m/2}$. The weight is unchanged. There is no factor $m^s$ here.

For a plane generator the orbital action is a sum of $2m$ terms with one linear coordinate coefficient. Differentiating such a coefficient twice gives zero. The spin action is a sum of $m$ fixed matrices. Consequently $$\begin{equation}
\label{eq:gen}
 \nu_s(D_{\mu\nu}F)\le C(m+s+1)\nu_{s+1}(F).
\end{equation}$$ One extra weight power pays the coordinate coefficient and one extra derivative pays the orbital derivative; both are included by $s+1$ in this seminorm convention. These operations preserve coincidence flatness.

**Theorem 3** (Six generator bounds imply a common path bound). *Suppose continuous functionals $S_{m,a}$ on $\mathcal S_0$ satisfy, for every test and each of the six planes, $$\begin{equation}
\label{eq:hyp}
 |S_{m,a}(D_{\mu\nu}F)|
 \le\varepsilon_a A^{m+1}(m!)^p\nu_{qm+r}(F),
 \qquad \varepsilon_a\longrightarrow0,
\end{equation}$$ with fixed nonnegative integers $q,r$ and fixed $A,p$. Then for all $R\in SO(4)$, $$\begin{equation}
\label{eq:path}
 |S_{m,a}(U_RF-F)|
 \le6\pi\,\varepsilon_a A^{m+1}(m!)^p
             21^{m/2}2^{qm+r}\nu_{qm+r}(F).
\end{equation}$$ This is a common cutoff rate and factorial exponent for all intermediate rotations as well as all endpoints. If the action and observable/contact parts separately have bounds of the form [\[eq:hyp\]](#eq:hyp), their rates add and the larger fixed $q,r,p$ may be used.*

*Proof.* Givens elimination in four dimensions expresses any $R\in SO(4)$ as a product of at most six coordinate-plane rotations, each with angle in $[-\pi,\pi]$. Choose positive pivots in the first three columns; determinant one forces the last diagonal entry to be positive. This yields a piecewise smooth path of total angular length at most $6\pi$ using the six plane generators, by left multiplication at each segment.

Along a segment, $\frac d{dt}U_{R(t)}F=\dot\theta(t)D_{\mu\nu}(U_{R(t)}F)$ in a consistent representation convention. Continuity permits application of $S_{m,a}$ and integration. Apply [\[eq:hyp\]](#eq:hyp) to the test $U_{R(t)}F$, then [\[eq:rotate\]](#eq:rotate); the latter bound is uniform in $t$ and in the endpoint. Integrate the path length. Fixed powers $21^{m/2}2^{qm+r}$ can be absorbed into a new constant to the power $m+1$, preserving $p,q,r$. ◻

This removes an additional path-uniformity hypothesis once [\[eq:hyp\]](#eq:hyp) has been proved as a joint-test bound. It does not create that bound from pointwise convergence for individual tests. In particular, it cannot be applied to the positive-endpoint hierarchy solely from the comparison-family result.
