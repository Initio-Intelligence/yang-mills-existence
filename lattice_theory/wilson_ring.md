# Compact Wilson rings and marked holonomy

## Result and relation to R1

A one-dimensional pinned cycle of arbitrary length in the four-dimensional Wilson lattice admits an exact compact-group estimate for its inherited exterior interaction after integration of *all* cycle links. The estimate holds for SU(N), independently varying complex scalar plaquette sources, and independent complex neighborhoods of its matched transverse transports. Small mismatches of the two transverse faces give additional local quadratic terms, bounded in §7. Its constants are uniform in the length and the weak coupling. This advances the fixed compact cycle in Cyclic Patch Obstruction and the Gaussian growing-patch calculation in Uniform Cyclic Gaussian Carriers on the subclass specified below. Section 6 gives a separate geometric check on Mixed R1 Extraction, §6.2. No identification of the ring kernel with a Balaban constrained E/B history is used.

### 1. Actual compact integral

Take a periodic lattice with at least four sites in each direction. In one longitudinal slab integrate direction-1 links at the transverse sites of a straight periodic line in direction 2 of length n. Set all other direction-1 links to the identity. Choose the transverse links independent of longitudinal coordinate. The two direction-2 neighbor plaquettes of each selected link couple it to the two neighboring selected links. The other four incident plaquettes couple it to pinned identity links. The latter actions are all equal to the pin action, with independent source coefficients. Transverse plaquettes lie entirely outside the integral. These are restrictions on the real exterior of a Wilson conditional integral, with no deletion or linearization of its internal Wilson action. Equally, the argument applies to an induced transverse cycle with two internal neighbors and four pinned neighbors per vertex.

Write $a(Q)=1-\operatorname{Re}\operatorname{tr} Q$, with normalized trace. In the literal convention $s=Na, \tau=N\beta_a, z_p=Nj_p, w_p=1-z_p/\tau$. At site i put $b_i=\sum_{p\text{ pin at }i}w_p$ and call the edge weight $u_i$. Independent changes of internal variables by unitary conjugations set all transverse transports along an open spanning path to identity. The remaining edge has holonomy g, the ordered product along the cycle. Haar measure and all pin terms are invariant. Define $Q_{n+1}=gQ_1g^{-1}$. The complete kernel is
\[
 Z_g(w)=\int\prod_{i=1}^n dQ_i\,
  \exp\Big[-\tau\sum_i\{b_i a(Q_i)+u_i a(Q_i Q_{i+1}^{-1})\}\Big]. \tag{1}
\]
In complex variables use $a^{\rm hol}(A)=1-\tfrac12\operatorname{tr}(A+A^{-1})$. The flat-exterior subtraction at the same source weights and its source-dependent remainder are
\[
 D_g(w)=\log[Z_g(w)/Z_I(w)],\qquad
 \Phi_g(z)=D_g(1-z/\tau)-D_g(1). \tag{2}
\]
Thus the zero-source mass $Z_g(1)$ is retained. The vacuum used here is exactly the flat-patch log ratio $\log[Z_I(1-z/\tau)/Z_I(1)]$.

**Theorem.** For fixed N there exist $\tau_*,r,\epsilon,C>0, 0<q<1$, independent of $n\ge4$, such that $D_g(w)$ has a branch extending its real value at $w=1$, holomorphic for $\|w-1\|_\infty<r$ and $g\in SU(N)\exp\{B\in\mathfrak{sl}_N(\mathbb C):\|B\|<\epsilon\}$, chartwise in g, whenever $\tau\ge\tau_*$. It satisfies $|D_g(w)|\le C q^n$ there. For real $g\in SU(N)$ the sharper bound is $Cq^n a(g)$. In particular, for $m\ge1$,
\[
 |D_z^m\Phi_g(0)[f_1,\ldots,f_m]|
 \le C q^n a(g) m! (C'/\tau)^m \prod_i\|f_i\|_\infty . \tag{3}
\]
Here f are directions of the normalized plaquette source z, and physical directions of j insert the additional factor $N^m$. For the single holonomy, this complex tube is expressed after fixing the path. The separate-link version below admits independent changes on all n matched transverse transports. Length suppression holds also for winding carriers with nontrivial flat holonomy, for which there need not be local exterior curvature on a spanning disk.

### 2. Compact transfer estimates

For a seam-free edge let $K_i$ be the integral operator on $L^2(SU(N),dQ)$ with kernel
\[
 \exp[-\tau\{b_i a(X)/2+u_i a(XY^{-1})+b_{i+1}a(Y)/2\}]. \tag{4}
\]
Let K denote the homogeneous operator at w=1. For the seam replace $XY^{-1}$ by $XgY^{-1}g^{-1}$ in the last kernel, calling it $K_{n,g}$. Direct kernel multiplication gives $Z_g=\operatorname{Tr}(K_1\cdots K_{n-1}K_{n,g})$, including nonconstant weights. Cutting the product at any vertex gives the actual partial Haar integrations and the correct residual endpoint variables.

Let $\lambda_\tau$ be the largest eigenvalue of K. It is simple with a positive normalized eigenfunction $e_\tau$. All kernels without the seam commute with simultaneous conjugation acting on functions of one group variable. In particular $e_\tau$ is a class function. Write $A=K/\lambda_\tau$. Uniformly for $\tau\ge\tau_*$, for constants $C$ and $\rho<1$,
\[
 \lambda_\tau\asymp\tau^{-d/2},\quad d=N^2-1,\quad
 \|A\|_{\rm HS}\le C,\quad \|A|_{e_\tau^\perp}\|\le\rho. \tag{5}
\]

Here are details of the uniform gap. In a fixed exponential neighborhood of identity set $X=\exp(x/\sqrt\tau)$ in anti-Hermitian coordinates of norm squared $-\operatorname{tr}(x^2)$. The unitary rescaling of Haar $L^2$ uses the square root of its coordinate Jacobian. After multiplying K by $\tau^{d/2}$ the rescaled kernel, extended by zero outside the rescaled chart, converges in Hilbert–Schmidt norm on Euclidean space to
\[
 c_N\exp[-\tfrac32(|x|^2+|y|^2)+\langle x,y\rangle]. \tag{6}
\]
Indeed $a(\exp X)=|X|^2/2+O(|X|^4)$, the real edge action is nonnegative, and the two pin factors give an integrable squared Gaussian majorant on the chart. The part of the compact operator with either endpoint outside the fixed chart is $O(\tau^{d/2}e^{-c\tau})$ in rescaled Hilbert–Schmidt norm. Thus embedding the chart and appending zero on its complement preserves the convergence needed for the first two singular values. The limiting Gaussian operator has a simple largest singular value with a strict gap. For example Mehler's formula diagonalizes (6) in a rescaled Hermite basis with successive degree ratios $3-\sqrt8<1$. Alternatively its compact square has a strictly positive kernel, so the Perron eigenvalue of its square is simple. The same strict positivity holds for K and its square. Singular-value continuity gives (5), including a uniform gap in *absolute* eigenvalue. These estimates use the Gaussian solely to prove uniform spectral separation of the exact compact transfer.

Normalize $A_i=K_i/\lambda_\tau, A_{n,g}=K_{n,g}/\lambda_\tau$. For small source radius r, $\|A_i-A\|_{\rm HS}\le C r$. To see this directly, the changed exponent is bounded in modulus by $Cr\tau[a(X)+a(Y)+a(XY^{-1})]$. In the difference of exponentials preserve half the real homogeneous coercivity and absorb the remaining polynomial factor. Integrating the two pin Gaussians gives the stated Hilbert–Schmidt bound after division by $\lambda_\tau$.

On a fixed small complex tube about the real g family one also has $\|A_{n,g}\|_{\rm HS}\le C$ uniformly. For $g=g_0e^B$, the variation of the seam action from $g_0\in SU(N)$ is bounded by
\[
 C\|B\|\,\|X-I\|_{\rm HS}\|Y-I\|_{\rm HS}. \tag{7}
\]
Indeed in the trace $\operatorname{tr}(XgY^{-1}g^{-1})$ the constant and the terms linear in either $X-I$ or $Y^{-1}-I$ are independent of g. Apply the same argument to the inverse trace and use that X,Y are unitary. Formula (7) is absorbed in the two pin energies; $a(X)=\|X-I\|_{\rm HS}^2/(2N)$ with unnormalized Hilbert–Schmidt norm. This proves the uniform analytic seam estimate and, on smaller tubes, its fixed-order derivatives. For real g the seam kernel is $K_n$ composed with a unitary conjugation, up to the orientation of that conjugation. With $P$ the orthogonal projection onto all class functions it follows that
\[
 P(A_{n,g}-A_n)=(A_{n,g}-A_n)P=0. \tag{8}
\]
The identity extends to the complex tube by the identity principle applied in Lie algebra coordinates to matrix elements. Every $A_i$ commutes with P by Haar averaging. Consequently its operator norm on $P^\perp$ is at most $\rho+Cr$, since $e_\tau\in\operatorname{ran}P$.

### 3. Lower bound for the inhomogeneous flat trace

A zero-free denominator is needed for complex sources on arbitrarily many plaquettes. Comparing each perturbed product to the homogeneous trace by a sum of n errors would give a radius shrinking with n. Instead put $\delta=Cr$ for the error bound above and set $a_0=1-2\delta, b=(1+\delta)(\rho+\delta)$. Shrink r so that $\rho+\delta<a_0$ and $b<a_0^2$. On the complex cone $s e_\tau+v, v\perp e_\tau, \|v\|\le|s|$, the new leading coefficient obeys $|s'|\ge a_0|s|$ while $\|v'\|\le(\rho+2\delta)|s|$. Shrink r so that $\rho+2\delta\le a_0$. This proves cone invariance for every $A_i$.

For $S=A_1\cdots A_n$, iterating the same product on the cone shows $r_{\rm spec}(S)\ge a_0^n$ by the spectral-radius formula. A compact operator with nonzero spectral radius has an eigenvalue $\lambda$ attaining it. Exterior-square estimates give
\[
 \|\wedge^2 S\|_1\le C b^{n-2}. \tag{9}
\]
Indeed the two largest singular values of $A_i$ are at most $1+\delta,\rho+\delta$. Its exterior square has operator norm at most b and Hilbert–Schmidt norm at most $\|A_i\|_{\rm HS}^2/\sqrt2$. Use two Hilbert–Schmidt factors and n−2 bounded factors. The eigenvalues of the exterior square include the products of pairs of nonzero eigenvalues of S, with algebraic multiplicities (restrict to their finite-dimensional generalized eigenspaces and triangularize). The sum of absolute eigenvalues is bounded by trace norm, also for a nonnormal operator. Therefore the sum of all other absolute eigenvalues of S is at most $Cb^{n-2}/|\lambda|$. The trace formula for trace-class operators gives
\[
 |\operatorname{Tr}S|\ge a_0^n/2 \tag{10}
\]
for all sufficiently large n, uniformly. Equivalently all trace and exterior-power estimates here follow first for conjugation-adapted finite-dimensional compressions containing $e_\tau$, then by Hilbert–Schmidt approximation for fixed n. This latter route only needs finite-dimensional triangularization and trace-ideal inequalities.

### 4. Twist and source derivatives

By (8), the twisted-minus-flat trace has support in $P^\perp$ in the transfer space. Use one seam Hilbert–Schmidt factor, one other Hilbert–Schmidt factor and the remaining n−2 operator norms on this subspace to obtain
\[
 |Z_g(w)-Z_I(w)|\,\lambda_\tau^{-n}\le C(\rho+\delta)^{n-2}.
 \tag{11}
\]
Dividing by (10) gives a bound $C q^n$ for the deviation of the ratio from one with $q=(\rho+\delta)/a_0<1$. For sufficiently large n it is less than $1/2$, so the analytic branch of the logarithm with its real value at $w=1,g\in SU(N)$ obeys the same bound.

For the finitely many smaller n, at real g and $w=1$ restrict each variable in (1) to a ball of radius $c/\sqrt\tau$. Every pin and edge action in that region is $O(\tau^{-1})$ including the twisted edge. Its Haar volume per variable is at least $c'\tau^{-d/2}$, uniformly in g. Thus $Z_g(1)/\lambda_\tau^n$ and the flat expression have strictly positive lower bounds for this finite set of lengths. The Hilbert–Schmidt estimates and (7) allow common smaller tubes for w and g with positive real part for both normalized traces (telescope the bounded number of factors). The logarithms on these tubes are uniformly bounded. Increasing C restores $Cq^n$ also for these lengths.

The logarithm is a holomorphic class function of the single seam g by simultaneous conjugation of all Q. At $g=I$ it vanishes. Its derivative there is an adjoint-invariant linear form on the semisimple Lie algebra and hence zero. Uniform Cauchy bounds on the g tube imply $|D_{\exp B}(w)|\le C q^n\|B\|^2$ near identity. On the real group this gives $Cq^n a(g)$ there, and away from identity compactness gives the same inequality by the previous bound. Finally Cauchy in independent source directions on the fixed w polydisk, with parameter radii $r\tau/(2m\|f_i\|_\infty)$, yields (3) by $m^m\le e^m m!$. This includes coincident insertions and derivatives of the logarithm of the *joint* actual integral.

**Independent transverse links.** Keep a transport $T_i$ in each edge in (4), giving $A_{i,T_i}$. Choose each $T_i=T_i^0 e^{B_i}$, with $T_i^0\in SU(N)$ arbitrary and $\|B_i\|<\epsilon$ independently. The argument of (7), with the extra factor $\|B_i\|$, bounds $\|A_{i,T_i}-A_{i,T_i^0}\|_{\rm HS}\le C\epsilon$. Indeed one can integrate along the path of deformations, absorb $\tau\|X-I\|\|Y-I\|$ in the pin energies, and divide by $\lambda_\tau$. For each real $T_i^0$ its conjugation in the transfer is unitary. Hence (8) gives exact equality of the two products on $\operatorname{ran}P$ and $\|A_{i,T_i}|_{P^\perp}\|\le\rho+C(r+\epsilon)$. On $P^\perp$ bound the original and flat traces separately by two Hilbert–Schmidt norms and $n-2$ contracting norms. After shrinking $r,\epsilon$ to ensure $\rho+C(r+\epsilon)<a_0$, equation (10) gives $|\log(Z_{\bf T}/Z_I)|\le C q^n$, with possibly enlarged $q<1$, on all independent tubes. For bounded $n$, the ball lower bound in §4 is uniform in the n independent real transports since conjugation preserves the distance to identity on every edge. Telescoping once per edge around its own real center gives a common zero-free neighborhood for these finitely many lengths. For real transports the conjugation reduction in §1 gives the stronger factor $a(g)$ with $g$ their ordered product. Separate complex tubes allow the complex product to travel beyond a fixed chart. The estimate uses the actual edge kernels throughout.

### 5. What can be inserted into an induction

For this one compact family the boundary interaction left after n exact integrations is (2). All pinning weights and seam-edge weights can carry different values. A physical radius independent of n and $\tau$ is included, and the stronger scaled radius in (3) holds on this pinned exterior family. The separate-link tube applies to matched transverse faces. Unequal transverse faces and nonidentity pin staples introduce forces. Section 7 admits those forces on their thermal scale and states their additional cost. The map (1) carries no axial selectors or Balaban old/current minimizer. Consequently the result is an interacting inherited readout for an explicit Wilson conditional patch, and the unrestricted kernels in (MR.27) remain open.

### 6. Raw ownership at the first boundary

B119 (1.20), p.251, places $\Lambda_1$ inside the two-layer erosion of $\Omega_1$, before filling small components of its complement by rectangular hulls. Filling increases $Z_1=\Lambda_1^c$. Thus the original group region $\Omega_1^c$ is surrounded inside $Z_1$ by a two-block buffer. A physical plaquette or a based clover meeting that original region on a literal raw bond has diameter at most two fine spacings in the maximum norm. With $LMR_1$ fine spacings per block and the admitted large M, its support lies in a single wall-connected component of $Z_1$: the block containing a point of intersection and its one-block neighborhood already contain the entire support. This is a geometric statement at birth. Some of its other links can lie in the fluctuation coordinates of (1.12)–(1.26); geometry cannot turn them into original Haar variables.

A tempting stronger assertion would infer a full block of distance between arbitrary different components of a block union. B109 p.257 defines a localization domain using successive cubes sharing a wall. Two diagonally opposite blocks in a transverse plane have no common wall, even though their closures intersect. A plaquette enclosing their common corner can have opposite vertices in the two blocks. Under the incident-bond convention all four links then touch these two blocks. This tests the inference from wall adjacency alone. It is not a construction of an allowed unbuffered R history. B119 p.247 surrounding (1.9) uses bonds with at least one endpoint in the indicated set, with the displayed deleted distinguished bonds. LFR II pp.378–379, (1.71)–(1.72), factors simultaneous old operations by actual components of Z. The ten-layer enlargement used in the no-new-birth case is described on p.384, and (1.84) on p.386 describes the merger argument, whose graph joins touching or intersecting domains. Neither the abstract wall-adjacency argument nor the initial raw buffer proves the source image after a historical regular integration or reconstruction. Physical intercomponent **effective** sources can persist even when the original support occupied one component.

The primary sources for this distinction are B119, pp.247 and 251, B109, p.257, and LFR II, pp.378, 384 and 386. The full mixed target still requires the already integrated complementary density and its two jets on their actual domains, the contact and dimension-four projections, and the invariant norm for their repeated use.

### 7. Thermal mismatches of the actual exterior faces

For a shared plaquette of the same cycle, write its literal action as $a(X A_i Y^{-1} B_i^{-1})$. The two transports $A_i,B_i$ are the actual exterior links on the two longitudinal faces. On the near-matched real region write
\[
 A_i=e^{D_i/2}T_i,\qquad B_i=e^{-D_i/2}T_i,\qquad D_i=\log(A_i B_i^{-1}).
\]
Each single-site plaquette gives $a(Q_i C_{i,p})$ after orientation, with the actual three-link staple $C_{i,p}=e^{D_{i,p}}$ near identity. For a pin on a negative edge this formula also follows by using invariance under reversal and cyclic permutation. No assumption of independence of these staples in the Wilson exterior is needed. Any external configuration yielding such coefficients is included. The integral has one shared action per edge and four single-site actions per vertex, with the same literal weights as above. Write it as $Z_{{\bf T},{\bf D}}(w)$. The flat comparison at the same weights is $Z_{{\bf I},0}(w)$.

Let $\eta_i=\sqrt{\tau}\max(\|D_i\|,\max_p\|D_{i,p}\|)$. There are constants $c,C>0$, $q<1$ uniform in $n,\tau$ on the interval above such that for all $\eta_i<c$, for the independent near-unitary complex $T_i$ tubes, and the fixed $w$ polydisk, one has
\[
 \left|\log\frac{Z_{{\bf T},{\bf D}}(w)}{Z_{{\bf T},0}(w)}\right|
      \le C\sum_i\eta_i^2,\qquad
 \left|\log\frac{Z_{{\bf T},{\bf D}}(w)}{Z_{{\bf I},0}(w)}\right|
      \le C\sum_i\eta_i^2+Cq^n. \tag{12}
\]
For real transports replace the last term by $Cq^n a(\prod_i T_i)$, with consistent cycle ordering. The first variation in all mismatch parameters at zero vanishes. Each local contribution in the proof has an exponentially localized representation in the site index. The source-dependent part of each logarithm in (12), obtained by subtracting its value at $w=1$, has order-$m$ jets bounded by the displayed right side multiplied by $m!(C'/\tau)^m\prod_i\|f_i\|_\infty$. This is an extensive energy cost for many thermal mismatches. Only the matched-face winding interaction has pure length suppression.

**Transfer estimates and parity.** Replace the two half pin energies in (4) by the corresponding weighted sums of the actual pin actions divided by two, keeping both halves associated to the same vertex. Use the actual shared edge action above. Denote the resulting transfer, divided by $\lambda_\tau$, by $M_i$. For bounded near-unitary $T$ one has
\[
 |a^{\rm hol}(X e^{D/2} T Y^{-1}T^{-1} e^{D/2})
    -a^{\rm hol}(X T Y^{-1}T^{-1})|
 \le C\{\|D\|(\|X-I\|+\|Y-I\|)+\|D\|^2\}. \tag{13}
\]
Taylor's formula in $D$, bounded matrix multiplication on the stated domain, and tracelessness give this inequality: the first derivative at $X=Y=I$ vanishes, the first derivative varies Lipschitzly in $X,Y$, and the second derivative is uniformly bounded. The same proof gives the pin bound with $Y=I$. Consequently for complex parameters of the indicated sizes, the change of exponent on an edge due to mismatches is bounded by $C[\eta(\sqrt\tau\|X-I\|+\sqrt\tau\|Y-I\|)+\eta^2]$, with $\eta=\max(\eta_i,\eta_{i+1})$. The pin weights in the real reference kernel absorb this by the Gaussian inequality. In the difference of the two exponentials retain the prefactor $\eta$ and integrate the Gaussian times a fixed polynomial as in §2. This gives
\[
 \| M_i-A^{(0)}_{T_i^0}\|_{\rm HS}\le C(r+\epsilon+\max(\eta_i,\eta_{i+1})), \tag{14}
\]
where $A^{(0)}_{T_i^0}$ is the homogeneous, real transported kernel. Holomorphy on the product tubes follows by the same domination. The homogeneous transported operator fixes $e_\tau$ on both left and right and contracts its orthogonal complement by $\rho$.

Let $J$ on transfer functions be induced by $X\mapsto X^{-1}$. Then $Je_\tau=e_\tau$ by invariance and the simple top mode. On the edge, replacing the internal variables by their inverses and swapping $A_i,B_i$ leaves the action unchanged: the trace of $X^{-1}B_i Y A_i^{-1}$ is the trace of the inverse of $X A_iY^{-1}B_i^{-1}$ by cyclicity, and $a^{\rm hol}$ is inversion invariant. On a pin the same statement interchanges $C$ and $C^{-1}$. Thus $J M_i({\bf D})J=M_i(-{\bf D})$, including complex $w,T,D$. This is simultaneous sign reversal. Cross terms between different mismatches may occur.

**Local logarithm of the cyclic product.** Let $\delta$ be the uniform right-hand side of (14) and reduce $r,\epsilon,c$ so $\delta$ meets the cone and exterior-square requirements in §3. On the unit ball of $e_\tau^\perp$, put
\[
 c_i(v)=\langle e_\tau,M_i(e_\tau+v)\rangle,\qquad
 F_i(v)= (I-|e_\tau\rangle\langle e_\tau|) M_i(e_\tau+v)/c_i(v).
\]
Use the scalar product linear in its second argument. Then $|c_i(v)-1|\le 2\delta$, and the cone estimate gives $\|F_i(v)\|\le1$. Subtracting the two fractions, or writing their difference as the numerator difference minus $F_i(v')$ times the denominator difference, shows that $F_i$ is Lipschitz with constant $\theta=(\rho+2\delta)/(1-2\delta)<1$. In fact the component of $M_i$ from $e_\tau^\perp$ to the leading row has norm at most $\delta$. Iterating from zero, with indices interpreted periodically, gives unique periodic vectors $v_i=F_i(v_{i+1})$, holomorphic by uniform convergence. They yield a product eigenvalue $\Lambda=\prod_i c_i(v_{i+1})$ of modulus at least $a_0^n$. The exterior-square proof (9) applies unchanged since the reference singular values are the same as those of A. It gives
\[
 \log[Z_{{\bf T},{\bf D}}(w)/\lambda_\tau^n]
       = \sum_i \log c_i(v_{i+1}) + E_n,\qquad |E_n|\le C q_1^n,\quad q_1<1. \tag{15}
\]
For large n, define $E_n=\log[Z/(\lambda_\tau^n\Lambda)]$ by the disk about one: the sum of the other absolute eigenvalues relative to $|\Lambda|$ is bounded by $C b^{n-2}/a_0^{2n}$. One can also prove this by finite-dimensional compression as in §3, since the cyclic fixed point is the limit under norm approximation. For bounded n, at the real matched reference with $w=1$ every homogeneous transported factor fixes $e_\tau$ and $\Lambda=1$. The actual positive ball lower bound of §4 is uniform in independent real $T_i^0$. Telescoping the finitely many factors using (14) and bounding $\prod c_i$ close to 1 gives a common positive-real-part chart for the ratio and a bounded $E_n$ there. Increase C to obtain the geometric bound for those lengths. These definitions choose the real branches at the real source-zero references. The $n$ site logarithms use the fixed disk about 1.

For clarity define $L_{i,d}=\log c_i(F_{i+1}\cdots F_{i+d}(0))$ for $d\ge0$, with the empty composition at zero. The difference for successive d is bounded on the product domains by $C\theta^{d-1}$ for $d\ge1$, and $|L_{i,0}|\le C$. Each such term depends only on the edges or sites indexed from $i$ through $i+d+1$, allowing periodic repetitions. The parity just proved implies the same simultaneous sign reversal invariance for $L_{i,d}$, since $F_i(-{\bf D})(Jv)=JF_i({\bf D})(v)$ and $J0=0$. The remainder $E_n$ is even as well. Choose the final c at most one quarter of an admissible analytic mismatch radius $c_{\rm out}$. For each local term, scale all its participating $D$ by a single complex number t. On $|t|\le c_{\rm out}/(2\max_{j\in[i,i+d+1]}\eta_j)$ its uniform bound still holds. Cauchy's formula and evenness imply that its difference between t=1 and t=0 is at most its preceding sup bound times $C\max_{j\in[i,i+d+1]}\eta_j^2$. Terms with zero maximum have zero difference. For each d, summing this maximum squared over i costs at most $(d+2)\sum_i\eta_i^2$; the geometric series over d converges. The same argument for $E_n$ bounds its change by $Cq_1^n\max_i\eta_i^2$. This proves (12), the exponential localization claim, and by the earlier source Cauchy estimate its full marked version. No conditioning on a rare-history denominator or replacement of the source by a centered observable occurs.

### 8. Arbitrary real face mismatches and positive real weights

The same compact family admits an additional real comparison without any small-mismatch restriction. For all real transports and pin staples, choose anti-Hermitian traceless logarithms $D_i$ and $D_{i,p}$ as in §7. Such logarithms exist by unitary diagonalization and adjustment of eigenangles by integer multiples of $2\pi$. Set $d_i=\max(\|D_i\|,\max_p\|D_{i,p}\|)$. For real weights $|w_p-1|<r$, the full conditional partition satisfies
\[
 -C q^n a(g)-C\tau\sum_i d_i^2
 \ \le\ \log[ Z_{{\bf T},{\bf D}}(w)/Z_{{\bf I},0}(w)]
 \ \le\ Cq^n,\qquad g=\prod_i T_i . \tag{16}
\]
The upper bound is independent of the magnitude and number of frustrated exterior faces. The lower estimate uses the indicated mismatch cost; logarithms minimizing the norm can be chosen. Real weights include positive inhomogeneous couplings. Formula (16) concerns values of the pressure. Its derivation supplies no corresponding zero-free complex source radius on general large-mismatch exteriors.

**Upper estimate.** Regard each selected pin as an edge with its other endpoint fixed, and take two real assignments $A=(A_e)$ and $B=(B_e)$ on all edges. For a pin with prescribed staple $C$, for example choose $A_e=C,\ B_e=I$ and orient the edge outwards. Put $h_p(U)=\exp[-\tau w_p a(U)]$. This central function is positive definite: $\operatorname{Re}\operatorname{tr} U$ is the average of the normalized fundamental character and its conjugate; products of normalized characters are positive definite by tensor products, and the exponential has nonnegative series coefficients. The full product
\[
 k(A,B)=\prod_{e}h_e(A_eB_e^{-1})
\]
is a positive-definite kernel on assignments. For $Q=(Q_i)$ at internal vertices, fixing $Q=I$ at pins, the action $A_e\mapsto Q_xA_eQ_y^{-1}$ preserves this kernel when applied to both arguments, by conjugation invariance. For completeness form the span of formal evaluation vectors $v_A$ with scalar product $k(A,B)$, quotient out its null space, then complete. This gauge action is unitary on that space. It is strongly continuous on evaluation vectors since $k$ is continuous, hence on their span and closure. Averaging over normalized Haar of $G^n$ gives an orthogonal projection $\Pi$. Its Gram kernel is exactly the compact Wilson integral
\[
 Z(A,B)=\int k(Q\cdot A,B)dQ
       =\langle\Pi v_A,\Pi v_B\rangle.
\]
Consequently $Z(A,B)\le [Z(A,A)Z(B,B)]^{1/2}$. Both diagonal integrals have the matched form of §1 with the same weights and comparison $Z_{{\bf I},0}(w)$; pin factors are independent of their matched transport. Apply the matched upper bound at each diagonal. This proves the right side of (16).

**Lower estimate.** Denote by $S_t$ the full weighted Wilson action before multiplication by $\tau$, with all $D$ multiplied by the same real number $t$. The reference $S_0$ uses the midpoint transports $T_i$ and flat pin staples. Its probability measure is invariant under simultaneous inversion of all internal variables. The first derivative $S'_0$ changes sign under this inversion by §7, so its mean is zero. For all $0\le t\le1$ all matrix factors are unitary, and differentiating the real traces twice yields $|S_t''|\le C\sum_i d_i^2$. This uniform bound uses only the fixed number of factors in each individual plaquette and the upper bound on the real weights. Taylor integration thus gives $\mathbb E_0(S_1-S_0)\le C\sum_i d_i^2$. Jensen yields
\[
 \log (Z_{{\bf T},{\bf D}}/Z_{{\bf T},0})
     =\log\mathbb E_0 e^{-\tau(S_1-S_0)}
     \ge -C\tau\sum_i d_i^2 .
\]
The matched lower bound in §4 finishes (16). This step uses the actual normalized conditional law solely to compare its two partition values; the original mass remains in the ratio identity.

**Remaining R1 estimate.** Equations (12) and (16) apply to an unconstrained Wilson conditional integral on a transverse cycle. The full R1 step still requires bounds on the complementary old densities in (MR.27) after earlier constrained regular integrations, including their mixed products with literal marks, their complex endpoint images and locality, and their field and contact projections in an invariant multiscale norm. Neither the uniform thermal-domain jets nor the arbitrary-real pressure comparison supplies that mixed-history estimate.

### 9. Applying the bound to the complementary marked operator

Fix real outer fine variables $v$ for the pin-cycle conditional law, and let $\mu_{0,v}$ be its normalized source-zero law. Write $V_f$ for the *literal* linear physical plaquette insertion. If the frozen transformation also retains variables or history labels $h$, represent their complete positive, source-independent transition by $H(dh\mid Q,v)$. Denote by $\kappa_0(dh\mid v)$ the induced law. The unnormalized conditional source measures, in two source directions, satisfy the exact identity
\[
 \frac{\int e^{\lambda V_f+\mu V_g}\mu_{0,v}(dQ)\,H(dh\mid Q,v)}
      {\kappa_0(dh\mid v)}
 = A(\lambda,\mu;v)\,\ell(\lambda,\mu;v,h),\quad
 A=\mathbb E_{0,v}e^{\lambda V_f+\mu V_g},\quad
 \ell=\frac{d\kappa_{\lambda,\mu}}{d\kappa_0}. \tag{17}
\]
Here the quotient on the left means Radon–Nikodym derivative with respect to $\kappa_0$ and $\kappa_{\lambda,\mu}$ is the law of $h$ under normalized source tilt before transformation. The displayed formula holds almost everywhere, for finite real or complex sources near zero, and can equally be tested against bounded functions without using ratios. Any deterministic source subtraction multiplies $A$ by its compensating exponential. Already at first order the extra term is
\[
 \ell_f=\mathbb E_0(V_f\mid v,h)-\mathbb E_0(V_f\mid v).
\]
At mixed order one has $\ell_{fg}=\mathbb E_0(V_fV_g\mid v,h)-A_{fg}-A_f\ell_g-A_g\ell_f$, with all jets evaluated at zero. The ring bounds estimate the first factor after its stated flat subtraction. They do not estimate these extra label scores. The identities concern complete positive real transformations; they do not postulate that an arbitrary individual complex history is a probability kernel.

A limited positive statement survives on the actual first mixed step. For one original plaquette $p$ whose regular variables have been integrated in B119 (1.26), take the unprojected source by inserting $s_p$ *inside the real integral* before that integration, pulling back the actual source by the same real coordinate changes. Its ratio $b_p$ to the unmarked positive integral is between 0 and $2N$ wherever the mass is positive; the marked submeasure vanishes where it is zero. Composition with a subsequent positive real old kernel gives $0\le T'_{k,r} b_p\le2N T'_{k,r}1$ when the inherited density is represented relative to that mass. Equivalently compose the two unnormalized positive measures and use $0\le s_p\le2N$ before composing. For two original plaquettes the corresponding undifferenced mixed density bound has constant $(2N)^2$. This retains the compulsory mass and survives nontrivial conditioning. It is a real estimate on individual unprojected marks. Summing its absolute values costs the full count of fine anchors. The regular flat/dimension-four subtractions and the subsequent decomposition into E and B have signed coefficients, so it does not identify their complementary density jets with $b_p$.

The first failing operation can be seen before any estimates of Schur kernels or transfer spectra. B119 (1.12) fixes coarse block observables and an axial gauge. Equations (1.21)–(1.22), p.251, change a boundary bond using the background correction $H_{1,\Lambda_1}$. The regular fluctuation integral (1.26), p.253, includes the selector $\chi^{(0)}$, the constrained fluctuation field $CA$, and a term coupling boundary data to the fluctuating field. Its subsequent logarithm is split into localized clusters, and the flat and Wilson projections are taken in the regular sector. These operations keep data depending on individual integrated links, whereas (1) integrates those links without fixing their coarse readout. At the receiving end, LFR II (1.71), pp.378–379, retains the local axial-gauge delta function, characteristic functions and the older operation $T_h$. Equation (1.72) also retains history-dependent intercomponent interactions. Changing the order of the ring integrals gives (17) with the same required $\ell$; dropping that factor changes the actual retained measure. Even a real thermal estimate on the face data provides no complex continuation of the reconstructed and already projected readout inside $T'_{k,c}$.

Accordingly, Mixed R1 Extraction, §§6.1–6.3 still requires the actual $T'_k B_f$ and $T'_k(V_fB_g+V_gB_f+B_{fg})$, including their intercomponent carriers. The specific missing estimate here is a complex-domain bound for the retained conditional scores after the prescribed projections, with locality at their old/current endpoints. A complete positive history sum, an independently centered ring source, or a larger geometric collar does not furnish that bound.
