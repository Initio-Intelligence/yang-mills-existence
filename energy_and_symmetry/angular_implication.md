# A conditional rotation theorem

## Conditional rotation theorem

Set the fixed physical unit $\ell_0=1$, take $h_l=L^{-l}$ and cutoff $a_K=h_K$, $L>1$. Increasing $l$ means moving toward the ultraviolet; the physical terminal level is $l=0$. Throughout, all fields, counterterms and histories are those of the specified Wilson hierarchy. No averaging of rotated theories and no replacement normalization are permitted.

For $m$ insertions let $V=\operatorname{Sym}^2(\Lambda^2\mathbb R^4)$ and take $V^{\otimes m}$-valued coincidence-flat Schwartz tests. The seminorm is exactly the joint-test convention, with a maximum over orthonormal tensor components: $$\nu_s(F)=\max_{|\alpha|\le s}\sup_X(1+|X|^2)^{s/2}|\partial^\alpha F(X)|.$$ Let $T_{m,K}$ and $S_{m,K}$ denote the actual connected and full distributions. A unit plane rotation generator acting simultaneously on coordinates and labels is denoted $D_e$, for one of the six planes $e$.

The hypotheses below produce sequences $q_l\ge0$, $Q=\sum_{l\ge0}q_l<\infty$, and numbers $C_0,\delta>0$. Define $$\begin{align}
 b_d&=C_0(1+d)L^{-\delta d},\\
 \eta_K&=b_K+\sum_{l=0}^K q_l b_{K-l}+a_K^2.\label{eq:rate}
\end{align}$$ Every constant in these formulas is independent of source order, volume, history and cutoff depth. For $d\ge0$, one can choose a fixed $B$ with $b_d\le B L^{-\delta d/2}$. Consequently $$\begin{equation}
\label{eq:rateexplicit}
 \eta_K\le B L^{-\delta K/2}
   +BQ L^{-\delta K/4}
   +B\sum_{l>\lfloor K/2\rfloor}q_l+a_K^2
 \longrightarrow0.
\end{equation}$$ This is an explicit rate in terms of the supplied summable majorant; no polynomial tail for that majorant is assumed.

**Theorem 1** (Conditional R-02--R-04). *Under hypotheses P0--P4 in Section 2, the action and observable/contact contributions to every connected angular Ward identity separately obey $$|G^A_{m,K,e}(F)|+|G^O_{m,K,e}(F)|+|C_{m,K,e}(F)|
 \le\eta_K C^{m+1}(m!)^p\nu_{qm}(F),$$ for fixed $q,p,C$ and every $m\ge1$, plane $e$ and cutoff $K$. Their corresponding marked full-moment contributions obey the same form of estimate. In particular, $$\begin{equation}
\label{eq:genfinal}
 |S_{m,K}(D_eF)|\le\eta_K C^{m+1}(m!)^p\nu_{qm}(F).
\end{equation}$$ For every $R\in SO(4)$, uniformly over all endpoints and the intermediate rotations used to reach them, $$\begin{equation}
\label{eq:rotfinal}
 |S_{m,K}(U_RF-F)|\le6\pi\,\eta_K C_*^{m+1}(m!)^p\nu_{qm}(F).
\end{equation}$$ Thus the action-defect conclusion of R-02, the all-label and all-order observable/contact conclusion of R-03, and the common path-budget conclusion of R-04 all follow. The proof is completed below. Verification of P0--P4 for the actual model is not claimed.*

## External premises, stated at the primitive level 

These premises must hold for the *same* physical matching, cofinal sequence and normalized full Wilson law. Constants may depend on the fixed group, blocking factor and physical units. Uniformity in arbitrary source order, volume and admitted history is part of each bound. They cannot be supplied by estimates only inside one chosen regular history.

#### P0: exact marked representation.

The connected angular identity has the exact decomposition $$\begin{equation}
\label{eq:exact}
 T_{m,K}(D_eF)=G^A_{m,K,e}(F)+G^O_{m,K,e}(F)+C_{m,K,e}(F).
\end{equation}$$ Here $A$ is the action-score insertion, $O$ is the field/matching insertion, and $C$ consists of point or shrinking-stencil contacts. For $\sigma=A,O$, exact marked transport gives $$\begin{equation}
\label{eq:marked}
 G^\sigma_{m,K,e}
  =\mathcal T^\sigma_{m,K,e}(u^\sigma_{K,0,e})
     +\sum_{l=0}^K\mathcal L^\sigma_{m,K,l,e}(u^\sigma_{K,l,e}).
\end{equation}$$ The two kinds of operators are respectively terminal and shell response maps. They act linearly on explicit local defect coefficients in a fixed normed space; they are not defined by dividing an unknown entire correlation by a small number. For a source-jet space, the norm includes its fixed factorial weights. All changes in conditional normalizers, outer means, retained histories, and collisions are included by the exact marked transport. The decomposition must be an identity of joint distributions, not merely an identity on separated tensor-product tests.

For the action, the extracted local marginal terms are vacuum constants and the reflection-even hypercubic-invariant gauge-polynomial terms of engineering dimension at most four. Their scalar part has zero angular variation; it is removed algebraically before forming $u^A$. For observables, $u^O$ includes the *compensated* matching commutator in the prescribed physical basis, all 21 channels and all higher source jets. It is not the commutator of a raw bare-to-renormalized matrix alone. Sections 3 and 4 justify these algebraic distinctions.

#### P1: coefficient contraction and controlled forcing.

The two coefficient families in [\[eq:marked\]](#eq:marked) satisfy, in their fixed norms, $$\begin{align}
 \left\|u^\sigma_{K,K,e}\right\|&\le C_u,\\
 u^\sigma_{K,l,e}&=B^\sigma_{K,l,e}u^\sigma_{K,l+1,e}
                         +f^\sigma_{K,l,e},\qquad 0\le l<K,\\
 \left\|B^\sigma_{K,l,e}\right\|&\le L^{-\delta},\qquad
 \left\|f^\sigma_{K,l,e}\right\|\le C_f L^{-\delta(K-l)}.\label{eq:recursion}
\end{align}$$ The physical angular marginal defect must be absent or included in a compensated coefficient family satisfying this recursion. A nonzero uncontracted angular marginal term is not allowed to disappear by terminology. The same fixed $\delta>0$ works for both families and all six planes. The observable coefficient norm dominates each compensated matrix commutator and the corresponding source-jet commutators with their fixed factorial weights.

P1 is a new, unverified actual-model requirement. General bounds on an RG remainder, ordinary hypercubic symmetry, and the original dependency lists do not themselves imply it. It is strictly a coefficient-level estimate; it assumes neither small angular correlations nor rotational invariance of the limiting hierarchy.

#### P2: response-kernel and terminal majorants.

For $m\ge2$ the shell response to $u$ has a representation $$\mathcal L(u)(F)=\sum_{|\alpha|\le r_*m}\int K_\alpha(X)\,\partial^\alpha F(X)\,d\lambda_K^{\otimes m}(X),$$ where $r_*\ge0$ is fixed. The measure $\lambda_K$ is either Lebesgue measure or normalized counting measure $a_K^4\sum_{x\in a_K\mathbb Z^4}\delta_x$, restricted to the admitted finite-volume embedding when appropriate. Thus this premise permits the derivative distributions of an actual lattice hierarchy. For a fixed $s_*\ge0$, the sum of the component kernel magnitudes satisfies $$\begin{equation}
\label{eq:treeinput}
 \sum_\alpha|K_\alpha(X)|
 \le\left\|u\right\| A^{m+1}(m!)^{p_0}h_l^{-4m}w_l(1+|x_1|^2)^{s_*m/2}
       \exp\left[-\frac{c\,\tau(X)}{(m+d_0)h_l}\right].
\end{equation}$$ Here $\tau$ is the minimum Euclidean spanning-tree length, $d_0\ge0$, $c>0$, and $p_0\ge0$ are fixed. Every carrier sum, differentiated preparation, marked position, and history contribution assigned to that shell has already been included in this nonnegative bound. The common weights satisfy $$q_l=h_lw_l,\qquad Q=\sum_{l\ge0}q_l<\infty.$$ The terminal response satisfies $$\begin{equation}
\label{eq:terminal}
 |\mathcal T^\sigma_{m,K,e}(u)(F)|
 \le\left\|u\right\| A^{m+1}(m!)^{p_T}\nu_{q_Tm}(F).
\end{equation}$$ Each one-point marked contribution is required to satisfy the terminal bound with coefficient $u_{K,0,e}$, or to vanish by a separately verified identity. Centering the unmarked field alone does not imply that its covariance with an action-score insertion vanishes. No one-point tree gain is inferred from coincidence flatness. These are full-law marked-insertion versions of the kernel and terminal inputs, not estimates merely for unmarked correlations.

#### P3: point contacts or quantitative shrinking contacts.

There are no coincidence contacts at source order one; any one-point local matching term is included in $O$ and must satisfy the one-point clause of P2. At each fixed source order, a contact is either supported exactly on a partial diagonal, with finite distribution order, or has a representation $$\begin{equation}
\label{eq:contactinput}
 C_{m,K,e}=\sum_{|\alpha|\le r_0m}\partial^\alpha\mu_{\alpha,m,K,e}
\end{equation}$$ for $m\ge2$. Each measure in this finite sum is supported within distance $c_0a_K$ of some partial diagonal. The constants $r_0,b\ge0,c_0>0$ are fixed, and for a fixed integer $q_C\ge r_0+\lceil b\rceil+4$, $$\begin{equation}
\label{eq:contactmeasure}
 \sum_\alpha\int(1+|X|^2)^{-q_Cm/2}
                           d|\mu_{\alpha,m,K,e}|(X)
 \le A_C^{m+1}(m!)^{p_C}a_K^{-bm}.
\end{equation}$$ For tensor contacts the component sum is included or absorbed into $A_C^{m+1}$. Angularly differentiated contacts must admit this representation with these constants; this includes derivatives of contact coefficients and finite stencils. Compatibility under truncation in $m$ is retained. Exact point contacts do not need a coefficient bound.

#### P4: the base hierarchy and joint-test partition theorem.

The actual unmarked connected distributions obey $$|T_{m,K}(F)|\le A_B^{m+1}(m!)^{p_B}\nu_{q_Bm}(F),$$ and the completed S-01 joint-distribution tensor-product, extension-independence and stability hypotheses hold. We use its theorem with $p\ge1$. This is not an assumption that every arbitrary distributional family with a scalar seminorm bound has a well-defined unrestricted product. S-01 supplies the required joint-test construction.

#### Dependencies.

P0 requires marked and history transport of the kind assigned to M-07, H-04/H-05 and S-04. P2 requires marked versions of C-08, H-04, S-03 and S-05. P3 is a quantitative realization of F-06/S-06. P4 uses the actual common hierarchy bound and the already completed S-01 bridge. These correspondences describe required interfaces, not claims that the named catalogue items already prove the premises. In particular P1 and the exact marginal/compensated extraction in P0 remain additional primitive verification obligations. No R-02, R-03, R-04 or R-05 conclusion is used as a premise.

## The exact Wilson starting identity 

On the finite link manifold $SU(N)^E$, let $L_b^A$ be left-invariant derivatives and $\mathcal V=\sum_{b,A}v_b^AL_b^A$ a smooth link vector field. For the normalized Wilson law $d\mu=Z^{-1}e^{-S}dU$, set $$W=\mathcal VS-\sum_{b,A}L_b^Av_b^A.$$ Haar integration by parts gives $$\mathbb EW=0,\qquad \mathbb E(\mathcal VO)=\operatorname{Cov}(O,W).$$ For a microscopic product observable $O_m(F)$ this yields the exact split $$\begin{equation}
\label{eq:ward}
 S_m(D_eF)=\operatorname{Cov}(O_m(F),W)
                  +\mathbb E\{O_m(D_eF)-\mathcal VO_m(F)\}.
\end{equation}$$ One can choose the local curvature vector field $$v_{x,\mu}=a^{-1}\sum_{\nu\ne\mu}\xi_\nu(x)\left[
 \tfrac12(U_{\nu\mu}-U_{\nu\mu}^\dagger)
 -\tfrac1{2N}\operatorname{Tr}(U_{\nu\mu}-U_{\nu\mu}^\dagger)I\right],$$ with a smooth compactly supported angular vector $\xi$. Then $W=\sum_bw_b$, where $w_b=\sum_A(v_b^AL_b^AS-L_b^Av_b^A)$ has a fixed local link carrier. This does not establish P1 or P2, but it specifies the microscopic insertions to which P0 must apply, including the Haar-divergence term. Passing from full to connected source coefficients is an exact formal operation at every finite order.

Exact conditional transport must preserve $$\operatorname{Cov}(O,W)=\operatorname{Cov}(\mathbb E[O\mid\mathcal G],\mathbb E[W\mid\mathcal G])
                 +\mathbb E\operatorname{Cov}(O,W\mid\mathcal G).$$ Thus P0/P2 explicitly retain the second term and the outer covariance, along with their higher-order versions. Boundary cutoffs used to localize $\xi$ must be included in these inputs and their summable majorants. Their removal is not inferred from microscopic locality alone.

## Why scalar marginal isotropy is algebraic 

**Lemma 2** (Reflection-even curvature quadratic). *Let $SU(N)$ be fixed. A local scalar quadratic in curvature that is gauge invariant and invariant under signed coordinate permutations is a multiple of $$\sum_{\mu<\nu}\langle F_{\mu\nu},F_{\mu\nu}\rangle.$$*

*Proof.* Gauge invariance contracts the two adjoint color indices by a multiple of the invariant quadratic form of the simple Lie algebra. A product of two distinct two-form components changes sign under a reflection of an index occurring in exactly one pair. Distinct pairs always have such an index, including complementary pairs. Hence every cross coefficient vanishes. Coordinate permutations act transitively on the six pairs, making the diagonal coefficients equal. The resulting quadratic is rotationally invariant. ◻

This applies to the extracted quadratic-curvature marginal sector in P0. Vacuum constants have zero angular variation and cancel from a normalized law. A reflection-odd pseudoscalar is excluded by the stated symmetry. This lemma does not classify a nonlocal effective action as local or prove that all remaining angular terms satisfy P1; those are precisely the retained primitive obligations. It also says nothing about the seven-channel normalization of the observables.

For the latter, one has, in the fixed Frobenius metric, $$\begin{equation}
\label{eq:matrix}
 \sum_e\left\|[J_e,Z]\right\|_{\rm HS}^2
 =48\big[(z_{T_d}-z_{T_o})^2+(z_{W_d}-z_{W_s})^2
                              +(z_{W_p}-z_{W_s})^2\big].
\end{equation}$$ The included exact rational certificate reconstructs the six $21\times21$ generators and seven projectors and verifies every block coefficient. The same formula may be used for a compensated matching matrix that has this seven-channel form. For a general matching matrix its full commutator is included in $u^O$. Assuming commutation of a raw matrix in place of compensated matching would change P0 and is not allowed.

## Contraction gives the primitive cutoff factor

**Lemma 3** (Uniform solution of P1). *P1 implies $\left\|u^\sigma_{K,l,e}\right\|\le b_{K-l}$ with $C_0=C_u+C_f$ (enlarged if necessary). In particular the terminal coefficient tends to zero.*

*Proof.* Iterating $d=K-l$ steps, the initial term has norm at most $C_uL^{-\delta d}$. A forcing created at layer $r\in\{l,\ldots,K-1\}$ is multiplied by at most $L^{-\delta(r-l)}$, and its norm is at most $C_fL^{-\delta(K-r)}$. Each of the $d$ forcing contributions is therefore at most $C_fL^{-\delta d}$. Add them. Finally $(1+d)L^{-\delta d/2}$ is bounded on the nonnegative integers, proving the exponential envelope used in [\[eq:rateexplicit\]](#eq:rateexplicit). ◻

For a compensated matrix $M_{K,l}$ whose commutators are included in $u^O$, the same coefficient bound also gives an operator-level finite-angle estimate. On orthogonal source and target representations, integrate the commutator along the six-plane path to get $$\left\|D(R)M_{K,l}-M_{K,l}D(R)\right\|\le6\pi b_{K-l}.$$ For a multilinear source jet, use its induced source and target representations and the weighted jet norm in P1. Thus the same statement holds with its fixed factorial factor. At every fixed physical layer $l$, these defects tend to zero as $K\to\infty$; the near-cutoff layers are instead handled by the shell sum below.

There is no derivative-order dependent choice of $\delta$ here. Any amplification from inverse running matrices or preparations must already be in the actual norms and maps of P1; it cannot be assigned norm one without proof.

## The full shell integral, including approaching diagonals

**Lemma 4** (A flat-test shell gain). *For $m\ge2$, $0<a\le h\le1$, and $F\in\mathcal S_0$, a response kernel as in P2 at scale $h$, including its test derivatives and root weight, satisfies $$\begin{equation}
\label{eq:shellout}
 |\mathcal L(u)(F)|\le\left\|u\right\|hw\,C^{m+1}(m!)^{p_0+5}\nu_{q_*m}(F),
 \qquad q_*=\lceil r_*\rceil+\lceil s_*\rceil+6.
\end{equation}$$ No positive separation of the test support from a partial diagonal is required. The same constants work for integration and normalized lattice summation.*

*Proof.* Hold $x_1$ and all variables other than $x_2$ fixed, and Taylor expand each $\partial^\alpha F$ in $x_2$ about $x_2=x_1$ to order four. All those Taylor coefficients vanish by flatness. Along the Taylor segment the first variable stays $x_1$, so the weighted derivative bound gives $$|\partial^\alpha F(X)|\le C\nu_{q_*m}(F)
 (1+|x_1|^2)^{-(q_*m)/2}|x_2-x_1|^5.$$ The directional derivative costs only the fixed dimension four, and $|\alpha|+5\le q_*m$. Multiplication by the root factor in P2 leaves a weight bounded by $(1+|x_1|^2)^{-3}$. Its integral and its normalized lattice sum for $a\le1$ are uniformly finite.

Let $\mathfrak T_m$ be the labeled spanning trees and $\ell_T(X)$ their lengths. Since $\tau=\min_T\ell_T$, for $s=(m+d_0)h$, $$|x_2-x_1|^5e^{-c\tau/s}
 \le\sum_{T\in\mathfrak T_m}\ell_T^5e^{-c\ell_T/s}
 \le C s^5\sum_T e^{-c\ell_T/(2s)}.$$ The first inequality follows by selecting a minimizing tree, whose path from 1 to 2 has length at least $|x_2-x_1|$; adding the remaining nonnegative tree terms only enlarges it. Root each tree at 1 and use its edge differences as integration variables. The Jacobian is one and each of its $m-1$ edge integrals costs $C s^4$. For a lattice sum the edge transformation is a bijection of lattice variables. Since $s=(m+d_0)h\ge a$, comparison with lattice cubes gives $$a^4\sum_{y\in a\mathbb Z^4}e^{-c|y|/(2s)}\le C s^4.$$ The distance to the cube center is at most $2a$, costing only a fixed exponential. Restricting a finite-volume sum only reduces the absolute majorant when the Euclidean embedding in P2 holds. There are $m^{m-2}$ labeled trees. The bound is therefore $$C^{m+1}(m!)^{p_0}\left\|u\right\|\nu_{q_*m}(F)w h^{-4m}
              m^{m-2}[(m+d_0)h]^{4m+1}.$$ The power of $h$ is exactly one. For fixed $d_0$, the remaining factor $m^{m-2}(m+d_0)^{4m+1}$ is at most $C^{m+1}(m!)^5$, by $m!\ge(m/e)^m$ and absorption of a fixed polynomial in $m$ into $C^m$. The sum over derivative indices is already included in P2. Summing tensor components costs at most $21^m$, absorbed into $C^{m+1}$. ◻

Combining Lemmas 3 and 4 gives the normally convergent bound $$\left|\sum_{l=0}^K\mathcal L^\sigma_{m,K,l,e}(u^\sigma_{K,l,e})(F)\right|
 \le\left(\sum_{l=0}^Kq_lb_{K-l}\right)
               C^{m+1}(m!)^{p_0+5}\nu_{q_*m}(F).$$ The terminal term adds $b_KA^{m+1}(m!)^{p_T}\nu_{q_Tm}(F)$. This proves the action and matching shell conclusions with all old scales and all spatial carriers accounted for by P2.

To verify [\[eq:rateexplicit\]](#eq:rateexplicit), split the shell sum at $l=\lfloor K/2\rfloor$. On the first part $K-l\ge K/2$, so $b_{K-l}\le BL^{-\delta K/4}$; on the second part use $b_{K-l}\le B$. Summability gives the stated tail tending to zero. This argument remains valid when the ultraviolet weights have no known power-law tail.

## Contacts: exact annihilation or a proved small error

Exact finite-order distributions supported on partial diagonals annihilate $F$, $D_eF$ and $U_RF$, since simultaneous rotations preserve those diagonals and the angular vector fields are tangent to them. This is valid at each finite source order regardless of the size of the contact coefficients.

**Lemma 5** (Shrinking-contact budget). *Under the shrinking-contact alternative of P3, $$|C_{m,K,e}(F)|\le a_K^2 C^{m+1}(m!)^{p_C}\nu_{q_Cm}(F).$$*

*Proof.* Set $n=\lceil b\rceil m+2$. For each $X$ in a measure support choose a pair of arguments whose distance is at most a fixed multiple of $a_K$, and move one to the other, leaving the other coordinates fixed. Taylor's formula for $\partial^\alpha F$ has zero coefficients at the coincidence point, to every order. The $n$th remainder requires at most $|\alpha|+n\le q_Cm$ derivatives.

The displacement is $O(a_K)$ in a fixed number of coordinates. Along this segment the ratio of $1+|X|^2$ to the corresponding shifted weight is bounded by a fixed constant. Raising it to $q_Cm/2$ costs at most a constant to the power $m$. Taylor's formula and the fixed-dimensional directional derivative bound therefore give $$|\partial^\alpha F(X)|
 \le C^{m+1}\nu_{q_Cm}(F)
       a_K^{\lceil b\rceil m+2}(1+|X|^2)^{-q_Cm/2}.$$ There is no need to partition the measure measurably by the selected pair: this pointwise upper bound is identical for every choice. Integrate against each total variation measure and use [\[eq:contactmeasure\]](#eq:contactmeasure), which already sums the derivative indices. The resulting exponent is $(\lceil b\rceil-b)m+2\ge2$, proving the assertion for $a_K\le1$. ◻

A fixed physical-size contact carrier does not meet P3. Neither does a coefficient growth faster than the stated linear-in-$m$ cutoff power. Such terms must be estimated elsewhere in P0--P2; they are not declared zero by flatness.

## Connected-to-full passage without losing source orders

Take $$p=\max\{1,p_0+5,p_T,p_C,p_B\},\qquad
 q=\max\{q_*,q_T,q_C,q_B\},$$ with integer $q$ enlarged once if the established S-01 interface requires it. The preceding lemmas and P4 bound the base connected hierarchy by $C^{m+1}(m!)^p\nu_{qm}$, and each marked connected family by $\eta_K$ times that bound.

Here is the marked use of the completed S-01 theorem. For a marked family $G$ and $\eta_K>0$, form the formal connected family $T+zG/\eta_K$. On $|z|\le1$ its connected bound has the same $q,p$ with a fixed larger constant. S-01 constructs its full partition family on joint flat tests with the same $q,p$, uniformly on that disk. At source order $m$ this is a polynomial in $z$. Cauchy's estimate at zero bounds its derivative by that common bound. Multiplying back by $\eta_K$ gives $$\begin{equation}
\label{eq:markedpartition}
 \left|\sum_{\pi}\sum_{B\in\pi}
      G_{|B|}\mathop{\bigotimes}_{B'\in\pi\setminus\{B\}}T_{|B'|}(F)\right|
 \le\eta_K C^{m+1}(m!)^p\nu_{qm}(F).
\end{equation}$$ The products in this formula are the S-01 joint-distribution products, not products defined only on simple tensor tests. If $\eta_K=0$, the marked families vanish and the assertion is immediate.

Apply [\[eq:markedpartition\]](#eq:markedpartition) separately to $G^A$, $G^O$ and $C$. Differentiation of the finite partition identity distributes the angular generator over its blocks, exactly producing their sum. Thus [\[eq:genfinal\]](#eq:genfinal) follows with the same normalization, all labels and every finite source order. Compatibility in $m$ follows from P0/P3 and the partition construction, not from a truncation of the list of generated vertices.

## Uniform rotation paths and completion of the proof

For every orthogonal $R$ and tensor test, $$\begin{equation}
\label{eq:testrotate}
 \nu_s(U_RF)\le21^{m/2}2^s\nu_s(F).
\end{equation}$$ Each coordinate derivative is mixed by a row of a $4\times4$ orthogonal matrix with absolute row sum at most 2. The tensor product action has dimension $21^m$, giving row sum at most $21^{m/2}$. The radial weight is invariant. Flatness is preserved. These facts prove [\[eq:testrotate\]](#eq:testrotate) with no dependence on the rotation or its path.

Givens elimination writes any $R\in SO(4)$ as at most six coordinate-plane rotations, each with angle in $[-\pi,\pi]$. Choosing positive pivots in the first three columns leaves last entry $+1$ because the determinant is one. Interpolate these factors by left multiplication, obtaining a piecewise smooth path of total angular length at most $6\pi$. Along each segment, $$\frac d{dt}U_{R(t)}F=\dot\theta(t)D_e(U_{R(t)}F).$$ Apply [\[eq:genfinal\]](#eq:genfinal) to the test $U_{R(t)}F$, then [\[eq:testrotate\]](#eq:testrotate) with $s=qm$, and integrate the path length. The factor $21^{m/2}2^{qm}$ is absorbed into $C_*^{m+1}$. This proves [\[eq:rotfinal\]](#eq:rotfinal) uniformly at intermediate points and endpoints. Every estimate used the same $\eta_K$, which tends to zero by [\[eq:rateexplicit\]](#eq:rateexplicit).

This completes the proof of Theorem 1: the action, observable/contact, and common-path conclusions have all been derived from P0--P4, with fixed source-order exponents and no additional uniformity assumption. A convergent subsequence of this same hierarchy would therefore be rotation covariant, but its existence, positivity and remaining reconstruction conditions are not asserted here.
