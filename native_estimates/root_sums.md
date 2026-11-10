# Hidden components and the multiscale sum over roots

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

**Propagation hypothesis.** Any use of a T-step bound on a holed ancestor requires the conditional single-ancestor estimate and, for connected products, a separate collective crossing estimate. An argument from the diameter of the union of paid components alone is invalid.

## 1. Conventions and the source facts used

### 1.1 Conventions

\(d\ge 2\) is the dimension (\(d=4\) in the application), \(L\ge2\) the block factor, \(M\) the side of a localization cube in lattice units of its own scale. At a step with current index \(k\), the scale-\(j\) lattice has mesh \(h_j=L^{j-k}\) in current units, and a *scale-\(j\) cube* is a closed cube of side \(s_j=Mh_j\) of the fixed grid \(\mathcal G_j\) (the family \(\pi_j\) of CMP109 p.257). Two cubes are *adjacent* if they share a \((d-1)\)-face. \(\mathbf D_j\) is the class of finite face-connected unions of scale-\(j\) cubes. For a set \(X\) of cubes, \(X^{\sim}\) is the set of grid cubes at \(\ell^\infty\) index distance \(\le1\) from \(X\) (CMP109 p.257: \(\square^{\sim n}\) is the concentric cube of side \((1+2n)M\)). A *box* is a product of intervals of grid cubes. \(|\cdot|_\infty\), \(|\cdot|_2\) are the sup and Euclidean norms; \(\operatorname{diam}_\infty\) the sup-norm diameter.

A *tree graph* is a compact connected union of finitely many segments in \(\mathbb R^d\); its length is the sum of the Euclidean lengths.

**Visiting size.** For a finite set \(E\) of cubes of side \(s\),
\[
 \delta_s(E)=s^{-1}\inf\{\,|T|:\ T\ \text{a tree graph in }\mathbb R^d\text{ meeting every cube of }E\,\}.
 \tag{1.1}
\]
The tree is *not* required to stay inside \(E\). Hence \(\delta_s(E)\) is dominated by every size functional occurring in the source: the linear size \(d_j(E)\) of CMP109 p.257 (tree inside \(E\)), the relative size \(d_{k,Z}(Y)\) of LFR II (1.67) (tree inside \(Y\) visiting the cubes of \(Y\setminus Z\)), and any reading of "\(d_k(X'\setminus\cup Y_i)\)" on LFR II p.391. All estimates below use only \(\delta\).

### 1.2 Source facts

| | Fact | Where | Checked |
|---|---|---|---|
| S1 | Eligible components: contained in a cube of side \(100MR_k\); every step adds at least ten layers of \(MR_k\)-cubes, "hence the size must be greater than \(20MR_k\)"; all regions of the last \(N\) steps in such a component are rectangular parallelepipeds. | LFR I p.177, (i)–(ii) | printed source |
| S2 | Components of a large-field region are joined when they intersect *or touch*; they are unions of \(MR_j\)-cubes. Hence distinct components are at distance at least one \(MR_k\)-cube. | LFR II p.386 (graph \(G\) below (1.85)); CMP119 p.256 | p.386 printed source for the convention "intersect, or touch"; the separation is an inference from the common \(MR_k\)-grid (CMP119 p.256, source) |
| S3 | After relocalization the remaining terms are indexed by "domains \(Y\in\mathbf D_k\) satisfying the property that the intersection \(Y\cap Z^{\sim}\) is a union of components of \(Z^{\sim}\), containing at least one component", with \(|V(Y)|\le\alpha e^{-(1+2\beta)\kappa d_{k,Z}(Y)}\) for \(Y\setminus Z^\sim\neq\emptyset\) (1.68) and a volume bound (1.69) when \(Y\) is a component of \(Z^\sim\). | LFR II p.377 | printed source |
| S4 | \(d_{k,Z}(Y)=M^{-1}\)(length of a shortest tree graph contained in \(Y\) and intersecting all \(M\)-cubes of the components of \(Y\setminus Z\)). | LFR II (1.67), p.376 | printed source |
| S5 | Normalized component operation: \(|(\mathbf T'_k(X)1)^{-1}\mathbf T'_k(X)F|\le e^{3\sup|\sigma|}\sup|F|\), with \(|\sigma|\le1\) used in (1.92). | LFR II (1.75), p.380; p.388 | printed source |
| S6 | Polymer bound: \(\prod_{Y\in\mathbf D}\alpha e^{-(1+2\beta)\kappa d_{k,Z'}(Y)}\le e^{-(1+\beta)\kappa d_{k,\cup Y_i}(X')}e^{-\frac{\beta\kappa}{3\cdot2^d}M^{-d}|X'\setminus\cup Y_i|}\cdots\), \(Z'=\cup Y_i\cup\cup X_{j_h}\); outputs \(|\mathbf R'^{(k)}(X)|\le O(1)c_1e^{-(1+\frac12\beta)\kappa d_{k,Z'_r}(X)}\), \(c_1=\alpha^{1/3}\) if \(X\) meets \(\cup Y_i\). | LFR II (1.92)–(1.99), pp.388–390 | p.388 printed source; rest from the text only |
| S7 | Alternative representation: \(\prod_i(\mathbf T'_k(Y_i)1)\,[\prod_i(\mathbf T'_k(Y_i)1)^{-1}\mathbf T'_k(Y_i)\exp\sum\mathbf B'^{(k)}(X)]\); the bracket is exponentiated with "\(\beta\) replaced by \((1/4)\beta\), \(\alpha\) by \(O(1)c_1\)", "the linear size \(d_k(X'\setminus\cup Y_i)\)", factors \(e^3\) per \(Y_i\subset X'\); the multipliers "depend only on the new field variables \(V_k\) restricted to \(Y_i\), therefore they do not participate in operations connected with next renormalization transformations". No final bound is displayed; the text says only "we obtain (1.98) for the expression in the square bracket". | LFR II pp.391–392, (1.103)–(1.104) | printed source |
| S8 | Relocalization factor for a record \(\mathbf E(X)\), \(X\in\mathbf D_j\): \(\exp\{-\beta\kappa d_j(X)-(1+3\beta)\kappa d_k(Y_0)-\delta d((Y_i^0)^c\cap Y_1\cap Y'_{i_0},X)-\sum_{i=2}^4(\kappa_1-1)M^{-d}|Y'_i|\}\) (the \(\kappa\) in the second term is missing in print); "the exponential decay of the functions \(\mathbf H''_k,\mathbf H_{\mathbf B_1},\mathbf H_k\) and \(\mathbf H(\mathbf B''_k(Y_1),\cdot)\) yields the additional factor … where \(i\) is the first index with a nonempty domain \(Y'_i\), and \(d(\cdot,\cdot)\) is the scaled distance". | LFR II (1.66), p.376 | printed source |
| S9 | First relocalization map: \(U''_k=U(\mathbf B''_k(Y_1),\dots)\) on \(Y_1\), with \(\mathbf B''_k(Y_1)=\mathbf B(Y_1)\cup\mathbf B''_k\); the arguments are the boundary-layer data on \((Y_1^0)^c\cap Y_1\) (the only place where \(\mathbf H''_k\) and \(U_1\) enter) and the unchanged fields \(V''\), \(M'(U_0^{(\Lambda L)})\) inside \(Y_1^0\); "\(Y_1\setminus Y_1^0\) is a boundary layer at the boundary \(\partial Y_1\), of the width \(2M_1\) at most, for the corresponding scale". | LFR II (1.61), p.373 | printed source |
| S10 | Prepared sequence in an eligible component: \(N_0\) is the smallest positive integer with \(L^{-N_0+1}MR_{k-N_0+1}=M\); \(Z''_k=(\Omega^{\sim5}_{k-N_0+1})^c\cap Z\), \(Z''_{k-N_0+1}=(\Omega^{\sim7}_{k-N_0+1})^c\cap Z\), completed so that \(Z''^c_{j+1}\) and \(Z''_j\) are separated by one layer of \(L^{-(k-j-1)}M\)-cubes; \(Z''_j=(\Omega_j^{\sim5})^c\cap Z\) for \(h+1\le j\le k-N_0\); \(Z''_j=Z_j\) for \(j\le h=k-N\); \(N>N_0\). | LFR I (1.10)–(1.12), p.179 | printed source |
| S11 | Ordinary geometry: \(\Lambda_{k+1}\) is obtained from \(Z_k\) by taking the \(LMR_{k+1}\)-cube cover, four layers, and further layers around \(P_{k+1},Q_{k+1},R_{k+1}\); ordinary \(\Omega_j,\Lambda_j\) are unions of \(MR_j\)-cubes with "distance between their boundaries at least \(2MR_j\)". | CMP119 pp.264–269, (3.2)–(3.20); p.256 | p.256; pp.264–269 from the text only |
| S12 | Ordinary inductive form of the boundary terms: \(\mathbf B^{(j)}(X)\), \(X\in\mathbf D_j\), \(X\cap\Omega_j\ne\emptyset\), \(X\cap Z_j\ne\emptyset\), analytic on \(\mathbf U_j^c(X,\cdot)\), \(|\mathbf B^{(j)}(X)|\le B_0e^{-\kappa d_j(X)}\); alternative: \(X\) contains or misses each component of \(Z_j\), with \(d_j(X\setminus Z_j)\), and "all constructions and proofs of the procedure can be carried on with these inductive assumptions". \(\kappa_0\) "can be chosen arbitrarily large, similarly as \(\kappa\)". | CMP119 (2.40)–(2.42), pp.261–262; p.260 | p.262 printed source (the alternative form and the quoted sentence); pp.260–261 from the text only |

| S13 | The source's weighted ("scaled") distance: for a sequence \(\{\Omega_j\}\) the distance \(d(y,y')\) is the infimum over admissible contours of the contour length, the part of the contour in \(B^j(\Lambda_j)\) being measured in units of the local mesh \(L^j\eta\) ("taking into account that natural scales are different on different subdomains"). The Green's functions and minimizers of a determining sequence decay like \(e^{-\delta_0d(y,y')}\) in this distance. | CMP96 (2.45)–(2.48), pp.230–232; CMP99 p.397 and Theorem 3.1 ff. | source input (the display (2.46) itself is not reproduced here) |

S7 and S12 contain *assertions without displayed proofs*. They are used below only inside named premises. S13 identifies the source's scaled distance with the graded distance \(d_g\) of §4.1 up to the fixed factor \(M\) (lattice units versus \(M\)-cubes).

## 2. Part A — geometry of carriers containing boxes (all deduction)

Throughout Part A the grid is \(\mathbb Z^d\) (cubes identified with integer points; side \(s\) restored when lengths are needed), \(d\ge2\).

### Lemma A1 (the shell of a box is face-connected)

Let \(Q=\prod_{i=1}^d[a_i,b_i]\) be a box and \(S(Q)=Q^\sim\setminus Q\), \(Q^\sim=\prod_i[a_i-1,b_i+1]\). Then \(S(Q)\) is face-connected, and
\[
 |S(Q)|=\prod_i(n_i+2)-\prod_in_i\ \ge\ 2\sum_i\prod_{j\ne i}n_j\ \ge\ 2d\,n_{\min}^{\,d-1},\qquad n_i=b_i-a_i+1.
 \tag{A.1}
\]

*Proof.* \(x\in S(Q)\) iff \(x\in Q^\sim\) and \(x_i\in\{a_i-1,b_i+1\}\) for some \(i\). So \(S(Q)=\bigcup_{i,\pm}F_i^\pm\), where \(F_i^+=\{x\in Q^\sim:x_i=b_i+1\}\) and \(F_i^-=\{x\in Q^\sim:x_i=a_i-1\}\). Each \(F_i^\pm\) is a \((d-1)\)-dimensional box, hence face-connected. For \(i\ne j\), \(F_i^\pm\cap F_j^\pm\ne\emptyset\) (fix both coordinates). Since \(d\ge2\), \(F_i^+\) and \(F_i^-\) both meet \(F_j^+\) for some \(j\ne i\). Hence the union is face-connected. The count follows by expanding the product. \(\square\)

### Definition (tag family, admissible carrier, exterior)

A *tag family* is a finite family \(\mathcal Q\) of boxes with

- **(T1)** distinct \(Q,Q'\in\mathcal Q\) have \(\ell^\infty\) index distance \(\ge2\) (equivalently \(Q^\sim\cap Q'=\emptyset\)).

A finite face-connected set \(X\) of cubes is *admissible for \(\mathcal Q\)* if

- **(T2)** for every \(Q\in\mathcal Q\): \(X\cap Q^\sim=\emptyset\) or \(Q^\sim\subset X\).

Put \(\mathcal H(X)=\{Q\in\mathcal Q:Q\subset X\}\) and \(E(X)=X\setminus\bigcup_{Q\in\mathcal H(X)}Q\) (the *exterior*).

### Lemma A2 (halo lemma)

Let \(X\) be admissible for \(\mathcal Q\) and \(E=E(X)\). Then:

1. \(S(Q)\subset E\) for every \(Q\in\mathcal H(X)\), and \(E\cap Q^\sim=\emptyset\) for \(Q\in\mathcal Q\setminus\mathcal H(X)\).
2. \(E\) is face-connected (and nonempty).
3. \(X=E\cup\bigcup\{Q\in\mathcal Q:S(Q)\subset E\}\). In particular \(X\mapsto E(X)\) is injective on admissible sets.
4. \(E\) and \(X\) have the same bounding box; hence \(\operatorname{diam}_\infty(\cup X)=\operatorname{diam}_\infty(\cup E)\).
5. Every continuous path from a point outside \(\bigcup_{Q\in\mathcal H(X)}\cup Q^\sim\) to a point of \(\cup X\) meets \(\cup E\) no later than it meets \(\cup X\setminus\cup E\). Consequently, for every path metric \(D\) on \(\mathbb R^d\) and every such starting point \(x\), \(D(x,\cup X)=D(x,\cup E)\).

*Proof.* (1) If \(Q\in\mathcal H(X)\) then \(X\cap Q^\sim\neq\emptyset\), so \(Q^\sim\subset X\) by (T2); by (T1) no cube of \(S(Q)\subset Q^\sim\) lies in another tag, and none lies in \(Q\); so \(S(Q)\subset E\). If \(Q\notin\mathcal H(X)\) and \(X\cap Q^\sim\ne\emptyset\), (T2) would give \(Q\subset Q^\sim\subset X\), a contradiction.

(2) Let \(c,c'\in E\) and let \(c=c_0,\dots,c_n=c'\) be a face-path in \(X\). Consider a maximal run \(c_p,\dots,c_q\) of consecutive cubes lying in \(\bigcup\mathcal H(X)\). Adjacent cubes cannot lie in different tags, by (T1); so the run lies in one \(Q\in\mathcal H(X)\). Since \(c_0,c_n\in E\), \(1\le p\le q\le n-1\). The cube \(c_{p-1}\) is adjacent to \(c_p\in Q\) and is not in \(Q\) (maximality), so \(c_{p-1}\in Q^\sim\setminus Q=S(Q)\); likewise \(c_{q+1}\in S(Q)\). By Lemma A1 replace \(c_p,\dots,c_q\) by a face-path inside \(S(Q)\subset E\). Doing this for every run gives a face-path in \(E\).

(3) By (1), \(Q\in\mathcal H(X)\Rightarrow S(Q)\subset E\). Conversely \(S(Q)\subset E\subset X\) gives \(X\cap Q^\sim\neq\emptyset\), hence \(Q\subset X\).

(4) For \(Q\in\mathcal H(X)\), the bounding box of \(Q\) is contained in that of \(S(Q)\subset E\).

(5) A path from outside \(\cup Q^\sim\) to a point of \(\cup Q\) must meet the closed set \(\cup Q^\sim\setminus\operatorname{int}(\cup Q)\) before it meets \(\operatorname{int}(\cup Q)\); every point of that set lies in a cube of \(S(Q)\) or on \(\partial(\cup Q)\), and each point of \(\partial(\cup Q)\) lies in a cube of \(S(Q)\) (the neighbour across the face, edge or corner). So the path meets \(\cup S(Q)\subset\cup E\) first. \(\square\)

**Remark A2′ (without (T2)).** With a modified definition of the hole set, (T2) is needed only for item 3 and for the second half of item 1. For an arbitrary finite nonempty face-connected \(X\) define instead \(\mathcal H(X)=\{Q\in\mathcal Q:Q^\sim\subset X\}\) and \(E(X)=X\setminus\bigcup\mathcal H(X)\) (for admissible \(X\) this is the same set). Then items 1 (first half), 2, 4 and 5 hold with the same proofs: in the proof of item 2 the cube \(c_{p-1}\) lies in \(S(Q)\subset X\), and \(S(Q)\) meets no tag by (T1), so \(c_{p-1}\in E\). Item 3 is replaced by: \(X\) is determined by \(E\) and the subset \(\mathcal H(X)\subset\{Q:S(Q)\subset E\}\); hence at most \(2^{n(E)}\) sets \(X\) have the same exterior \(E\), where \(n(E)=\#\{Q:S(Q)\subset E\}\le|E|/\min_Q|S(Q)|\) when the shells are pairwise disjoint.

### Lemma A3 (size lemma)

Let \(E\) be a finite set of grid cubes of side \(s\) and \(T\) a tree graph of length \(\ell\) meeting every cube of \(E\). Then
\[
 |E|\le 2^d\Bigl(\frac{2\ell}{s}+1\Bigr),\qquad \operatorname{diam}_\infty(\cup E)\le \ell+2s.
 \tag{A.2}
\]
Hence \(|E|\le2^d(2\delta_s(E)+1)\) and \(\operatorname{diam}_\infty(\cup E)\le s(\delta_s(E)+2)\).

*Proof.* \(T\) is a connected finite graph embedded with straight edges of total length \(\ell\). Doubling every edge gives an Eulerian multigraph, so there is a closed walk traversing every edge twice: a \(1\)-Lipschitz surjection \(\gamma:[0,2\ell]\to T\) (if \(\ell=0\), \(T\) is a point). Put \(m=\lfloor2\ell/s\rfloor+1\) and cut \([0,2\ell]\) into \(m\) closed intervals of equal length \(2\ell/m<s\). Each image has Euclidean, hence sup-norm, diameter \(<s\), so each of its coordinate projections lies in a closed interval \([\alpha,\beta]\) with \(\beta-\alpha<s\). A grid interval \([js,(j+1)s]\) meets \([\alpha,\beta]\) only if \(\alpha/s-1\le j\le\beta/s\), a range of length \(<2\), which contains at most two integers. So each image meets at most \(2^d\) grid cubes. As \(T\) meets every cube of \(E\), \(|E|\le2^dm\le2^d(2\ell/s+1)\).

For the diameter, let \(x\in c\in E\), \(y\in c'\in E\) and pick \(x'\in T\cap c\), \(y'\in T\cap c'\). Then \(|x-y|_\infty\le|x-x'|_\infty+|x'-y'|_\infty+|y'-y|_\infty\le s+\ell+s\), because \(x',y'\) are joined inside \(T\) by a path of length \(\le\ell\). \(\square\)

### Lemma A4 (counting)

The number of face-connected sets of \(n\) grid cubes containing a given cube is at most \((2d)^{2(n-1)}\).

*Proof.* Take a spanning tree of the adjacency graph of the set, rooted at the given cube; its depth-first traversal is a closed walk of \(2(n-1)\) steps, each to one of \(2d\) neighbours, and it visits exactly the set. \(\square\)

**Counting constant.** For \(a>0\) put
\[
 \tau(a)=\frac{a}{2^{d+1}}-2\log(2d).
 \tag{A.3}
\]
The condition \(\tau(a)>0\) reads \(a>\kappa_{\rm cnt}additional assumption:=2^{d+2}\log(2d)\) (\(\approx133\) for \(d=4\)). This is not optimal; it is admissible because the source permits \(\kappa\) arbitrarily large (S12). No attempt is made here to optimize it.

## 3. Part B — carriers of completed components are ordinary carriers

### 3.1 The reduction

**Proposition B1.** Let \(\mathcal Q\) be a tag family of boxes made of scale-\(b\) cubes (side \(s=Mh_b\)) and let \(X\) be admissible, \(E=E(X)\). Then

1. \(E\in\mathbf D_b\) (a genuine localization domain), \(X\) is determined by \(E\), and
 \[
 \operatorname{diam}_\infty(\cup X)\le s\,(\delta_s(E)+2),\qquad |E|\ge\sum_{Q\in\mathcal H(X)}|S(Q)|\ \ \text{if the shells are pairwise disjoint}.
 \tag{B.1}
 \]
2. Each of the following is \(\ge\delta_s(E)\): the linear size \(d_b(E)\); the relative size \(d_{b,\cup\mathcal H(X)}(X)\) of (1.67); the length (in units \(s\)) of any tree spanning the cubes of \(E\) in \(X\) or in \(\mathbb R^d\). Since \(E\) is connected, "the sum of the sizes of the exterior components" is the size of the single component \(E\).
3. For every point \(x\notin\bigcup_{Q\in\mathcal H(X)}\cup Q^\sim\) and every path metric \(D\), \(D(x,\cup X)=D(x,\cup E)\).

*Proof.* Lemma A2 and Lemma A3. The lower bound on \(|E|\) holds when the shells of distinct tags are pairwise disjoint, i.e. when distinct tags have index distance \(\ge3\); (T1) alone (distance \(\ge2\)) does not give it: for \(Q=\{(0,0)\}\), \(Q'=\{(2,0)\}\), \(X=Q^\sim\cup Q'^\sim\) in \(d=2\) one has \(|E|=13<16\). Everything else in the proposition needs only (T1). \(\square\)

**Proposition B2 (rooted sums).** Let \(a>\kappa_{\rm cnt}(d)\), \(\tau=\tau(a)\), and let \(X\mapsto w_X\ge0\) be defined on admissible sets with \(w_X\le Ae^{-a\delta_s(E(X))}\). Then

1. for every cube \(c\): \(\displaystyle\sum_{X:\,c\in E(X)}w_X\le A\,\frac{e^{a/2}\,e^{-a/2^{d+1}}}{1-e^{-\tau}}=:A\,C_1(d,a)\);
2. for every set \(S\) of cubes: \(\displaystyle\sum_{X:\,S\subset E(X)}w_X\le A\,\frac{e^{a/2}}{(2d)^2(1-e^{-\tau})}\,e^{-\tau|S|}\). In particular, for a tag \(Q\), \(\sum_{X\supset Q}w_X\le A\,e^{a/2}(2d)^{-2}(1-e^{-\tau})^{-1}e^{-\tau|S(Q)|}\).

*Proof.* By Lemma A2(3) the sums may be taken over the face-connected sets \(E\). By Lemma A3, \(\delta_s(E)\ge|E|/2^{d+1}-\tfrac12\), so \(w\le Ae^{a/2}e^{-a|E|/2^{d+1}}\). By Lemma A4, with \(n=|E|\) and root \(c\) (resp. a fixed cube of \(S\), and \(n\ge|S|\)),
\[
 \sum_{n\ge n_0}(2d)^{2(n-1)}e^{-an/2^{d+1}}=(2d)^{-2}\frac{e^{-\tau n_0}}{1-e^{-\tau}},
\]
with \(n_0=1\) resp. \(n_0=|S|\); for \(n_0=1\) note \((2d)^{-2}e^{-\tau}=e^{-a/2^{d+1}}\). \(\square\)

**Remarks.**

- *No attachment entropy.* A carrier that uses a tag contains its whole shell, so it can be rooted at one fixed shell cube. The polynomial factor \((1+R_j)^s\) of (CR.10)/(CR.20) is unnecessary; what appears instead is the gain \(e^{-\tau|S(Q)|}\), with \(|S(Q)|\ge2d(20R_k)^{d-1}\) by S1 and (A.1).
- *No separation or collar hypothesis.* (B.1) pays the full sup-norm diameter of \(X\), *including the traversal of every tag*, by the exterior size alone, with constant one. The relative separation (G4)/(CR.5), the proportional collar (G6) and the extracted guard (CR.7) are not needed for this purpose.
- *Weighted versions.* Replacing \(w_X\) by \(w_Xe^{\theta\delta_s(E)}\) replaces \(a\) by \(a-\theta\).
- *Without (T2).* For arbitrary face-connected carriers, with \(\mathcal H(X)\), \(E(X)\) as in Remark A2′ and pairwise disjoint shells of size \(\ge S_{\min}\), the multiplicity \(2^{n(E)}\le e^{|E|\log2/S_{\min}}\) changes Proposition B2 only by replacing \(\tau\) with \(\tau-\log2/S_{\min}\) (which must be positive) and, in the last sentence of item 2, "\(X\supset Q\)" by "\(X\supset Q^\sim\)". So admissibility is a convenience, not a necessity, *provided the pointwise bound charges every cube of \(E(X)\)*, i.e. every cube of the carrier outside the fully shelled tags.

### 3.2 Consequences for the printed LFR II objects conditional

Let \(Z\) be the union of eligible components at an R step of scale \(k\) (S1): boxes of scale-\(k\) cubes with all sides \(\ge20R_k\) cubes, pairwise separated by at least one \(MR_k\)-cube, i.e. by \(R_k\) scale-\(k\) cubes (S2). They form a tag family (T1), and for \(R_k\ge2\) their shells are pairwise disjoint. By S3 every \(Y\) indexing a term \(V(Y)\) is admissible (T2). A face-connected union of admissible sets is admissible. A polymer of the expansions (1.90)–(1.98) is a connected union of such \(Y\)'s and of bare first-class components \(X_j\); a bare \(X_j\) that is not inside some \(Y\) of the polymer is not adjacent to any \(Y\) of the polymer (a \(Y\) sharing a face with \(X_j\) contains a cube of \(X_j^\sim\), hence all of \(X_j^\sim\)). So a polymer is either a single bare first-class component — these give R terms with the *full-tree* bound (1.100) and no holes, and are ordinary records — or it contains at least one \(Y\) and is admissible. In particular every boundary term whose carrier touches a retained component \(Y_i\) has an admissible carrier. Write \(S_{\min}=2d(20R_k)^{d-1}\).

**Corollary B3.** Assume (1.68), (1.75) and S3 as printed, \(R_k\ge2\) (so that the shells of distinct components are disjoint), and \((1+2\beta)\kappa-\lambda-4>\kappa_{\rm cnt}(d)\) for a weight \(\lambda\ge0\). Put \(a=(1+2\beta)\kappa-\lambda-4\).

1. *Every nonself interaction is exponentially small in \(R_k^{\,d-1}\):* for \(Y\setminus Z^\sim\neq\emptyset\),
 \[
 |V(Y)|\le\alpha\exp\Bigl\{-(1+2\beta)\kappa\Bigl(\frac{S_{\min}}{2^{d+1}}-\frac12\Bigr)\Bigr\}.
 \tag{B.2}
 \]
2. *Diameter:* \(\operatorname{diam}_\infty(Y)\le M(d_{k,Z}(Y)+2)\).
3. *Component-incidence load.* Let \(I_Y\) be the set of components of \(Z\) contained in \(Y\). Then for every component \(v\), summing over the nonself carriers (those with \(Y\setminus Z^\sim\ne\emptyset\); the self term \(Y=v^\sim\) stays inside \(\mathbf T'_k(v)\), cf. (1.69), (1.71)),
 \[
 \sum_{Y\supset v,\ Y\setminus Z^\sim\ne\emptyset}e^{4|I_Y|}\,|V(Y)|\,e^{\lambda(d_{k,Z}(Y)+2)}
 \le\alpha\,\frac{e^{2\lambda+a/2}}{(2d)^2(1-e^{-\tau(a)})}\,e^{-\tau(a)S_{\min}}.
 \tag{B.3}
 \]

*Proof.* Write \(E=E(Y)=Y\setminus Z\) and \(\delta=\delta_M(E)\). \(E\) contains the pairwise disjoint shells of the components in \(I_Y\), so \(|E|\ge|I_Y|S_{\min}\ge S_{\min}\). By S4 and (1.1), \(d_{k,Z}(Y)\ge\delta\ge|E|/2^{d+1}-\frac12\) (Lemma A3). This gives (B.2). Item 2: a tree realizing \(d_{k,Z}(Y)\) meets all cubes of \(E\), so \(\operatorname{diam}_\infty(\cup E)\le M(d_{k,Z}(Y)+2)\) by (A.2), and \(\operatorname{diam}_\infty(Y)=\operatorname{diam}_\infty(\cup E)\) by Lemma A2(4).

Item 3. Since \(S_{\min}\ge3\cdot2^d\), we have \(\delta\ge S_{\min}/2^{d+1}-\frac12\ge1\) and \(|I_Y|\le|E|/S_{\min}\le2^d(2\delta+1)/S_{\min}\le3\cdot2^d\delta/S_{\min}\le\delta\). Hence, using \(d_{k,Z}(Y)\ge\delta\) and \((1+2\beta)\kappa-\lambda\ge0\),
\[
 e^{4|I_Y|}\,|V(Y)|\,e^{\lambda(d_{k,Z}(Y)+2)}\le\alpha e^{2\lambda}e^{4\delta}e^{-((1+2\beta)\kappa-\lambda)\delta}=\alpha e^{2\lambda}e^{-a\delta}.
\]
The carriers \(Y\supset v\) are admissible sets with \(S(v)\subset E(Y)\). Apply Proposition B2(2) with \(A=\alpha e^{2\lambda}\), \(S=S(v)\), \(|S(v)|\ge S_{\min}\). \(\square\)

**Meaning for the finite-cutoff construction conditional theorem.** In the notation of the finite-cutoff construction, (B.3) is the component load (R11), \(2\sup_v\sum_{e\ni v}w_ee^{|I_e|}\le1\), for the interactions \(e=V(Y)\) *that the normalized kernels of LFR II actually integrate*, with operator constant \(M_{\rm op}=e^3\) from (1.75), extent \(\ell_e=\operatorname{diam}_\infty(Y)/M\), on the source's native domain \(\widetilde{\mathbf U}{}^c_k(Y,\tilde\alpha_0,\tilde\alpha_1)\). The margin is \(e^{-\tau S_{\min}}\). The transfer from the native domain to the common current contour is premise P2 below; it is not proved here.

**The two-attachment diagnostic.** In (R29) the two carriers are \(X_x=H\cup Q_x\), \(X_y=H\cup Q_y\) with one exterior cube each. Such carriers violate (T2): by S3 a carrier containing \(H\) contains the whole shell \(S(H)\). For admissible carriers the amplitude bound (B.2) applies to each interaction, and the mixed derivative produced by integrating \(H\) is bounded by the *product* of two such amplitudes, while the endpoint separation is at most \(M(\delta+2)\) by (B.1). The collar condition \(\chi(C_D+2)<2\kappa\) of (R31) is therefore not the operative mechanism for source carriers; the shell is. (The diagnostic itself was correctly labelled an abstract example.)

## 4. Part C — a multiscale root-sum theorem

This part is self-contained. It treats a family of scalar "records" born at different scales, seen from a current coordinate, and bounds the rooted derivative sums with constants independent of the number of scales and of the volume.

### 4.1 Setting

Fix \(d\ge1\), an integer \(L\ge2\), \(M\ge1\), \(K\ge1\), and \(h_n=L^{n-K}\) for \(1\le n\le K\) (so the current mesh is \(h_K=1\)).

**Grades and graded metrics.** Let \(g:\mathbb R^d\to\{1,\dots,K\}\) be Borel (on a torus, replace \(\mathbb R^d\) by the torus; nothing changes). For \(1\le b\le K\) and a rectifiable path \(\gamma\) put
\[
 \ell^{(b)}(\gamma)=\int_\gamma\frac{|dx|_2}{M\max(h_{g(x)},h_b)},\qquad
 d^{(b)}(x,y)=\inf_\gamma\ell^{(b)}(\gamma),\qquad d_g:=d^{(1)}.
 \tag{C.1}
\]
\(d_g\) is the *graded distance* (local unit: one \(M\)-cube of the local scale); \(d^{(b)}\) is the same with units capped from below at scale \(b\). Clearly
\[
 d_g\ \ge\ d^{(b)}\ \ge\ \frac{|x-y|_2}{M}\ \ge\ \frac{|x-y|_\infty}{M}.
 \tag{C.2}
\]

**(Geo) layer hypothesis.** There are numbers \(\omega_n\ge0\) (\(2\le n\le K-1\)) with
\[
 \operatorname{dist}_2\bigl(\{g\le n-1\},\{g\ge n+1\}\bigr)\ \ge\ \omega_nMh_n ,
 \tag{C.3}
\]
and constants \(c>0\), \(\gamma>0\), \(C_0\ge0\) such that for all \(1\le b\le K-1\)
\[
 \frac c2\sum_{n=b+1}^{K-1}\omega_n\ \ge\ (d\log L+\gamma)(K-1-b)-C_0.
 \tag{C.4}
\]

**Sites.** \(I\) is a finite set of current coordinates with positions \(x_i\), \(g(x_i)=K\), and density \(\#\{i:x_i\in B\}\le n_I(r+1)^d\) for every cube \(B\) of side \(r\ge0\).

**Records.** \(\mathcal R\) is a finite family. Each \(\rho\in\mathcal R\) has

- a birth \(b=b(\rho)\in\{1,\dots,K\}\);
- a finite set \(E_\rho\) of closed cubes of the grid \(\mathcal G_b\) of mesh \(s_b=Mh_b\);
- an anchor cube \(q_\rho\in E_\rho\) with \(q_\rho\cap\overline{\{g\le b\}}\ne\emptyset\);
- a weight \(w_\rho\ge0\) and a function \(F_\rho\) holomorphic on \(D_P=\{z\in\mathbb C^I:|z_i|<P\ \forall i\}\) with

\[
 \textbf{(Loc)}\qquad |\partial_iF_\rho(z)|\le\frac{w_\rho}{P}\,e^{-\nu\,d_g(x_i,\cup E_\rho)}\qquad(i\in I,\ z\in D_P).
 \tag{C.5}
\]

**Rooted norms.** With \(\delta_b=\delta_{s_b}\) from (1.1), for \(\theta\ge0\)
\[
 \mathcal A_b(\theta)=\sup_{q\in\mathcal G_b}\ \sum_{\rho:\ b(\rho)=b,\ q_\rho=q}w_\rho\,e^{\theta\delta_b(E_\rho)}.
 \tag{C.6}
\]

No connectivity of \(E_\rho\) is needed in this part; it enters only when \(\mathcal A_b\) is estimated (Part B).

### 4.2 Two lemmas

**Lemma C1 (layer crossing).** Let \(1\le b\le K-1\), \(a\in\overline{\{g\le b\}}\) and \(g(x)=K\). Then
\[
 d^{(b)}(deduction; x)\ \ge\ \sum_{n=b+1}^{K-1}\omega_n.
 \tag{C.7}
\]

*Proof.* Let \(\gamma:[0,1]\to\mathbb R^d\) be a rectifiable path from \(a\) to \(x\). For \(b<n<K\) put \(\sigma_n=\sup\{t:\gamma(t)\in\overline{\{g\le n-1\}}\}\) (the set contains \(0\)) and \(\tau_n=\inf\{t>\sigma_n:\gamma(t)\in\overline{\{g\ge n+1\}}\}\) (the set contains \(1\), since \(g(x)=K\ge n+1\); and \(\sigma_n<1\) unless \(\omega_n=0\), in which case there is nothing to prove for this \(n\)). On \((\sigma_n,\tau_n)\) the path avoids \(\{g\le n-1\}\) and \(\{g\ge n+1\}\), so \(g=n\) there and the local unit in (C.1) is \(M\max(h_n,h_b)=Mh_n\). The Euclidean length of \(\gamma|_{[\sigma_n,\tau_n]}\) is at least \(\operatorname{dist}_2(\{g\le n-1\},\{g\ge n+1\})\ge\omega_nMh_n\). Hence this piece has capped graded length \(\ge\omega_n\). For \(n<n'\) every \(t\in(\sigma_n,\tau_n)\) has \(g(\gamma(t))=n\le n'-1\), so \(\sigma_{n'}\ge\tau_n\): the pieces are disjoint. Summing gives (C.7). \(\square\)

**Lemma C2 (from the record to its anchor).** For a record \(\rho\) of birth \(b\), any \(a\in q_\rho\) and any \(x\):
\[
 d^{(b)}(x,a)\ \le\ d_g(x,\cup E_\rho)+\delta_b(E_\rho)+2\sqrt d.
 \tag{C.8}
\]

*Proof.* Let \(p\in\cup E_\rho\), \(p\in c\in E_\rho\), and let \(T\) be a tree graph meeting all cubes of \(E_\rho\). Go from \(p\) straight to a point of \(T\cap c\) (length \(\le\sqrt d\,s_b\)), along \(T\) to a point of \(T\cap q_\rho\) (length \(\le|T|\)), and straight to \(a\) (length \(\le\sqrt d\,s_b\)). The capped unit is \(\ge Mh_b=s_b\) everywhere, so this path has \(\ell^{(b)}\le(|T|+2\sqrt d\,s_b)/s_b\). Take the infimum over \(T\) and over \(p\), and use \(d^{(b)}\le d_g\). \(\square\)

### 4.3 The theorem

Put \(S_d(t)=\sum_{j\ge0}(j+1)^de^{-tj}\) and
\[
 \Gamma_b=\begin{cases}1,& b=K,\\ L^d\,e^{C_0}\,e^{-\gamma(K-1-b)},&1\le b\le K-1.\end{cases}
 \tag{C.9}
\]

**Theorem C.** Assume the setting of §4.1 with \(\nu>0\), \(0\le\chi\le\nu/(4M)\), and (Geo) with \(c=\nu/4\). Then for every \(m\ge1\), every \(i_1\in I\) and every \(z\in D_{P/2}\),
\[
 \sum_{\rho\in\mathcal R}\ \sum_{i_2,\dots,i_m\in I}
 e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}\,
 \bigl|\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)\bigr|
 \ \le\ \frac{C_a\,C_b^{\,m-1}\,((m-1)!)^{d+1}}{P^m}\ \sum_{b=1}^{K}\Gamma_b\,\mathcal A_b\!\left(\tfrac\nu2+1\right),
 \tag{C.10}
\]
with
\[
 C_a=3^dS_d(\nu/8)\exp\Bigl\{3+\nu\Bigl(\tfrac12+\tfrac{\sqrt d}2+\tfrac1{16}\Bigr)\Bigr\},\qquad
 C_b=2n_I(2M+1)^d\Bigl[(2d)^d+\Bigl(\frac{8de}{\nu}\Bigr)^d\Bigr].
 \tag{C.11}
\]
The constants depend only on \(d,M,\nu,n_I\); the right side depends on the family only through \(\sum_b\Gamma_b\mathcal A_b\). In particular (\(m=2\)) the weighted Hessian row satisfies
\[
 \sup_i\sum_{l}e^{\chi|x_i-x_l|_\infty}\Bigl|\partial_i\partial_l\sum_\rho F_\rho(z)\Bigr|\le\frac{C_aC_b}{P^2}\sum_b\Gamma_b\mathcal A_b\!\left(\tfrac\nu2+1\right),
 \tag{C.12}
\]
and (\(m=1\)) \(\sup_i|\partial_i\sum_\rho F_\rho|\le C_aP^{-1}\sum_b\Gamma_b\mathcal A_b(\nu/2+1)\).

Since the minimal tree length satisfies \(\tau(i_1,\dots,i_m)\le(m-1)\max_s|x_{i_1}-x_{i_s}|_2\le(m-1)\sqrt d\max_s|\cdot|_\infty\), (C.10) contains the divided-tree weight \(e^{\sigma\tau/m}\) of (AB17.5) for \(\sigma\le\chi/\sqrt d\).

*Proof.* Fix \(\rho\) of birth \(b\), write \(E=E_\rho\), \(d_s=d_g(x_{i_s},\cup E)\), \(u=\delta_b(E)+2\).

*Step 1 (Cauchy).* Let \(s^*\) maximize \(d_s\). Then \(\partial_{i_1}\cdots\partial_{i_m}F_\rho=\partial^\alpha(\partial_{i_{s^*}}F_\rho)\) with \(|\alpha|=m-1\). For \(z\in D_{P/2}\) the polydisc of radius \(P/2\) about \(z\) lies in \(D_P\); Cauchy's estimate and (C.5) give
\[
 |\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)|\le\alpha!\Bigl(\frac2P\Bigr)^{m-1}\frac{w_\rho}{P}e^{-\nu\max_sd_s}\le(m-1)!\,\frac{2^{m-1}w_\rho}{P^m}e^{-\nu\max_sd_s}.
\]

*Step 2 (weight).* By (C.2), \(\operatorname{dist}_\infty(x_{i_s},\cup E)\le Md_s\), and by Lemma A3, \(\operatorname{diam}_\infty(\cup E)\le s_b(\delta_b(E)+2)\le Mu\). Hence \(\max_s|x_{i_1}-x_{i_s}|_\infty\le Mu+2M\max_sd_s\) and, as \(2\chi M\le\nu/2\),
\[
 e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}e^{-\nu\max_sd_s}\le e^{\chi Mu}e^{-\frac\nu2\max_sd_s}\le e^{\chi Mu}\,e^{-\frac\nu4d_1}\prod_{s=2}^me^{-a d_s},\qquad a=\frac{\nu}{4(m-1)}
\]
(for \(m=1\) the product is empty).

*Step 3 (sum over \(i_2,\dots,i_m\)).* Sites with \(d_g(x_i,\cup E)\le t\) lie within sup-distance \(Mt\) of \(\cup E\), hence in a cube of side \(Mu+2Mt\); so their number is \(N(t)\le n_I(Mu+2Mt+1)^d\le n_I(2M+1)^d(u+1+t)^d\). Therefore
\[
 \sum_ie^{-ad_g(x_i,\cup E)}=\int_0^\infty ae^{-at}N(t)\,dt\le n_I(2M+1)^d\sum_{j=0}^d\binom dj(u+1)^{d-j}\frac{j!}{a^j}\le n_I(2M+1)^d\Bigl(u+1+\frac da\Bigr)^d.
\]
With \(N=d(m-1)\) and \(B=d/a=4d(m-1)/\nu\): \((u+1+B)^N\le2^N((u+1)^N+B^N)\), \((u+1)^N\le N!\,e^{u+1}\), \(N!\le d^N((m-1)!)^d\), \(B^N=(4d/\nu)^N(m-1)^{d(m-1)}\le(4de/\nu)^N((m-1)!)^d\). So
\[
 \prod_{s=2}^m\sum_{i_s}e^{-ad_s}\le\bigl[n_I(2M+1)^d\bigr]^{m-1}((m-1)!)^d\,e^{u+1}\Bigl[(2d)^d+\Bigl(\frac{8de}\nu\Bigr)^d\Bigr]^{m-1}.
\]
Collecting,
\[
 \sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}|\partial^mF_\rho(z)|
 \le\frac{w_\rho}{P^m}\,C_b^{\,m-1}((m-1)!)^{d+1}\,e^{(\chi M+1)u+1}\,e^{-\frac\nu4d_g(x_{i_1},\cup E)}.
\]

*Step 4 (root to anchor).* For each grid cube \(q\in\mathcal G_b\) meeting \(\overline{\{g\le b\}}\) fix once a point \(a_q\in q\cap\overline{\{g\le b\}}\). By Lemma C2, \(e^{-\frac\nu4d_g(x_{i_1},\cup E)}\le e^{\frac\nu2\sqrt d}e^{\frac\nu4\delta_b(E)}e^{-\frac\nu4d^{(b)}(x_{i_1},a_{q_\rho})}\). Since \(\chi M+1+\nu/4\le\nu/2+1\) and \(e^{(\chi M+1)2+1}\le e^{3+\nu/2}\),
\[
 \sum_{\rho}\ \sum_{i_2,\dots,i_m}(\cdots)\le\frac{C_b^{\,m-1}((m-1)!)^{d+1}}{P^m}e^{3+\frac\nu2+\frac\nu2\sqrt d}\sum_{b=1}^K\mathcal A_b\!\left(\tfrac\nu2+1\right)\sum_{q}e^{-\frac\nu4d^{(b)}(x_{i_1},a_q)} ,
\]
the inner sum over the cubes \(q\in\mathcal G_b\) meeting \(\overline{\{g\le b\}}\).

*Step 5 (anchor sum).* By (C.2) and Lemma C1, \(d^{(b)}(x_{i_1},a_q)\ge\frac12\sum_{n=b+1}^{K-1}\omega_n+\frac12|x_{i_1}-a_q|_\infty/M\). The centre of \(q\) is within \(s_b/2\le M/2\) of \(a_q\) in sup norm. The number of grid cubes whose centres have sup-distance in \([jM,(j+1)M)\) from \(x_{i_1}\) is at most \((2(j+1)M/s_b+1)^d\le(3(j+1))^dL^{d(K-b)}\). With \(c=\nu/4\):
\[
 \sum_qe^{-c\,d^{(b)}(x_{i_1},a_q)}\le e^{c/4}\,3^dS_d(c/2)\,L^{d(K-b)}e^{-\frac c2\sum_{n=b+1}^{K-1}\omega_n}\le e^{\nu/16}3^dS_d(\nu/8)\,\Gamma_b ,
\]
by (C.4) for \(b\le K-1\) (note \(L^{d(K-b)}=L^dL^{d(K-1-b)}\)), and trivially for \(b=K\). This gives (C.10). \(\square\)

### 4.4 Remarks on the hypotheses

1. **What pays the fine-site multiplicity.** There are \(L^{d(K-b)}\) scale-\(b\) anchors per current cube. Lemma C2 converts the record's own tree (in scale-\(b\) cubes) and the kernel distance (graded) into one capped distance to the anchor; Lemma C1 says that distance crosses every layer between grade \(b\) and grade \(K\). Condition (C.4) is the precise statement that the crossings pay \(L^d\) per grade *on aggregate*. No per-record age factor \(e^{-\Gamma(k-j)}\) is assumed in (Loc); it is derived.
2. **Thin layers are allowed.** (C.4) is an aggregate condition on suffix sums. Call a layer *thick* if \((\nu/8)\omega_n\ge d\log L+\gamma\). If all layers are thick, (C.4) holds with \(C_0=0\); in the ordinary source geometry (S11) \(\omega_n\ge2R_n\), so this is the case as soon as \(\nu R_{\min}/4\ge d\log L+\gamma\). Layers with no lower bound at all (\(\omega_n=0\)) can be absorbed in two ways. (i) If the *total* number of non-thick layers is at most \(N_0\), take \(C_0=N_0(d\log L+\gamma)\), i.e. a factor \(e^{C_0}=L^{dN_0}e^{\gamma N_0}\), which is polynomial in \(R\) when \(L^{N_0-1}\le R\). (ii) If the non-thick layers come in runs of at most \(N_0\) consecutive grades, each run is immediately followed by its own layer \(n^*\le K-1\) with \((\nu/8)\omega_{n^*}\ge(N_0+1)(d\log L+\gamma)\) (for instance \(\omega_{n^*}\ge2R\) and \(\nu R/4\ge(N_0+1)(d\log L+\gamma)\)), and all other layers are thick, then (C.4) holds with \(C_0=0\): every suffix sum that contains part of a run also contains that run's \(n^*\), which pays for the run and for itself. (Distinct runs need distinct compensating layers; one layer shared by two runs does not suffice.)
3. **Polynomial age factors.** If \(w_\rho\) carries a factor \((1+K-b)^{b_0}\) (as in (AB17.9)), it is absorbed by \(e^{-\gamma(K-1-b)}\) in \(\Gamma_b\).
4. **A sufficient condition for (Loc).** If \(F_\rho(z)=f_\rho(\Phi(z))\), where \(f_\rho\) is holomorphic and bounded by \(w_\rho\) on the ball of radius \(r\) (in some norm \(\|\cdot\|_\rho\) on the native data restricted to the carrier) around every \(\Phi(z)\), \(z\in D_P\), and \(\|\partial_i\Phi(z)\|_\rho\le(r/P)e^{-\nu d_g(x_i,\cup E_\rho)}\), then (C.5) holds, by Cauchy's estimate in the direction \(\partial_i\Phi(z)\). This is the "native directional disc" argument of (AB17.19); whether its two inputs hold on the actual common contour is premise P2.
5. **Relation to the finite-cutoff construction statement (R20).** (R20) asked for \(\sup_i\sum_Xb_Xe^{\lambda\operatorname{diam}X}e^{-\nu\operatorname{dist}(i,X)}<\infty\) with the *physical* distance. With physical distance and fine births that sum cannot be uniformly bounded in general (the multiplicity \(L^{d(K-b)}\) is unpaid). Theorem C is the corrected statement: the distance in (Loc) must be the graded one, and then the sum is bounded under (Geo).

## 5. Part D — the age estimate inside a prepared component

### 5.1 the finite-cutoff construction objection, restated

Inside an eligible component, the last \(N_0\) prepared collars are one cube wide at their scales (S10), and \(\sum_{r}Mh_r<Mh_k/(L-1)\): a path crossing all of them fits in a bounded number of current cubes. So a factor measured in current-grid volume, such as \((\kappa_1-1)M^{-d}|Y'_i|\) in (1.66), cannot be charged once per grade. (CR.Summation over roots with hidden holes) charged \(\min\{\beta_{\rm s}\kappa,\delta M,\kappa_1-1\}\) per grade without assigning grades to factors. The required bound is on the unsimplified transport, with each factor measured in its native grade.

Theorem D supplies the alternative bound: the prepared grades do not need to be charged at all.

### 5.2 Setting and theorem

Fix \(d\ge1\), integer \(L\ge2\), \(M\ge1\), \(k\ge2\), \(h_j=L^{j-k}\). Let \(Z\subset\mathbb R^d\) be contained in a cube of side \(D_ZM\), and let
\[
 \emptyset=W_0\subset W_1\subset\cdots\subset W_k\subset Z,\qquad W_{k+1}:=\mathbb R^d,
\]
be closed sets. Define the grade \(g(x)=\min\{j\ge0:x\in W_{j+1}\}\in\{0,\dots,k\}\) and, for \(1\le b\le k\), the capped graded distance \(d^{(b)}\) as in (C.1) with unit \(M\max(h_{\max(g(x),1)},h_b)\). Let \(0\le N_0\le k-1\), \(\omega>0\), \(D_{\rm col}>0\), and assume

- **(D1)** \(\operatorname{dist}_2(W_j,\mathbb R^d\setminus W_{j+1})\ge\omega Mh_j\) for \(1\le j\le k-N_0-1\) *(charged layers)*;
- **(D2)** \(\operatorname{dist}_2(W_k,\mathbb R^d\setminus Z)\ge D_{\rm col}M\).

For \(1\le b\le k-1\) let \(A_b\subset Z\) be a set of points with pairwise sup-distance \(\ge Mh_b\) such that

- **(D3)** \(A_b\subset W_{b+1}\) if \(b\le k-N_0-1\) *(old births are grade-faithful)*;
- **(D4)** \(\operatorname{dist}_2(a,\mathbb R^d\setminus Z)\ge D_{\rm col}M\) for \(a\in A_b\) if \(b\ge k-N_0\) *(recent births are deep)*.

No hypothesis is made on the layers \(W_{j+1}\setminus W_j\) with \(j\ge k-N_0\).

**Theorem D (age-free anchor sum).** For every \(c>0\) with \(q:=L^de^{-c\omega}<1\),
\[
 \sum_{b=1}^{k-1}\ \sum_{a\in A_b}\exp\bigl\{-c\,d^{(b)}(deduction; \mathbb R^d\setminus Z)\bigr\}
 \ \le\ (D_Z+1)^d\,L^{d(N_0+1)}\,e^{-cD_{\rm col}}\Bigl[N_0+\frac1{1-q}\Bigr].
 \tag{D.1}
\]
The right side does not depend on \(k\).

*Proof.* Open sup-norm cubes of side \(Mh_b\) centred at the points of \(A_b\) are disjoint and lie in a cube of side \(D_ZM+Mh_b\); so \(|A_b|\le(D_ZL^{k-b}+1)^d\le(D_Z+1)^dL^{d(k-b)}\).

Let \(\gamma:[0,1]\to\mathbb R^d\) be a path from \(a\in A_b\) to a point outside \(Z\). The unit in (C.1) never exceeds \(M\), so \(\ell^{(b)}(\gamma)\ge|\gamma|/M\).

*Recent births, \(b\ge k-N_0\).* By (D4), \(\ell^{(b)}(\gamma)\ge D_{\rm col}\). Their total contribution is at most \(\sum_{b=k-N_0}^{k-1}(D_Z+1)^dL^{d(k-b)}e^{-cD_{\rm col}}\le(D_Z+1)^dN_0L^{dN_0}e^{-cD_{\rm col}}\).

*Old births, \(b\le k-N_0-1\).* By (D3), \(a\in W_{b+1}\subset W_j\) for all \(j\ge b+1\). For \(b+1\le j\le k-N_0-1\) let \(\sigma_j=\sup\{t:\gamma(t)\in W_j\}\) and \(\tau_j=\inf\{t>\sigma_j:\gamma(t)\notin W_{j+1}\}\). On \((\sigma_j,\tau_j)\), \(\gamma\in W_{j+1}\setminus W_j\), so \(g=j>b\) and the unit is \(Mh_j\); the Euclidean length of this piece is \(\ge\operatorname{dist}_2(W_j,\mathbb R^d\setminus W_{j+1})\ge\omega Mh_j\) by (D1). So each such piece has capped length \(\ge\omega\). Let \(\sigma_k=\sup\{t:\gamma(t)\in W_k\}\); the piece \(\gamma|_{[\sigma_k,1]}\) has Euclidean length \(\ge D_{\rm col}M\) by (D2), hence capped length \(\ge D_{\rm col}\). As in Lemma C1 the pieces are pairwise disjoint (points of \((\sigma_j,\tau_j)\) lie in \(W_{j+1}\subset W_{j'}\) for \(j'>j\), so \(\sigma_{j'}\ge\tau_j\); and \(\sigma_k\ge\tau_j\) for all \(j\le k-1\)). Hence
\[
 d^{(b)}(deduction; \mathbb R^d\setminus Z)\ge\omega\,(k-N_0-1-b)+D_{\rm col}.
\]
Their total contribution is at most
\[
 \sum_{b\le k-N_0-1}(D_Z+1)^dL^{d(k-b)}e^{-c\omega(k-N_0-1-b)}e^{-cD_{\rm col}}\le(D_Z+1)^dL^{d(N_0+1)}e^{-cD_{\rm col}}\sum_{m\ge0}q^m.\qquad\square
\]

### 5.3 The source numbers source input; conditional

In an eligible component of an R step at scale \(k\), take \(W_j=Z''_j\) (S10). Then:

- \(D_Z=100R_k\) (S1).
- **(D2) with \(D_{\rm col}\ge10R_k\).** \(Z''_k=(\Omega^{\sim5}_{k-N_0+1})^c\cap Z\subset\Omega_{k-N_0+1}^c\cap Z\subset Z_{k-N_0+1}\cap Z\). By S1(ii) no large field was created in the component during the last \(N>N_0\) steps, so \(Z\cap Z_j=S(Z\cap Z_{j-1})\) for \(h<j\le k\), where \(S\) adds ten layers of \(MR_j\)-cubes (LFR II p.384, source). Thus for \(N_0\ge2\), \(\operatorname{dist}(Z''_k,Z^c)\ge\operatorname{dist}(Z_{k-1}\cap Z,Z^c)\ge10MR_k\).
- **\(N_0\) and the multiplicity.** \(L^{N_0-1}=R_{k-N_0+1}=:R_\#\) (S10), so \(L^{d(N_0+1)}=L^{2d}R_\#^{\,d}\) and \(N_0=1+\log_LR_\#\). By CMP119 (2.9) (p.256: \(R_m\le(L+1)(n-m)^{\beta_0}R_n\) for \(m<n\)), \(R_\#\le(L+1)N_0^{\beta_0}R_k\).
- **(D1).** For \(j\le h-1\) the layer between \(Z_j\) and \(Z_{j+1}^c\) contains ten layers of \(MR_{j+1}\)-cubes (S1), i.e. \(\omega\ge10LR_{j+1}\). For \(h\le j\le k-N_0-1\) the layer between \((\Omega_j^{\sim5})^c\) and \(\Omega_{j+1}^{\sim5}\): since \(\Omega_{j+1}^c\) contains \(Z_j\supset\Omega_j^c\) enlarged by at least eight layers of scale-\((j+1)\) \(MR_{j+1}\)-cubes (S11), at least three such layers remain after the five-layer enlargement of \(\Omega_{j+1}\); so \(\omega\ge3LR_{j+1}\). *(This last count is the interpretation of S10–S11 in the source; the exact number of layers should be rechecked against CMP119 pp.264–269. Any \(\omega\) with \(L^de^{-c\omega}<1\) suffices.)*
- **(D3)–(D4).** A record of birth \(b<k\) is anchored at a scale-\(b\) cube meeting \(Z_b\) (S12). If the anchor is inside the component: for \(b\le h\), \(Z_b=Z''_b\subset W_{b+1}\); for \(h<b\le k-N_0-1\), \(Z_b\subset\Omega_{b+1}^c\) and \(Z''_{b+1}=(\Omega_{b+1}^{\sim5})^c\) contains \(Z_b\) with the same three-layer margin, so the anchor lies in \(W_{b+1}\) (D3). For \(b\ge k-N_0\): \(Z_b\cap Z\subset Z_{k-1}\cap Z\), at distance \(\ge10MR_k\) from \(Z^c\); with the anchor cube this gives (D4) with \(D_{\rm col}=10R_k-1\). The new boundary terms created by the \(N\) preparatory integrations are anchored at the boundary of an integration shell \(Z_{j+1}\setminus Z''_{j+1}\) and carry scale \(j+1\); the same inclusions put them in case (D3) or (D4). *(an additional hypothesis: the birth labels and anchors of the preparatory terms are not displayed in LFR I; It follows them from "we can use the results of the third section" [III].)*

**Corollary D2.** With these numbers and any \(c>0\), \(\omega\) with \(L^de^{-c\omega}\le\frac12\),
\[
 \sum_{b<k}\sum_{a\in A_b}e^{-c\,d^{(b)}(deduction; Z^c)}\le(100R_k+1)^d\,L^{2d}R_\#^{\,d}\,(3+\log_LR_\#)\,e^{-c(10R_k-1)}.
 \tag{D.2}
\]
This tends to zero as \(R_k\to\infty\), uniformly in \(k\) and in the ages \(k-b\).

### 5.4 Which factor of (1.66) pays what

The three factors of (1.66) (S8) are: the record's own tree \(\beta\kappa d_j(X)\) (in scale-\(j\) cubes); the distance factor \(\delta\,d((Y^0_{i_0})^c\cap Y_1\cap Y'_{i_0},X)\) (scaled distance); the current-grid volumes \((\kappa_1-1)M^{-d}|Y'_i|\).

- **Physical depth \(D_{\rm col}\).** Consider a record \(X\) lying in one component \(Z_1\) of \(Z\), anchored at depth \(\ge D_{\rm col}M\). Then \(Y_1=Z_1\) (S9: the smallest domain containing \(X\) and the components of \(Z\) meeting \(X\)), and the boundary layer \(Y_1\setminus Y_1^0\) lies within \(2M_1\) of \(Z_1^c\). For a term with some \(Y'_i\ne\emptyset\), the own tree of \(X\) (from the anchor to the point of \(X\) nearest the layer) followed by the gap measured by the distance factor is a connection from the anchor to within \(2M_1\) of \(Z^c\). Both are measured in units \(\le\) one current \(M\)-cube. Hence, if \(\delta'\) denotes the decay rate of the distance factor per current \(M\)-cube, their product is \(\le\exp\{-\min(\beta\kappa,\delta')(D_{\rm col}-2M_1/M-2)\}\), *however the connection is split between the two*. For an exceptional nonself term (all \(Y'_i=\emptyset\), \(Y_0\setminus Z\ne\emptyset\)) the carrier \(X\) itself leaves \(Z\), and the own tree alone gives the same bound. No assignment of grades to factors is needed. By Theorem D this pays the whole multiplicity of the prepared grades and of the recent births. *(If, as Conjecturally, but did not verify, every component of \(\Lambda\) lies at depth \(\ge D_{\rm col}M\), then the volume factor of the first nonempty \(Y'_i\), whose components join \(\Lambda\) to the boundary layer, gives an independent \(e^{-(\kappa_1-1)(D_{\rm col}-O(1))}\).)*
- **Unprepared grades of old births** (\(b\le k-N_0-1\)). Here the multiplicity \(L^{d(k-N_0-b)}\) is unbounded in the age, and a flat (current-unit) payer gives only \(e^{-cD_{\rm col}}\). A graded payer is necessary. The own tree is graded automatically (Lemma C2: it is measured in scale-\(b\) cubes). The current-grid volume is *not* graded and is not used. The distance factor is graded **if** its scaled distance is that of a determining set which still contains the old layers.

**Premise GP (graded payment).** For a record \(X\in\mathbf D_b\) with anchor in the component, the distance factor in (1.66) satisfies
\[
 d\bigl((Y^0_{i_0})^c\cap Y_1\cap Y'_{i_0},X\bigr)\ \ge\ c_{\rm GP}\,d^{(b)}\bigl(\cup X,\ \mathbb R^d\setminus Z\bigr)-C_{\rm GP}
\]
for each \(i_0\in\{2,3,4\}\), where \(d^{(b)}\) is the capped graded distance of the *prepared* sequence \(\{Z''_j\}\).

**Evidence for GP (an additional hypothesis).**

1. *The printed list.* S8 lists four functions whose decay produces the distance factor: \(\mathbf H''_k\), \(\mathbf H_{\mathbf B_1}\), \(\mathbf H_k\) **and** \(\mathbf H(\mathbf B''_k(Y_1),\cdot)\). The first three are the functions localized by \(Y'_2,Y'_3,Y'_4\) in (1.61)–(1.63). The fourth is the response function of the configuration \(U(\mathbf B''_k(Y_1),\cdot)\) of (1.61).
2. *Structure of (1.61).* By S9, on \(Y_1\) the old background is \(U(\mathbf B''_k(Y_1);\ \text{boundary-layer data},\ \text{unchanged interior fields})\). The later representations (1.62), (1.63) and the fields of \(\Lambda\) enter *only* through the boundary-layer data on \((Y_1^0)^c\cap Y_1\), a layer of width \(\le2M_1\) at \(\partial Y_1\). Hence, for every \(i_0\), the dependence of a record \(X\subset Y_1\) on anything outside its own interior data passes through \(U(\mathbf B''_k(Y_1),\cdot)\), from the boundary layer of \(Y_1\) to \(X\). The factor carries "\(\cap Y_1\)" for every \(i\), consistently.
3. *The determining set.* \(\mathbf B''_k(Y_1)=\mathbf B(Y_1)\cup\mathbf B''_k\) coincides with the prepared set \(\mathbf B''_k\) on \(Y_1^0\). By S13 the scaled distance of a determining sequence measures each layer in its own mesh. So the scaled distance of \(\mathbf B''_k(Y_1)\) from \(\partial Y_1\) to a record deep in the component crosses the prepared layers \(Z''_{j+1}\setminus Z''_j\) in their own units, which is GP.
4. *Consistency.* The source sums over \(j\) at fixed \(Y\) with only these factors ("For the boundary terms we have just the summations over \(X\) and \(j\)", p.376). The geometric rules S1–S2 alone do not exclude a number of scale-\(b\) regions inside one component that grows exponentially with \(k-b\) (components may merge, and are then replaced by the enclosing parallelepiped). With a flat distance such a configuration is not controlled by the displayed factors (see the obstruction below). So either the distance is graded, or the resummation tacitly uses the large-field factors of the component; the second alternative is not available for the normalized expression.

This is an inference from a terse text. It is the per-map assignment needed by the finite-cutoff construction; it is not a proof that the source's estimate holds.

**Obstruction to any flat-metric proof.** Take \(d\ge1\), \(A_b\) a full grid of mesh \(Mh_b\) in a cube of side \(M\) at depth \(D_{\rm col}M\) in \(Z\), for every \(b<k\) (so (D3) fails for old \(b\)), and a weight depending only on the *physical* distance to \(Z^c\). Then \(\sum_b\sum_{a\in A_b}e^{-c\operatorname{dist}(a,Z^c)/M}\ge\sum_{b<k}L^{d(k-b)}e^{-c(D_{\rm col}+1)}\), which is unbounded in \(k\). So an anchored age estimate cannot be obtained from factors that decay only in current units, unless the number of old anchors is limited by some other input. This confirms the finite-cutoff construction objection in the form: *the current-grid volume cannot pay unprepared grades*; and it shows that (D3) (grade-faithful anchoring) together with a graded payer is exactly what is needed.

### 5.5 The replacement for (CR.Summation over roots with hidden holes)–(CR.Noneligible components and the sum over births) conditional

**Proposition D3.** In the setting of §5.2, let \(\mathcal R^{\rm in}\) be a finite family of incoming records; each \(\rho\) has a birth \(b<k\), a finite set \(E_\rho\) of scale-\(b\) cubes with an anchor cube \(q_\rho\in E_\rho\) whose centre \(a_\rho\) satisfies (D3)/(D4), distinct anchor cubes giving distinct centres, and a number \(v_\rho\ge0\). Suppose \(\Phi_\rho\ge c_1\delta_b(E_\rho)+c_2\,d^{(b)}(\cup E_\rho,\mathbb R^d\setminus Z)\) with \(c_1,c_2>0\), and put \(c=\min(c_1,c_2)/2\). If \(L^de^{-c\omega}\le\frac12\), then
\[
 \sum_{\rho\in\mathcal R^{\rm in}}v_\rho\,e^{-\Phi_\rho}
 \le e^{2c\sqrt d}\ \Bigl[\sup_{b<k}\ \sup_q\sum_{\rho:\,b(\rho)=b,\ q_\rho=q}v_\rho\,e^{-(c_1-c)\delta_b(E_\rho)}\Bigr]\ (D_Z+1)^dL^{d(N_0+1)}(N_0+2)\,e^{-cD_{\rm col}}.
 \tag{D.3}
\]

*Proof.* As in Lemma C2, \(d^{(b)}(a_\rho,Z^c)\le d^{(b)}(\cup E_\rho,Z^c)+\delta_b(E_\rho)+2\sqrt d\). Hence \(\Phi_\rho\ge(c_1-c)\delta_b(E_\rho)+c\,d^{(b)}(a_\rho,Z^c)-2c\sqrt d\) (using \(c\le c_2\); \(c\le c_1/2\) only keeps \(c_1-c>0\)). The anchor cubes are cubes of the fixed grid \(\mathcal G_b\), so their centres are \(Mh_b\)-separated and Theorem D applies. Sum first over the records with a given anchor cube, then over anchors by Theorem D. \(\square\)

**Use.** With \(v_\rho e^{-\Phi_\rho}\) the bound of the sum of all terms of record \(\rho\) whose final localization leaves the component (the source's (1.66) after its resummation over \(Y'_i\)), \(c_1=\beta\kappa\), and \(c_2\) from GP, (D.3) says:

> *the total contribution of all older births to the nonself output of one eligible component is at most (the supremum over births of their own-scale rooted norms) times \(C\,R_k^{2d}\log R_k\,e^{-c(10R_k-1)}\).*

There is no factor \(L^{4(k-b)}\) left and no age weight is required. In the notation of Annex AU this replaces (CR.Noneligible components and the sum over births) by
\[
 \text{(contribution of all births } b<k\text{ to a fixed new root)}\ \le\ \zeta'_k\,\sup_{b<k}A_b,\qquad
 \zeta'_k\le C R_k^{2d}\log R_k\,e^{-c(10R_k-1)},
\]
and the recurrence (CR.23)–(CR.25) by the elementary
\[
 A_k\le C_{\rm fresh}\zeta_k\bigl(F_0+\sup_{b<k}A_b\bigr)\ \Longrightarrow\ \sup_kA_k\le 2C_{\rm fresh}F_0\sup_k\zeta_k\quad\text{if }C_{\rm fresh}\sup_k\zeta_k\le\tfrac12 ,
\]
(induction on \(k\) with \(A_0=0\)). The weighted norm \(\mathcal A_k=\sum_be^{-\lambda(k-b)}A_{b,k}\) and the threshold (CR.Summation over roots with hidden holes) \(\Gamma_{\rm v}>4\log L+\lambda+\dots\) are not needed.

**Records anchored outside the component.** A record of birth \(b<k\) whose anchor lies in another component of \(Z_k\) and whose carrier reaches \(Z\) crosses a gap of at least \(R_k\) scale-\(k\) cubes (S2), i.e. \(R_kL^{k-b}\) of its own cubes; by (A.2), \(\delta_b(E)\ge R_kL^{k-b}-2\), so its own tree gives \(e^{-\beta\kappa(R_kL^{k-b}-2)}\). Rooting such records at a scale-\(b\) cube in \(Z\): \(\sum_{b<k}(D_Z+1)^dL^{d(k-b)}e^{-c(R_kL^{k-b}-2)}\le(D_Z+1)^de^{2c}\sum_{n\ge1}L^{dn}e^{-cR_kL^n}\), which is \(\le 2(D_Z+1)^dL^de^{2c-cR_kL}\) once \(cR_kL(L-1)\ge d\log L+\log2\) (the ratio of consecutive terms is then \(\le\frac12\)). Here \(c<\beta\kappa\), the remainder \(\beta\kappa-c\) being kept for the rooted own-scale sum, and the count is of scale-\(b\) grid cubes contained in \(Z\). deduction, given S2.

**What Proposition D3 does not do.** It does not prove (1.66) or its resummation over \(Y'_i\); it does not prove GP; and it concerns values of the resummed activities on the source's analytic domain, not marked or differentiated families.

## 6. Assembly: a conditional theorem for the inherited-B and completed-R sectors conditional

### 6.1 Premises

Consider the fluctuation step from scale \(k\) to \(k+1\); in Part C take \(K=k+1\), grade \(n\) on \(\Omega_n\setminus\Omega_{n+1}\) (\(\Omega_{K+1}=\emptyset\)), current coordinates \(z=(z_i)_{i\in I}\) on the free bonds of \(\Lambda_{k+1}\subset\Omega_{k+1}\).

- **P1 (representation; source S7, S12).** On the fixed retained slice, the current-dependent part of the inherited boundary action and of the completed-component boundary action is \(\sum_{\rho\in\mathcal R}F_\rho(z)\), where each record \(\rho\) has a birth \(b\le k\) and a carrier \(X_\rho\in\mathbf D_b\) with \(X_\rho\cap Z_b^{\sim}\neq\emptyset\); records with the same birth and carrier have been summed into one. The eligible components of the R step at scale \(b\) form a tag family \(\mathcal Q_b\) with pairwise disjoint shells (S1, S2, \(R_b\ge2\)). Each record is of one of two kinds: *ordinary*, with \(E_\rho=X_\rho\) (no holes; full-tree norm); or *tagged*, with \(X_\rho\) admissible for \(\mathcal Q_b\) (T2), \(\mathcal H(X_\rho)\ne\emptyset\) and \(E_\rho=E(X_\rho)\). The multipliers \(\mathbf T'_b(Y)1\) are independent of \(z\). *(The alternative representation is used at every R step; this is the source's "final remark", stated without a displayed proof.)*
- **P2 (first-derivative bound on the common contour).** Each \(F_\rho\) is holomorphic on \(D_P\), \(P\) a fixed multiple of \(P_k\), and satisfies (Loc) (C.5) with the graded distance of the current sequence \(\{\Omega_n\}\) and
 \[
 w_\rho\le W_b\,e^{-\kappa_*\delta_b(E_\rho)},
 \]
 where \(W_b=W_b^{\rm ord}\) for records without tags and \(W_b=W_b^{\rm tag}\) for records with at least one tag. *(Source inputs: the pointwise bounds S12, S6/S7, and the analytic domains; analytic inputs: Annexes AO–AR, AD17, CR.2 for the common contour and the kernel rows. Not re-derived here.)*
- **P3 (geometry).** (Geo) holds for \(\{\Omega_n\}\) with \(c=\nu/4\); every ordinary record has a cube of \(E_\rho=X_\rho\) meeting \(\overline{\{g\le b\}}=\overline{\Omega_{b+1}^{\,c}}\) (a cube meeting \(Z_b^\sim\), which lies in \(\Omega_{b+1}^c\)), and for a tagged record *every* shell cube of each of its tags meets \(\overline{\{g\le b\}}\) (the shells lie in \(Z_b^\sim\subset\Omega_{b+1}^c\)); sites have density \(n_I\). *(Source: S11 gives \(\omega_n\ge2R_n\) in ordinary layers; thin prepared layers survive only inside failed-prefix components and are covered by Remark 4.4(2).)*

### 6.2 Theorem E

**Theorem E.** Assume P1–P3, \(0\le\chi\le\nu/(4M)\), and \(a:=\kappa_*-\nu/2-1>\kappa_{\rm cnt}(d)\); put \(\tau=\tau(a)\), \(S_b=2d(20R_b)^{d-1}\). Then for all \(m\ge1\), \(z\in D_{P/2}\),
\[
 \sup_{i_1}\sum_{\rho}\sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}|\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)|
 \le\frac{C_aC_b^{\,m-1}((m-1)!)^{d+1}}{P^m}\sum_{b\le k}\Gamma_b\Bigl[C_1(additional assumption; a)\,W_b^{\rm ord}+\frac{e^{a/2}\,e^{-\tau S_b}}{(2d)^2(1-e^{-\tau})}\,W_b^{\rm tag}\Bigr],
 \tag{E.1}
\]
with \(C_a,C_b\) from (C.11), \(\Gamma_b\) from (C.9), \(C_1\) from Proposition B2. All constants depend only on \(d,L,M,\nu,n_I,\gamma,C_0,\kappa_*\).

*Proof.* Choose anchors: for an ordinary record a cube of \(E_\rho=X_\rho\) meeting \(\overline{\{g\le b\}}\), supplied by P3; for a tagged record the lexicographically first cube of the shell of its lexicographically first tag. By P3 these are admissible anchors for Part C. For a fixed anchor cube \(q\), ordinary records with \(q_\rho=q\) are in one-to-one correspondence with distinct face-connected sets \(E\ni q\); tagged records with \(q_\rho=q\) are among the admissible \(X\) with \(S(Q)\subset E(X)\), where \(Q\) is the unique tag whose shell contains \(q\) (shells are disjoint), and \(X\mapsto E(X)\) is injective on them (Lemma A2(3)). Proposition B2 with weight \(e^{(\nu/2+1)\delta_b}\) gives \(\mathcal A_b^{\rm ord}(\nu/2+1)\le W_b^{\rm ord}C_1(d,a)\) and \(\mathcal A_b^{\rm tag}(\nu/2+1)\le W_b^{\rm tag}e^{a/2}(2d)^{-2}(1-e^{-\tau})^{-1}e^{-\tau S_b}\) (S1 and (A.1) for the shell size). Proposition B1(3) shows that \(d_g(x_i,\cup X_\rho)=d_g(x_i,\cup E_\rho)\) for the current sites, which lie outside \(Y^\sim\) for every tag (S11), so P2 may be stated with either. Apply Theorem C. \(\square\)

### 6.3 Reading (E.1) against the completion test

- **Volume.** No sum over the volume appears; (E.1) is a supremum over the root.
- **Depth/age.** The sum over births is \(\sum_b\Gamma_bW_b\) with \(\Gamma_b=L^de^{C_0}e^{-\gamma(k-b)}\); it converges if \(W_b\) grows at most subexponentially in the age.
- **Hidden carrier distance.** The diameter of a completed component does not appear. A tag contributes only the gain \(e^{-\tau S_b}\). The physical separation of two current roots on opposite sides of a component is paid by \(\delta_b(E)\) through (B.1).
- **Smallness.** With \(W_b^{\rm ord}=CB_0\theta_k(1+k-b)^{b_0}\) (the form claimed in (AB17.19)) the ordinary part of \(P^{-2}\times\)(E.1)\(_{m=2}\) is \(O(\theta_kP_k^{-2})\), as in (AB17.30). The tagged part is smaller than any power of \(g_b\): \(e^{-\tau S_b}\le\exp\{-2d\tau(20R_b)^{d-1}\}\) while \(g_b^{-2}=e^{\ell_b}\), \(R_b\ge\ell_b^{\,r}\).
- **Factorial growth.** \(((m-1)!)^{d+1}\); for \(d=4\) this is the power five of (AB17.5).

What (E.1) does **not** contain: the sectors listed in §0.3, and any statement on native-anchored jets.

| the finite-cutoff construction check | Status after this note |
|---|---|
| 1. Exact reduced representation | Unchanged; it is premise P1. |
| 2. Common contour, kernel tails | Needed only in the form P2: a first-derivative bound in the graded metric. Operator-norm localizers \(\pi_v^r\) for the normalized kernels are not needed on this route, because the kernel response is inside the source's analytic activity \(\mathbf B'^{(b)}(X,(\mathbf U,\mathbf J))\). |
| 3. Component and current-root loads | Component load: verified for the printed interactions, Cor. B3 conditional. Current-root load: replaced by Theorem C deduction, with rooted norms from Prop. B2 deduction. |
| 4. Persistence through repeated histories | Geometric part: tagged carriers are ordinary carriers (Prop. B1) at every later step, with no separation or collar premise. Value part: reduced to P1; the disputed age step is replaced by Theorem D/Prop. D3 deduction given GP additional assumption. |
| 5. Full proposition and HC interface | Unchanged. (E.1) with \(m=2\) has the form required by HC.18 for these sectors. |
