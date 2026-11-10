# Ordinary older Gaussian and Schur response

**Annex AS.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. The current factorization and its response factor

Being supported in the old large-field region does not by itself make an operation independent of a newer current coordinate. CMP119 (1.29), (2.21) contains background-dependent quadratic forms and constrained covariances. LFR II (1.71), pp.379–380, explicitly retains a dependence of the completed operation on its native pair \((U,J)\). If that pair is a function of the newer current, its response must be kept unless an exact determining-data identity makes it constant.

Fix a positive history branch, every old integration coordinate \(a\), and the current free variable \(z\). Suppose its old-operation density is \(w(z,a;v)\), with common support in \(a\) on the fixed chart, and choose the reference current \(z=0\). Then, wherever the reference density is positive, the exact additional current exponent is

\[
 \Theta(z,a;v)=\log\frac{w(z,a;v)}{w(0,a;v)}.
 \tag{OR17.1}
\]

The reference factor \(w(0,a;v)\) remains in the outer measure. Zero sets common to the support do not affect the identity. It is not permissible to replace \(w(z,a;v)\) by \(w(0,a;v)\) without the factor \(e^{\Theta}\). If the density is a product of explicit exponentials and fixed selectors, (OR17.1) is the sum of their exact exponent differences and requires no logarithm of a possibly small total integral.

This observation does not establish common support, native analyticity, or a spatial bound for the actual source density. Those are source matching requirements below. A background-dependent delta constraint or selector would need a separate exact coordinate treatment; it cannot be absorbed into an ordinary analytic logarithm.

### 2. Exact response of a retained Gaussian Schur form

Let \(K(\xi)\) be a holomorphic symmetric matrix on fixed free coordinates, positive on the real slice. Split its indices into the already integrated set \(I\) and the retained set \(O\). Assume \(K_{II}\) is invertible throughout the admitted chart. Define

\[
 G=K_{II}^{-1},\qquad
 S=K_{OO}-K_{OI}G K_{IO},\qquad
 \mathcal E a=(-G K_{IO}a,\ a).
 \tag{OR17.2}
\]

Here the first component is indexed by \(I\). All transposes below are bilinear transposes in the holomorphic continuation, agreeing with real transposes on the real slice. The exact retained exponent is

\[
 q(\xi,a)=-\tfrac12 a^{\mathsf T}S(\xi)a
          =-\tfrac12(\mathcal E a)^{\mathsf T}
                         K(\xi)(\mathcal E a).
 \tag{OR17.3}
\]

For any admitted directional variation \(\dot\xi\),

\[
 \dot S=\mathcal E^{\mathsf T}\dot K\mathcal E,
 \qquad
 \dot q=-\tfrac12(\mathcal E a)^{\mathsf T}
                          \dot K(\mathcal E a).
 \tag{OR17.4}
\]

**Proof.** The \(I\)-component of \(K\mathcal E a\) is zero, while the \(O\)-component of \(\dot{\mathcal E}a\) is zero. Thus both terms differentiating \(\mathcal E\) in (OR17.3) vanish. The remaining term is (OR17.4). Equivalently, differentiate \(G\) using \(\dot G=-G\dot K_{II}G\) and collect the four Schur-complement terms. No derivative of the covariance is discarded. The identity holds on the complex chart as an algebraic matrix identity. \(\square\)

If the source retains only within-component quadratic terms, extend the retained vector by zero outside one component and apply the same identity component by component. Older cross-component terms assigned to primitive B must not be counted again in (OR17.3).

#### A spatial consequence, with its exact hypotheses

Suppose that in old current units, for a local native direction at an anchor \(x\),

\[
 |\dot K_{bc}|\le A\,u(x)
   e^{-c[\rho(b,x)+\rho(c,x)]},
 \quad
 |\mathcal E_{br}|\le A e^{-c\rho(b,r)},
 \quad r\in O.
 \tag{OR17.5}
\]

Let \(a\) be supported in \(C\subset O\), with \(\|a\|_\infty\le P\). Exponential convolution and (OR17.4) give, at reduced fixed rates,

\[
 |\dot q|\le C A^3 P^2 u(x)
        \left(\sum_{r\in C} e^{-c'\rho(x,r)}\right)^2
 \le C' A^3P^2u(x)
       \sum_{r\in C}e^{-c''\rho(x,r)}.
 \tag{OR17.6}
\]

The second inequality uses the volume-independent lattice sum
\(\sup_x\sum_{r}e^{-c'\rho(x,r)}<\infty\). Lie-algebra coordinate multiplicities enter fixed constants. The same argument works on tori, with their periodic distance, and for principal restrictions. No factor equal to the size of \(C\) appears without an exponential anchor.

This is a consequence of a **local coefficient-response bound** in (OR17.5). Exponential decay of \(K_{bc}\) alone is not that bound. A spatially nonlocal dependence of a single entry on a parameter would violate the inference. For the actual application the local response must be obtained from the source operators, their localized expansions or their exact resolvent variations, with their physical measures and old-layer weights retained.

### 3. What would close the additional old-operation row

For an actual old operation of scale \(j\), the current pullback of its native arguments must be the same admitted family as that operation's source definition, including its local collar reconstructions. The exact C-05 endpoint/current-domain results can be used only after this identification.

A sufficient concrete old-operation row is

\[
 |\partial_{z_i}\Theta_{j,X}(z,a;\xi)|
 \le \frac{K_{j,X}}{P_k}\,
       \theta_k(1+k-j)^b
       e^{-\Gamma(k-j)-c_{\rm col}M R_k}
       e^{-c d_X(i)}
 \tag{OR17.7}
\]

on the full common current/native contour. Here each prefactor and carrier count must be actual, rather than postulated: a Gaussian coefficient can carry \(P_j^2\); a replaced component can have its displayed source polynomial size cost. The available fixed logarithmic and age powers must be stated before summation. Fixed powers of \(g_j^{-1}\), if present, also need an explicit current-collar payment and an AF age comparison.

With a summable carrier decomposition, (OR17.7) supplies the all-order jets by BC16, including the weighted Hessian row. This is a sufficient implication, not an assertion that the source matching is already done.

The Gaussian calculation uses CMP119 (2.21) and CMP99 (3.155)–(3.158), Theorem 3.15. The replaced operation uses LFR II (1.65), (1.71)–(1.75). A normalized-kernel value bound alone does not control its current response.

### 4. The actual ordinary Gaussian operation

This section applies the response argument to the unreplaced operations of CMP119 (2.21). It does not assert an analogous pointwise application to all hidden variables of a completed R operation. That is a distinct question, and the alternative representation in LFR II (1.103)–(1.104) is treated separately in Annex AT, Section 7.

#### 4.1 Exact source coefficients and their local dependence

The source free-coordinate precision is
\[
 K_j=C_j^*\Delta^{(j)}C_j.
 \tag{OR17.8}
\]
Its definition includes the background-current term in CMP99 (3.156). The source covariance in (3.158) is the inverse principal block in these free coordinates. Thus the within-component quadratic form in CMP119 (2.21) is exactly (OR17.3), with the retained vector supported in that component. This is the same ordinary Gaussian law, not a Laplacian substitution.

The following primary results provide **local dependence** as well as off-diagonal kernel decay:

- CMP99 p.413, Theorem 3.9: each localized inverse coefficient depends only on the background restricted to the specified fixed enlargement of its carrier.
- CMP99 pp.415–416, Theorem 3.10 and (3.108): the walk representation has the stated walk/tree decay and depends only on the union of the indicated enlarged blocks.
- CMP99 p.422: the inverse coarse averaging operator occurring in (3.156) is handled by the same construction. The current correction and the \(H_1\) factors have the corresponding expansions, including the branches described on p.427; the shortest-tree length replaces the single-line length.
- CMP99 p.432, Theorem 3.15 and (3.187): the actual principal-restriction fluctuation covariance has the same localized expansion and locality consequences.

The analytic coefficient extension is the one in Section B of that paper, pp.399–400, and its stated current extension. The actual native current term is retained. The current external pair in the present application lies in a smaller uniform strong domain by NP.5 and the older-scale embedding used there. A regular complex neighborhood of the principal inverse is obtained either directly from the stated source domain or by the uniform real lower bound and a fixed small complex perturbation. Its radius is fixed before summing over old operations.

The local map \(C_j\) introduces neither an extra long-range dependence nor a noncovariant substitution. It solves the actual linear averaging constraint on the fixed exceptional bonds. Under a simultaneous gauge change, that equation and the zero tree conditions transform covariantly. Uniqueness of the exceptional-bond solution therefore gives the endpoint-adjoint transformation rule for \(C_j\). Scalar localization cutoffs commute with this rule. Products, localized inverses and the displayed current correction consequently give endpoint-adjoint covariance for each localized free-coordinate coefficient. This verifies the gauge rule needed below; covariance of a fine Green function alone would not suffice.

Use the actual physical measures in these kernel compositions. The source walk bounds include their normalized row sums; multiplying their kernels is not an unweighted count of fine bonds. The resulting localized expansion of the Schur form has primitive terms
\[
 q_{j,\mathcal W,r,s}
   =-\tfrac12 a_r^{\mathsf T}
          S_{j,\mathcal W}(r,s;U,J)a_s,
 \qquad r,s\in C,
 \tag{OR17.9}
\]
where \(\mathcal W\) denotes the actual finite tree/walk data and its carrier contains the two old endpoints. At every fixed cutoff the sum is exact. Absolute normal convergence and the fixed decay reserves justify its grouped carrier form. With the source parameters chosen as in the existing carrier analysis, its rooted analytic norm is bounded by
\[
 C P_j^2 e^{-\kappa\, t_j(\mathcal W)}.
 \tag{OR17.10}
\]
Here \(t_j\) is the source tree/walk length, with the fixed equivalent carrier convention, and the bound includes the summation of internal walk labels at a fixed root. The retained old field is bounded by \(C\varepsilon_j/g_j\le C'P_j\), by the actual preliminary small-field restriction; constants include \(A_0/A_1\). No small-field restriction is imposed on a raw large-field link outside that ordinary fluctuation region, since it is not one of the \(a\) variables in this quadratic form.

#### 4.2 Gauge and current admission with old fields fixed

Each scalar in (OR17.9) has only two displayed old adjoint slots. They are on the ordinary \(j\)-grid in \(\Omega_{j+1}\cap Z_{j+1}\). Apply AD17.3 to the actual required endpoints, using its proved terminal-layer grading and the converter bound JI.40. Its double real covariance identity gives an admitted holomorphic fixed-old-field expression for (OR17.9). There is no need to rotate an arbitrary hidden raw variable or to assume an unprinted complex old-field product domain.

The strong native ball is simultaneous with the full current contour and with the independent-current slot. The source-local enlarged carrier and the interpolation collar differ by fixed physical-scale factors. Cauchy on that genuine ball, using the original-map one-current endpoint row, gives the analogue of (BC16.4) with primitive prefactor (OR17.10). All derivatives of the actual \(C_j\), constrained Hessian, principal inverse and nonlinear current insertion are included by this composed analytic function. The elementary identity (OR17.4) independently verifies that the covariance response has not been frozen.

Every primitive carrier in (OR17.9) meets an old retained fluctuation site in \(Z_{j+1}\). The actual current-to-boundary path, together with the source tree connector when the native attachment is elsewhere on that carrier, therefore supplies the collar and age factors exactly as in BV.6–BV.12 and BC16.5. Reserve separate fixed portions of the decay for the current collar, the old-age count, and the final spatial weight. This gives (OR17.7), with \(K_{j,X}\) carrying the explicit \(P_j^2\) factor.

The distinction between a path to an old boundary and a path to an earlier output layer remains in force. For an output layer earlier than \(j+1\), use the actual path to that layer; for a later output layer use the carrier connection to the old endpoint. This is the combined path/carrier argument already established in BC16.5, not an assignment of the same decay to two different costs.

#### Theorem OR17.1 — ordinary old-operation response budget

On the retained source class and the common current/native contour, the sum of the exact ordinary Gaussian density responses has the same all-order anchored current estimate as BC16.13, with prefactor
\[
 \mathcal K^{\rm G}_{T,k}
 \le C\,\theta_k P_k^2 e^{-c_{\rm G}M R_k},
 \qquad \theta_k=\ell_k^{p_0-q}.
 \tag{OR17.11}
\]
In particular its weighted current Hessian is at most
\[
 C\theta_k e^{-c_{\rm G}M R_k}\longrightarrow0.
 \tag{OR17.12}
\]
The constants are independent of cutoff depth, volume and admitted history. Fixed native directional jets are obtained on the common smaller strong ball with the Cauchy costs stated in AB17.6.

**Proof.** The verified native first-response bound, (OR17.10) and the connector give the premises of the BC16 endpoint theorem. The exact AF comparison implies
\[
 \frac{P_j^2}{P_k^2}
 =\left(\frac{\ell_j}{\ell_k}\right)^{2p_0}
 \le C(1+k-j)^{b_0}
 \tag{OR17.13}
\]
for one fixed \(b_0\). Indeed \(g_j^{-2}\le C(1+k-j)g_k^{-2}\), so \(\ell_j\le\ell_k+\log[C(1+k-j)]\), and \(\ell_k\) has a fixed lower bound. The conservative old-root count contributes \(L^{4(k-j)}\), while the current/native radius and finitely many profile embeddings contribute fixed polynomial and dyadic costs. Choose the already fixed layer-separation reserve so that their age sum converges. The walk/tree counting and the all-order current-position count are exactly those in BC16; no derivative-order-dependent geometry parameter is selected. This yields (OR17.11) and a fixed factorial exponent five. Setting the current order to two proves (OR17.12). \(\square\)

#### 4.3 The other literal factors in an ordinary operation

CMP119 (2.21) contains the old raw Haar integration, its exact raw averaging delta, the displayed \(\zeta,\chi\) factors, and the within-component quadratic form. It does not contain an additional determinant to be silently differentiated: CMP119 p.254 after (1.30) assigns the earlier fluctuation normalization to E, and the general step keeps its constants in the corresponding action/vacuum factors. Those assigned terms are already in the appropriate sector of the boundary ledger.

For the fixed raw/delta/selector factors, use their actual local data, not a global-background surrogate. LFR I p.183, after (1.28), states their dependence on field variables localized in the corresponding large-field components. The current substitution, including its one-step constraint stencil, stays beyond the old-component collar and leaves those determining variables unchanged. Thus their supports and values are constant under the current variable in this ordinary-operation chart. This is an exact retained-data statement for these factors. It is not the incorrect inference that the quadratic coefficients are constant merely because their old integration variables have the same support.

The theorem just proved supplies the response for the latter coefficients. The exact exponent (OR17.1) with that Gaussian response gives the correct outer-law factorization without deleting a derivative. Statements about a normalized posterior containing arbitrary marked old observables, or about a completed R operation on its unintegrated hidden variables, remain separate.
