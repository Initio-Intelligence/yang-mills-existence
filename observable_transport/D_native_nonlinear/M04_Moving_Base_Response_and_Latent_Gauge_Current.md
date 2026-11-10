# Moving ancestor bases, fixed innovations, and exact latent-gauge current transport

This note separates two different terminal responses that cannot be identified. The source's direct multiscale derivative controls a coherent critical chain, including the moving-reference part of a relative minimum. It does so without multiplying one-step constants. An actual chronological chain with a nonzero **fixed raw innovation** has an additional term. A terminal gauge change rotates that innovation relative to its moving reference; the resulting change can be physical and has no ancestor-distance factor pointwise.

We give an admitted finite-chain example of that additional response, and derive the exact normalized current transport law, including the Q boundary and the original insertion/kernel labels. Its divergence identity permits cancellation inside a complete integral before absolute values. It does not permit cancellation between separately prescribed absolute current norms. A final resolvent calculation specifies what would still be needed for a transverse common-family estimate after the latent gauge terms have been handled.

The statements concern actual source maps and finite admitted chains; no arbitrary-depth interacting density construction is inferred.

## 1. The direct terminal response is a statement about a critical chain

Write \(h_i=L^i\eta\). Let

\[
 W(t)=e^{it g_k H}W_0,\qquad F(t)=U_k(W(t)),
 \tag{MB.1}
\]

where H is a whole terminal link array, \(\|H\|_\infty\le1\), the prescribed orientation convention is retained, and the real path lies in the source's strict native neighborhood. A single normalized raw coordinate direction is a special case. The coupling and every grid remain fixed along this path.

### Lemma MB.1 — a direct, age-uniform quotient response

For every \(j\le k\), source Proposition 9 supplies a relative Landau representative of (MB.1) whose velocity satisfies

\[
 \|\dot F\|_{\mathcal R_j,\mathrm{rel}}
       \le C g_k L^{-(k-j)}\|H\|_\infty.
 \tag{MB.2}
\]

The notation is the dimensionally normalized relative-potential norm of AP: its entries include \(h_j\|A\|\), \(h_j^2\|\nabla A\|\) and the force-control entry \(h_j^3\|D^*DA\|\). The derivative is taken in the displayed moving relative Landau representative. For the actual averaged-gauge j-readout there is a block-constant real gauge v(t), with v(0)=I, such that

\[
 \bar V_j(t)^{v(t)}=e^{ia_j(t)}\bar V_j(0),
 \qquad
 \|\dot a_j(0)\|_\infty
          \le C_Lg_kL^{-(k-j)}\|H\|_\infty.
 \tag{MB.3}
\]

The same conclusion applies to the actual zero-intermediate-innovation chain obtained from the readouts of F(t), understood on the common critical orbit. It does not describe an arbitrary fixed-innovation chronological chain.

**Proof.** Differentiate the relative minimum at the terminal scale k using CMP102 (182)–(190), rather than differentiating a composition of k-j one-step maps. The homogeneous terminal row measure cancels the factor \(h_k^{-4}\) in (190). The potential, first covariant derivative and force-control terms are bounded respectively by \(Cg_k/h_k\), \(Cg_k/h_k^2\), \(Cg_k/h_k^3\). Multiplication by the j-native powers gives (MB.2); the higher entries have stronger scale factors. This is exactly the direct scale normalization used in AP and BG.

The literal nonlinear j-readout has the uniform analytic averaging bounds used in AP.1. Its relative link angle has the factor \(h_j/h_k\). Canonicalize the two readouts and apply BG.10–BG.17 to this one relative pair. The transport splits as \(s v\), with v block constant and the small residual s bounded by the relative angle. Differentiating its zero-subtracted local formulas at t=0 gives (MB.3). All large real conjugations are isometries.

Finally, F(t) is critical for each finer averaging fiber: its tangent space is a subspace of the terminal fiber tangent space, and the field satisfies the finer regularity requirements. The source uniqueness of the regular critical orbit therefore identifies the intermediate minimizing readouts, as in VN/AP. This is an orbit statement; independent source gauge representatives are related by their prescribed gauge maps. No one-step derivative constant has been raised to the age. \(\square\)

## 2. A genuinely controlled moving-reference term

Let \(\mathcal A_j(B,U)\) be the relative Landau solution of CMP102 (174)–(175), or its force-corrected version (179)–(180), at j-scale relative target B and external regular reference U. The final paragraph of Section G and Proposition 9 explicitly continue these equations analytically in U. On that chosen extension,

\[
 \mathcal A_j(0,U)=0.
 \tag{MB.4}
\]

The physical identification with the relative minimum is asserted when U is the actual reference critical field. At other regular U this is the source's specified analytic extension; it is not asserted to be a new stationary field for an undeformed action.

Let \(a_{b,j}(B,U)\) denote its relative birth-b readout, followed by the local canonical comparison used in BG. If the reference is allowed to leave the canonical submanifold, use the explicitly relative continuation BG.17a; its zero subtraction at B=0 is then an identity on the whole local reference tube.

### Lemma MB.2 — the reference derivative retains the physical age factor

On fixed smaller native tubes, uniformly in the admitted real centers,

\[
 \|D_Ua_{b,j}(B,U)[\dot U]\|_\infty
       \le C_L L^{-(j-b)}\|B\|_\infty
                            \|\dot U\|_{\mathcal R_j,\mathrm{rel}},
 \tag{MB.5}
\]

and the residual maps have the same estimate. In particular the total native differential has the form

\[
 \|\dot a_{b,j}\|+\|\dot s_{b,j}\|
       +\|\dot{\widetilde a}_{b,j}\|
 \le C_LL^{-(j-b)}
       \bigl(\|\dot B\|+
               \|B\|\,\|\dot U\|_{\mathcal R_j,\mathrm{rel}}\bigr).
 \tag{MB.6}
\]

All velocities in this formula use one relative native reference chart. Returning to a field-dependent raw gauge adds the corresponding gauge velocity, as in Section 3 below.

**Proof.** The source analytic equations and (190), with their stated external-reference continuation, give

\[
 \|a_{b,j}(B,U)\|\le C_LL^{-(j-b)}\|B\|
 \tag{MB.7}
\]

uniformly on a fixed complex j-native reference tube. Its radius is in the dimensionally normalized regularity norm, not in an unscaled microscopic link supremum. The higher regularity entries and the complete force correction are included. The zero subtraction (MB.4) and BG.17a prevent a reference-only constant term. Apply the one-variable Banach-valued Cauchy estimate in the direction \(\dot U\) on a fixed smaller reference tube. The retained factor \(\|B\|\) in (MB.7) gives (MB.5). Cauchy or the source derivative in B gives the first term in (MB.6). The local analytic residual maps in BG preserve the same bound by their zero-subtracted chain rule. \(\square\)

Along the coherent critical reference \(U=U_k(W(t))\), Lemma MB.1 inserted into (MB.5) gives

\[
 \|D_Ua_{b,j}(B,U)[\dot U]\|
       \le C_L\|B\|\,g_k L^{-(k-b)}\|H\|_\infty.
 \tag{MB.8}
\]

This is a real improvement over treating the reference velocity as an unspecified constant. It controls the moving-reference contribution for that actual critical reference path. The term \(D_Ba[\dot B]\) remains. In a chronological reconstruction B is its **actual** relative target array, determined by the exact target and its independent innovation. Holding B constant in a transported chart is generally different from holding the original innovation fixed. Equations (MB.6)–(MB.8) do not identify those two operations.

## 3. The exact extra term at a fixed innovation

Use physical independent coordinates x and the actual fixed-target solve \(\Xi(W,x)\). Its normalized version is \(\Psi_W(z)=\Xi(W,g_jz)\). Endpoint covariance and uniqueness of the exceptional solve give, for a real retained gauge v and its specified block lift \(\widetilde v\),

\[
 \Xi(W^v,T_{\widetilde v}x)=\Xi(W,x)^{\widetilde v}.
 \tag{MB.9}
\]

Every target and local reference in this equality is transformed. Thus

\[
 \Xi(W^v,x)^{\widetilde v^{-1}}
       =\Xi(W,T_{\widetilde v}^{-1}x).
 \tag{MB.10}
\]

Let \(\mathfrak d_W\xi\) be the infinitesimal gauge variation of W, and \(A_{\widetilde\xi}=dT_{e^{t\widetilde\xi}}/dt|_0\) its adjoint generator on the independent fibers. Differentiating (MB.9) at a fixed physical point gives the exact identity

\[
 D_W\Xi[\mathfrak d_W\xi]
    =\mathfrak d_{\Xi(W,x)}\widetilde\xi
        -D_x\Xi[A_{\widetilde\xi}x].
 \tag{MB.11}
\]

The first term on the right is an output gauge direction. The second term is a physical innovation response in general. Removing the output gauge does not remove it. If the latent innovation is transported at the same time, \(\dot x=A_{\widetilde\xi}x\), the second term cancels. This is an actual change of latent variables, and its insertion, density and domain responses must all be retained.

### Proposition MB.3 — an admitted fixed-innovation response without age suppression

Fix an innovation level \(\ell\ge2\), and let the terminal level k exceed \(\ell+1\). There are actual admitted homogeneous real chains with all innovations above \(\ell\) zero and one small fixed innovation at level \(\ell\), for which a terminal pure-gauge raw variation has

\[
 \left|\frac d{dt}\mathcal O(V_\ell(t))\bigg|_{0}\right|
       \ge c_Lg_k a^2,
 \qquad 0<a\le c\delta_\ell,
 \tag{MB.12}
\]

where \(\mathcal O\) is a fixed finite coarse-plaquette observable and a is the physical innovation amplitude. The constants and the size of its detecting footprint are independent of \(k-\ell\). The same response is a gauge-invariant observable of the actual base minimum \(U_\ell(V_\ell(t))\).

**Proof.** Choose a terminal k-block and a real terminal gauge

\[
 v_k(t)(y)=e^{it g_kH}
 \tag{MB.13}
\]

at its center, equal to I at all other terminal centers, with H a fixed Hermitian traceless generator. Put \(W(t)=I^{v_k(t)}\). Its microscopic lift u(t) is block constant on that terminal block. The higher zero-innovation source fields are the actual flat critical fields \(I^{u(t)}\), by CMP102 (181); their intermediate targets are the literal readouts. They are already canonical at every lower block partition on which the lift is constant. The terminal derivative has at most a fixed number of nonzero normalized link directions, each of size \(g_k\).

Take two adjacent \((\ell+1)\)-blocks on the opposite sides of a face of that terminal block, away from its corners. On the \(\ell\)-grid use AF.9–AF.10's two matching tangential cochains a_0,b_0. They have fixed finite support, unit scalar normalization, zero next coarse average separately, and no exceptional-bond entries. Their actual linear exceptional embeddings are therefore themselves. Their flat coarse Wilson cross pairing is \(-c_W\), \(c_W>0\). For completeness, the scalar arrays can be chosen in the common nullspace of the at most 4d average conditions on matching tangential bonds; the allowed fixed large L leaves a nonzero array. The only common curl plaquettes cross the shared face and have opposite tangential signs, giving that nonzero cross pairing.

Choose unit Lie colours S,T with \(\langle S,T\rangle=0\) and
\(\langle i[H,S],T\rangle\ne0\). Such a triple lies in an su(2) subalgebra. Set the physical independent innovation to

\[
 x=a(a_0S+b_0T),\qquad z=x/g_\ell,
 \tag{MB.14}
\]

and hold z, equivalently x, fixed. With the actual target \(V_{\ell+1}(t)\) from the higher flat chain define
\(V_\ell(t)=\Xi(V_{\ell+1}(t),x)\). At t=0 the target is I. The lift of (MB.13) acts by the same adjoint rotation on the entire support of a_0 and is identity on b_0. Equation (MB.10) therefore reduces the gauge-invariant response to the exact local function

\[
 \mathcal O(V_\ell(t))
  =\mathcal O\!\left(\Xi\left(I,
       a[a_0\operatorname{Ad}_{e^{-it g_kH}}S+b_0T]\right)\right).
 \tag{MB.15}
\]

Choose \(\mathcal O(V)=\sum_{p\in\mathscr P}[N-\operatorname{ReTr}V(p)]\), where the fixed plaquette set \(\mathscr P\) contains the curl supports of these two cochains and the fixed exceptional-solve stencil. The exact solve has linear embedding identity on a_0,b_0. Its nonlinear corrections begin at second order. Consequently the analytic Taylor expansion at the flat field gives

\[
 \mathcal O(\Xi(I,a[a_0S'+b_0T]))
  =\frac{a^2}{2}\{c_a\|S'\|^2+c_b\|T\|^2
                         -2c_W\langle S',T\rangle\}+O_L(a^3).
 \tag{MB.16}
\]

The t derivative of the remainder in (MB.16) is \(O_L(g_ka^3)\), because all its defining paths and independent coordinates have this fixed finite stencil. The self-pairings are invariant under the adjoint rotation. The cross term has nonzero derivative \(c_Wg_ka^2\langle i[H,S],T\rangle\), up to its immaterial sign. Reduce the fixed amplitude ceiling to absorb the cubic remainder. This proves (MB.12).

For real t, the higher backgrounds remain flat. At the innovation layer, remove the higher real block-constant gauge. The independent physical entries in (MB.15) have size at most Ca. The fixed-target solve, Q reference comparison and axial cutoff have the same strict small-neighborhood admission as in AF/BA. Taking \(a\le c\delta_\ell\), with c sufficiently small for the fixed source hierarchy, gives the literal Q and preceding-selector margins. All subsequent gauge transformations of their references are the allowed block-constant ones. The R partition may be summed. Below this layer the actual regular minimum \(F_\ell(t)=U_\ell(V_\ell(t))\) exists by the source theorem, and its zero-innovation finer readouts give a finite admitted critical chain. No interacting-density induction is being used.

Finally \(\mathcal M^\ell F_\ell(t)=V_\ell(t)\) exactly. Thus \(\mathcal O\circ\mathcal M^\ell\) is a gauge-invariant detector of the same response of the actual minimum. An output gauge cannot eliminate (MB.12). \(\square\)

To compare with a proposed pointwise quotient bound, fix \(b<\ell\) as well. Constants in this comparison may depend on the fixed lower geometry \((\ell,b)\), as well as L and the fixed source conventions; they do not depend on \(k-\ell\). On that lower geometry, the derivative of \(\mathcal O\circ\mathcal M^\ell\) is at most \(C_{L,\ell,b}a\) times the b-native relative velocity. Therefore a claimed bound
\(\|\dot F_\ell\|_{\mathcal R_b,\mathrm{quot}}\le Cg_kL^{-(k-b)}\)
for all fixed innovations would force

\[
 a\le C'_{L,\ell,b} L^{-(k-b)}.
 \tag{MB.17}
\]

That restriction is absent from the actual innovation domain: its ceiling is \(c\delta_\ell\), not a terminal-distance exponential. The exact finite-chain lower bound (MB.12) holds for every supplied admitted trajectory. In any family of such trajectories for which \(L^{k-b}\delta_\ell\) is unbounded, (MB.17) disproves a uniform constant in the proposed fixed-innovation estimate. This is the relevant sum-of-scales distinction; no existence of an infinite interacting trajectory is asserted here.

This example is pointwise in the latent innovation. It does **not** give a nonzero derivative of the completed conditional under a terminal gauge transformation. The latent change of variables in (MB.10), applied to the density and the Q domain as well, cancels that total response exactly. At a flat Gaussian reference even some of the separate integrated first responses vanish by colour symmetry, as shown next.

## 4. Exact normalized transport with the Q boundary retained

Consider one actual real conditional node,

\[
 H(t)=Z_t^{-1}\int_{D_t}\rho_t(z)f_t(z)\,dz,
 \qquad Z_t=\int_{D_t}\rho_t(z)\,dz.
 \tag{MB.18}
\]

Its complete \(\rho_t\) contains its force-corrected Gaussian, the determinant of that same covariance, all interactions and Haar/coarea factors. The actual old conditional denominators are retained whenever they occur inside a test or a density. Let \(s_t=\partial_t\log\rho_t\) on this real path. If a boundary is differentiable, denote its normal velocity by \(v_D\cdot n\). More generally write
\(\mathcal B_t(F)=\langle\partial_t1_{D_t},F\rangle\)
for its prescribed weak first boundary current. The existing Q first-shell representation supplies this interpretation; no second raw derivative of a sharp intersection is assumed.

Differentiation of the **same** numerator and denominator gives the original owned contributions

\[
 I_t=\mathbb E_t[\partial_tf_t],\qquad
 K_t=\operatorname{Cov}_t(f_t,s_t),\qquad
 B_t=Z_t^{-1}\mathcal B_t(\rho_t(f_t-H(t))),
 \qquad \dot H=I_t+K_t+B_t.
 \tag{MB.19}
\]

Here I is insertion-at-fixed-z, K is kernel-at-fixed-test, and B is its physical domain contribution. Centering in K and B is the derivative of the full normalizer, not a discarded vacuum term.
The boundary contribution remains attached to its original physical kernel label. The displayed bulk/shape separation does not create a new independent source origin or reassign any old one.

Choose a real differentiable latent change of variables with velocity w_t(z), and put

\[
 \delta_{\rho_t}w_t
       =\operatorname{div}w_t+w_t\cdot\nabla\log\rho_t.
 \tag{MB.20}
\]

Define its own boundary functional without requiring a smooth boundary by

\[
 \mathcal F_{w,t}(F)=\int_{D_t}\operatorname{div}(Fw_t)\,dz.
 \tag{MB.21}
\]

When the usual boundary integral is available, this equals \(\int_{\partial D_t}F w_t\cdot n\). For a Q domain carried by a real diffeomorphism, (MB.21) is also its exact weak transport derivative, directly by change of variables.

### Theorem MB.4 — the full current transport identity

At every admitted differentiability point, or in the corresponding weak path-integrated sense,

\[
 \begin{split}
 \dot H={}&\mathbb E_t[(\partial_t+w_t\cdot\nabla)f_t]\\
 &+\operatorname{Cov}_t(f_t,s_t+\delta_{\rho_t}w_t)\\
 &+Z_t^{-1}(\mathcal B_t-\mathcal F_{w,t})
                              (\rho_t(f_t-H(t))).
 \end{split}
 \tag{MB.22}
\]

Equivalently the transport correction obeys the exact integration-by-parts identity

\[
 \mathbb E_t[w_t\cdot\nabla f_t]
   +\operatorname{Cov}_t(f_t,\delta_{\rho_t}w_t)
       = Z_t^{-1}\mathcal F_{w,t}
                              (\rho_t(f_t-H(t))).
 \tag{MB.23}
\]

**Proof.** Expand
\(\operatorname{div}(\rho_t(f_t-H)w_t)\).
Its integral is the right side of (MB.23). Dividing by Z gives
\(\mathbb E[w\cdot\nabla f]+\mathbb E[(f-H)\delta_\rho w]\), proving that formula with its exact centered normalizer. Add the resulting zero to (MB.19). This proves (MB.22). For a transported measurable real domain the same calculation is justified first against smooth test functions using the exact change of variables; it gives the weak form (MB.21). The existing common first-current majorants then justify the path integral and the primitive coefficient applications. No independent Gaussian determinant is introduced. \(\square\)

For a pure source gauge path, let \(T(t)\) be the full block-constant adjoint action on the independent coordinates. The complete covariance identities are

\[
 f_t(T(t)y)=f_0(y),\quad
 \rho_t(T(t)y)\det T(t)=\rho_0(y),\quad
 D_t=T(t)D_0.
 \tag{MB.24}
\]

Choose \(w_t(z)=\dot T(t)T(t)^{-1}z\). Then the three terms on the right of (MB.22) vanish individually: the material insertion derivative is zero, the material score is zero, and the domain current is exactly \(\mathcal F_w\). Thus the completed gauge response is zero, with all Q references and both normalizers included. In the original origins, however,

\[
 I_t=-\mathbb E_t[w_t\cdot\nabla f_t],\quad
 K_t=-\operatorname{Cov}_t(f_t,\delta_{\rho_t}w_t),\quad
 B_t=Z_t^{-1}\mathcal F_{w,t}(\rho_t(f_t-H)),
 \tag{MB.25}
\]

which need not vanish separately. Their exact sum is zero by (MB.23). Replacing those three numbers, or their coefficient integrands, by separate absolute majorants destroys that cancellation.

For a joint finite chronology the same identity may be applied at each original conditional node. A triangular gauge change
\(z_i=T_i(t,z_{>i})y_i\)
has unit Jacobian when each diagonal block is a real adjoint map: its determinant is the product of the diagonal determinants, each equal to one. Its infinitesimal diagonal divergence is zero because T_i is independent of its own z_i. The off-diagonal derivatives in later variables are still present in the velocity and in the transformed tests. All earlier kernels and Q references must be pulled back at the same time. This is an exact finite-dimensional transport identity; it is not a support estimate for a globally selected gauge. If a gauge depends on the same coordinate it transforms, its nontrivial Jacobian and divergence remain in (MB.20)–(MB.22).

## 5. What Gaussian and colour cancellation actually give before absolute values

At a flat Gaussian node put \(\rho(z)=\exp(-z^{\mathsf T}Kz/2)\), with the actual inherited positive precision K and the same determinant normalization. For \(w(z)=Az\), \(A^{\mathsf T}=-A\),

\[
 \delta_\rho w=\frac12z^{\mathsf T}[A,K]z,
 \qquad [A,K]=AK-KA.
 \tag{MB.26}
\]

This commutator is symmetric. The pure-gauge score is its negative. No trace determinant term has been lost: \(\operatorname{Tr}(K^{-1}[A,K])=0\), and the adjoint Jacobian is one. On an invariant fixed P domain, \(\mathcal F_w=0\); on a moving Q domain it is the retained Q boundary current in (MB.25).

For an untruncated Gaussian and a quadratic test \(f=z^{\mathsf T}Lz/2\), \(C=K^{-1}\), Wick contraction gives

\[
 \mathbb E[w\cdot\nabla f]
       =-\frac12\operatorname{Tr}(A[L,C]),\qquad
 \operatorname{Cov}(f,\delta_\rho w)
       =\frac12\operatorname{Tr}(A[L,C]).
 \tag{MB.27}
\]

This is an exact calculation with the complete inherited Gaussian, not a replacement by a bare Maxwell covariance.

At flat background \(K=K_{\rm sp}\otimes I_{\rm colour}\), and the quadratic part of a gauge-invariant scalar has \(L=L_{\rm sp}\otimes I_{\rm colour}\). A local gauge generator is block diagonal with colour blocks \(\operatorname{ad}\xi_x\), each traceless. Each trace in (MB.27) is then zero separately. The cross-energy integrand in Proposition MB.3 can nevertheless be nonzero pointwise; its first antisymmetric colour response averages to zero.

There is a version that does not require an untruncated Gaussian. Suppose the full real node at its flat external data, its domain, and its scalar test are invariant under simultaneous constant colour conjugation. For a fixed spatial gauge-generator profile, each of the three expressions in (MB.25) is a linear functional of its Lie-algebra generator values. Conjugating all integration variables shows that this functional is invariant under their simultaneous adjoint conjugation. On the simple Lie algebra there is no invariant linear functional; varying one generator value at a time shows that each such first integrated response is zero. This argument includes the domain functional, when its full flat references are retained. It does not say that the absolute integrals of those responses are zero.

Thus the useful order of operations is to form the actual complete owned coefficient integral, keep its determinant and inverse together, and use its permitted colour or divergence identity before taking its absolute coefficient bound. A quantitative bound away from flat data still requires the physical source tube and labelled mixed derivatives. OP's independent-copy parity calculation is one such fixed-depth statement; the pointwise obstruction above does not contradict it. A total Ward identity alone does not assign its cancellation to every old label.

## 6. The exact resolvent question after the latent terms are retained

The source's direct critical-chain maps have a semigroup derivative because the underlying critical-orbit nesting is an identity. On a common quotient tangent frame denote these coherent linear lifts by \(H_{i,r}\), with

\[
 H_{i,r}H_{r,s}=H_{i,s},\qquad
 \|H_{i,r}\|\le C_HL^{-(r-i)}.
 \tag{MB.28}
\]

At a general finite chronological path, linearize its **actual** fixed-target reconstructions, retaining the chosen latent velocities. In any already specified common tangent identifications this has the algebraic form

\[
 h_i=L_i h_{i+1}+M_i\dot z_i.
 \tag{MB.29}
\]

Here L_i is the actual target derivative, M_i the actual independent-coordinate derivative. Equation (MB.11) identifies the extra forcing if a gauge component is removed while the raw z_i is fixed. It must either remain in (MB.29) or be transferred by (MB.22); it cannot be set to zero by quotient notation.

Let \(E_i=L_i-H_{i,i+1}\). A finite telescoping substitution gives the exact Duhamel identity

\[
 h_i=H_{i,k}h_k+
    \sum_{r=i}^{k-1}H_{i,r}
                  \{E_rh_{r+1}+M_r\dot z_r\}.
 \tag{MB.30}
\]

For \(0<\alpha<1\), define \(\|h\|_{\alpha,k}=
\sup_{i\le k}L^{\alpha(k-i)}\|h_i\|\). The exact sufficient resolvent estimate for the homogeneous response is

\[
 q_\alpha:=\sup_i\sum_{r\ge i}
       L^{\alpha(r+1-i)}\|H_{i,r}E_r\|<1.
 \tag{MB.31}
\]

Indeed the right-hand sum acting on h has operator norm at most q_alpha in this weighted space. The finite triangular Neumann series and (MB.28) then give

\[
 \|h\|_{\alpha,k}
   \le\frac{C_H\|h_k\|+
       \sup_i L^{\alpha(k-i)}
        \|\sum_{r\ge i}H_{i,r}M_r\dot z_r\|}
              {1-q_\alpha}.
 \tag{MB.32}
\]

If, on an actual common family, \(\|E_r\|\le e_*\) were known uniformly, (MB.28) would bound

\[
 q_\alpha\le
      \frac{C_He_*L^\alpha}{1-L^{-(1-\alpha)}}.
 \tag{MB.33}
\]

This explains how a strictly smaller age exponent could absorb small errors without a product of one-step constants. It also displays the two genuine remaining requirements. First, the target/innovation/gauge identifications used in L_i and E_i must exist on the **same** raw, component-compatible, core-preserving outside family, including the saved targets and Q references. Separate native estimates at different stationary fields are not that statement. Second, the explicit forcing in (MB.11) and the labelled divergence/boundary terms in (MB.22) need their own common integral estimates. Proposition MB.3 proves that they cannot be bounded by deleting them from a pointwise fixed-innovation inequality.

Equations (MB.30)–(MB.33) are an exact algebraic resolvent target and its proof, not a claim that its model-specific common-family hypothesis has been established. The new proved source information in this note is the direct moving-reference estimate (MB.5)–(MB.8), the actual fixed-innovation response (MB.12), and the complete normalized current identity (MB.22), with its separate origins and Q boundary.

Primary inputs: CMP102, Section G, (174)–(190), especially the explicit external-reference analyticity on pp.308–309; the exact nonlinear averaging and fixed-target covariance in CMP98/CMP109; CMP119's block-constant covariance of the full Q references; the real critical nesting VN/AP; BG's exact small-residual/block-constant factorization; AF's Q-null tangential cross-cochains; and the existing first-Q-current convention DP/QS/NC/TS. EC supplies the complete scalar gauge-orbit identity used only at its stated integrated scope.
