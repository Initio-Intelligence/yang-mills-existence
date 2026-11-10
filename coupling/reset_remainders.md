# Reset remainders on an admitted Wilson interval

The identification of the cumulative Gaussian marginal with a linear drift up to a uniformly bounded remainder is a separate hypothesis (GC). An arithmetic consequence of that drift does not prove GC or match a prescribed physical endpoint.

**Summary.** The direct contribution of the currently absorbed resets satisfies (D) at arbitrary admitted age, with earlier regular fields held fixed. The fresh reset norm and the numerical renewal step admit repairs. A fractional derivative suffices for the periodic curvature cancellation. The published bulk recursion also permits a different comparison in which only mature resets enter the coupling integral. A conditional reduction of the all-depth problem to one complex single-step estimate for that integral is given below. The single-step estimate on its required domain is not established here. B-03 remains open.

The symbols \(Y_k=g_k^{-2}\), \(\ell_k=\log Y_k\), \(r_k\asymp g_k\ell_k^q\), \(q>p_0\), and the signed pre-exit prefix have the meanings fixed in this chapter. A prefix has a fixed lower ceiling \(Y_k\ge Y_*\), lower linear growth \(Y_i\ge c(Y_k+k-i)\) for \(i\le k\), and upper slope \(Y_i-Y_k\le D_0(k-i)+B\) with fixed constants. These estimates are used as induction hypotheses on the preceding prefix. The last output can be computed provisionally with \(g_n\) before admitting \(g_{n+1}\).

## 1. Fresh reset and the spatial rates

Use the source size \(d_i(X)\), the length of a shortest tree in \(X\) meeting every constituent \(M\)-cube, divided by \(M\). The size controlling shape entropy differs from Euclidean diameter. CMP109 p.257 gives this definition; LFR II (1.67) gives its relative version and distinguishes the \(MR_i\)-based *primed* size after (1.75). Grid periodicity and the units in a contour radius must be tracked separately. The number of rooted connected carriers with \(d_i(X)\le t\) is at most \(C\exp(C_dt)\). A shortest edge tree with \(\le t+1\) edges meets at most \(C_d(1+t)\) cubes, including cubes met just at a vertex. A rooted connected family of \(s\) cubes can be encoded by a depth-first traversal of length \(\le 2(s-1)\) with \(2d\) choices per edge.

Let \(\kappa_s\) be the source exponent in LFR II (1.100), with the source parameters chosen sufficiently large for the rates below. Choose an **estimate** exponent \(\tau=3\kappa_s/4\) and the weight \(\omega=5\tau/4=15\kappa_s/16\). In the following estimates \(\kappa_s\) is kept fixed. For a family on any subdomain of its native domain put
\[
 \|H\|_{\omega,i}^\sharp
  =\sup_{X,U,J}\frac{|H(X,U,J)|e^{\omega d_i(X)}}{r_i^2(1+d_i(X))^2}.
\]
For the newly integrated \(R'\) of (1.100) and the *complete* native \(R^{(i)}\) of CMP119 (2.31), respectively,
\[
 \|R'^{(i)}\|_{\omega,i}^\sharp\le r_i^{-2} e^{-p_0(g_i)},\qquad
 \|R^{(i)}\|_{\omega,i}^\sharp\le r_i^{-2} g_i^{\kappa_0}.
 \tag{1}
\]
Vacuum subtraction costs at most two. Multiplying by any fixed polynomial in \(1+d_i\) costs a constant depending only on that polynomial and the margin \(\kappa_s-\omega\). This proves the reset birth estimate without needing a stronger version of (1.100). In the ordinary T decay statement the choice \((1-10\delta)L/2=3/2\) gives formal output rate \(3\tau/2>\omega\); all source smallness and entropy conditions at \(\tau\) must be imposed when fixing \(L,\kappa_s,\kappa_1,M\). This numerical margin does not imply a derivative of T is bounded between the corresponding spaces. For comparison, a full-derivative estimate uses \(\omega=5\kappa_s/4\) on the input itself. LFR II, printed p.390, (1.99)–(1.101) · CMP119, pp.259–262

## 2. Fractional gain for a periodic curvature quadratic

Write \(h=L^{-(k-i)}\). In the local coordinates of CMP109 (3.30)–(3.34), (4.16)–(4.18) give bounds of sizes \(Qh,Qh^2,Qh^{2+\beta}\) for \(B,\Delta B,\Delta^2B\) with fixed \(0<\beta<1\) and unit forward coordinate differences. The source gives the corresponding estimates for its insertion variation. These are the powers in (RM.3) of Annex AE §10. Use \(Q\le1\). For the curvature expression actually used in CMP119 (3.55)–(3.56),
\[
 F_{\mu\nu}=\Delta_\mu B_\nu-\Delta_\nu B_\mu+i[B_\mu,B_\nu],
 \qquad |F|\le C Q h^2,\quad |\Delta F|\le C Q h^{2+\beta}.
 \tag{2}
\]
Indeed, a difference of the commutator has size \(C Q^2h^3\), and \(h^3\le h^{2+\beta}\). This calculation is in the common gauge of the coordinate calculation. It does not compare Lie-algebra coordinates in unrelated gauges. The bilinear polarization with one insertion obeying the same three inequalities with size \(D\) has bounds \(C QD h^4\), \(C QD h^{4+\beta}\) for the quadratic and its first difference. For example, \(\delta F\) consists of the curl of \(\delta B\) and the two commutators with \(B\). Consequently \(|\delta F|\le C D h^2\), \(|\Delta\delta F|\le C D h^{2+\beta}\). This retains relative smallness \(D/Q\) when an insertion has that reserve.

Suppose a bounded tensor \(C_x\), periodic on a cell of old-lattice side \(P\), has cell mean zero. For any such cell \(H\), put \(W_x=F_x\otimes F_x\) or its polarized variation. Subtract \(W_{x_H}\), a constant tensor, at one point of \(H\). Then, for the unpolarized case,
\[
 \left|\sum_{x\in H}C_x:W_x\right|
 \le C |H|\|C\|_\infty Q^2h^4\min(1,P h^\beta).
 \tag{3}
\]
The two bounds follow from the size of \(W\) and from telescoping \(\Delta W\) along at most \(4P\) links. For the polarized version replace \(Q^2\) by \(QD\). A finite-period compatible torus is tiled by cells. Each old-to-current root count \(h^{-4}\) cancels the four explicit powers. If \(P\lesssim M\ell_i^r\), the ages on which the gain is one number at most \(1+\lceil\log_L P/\beta\rceil\). Thereafter it is bounded by a geometric sequence of ratio \(L^{-\beta}\). Its age sum is \(O(1+\log\ell_i)\), with constants depending on \(M,r,\beta,L\). The onset occurs later than in the full-derivative estimate. The price remains logarithmic. This proves a periodic-tensor estimate. Applying it inside localization requires the marginal tensor of the differentiated activity, its matching Wilson subtraction and the cell grouping with all decoupling variables present. A bound on an unrestricted sum cannot be assigned to its localized pieces after taking absolute values. CMP109, pp.276–277, 285, (4.16)–(4.18) · CMP119, pp.280–283, (3.49)–(3.67)

## 3. An age-sum renewal without a uniform exponential resolvent tail

Here is a sufficient numerical bound for any implementation of that localized transfer. Set \(a=k-i\),
\[
 K_i(a)=C\,[K_0(a)+\min(1,P_i L^{-\beta a})],
 \quad P_i\le C(1+\ell_i)^r,\quad
 K_0(a)\le C(1+a)^t L^{-\epsilon a}.
\]
The index in \(K_0\) denotes a fixed kernel. Assume the insertion prefactor is \(\rho_k\le C\ell_k^{-s}\), \(s>0\). Then on every signed prefix
\[
 \sup_{i\le n}\sum_{k=i}^n \rho_k K_i(k-i)\le\varepsilon(Y_*),
 \qquad \varepsilon(Y_*)\longrightarrow 0.
 \tag{4}
\]
For \(a\le c_0Y_i\) choose fixed \(c_0>0\) with \(D_0c_0<1/4\). The upper slope gives \(Y_k\ge Y_i/2\) at a sufficiently large ceiling. The sum in this range is bounded by \(C\ell_i^{-s}(1+\log(2+\ell_i))\) by (3). For \(a>c_0Y_i\) use \(\rho_k\le C\), then sum \(K_0\) and \(P_i L^{-\beta a}\). The tails are \(O(e^{-cY_i})\) after absorbing fixed powers. Taking the supremum proves (4), including changes of birth grid. This is a small **column sum** of the actual time-dependent majorant. It permits a fresh logarithmic plateau at each generation.

For clarity consider a single immigrant of amplitude \(b_j\le e\), \(M_j\le C e\), its subsequent irrelevant sizes \(b_k\), and absolute scalar mismatch \(M_k\). Suppose one has the nonnegative inequalities
\[
 b_{k+1}\le T_k+C M_k/Y_k,\quad
 M_{k+1}\le (1+C/Y_k)M_k+C T_k,\quad
 T_k=\rho_k\sum_{i=j}^k K_i(k-i)b_i .
 \tag{5}
\]
Summing (5) gives \(\sum_{k=j}^{n-1}T_k\le\varepsilon\sum_{i=j}^{n-1} b_i\). If \(\varepsilon\le1/2\), then
\[
 \sum_{i=j}^{n}b_i\le 2e+2C\sum_{k=j}^{n-1}M_k/Y_k,\qquad
 M_n\le C'e+C'\sum_{k=j}^{n-1}M_k/Y_k.
\]
Discrete Grönwall bounds \(M_n\) and, by the same estimate or a product telescope, \(\sum_{i=j}^n b_i\) by \(C''e\exp(C'\sum_{k=j}^{n-1}1/Y_k)\). For the signed prefix this is \(C'''e(Y_j/Y_n)^{b_*}\) with fixed \(b_*>0\), allowing a fixed additive slack in the harmonic sum. The theorem needs neither a time-translation-invariant kernel nor an exponential tail of its resolvent. It remains conditional on deriving (5) for the appropriate localized objects. A scalar mismatch coefficient at birth which costs a fixed power of \(\ell_j\) introduces the same factor in this bound.

## 4. A shorter comparison in the source’s actual allocation of resets

CMP119 pp.270–272 separates the mature \(R^{(i)}\) which have attained the outgoing lattice symmetry from the recent terms *before* defining the E-producing log integral in (3.28). The separate recent-R interpolation in (3.26) produces \(R''^{(k+1)}\) and boundary terms. Page 279 identifies the coupling subtraction as the projection of the new **E** term. LFR II (1.101) subsequently adds the post-R-operation terms. Thus (1.100) is a bound for the freshly integrated \(R'\). The general input bound for the complete \(R^{(i)}\), including earlier \(R''\) contributions, is CMP119 (2.31). Mature input produces an E birth whose summed density has the full outgoing covariance (3.39)–(3.42). This suggests comparing on the native E recursion directly; it avoids assigning a joint recent-plus-mature T projection to the actual Wilson coefficient.

### A physical estimate for the direct mature-reset contribution

At an admitted step let \(c_{k+1}^{[-R\mid E]}\) be the projected birth with the **same complete incoming E** and its actual earlier subtractions, suppressing only the mature \(R\)-difference in the last log of (3.28). It can be formed as a comparison integral even if no bare theory follows this modified prescription. At the published single-step construction footing, on a signed prefix,
\[
 |c_{k+1}-c_{k+1}^{[-R\mid E]}|
 \ \le C\,Y_k^{\,2-\kappa_0/2}(1+\log Y_k)^C.                 \tag{D}
\]
For \(\kappa_0\ge8\) this is \(O(Y_k^{-3/2})\). The constant is independent of the number of earlier nonzero resets. This is a bound on the direct contribution and uses the actual previously generated regular fields on both sides.

**Proof.** On every retained compatible real flux configuration, (2.44) applied to the old configurations at the two endpoints of the fluctuation difference gives the magnitude of the omitted exponent at most \(2R_1 V_k\sum_{j\in I_k} g_j^{\kappa_0}\), where \(I_k\) is the set of absorbed old indices. Comparison of the two positive real integrals, subtraction at the flat field and division by the outgoing volume give \(m=4L^4R_1\sum_{j\in I_k} g_j^{\kappa_0}\) as a bound for the difference of their vacuum-subtracted log densities. All old E terms, including the reset-induced terms they already contain, cancel from the exponent difference. The real pressure inequality uses no independence assumption.

Here the comparison birth in  needs its *one-step shrinking chart*, not fixed charts for every previous E. Obtain it by using the unrestricted pre-subtraction construction for (23) of that reference a second time. Keep the incoming E, its stored coefficient in each matching Wilson subtraction, \(Y_{\le k}\), its Gaussian, the one-step physical cutoff and every chart unchanged. In the estimates of the preintegration step, the E differences are bounded with their own Wilson cancellation (CMP119 (3.56)–(3.67)). Mature R differences have their own, separately bounded, unsubtracted term (p.276 and (2.44), proof on p.283). Its deletion replaces its majorant by zero. No E counterterm was chosen to cancel any of this omitted R difference. The field maps, integration support and contour construction in the provisional calculation depend on the fixed numerical/geometry inputs. The absolute bounds for \(V\) in CMP116 (1.41)–(1.43) and for the differentiated rooted integrand of (3.37) are therefore still valid after deletion. In the source's connected representation (3.44)–(3.47), this applies both to the distinguished numerator and to the ordinary denominator polymers. The spatial estimate follows by the same positive majorant series. This reasoning compares the **majorants**; individual signed cluster coefficients or actual expectation values need not decrease. Equations (3.39)–(3.42) still give the outgoing covariance since the mature sum and zero both have that symmetry. This is a single calculation using actual incoming data and an unaltered current \(Y_k\). No estimate on a future synthetic E input and no new self-consistent coupling sequence is invoked.

The actual and omission births thus both have the required provisional carrier and local affine-flux disc bounds. The real-to-complex estimate (9) gives \(C a^{-2}m(1+\log(1/m)+\log Y_k)^C\) for \(0<m<1/4\) and \(a\ge cY_k^{-1/2}\). Its proof takes the growing compatible torus limit before the local quadratic projection. The case \(m=0\) is exact. The prefix lower slope bounds \(\sum_{j\le k}Y_j^{-\kappa_0/2}\le C Y_k^{1-\kappa_0/2}\) for \(\kappa_0>2\). Monotonicity of \(x(1+\log(1/x)+\log Y_k)^C\) at sufficiently small \(x\) proves (D), including the case of a much smaller actual \(m\). The constants are in \(Y\) units. This extension of the first-insertion argument leaves \(c_{k+1}^{[-R\mid E]}-d_k^G\) to be controlled. The omitted R inputs at **earlier** steps are encoded in the actual E used on both sides of (D).

### A single uniform complex parameter for the remaining feedback

**One-step proof target.** Let \(\mathcal H_{k+1}(E_{\le k},R_{\rm mat};Y_{\le k})\) denote the canonical homogeneous raw E birth in (3.28), localized by (3.37)–(3.47), before vacuum and Wilson subtraction. Each earlier raw E coefficient is evaluated with its own subtracted vacuum and Wilson projection as in (2.23)–(2.27). Prescribe the actual numerical \(Y_i\), all cutoff choices and the old grids. Define \(H_0(z)\) by the bare state, and recursively define \(H_{k+1}(z)\) by this same operation with old E births \(H_i(z)\), their own vacuum and \(P_i H_i(z)\) subtractions, and mature inputs \(zR^{(i)}\) taken from the **actual** prefix. At each artificial step use the prescribed next Wilson coefficient. This amounts to adding a compensating Wilson counterterm if \(P_iH_i(z)\) differs from its actual value. It makes no claim that synthetic trajectories are physical Wilson measures. At \(z=1\) the compensation vanishes and each raw E birth agrees with the actual homogeneous E birth by induction. At \(z=0\) the formula gives the ordinary E-only map at the same externally specified couplings.

A sufficient test for iteration is the following. For each input of this family through \(k\) satisfying the native bounds (2.26)–(2.29) with a common \(E_0,\kappa_s\), and each amplified mature input satisfying (2.31) at a working exponent \(\nu\), the canonical output must satisfy
\[
 \sup_{(U,J)\in\mathcal U^c_{k+1}(X,\alpha_{0,k+1},\alpha_{1,k+1})}
       |H_{k+1}(X;U,J,z)| \ \le E_0 e^{-\kappa_s d_{k+1}(X)}
 \tag{6}
\]
in the source's anchored convention (with the anchor fixed), jointly holomorphic in \(z\), with the same real cutoff, map parameters and \(E_0\) at every step. A smaller output decay can be used if the input exponent in the ensuing induction is reduced to that same value and is regenerated at each step. The trial final output uses \(g_n\) in the radii. For (6), analyticity at each finite step without a uniform output budget is insufficient.

**Amplification lemma.** Fix a signed admitted prefix through \(n\), and assume complete inputs satisfy (2.31) at exponent \(\nu+D\). It suffices to take fixed \(D>4\) if the eventual spatial readout includes a fixed logarithmic loss. For \(i\le n\), \(g_i\le C_g g_n\). Thus on the disk \(|z|\le A_n=(C_g g_n)^{-D}\), each \(z R^{(i)}\) satisfies the working (2.31) bound \(g_i^\nu e^{-\kappa_s d_i(X)}\), with any fixed source prefactor absorbed into \(A_n\). Size, support, covariance and gauge invariance of these inputs are therefore preserved. If (6) holds for this block operation, induction establishes the native \(E_0\) bound on the **same** disk at every precursor step.

The linear flux projector applied to an \(E_0\)-bounded native E family costs at most \(C r_n^{-2}\): on a nonwinding carrier of tree size \(d\), use its local Cartan disc of radius \(c r_n/[M(1+d)]\), apply second-order Cauchy and sum with the rooted entropy estimate. Winding carriers tend to zero in the thermodynamic projection. Fixed ratios of consecutive \(r_i\) affect only constants. Equivalently one can retain a fixed logarithmic factor in this statement. Normal convergence on smaller parameter disks gives holomorphy of the projected sum. Cauchy coefficients on \(|z|<A_n\) then give
\[
 |P_{n+1}H_{n+1}(1)-P_{n+1}H_{n+1}(0)|
 \le \frac{C r_n^{-2}}{A_n-1}=O(g_n^{D-2}\ell_n^{-2q}).
 \tag{7}
\]
A fixed logarithmic readout factor is absorbed by \(D>4\). This comparison uses a single complex variable throughout the prefix. It buys the powers for the readout once; no new inverse radius is multiplied in at each age. A one-step version with actual incoming E held fixed gives the same difference estimate for just the current absorbed R forcing. The coefficient test follows from (7) if the driven E-only endpoint has the fixed-chart bound \(|P H_{n+1}(0)-d_n^G|\le C/Y_n\) and the stated Gaussian prefix calibration. The even physical-amplitude comparison in  is applicable to E inputs with their own projections and certified fixed physical charts. Uniform availability of those charts for this externally driven recursion must be checked; the previously used comparator has a self-consistent shifted coupling.

**What the references establish about (6).**

- CMP119 pp.270–272, 275–279 gives the canonical bulk operation and the denominator-cancelling cluster expressions. In (3.44)–(3.47) a rooted numerator polymer and disjoint denominator clusters produce a connected local series. Once its input majorants hold on the desired domain, adding a complex scalar parameter to the activities introduces no new denominator estimate: finite polymer coefficients are analytic and normal convergence gives the analytic log branch. Positivity of a synthetic complex measure would be the wrong tool here.
- CMP116 Lemmas 1–2 and §2 give a full native output for pure E with its fixed input hypotheses. The mature R calculation at CMP119 (3.49), (2.44) supplies four old-scale powers without the E Wilson subtraction. Annex AE (RM.5)–(RM.10) proves smallness of those localized primitive R pullbacks on the **reduced** joint contour, with budget \(C g_k^{\nu-11}e^{-\kappa_*d_k(Y)}\). It makes amplification of the *inputs* feasible already at the level of the five-radius and six-summation losses. It does not state (6) on the uniform native output domain for the iterated synthetic E births.
- CMP119 p.262 discusses the inductive map between density spaces, and Theorem 1 explicitly assumes the self-generated coupling array. On the homogeneous region (2.24) also encodes that consistency. For the synthetic array \(Y_i-Y_{i+1}\) and \(P H_{i+1}(z)\) can differ. The formula at \(z=1\) is exact, but a proof of (6) must check where the native E estimate uses that identity, or run the single-step estimates directly with the compensating Wilson term outside the fluctuation integral. The term is not a physical density identity at general \(z\). On the ordinary full cutoff, the synthetic inherited E arguments must all remain within their native domains, with the independently extended current and simultaneous decoupling parameters. Annex AD (E14.46)–(E14.49) maps a reduced output background ball into a larger input ball, which does not supply the same-radius iterative hypothesis. The ordinary-cutoff and contour issue arises before applying the numerical inference (7).
- The parameter order must make the exponent \(\nu+D\) available for the **complete** native \(R^{(i)}\) and the work at \(\nu\) on the same scheme. CMP119 (2.31) permits large fixed exponents with compatible parameter choices. The elementary inequality \(e^{-p_0(g)}\le C_Ng^N\) by itself addresses only the post-R portion (1.100). Applying it to a pre-R \(R''\) born from (3.26) would omit its source of smallness.

Thus (1), (3), the renewal implication (4)–(5), the direct one-step estimate (D), and the implication (6) \(\Rightarrow\) (7) are explicit repairs. In the direct route (6) is the first actual-map bound still to verify. A uniform estimate for the induced E *difference* on an invariant smaller domain with an adequate flux readout would also suffice. The existing window and the coefficient conversion \(d_B=11N^2\log L/(12\pi^2)>0\) remain the established B-03 evidence; the frozen all-age remainder and the separate B-05 matching problem receive no completion credit here. Published small-field localization · Published bulk and mature reset construction ·
