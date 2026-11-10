# A three-layer adaptive microscopic root and its actual path velocities

This is a fixed-depth statement.

This is for the actual third homogeneous, R-averaged native operation. The unmarked third component certificate and the nested real-domain certificate are supplied by M04_Third_Step_Analytic_Base_and_Joint_Certificate.md (TC) and M04_Third_Step_Nested_Core_Admission.md (NC). The precise uses of those actual inputs are stated below. The combined full third-step theorem is a separate application; nothing here is an induction in depth.

## 1. The observable, actual kernels, and scale factors

Put
\[
 h_j=L^jh_0,\qquad
 \beta_j=(Ng_j^2)^{-1},\qquad
 \rho_{j0}=g_j/g_0,\qquad 0\le j\le3 .
 \tag{TR.1}
\]
The finitely many adjacent coupling ratios are bounded on the source weak-coupling interval. They are retained in every physical fluctuation row. In particular no equality between a projected coupling scheme and the leading coefficient of an inherited analytic action is assumed.

For clarity, the cutoff subscripts in this note name the integration number, whereas TC's \(p_i\) and NC's \(P_i\) name the innovation/birth index:
\[
 P_0=p_0=P_{Q,0},\qquad
 P_{{\rm aux},2}=p_1=P_1=c_1P_{Q,1},\qquad
 P_{{\rm aux},3}=p_2=P_2=c_2P_{Q,2}.
 \tag{TR.1a}
\]
The positive \(c_1,c_2\) are fixed comparison fractions. Birth colours 0, 1 and 2 refer respectively to these three integrations, not to the coarse lattice on which a later copied payload is represented.

The microscopic scalar is the original one:
\[
 F(U)=\alpha\beta_0\sigma_{h_0}(x;U)-c,\qquad
 b=|\alpha|+h_0^4|c|.
 \tag{TR.2}
\]
Its identity part is not absorbed into a curvature regulator.

Write the exact successive reconstructions as
\[
 V_2=\Psi^{(2)}_W(z_2),\qquad
 V_1=\Psi^{(1)}_{V_2}(z_1),\qquad
 U=\Phi_{V_1}(z_0),\qquad W=V_3 .
 \tag{TR.3}
\]
They include the actual nonlinear averaging constraints, fixed-target exceptional solves, averaged gauge conversion, and the original measure/coarea factors. The normalized preimage Haar variables can be retained explicitly; the scalar is gauge invariant.

Let \(q_{0,P}\) be the actual first fixed-P conditional. Let \(q_{1,A}\) be the second auxiliary-P conditional whose coarse density is the analytic base in AD. Let \(q_{2,A}\) be TC's third auxiliary-P conditional constructed from that same analytic base, with its actual inherited action and its own full normalizer. Thus
\[
 T_{AAA}F(W)=q_{2,A,W}\,
        q_{1,A,\Psi^{(2)}_W(z_2)}\,
        q_{0,P,\Psi^{(1)}_{\Psi^{(2)}_W(z_2)}(z_1)}
        F\bigl(\Phi_{\Psi^{(1)}_{\Psi^{(2)}_W(z_2)}(z_1)}(z_0)\bigr).
 \tag{TR.4}
\]
The first letter A in this notation means the first fixed P domain. This is a convenient label for the all-smooth baseline, not a new change in its first cutoff.

The leading third classical quadratic may carry
\(\lambda_2=(g_2/g_1)^2\), when the second analytic base retains its literal \(g_1^{-2}\) classical coefficient. Its actual soft sampler keeps its \(g_2\) normalization. TC's uniform covariance bounds include these bounded positive factors. We do not replace that precision by the first-step bare Wilson Hessian.

For a complete final raw carrier \(Y\) define
\[
 E_Y^{(3)}(W)=\sum_{p\subset Y}\beta_3s(W_p),\qquad
 R_Y(W)=1+E_Y^{(3)}(W).
 \tag{TR.5}
\]
Every reference, constraint, averaging, gauge, and response footprint is included. All norms below are pointwise native value/current norms. No averaged M03 term is asserted without an additional outer-law moment theorem.

## 2. A classical background with the correct microscopic normalization

Use the BR local reference at current scale \(h_3\), evaluated on the microscopic lattice \(h_0\). At this fixed depth the number of microscopic coordinates above one current block is a fixed \(L\)-dependent constant. BR.23, with the literal source normalization of the force, gives
\[
 \beta_0\sum_{p\ {\rm read\ in}\ X}s(U_{{\rm ref},p})
 +\beta_0\sum_{e\ {\rm read\ in}\ X}|J_e(U_{\rm ref})|^2
 \le C_L\frac{\beta_0}{\beta_3}E_{X^{+c}}^{(3)}(W).
 \tag{TR.6}
\]
The prescribed-average mismatch is
\[
 B_c=\log\{W_c[\mathcal M^3U_{\rm ref}]_c^{-1}\}.
 \tag{TR.7}
\]
The straight subdivided reference edge is exactly \(W_c\). Each literal averaging contour differs from it by the plaquette fillings used in BR.25--26. Applying that recurrence for three steps with its actual local defect, rather than its geometric ceiling, proves
\[
 \beta_0\sum_{c\ {\rm read\ in}\ X}|B_c|^2
 \le C_L\frac{\beta_0}{\beta_3}E_{X^{+c}}^{(3)}(W).
 \tag{TR.8}
\]
Both sides vanish on locally flat data, including flat data with nontrivial local transports. No bound for an absolute connection potential is used.

In BR.29 every relative-correction Picard tree has a force or mismatch leaf. Distinguish one such leaf, bound the remaining leaves by the fixed contraction ceiling, and sum the differentiated contraction majorant. The common decoupled propagators have the same strictly summable raw carriers as in BR. This proves, at depth three, the matrix version of CB.9:
\[
 |A_{e,X}|\le a_{e,X}
 \left(\sum_{f\in{\rm foot}X}|J_f|^2+
             \sum_{c\in{\rm foot}X}|B_c|^2\right)^{1/2},
 \qquad
 \sup_e\sum_Xe^{\nu n(X)}a_{e,X}\le C_L .
 \tag{TR.9}
\]
The source normalized force and mismatch, the native-to-raw cover, and all fine incidences have been kept in this estimate. Its constant is allowed to depend on three fixed levels.

Let \(U_3(W)\) be the actual three-level constrained minimum. Combining the compact-reference plaquette matrix bound with (TR.6)--(TR.9) gives supported envelopes \(b_{p,X}\) such that
\[
 \sqrt{\beta_0}\,
   \|[U_{3,p}-I]_X\|
 \le C_L b_{p,X}
       \sqrt{\beta_0/\beta_3}\sqrt{E_X^{(3)}(W)},\qquad
 \sup_p\sum_Xe^{\nu n(X)}b_{p,X}\le C_L .
 \tag{TR.10}
\]
This is a bound for a matrix defect on the common coefficient polydiscs. It is not obtained by taking a square root of a complex Wilson trace.

The zero-innovation reconstruction in (TR.3) lies on the same critical orbit as \(U_3(W)\). Indeed, exact recursive averages make each finer tangent kernel a subspace of the next coarser tangent kernel. The coarser critical field is in the finer regular class and is critical for that smaller tangent space. The source uniqueness of the finer regular critical orbit applies twice. This is the VN argument; no inclusion between complete regular competitor classes is claimed.

## 3. Three compatible innovation leaves

Choose the zero-innovation background \(U_*(W)\) to be the common \(U_3\) coefficient family in the actual first representative. The required gauge conversion is a composition of the fixed-block, center-fixed averaged-gauge maps. It is analytic and has its full local footprint. The background Wilson trace is unchanged.

At the physical parameter the exact reconstruction can be factored in local relative charts as
\[
 U(z_0,z_1,z_2,W)
  =e^{i\Theta^{(0)}}e^{i\Theta^{(1)}}e^{i\Theta^{(2)}}U_*(W).
 \tag{TR.11}
\]
Here the successive relative differences compare:

1. \(\Phi_{V_1}(z_0)\) with \(\Phi_{V_1}(0)\);
2. \(U_1(\Psi^{(1)}_{V_2}(z_1))\) with \(U_1(\Psi^{(1)}_{V_2}(0))\);
3. the zero-\(z_0,z_1\) reconstruction at \(\Psi^{(2)}_W(z_2)\) with its value at \(\Psi^{(2)}_W(0)\).

Each difference is formed and zero-subtracted before localization. Consequently
\[
 \Theta^{(i)}(z_i=0,z_{i+1},\ldots,W)=0
 \quad\hbox{coefficientwise},\qquad i=0,1,2 .
 \tag{TR.12}
\]
The third difference can equivalently be evaluated along the actual two-level minimum, in the prescribed representative, by the critical-orbit identification just proved. Integrating its source variational derivative along
\(\Psi^{(2)}_W(tz_2)\) inserts a physical \(g_2z_2\) leaf. The first two differences insert \(g_0z_0\) and \(g_1z_1\). CMP102 Proposition 9 controls the actual variational derivative and contraction inverse; the fixed-target local solves and local gauge maps have the same analytic fixed-depth bounds. Apply component decoupling before summing those derivatives.

Thus there are deterministic coefficient envelopes, uniform on the declared physical fluctuation tubes and coefficient polydiscs, with
\[
 |\Theta^{(i)}_{e,X}|
       \le C_L a^{(i)}_{e,X}g_i\|z_{i,X}\|,
 \qquad
 \sup_e\sum_Xe^{\nu n(X)}a^{(i)}_{e,X}\le C_L,
 \quad i=0,1,2 .
 \tag{TR.13}
\]
Products and relative logarithms can enlarge a carrier by a fixed number of its actual local footprints. They introduce no support chosen from a numerical decay estimate alone.

Away from the physical localization parameter, (TR.11) is the chosen compatible continuation: multiply this common \(U_3\) background by the three coefficientwise zero-subtracted families. It is not asserted to coincide with separately decoupled nested stationary points. The density always uses its own already-canceled TC continuation. In particular no residual \(g_i^{-1}J\cdot z_i\) term is introduced by re-expanding at an artificial noncritical saddle.

### Lemma TR.1 — a joint three-innovation microscopic root

There is an anchored connected raw expansion
\[
 h_0^4F(U(z_0,z_1,z_2,W))
      =\sum_{Y\ni x^{(3)}}f_Y(z_0,z_1,z_2,W)
 \tag{TR.14}
\]
with strictly summable coefficient envelopes \(a_Y\). Put
\(c_Y(W)=f_Y(0,0,0,W)\). Then
\[
 |c_Y|\le C_L b a_Y R_Y,
\]
\[
 |f_Y-c_Y|
 \le C_L b a_Y
 \left[
     \sqrt{R_Y}\sum_{i=0}^2\rho_{i0}\|z_{i,Y}\|
       +\sum_{i=0}^2\rho_{i0}^2\|z_{i,Y}\|^2
 \right].
 \tag{TR.15}
\]
The bounds hold as absolute coefficient envelopes on the common component domains. The number \(d_Y\) of root coordinates at all three levels is at most \(C_L(1+n(Y))\).

Writing \(\xi=(z_0,z_1,z_2)\), the exact Taylor identity is
\[
 f_Y-c_Y=\sum_i\ell_{Y,i}(W)\xi_i+
                \sum_{i,j}\xi_i v_{Y,ij}(g_0z_0,g_1z_1,g_2z_2,W)\xi_j .
 \tag{TR.16}
\]
After a fixed polynomial allowance for coordinate incidence,
\[
 \sum_i|\ell_{Y,i}|
     \le C_L b a_Y(1+d_Y)^3\sqrt{R_Y},\qquad
 \sum_{i,j}\sup|v_{Y,ij}|
     \le C_L b a_Y(1+d_Y)^3.
 \tag{TR.17}
\]
The same bounds, with a fixed carrier-incidence polynomial, hold for a normalized final-field derivative of the coefficient family on its fixed current discs.

**Proof.** The exact holomorphic Wilson identity is
\(\mathsf s(P)=-\tfrac12{\rm Tr}[(P-I)^2P^{-1}]\).
Use the matrix background envelope (TR.10) for its first derivative and (TR.13) for the relative increments. Every fluctuation derivative retains its own \(g_i\); hence the quadratic factors are exactly
\[
 \beta_0g_ig_j=\rho_{i0}\rho_{j0}/N.
 \tag{TR.18}
\]
Mixed rows use \(2ab\le a^2+b^2\) on their union carriers. The integral Taylor remainder retains second derivatives of the reconstruction, not only the Wilson Hessian. The coefficient functions and their fixed-order derivatives are bounded on the fixed physical chart. Their supported convolutions and coordinate incidences are paid by a strict carrier-rate reduction. This proves (TR.15)--(TR.17).

For a final normalized raw current, the physical input is \(g_3\). The background reference and its force and mismatch derivatives, the actual variational responses, and every zero-subtracted reconstruction coefficient are continued on the same fixed native tube. A normalized one-coordinate complex disc adds a bounded amount to the real-center final energy because \(\beta_3g_3^2=1/N\). Taking that disc after forming the deterministic matrix and Taylor-row envelopes proves the stated current version. This step does not differentiate an adaptive source radius. ∎

The full original background is present in \(c_Y\) and in the two later innovation leaves. In particular the intermediate quantity \(F(\Phi_{V_1}(0))\), which depends on \(z_1,z_2\), has not been dropped when passing to a later integral.

## 4. Actual lifted velocities and their coupling cancellation

Take one buffered normalized final path \(W(\theta)\). At fixed original \(z_2\), the path in \(V_2\) is \(\Psi^{(2)}_{W(\theta)}(z_2)\). At fixed \(z_1,z_2\), the path in \(V_1\) is its further reconstruction. The physical derivatives of these maps have the source analytic bounds \(C_Lg_3\), with summed supported coefficient envelopes. Relative logarithms at level \(i\) divide by their actual \(g_i\); they therefore produce \(g_3/g_i\), not a bare inverse coupling.

More generally, in NC's common nested real frames write
\[
 z_2=T_2(B_2,\theta),\qquad
 z_1=T_1(B_1,B_2,\theta),\qquad
 z_0=T_0(u_0,B_1,B_2,\theta).
 \tag{TR.19}
\]
The diagonal chart inverses are uniformly bounded. Its supported rows satisfy
\[
 \|\partial_\theta T_i\|\le C_L g_3/g_i,\qquad
 \|D_{B_j}T_i\|\le C_Lg_j/g_i\quad(j>i).
 \tag{TR.20}
\]
Here and below the norm includes the actual summed-direction coefficient envelope after a fixed carrier-rate loss; it is not an assertion that the number of held old coordinates inside a changing-depth cell is bounded. At three fixed levels that number is \(L\)-dependent and is counted.

Define the compensating velocities backwards:
\[
 v_2=(D_{B_2}T_2)^{-1}\partial_\theta T_2,\qquad
 v_i=(D_{B_i}T_i)^{-1}
       \left(\partial_\theta T_i-\sum_{j>i}D_{B_j}T_i\,v_j\right)
       \quad(i=1,0).
 \tag{TR.21}
\]
The notation \(B_0=u_0\) is used in this formula. Each summand has the same normalization:
\[
 (g_j/g_i)(g_3/g_j)=g_3/g_i.
 \tag{TR.22}
\]
Consequently the full three-level transport has the bounds \(C_Lg_3/g_i\) with genuine supported coefficients and polynomial incidence losses. There are two backward additions, not a depth-dependent iteration.

The physical origin of a derivative is assigned before (TR.19). The transformed operator keeping all original free coordinates fixed is
\[
 \mathscr L=\partial_\theta-\sum_{i=0}^2v_i\cdot\partial_{B_i}.
 \tag{TR.23}
\]
For \(J_i=\det D_{B_i}T_i\), its appropriate fiber identity is
\[
 \left(\partial_\theta-\sum_{j\ge i}v_j\cdot\partial_{B_j}\right)
       \log J_i=\operatorname{div}_{B_i}v_i .
 \tag{TR.24}
\]
It follows by differentiating the defining transport equation for \(T_i\) with respect to its own fiber coordinate. The dependence on coarser \(B_j\) is retained. Equivalently, multiplying by all three Jacobians gives the full triangular transport/divergence identity. These identities preserve factor ownership; they do not transfer the derivative of an old normalizer into an older label merely because equal zero-jet factors later cancel.

In the smooth baseline, the joint bound for an old current along the actual lifted path can also be obtained by varying only the corresponding final-field copy in Section 6. This is a derivative of its actual primitive factors along that lifted path. It is not a sum of stored old elementary finite differences and is valid even when the eventual Q path lies in a cutoff-tie stratum. For the Q factors themselves, the joint latent shape argument is reapplied in NC, before any such integration.

## 5. One deterministic reserve for all three levels

At a localized component the centered reference has the triangular form
\[
 d\mu_2(z_2)\,d\mu_{1,z_2}(z_1)\,
                  d\mu_{0,z_1,z_2}(z_0).
 \tag{TR.25}
\]
It is not assumed to be an independent product. TC supplies uniform covariance bounds for these actual centered conditional references, including the inherited force-corrected precisions and the real capped later inputs. Each complex continuation uses one covariance for its inverse and determinant. Its tunably small full-rank losses are paid per constituent primitive marginal.

### Lemma TR.2 — the three-level trace store

Let \(D_i\ge0\) be deterministic diagonal stores, independent of all three integration variables, with
\(\sum_{i=0}^2{\rm Tr}D_i\le C_*\).
For a sufficiently small fixed \(a>0\),
\[
 \int \exp\!\left(a\sum_{i=0}^2z_i^TD_iz_i\right)d\mu
       \le \exp\!\left(Ca\sum_{i=0}^2{\rm Tr}D_i\right).
 \tag{TR.26}
\]
The covariance of a lower level may depend arbitrarily on later real variables subject to the stated uniform bounds.

**Proof.** Integrate \(z_0\) first and apply the normalized Gaussian determinant formula for a quadratic tilt. Its bound is \(\exp(Ca{\rm Tr}D_0)\), independent of \(z_1,z_2\). Repeat for \(z_1\), then \(z_2\). Small full-rank tilts already present in the complex majorants change the covariance constants by a fixed factor and retain their declared small rank costs. No probability of a whole-volume cutoff event is divided out. ∎

For its application take deterministic suprema of all Taylor and response coefficient rows over the entire real path, copy box, source circles, outside coefficient polydiscs, and capped physical fluctuation tube. The stores are constructed from these suprema before integration. In particular neither \(D_2\) nor \(D_1\) is chosen after observing a later innovation.

An absolute linear row with normalized \(\ell^1\) mass at most one is bounded by the square root of a diagonal quadratic store of trace at most one. An absolute quadratic row is bounded by the diagonal store with entries half its row-plus-column sums. Cross-level entries are paid by \(2|z_i z_j|\le z_i^2+z_j^2\). Summing these fixed stores for the single root and its differentiated reconstruction rows leaves a fixed trace budget. Physical factors \(\rho_{i0}\) and \(g_3/g_i\) stay in their bounded fixed-depth constants.

This fixed-trace assertion concerns the marked rows. It does not assign a rank-independent trace budget to an arbitrary density score. Gaussian, action, and normalizer responses use TC's existing small full-rank reserve on the same parameter disc, with the declared rank and carrier-incidence polynomial. The additional marked store fits inside its unused quadratic margin. Thus the smooth current Cauchy estimate in Section 7 controls the marked row and the density response simultaneously, rather than multiplying two separately integrated moment bounds.

This construction is the required joint energy--velocity control. The response and the root are bounded on one common primitive box before taking the conditional expectations. A separate moment bound for old energy followed by a separate bound for the path velocity would not establish (TR.26) for their product.

## 6. Four copies, one source circle, and all smooth origins

Let \(W_M,W_0,W_1,W_2\) be independent admitted copies in the same final normalized elementary path box. Define
\[
 \begin{split}
 \mathcal A_A(W_M,W_0,W_1,W_2)
 ={}&\int q_{2,A}(dz_2\mid W_2)
       \int q_{1,A}(dz_1\mid\Psi^{(2)}_{W_1}(z_2))\\
 &\times\int q_{0,P}
    (dz_0\mid\Psi^{(1)}_{\Psi^{(2)}_{W_0}(z_2)}(z_1))\\
 &\times F\!\left(
 \Phi_{\Psi^{(1)}_{\Psi^{(2)}_{W_M}(z_2)}(z_1)}(z_0)\right).
 \end{split}
 \tag{TR.27}
\]
Every density is the continuation of its own already-canceled actual normal form. The copies do not ask a density to be re-expanded about the mark's background.

The required real and complex admission follows from the fixed native buffers in TC/NC and the additional \(O(g_3)\) copy perturbations. All three P domains are fixed. A common positive regulator is
\[
 \mathcal R_Y=1+\sum_{r=M,0,1,2}E_Y^{(3)}(W_r)
       \le4\widehat R_Y
 \tag{TR.28}
\]
on the real endpoint rectangle. One-coordinate normalized complex discs have the same bounded additive energy allowance as in Lemma TR.1. Freeze a number \(R_Y^{\rm box}\) dominating these envelopes on the whole box.

For a root \(Y\) choose
\[
 A_Y=C_L b a_Y(1+d_Y)^3(1+\sqrt{R_Y^{\rm box}}),\qquad
 \rho_Y=\frac{r_*e^{-\lambda n(Y)}}{A_Y}.
 \tag{TR.29}
\]
If \(A_Y=0\), omit that coefficient. The source couples to dimensionless \(f_Y\); the physical source for \(F_Y\) has radius \(h_0^4\rho_Y\). Freeze this same radius for every current.

The single source factor is
\[
 e^{\tau(f_Y-c_Y)}-1.
 \tag{TR.30}
\]
Apply the normalized row construction and Lemma TR.2, using one auxiliary small amplitude to extract this factor by Cauchy. On \(|\tau|\le2\rho_Y\), its positive primitive majorant has a small prefactor
\(Cr_*e^{-\lambda n(Y)}\) and exactly one \(D_0,D_1,D_2\) store. The stores and prefactor are simultaneous, uniform over the four copies. No source disk is separately optimized for each copied old logarithmic payload.

## 7. Three exact conditional normalizations

For the root source define \(N_Y(\tau)\) from (TR.27) by replacing its last line by
\(\exp\{\tau[f_Y-c_Y]\}\). Then
\[
 N_Y(0;W_M,W_0,W_1,W_2)=1
 \tag{TR.31}
\]
for all admitted copies. This identity retains the two inherited conditional normalizers and the new denominator.

The normalization is performed in the following order.

**First level.** Insert the single factor (TR.30) into the first P numerator. Its normalized connected expansion is CN's excluded-vacuum expansion for that same first P gas. Exactly one distinguished old copy carries the root and the remaining \(D_1,D_2\) stores. All additional old vacuum copies have the uniform-in-later-variables TC certificate and add no later quadratic root store.

**Middle level.** Compose the resulting supported normalized family with the actual middle readout registry, keeping all its old connectors. Normalize by the actual second auxiliary-P denominator. The marked branch carries \(D_1,D_2\). Integrate its middle Gaussian using \(D_1\); the one remaining store is \(D_2\). Additional middle unmarked vacuum factors retain their old depth-one conditional copies and their uniform-in-\(z_2\) TC certificates. They do not receive a new \(z_2^2\) tilt for each such copy.

**Third level.** Compose with the common third raw registry, and normalize with the actual \(q_{2,A}\) denominator. The distinguished branch has one \(D_2\) store. All old copied trees have already been bounded uniformly in that same real \(z_2\). Integrate the third Gaussian once.

At each stage the incident-vacuum expansion uses the full root carrier, including its previous analytic connectors. Disjoint components cancel by the exact component restriction of the same unmarked family. These are not estimates for the pointwise reciprocal of an extensive partition function.

Every rank loss is charged before the relevant cluster sum to its own constituent primitive marginal:
\[
 r_i\le C_{m_i}|I_i|.
 \tag{TR.32}
\]
The fixed buffer tail is chosen first so its small exponent times \(C_{m_i}\) fits a strict ordinary carrier margin. The fixed-depth physical perturbations are then made small by the common coupling ceiling. Repeated copies retain multiplicity. There is no bound on their total latent rank by the volume of the union of their carriers, and no such bound is used.

### Proposition TR.3 — the normalized smooth adaptive root

Under the actual TC common component inputs just enumerated, choose fixed localization margins and then a positive final carrier rate \(\kappa\). The three-stage construction gives
\[
 \sum_{Z\supset Y}e^{\kappa n(Z)}
      \sum_\gamma\sup_{|\tau|\le\rho_Y}
           |[N_Y(\tau)-1]_{Z,\gamma}|
       \le Cr_*e^{-\lambda' n(Y)}.
 \tag{TR.33}
\]
The same deterministic majorants control each first current copy, with a polynomial carrier incidence loss paid by spare rate.

**Proof.** Use (TR.30), the three-level trace store, and the three exact normalizations above. Each stage is the positive connected component/tree majorant of its own source-free gas with one distinguished root. The source prefactor pays the initial root weight, each incident-vacuum exponential uses its small anchored budget, and ordinary connectors have only fixed collars. The fixed TC source blocks and outside discs are chosen with strict margins for the three fixed cover conversions. Choose \(\lambda\) below the remaining root reconstruction decay and above the fixed root costs, then \(\kappa\) below the resulting rate.

Here is an explicit rate ledger for that choice. Let \(\nu_R>0\) be a remaining rate of the root envelopes after the three fixed native-to-raw conversions. Let \(C_{\rm cov}\) bound the fixed root/ordinary-buffer cover incidences; let \(\varepsilon_i\) be the anchored incident-vacuum budget at level \(i\), and let \(\eta_i r_i\) be that level's small marginal-rank loss. Choose the fixed buffers comparably, \(m_i=a_i m\), with the fixed \(a_i\) large enough to contain the earlier covers. Their omitted covariance tails decrease exponentially in \(m\), whereas their volume/rank constants grow only polynomially. Hence \(m\) can first be chosen to make the tail part of
\(\sum_i C_{\rm cov}\eta_i C_{m_i}\) as small as desired. Then choose the physical perturbation ceiling and the coupling so that
\[
 \Lambda_{\rm excl}
   :=C_{\rm cov}\sum_{i=0}^2
                (\varepsilon_i+\eta_i C_{m_i})<\nu_R/16.
 \tag{TR.33a}
\]
This is possible because the ordinary interaction/failed-P budgets are small and the Gram omitted-tail loss is tunably small. The normalized Gaussian references themselves have unit mass: there is no unaccounted fixed factor \(C^{r_i}\) in this assertion.

Reserve a further rate loss below \(\nu_R/16\) for fixed-degree incidence polynomials, choose \(\kappa C_{\rm cov}<\nu_R/16\), and take, for example, \(\lambda=\nu_R/4\). The three exclusions and initial carrier weight then use less than \(3\nu_R/16\), leaving \(\lambda'>0\) in (TR.33). After source Cauchy returns \(e^{\lambda n(Y)}\), the root still has rate at least \(\nu_R-\lambda\) before the smaller final incidence losses. These choices are fixed-depth choices made once. They do not assume a non-tunable \(C^{|Y|}\) loss can be overcome by making the coupling small.

The four copies are analytic with fixed domains here. A normalized one-coordinate disc in any one copy therefore differentiates that copy's actual primitive factors, including its inverse/determinant, coarea and normalizer. It has the same source radius and the same joint stores. Cauchy is taken before summing the deterministic envelopes. The response is zero outside the complete carrier; summing final directions contributes only its fixed polynomial incidence. This proves both claims. ∎

Take \(r_*\) so the rooted norm is below one half. The logarithm of \(N_Y\) exists by its convergent rooted series, not by a presumed whole-kernel zero-free tube. Products remain connected because they share \(Y\). Source Cauchy and restoration of \(c_Y\) give an absolute final-energy bound. Each kernel-copy derivative of \(c_Y\) is zero by that kernel's own normalization; its microscopic-origin response retains the classical energy derivative.

On the diagonal, differentiating the four copies in (TR.27) gives the actual infinitesimal origins \(M,0,1,2\). In particular the copy \(W_0\) differentiates the first kernel along the full lifted path
\(\Psi^{(1)}_{\Psi^{(2)}_{W(\theta)}(z_2)}(z_1)\), with the later innovations fixed. It does not use old elementary current values. The analogous statement holds at the middle level.

Thus the smooth baseline has a common value/first-jet registry with
\[
 h_3^4\sum_Ze^{\kappa n(Z)}
 \left[
    \sup_W\frac{|A_Z|}{R_Z}
    +\sup_W\sum_d\sup_{0<|t|\le1}
        \frac{\sum_{r=M,0,1,2}|J^r_{Z,d,t}|}
             {\widehat R_Z^{3/2}}
 \right]
       \le C_L L^{12}b .
 \tag{TR.34}
\]
Here \(J^r\) is the integral of its actual diagonal infinitesimal origin on the path, divided by \(t\). Smooth fixed-domain endpoint rectangles could also be formed, but (TR.34) is the path convention needed for subsequent Q comparisons.

## 8. The native root on the Q-core and shell families

For the one-moving-domain extension and the inherited rare colours, a weaker unweighted native bound suffices. Put
\[
 P_{\max}=\max(P_0,P_{Q,1},P_{Q,2}).
 \tag{TR.35}
\]
At three adjacent native levels these radii are comparable up to fixed constants, including the chosen small fixed auxiliary-P fractions. The actual caps and contour plateaux use the full Q radii, not those auxiliary fractions.

On TC/NC's admitted nested coefficient family, the total physical background and innovation inputs are bounded by
\[
 C_L(\epsilon_3+g_2P_{Q,2}+g_1P_{Q,1}+g_0P_0),
 \tag{TR.36}
\]
plus a fixed \(O(g_i)\) displacement on a moved coordinate. The literal source choice has \(\epsilon_j=g_jp_0(g_j)\) and \(\delta_j/\epsilon_j\) a fixed positive hierarchy ratio. The adjacent-coupling bounds of CMP119 (2.6) keep these logarithmic cutoffs comparable over three fixed levels. Dividing (TR.36) by \(g_0\) therefore gives \(C_LP_{\max}\). The same two-curvature-leaf proof as in Lemma TR.1 gives the full, not background-subtracted, primitive source envelope
\[
 M_F=C_L b h_0^{-4}P_{\max}^2.
 \tag{TR.37}
\]
Its first-origin versions have a fixed polynomial in the native radii and carrier incidences. This bound uses the actual root before any lower conditional integration. It is not inferred from the already integrated MB norm.

The root remains analytic on a moved outer coordinate because every inner fixed-P domain stays fixed and every old coefficient input lies in its native fixed tube. NC's complete-stencil frame and zero-completion argument provides the real admission on the whole third-Q fiber. The independently copied smooth inputs differ by \(O(g_3)\), which preserves the fixed old-selector slack. Their complex continuations use that fixed tube, not a holomorphic continuation of a smooth ambient guard.

On the contour, cap the coefficient inputs only and keep every leading Gaussian quadratic on its original variables. The moved-coordinate caps are identically one on the whole contour/homotopy. The cap radius is based on \(P_{Q,2}\); no replacement by the printed later narrow R radius is made.

### Proposition TR.4 — one source can be attached to the actual rare primitive families

Use a fixed source circle \(|t|\le c/M_F\). The common three-level primitive family with the additional factor \(e^{tF}\) satisfies TC's strict positive component majorants after a fixed reduction of its margin. A connected difference between two routes that changes a Q/P domain or an inherited defect colour has both a source-containing part and the changed colour. Its first source derivative, including any one of the four physical path origins, has a majorant of the form
\[
 C_L b h_0^{-4}\,
   A_{\mathcal I}\,
   {\rm poly}(P_{\max},R_0,R_1,R_2,n(\mathcal I))\,
   e^{\eta_0r_0+\eta_1r_1+\eta_2r_2+C|S|}
   e^{-c(n_0P_0^2+n_1P_{{\rm aux},2}^2+n_2P_{{\rm aux},3}^2)} .
 \tag{TR.38}
\]
The current source factor \(M_F\) is extracted exactly once. The displayed polynomial can include that \(P_{\max}^2\) factor; it is not an additional second source normalization.

**Proof.** The full root's absolute native coefficient norm is at most \(M_F\). Its source Mayer factor therefore has arbitrarily small positive component norm on the stated fixed circle. It is inserted into the same primitive gases, with their actual latent copies. Source-only factors in a lower smooth gas have fixed domains and no nonanalytic growing core; their small rank losses are paid per primitive before logarithmic clustering. Source-containing old-Q payloads retain their existing uniform-in-later-real-variable conditional certificates. The common third Gaussian is still integrated once.

The source-dependent logarithmic difference is formed after subtracting its zero-source value. Each surviving connected tag has a source and at least one changed defect colour. The positive fugacity argument and same-gas normalizations are those of the actual TC construction, now with a small source species included. They preserve the indicated generation tails and full raw core footprints.

For smooth responses differentiate the owned primitive factors on their native discs. For moving-domain responses use the real shell/chain certificate on the appropriate owned Q factor. Its velocity is (TR.20)--(TR.22). On a birth-0 or birth-1 surface, its own lower conditional reserve supplies the corresponding old tail. A new whole-Q surface on a specified old core uses the uniform-in-new-variable old certificate, so that old tail is still present even when no new tail is spent. NC's triangular transport retains the original velocities on joint ties, the fiber Jacobians, and each occurrence's zero-mass normalizer identity.

The smooth and shell factors have only fixed-order coordinate, trace and perimeter polynomials. Source Cauchy costs \(M_F\) once. A fixed part of a present generation tail pays the cutoff/core polynomials and that generation's allocated enlarged core volume; fixed-depth radius comparison permits using \(P_{\max}\) in this payment. Polynomial incidence on arbitrary ordinary analytic connectors is paid by their strict spatial rate, not by a tail at an unrelated core. For repeated latent ranks, the ordinary contribution uses its constituent spatial margin as in (TR.32); a growing-core contribution uses its own distinct occurrence's separately allocated birth-tail fraction, exactly as in TC.11a. Multiplicity is retained and no allocated fraction is spent twice. This proves the displayed majorant. ∎

### 8.1 A changed colour survives in each origin separately

For the inherited-colour comparison, denote the full route by F and the first-P/second-auxiliary-P/third-Q route by A. All reconstructions are the same actual physical maps on the diagonal. Write \(q_i^F,q_i^A\) for their normalized kernel occurrences, with their arguments in (TR.3) understood. Set
\[
 \begin{array}{ll}
 N_0^F=n_{0,Q},&N_0^A=n_{0,P},\\
 N_1^F=n_{1,Q}m_0,&N_1^A=n_{1,A},\\
 N_2^F=n_{2,Q}m_2,&N_2^A=n_{2,Q},
 \end{array}
 \qquad
 m_0=Z_{0,Q}/Z_{0,P},\quad m_2=e^{E_2}.
 \tag{TR.38a}
\]
Here \(n_{1,Q}=\chi_{Q,1}D_1\), \(n_{1,A}=\chi_{p_1}D_1\), and \(n_{2,Q}=\chi_{Q,2}D_2\), with all measure factors included. This is TC.29a before cancellation. The unnormalized differences are exactly
\[
 \begin{split}
 \Delta N_0&=n_{0,Q}-n_{0,P},\\
 \Delta N_1&=(n_{1,Q}-n_{1,A})+n_{1,Q}(m_0-1),\\
 \Delta N_2&=n_{2,Q}(m_2-1).
 \end{split}
 \tag{TR.38b}
\]
They contain respectively colour 0, colour 1 or 0, and colour 0 or 1. Ordinary fixed-P failed-cutoff factors remain in both baseline gases; they are not themselves relabeled as an inherited Q colour.

For each level put \(\Delta Z_i=\Delta N_i(1)\). The exact normalized difference and its own first jet are
\[
 q_i^F-q_i^A=(Z_i^F)^{-1}
                \{\Delta N_i-q_i^A\Delta Z_i\},
 \tag{TR.38c}
\]
\[
 \begin{split}
 \dot q_i^F-\dot q_i^A
 ={}&\dot{(Z_i^F)^{-1}}
              (\Delta N_i-q_i^A\Delta Z_i)\\
 &+(Z_i^F)^{-1}
    (\dot{\Delta N_i}-\dot q_i^A\Delta Z_i
                          -q_i^A\dot{\Delta Z_i}).
 \end{split}
 \tag{TR.38d}
\]
The dot belongs only to this kernel occurrence, with its original test and its original free coordinates held fixed. A differentiated defect retains the same birth label even where the undifferentiated coefficient happens to vanish. No division by that coefficient is used. Every term on the right therefore still contains a changed colour before absolute values. The inverse jets are the actual normalized same-gas jets, not pointwise estimates of inverse rare masses.

The four complete origins are
\[
 \begin{array}{ll}
 j_M^\eta=q_2^\eta q_1^\eta q_0^\eta\,\dot f,&
 j_0^\eta=q_2^\eta q_1^\eta\,\dot q_0^\eta[f],\\
 j_1^\eta=q_2^\eta\,\dot q_1^\eta[q_0^\eta f],&
 j_2^\eta=\dot q_2^\eta[q_1^\eta q_0^\eta f].
 \end{array}
 \tag{TR.38e}
\]
The test in square brackets is held fixed for the displayed dot. Telescope each product at those same three ordered positions. For example,
\[
 \begin{split}
 j_0^F-j_0^A={}&
 q_2^Fq_1^F(\dot q_0^F-\dot q_0^A)[f]\\
 &+q_2^F(q_1^F-q_1^A)\dot q_0^A[f]
 +(q_2^F-q_2^A)q_1^A\dot q_0^A[f],\\
 j_2^F-j_2^A={}&
 \dot q_2^Fq_1^F(q_0^F-q_0^A)[f]\\
 &+\dot q_2^F(q_1^F-q_1^A)q_0^A[f]
 +(\dot q_2^F-\dot q_2^A)q_1^Aq_0^A[f].
 \end{split}
 \tag{TR.38f}
\]
The M and 1 formulas are the same ordered product identity with the dot at their respective position. Every summand has one normalized difference or one difference of its owned jets, so (TR.38c)--(TR.38d) give a changed colour. This verifies the per-origin cancellation independently of any value-level logarithmic ratio.

Equivalently, use the square-zero algebra with generators
\(\varepsilon_M,\varepsilon_0,\varepsilon_1,\varepsilon_2\) and all products of two generators zero. Assign each original factor and inverse normalizer its owned jet before changing coordinates. Introduce primitive birth fugacities \(\xi_0,\xi_1\), distinct from toggles multiplying an already integrated density correction. Setting both \(\xi_i=0\) gives the entire A family, including each first-jet coefficient. In that algebra the normalized source mean obeys
\[
 G_\xi(0)=1,\qquad
 [t\varepsilon_r]\log G_\xi(t)
       =[t\varepsilon_r]G_\xi(t).
 \tag{TR.38g}
\]
The second equality follows from the first, including its first-jet part. Therefore
\([t\varepsilon_r](\log G_\xi-\log G_0)\) has positive old-colour degree for every \(r\). The primitive component identity, exact inverse-jet rule and CN root deletion preserve that degree and its complete support. The same-valued \(Z_{0,Q}\) or \(Z_{1,QQ}\) occurring inside a newer mass is assigned to the newer kernel in (TR.38a); its derivative is not silently identified with the older inverse-normalizer occurrence.

The source-containing, coloured first-jet series is estimated by the common positive envelopes in Proposition TR.4 before any per-origin absolute sum. Each own kernel jet annihilates 1, so no source-free extensive current is left over to be canceled against another origin. This is the precise first-current content of that proposition. It asserts neither arbitrary off-diagonal Q holomorphy nor an all-orders source theorem.

## 9. What the root result supplies to the combined theorem

First apply Proposition TR.4 to replace only the third auxiliary P by its actual Q, while the first two conditionals retain their fixed P domains. The only moving domains belong to the outer kernel. This gives the actual baseline
\[
 T_{AAQ}F=q_{2,Q}^{\rm analytic\ base}\,q_{1,A}\,q_{0,P}F
 \tag{TR.39}
\]
with the absolute bound (TR.34); the correction is unweighted and bounded by
\(C_LL^{12}b\,e^{-cP_{{\rm aux},3}^2}\). The four separate physical path origins are retained.

For the full inherited density the exact outer kernel is
\[
 q_{2,{\rm full}}(dz_2\mid W)
   =\frac{D_2(z_2,W)\chi_{Q3}(z_2,W)
                  e^{E_2(V_2)}\,dz_2}
          {\int D_2\chi_{Q3}e^{E_2(V_2)}\,dz_2},
 \qquad V_2=\Psi^{(2)}_W(z_2).
 \tag{TR.40}
\]
Here \(E_2=\delta E_{{\rm new},2}+\Delta_2\) is AD's exact two-colour density correction, and \(D_2\) includes the same analytic base as in (TR.39). It occurs once. Every derivative of this occurrence of \(E_2\), and of the denominator in (TR.40), belongs to the new origin 2.

To compare microscopic outputs, use the full lower source mean \(G_{2,{\rm full}}(t;V_2)\), including the intermediate background source, inside
\[
 \int D_2\chi_{Q3}e^{E_2(V_2)}
                         G_{2,{\rm full}}(t;V_2)\,dz_2 .
 \tag{TR.41}
\]
Its normalization is its value at \(t=0\). The baseline uses \(G_{2,AA}\) with no \(E_2\), and its own actual value at \(t=0\). Neither the lower source mean nor the inherited density is replaced by a finite-order Taylor approximation.

The occurrence-level first jets assign the microscopic readout to M, the first conditional and its own inverse normalizer to 0, the middle conditional and its own inverse normalizer to 1, and every factor and normalization in (TR.40) to 2. Equal zero-jet masses may cancel algebraically only after their first jets have been assigned. Each conditional's own kernel jet annihilates the constant test.

Proposition TR.4 supplies the missing microscopic root and joint energy--velocity estimates for the combined same-gas construction. With TC's actual full inherited normalization and NC's joint domain/path identities, the old-colour correction has four-origin unweighted budget
\[
 C_LL^{12}b\,
        \bigl(e^{-cP_0^2}+e^{-cP_{{\rm aux},2}^2}\bigr).
 \tag{TR.42}
\]
This application takes the difference within each physical origin before its absolute sum. It is not a comparison of bare conditional densities by total variation and not an inference from the unmarked size of \(E_2\). The full connected construction must use the actual denominator in (TR.40).

TC and NC supply the actual source checks used in this application. The combined full third-step statement, including its final shared value/first-jet carrier registry, is recorded separately. The present proof supplies its marked analytic input and the explicit normalization/ownership calculus; it does not replace either source certificate with an already integrated old bound.

## 10. Limits

All constants and cover conversions are for three fixed homogeneous native levels. The displayed engineering factor is exactly \(h_3^4/h_0^4=L^{12}\). No summable-in-depth current budget, ambient compact-field extension, complementary P/Q history sector, engineering contraction, or outer-law moment estimate is derived here.

The origins are the amended actual diagonal path origins. Full arbitrary off-diagonal QQ/Q rectangular kernels are not asserted. Elementary finite-current values alone still do not provide the primitive joint path certificate for a fourth step.

The new ingredients beyond the two-level result are the third actual force-and-mismatch background comparison, the third zero-subtracted physical innovation leaf, the complete three-level deterministic trace store, the backward triangular coupling cancellation, and the single distinguished-root passage through three exact normalized gases. The actual inherited unmarked and nested-core inputs remain visibly assigned to TC and NC.
