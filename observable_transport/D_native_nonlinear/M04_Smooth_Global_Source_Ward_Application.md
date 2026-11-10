# An actual smooth global-source Hessian for the quadratic Ward projector

This note establishes the two prerequisites left explicit in EJ and WQ for one particular actual marked object: the spatially summed microscopic Wilson scalar transported through the three homogeneous auxiliary operations. It constructs its infinite-lattice quadratic response and applies WQ there. The operation is the first P / second auxiliary P / third auxiliary P operation of AD, TC and TR. Every running coupling, minimizing map, gauge kernel and cutoff is specified at zero microscopic source. There are no sharp Q-domain corrections in this statement.

The proof does not identify a local-source momentum projector, a nonlinear irrelevant remainder, a uniform-depth estimate, or an exact periodization of the finite-torus answer.

## 1. The exact constant source and its normalization

Use the F01/SE scalar and the conventions of TR:
\[
 F_x(U)=\alpha\beta_0\sigma_{h_0}(x;U)-c,\qquad
 \beta_0=(Ng_0^2)^{-1},\qquad
 b=|\alpha|+h_0^4|c|.
\]
The exact plaquette multiplicity identity is
\[
 S_0(U):=h_0^4\sum_xF_x(U)
   =\frac{2\alpha\beta_0}{\sqrt6}\sum_p s(U_p)
      -c h_0^4|\Lambda_0|,
 \qquad s(U)=N-\operatorname{Re}\operatorname{Tr}U.
 \tag{SW.1}
\]
Thus inserting \(\exp(\tau S_0)\) into the original Wilson density changes its Wilson coefficient to
\[
 -\beta_0\sum_ps(U_p)+\tau S_0(U)
   =-\theta(\tau)\beta_0\sum_ps(U_p)
       -\tau c h_0^4|\Lambda_0|,
 \qquad
 \theta(\tau)=1-\frac{2\alpha}{\sqrt6}\tau .
 \tag{SW.2}
\]
All source-free gauge, Haar and coarea factors remain unchanged.

Let \(\mathcal T_i^{P_i}\) denote the exact unnormalized auxiliary integration at layer \(i\), with the original constant gauge normalizations and the fixed source-free coordinate maps. Here \(P_0=P\), \(P_1=P_{\mathrm{aux},2}\), and \(P_2=P_{\mathrm{aux},3}\); these are not the later printed R-good radii. Define
\[
 \rho_{\Lambda,3}^{\tau}
   =\mathcal T_2^{P_2}\mathcal T_1^{P_1}
       \mathcal T_0^{P_0}
          \bigl(e^{\tau S_0}\rho_{\Lambda,0}\bigr).
 \tag{SW.3}
\]
The maps \(\mathcal T_i^{P_i}\) do not change with \(\tau\). In particular no derivative of a running coupling, selector, gauge choice or saddle is being taken.

At \(\tau=0\), exact conditional disintegration of these three positive integrations gives
\[
 \frac{\rho_{\Lambda,3}^{\tau}(W)}
      {\rho_{\Lambda,3}^{0}(W)}
  =\mathbb E_{\Lambda,W}^{\,aaa}e^{\tau S_0},
 \qquad
 \left.\partial_\tau\log\rho_{\Lambda,3}^{\tau}(W)\right|_0
   =h_0^4\sum_x(\mathcal T^{\,aaa}F_x)(W).
 \tag{SW.4}
\]
The expectation is the same normalized three-layer law used for TR's smooth baseline. All inherited masses and all three conditional denominators occur once. One may verify (SW.4) directly by multiplying the three conditional-density quotients: the successive intermediate masses cancel in the joint integral, leaving precisely (SW.3). If an effective-action convention subtracts a source-dependent vacuum constant, that constant must be restored in (SW.4); it has no effect on the field Hessian below.

The constant source is therefore an actual placement of the block-summed marked observable in the unnormalized analytic action family. It is not a derivative of an adaptively retuned renormalization scheme.

## 2. Exact symmetries of this auxiliary operation

### 2.1 The averaging convention matters

CMP109, printed pp.252--254, explicitly notes that the earlier averaging prescription was not lattice-Euclidean symmetric. Its replacement uses the full family \(G(y,x)\) of shortest coordinate-permutation paths, (0.4), and the permutation-symmetric group mean, (0.5)--(0.11). The averaged axial sampler uses that same family. The present argument uses this later prescription, which is the one used in the homogeneous effective-action construction.

Under a signed permutation or a translation preserving the next coarse lattice, \(G(y,x)\) maps bijectively to the corresponding transformed family. Endpoint gauge covariance and permutation invariance of the group mean then give the exact covariance of both the nonlinear coarse average and the averaged gauge sampler. The blocks are centered blocks with odd \(L\); the full symmetry group of the final coarse lattice preserves every intervening nested lattice.

### 2.2 The exceptional free-coordinate convention also transforms exactly

CMP109 p.267, immediately after (2.10), defines \(b_0(c)\) as the fine bond that is both contained in the straight coarse bond \(c\) and belongs to the crossing corridor \(B(c)\). It is the central crossing bond, with its induced orientation. Consequently
\[
 r b_0(c)=b_0(rc),\qquad b_0(-c)=-b_0(c).
 \tag{SW.5}
\]
The exceptional set and its free complement are therefore preserved by every such lattice symmetry. This would not follow for an arbitrary chosen crossing bond.

The source's negative-orientation rule (2.18), p.269, is a background adjoint transformation followed by inverse/orientation reversal. On the free Lie coordinates it is a signed pointwise orthogonal map. The constraint-linearizing correction changes only exceptional bonds, and its defining equation has a unique local solution. Equivariance of that equation thus gives equivariance of the nonlinear correction and of the linear embedding \(C\); the independent free coordinates retain the stated signed-adjoint transformation. Its Jacobian has absolute value one.

It follows that every product domain
\[
 \prod_{e\ {\rm free}}\{|z_e|<P_i\},
 \tag{SW.6}
\]
with a constant radius at its layer and an adjoint-invariant norm, is preserved exactly. Changing the source's auxiliary radius to the fixed small fraction used in AD/TC does not alter this argument. The fixed real caps used to continue coefficient inputs equal the identity on (SW.6), so their off-support convention is irrelevant to this exact physical identity. They need not be declared holomorphic.

CMP109 (2.16)--(2.18) proves this invariance for the complete transformed integral, including its measure. The argument retains the Haar/coarea factors, the soft sampler and all Gaussian normalizers. A gauge change of the retained coarse field acts by the corresponding block-constant lift on each preceding field and by an orthogonal adjoint map on its free variables. Gauge fixing is therefore not being ignored.

### Lemma SW.1 — physical symmetry

For the exact operation (SW.3), at every admitted real coarse field and every real \(\tau\) in a neighborhood of zero,
\[
 \rho_{\Lambda,3}^{\tau}(W^v)=\rho_{\Lambda,3}^{\tau}(W),
 \qquad
 \rho_{\Lambda,3}^{\tau}(rW)=\rho_{\Lambda,3}^{\tau}(W).
 \tag{SW.7}
\]
The source \(S_0\) is gauge invariant and is invariant under all these lattice symmetries by (SW.1). Applying the three measure-preserving changes of variables just described proves (SW.7). The same identities hold for their analytic continuations wherever both sides are in the fixed native tube.

If \(B_3(n)\) is a centered final block, define the dimensionless block readout
\[
 \Phi_{\Lambda,n}(W)
     =h_0^4\sum_{x\in B_3(n)}(\mathcal T^{\,aaa}F_x)(W).
 \tag{SW.8}
\]
Then \(\Phi_{\Lambda,n}(W^v)=\Phi_{\Lambda,n}(W)\), and
\(\Phi_{\Lambda,rn}(rW)=\Phi_{\Lambda,n}(W)\). The summed readout
\(\sum_n\Phi_{\Lambda,n}\) is exactly (SW.4).

## 3. A fixed source disc for the complete analytic action

One must not regard the extensive term \(\tau g_0^{-2}A(U)\) as a uniformly bounded small Mayer vertex. Instead keep \(\theta\) in each actual classical quadratic form.

The minimizing Wilson orbit is unchanged by multiplication of its action by a positive constant. Its critical constraint cancellations are multiplied by the same constant. Thus the fixed zero-source minimizing maps are the actual classical minimizing maps for real \(\theta\) near one. Analytic continuation in \(\theta\) then uses those same maps.

At every one of the three layers the complete classical constrained quadratic form, including its constraint-force correction, is multiplied by \(\theta\). The actual soft-gauge coefficient is unchanged. In the notation of TC, a factor such as \(\lambda_2=(g_2/g_1)^2\) stays in place:
\[
 K_i^\theta=\theta K_{i,\mathrm{cl}}+K_{i,\mathrm{gf}},
 \qquad
 \|K_i^\theta-K_i^1\|_\rho
       \le C_L|\theta-1|.
 \tag{SW.9}
\]
Here \(K_{i,\mathrm{cl}}\) denotes the complete classical part in the chosen fixed-depth normalization, not a bare first-step Laplacian. Any fixed running-coupling counterterm introduced by the chosen split is retained in the analytic inherited interaction; the identity of the original density (SW.3) is unchanged.

The source gaps, finite three-level coupling ratios and complete native analytic row bounds used in BA/TC imply that a fixed disc
\[
 |\theta-1|<\delta_*,\qquad \delta_*>0,
 \tag{SW.10}
\]
preserves the relative Gaussian reserves and the source fixed-point tubes. \(\delta_*\) is independent of volume and of the microscopic cutoff along the admitted weak-coupling regime, but may depend on fixed \(L\), the three levels and the chosen buffers. The normalized covariance and its inverse/determinant must be constructed from the same \(K_i^\theta\). All resulting source-dependent Gaussian determinant factors remain in the action.

For example, if the fixed zero-source split is \(g_1^{-2}=g_0^{-2}-\beta_1\), then
\[
 -\theta g_0^{-2}A
      =-\theta g_1^{-2}A-\theta\beta_1 A .
 \tag{SW.10a}
\]
Keep the first term as the next classical action and the second, with its displayed sign, in the inherited \(E^\theta\). The source's bounded coefficient \(\beta_1\) is specified; its extra normalized fluctuation quadratic is of order \(g_1^2\beta_1\), and the same finite-depth bookkeeping applies at the next split. No \(g_1(\tau)\), retuned beta function, or derivative of a running map is introduced. This makes (SW.9) exact in the chosen renormalized splitting without dropping the source-dependent counterterm.

For completeness, the strict estimates permit this extra parameter before any infinite-volume argument. The classical higher terms are multiplied by a uniformly bounded \(\theta\); their small fluctuation budgets remain \(C_L(g_iP_i^3+g_i^2P_i^4+\cdots)\). The Haar/coarea terms are unchanged. At the next layer the already integrated terms are holomorphic in the same source disc and native field tube. Their localized Cauchy bounds and substitution estimates therefore run with \(\theta\) included as an external parameter. Conditional old Gaussian integrations retain the uniformity in the later real coordinates used in TC. No additional later quadratic store is incurred for each copied old factor.

If the complex comparison of \(K_i^\theta\) contributes \(\exp(C|\theta-1|r)\), use the fixed-buffer rank bound for each primitive marginal, before its cluster sum. Choose \(\delta_*\) so that this rate cost fits the strict ordinary-carrier margin; then choose the original coupling small enough for the fluctuation activities. This is a fixed-disc choice, not a division by the probability of a whole auxiliary event. There is no growing Q core in this all-auxiliary construction.

These observations replay the actual fixed-depth analytic-base argument of TC on (SW.10). They prove a common complete coefficient family for \(\log\rho_{\Lambda,3}^{\tau}\), after its explicit classical and field-independent factors are included. Normalized raw derivatives of fixed finite order and the source derivative can be taken termwise with a remaining carrier-rate margin. For \(\alpha=0\) the field-dependent source response is zero. Otherwise source Cauchy on (SW.10) costs a fixed multiple of \(|\alpha|\).

## 4. Cross-volume compatibility: local coefficients and winding terms

The conclusion here is stronger than a numerical decay estimate on each torus, but weaker than exact periodization.

Choose one stencil registry on the infinite nested lattice: the literal averaging and exceptional-bond rules, the local reference paths and partitions, the finite local matrix solves, the local fixed-point branches, and the ordering/grouping of the convergent series. On a sufficiently large periodic quotient, use its periodic images. Periods are chosen compatible with the finitely many fixed localization meshes; the source tori have arbitrarily large such periods.

This is a choice of representation of the same actual auxiliary integral. It does not change its density or its cutoff. The existing physical localizations can be replayed with this choice for the following explicit reasons.

* Every bare action, averaging, gauge-sampler, Haar and exceptional-coarea factor is a finite-stencil analytic function. Its definition on an embedded footprint is identical in the infinite lattice and every containing quotient.
* The BR reference uses bounded paths, finite local matrices and fixed geometric weights. Its restriction on an embedded full footprint has the same formula in every quotient. Global topology is not used to select those local data.
* For each propagator, use the PR local-parametrix expansion. Its principal inverse is the inverse of a finite local matrix. For an exponentially localized input, first truncate its *complete primitive carriers* as in PR.2; then expand the remaining tail by the common resolvent identity. Thus a local inverse does not conceal ambient-dependent matrix entries. Products, the all-\(t\) Stieltjes integral and finite marginal inverse/determinant branches inherit the same local identity.
* The source nonlinear fixed point and its CMP116 decoupling are expansions in those same local analytic functions and propagators. CMP116 (1.9)--(1.10), printed pp.4--5, explicitly reduces a surviving term to the component containing its root, with the propagators and input fields restricted to that component. At fixed depth their raw substitutions retain all determining-data carriers. Uniqueness of the local analytic branches fixes the same coefficients on an embedded component.
* The fixed P-domain integrals, Mayer products, connected logarithms, and CN same-gas exclusions use only the resulting finite-component integrands. Repeated latent copies remain distinct. Their integrals and their own normalizers are identical when their complete tagged footprints are identified. A discarded global conditional denominator is not used in this step.

In these statements a tag's **complete footprint** includes every local-solve halo, every propagator word footprint, every raw substitution footprint, its integrated coordinate list, and every connector in the logarithm. It is not merely the union of the visible mark anchors. Where a fixed partition is not invariant under a one-site translation or a reflection, average the coefficient representation over its finitely many mesh phases and signed-permutation images. Every representation sums to the same physical function. The average preserves the bounds and cross-volume identities and makes the registry covariant. This finite averaging is not a modification of the auxiliary kernel.

### Lemma SW.2 — embedded coefficient identity and winding tail

There is an expansion of the actual source-dependent, field-dependent action and of its source/field derivatives, on the disc (SW.10), with these properties:

1. A complete connected tag whose footprint has an injective lift to the infinite lattice has the same finite-dimensional formula in every quotient realizing that lift.
2. The absolute tagged estimates have one fixed positive rate after the fixed number of source/field Cauchy derivatives.
3. If a tag cannot be compared on two quotients by such an embedded lift, its full footprint has diameter at least a fixed multiple of the smaller quotient's side, measured in final coarse units.

**Proof.** The preceding list is an induction on the actual local algebraic construction. Finite matrix inverses use the same entries and branch; convergent fixed-point coefficients use the same local equations; integration domains and normalized marginal densities agree; and every product or connected cluster retains the union of the input footprints. These operations preserve the embedded identity. A winding propagator word or cluster cannot be supported in a simply embedded set. Conversely all operations on a simply embedded complete footprint are literally the same finite operations. The strict absolute majorants are those of the fixed-depth construction, uniformly on (SW.10). A connected footprint with a winding obstruction must traverse a period, so its size is at least \(c\ell_\Lambda\). Exponential summation bounds its anchored contribution by \(C e^{-c'\ell_\Lambda}\), with fixed polynomial incidence and derivative counts paid by spare rate. \(\square\)

CMP109 p.264 explicitly takes the infinite-lattice polarization limit using its localized representation (1.7); pp.292--293, (5.1)--(5.11), explain the ensuing analytic Fourier symbol. Lemma SW.2 verifies the additional common-registry step for the present constant-source derivative instead of inferring it from a separate finite-volume bound.

There can be extra winding products. For example, squaring a periodized Gaussian covariance creates cross terms with different winding numbers. They are among the large-footprint terms in Lemma SW.2. Thus no exact identity between the finite-torus answer and the periodization of its infinite-lattice limit is asserted.

## 5. The actual infinite-lattice marked Hessian

Write the final raw link near identity as
\[
 W_\mu(n;a)=\exp\!\left(g_3\sum_Aa_\mu^A(n)T_A\right).
\]
On a finite torus define
\[
 K_{\Lambda;\mu\nu}^{AB}(n,m)
   =\left.
      \partial_{a_\mu^A(n)}\partial_{a_\nu^B(m)}
      \partial_\tau\log\rho_{\Lambda,3}^{\tau}(W(a))
     \right|_{\tau=0,a=0}.
 \tag{SW.11}
\]
This is the Hessian of the **actual spatial sum** in (SW.4), in the same normalized raw angular coordinates used by EJ. All retained-background source terms are included.

Source Cauchy and two raw Cauchy derivatives, followed by Lemma SW.2, give an infinite-lattice kernel \(K_\infty\) and an exponential edge-centered norm
\[
 \|K_\infty\|_\rho\le C_L L^{12}b
 \tag{SW.12}
\]
for some \(\rho>0\). One can also obtain this budget directly from EJ.3: sum the microscopic root over one final block, use the same actual source-linear family, and sum the translated root carriers that contain the two differentiated edges. Their incidence and second spatial moments cost only a fixed polynomial in the complete carrier size. This proves absolute convergence of the sum over source positions; it does not require a finite total volume.

The embedded identity and winding estimate imply, for any smaller \(\rho'>0\),
\[
 \left\|K_\Lambda-\operatorname{Per}_\Lambda K_\infty
       \right\|_{\rho',\Lambda}
       \le C_L L^{12}b\,e^{-c\ell_\Lambda}.
 \tag{SW.13}
\]
Here the finite-torus norm uses shortest edge-centered distance, and constants may change when passing to the smaller exponential rate. Terms of the periodized infinite kernel whose lifted footprint reaches around a period are also placed in the tail when proving (SW.13). This is an estimate on the difference, not equality of the two kernels.

By Lemma SW.1 and passage to the local limit, \(K_\infty\) is translation invariant, real and self-adjoint, covariant under all signed permutations in the oriented edge convention, and colour-scalar. The first field derivative at the identity is zero: global \(SU(N)\) invariance leaves no nonzero invariant linear adjoint vector. Differentiating the exact retained gauge invariance then gives
\[
 K_\infty d=0 .
 \tag{SW.14}
\]
No assertion of a Ward identity at arbitrarily interpolated finite-torus momenta is needed.

### Theorem SW.3 — WQ applies to the smooth integrated marked response

The actual \(K_\infty\) in (SW.11)--(SW.14) satisfies WQ's hypotheses. With the edge-centered symbol and \(\widehat p_\mu=2\sin(p_\mu/2)\), there is one bounded real coefficient \(c_{\mathrm{mark}}\) such that
\[
 \mathscr K_\infty(p)=c_{\mathrm{mark}}K_W(p)+\mathscr R(p),
 \qquad
 K_W(p)=|\widehat p|^2 I-\widehat p\,\widehat p^{\,T},
 \tag{SW.15}
\]
\[
 \mathscr R(p)\widehat p=0,\qquad
 |\langle v,\mathscr R(p)v\rangle|
   \le C_L L^{12}b\,|p|^2\langle v,K_W(p)v\rangle
 \tag{SW.16}
\]
for sufficiently small real \(p\). In particular, for fields with Fourier support in \(|p|\le h_3/H\),
\[
 |Q_{\mathscr R}(A)|
     \le C_L L^{12}b\,(h_3/H)^2 Q_{K_W}(A).
 \tag{SW.17}
\]
The coefficient is the zero-momentum quadratic Ward coefficient, not the finite-pulse coefficient.

The finite torus has the additional winding Hessian (SW.13). An absolute bound on that term is not automatically a bound relative to Wilson energy on a torus holonomy mode, where the latter vanishes. The theorem therefore applies WQ directly to \(K_\infty\); it keeps this finite-volume distinction explicit.

## 6. Scope and remaining renormalization task

The result is an actual smooth **spatially summed**, fixed-three-layer marked Hessian. The constant source is inserted in the original Wilson density, its classical coefficient is resummed, the literal auxiliary domains are unchanged, and the infinite-lattice coefficients are obtained from the same actual local construction.

It does not provide the separate source-position momentum estimates needed for a local marked density; higher nonlinear Ward matching; a sharp arbitrary-field conditional rescaling estimate; a microscopic M03 remainder contraction; higher derivatives of the hard Q corrections; or an interacting uniform-depth theorem. The constants in (SW.12)--(SW.17) retain the fixed-depth \(C_L\) dependence and the exposed engineering normalization. The result fills the two stated prerequisites for this integrated quadratic application of WQ, while leaving those distinct later tasks open.

Primary sources used directly: CMP109 pp.252--255, (0.4)--(0.16); pp.263--264, (1.19)--(1.22); pp.267--269, the definition of \(b_0(c)\) and (2.16)--(2.18); pp.292--293, (5.1)--(5.11); CMP116 pp.3--7, component restriction (1.9)--(1.10), and its normalized Gaussian/Mayer construction. Fixed-depth analytic/marked inputs: PR, BR, AD, TC, TR, EJ; the same-gas normalization identities of CN; and the WQ theorem.
