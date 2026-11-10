# Interior response integrated over the Wilson exterior

For the three disjoint \(SU(2)\) scalar stencils in the corresponding estimate, the positive rational first correction survives as a **specified summand** after removing the near-flat collar conditioning. Its error is \(O(\beta^{-2})\) under the full periodic Wilson measure. The other summand includes the normalized conditional means and the source-dependent motion of the classical minimum. It can contribute at the same order. All distances in the first three sections are fixed in lattice units. The estimate is uniform over even cubic sides \(n\ge12\) in the compact reserve class \(\sup\log(1+\beta)/n<\infty\), with \(\beta=2Nx_0\) and \(N=2\). No trajectory or operator matching is assumed. Earlier seven-link calculation, §5 · Rectangular reserve, (1)

## 1. Typical visible fields and the actual normalized conditional integral

Let \(I\) comprise the seven outgoing spatial 1-links at \(je_0\), \(0\le j\le6\). Observe \(Y_i=\beta a^4 w_a(t_i e_0+e_2)\), \(t_i=0,3,6\); \(i=1,2,3\) labels the three stencils, including all four-vertex weights. Condition on all other links with their unmodified Wilson marginal \(\mu_{\rm ext}\). Only the exterior bonds of the incident plaquettes and three stencils are needed in the normalized conditional source integral. Add a fixed finite connected **exterior** forest of paths to put these bonds in one rooted tree gauge. Such paths exist inside a fixed lifted box: bypass each missing live 1-link by three exterior links around its positive \(12\) plaquette. Enlarge the fixed collar by this routing and choose a tree therein. All loops used below are contractible in this lift. The gauge changes only the coordinates of integration of the seven live links, with unit Haar Jacobian.

Write \(b\) for the logarithms of non-tree visible links on a sufficiently small neighborhood of the flat collar. They are the logs of the corresponding fundamental loop holonomies transported to the same root. For the original compact Wilson field, each loop is an ordered product of a fixed number of unitarily conjugated elementary plaquettes/inverses in a bounded filling. The filling may use live links; the loop itself is exterior measurable. Hence its distance to identity is at most the sum of the plaquette distances. Since \(\|1-U_p\|_{\rm HS}^2=2s_p\), (1) of the reserve gives, with constants depending on the chosen finite collar,
\[
 \Pr(G^c)\le C e^{-c\beta},\qquad
 \|\mathbf 1_G |b|^k\|_{L^p(\mu_{\rm ext})}
 \le C_{p,k}\beta^{-k/2} \quad(p,k\text{ fixed}).                 \tag{1}
\]
Here \(G\) is a fixed, simultaneous, sufficiently small real chart for these loops. The tree-gauge condition uses no orientation constraint on the Haar marginal.

Denote the conditional log generating function by \(W_b(t)=\log\mathbb E[\exp(\sum_i t_iY_i)\mid{\rm ext}]\). On \(G\), let \(S(t,b,u)\) be the exact local Wilson action of the incident plaquettes minus \(\sum_i t_i a^4w_a\), with all visible-only contributions in the sources retained. Choose \(|t_i|\) small once. At \(b=0,t=0\) the unique flat minimum is the identity and its Hessian is the positive tridiagonal matrix of the corresponding estimate tensored with the three color directions. Compactness gives a positive gap outside a small chart. The same holds for small real \(t,b\) by continuity, the implicit function theorem and strict convexity in that chart. Denote the minimum by \(s(t,b)\); let \(d(t,b)\) be the log of the leading Laplace amplitude, i.e. the invariant Haar density at the minimum divided by the square root of the Hessian determinant, followed by the logarithm. Use \(\Delta h(t,b)=h(t,b)-h(0,b)\). There is a real analytic first Laplace correction \(L(t,b)\), and
\[
 W_b(t)=-\beta\Delta s(t,b)+\Delta d(t,b)
        +\beta^{-1}\Delta L(t,b)+O_{C_t^3}(\beta^{-2}) .          \tag{2}
\]
The bounds are uniform on this fixed small chart. To check the derivative remainder, center local coordinates at the smoothly moving minimizer and subtract its minimum before rescaling by \(\beta^{-1/2}\). Parameter derivatives of the resulting action start at quadratic degree in these centered coordinates. Up to three derivatives therefore add fixed polynomial factors in the rescaled Gaussian variable. Its precision stays in a fixed compact positive range. Taylor expansion of the smooth local density and action through order three in \(\beta^{-1/2}\) gives a dominated order-four remainder after integration; take a symmetric ball \(|y|\le\beta^{1/32}\) and Gaussian tails outside. Odd terms integrate to zero. The exponentially small complement of the chart remains negligible even after three differentiations. The leading amplitude is bounded away from zero. Division and the logarithm thus preserve the stated three-derivative bound. This real-parameter argument needs no contour deformation at a complex source saddle.

Global conjugation of the rooted loop coordinates fixes \(s,d,L\). The only invariant linear form on any number of copies of \(\mathfrak{su}(2)\) under simultaneous conjugation is zero. Thus for \(h=s,d,L\), all \(|J|\le3\) satisfy
\[
  |\partial_t^Jh(t,b)-\partial_t^Jh(t,0)|\le C |b|^2 .           \tag{3}
\]
In particular \(s(t,0)=0\) for all small real \(t\): the source weights leave the flat minimum at zero. This gives bounded fixed moments of the derivatives of \(\beta\Delta s\) under (1). Smoothness and gauge invariance apply also to \(L\) at nonzero \(t\); using an uncentered Hessian or dropping the Haar factor would change this calculation.

## 2. An exterior-averaged identity with a signed coefficient and a smaller error

On \(G\) set \(A_b(t)=-\beta\Delta s(t,b)+\Delta d(t,b)\); put \(A_b(t)=0\) on \(G^c\) for definiteness. Define
\[
 T_{\rm ext}(\beta)=
 \left.\partial_{123}\log\int \exp(A_b(t))\,d\mu_{\rm ext}(b)\right|_{t=0}.
\]
This is fully specified by the seven-link source-dependent minimizer, its leading Haar/Hessian amplitude, and the **true** exterior measure. It uses no interior thermal integrals. The result is
\[
 \boxed{\displaystyle
 \kappa_3^\mathrm{Wilson}(Y_1,Y_2,Y_3)-T_{\rm ext}(\beta)
  =\frac{1318200203}{3633942857366347382784}\,\beta^{-1}
    +O(\beta^{-2}).}                                               \tag{4}
\]
Unlike a conditional estimate on an exceptional event, (4) is an identity with a uniform error for the unrestricted periodic observable. The subtraction depends on the live region. It does not assign this summand to the total first coefficient independently of that choice.

Here is how the exterior covariances enter the proof. For any normalized conditional logarithm with derivatives \(M_i,C_{ij},K_{123}\) at zero, its integrated third logarithmic derivative is
\[
 \mathcal T(M,C,K)
 =\mathbb E K_{123}+\sum_{\rm cyc}\operatorname{Cov}(M_i,C_{jk})
      +\kappa_3(M_1,M_2,M_3).                                    \tag{5}
\]
This follows by differentiating at zero, including the conditional normalizers before computing the cumulant. It applies also to the approximate source \(A_b\), for which a positive generating measure in the sources is unnecessary. For each nonempty derivative \(J\subset\{1,2,3\}\), (1)–(3) imply
\[
 \partial_J W_b(0)-\partial_J A_b(0)
   =\beta^{-1}\partial_J L(0,0)+O_{L^p}(\beta^{-2}) ,
                                                                  \tag{6}
\]
for any fixed \(p<\infty\); the notation \(L(0,0)\) under a derivative means evaluation after differentiating its first argument. On the exceptional complement each \(Y_i\) is bounded by \(C\beta\) and its conditional jets by \(C_J\beta^{|J|}\). The complement therefore satisfies (6) with an exponentially small contribution. All other jets in (5) have bounded fixed moments by (1)–(3). Constants vanish in covariance and connected cumulants of order at least two. Applying Hölder in the differences of products in (5) leaves precisely \(\beta^{-1}\partial_{123}L(0,0)\); all mixed terms containing an exterior fluctuation of the first correction are \(O(\beta^{-2})\). The flat sourced chain and the \(4^{-3}\) scalar placement in the corresponding estimate §5 give its stated rational value. In particular \(T_{\rm ext}\) approximates the unrestricted scalar cumulant **from below** for all sufficiently large \(\beta\), at these fixed stencils, by at least half the coefficient in (4) divided by \(\beta\).

## 3. Reducing the remaining exterior term to degree-eight visible moments

The size and sign of \(T_{\rm ext}\) at order \(\beta^{-1}\) are not controlled by (4). There is a more explicit finite reduction. Write \(X=\sqrt{\beta}\,b\) on \(G\) and set \(X=0\) on its complement. For each \(J\) in (6), use the homogeneous Taylor polynomials \(S_{J,k}\) and \(D_{J,k}\) of degree \(k\) in \(b\) for \(\partial_Js(0,b)\) and \(\partial_Jd(0,b)\), respectively. All coefficients involve only the specified regular stationary point of the seven-link finite action and its derivatives at identity. Set
\[
 B_J=D_{J,0}-S_{J,2}(X)
     -\beta^{-1/2}S_{J,3}(X)
     +\beta^{-1}\{D_{J,2}(X)-S_{J,4}(X)\}.
\]
Conjugation kills both linear terms. Taylor remainders and (1) show that \(\partial_J A_b(0)-B_J=O_{L^p}(\beta^{-3/2})\); assigning constants differently on \(G^c\) costs exponentially little. Substituting \(B_i,B_{ij},B_{123}\) in (5) and discarding products of explicit powers of \(\beta^{-1/2}\) beyond power two changes \(T_{\rm ext}\) by \(O(\beta^{-3/2})\). Indeed every resulting polynomial of \(X\) has bounded moments under (1). The retained expectations involve joint moments of the visible, rooted logarithms of degree at most eight: in a triple of leading means the degree is at most six, and two extra half-orders add at most two more degrees. All contractions are invariant under the remaining root gauge. This gives an explicit local algebraic test for the exterior cancellation, with an error smaller than \(\beta^{-1}\). It does not replace these visible moments by those of a Gaussian. The combinations multiplying powers \(1,\beta^{-1/2},\beta^{-1}\) need absolute errors respectively \(o(\beta^{-1}),o(\beta^{-1/2}),o(1)\) to identify a total first coefficient by this reduction.

There is also a slice of this list whose replacement needs **no rate**. For the \(\beta^{-1}\) coefficient only the limiting visible moments are used. Under the compatible weak-sequence hypotheses of Annex O §§18–22, the finite list \(X\) converges in invariant polynomial moments to the rooted Gaussian loop fluxes. To verify the particular logarithms, fill every fundamental loop in this fixed contractible lift, express its ordered holonomy as a product of plaquette conjugates, and use one common local forest frame. Apply the finite-stencil transport argument of Annex O §§18 and 26 at fixed paths. To first order the loop logarithm is the sum of its oriented, based plaquette curls. Quadratic product/log errors vanish in probability in the \(\sqrt\beta\) scaling; the fixed-loop norm moments from (1) give uniform integrability. Root conjugation drops out of the joint invariant polynomial. The covariances of these Gaussian sums are the finite filling contractions of the lattice curl projector \(P\). Thus the \(\beta^{-1}\)-weighted polynomial has a computable unconditional Gaussian coefficient with \(o(\beta^{-1})\) error. The order-one and order-\(\beta^{-1/2}\) groups need the indicated sharper convergence of their own exterior moments.

## 4. Longer chains and the order of limits

The interior fraction has a geometric limitation. Repeat the construction with \(2m+1\) live parallel links, probe times \(0,m,2m\), and \(m\ge3\). Take \(n\ge 2m+6\) in the same reserve class. For each **fixed** \(m\) the preceding proof applies with constants depending on \(m\). The first interior coefficient \(c_m=\partial_{123}L_m(0,0)\) still follows from the formula of the corresponding estimate §5 with the new chain and three probes. One has
\[
 |c_m|\le C(2m+1)3^{-4m},\qquad m\ge3.                         \tag{7}
\]
To prove this, \(D_0=6I-A\) with \(A\) the nearest-neighbor chain adjacency. The inverse Neumann sum gives
\(0\le g_{ij}\le\tfrac14\,3^{-|i-j|}\), since a length-\(q\) walk has at most \(2^q\) choices and cannot arrive before \(|i-j|\). Sourced inverse entries have the ordered insertion formula of the corresponding estimate. A sourced diagonal entry is a closed walk through the indices at which it was differentiated. For the quartic term, the two inverse-entry factors are either two closed walks anchored at the endpoints of one edge (possibly the same endpoint), or two paths between the endpoints of that edge. In the first case join the closed walks with two steps of total length at most two; in the second case they already form one closed walk. Pinned edges have only the nonzero single endpoint. If one derivative hits a pinned weight, its source is at that same endpoint. Every retained product therefore visits all three probe times on a closed walk with total length at least \(4m\), counting at most two added steps. The finite derivative permutations and the lost factor \(3^2\) cost a fixed constant. Summing the \(O(2m+1)\) possible edge/site origins proves (7). The Gaussian interior determinant's direct three-probe coefficient has the same exponential decay by its three inverse entries.

In particular on the ordered limit with \(\beta\to\infty\) at fixed \(m\) first,
\[
 \lim_{m\to\infty}m^{12}
 \limsup_{\beta\to\infty}\beta
 \big|\kappa_3^\mathrm{Wilson}(Y_1,Y_2,Y_3)-T_{{\rm ext},m}(\beta)\big|=0 .
\]
The inner statement is uniform in the allowed period at fixed \(m\). There exists a sufficiently slow diagonal \(m(\beta)\to\infty\) with the same conclusion by the fixed-\(m\) error bounds, as long as the periods grow to contain the collar and satisfy the reserve. No effective growing chain rate is claimed. In this geometry nearly all of a putative power-law separated interaction at first order would have to appear in the exterior integral, even though the short-chain interior contribution (4) has a strict sign. This argument provides no physical matching or prescribed joint continuum/UV ordering. **U-01 and U-02 remain open.**

## 5. A positive-law comparison that measures the signed term

There is a way to test the sign without computing any realizing minimizer, Hessian or exterior-loop moment. Sample the full exterior once from the original Wilson measure at \(\beta\). Given it, take two **independent**, normalized seven-link compact heat-bath draws. In law A use local inverse couplings \((\beta,3\beta)\); in law B use \((2\beta,2\beta)\). At each of the three stated sites measure the **sum** of the two actual four-vertex scalars with each multiplied by its own inverse coupling and \(a^4\). Write \(\kappa_3^{A}\) and \(\kappa_3^{B}\) for the connected cumulants after integrating the exterior. Both are ordinary cumulants of explicit positive finite-dimensional laws. The \(\beta\) draw in A is precisely the original interior conditional law; together with the sampled exterior it has the original compact Wilson marginal.

At local inverse coupling \(r\beta\) the source-normalized log is (2) with \(\beta\) replaced by \(r\beta\), on the same exterior \(b\) and with identical \(s,d,L\). Conditional independence adds those logarithms. The leading terms of each pair are exactly \(-4\beta\Delta s+2\Delta d\) on \(G\). Their first corrections have respective factors \(4/(3\beta)\) and \(1/\beta\). Applying (3), (5) and the moment estimates (1) to the two sets of genuine conditional jets gives the unrestricted positive-ensemble contrast
\[
 \boxed{\displaystyle
 \kappa_3^{A}-\kappa_3^{B}
    =\frac{1318200203}{10901828572099042148352}\,\beta^{-1}
     +O(\beta^{-2})>0
 \quad\text{for sufficiently large \(\beta\)} .}                 \tag{8}
\]
The denominator is three times the denominator in (4). The two replicas share the exterior in each law, including the visible-only terms in all source stencils. Independently resampling two exteriors would change the covariance terms in (5). Equation (8) isolates a nonzero interacting response by a finite positive-law experiment while leaving the common exterior entirely unconditioned. Its paired local-coupling observable is distinct from the single physical scalar required in U-02.

### A one-copy contrast containing the original Wilson three-point function

In fact one need not duplicate the observable. For \(r>0\) resample the seven live links once at inverse coupling \(r\beta\), with all exterior links sampled from the true \(\beta\) marginal. Define \(K_\beta(r)\) to be the resulting unrestricted third cumulant of \(r\beta a^4w_a\) at the same three sites. Then \(K_\beta(1)\) is exactly the three-point cumulant of the original Wilson law. There is a polynomial \(P_\beta\) of degree at most three in \(r\) such that on each fixed compact subinterval of \(r>0\)
\[
 K_\beta(r)=P_\beta(r)+\frac{c_7}{r\beta}
                          +O_{C^4_r}(\beta^{-2}),\qquad
 c_7=\frac{1318200203}{3633942857366347382784}.                 \tag{9}
\]
Specifically \(P_\beta\) is (5) evaluated on the conditional jets of \(\mathbf1_G[-r\beta\Delta s+\Delta d]\). Every jet is affine in \(r\), and \(\mu_{\rm ext}\) is fixed; expectation, covariance and the third cumulant in (5) are respectively linear, bilinear and trilinear. This gives the exact degree bound even when the exterior distribution itself is far from Gaussian. Equations (2)–(6) yield the only surviving inverse power at order \(\beta^{-1}\). For the stated \(C^4_r\) remainder in (2), center at the same minimizer independent of \(r\), change coordinates \(u-u_*=\beta^{-1/2}y\), and keep \(r\) in the rescaled quadratic exponent. Each of four \(r\) derivatives of the normalized integral adds at most a fixed polynomial weight in \(y\) once the moving minimum is subtracted; the Gaussian bound uses the fixed positive lower endpoint of \(r\). The same expansion works jointly with the three \(t\) derivatives. Off \(G\) these finitely many derivatives cost at most a fixed power of \(\beta\) by boundedness of the compact action and its marks. The \(C^4_r\) bound follows through the finite multilinear formula (5).

The fourth finite difference at \(r=1\) annihilates \(P_\beta\), and \(\sum_{j=0}^4(-1)^j\binom4j/(1+j)=\int_0^1(1-x)^4dx=1/5\). In particular
\[
 K_\beta(1)-4K_\beta(2)+6K_\beta(3)-4K_\beta(4)+K_\beta(5)
       =\frac{c_7}{5\beta}+O(\beta^{-2}),\qquad
 K_\beta^{(4)}(1)=\frac{24c_7}{\beta}+O(\beta^{-2}).            \tag{10}
\]
Both left sides are strictly positive for sufficiently large \(\beta\). This is an estimate with error smaller than the first interacting term, using only positive single-copy measures with their actual conditional denominators. The derivative varies exclusively the seven-link conditional temperature and the specified scalar prefactor, keeping the original exterior marginal fixed. A uniform global variation of the Wilson coefficient would differentiate that marginal as well. Equations (9)–(10) bound a response of the original scalar cumulant; by themselves they do not determine \(P_\beta(1)\).

For a direct expression at the original measure, let \(J=\beta\sum_{p:\,p\cap I\ne\varnothing}s_p\) sum once over plaquettes containing a live link, let \(\mathcal B\) be the full exterior, and use the original marks \(Y_i=\beta a^4 w_a\). Then the derivative in (10) equals
\[
 \left.\partial_s^4\partial_{t_1t_2t_3}
 \log\mathbb E_\beta\!\left[
    \frac{\exp(-sJ+(1+s)t\cdot Y)}
         {\mathbb E_\beta[\exp(-sJ)\mid\mathcal B]}
 \right]\right|_{s=t=0}.                                         \tag{11}
\]
This is the conditional Radon–Nikodym identity at finite cutoff. The denominator is positive for real \(s\) and differentiable under the compact finite-dimensional integral. Its derivatives generate the centered conditional thermal scores, including all lower-order normalization subtractions. In particular (10) gives a signed quantitative asymptotic for a mixed local thermal/source response evaluated in the original unconditioned Wilson ensemble.

## 6. Exact placement cancellation in the separated Gaussian comparator

There is a finite-mesh version of the scalar cancellation that retains the actual plaquette placements. Let \(V_x=a^4w_a(x)\) denote the four-vertex scalar and \(C_x\) the closed-cube scalar of Annex O §53 with lower cube corner \(x\). Each assigns weight \(1/4\) to each of four plaquettes per orientation. In the Gaussian comparator take each individual energy to be its half curl square. Suppose the distinct \(V_{x_i}\) stencils are pairwise disjoint **as plaquette sets**. For all \(m\ge2\), with \(P\) the infinite-lattice curl covariance,
\[
 \kappa_m^G(V_{x_1},\ldots,V_{x_m})
    =(-1)^m\kappa_m^G(C_{x_1},\ldots,C_{x_m}).                    \tag{12}
\]
The compact Wilson stencils themselves obey no Gaussian duality assumption.

To prove (12), associate to a primal positively oriented plaquette its complementary oriented dual plaquette at the *same midpoint*, with the exterior-algebra Hodge sign. Identify the dual lattice with the primal by subtracting \(h=(1/2,1/2,1/2,1/2)\). This signed permutation of plaquettes is unitary on real square-summable two-forms. In midpoint Fourier coordinates the curl image at nonzero momentum is \(\hat k\wedge\mathbb R^4\), \(\hat k_j=2\sin(k_j/2)\), with its complexification. Its Hodge image is its orthogonal complement in two-forms. The half-translation contributes only a common scalar phase in these coordinates. Thus the transported projection is \(I-P\); the excluded Fourier point has measure zero on the infinite lattice. For orientation \(\mu\nu\), the four midpoints at \(x\pm e_\mu/2\pm e_\nu/2\), after dualization and subtraction of \(h\), are the four *complementary* faces of the cube with lower corner \(x-\mathbf1\). Indeed their \(\mu,\nu\) coordinates are \(x_j-1\) or \(x_j\), while their two complementary coordinates are \(x_j-1/2\). Conjugation by the signed permutation therefore carries the diagonal weight of \(V_x\) to that of \(C_{x-\mathbf1}\), \(\mathbf1=(1,1,1,1)\). It preserves disjointness. In a connected quadratic Wick cycle all edges join distinct insertions. An identity covariance entry on any edge is zero between their disjoint plaquette sets. Hence each transported \(I-P\) supplies a minus sign and a \(P\). Translation invariance then removes the common \(-\mathbf1\) shift. This argument does not assert the same finite-period formula with the harmonic sector discarded.

For \(m=3\), using both actual Wilson placements, the average of the **two cumulants** has no Gaussian lattice contribution at any separated mesh sites. On the compatible weak tori of the corresponding estimate (1), in \(\beta^3\) units its absolute value is \(O(\beta^{-\epsilon/6}+R/l)\), and multiplying by \(R^{12}\) gives the corresponding magnified bound. Each placement uses the same elementary-plaquette moment comparison. This cancels the lattice artifact exactly, without replacing the full Wilson measure. It is an average of two separately measured triples, not the cumulant of their pointwise half-sum, which would introduce mixed placements. The error still exceeds the first physical interacting order. Passing from this comparison to the exact prescribed vertex field would also need control of their interacting placement difference at that order. Curl covariance and actual placements, Annex O §§18, 53
