# A direct multi-component theorem for C-05

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

## What this proves

This note proves a self-contained sufficient theorem for a finite family of completed components. It accommodates holomorphic, current-dependent normalized kernels. The theorem gives a zero-free reduced scalar partition function, a normally convergent connected expansion, a rooted scalar bound, and weighted Hessian estimates. No original-birth labels enter the proof.

The source-specific task is to verify its component-incidence and current-root incidence hypotheses for the actual rebased crosspotentials, on a common current/native domain. That verification is not supplied by merely citing a pointwise activity bound.

The companion [C-05: normalized components and a direct rooted analytic norm](one component and cauchy) proves the one-component version, exact kernel-response identities, and the directional Cauchy argument used at the end.

## 1. Exact product-kernel setup

Let \(\mathcal V\) be a finite set of components. Component \(v\) has internal variables \(\omega_v\) and a holomorphic family of bounded linear functionals \(\Pi_{v,z}\), defined on a common unital Banach algebra of functions of those variables, with the supremum norm. A fixed algebra of bounded holomorphic functions on an internal complex domain is allowed. All interactions below, their products, and their norm-convergent exponentials must belong to the compatible joint function algebra. Assume

\[
\Pi_{v,z}1=1,\qquad \|\Pi_{v,z}\|\le M,\qquad M\ge1,
\tag{MC1}
\]

uniformly on a common complex parameter domain \(D\). The family is holomorphic in operator norm. Set

\[
\Pi_z=\bigotimes_{v\in\mathcal V}\Pi_{v,z}.
\]

The tensor product means that the kernels integrate disjoint internal slots and their coefficients depend only on the fixed external parameters \(z\), not on another component's integration variable. Any cross-component dependence belongs in the interaction below.

More precisely, assume that the iterated product functionals exist on the function algebra used here, are holomorphic in \(z\) in the operator norm of that algebra, factorize on functions of disjoint slot sets, and satisfy

\[
\left|\Pi_z F(\omega_I)\right|\le M^{|I|}\|F\|_\infty
\quad(I\subset\mathcal V).
\tag{MC1a}
\]

Finite complex integral kernels, holomorphic in variation norm and of total variation at most \(M\), have these properties. They are explicit assumptions if the \(\Pi_{v,z}\) are specified only as abstract bounded functionals; an arbitrary formal tensor product is not enough. A source operator that evaluates analytic observables at complex arguments must be checked on its actual common analytic function algebra. It is not asserted to act analytically on every bounded nonanalytic observable.

Let \(\mathcal E\) be a finite or countable family of holomorphic interactions \(V_e(z,\omega_{I_e})\), with nonempty finite \(I_e\subset\mathcal V\). Let

\[
v_e=\sup_{z\in D}\|V_e(z)\|_\infty.
\]

Terms with \(I_e=\varnothing\) are deterministic external scalar terms and can be added separately.

For spatial bookkeeping, assign a current-coordinate support \(S_e\) to interaction \(e\) that includes both:

- the current parameters on which \(V_e\) depends;
- the current parameters on which any \(\Pi_{v,z}\), \(v\in I_e\), depends.

This enlargement retains the moving-kernel response. Native carrier support and actual current-coordinate support must not be conflated.

Assume nonnegative extents \(\ell_e\) have the following property: for any family \(e_1,\ldots,e_n\) connected by overlaps of their \(I_e\)'s,

\[
\sup_{i,j\in \bigcup_{a=1}^n S_{e_a}}\rho(i,j)
\le\sum_{a=1}^n\ell_{e_a}.
\tag{MC2}
\]

The condition is vacuous if the union is empty. One sufficient construction is to place an anchor for every component in the spatial metric, include the anchors of \(I_e\) together with \(S_e\), and take \(\ell_e\) to dominate that enlarged set's diameter. Overlapping interactions then share an anchor.

Fix \(\chi\ge0\) and define

\[
w_e=M^{|I_e|}v_e e^{\chi\ell_e}.
\tag{MC3}
\]

The two quantitative hypotheses are

\[
2\sup_{v\in\mathcal V}
\sum_{e:\,v\in I_e}w_e e^{|I_e|}
\le1,
\tag{MC4}
\]

and

\[
K_\chi
:=
\sup_i\sum_{e:\,i\in S_e}w_e e^{|I_e|}
<\infty.
\tag{MC5}
\]

For a uniform small Hessian bound, \(K_\chi/P^2\) will have to be small on the actual common current polydisc of radius \(P\). Condition (MC4) alone does not establish that separate root estimate.

## 2. The theorem

Define

\[
Z(z)=\Pi_z\exp\left(\sum_{e\in\mathcal E}V_e(z)\right).
\tag{MC6}
\]

Under (MC1)–(MC5), the sum of interactions is absolutely convergent in the bounded-function norm, \(Z(z)\ne0\) on \(D\), and there is a holomorphic logarithm \(F(z)\) defined by the connected expansion

\[
F(z)
=
\sum_{n\ge1}\frac1{n!}
\sum_{e_1,\ldots,e_n}
\kappa_{\Pi_z}(V_{e_1},\ldots,V_{e_n}).
\tag{MC7}
\]

The series is normally convergent. Terms whose overlap graph is disconnected vanish.

For each current root \(i\), the absolute connected-series norm satisfies

\[
\sum_{n\ge1}\frac1{n!}
\sum_{\substack{e_1,\ldots,e_n\\
i\in S_{e_1}\cup\cdots\cup S_{e_n}}}
e^{\chi R_i(S_{e_1}\cup\cdots\cup S_{e_n})}
\sup_D
\left|
\kappa_{\Pi_z}(V_{e_1},\ldots,V_{e_n})
\right|
\le K_\chi,
\tag{MC8}
\]

where \(R_i(S)=\sup_{j\in S}\rho(i,j)\).

If \(D\) includes a common current polydisc of radius \(P\), then on its concentric \(\theta P\) subdomain, \(0\le\theta<1\),

\[
\sup_i\sum_j e^{\chi\rho(i,j)}
\|D_iD_jF\|_{\mathrm{op}}
\le
\frac{4d_*K_\chi}{(1-\theta)^2P^2}.
\tag{MC9}
\]

Here \(d_*\) bounds the dimension of a current-coordinate block. For scalar coordinates, \(d_*=1\).

For every fixed scalar root \(i\) and directions \(\|v_a\|_\infty\le1\),

\[
|D^mF[e_i,v_2,\ldots,v_m]|
\le
\frac{m^mK_0}{[(1-\theta)P]^m}
\le
\frac{e^m m!K_0}{[(1-\theta)P]^m}.
\tag{MC10}
\]

This higher-order conclusion is a directional multilinear bound. It is not a dimension-free absolute sum of every tensor coefficient.

## 3. Dependency-graph cumulant bound

The required combinatorics can be proved directly.

For a tuple \(e_1,\ldots,e_n\), define a simple graph \(G\) on \(\{1,\ldots,n\}\) by connecting \(a,b\) whenever \(I_{e_a}\cap I_{e_b}\ne\varnothing\). Repeated interaction labels are allowed and give distinct vertices.

Set \(a_e=M^{|I_e|}v_e\). For a vertex subset \(B\), its joint moment obeys

\[
|m(B)|
:=
\left|\Pi_z\prod_{a\in B}V_{e_a}\right|
\le
M^{|\bigcup_{a\in B}I_{e_a}|}
\prod_{a\in B}v_{e_a}
\le
\prod_{a\in B}a_{e_a}.
\tag{MC11}
\]

Moreover, \(m(B)\) factorizes over the connected components of \(G[B]\), because the associated sets of internal slots are disjoint and the untouched kernels evaluate \(1\) to \(1\).

### Lemma MC1

Writing \(\tau(G)\) for the number of spanning trees of \(G\), with \(\tau(G)=0\) when \(G\) is disconnected and \(\tau(G)=1\) for a single vertex,

\[
|\kappa_{\Pi_z}(V_{e_1},\ldots,V_{e_n})|
\le
2^{n-1}\tau(G)\prod_{a=1}^n a_{e_a}.
\tag{MC12}
\]

**Proof.** Start from the moment-cumulant formula

\[
\kappa
=\sum_{\pi\in\Pi_n}
(-1)^{|\pi|-1}(|\pi|-1)!
\prod_{B\in\pi}m(B).
\tag{MC13}
\]

Refine every block of \(\pi\) into its connected components in \(G\), obtaining a partition \(\sigma\) into connected blocks. The quotient \(G/\sigma\) has one vertex for each block and an edge for each adjacency between distinct blocks; internal edges are discarded, so they do not become loops. For a fixed \(\sigma\), the coefficient of \(\prod_{C\in\sigma}m(C)\) equals the coefficient of \(t\) in the chromatic polynomial of this quotient. Indeed, the original blocks are exactly partitions of the quotient vertices into independent sets, and the coefficient of \(t\) in the falling factorial \((t)_q\) is \((-1)^{q-1}(q-1)!\).

For a connected loopless graph \(H\), the absolute value of this linear chromatic coefficient is at most \(\tau(H)\). This follows by deletion-contraction: after applying the sign \((-1)^{|V(H)|-1}\), the coefficient is nonnegative and satisfies the same additive recurrence as spanning-tree counts on nonbridge edges, with the bridge and single-vertex cases giving the initial inequalities. Parallel edges can only increase the spanning-tree count; a loop makes the chromatic coefficient zero.

Thus, for connected \(G\),

\[
|\kappa|
\le
\left[
\sum_{\sigma\text{ with connected blocks}}
\tau(G/\sigma)
\right]\prod_a a_{e_a}.
\]

Use the quotient multigraph when counting trees; this only increases the bound. Since every induced connected block has at least one spanning tree,

\[
\begin{aligned}
\sum_\sigma\tau(G/\sigma)
&\le
\sum_\sigma
\tau_{\mathrm{multi}}(G/\sigma)
\prod_{C\in\sigma}\tau(G[C])\\
&=2^{n-1}\tau(G).
\end{aligned}
\tag{MC14}
\]

For the equality, choose a spanning tree \(T\) of \(G\) and a subset of its \(n-1\) edges. The components of the chosen forest form \(\sigma\), the chosen edges give the internal block trees, and the remaining edges give the quotient tree. This is a bijection with the objects counted on the previous line.

If \(G\) is disconnected, all relevant quotient graphs are disconnected, their chromatic polynomials have no linear term, and the cumulant vanishes. This proves (MC12).

The proof uses product factorization and bounded normalized kernels. It does not assume that the complex kernels are probability measures.

## 4. Rooted-tree summation

Let interactions \(e,f\) be adjacent when \(I_e\cap I_f\ne\varnothing\). For a fixed root interaction \(e\), define the nonnegative rooted-tree sum

The summation relation \(f\sim e\) includes \(f=e\). This is necessary because different vertices of a cumulant tuple may carry the same interaction label.

\[
\mathcal T_e
=
\sum_{n\ge1}\frac{2^{n-1}}{(n-1)!}
\sum_{e_2,\ldots,e_n}
\sum_{T\in\mathsf T_n}
\prod_{a=2}^n w_{e_a}
\prod_{\{a,b\}\in T}
\mathbf1_{I_{e_a}\cap I_{e_b}\ne\varnothing},
\quad e_1=e.
\tag{MC15}
\]

The exponential generating function for the children of a rooted tree gives the monotone recursion

\[
\mathcal T_e
=\exp\left(2\sum_{f\sim e}w_f\mathcal T_f\right).
\tag{MC16}
\]

One can use this as a formal nonnegative series identity, or obtain it by truncating tree height and then taking monotone limits.

Put \(A_e=|I_e|\). From (MC4),

\[
2\sum_{f\sim e}w_f e^{A_f}
\le
2\sum_{v\in I_e}\sum_{f:\,v\in I_f}w_f e^{A_f}
\le|I_e|=A_e.
\tag{MC17}
\]

Induction on truncated height therefore gives

\[
\mathcal T_e\le e^{|I_e|}.
\tag{MC18}
\]

This establishes the required tree summation uniformly in the number of components.

## 5. Rooted connected norm and convergence

For a connected tuple, (MC2) and (MC12) imply

\[
e^{\chi R_i(S_{e_1}\cup\cdots\cup S_{e_n})}
\sup_D|\kappa|
\le
2^{n-1}\tau(G)\prod_{a=1}^n w_{e_a}.
\tag{MC19}
\]

If the union of the current supports contains \(i\), at least one tuple entry has \(i\in S_{e_a}\). Bound this indicator by the sum of these \(n\) indicators. Symmetry changes \(1/n!\) into \(1/(n-1)!\). Rooting at the selected entry and using (MC18) gives

\[
\text{left side of (MC8)}
\le
\sum_{e:\,i\in S_e}w_e\mathcal T_e
\le
\sum_{e:\,i\in S_e}w_e e^{|I_e|}
\le K_\chi.
\]

For the unrooted series, mark any interaction in the tuple in the same way. Its total absolute value is at most
\(\sum_e a_e e^{|I_e|}\), which is finite because every \(I_e\) is nonempty and (MC4) bounds its sum by a constant times \(|\mathcal V|\).

This also gives \(\sum_e v_e<\infty\), so the interaction sum and its exponential are well-defined in the bounded-function algebra.

To identify the logarithm, insert a scalar parameter \(\lambda\) in front of every \(V_e\). Near \(\lambda=0\), (MC7) is the ordinary convergent cumulant Taylor series of \(\log Z(\lambda,z)\). The tree majorants make the connected series normally convergent for \(|\lambda|<1\), with absolute convergence up to \(|\lambda|=1\). Analytic continuation yields

\[
Z(\lambda,z)=\exp F(\lambda,z)
\]

throughout \(|\lambda|<1\), and continuity gives the same equality at \(\lambda=1\). Consequently \(Z(1,z)\ne0\), and (MC7) supplies its holomorphic logarithm on \(D\).

Uniform convergence on the common current/native domain and the rooted estimate justify the termwise derivatives. Applying the mixed-direction Cauchy argument of DN10–DN12 to each cluster coefficient gives (MC9); the \(m\)-direction version gives (MC10).

## 6. Absolute all-order jets with a physical-tree reserve

The directional bound (MC10) can be strengthened to an absolute sum over all remaining derivative endpoints. This requires additional physical geometry and a reserve in the exponential weight; directional Cauchy alone does not supply that sum.

Take the current parameter indices to lie on a metric lattice satisfying

\[
|B_\rho(i,t)|\le C_d(1+t)^d,\qquad t\ge0.
\tag{MC20}
\]

For now each lattice index labels one scalar coordinate. A fixed finite number of coordinates per site changes only exponential-in-order constants.

Strengthen (MC2) as follows. Each interaction has a genuine connected tree \(T_e\) in the physical metric, visiting \(S_e\) and one specified anchor for every component in \(I_e\), of total length at most \(\ell_e\). When two interactions share a component, their trees meet at its anchor. Thus every overlap-connected tuple has a connected union of these trees. Writing \(t=\sum_a\ell_{e_a}\), that union has length at most \(t\), visits its entire current support \(S\), and yields

\[
\tau_\rho(i,j_2,\ldots,j_m)\le t,
\qquad
|S|\le C_d(1+t)^d
\quad\text{if }i,j_2,\ldots,j_m\in S.
\tag{MC21}
\]

Here \(\tau_\rho\) is the infimum of the length of a connected physical tree visiting the displayed endpoints. No contraction of omitted component interiors is built into this definition.

Assume (MC4)–(MC5) at an exponent \(\lambda>\chi\ge0\), with weights \(M^{|I_e|}v_e e^{\lambda\ell_e}\), and put \(\delta=\lambda-\chi\), \(p=(1-\theta)P\). Then for \(m\ge1\),

\[
\begin{aligned}
\sup_i\sum_{j_2,\ldots,j_m}
e^{\chi\tau_\rho(i,j_2,\ldots,j_m)}
\left|D_iD_{j_2}\cdots D_{j_m}F\right|
\le {}&
\frac{K_\lambda m!}{p^m}
C_d^{m-1}e^\delta
\frac{[d(m-1)]!}{\delta^{d(m-1)}}.
\end{aligned}
\tag{MC22}
\]

For \(m=1\), the endpoint sum is empty, the tree length is zero, and the formula uses \(0!=1\).

**Proof.** Fix a connected coefficient in (MC7), with current support \(S\) and total tree-length bound \(t\). Ordinary multivariate Cauchy on the radius-\(p\) polydisc gives, for each ordered endpoint tuple,

\[
|D_iD_{j_2}\cdots D_{j_m}A|
\le m!p^{-m}\sup_D|A|.
\]

This follows because the product of the factorials of repeated-coordinate multiplicities is at most \(m!\). Derivatives vanish unless every endpoint belongs to \(S\). There are at most \(|S|^{m-1}\) choices of the unanchored endpoints. By (MC21), their total weighted derivative contribution is at most

\[
m!p^{-m}C_d^{m-1}(1+t)^{d(m-1)}e^{-\delta t}
\left(e^{\lambda t}\sup_D|A|\right).
\]

For an integer \(r\ge0\),

\[
(1+t)^r e^{-\delta t}
\le e^\delta r!\delta^{-r},
\tag{MC23}
\]

because the degree-\(r\) term of \(e^{\delta(1+t)}\) is \([\delta(1+t)]^r/r!\). Apply this with \(r=d(m-1)\). The proof of (MC8), at weight \(\lambda\), bounds the sum of the parenthesized quantities over connected coefficients anchored at \(i\) by \(K_\lambda\): in that proof one may use the full product weight \(e^{\lambda t}\), before weakening it to \(e^{\lambda R_i(S)}\). This proves (MC22).

In four dimensions,

\[
[4(m-1)]!\le4^{4(m-1)}[(m-1)!]^4,
\]

by the multinomial theorem. Hence (MC22) has the form

\[
\sup_i\sum_{j_2,\ldots,j_m}
e^{\chi\tau_\rho(i,j_2,\ldots,j_m)}
\left|D_iD_{j_2}\cdots D_{j_m}F\right|
\le K_\lambda C^m(m!)^5p^{-m},
\tag{MC24}
\]

where \(C\) depends only on \(C_4\) and the fixed reserve \(\delta>0\). Fixed block dimensions can be absorbed into \(C^m\). The sharper dimension-free second-order bound (MC9) remains available and does not need this endpoint-counting loss.

This corollary supplies the factorial calculation once the actual input has the strengthened physical-tree norm. It does not establish that input for Yang–Mills histories. Native-anchored jets require their own root incidence and complex radii. Bounds rooted only in current coordinates do not bound arbitrary terms depending solely on retained data.

## 7. Scalars that touch no integrated component

Interactions with \(I_e=\varnothing\) are not omitted from the action. Write their sum separately as \(W(z)\). If a normally convergent local scalar expansion of \(W(z)-W(z^0)\) has rooted analytic norm \(L_\chi\), then

\[
e^{W(z)}\Pi_z e^{\sum_eV_e(z)}
\]

has logarithm \(W+F\) with the same chosen additive reference value, and the current Hessian bound is

\[
\sup_i\sum_j e^{\chi\rho(i,j)}\|D_iD_j(W+F)\|_{\mathrm{op}}
\le\frac{4d_*(L_\chi+K_\chi)}{(1-\theta)^2P^2}.
\tag{MC25}
\]

The all-order conclusions similarly add the corresponding rooted scalar norm of \(W\). A factor depending only on retained data has zero current derivatives on the slice that fixes those data, but remains part of the outer measure. This observation does not bound its independently native-anchored derivatives.

## 8. Application checklist for the actual source construction

The source expression (1.103) is algebraically of the form (MC6) when the completed-component kernels have been normalized and all remaining couplings are put in \(V\).

The analytic theorem above does not require preservation of original birth labels. It does require:

1. **Exact rebasing:** old factors internal to one new component are included in that component's actual kernel. Terms coupling distinct components remain in \(V\); they cannot be hidden in a product kernel.
2. **Common domain:** the normalized source bound, such as (1.75), holds for the exact rebased kernels on the pulled-back complex current/native domain.
3. **Component incidence:** the actual crosspotentials satisfy (MC4), including \(M^{|I_e|}\), the extent weights, and the exponential size factor.
4. **Current incidence:** (MC5) is uniform in the actual histories and small enough after division by the current Cauchy radius squared.
5. **Spatial extent:** the actual carrier geometry and current-map localization establish (MC2). This must use the source's real definition of its tree metric.

If a per-component total crosspotential is bounded by \(C\alpha_k\operatorname{poly}(R_k)\), and the source supplies sufficiently small \(\alpha_k\), that may help prove (MC4). It is not yet a proof of (MC5), nor of the spatial extent property. Conversely, if the source decay metric is an ordinary spanning-tree metric of all active exterior cubes, its existing decay can pay spatial extent directly; one should not replace it by a weaker zero-cost-hole metric.

**Status:** The multi-component theorem is proved above under explicit hypotheses. Its verification for the complete admitted Yang–Mills construction remains the decisive application obligation. No C-05 closure is claimed solely from this abstract theorem.
