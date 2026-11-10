# A local source alias gain for the actual inherited Gaussian lift

The spatially integrated quadratic estimate FH has zero source momentum. This note keeps the source anchor and both field momenta. The literal block sum produces an exactly unitary alias matrix, so it does not cost an extra factor `L^4`. An exponentially summable curvature-pair representation of the local Ward remainder makes that observation usable. Its mixed-derivative channels gain `L^(-2)`; the present estimate of its same-leg second-derivative channels gains `L^(-3/2)`. Both are actual positive gains for arbitrary coarse momenta, including nonzero source momentum.

The second exponent is not replaced by `L^(-2)` without proof. The second weighted alias Gram is naturally bounded here by `L^(-3)`, whose square root is `L^(-3/2)`. At zero source momentum the stronger FH estimate still applies.

For the actual third smooth conditional, SC adds its controlled `B_3 eta^2` quadratic error. NW then removes its small local marginal coefficient. A separate interpolation statement converts a real-momentum bound and a proved fixed-depth exponential pair envelope into explicit anchored pair-moment bounds. These pair norms are not the specified volume-plus-tree physical-carrier norm M03, and no closure of that norm is inferred.

## 1. An anchored curvature-pair representation

Work on the infinite level-b lattice, spacing one, with centered oriented edges and plaquettes. Write `F=dA`, and denote a positive plaquette by `(r,alpha)`, where `alpha=(mu,nu)`, `mu<nu`, and its geometric center is

\[
 z_{r\alpha}=r+(e_\mu+e_\nu)/2.
 \tag{LA.1}
\]

Let `Q_x(A)` be a translation-covariant family of real local quadratic forms, with root x. Suppose it comes from the Hessian of the invariant rooted coefficient representation in NW Section 4.1 after its local Wilson subtraction. Thus each complete scalar tag is gauge invariant and rooted hypercubic, has its marginal coefficient removed, and its normalized Hessian has an anchored exponential coefficient envelope. This hypothesis is fulfilled by the actual two-level smooth mark using PJ/EC/NW stopped at that depth. It is more than a pointwise Fourier inequality.

### Lemma LA.1 — actual summable curvature coefficients

There is a curvature-pair kernel c such that

\[
 Q_0(A)=\frac12\sum_{r,s,\alpha,\beta}
       \langle F_\alpha(r),c_{\alpha\beta}(r,s)F_\beta(s)\rangle,
 \tag{LA.2}
\]

and, for some positive rho,

\[
 \mathfrak C_{\rho}
   :=\sum_{r,s,\alpha,\beta}
      e^{\rho(|z_{r\alpha}|+|z_{s\beta}|)}
                            \|c_{\alpha\beta}(r,s)\|<\infty.
 \tag{LA.3}
\]

Its value is bounded by a strict-rate-loss multiple of the actual incoming anchored Hessian envelope. In particular its second moment

\[
 \mathfrak C_2
   :=\sum_{r,s,\alpha,\beta}
      (|z_{r\alpha}|+|z_{s\beta}|)^2
                           \|c_{\alpha\beta}(r,s)\|
 \tag{LA.4}
\]

is finite. Its independent-momentum kernel

\[
 C(k,l)=\sum_{r,s}e^{-ik\cdot z_{r\alpha}-il\cdot z_{s\beta}}
                         c_{\alpha\beta}(r,s)
 \tag{LA.5}
\]

can be chosen to satisfy

\[
 C(0,0)=0,
 \qquad DC(0,0)=0,
 \qquad C(-k,-l)=C(k,l).
 \tag{LA.6}
\]

This is a representation of a **quadratic pair kernel**. Plaquettes used to construct it do not enlarge the original nonlinear coefficient's physical support.

**Proof.** Work first with one finite, already invariant rooted tag X. Choose the forest of GC.1 in its actual raw input edge graph. The Hessian is exactly a sum of pairings of the linearized fundamental loop sums. Each loop has length at most `C n(X)` and lies within distance `C n(X)` of the anchor. A closed lattice loop in such a box can be reduced to the empty word by interchanging coordinate steps and canceling inverse steps. Each interchange is an elementary plaquette. It gives an integer plaquette 2-chain `z_e` with boundary the loop, total multiplicity at most `C n(X)^2`, and all its plaquettes within the same `C n(X)` box. At the linear cochain level,

\[
 L_e(A)=\sum_p z_e(p)(dA)(p).
 \tag{LA.7}
\]

The GC Hessian identity therefore gives the exact finite pair kernel

\[
 c_X(p,p')=\sum_{e,f}h_{ef}z_e(p)z_f(p').
 \tag{LA.8}
\]

The sum of absolute coefficients h is bounded by the complete raw Hessian's summed-coordinate norm: h is obtained by restricting that Hessian to nontree directions and taking the fixed colour trace. Multiplying by the two plaquette-chain norms costs at most `C n(X)^4`. Positions in (LA.8) are at most `C n(X)` from the root. Consequently a smaller positive anchored exponential rate, with its spare polynomial margin, sums (LA.8) over all actual tags and proves (LA.2)–(LA.4).

Average this curvature representation over the finite rooted hypercubic group. Its quadratic form stays equal to `Q_0` because that form is invariant; its pair norm changes only by a fixed group constant, and its positions have the same radius. In particular inversion acts evenly on each two-form component, so its multiplier satisfies `C(-k,-l)=C(k,l)`. This gives the first-derivative zero in (LA.6).

The degree-two raw one-form tensor represented by the constant matrix `C(0,0)` is zero because the local Wilson coefficient was removed by NW. At the linearized level it is the pairing of `k wedge u` and `l wedge v` through that constant matrix, for independently variable k,l,u,v. Each elementary basis two-form is obtained by choosing `k=e_mu,u=e_nu`; the two legs are independent. Hence all entries of `C(0,0)` vanish. This proves (LA.6).

The fillings are used only in the exact identity (LA.7) and the pair-kernel estimates. The original function, its Hessian on raw links, and its declared determining inputs remain unchanged. In particular no estimate with `exp(kappa * area of filled surface)` is asserted. A filling has polynomial multiplicity and position radius here; promoting its area to a new physical carrier would be a different norm claim. \(\square\)

This proof also shows why a numerical inequality such as NW.20 alone is insufficient as a replacement for LA.1: a bounded matrix on two momentum variables need not have a bounded Schur multiplier norm on alias arrays. The separable Fourier coefficients in (LA.5) supply the missing structure.

## 2. The exact inherited lift and its additional Gram estimate

Use FH's actual symmetric averaging operation with odd block size `L>=3`. Let `C_b(k)` be the inherited curvature covariance shape after b earlier Gaussian eliminations, and let

\[
 k_n=(p+2\pi n)/L,
 \quad
 M_n(p)=L^{-2}D_2(n)\operatorname{diag}(q(k_n))\big|_{\mathcal E(k_n)},
 \tag{LA.9}
\]

with precisely FH.5–FH.11. All aliases lie in the real fine Brillouin cube. Write

\[
 A_b(p)=\sum_n M_n C_b(k_n)M_n^*,
 \quad
 T_n(p)=C_b(k_n)M_n^*A_b(p)^{-1}.
 \tag{LA.10}
\]

These maps act on the coarse exact-curvature space. A common positive scalar coefficient of the inherited action cancels from T; no covariance is reset to bare Wilson. For `f=hat(d_c a)(p)` the minimizing fine curvature array in the FH unitary convention is `u_n=T_n f`.

Set

\[
 E_j(p;f)=\sum_n|\widehat k_n|^{2j}|T_n(p)f|^2,
 \qquad j=0,1,2.
 \tag{LA.11}
\]

FH.33–FH.37 give, with constants independent of b and L,

\[
 E_0\le C|f|^2,
 \qquad E_1\le C L^{-2}|\widehat p|^2|f|^2.
 \tag{LA.12}
\]

### Lemma LA.2 — second weighted alias Gram

With the same uniformity,

\[
 E_2(p;f)\le C L^{-3}|\widehat p|^4|f|^2.
 \tag{LA.13}
\]

**Proof.** Define the bare positive matrix

\[
 B_2(p)=\sum_n|\widehat k_n|^4 M_n M_n^*.
 \tag{LA.14}
\]

Use the exact-form projection before taking its trace, as in FH.17. For the term associated with an ordered distinct pair `(mu,nu)`, cancel
`S_mu^2 hat(k_mu)^2=hat(p_mu)^2`. The remaining weighted trace is bounded by the sum over j of

\[
 L^{-12}\widehat p_\mu^2
    \sum_n \widehat k_{n,j}^{\,2}
                  S_\nu^4\prod_{\lambda\ne\nu}S_\lambda^2.
 \tag{LA.15}
\]

If `j=nu`, use `S_nu^4 hat(k_nu)^2=hat(p_nu)^2 S_nu^2`; the four alias sums then give
`L^(-4) hat(p_mu)^2 hat(p_nu)^2`. If `j!=nu`, the j sum is

\[
 \sum_{n_j}S_j^2\widehat k_{n,j}^{\,2}
       =L\widehat p_j^2,
 \tag{LA.16}
\]

the nu sum is at most `L^4`, and the two other sums are `L^2` each. The term is at most `L^(-3) hat(p_mu)^2 hat(p_j)^2`. Summing the three possible nu for each mu, and using `L^(-4)<=L^(-3)`, gives

\[
 0\le B_2(p)\le\operatorname{Tr}B_2(p)I
        \le 3L^{-3}|\widehat p|^4I.
 \tag{LA.17}
\]

For the inherited map, `C_b(k)^2<=P_2(k)` and the uniform lower bound on `A_b` imply

\[
 E_2=f^*A_b^{-1}
     \left(\sum_n|\widehat k_n|^4 M_nC_b(k_n)^2M_n^*\right)
        A_b^{-1}f
     \le C\|B_2\|\,|f|^2.
 \tag{LA.18}
\]

The last step uses the operator-norm bound for `A_b^(-1)` and does not compare `A_b^(-1) B_2 A_b^(-1)` with `B_2` as quadratic forms; those matrices need not commute. Equation (LA.17) now proves (LA.13). The appearance of L rather than `L^0` in (LA.16) is the extra alias count that prevents this argument from giving `L^(-4)` for the second Gram. \(\square\)

Replacing `|hat k|` by `|k|` in (LA.11) changes only numerical constants on the fine Brillouin cube. At `p=0` actual periodic exact curvature is zero; all estimates are interpreted on the exact-form spaces or by limits from nonzero momenta. Harmonic one-cochains have zero-curvature lifts as in FH and do not contribute.

## 3. The literal local block sum is a unitary alias pairing

Consider the actual dimensionless block readout of the quadratic insertion,

\[
 Q^{\rm out}_N(a)=\rho^2\sum_{x\in B_L(LN)}Q_x(H_{b,L}a),
 \qquad \rho=g_{b+1}/g_b.
 \tag{LA.19}
\]

The factor rho is the literal ratio between normalized incoming and outgoing link angles. The sum is the block sum, not a block mean; it contains `L^4` sites.

For nonunitary infinite-volume Fourier transforms the fine curvature reconstruction is

\[
 F_H(x)=L^{-2}\int_{\mathrm{BZ}_c}
       \sum_n e^{ik_n\cdot x}T_n(p)f(p)\,\frac{dp}{(2\pi)^4},
 \tag{LA.20}
\]

with the appropriate plaquette-center phase. This is exactly FH's convention `u_n=L^(-2) hat F(k_n)`: changing fine momentum to its aliases contributes `L^(-4)` to the inverse transform. Thus each leg supplies `L^(-2)` in (LA.20).

Let `l_m=(q+2 pi m)/L`. The block sum in (LA.19), after the two factors in (LA.20), gives

\[
 S_{nm}(p,q)
   =L^{-4}\sum_{x\in B_L(0)}e^{i(k_n+l_m)\cdot x}
   =B_L(k_n+l_m).
 \tag{LA.21}
\]

### Lemma LA.3 — exact source matrix

For every pair of real coarse momenta, S is a unitary `L^4` by `L^4` matrix on alias space.

**Proof.** Let `U_{xn}=L^(-2) exp(2 pi i n dot x/L)` be the unitary discrete Fourier matrix of the centered block. Let `D_{xx}=exp(i(p+q) dot x/L)`. Equation (LA.21) is

\[
 S=U^{\mathsf T}DU.
 \tag{LA.22}
\]

The transpose of a unitary matrix is unitary, and D is unitary for real p,q. This proves the assertion. Multiplication of S on either side by any diagonal phases also preserves its norm one. \(\square\)

The source anchor has not been integrated out. Translation to a coarse anchor N multiplies the resulting two-momentum kernel by the expected phase `exp(i(p+q) dot N)`. Nonzero `p+q` appears exactly in D. At `q=-p`, S is the alias pairing permutation; this recovers the integrated FH situation.

The exact curvature multiplier of the root-zero block readout is, with bilinear Fourier conventions,

\[
 C_{\rm out}(p,q)
   =\rho^2\sum_{n,m}S_{nm}(p,q)
           T_n(p)^{\mathsf T}C(k_n,l_m)T_m(q).
 \tag{LA.23}
\]

Transposes are used because the independent Fourier legs describe the complex-bilinear extension of a real quadratic form. The absolute estimates below equally control its sesquilinear version after changing the sign of the first momentum. The operator norms use the ordinary complex Euclidean norms.

## 4. Same-leg and mixed-derivative gains

### Theorem LA.4 — a rooted two-momentum quadratic gain

On the exact-curvature input spaces,

\[
 \begin{split}
 |f^{\mathsf T}C_{\rm out}(p,q)g|
 \le C\rho^2\mathfrak C_2\bigl\{
       &L^{-3/2}(|\widehat p|^2+|\widehat q|^2)\\
       &+L^{-2}|\widehat p|\,|\widehat q|\bigr\}|f|\,|g|.
 \end{split}
 \tag{LA.24}
\]

The constants are independent of inherited Gaussian depth b, block size L and volume. In particular the rooted one-form Hessian `V_out` obeys

\[
 \boxed{
 |u^{\mathsf T}V_{\rm out}(p,q)v|
 \le C\rho^2\mathfrak C_2 L^{-3/2}
       (|\widehat p|+|\widehat q|)^2
       |\widehat p\wedge u|\,|\widehat q\wedge v|.
 }
 \tag{LA.25}
\]

Its local marginal Wilson coefficient is zero. At zero source momentum the sharper `L^(-2)` energy estimate of FH remains available.

**Proof.** By (LA.6) the second Taylor remainder of C is the absolutely convergent expression

\[
 C(k,l)=-\sum_{z,w}c(z,w)
     \int_0^1(1-t)(k\cdot z+l\cdot w)^2
                    e^{-it(k\cdot z+l\cdot w)}\,dt.
 \tag{LA.26}
\]

The zero constant and linear moments justify this identity exactly; no low-momentum restriction is used. Expand the square into its two same-leg terms and its mixed term. Fix one coefficient matrix c(z,w) and t. The phases in (LA.26) multiply the two alias arrays separately, so Lemma LA.3 still gives norm one for their pairing through S.

For a same-leg term, bilinear Cauchy–Schwarz on alias space bounds its absolute value by

\[
 \|c(z,w)\|\,|z|^2
        E_2(p;f)^{1/2}E_0(q;g)^{1/2}
 \le C\|c(z,w)\|\,|z|^2
                L^{-3/2}|\widehat p|^2|f|\,|g|.
 \tag{LA.27}
\]

The other same-leg term has w,q in place of z,p. The mixed term is bounded by

\[
 C\|c(z,w)\|\,|z|\,|w|
      E_1(p;f)^{1/2}E_1(q;g)^{1/2}
 \le C\|c(z,w)\|\,|z|\,|w|
               L^{-2}|\widehat p|\,|\widehat q|\,|f|\,|g|.
 \tag{LA.28}
\]

Sum the absolute second moments and integrate t to get (LA.24). Restoring the two coarse curl maps gives (LA.25). Its bound vanishes to total degree at least four in the two one-form momenta, so NW.14 extracts zero marginal coefficient. All source positions remain in (LA.21)–(LA.23). \(\square\)

For clarity define the concrete rooted Fourier seminorm

\[
 \|V\|_{\rm root,W}
  =\sup_{p,q,u,v}
   \frac{|u^{\mathsf T}V(p,q)v|}
    {(|\widehat p|+|\widehat q|)^2
               |\widehat p\wedge u|\,|\widehat q\wedge v|},
 \tag{LA.29}
\]

with zero denominators handled by continuity and restriction to nonzero transverse directions. Equation (LA.25) gives

\[
 \|V_{\rm out}\|_{\rm root,W}
                  \le C\rho^2\mathfrak C_2L^{-3/2}.
 \tag{LA.30}
\]

Unlike an integrated action norm, (LA.29) retains every source momentum and hence every translated local anchor. It is still a Fourier/curvature seminorm, not an exponential physical-carrier norm. This distinction is relevant when this estimate is used below.

## 5. Supported local moments and a quantitative interpolation

There is an independent actual fixed-depth exponential envelope for the raw output pair kernel. Here is the source-specific reason, rather than an assumption about the pseudoinverse factors in (LA.10). The actual flat minimizing lift can be differentiated in its physical constrained coordinates: it is a finite face lift plus the constraint/gauge-corrected response obtained from the complete constrained inverse. PR's gapped local inverse expansion and the TC.9 raw minimum registry give an exponentially summable linear response with every determining input retained. At the flat point this is exactly the H used in FH and SC. No analytic extension of the separate projection `P_2(p)` through its zero-momentum singularity is needed.

At the two incoming and one outgoing fixed levels, choose a positive coarse-distance rate sigma below that actual response rate. Substituting the two supported H responses in the incoming anchored raw Hessian gives

\[
 J_L:=\sum_{y,z,\mu,\nu}
       e^{\sigma(|y+e_\mu/2|+|z+e_\nu/2|)}
              |K^{\rm out}_{y\mu,z\nu}|
       \le C_L\rho^2 L^4\,\mathfrak K_{\rm in}.
 \tag{LA.31}
\]

Here `mathfrak K_in` is an incoming anchored exponential raw-Hessian norm at a compatible positive rate. The displayed `L^4` is the literal number of incoming roots; sharper bounds for H might reduce it, but are not assumed. Constants and sigma in (LA.31) are fixed-depth quantities and are not asserted uniform in L. This envelope has a different purpose from the cancellation in (LA.21): it proves actual pair locality, while (LA.25) proves smallness on real momenta.

For completeness, the general interpolation from these two facts is elementary. If a rooted kernel in two four-dimensional lattice variables has real Fourier supremum at most epsilon and exponential pair norm at most J at rate sigma, every coefficient is at most epsilon by Fourier inversion. Splitting the coefficient sum at distance R, and using the exponential envelope in the tail, gives for every fixed s

\[
 \sum_{y,z}(1+|y|+|z|)^s|K_{y,z}|
 \le C_s a\left[1+\sigma^{-1}
                       \log(2+J/a)\right]^{8+s},
 \qquad a=\min(\epsilon,J).
 \tag{LA.32}
\]

Fixed edge-center and colour constants are absorbed in `C_s`. If a is zero, either the real Fourier supremum or the exponential coefficient norm is zero, so the kernel is identically zero; that case is handled separately and no quotient `J/a` is formed. Indeed the near part in the nonzero case contains at most `C(1+R)^8` pairs and has its stated polynomial moment. For the far part, spend half the rate to pay that moment and choose `R` a sufficiently large multiple of `sigma^(-1) log(2+J/a)`. This bounds the remaining tail by `C_s a` with the displayed sigma dependence included.

A smaller positive exponential rate is also controlled. For `0<theta<1`, the same split gives

\[
 \|K\|_{\theta\sigma}
  \le C_{\sigma,\theta}\,
        a^{1-\theta}J^\theta
                    [1+\log(2+J/a)]^8.
 \tag{LA.33}
\]

Applying (LA.32)–(LA.33) to the actual kernel, with
`epsilon=C rho^2 mathfrak C_2 L^(-3/2)` from (LA.25) and J from (LA.31), gives explicit anchored output pair moments and a smaller-rate exponential pair norm. It is an actual estimate with its L dependence and locality constants exposed. It is not an L-uniform contraction claim: the size of `C_L` and the available sigma still matter, and a pair-distance norm is not the volume-plus-tree support norm of M03.

## 6. The actual smooth interacting local Hessian

Apply this result at incoming level two to the actual local mark after NW's local Wilson subtraction. Its block sum is the incoming observable in SC, with the same fixed counterterm summed over the block. The Gaussian endpoint of SC is exactly (LA.19): its fixed P-truncated conditional is centered, and its vacuum-subtracted quadratic expectation equals evaluation at the same minimizing lift. No truncation-bias term remains in that identity.

Let `V_act` be the actual local output Hessian of that smooth conditional, and `V_G` the Hessian in (LA.25). SC.32 gives their difference with every fixed source-anchor and field-position moment:

\[
 \|V_{\rm act}-V_G\|_{\rm anchored\ moments}
                     \le C_L B_3\eta^2,
 \quad
 \eta=C_L\{g_2P^3+(1+E_2)g_2P\}.
 \tag{LA.34}
\]

Both actual and Gaussian local Hessians satisfy the two local Ward identities and the rooted hypercubic symmetry. For the Gaussian term a coarse gradient has a fine pure-gradient lift, which its incoming local Hessian annihilates. Its local marginal is zero by (LA.25). Thus NW's local projector, applied to the difference in (LA.34), gives

\[
 |c_{\rm act}|\le C_L B_3\eta^2,
 \tag{LA.35}
\]

and

\[
 \boxed{
 \|(I-\Pi_{\rm loc})V_{\rm act}\|_{\rm root,W}
  \le C\rho^2\mathfrak C_2L^{-3/2}
                         +C_LB_3\eta^2.
 }
 \tag{LA.36}
\]

This is an actual interacting **local** quadratic estimate, including nonzero source momentum. The error's source normalization remains
`B_3=L^12 |alpha| (g_3/g_0)^2` from SC/PJ, since its incoming observable contains the whole final microscopic block. It is not silently identified with the one-incoming-site moment `mathfrak C_2`. The full nonlinear local Wilson completion of the small coefficient (LA.35) is NW.22; GC supplies a different support-preserving completion of the remaining entire Hessian.

The actual output already has the physical supported coefficient representation and moments from SC/PJ. The pair-kernel interpolation (LA.32) can be applied to its Wilson-subtracted Hessian using those fixed-depth envelopes. Neither that fact nor (LA.36) splits the gain among OP's separate current rows, which may lack a Ward identity in the current-direction slot. A full native nonlinear transfer estimate still needs that additional analysis.

## 7. Topology and limits

The construction above is on the infinite lattice or a compatible periodization of its embedded kernels. A torus tag with nontrivial winding cannot be filled by a finite plaquette chain in the torus in the manner of (LA.7). SW/PJ bound the separate winding coefficients exponentially in the period; they are retained as separate raw-kernel errors. They are not bounded by a pure curvature seminorm on a short torus, since flat holonomy can have zero local curl.

The new results are the anchored curvature-pair construction, the second weighted alias Gram, the exact unitary source pairing, and the resulting local positive gain and interacting local marginal estimate. The proof uses the actual averaging map and inherited Gaussian shape from FH, the actual smooth comparison from SC, and the literal local invariant source from NW/PJ/EC. It does not assume the desired nonlinear contraction, alter a hard Q domain, or prove an all-depth Yang–Mills construction.
