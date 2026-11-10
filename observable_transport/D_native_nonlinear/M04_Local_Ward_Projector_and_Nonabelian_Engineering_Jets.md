# Local Ward matching and the non-Abelian engineering jets of the actual smooth mark

This note constructs the local, source-position-dependent version of the quadratic extraction in WQ and applies it to the actual three-layer smooth microscopic Wilson insertion. The local Hessian has two independent field momenta, so its Ward identity is stronger than the identity for the spatially integrated insertion. Its unique marginal coefficient is an explicit moment measured from the source anchor. Subtracting the full local Wilson function with that coefficient gives an exactly gauge-invariant nonlinear remainder. Its smooth-background engineering expansion begins at degree six, including the non-Abelian vertices, rather than only its integrated quadratic expansion having a fourth-order momentum zero.

The object is the first P / second auxiliary P / third auxiliary P mark of SW and PJ, with all maps, couplings, cutoff conventions and conditional normalizers specified at zero microscopic source. A full hard-Q density, a uniform-depth induction, and an irrelevant-field contraction on arbitrary native fields are not inferred from this local finite-jet result. Those require additional estimates.

## 1. The local marked object and its supported limit

Use the actual source of F01, SE and PJ:

\[
 F_x=\alpha\beta_0\sigma_{h_0}(x)-c_0,
 \qquad \beta_0=(Ng_0^2)^{-1},
 \qquad
 \Phi_{\Lambda,n}(W)
   =h_0^4\sum_{x\in B_3(n)}
          (\mathcal T^{aaa}F_x)(W).
 \tag{NW.1}
\]

Here the final block is the literal centered block of SW.8, containing \(L^{12}\) microscopic sites. The block factor is retained throughout. The identity insertion transports exactly. It can be removed by replacing \(\Phi_{\Lambda,n}\) with

\[
 \Phi_{\Lambda,n}^{\alpha}
     =\Phi_{\Lambda,n}+c_0h_0^4|B_3(n)|.
 \tag{NW.2}
\]

This replacement does not change any field derivative or any difference from its flat value. The three integrations are the actual normalized fixed-domain auxiliary integrations, including their complete precision, soft gauge, Haar/coarea factors and inherited interactions. The source is inserted before them, and no retained-background part of the microscopic source is discarded.

The input from PJ.1–PJ.2 is the supported analytic continuation

\[
 \Phi^{\alpha}_{\Lambda,n}(e^B)
      =\sum_{X\ni n}f_{\Lambda,n,X}(B_X),
 \qquad
 \sup_n\sum_{X\ni n}e^{\kappa_0 n(X)}
       \sup_{\|B_X\|_\infty<2r_0}|f_{\Lambda,n,X}(B_X)|
       \le \mathfrak B,
 \tag{NW.3}
\]

where

\[
 \mathfrak B=C_L L^{12}|\alpha|g_0^{-2}.
 \tag{NW.4}
\]

The physical radius \(r_0>0\) and positive carrier rate are independent of volume and microscopic cutoff at these three fixed levels. Constants may depend on the fixed block size, meshes, buffers, group and bounded adjacent coupling ratios. The source radii have their actual polylogarithmic growth, in particular \(g_iP_i^3\to0\). This is stronger than \(g_iP_i\to0\), which would not suffice for the bounded fluctuation vertices in PJ.

Every X in (NW.3) contains the source block root and the complete determining footprint, including local inverse halos, propagator words, substitutions, integrated coordinate lists and normalization connectors. It is not just a list of visible source positions. The explicit retained selectors have been factored out on the admitted domain. Equation (NW.3) continues their smooth coefficient family; it does not continue a sharp characteristic function.

### Lemma NW.1 — the actual local infinite-volume mark

Choose the common infinite nested-lattice registry of SW.2. There is a compatible anchored infinite-lattice family \(\Phi_n\) with (NW.3), its fixed-order field jets, and the physical symmetries

\[
 \Phi_n(W^u)=\Phi_n(W),\qquad
 \Phi_{Rn}(RW)=\Phi_n(W),
 \tag{NW.5}
\]

for real retained gauges and the full rooted hypercubic group. It is translation covariant on the final lattice. For a finite torus of shortest final-lattice period \(\ell\), its local coefficient comparison with this family has a winding remainder bounded, after any fixed q normalized derivatives and fixed carrier moments, by

\[
 C_{L,q,s}\mathfrak B g_3^q e^{-c\ell}.
 \tag{NW.6}
\]

This is a comparison estimate, not an exact periodization identity.

**Proof.** Insert a source for the one finite microscopic block in (NW.1) before the three conditional operations. Its inverse-beta source circle has radius \(c g_0^2/(L^{12}|\alpha|)\), as in PJ.1(d). The same-gas normalization returns its first derivative once. No whole-volume source is treated as a small bounded vertex, and no running parameter is differentiated.

The complete embedded-coefficient argument of SW.2 now applies with this one source root: the primitive insertion is a finite-stencil function; all zero-source references, local inverses, fixed-point branches, integrals and denominators are the same source-free ones. Each term with an injectively lifted complete footprint has the same finite formula on every containing quotient. A term for which this comparison fails traverses a period and has size at least \(c\ell\). The positive exponential rate in (NW.3), with a strict reduction for the desired Cauchy derivatives and incidence polynomials, gives (NW.6).

The normally convergent embedded family defines the infinite-lattice mark and all the stated jets. The exact local symmetries are already the identities SW.8 for the physical scalar. Finite averaging of the coefficient representation over the fixed mesh phases and signed permutations gives a common covariant registry without changing that scalar. Passing to the local limit gives (NW.5). The same argument gives translation covariance. No ambient-volume vacuum constant is used to define this anchored observable. \(\square\)

The local source in this proof is distinct from SW's constant extensive source. Its inverse-beta source radius suffices for a bounded block insertion. SW's resummation of the extensive classical Wilson coefficient remains necessary for its larger constant-source disc; it is not being replaced by the local argument.

## 2. The two-momentum Hessian and its exact Ward identities

Set final spacing to one for the Fourier discussion. Write

\[
 W_e(a)=\exp(g_3a_e),\qquad
 \langle X,Y\rangle=-\operatorname{Tr}(XY),
 \tag{NW.7}
\]

on \(\mathfrak{su}(N)\), with the corresponding orthonormal colour basis. Positive edges are \((r,\mu)\), centered at
\(x_{r\mu}=r+e_\mu/2\). Negative orientations are inverse links.

Let \(K_{r\mu,s\nu}^{AB}\) be the Hessian of \(\Phi_0(e^{g_3a})\) at \(a=0\). Global colour conjugation makes it a scalar in colour:

\[
 K_{r\mu,s\nu}^{AB}=\delta^{AB}k_{r\mu,s\nu}.
 \tag{NW.8}
\]

Indeed a commuting endomorphism of the complexified adjoint representation of the simple Lie algebra is scalar; the same argument makes the first field derivative zero. Thus this Hessian is independent of the local coordinate choice to second order. Hessian symmetry gives
\(k_{r\mu,s\nu}=k_{s\nu,r\mu}\).

For some \(\rho>0\), (NW.3) and physical Cauchy estimates imply

\[
 M_\rho
  :=\sum_{\mu,\nu,r,s}
       e^{\rho(|x_{r\mu}|_1+|x_{s\nu}|_1)}
                  |k_{r\mu,s\nu}|
       \le C_L\mathfrak B g_3^2.
 \tag{NW.9}
\]

To see the exponential moment, both differentiated edges are within the complete anchored carrier. Their distances from the root are at most a fixed multiple of its size. Choose \(\rho\) below the corresponding unused carrier rate. The two-coordinate Cauchy bound contributes \(g_3^2\); the number of possible coordinate pairs is a fixed carrier-size polynomial, paid by another strict rate reduction. This is stronger than merely quoting finitely many numerical moments.

Define the local Fourier Hessian with independent momenta:

\[
 V_{\mu\nu}(p,q)
   =\sum_{r,s}
       e^{-ip\cdot x_{r\mu}-iq\cdot x_{s\nu}}
                         k_{r\mu,s\nu},
 \qquad \widehat p_\mu=2\sin(p_\mu/2).
 \tag{NW.10}
\]

It is analytic in a fixed complex strip in both momenta. The momentum \(p+q\) is the source momentum. Restricting immediately to \(q=-p\) would discard this information.

### Lemma NW.2 — local double Ward identity

For all real momenta,

\[
 \widehat p^{\mathsf T}V(p,q)=0,
 \qquad V(p,q)\widehat q=0.
 \tag{NW.11}
\]

Moreover,

\[
 V(0,q)=V(p,0)=0,
 \qquad V(Rp,Rq)=R V(p,q)R^{\mathsf T},
 \qquad V(-p,-q)=V(p,q).
 \tag{NW.12}
\]

**Proof.** Differentiate the exact local identity \(\Phi_0(W^u)=\Phi_0(W)\) once in an arbitrary field direction and once in a site-gauge direction at identity. Terms involving the first derivative of \(\Phi_0\) vanish by global colour. The Hessian therefore annihilates every lattice gradient in either slot. Edge-centering makes the gradient multiplier \(i\widehat p\), with a harmless overall sign depending on the gauge convention, and proves (NW.11). This uses local gauge invariance of the insertion, not only gauge invariance after summing its anchors.

For fixed q set \(p=t e_j\) in the first identity and take \(t\to0\). Every row of \(V(0,q)\) is zero. Use the second identity in the same manner for \(V(p,0)\). The rooted lattice symmetries in (NW.5), with oriented edge centers, give the covariance identity in (NW.12). Its case \(R=-I\) gives the last identity. Absolute convergence justifies every differentiation and Fourier operation. \(\square\)

## 3. A local Wilson projector, including nonzero source momentum

### Theorem NW.3 — the unique marginal local tensor

There is a real scalar \(c_\Phi\), for real microscopic source, such that the total-degree-two Taylor term is

\[
 V_{2,\mu\nu}(p,q)
   =c_\Phi\{q_\mu p_\nu-(p\cdot q)\delta_{\mu\nu}\}.
 \tag{NW.13}
\]

For any \(\mu\ne\nu\),

\[
 c_\Phi
   =-\partial_{p_\nu}\partial_{q_\nu}V_{\mu\mu}(0,0)
   =\sum_{r,s}r_\nu s_\nu k_{r\mu,s\mu},
 \qquad
 |c_\Phi|\le C_\rho M_\rho.
 \tag{NW.14}
\]

The scalar is the same coefficient extracted by SW/WQ from the integrated mark; it is not a second matching prescription.

**Proof.** By (NW.12) every nonzero term has positive degree in each momentum, and inversion removes odd total degrees. A hypercubic-covariant tensor bilinear in p and q has the form

\[
 A(p\cdot q)\delta_{\mu\nu}
  +B p_\mu q_\nu+C q_\mu p_\nu
  +D\delta_{\mu\nu}p_\mu q_\mu.
 \tag{NW.15}
\]

For completeness this list follows by reflecting each coordinate: a coefficient with indices \(\mu,\nu,\rho,\sigma\) can be nonzero only when every coordinate index appears an even number of times. Permutations identify the three pairings, and the case in which all four indices agree supplies the fourth displayed tensor. Full reflections exclude an epsilon tensor.

The lowest-order part of the first Ward identity is

\[
 (A+C)p_\nu(p\cdot q)+B|p|^2q_\nu+D p_\nu^2q_\nu=0.
 \tag{NW.16}
\]

Choose \(p_\nu=0\), then an independent q, to get \(B=0\). The terms with q in a coordinate distinct from \(\nu\) give \(A+C=0\); the remaining term gives \(D=0\). Set \(c_\Phi=C=-A\). The second Ward identity is then also satisfied. Formula (NW.14), including its sign, follows directly from (NW.10). Its bound is the anchored second moment in (NW.9).

By translation covariance, the Hessian of \(\sum_n\Phi_n\) has multiplier \(V(p,-p)\), with the same field normalization. Equation (NW.13) becomes
\(c_\Phi(|p|^2I-pp^{\mathsf T})\). Thus the WQ coefficient of that integrated Hessian equals \(c_\Phi\). Finite-volume comparison is understood as in (NW.6); exact periodization is unnecessary. \(\square\)

Introduce the **actual local Wilson function**

\[
 w_n(U)=\frac14\sum_{\mu<\nu}
     \sum_{\epsilon,\epsilon'=\pm1}
       \{N-\operatorname{Re}\operatorname{Tr}
                     P_{\epsilon e_\mu,\epsilon'e_\nu}(n;U)\}.
 \tag{NW.17}
\]

For analytic arguments use its holomorphic continuation
\(N-\tfrac12\operatorname{Tr}(P+P^{-1})\). On real links this equals (NW.17). Each unoriented plaquette is counted at its four vertices, so
\(\sum_nw_n=\sum_p s(U_p)\).

Let \(\mathscr W(p,q)\) be the local Hessian of
\(g_3^{-2}w_0(e^{g_3a})\). It has both exact Ward identities, has coefficient one in (NW.14), and obeys

\[
 \mathscr W(p,-p)=|\widehat p|^2I
                      -\widehat p\widehat p^{\mathsf T}.
 \tag{NW.18}
\]

Consequently

\[
 \Pi_{\rm loc}V=c_\Phi\mathscr W,
 \qquad R_2=V-c_\Phi\mathscr W
 \tag{NW.19}
\]

is a bounded linear idempotent local quadratic projector. It removes the degree-two tensor for every source momentum. Its remainder has zero Taylor coefficients of total degree at most three, and vanishes if either field momentum is zero.

### Corollary NW.4 — the joint local low-momentum gain

For real \(p,q\in[-\pi,\pi]^4\) and complex edge-polarization vectors u,v,

\[
 \boxed{
 |u^*R_2(p,q)v|
 \le C_\rho M_\rho (|p|+|q|)^2
          |\widehat p\wedge u|\,|\widehat q\wedge v|.
 }
 \tag{NW.20}
\]

Here \(|\widehat p\wedge u|^2=|\widehat p|^2|u|^2
-|\widehat p^{\mathsf T}u|^2\), and the bound extends continuously to either zero momentum. There is no Hermiticity assertion for the independent-momentum matrix \(R_2(p,q)\).

**Proof.** Since \(R_2(p,0)=R_2(0,q)=0\), integrate one derivative in each leg. The constant term of \(\partial_p\partial_qR_2\) has been subtracted, and its linear terms vanish by total inversion parity. A fourth-moment bound from (NW.9) gives

\[
 \|R_2(p,q)\|\le
       C_\rho M_\rho|p||q|(|p|+|q|)^2.
 \tag{NW.21}
\]

The straight segments used in these integral remainders stay in the real Brillouin cube, so the same derivative bound applies there. The exact two Ward identities give \(R_2=P_pR_2P_q\), where the real orthogonal projectors remove the directions \(\widehat p,\widehat q\). On this cube \(|p|\le(\pi/2)|\widehat p|\). Applying (NW.21) to the projected u and v proves (NW.20). \(\square\)

In particular low field momenta of order \(L^{-1}\) have an additional factor \(L^{-2}\) relative to the product of their two curvature amplitudes. This is a Fourier statement about the local quadratic kernel. Turning it into a block transfer estimate requires the actual transfer and its norms; neither a Fourier cutoff nor the flat Gaussian law is inserted into the nonlinear conditional law here.

## 4. The exact nonlinear Wilson subtraction and its physical normalization

Define

\[
 \mathscr R_n(U)
    =\Phi_n(U)-\Phi_n(I)-\frac{c_\Phi}{g_3^2}w_n(U).
 \tag{NW.22}
\]

Every term is a genuine gauge-invariant scalar. Thus (NW.22) is an exact nonlinear definition on the admitted native domain and its smooth coefficient continuation. It is not the subtraction of a raw quadratic polynomial. Its Hessian is exactly the local remainder in (NW.19). Also

\[
 h_3^4\beta_3\sigma_{h_3}(n)
       =\frac{2}{\sqrt6Ng_3^2}w_n(U).
 \tag{NW.23}
\]

Therefore the coefficient of the F01 scalar in the dimensionful density \(h_3^{-4}\Phi_n\) is

\[
 a_{\rm F01}=\frac{\sqrt6N}{2}\,c_\Phi.
 \tag{NW.24}
\]

The factor \(L^{12}\) in the block readout and the ratio \((g_3/g_0)^2\) in its normalized Hessian have not disappeared:

\[
 |c_\Phi|\le C_LL^{12}|\alpha|(g_3/g_0)^2.
 \tag{NW.25}
\]

No coupling, map, selector or finite-probe convention is retuned to force this coefficient to a prescribed value. The finite-pulse extraction SE is a different bounded projection; NW.24 is the coefficient of the actual marginal engineering jet.

### 4.1. A true supported counterterm, before absolute summation

The Ward identity for a sum does not imply that every original tag is separately gauge invariant. Apply the scalar Haar projection EC.1 to the complete scalar coefficients of (NW.3), using the orbit-uniform tube PJ.1a. This leaves their sum, anchor, raw determining support and analytic norm unchanged. It does not project overlapping uncontracted factors separately.

Next average each resulting anchored scalar coefficient over the finite rooted hypercubic group \(H_4\), of order \(2^4 4!=384\). For an original tag X at root zero set

\[
 f_X^{\circ}(U)
    =\frac1{|H_4|}\sum_{R\in H_4}
                   (\mathcal P f_X)(R^{-1}U),
 \qquad
 X^{\circ}=\bigcup_{R\in H_4}RX.
 \tag{NW.26}
\]

The carrier union is connected through its common root. Its size is at most a fixed constant \(C_H n(X)\), including the fixed geometric storage convention. Hence a choice \(\kappa_1<\kappa_0/C_H\) preserves a positive exponential rate and the bound (NW.3), up to a fixed constant. This is an explicit single finite loss, not an assertion that the same loss can be repeated at all depths. Each coefficient in (NW.26) is individually gauge invariant and rooted hypercubic. Their normally convergent sum is still \(\Phi_0^\alpha\), because the physical mark has these symmetries.

For each such coefficient apply the linear anchored moment functional

\[
 c_X=\frac1{12d_G}\sum_{\mu\ne\nu}
       \sum_{r,s,A}r_\nu s_\nu
       D_{a_{r\mu}^{A}}D_{a_{s\mu}^{A}}
                   f_X^{\circ}(e^{g_3a})\big|_{a=0},
 \qquad d_G=N^2-1.
 \tag{NW.27}
\]

Each coefficient satisfies Theorem NW.3, so this average is exactly its unique marginal coefficient. Absolute moment summability gives

\[
 \sum_X c_X=c_\Phi,\qquad
 \sum_Xe^{\kappa_2n(X^{\circ})}|c_X|
             \le C\mathfrak B g_3^2,
 \qquad 0<\kappa_2<\kappa_1.
 \tag{NW.28}
\]

Assign

\[
 r_X(U)=f_X^{\circ}(U)-f_X^{\circ}(I)
                              -\frac{c_X}{g_3^2}w_0(U)
 \tag{NW.29}
\]

to \(X^+=X^{\circ}\cup\operatorname{supp}w_0\). This is a fixed finite-stencil enlargement, with \(n(X^+)\le n(X^{\circ})+C\). It gives a normally convergent, genuinely supported representation of (NW.22) with norm \(C\mathfrak B\). Its local quadratic cancellation and the nonlinear engineering cancellation below hold **for each \(r_X\)** before taking absolute values. This is why the symmetry projection is performed on complete scalar tags first.

For a finite raw endpoint path, the corresponding exact identity is

\[
 \Delta r_X
   =\sum_{\ell=M,0,1,2}\Delta j_X^{\ell,\circ}
                   -\frac{c_X}{g_3^2}\Delta w_0.
 \tag{NW.30}
\]

Here \(\Delta j_X^{\ell,\circ}\) denotes the original labelled covector representation pulled back by the fixed gauge and lattice maps and then averaged, as in EC.13–EC.14. It is not a newly chosen value representation after differentiation. These are transported labelled representatives whose sum is the derivative of the symmetrized scalar. Identifying their full sums individually with the original physical-origin currents requires covariance of each origin under the lattice maps; it is not inferred here from covariance of the total scalar. In particular a reflected link can require a background-dependent adjoint conversion of free variables. The Wilson subtraction has its explicit current. Equation (NW.30) retains the labelled decomposition and the applicable pulled-back bounds; it does not claim an irrelevant gain or an unchanged physical-origin interpretation for each old label separately. Cancellation of the complete scalar is insufficient to infer either claim.

## 5. Non-Abelian engineering jets, proved by exact parallel transport

There is a useful rigorous meaning of the nonlinear engineering jet that avoids replacing a group link by an unjustified linear continuum sample. Let A be a globally bounded \(C^6\) connection on \(\mathbb R^4\), valued in \(\mathfrak{su}(N)\). For real t define

\[
 U_t(A)_{r\mu}
   =\text{parallel transport from }t(r+e_\mu)\text{ to }tr
                    \text{ for the connection }d+A.
 \tag{NW.31}
\]

Thus the link has source-endpoint covariance
\(U_t(A^v)_{r\mu}=v(tr)U_t(A)_{r\mu}v(t(r+e_\mu))^{-1}\).
Its leading logarithm is \(tA_\mu(tr)\). All couplings and source-zero maps remain fixed while t varies. It is a background-scale parameter, not a change of cutoff or a derivative of a running coupling.

For \(|t|\|A\|_\infty\) sufficiently small these links lie in the fixed physical chart uniformly in r. Their logarithms and first six t derivatives have bounds by fixed polynomials in \(1+|r|\) and \(1+\|A\|_{C^6}\). The supported analytic norm and spare carrier rate justify differentiating the local mark through order six, term by term. Each coefficient at t=0 is a local differential polynomial in the finite jet of A at the anchor. Far edges have position-polynomial coefficients, and their sums converge absolutely. A global Taylor approximation of A on the entire lattice is not used.

### Theorem NW.5 — the complete local remainder starts at degree six

For (NW.22),

\[
 \left.\frac{d^m}{dt^m}
        \mathscr R_0(U_t(A))\right|_{t=0}=0,
       \qquad 0\le m\le5.
 \tag{NW.32}
\]

Quantitatively, for \(|t|\|A\|_\infty\le c r_0\),

\[
 |\mathscr R_0(U_t(A))|
     \le C\mathfrak B\,(1+\|A\|_{C^6})^{12}|t|^6.
 \tag{NW.33}
\]

The same statement holds coefficientwise for (NW.29), and at a smaller positive carrier rate its absolute supported sum satisfies

\[
 \sum_X e^{\kappa_3n(X^+)}
        |r_X(U_t(A))|
     \le C\mathfrak B\,(1+\|A\|_{C^6})^{12}|t|^6.
 \tag{NW.34}
\]

The exponent twelve is just a fixed generous bound for the finite differentiation polynomial; it is not a critical exponent. Constants are independent of lattice volume in the infinite family. Winding corrections on finite tori require their separate treatment in (NW.6).

**Proof.** There are three points: the use of an admissible local gauge, identification of the fourth-order term with the same \(c_\Phi\), and a uniform sixth-derivative remainder.

**Local radial gauge for the jets.** A gauge transformation equal to identity at the origin can put A in radial gauge near the origin. On a sufficiently small ball its value lies in a fixed logarithm chart. Multiply that logarithm by a smooth cutoff and exponentiate to extend this gauge to identity outside a larger ball. The transformed connection is still globally bounded with at least five bounded derivatives, enough for the jets under consideration, and agrees with radial gauge near the anchor. No sixth-derivative bound for that transformed connection is needed. Exact lattice gauge invariance of (NW.31) means that the Taylor coefficients through degree five of \(\Phi_0(U_t(A))\) equal those computed after this transformation. For sufficiently small t both paths lie in the analytic germs; exact physical gauge invariance supplies the equality there.

In that local radial gauge,

\[
 A_\mu(y)=\int_0^1s y^\nu F_{\nu\mu}(sy)\,ds
        =\frac12y^\nu F_{\nu\mu}(0)+O(|y|^2).
 \tag{NW.35}
\]

For each fixed edge,

\[
 \log U_t(A)_{r\mu}
       =\frac{t^2}{2}
          (r+e_\mu/2)^\nu F_{\nu\mu}(0)+O(t^3).
 \tag{NW.36}
\]

The first field derivative of the scalar at identity is zero. In this gauge every link-angle jet starts at order two, so all field Taylor terms of order three or higher start at engineering order six. The quadratic term starts at order four. These statements are about termwise jets justified by the absolute spatial moments; a uniform \(O(t^2)\) small-link bound at arbitrarily distant edges is neither asserted nor needed. Consequently the constant-subtracted scalar has no engineering terms of degree one, two or three.

**Identification of the quartic term.** Define the normalized-coordinate quadratic moment tensor

\[
 M_{\mu\nu}^{\rho\sigma}
   =\sum_{r,s}(x_{r\mu})_\rho(x_{s\nu})_\sigma
                                k_{r\mu,s\nu}.
 \tag{NW.37}
\]

From (NW.13),

\[
 M_{\mu\nu}^{\rho\sigma}
      =c_\Phi(\delta_{\rho\sigma}\delta_{\mu\nu}
                          -\delta_{\sigma\mu}\delta_{\rho\nu}).
 \tag{NW.38}
\]

Inserting (NW.36) into the quadratic Taylor form, recalling that the Hessian in physical B coordinates is \(g_3^{-2}K\), gives

\[
 [t^4]\{\Phi_0(U_t(A))-\Phi_0(I)\}
   =\frac{c_\Phi}{2g_3^2}
                \sum_{\mu<\nu}\langle F_{\mu\nu}(0),F_{\mu\nu}(0)\rangle.
 \tag{NW.39}
\]

In detail the two contractions in (NW.38) each contribute twice the sum over \(\mu<\nu\); the two factors \(1/2\) in (NW.36) and the \(1/2\) in the quadratic Taylor formula give the displayed normalization. On the other hand the four oriented small plaquettes in each plane give

\[
 w_0(U_t(A))
       =\frac{t^4}{2}
            \sum_{\mu<\nu}\langle F_{\mu\nu}(0),F_{\mu\nu}(0)\rangle
          +O(t^5).
 \tag{NW.40}
\]

Thus the full Wilson subtraction (NW.22) removes this coefficient with exactly the scalar from the local two-momentum projector. In the original gauge this removes the associated quadratic, cubic and quartic connection terms together. It is not necessary to postulate a relation between those vertices: the exact gauge transformation and the local Ward tensor prove it.

**The odd terms.** Rooted inversion gives the exact identity
\(\Phi_0(U_{-t}(A))=\Phi_0(U_t(A))\). Indeed applying lattice inversion to the link field in (NW.31) produces precisely \(U_{-t}(A)\), including its reversed orientations. The same is true of \(w_0\) and of every scalar coefficient in (NW.26). All odd engineering derivatives vanish, in particular the fifth. Together with the constant subtraction and (NW.39) this proves (NW.32).

**The quantitative remainder.** Estimate the sixth derivative in the original connection, without using the estimating radial gauge. Parallel-transport differentiation on a segment of length \(|t|\), followed by the fixed logarithm chart, bounds its k-th t derivative for \(k\le6\) by
\(C_k(1+|r|)^k(1+\|A\|_{C^6})^{2k}\), uniformly when \(|t|\|A\|_\infty\le c r_0\). A chain-rule term of total order six contains derivatives whose orders sum to six. Physical Cauchy bounds for q field derivatives, \(q\le6\), cost only fixed powers of \(r_0^{-1}\) times (NW.3). The coordinate incidence factors and all position polynomials are paid by a fixed spatial moment and a strict rate reduction. This gives
\(C\mathfrak B(1+\|A\|_{C^6})^{12}\) for the sixth derivative. The explicit Wilson term has the same bound because \(|c_\Phi|/g_3^2\le C\mathfrak B\).

Taylor's integral remainder and (NW.32) prove (NW.33). For (NW.34) apply the argument to the individually invariant rooted coefficients (NW.29), using (NW.28) for their Wilson terms, and sum their nonnegative sixth-derivative majorants. Every cancellation occurs within one supported scalar before this sum. \(\square\)

The compact extension of radial gauge is important. A global radial gauge can grow with distance even for a bounded connection; using it as a uniform physical-tube estimate would be invalid. Here it is used only to identify finite jets. The numerical remainder is estimated in the original bounded connection.

## 6. Relation to the native quadratic completion and to the remaining transfer problem

There are two distinct useful completions.

* Equation (NW.22) completes only the unique local marginal jet with the actual local Wilson function. It leaves the higher-momentum quadratic response and the nonlinear irrelevant response together in one gauge-invariant scalar.
* The support-preserving cycle construction developed separately in [M04 Gauge Invariant Quadratic Completion](M04_Gauge_Invariant_Quadratic_Completion.md) completes the **entire** Hessian of an invariant carrier by bounded based-loop functions. Subtracting that completion leaves a third-order zero in raw link coordinates. That is the appropriate algebraic starting point for native weak-curvature Taylor estimates using local estimating gauges.

Neither operation alone proves that a nonlinear conditional kernel acts contractively on the specified M03 irrelevant norm. FH supplies an actual flat Gaussian transfer estimate, and PJ supplies explicit coupling powers for the actual smooth nonlinear jets. The complete local Ward extraction here identifies what has to be subtracted, including nonzero source momentum and its exact non-Abelian Wilson completion. Comparing the actual normalized conditional transport with the inherited Gaussian transfer, retaining separate physical currents and any cutoff corrections, remains a separate calculation. A smooth-background estimate such as (NW.34) is not substituted for that calculation.

The primary non-Abelian mechanism is consistent with CMP109, printed pp.282–290, especially the exact gauge identities (4.9)–(4.15) and their local polarization expansion. Those source identities are not used as a blanket assertion that every previously constructed tag has the requisite invariance; EC and (NW.26) supply that representation here. CMP109's later minimizing-background estimates also have a different regularity scale: its (4.18) is a \(C^{1,\gamma}\)-type second-difference estimate and does not by itself give the uniform sixth-order smooth-background bound proved above for prescribed \(C^6\) probes. No derivative gain beyond that source hypothesis is silently imposed on the actual minimizing field.

### Hypotheses and scope

This note uses the specified local physical symmetry and complete footprint registry SW.8/SW.2; the actual smooth physical tube and finite coupling-weighted jets PJ.1–PJ.2; and the support-preserving scalar real-gauge projection EC.1–EC.3. The moment classification, two-momentum projector, exact normalization, finite rooted symmetrization and nonlinear finite-jet argument are proved here. All constants remain fixed-three-layer constants. The result establishes a local nonlinear Ward extraction for the actual smooth block mark, with explicit supported and coupling-normalized bounds, and makes no claim that M04 or Yang–Mills existence is complete.
