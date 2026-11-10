# A positive local Gaussian marginal construction for the ambient Gram extension

This note proves the Gaussian bridge for a fixed free-coordinate geometry. It uses exact normalized Gaussian marginals, so no independently modified cross operator or covariance square root appears in the integration formula. It does not address a change of history geometry or a completed residual-component quotient.

## 1. Input and the positive restriction family

Let the real independent Gaussian coordinates be indexed by a finite periodic lattice with a fixed number of coordinates per physical block. Their storage blocks form a graph of fixed polynomial growth. All carriers below are connected sets of physical blocks and contain the storage blocks of the matrix endpoints and every raw retained variable on which the coefficient depends.

Suppose a real matrix field has an actual supported expansion

\[
 B(v)=\sum_X B_X(v_X),\qquad \|B\|_{\nu}\le b_0,
 \qquad \nu>0,                                      \tag{GM.1}
\]

where the norm is the two-sided absolute row/column coefficient norm of PR.2. The retained functions can be smooth; holomorphy in the raw retained variables is not required here. In the application these are the locally cut off Gram coefficients. Fix \(\sigma>0\) and put

\[
 K=\sigma I+B^{\mathsf T}B,
 \qquad C=K^{-1}.                                   \tag{GM.2}
\]

For every set \(H\) of physical blocks, define

\[
 B^H=\sum_{X\subset H}B_X,\qquad
 K^H=\sigma I+(B^H)^{\mathsf T}B^H,
 \qquad C^H=(K^H)^{-1}.                             \tag{GM.3}
\]

The mass \(\sigma I\) is present everywhere, including outside \(H\). Thus every member of this family obeys

\[
 \sigma I\le K^H\le\Lambda I,
 \qquad \Lambda:=\sigma+b_0^2,                      \tag{GM.4}
\]

after harmless fixed norm-convention factors. It is independent of retained variables outside \(H\), and is a direct sum over the connected components of \(H\), with independent mass coordinates outside \(H\).

There is a useful exact restriction identity. Expand the Gram product into its individual pairs, and assign the pair \(B_X^{\mathsf T}B_Y\) the carrier \(X\cup Y\); a nonzero pair meets at its summed matrix index, so this carrier is connected. After pairing with the transpose or grouping pairs with the same carrier, write

\[
 K=\sigma I+\sum_Z A_Z,
 \qquad K^H=\sigma I+\sum_{Z\subset H}A_Z.           \tag{GM.5}
\]

The second equality is exact because \(X\subset H\) and \(Y\subset H\) are equivalent to \(X\cup Y\subset H\). This is stronger than merely compressing the summed precision to \(H\).

## 2. A common, restriction-consistent covariance expansion

### Lemma GM.1

There are a common set of tags \(\gamma\), fixed connected carriers \(X_\gamma\), and matrix coefficients \(C^H_\gamma\) such that, simultaneously for every \(H\),

\[
 C^H=\sum_\gamma C^H_\gamma,
 \qquad
 \sum_\gamma C^H_\gamma(i,j)=0
 \text{ termwise unless }i,j\in X_\gamma.             \tag{GM.6}
\]

The last clause means each summand vanishes unless both endpoint storage blocks belong to its carrier. For some \(\nu_1>0\), the expansion admits nonnegative entry majorants independent of \(H\) and \(v\), whose two-sided weighted row/column norm is at most a fixed \(c_C\). In particular,

\[
 \sup_i\sum_{\gamma}\sum_j e^{\nu_1|X_\gamma|}
       \sup_{H,v}|C^H_\gamma(i,j;v)|\le c_C,          \tag{GM.7}
\]

and similarly for columns. Every coefficient is a function of \(v\) restricted to \(X_\gamma\), and

\[
 H\cap X_\gamma=H'\cap X_\gamma
 \quad\Longrightarrow\quad C^H_\gamma=C^{H'}_\gamma.
                                                               \tag{GM.8}
\]

The coefficients can be chosen real symmetric, without changing these assertions.

#### Proof

Apply the constructive proof of PR.2 to the entire family (GM.5), with common choices. Its coefficient norm and gap are uniform in \(H\), so choose the same carrier truncation size \(n\). The finite-range matrix

\[
 K_n^H=\sigma I+\sum_{|Z|\le n,\,Z\subset H}A_Z
\]

has a uniform positive gap, since the omitted coefficient tail is uniformly exponentially small. Use the same fixed cube partition, local principal inverses, parametrix error series and tail Neumann series for every \(H\). The common tag \(\gamma\) records its local cubes, tail carriers, word lengths and summed matrix indices.

A local principal inverse on \(Q\) sees only primitive coefficient carriers in the fixed halo \(Q^{+n}\). If two restrictions agree there, its input matrix, hence its inverse, is identical. The same is true of the commutator-error coefficient. Every subsequent multiplication joins the declared carriers at a matrix index. Therefore its dependency on the set \(H\) and on the retained variables is confined to the declared union \(X_\gamma\). This proves (GM.8).

The proof gives the stronger common majorant (GM.7), not only separate bounds for each \(H\). The Combes–Thomas entry bound for every local inverse uses the same gap and the same primitive absolute first-moment bound. It is thus an entry majorant uniform in \(H\). Absolute commutator and primitive-tail bounds have the same property. Their nonnegative matrix products dominate the individual Neumann-word tags for every \(H\); the same geometric series sums them. These are precisely the majorants used in PR.1–PR.2, with the supremum over \(H\) now retained before their sums.

The construction is real. Pair each tagged matrix with its transpose, keeping the same carrier, to make it symmetric. The two-sided norm makes this operation contractive at the level of its common majorants. Its sum is unchanged because \(C^H\) is symmetric. This also preserves (GM.8). \(\square\)

In particular, writing \(\Lambda_{\rm lat}\) for the whole block set,

\[
 C-C^D=\sum_{\gamma:X_\gamma\not\subset D}
     \bigl(C^{\Lambda_{\rm lat}}_\gamma-C^D_\gamma\bigr).
                                                               \tag{GM.9}
\]

All terms with carrier contained in \(D\) cancel individually. There is no subtraction of two unrelated covariance localizations.

## 3. The exact local positive marginal and its analytic continuation

Let \(I\) be a finite union of coordinate supports and raw dependency footprints of the current Mayer and failed-cutoff factors. When necessary include raw blocks with no integrated coordinate in this definition. Let \(\mathscr I\) be the integrated coordinate indices belonging to those factors.

Choose a partition into cubes of a fixed large integer side \(m\). Define \(D=D(I)\) as the union of all cubes meeting the graph \(m\)-neighborhood of \(I\). Thus \(D\) is a union of partition cubes,

\[
 d(I,D^c)\ge m,\qquad |D|\le c_d m^d|I|.             \tag{GM.10}
\]

This choice is additive under unions: \(D(I_1\cup I_2)=D(I_1)\cup D(I_2)\).

The positive reference covariance for integration is the actual marginal

\[
 C_{I,0}:=P_{\mathscr I}C^D P_{\mathscr I}^{\mathsf T}.
                                                               \tag{GM.11}
\]

It depends only on raw retained variables in \(D\), and

\[
 \Lambda^{-1}I\le C_{I,0}\le\sigma^{-1}I.             \tag{GM.12}
\]

Introduce one parameter \(s_\Delta\) for each partition cube outside \(D\). For each tag in (GM.9), let \(O(\gamma)\) be the cubes outside \(D\) meeting \(X_\gamma\), and put

\[
 C_I(s)=C_{I,0}+
 \sum_{\gamma:X_\gamma\not\subset D}
 \left(\prod_{\Delta\in O(\gamma)}s_\Delta\right)
 P_{\mathscr I}\bigl(C^{\Lambda_{\rm lat}}_\gamma-C^D_\gamma\bigr)
 P_{\mathscr I}^{\mathsf T}.                          \tag{GM.13}
\]

Then \(C_I(1)=C_{\mathscr I\mathscr I}\), the exact full Gaussian marginal, and \(C_I(0)=C_{I,0}\).

### Lemma GM.2 — a large-polydisc small perturbation

For any fixed \(R>1\), the side \(m\) can be chosen sufficiently large, depending only on \(R,\nu_1,c_C,\sigma,\Lambda\), such that (GM.13) is analytic on \(|s_\Delta|\le R\) and

\[
 \|C_I(s)-C_{I,0}\|_{\rm row/column}
 \le \varepsilon_m,
 \qquad \varepsilon_m\longrightarrow0\quad(m\longrightarrow\infty),
                                                               \tag{GM.14}
\]

uniformly in \(I\), volume and real retained data. One may take

\[
 \varepsilon_m\le
 2c_C\exp\!\left(a_d\log R-\tfrac34\nu_1m\right),
 \quad m\ge4a_d\log R/\nu_1.                         \tag{GM.15}
\]

#### Proof

A connected lattice set \(X\) meets at most \(a_d(1+|X|/m)\) partition cubes. One proof colors the cubes by their coordinates modulo three. Cubes of one color are separated by a distance of order \(m\); a connected graph visiting \(k\) such cubes contains at least \(c m(k-1)\) edges. Summing over the fixed color set gives the asserted bound.

Consequently the parameter product in (GM.13) is bounded by
\(R^{a_d}\exp[(a_d\log R/m)|X_\gamma|]\). For an entry with first endpoint in \(\mathscr I\), a surviving carrier is connected, meets \(I\), and leaves \(D\). Therefore \(|X_\gamma|\ge m\). Spend at most one quarter of the weight in (GM.7) on the parameter product and use the rest on this lower bound. Sum the common tag majorants. The column estimate is identical. This proves (GM.14)–(GM.15) and normal convergence on the closed polydisc. \(\square\)

Choose \(m\) so \(u_m:=\Lambda\varepsilon_m<1/8\). The complex symmetric covariance (GM.13) is then invertible, and its inverse has positive real part. Define its density by the analytic determinant branch equal to the positive one at \(s=0\):

\[
 d\mu_{I,s}(z)=
 (2\pi)^{-r_I/2}\det C_I(s)^{-1/2}
 \exp\{-\tfrac12z^{\mathsf T}C_I(s)^{-1}z\}\,dz,
 \quad r_I=|\mathscr I|.                              \tag{GM.16}
\]

It is an exactly normalized complex Gaussian measure. Indeed it is the analytic Gaussian integral on a domain where the real part of its precision is positive, and its normalization agrees with one at the positive reference.

Writing
\(E_s=C_{I,0}^{-1/2}(C_I(s)-C_{I,0})C_{I,0}^{-1/2}\), one has \(\|E_s\|\le u_m\). The convergent matrix logarithm and inverse series give

\[
 \left|\log\frac{\det C_I(s)}{\det C_{I,0}}\right|
       \le \frac{r_Iu_m}{1-u_m},
 \qquad
 \|C_I(s)^{-1}-C_{I,0}^{-1}\|
       \le\frac{\Lambda u_m}{1-u_m}.                 \tag{GM.17}
\]

Thus, pointwise on the real integration coordinates,

\[
 |d\mu_{I,s}(z)|
 \le \exp\{c u_m r_I\}
       \exp\{c\Lambda u_m|z|^2\}
       d\mu_{I,0}(z).                               \tag{GM.18}
\]

The determinant loss has a tunably small coefficient times the local rank. It is not a global-volume normalizer estimate.

## 4. Physical support and exact component factorization

Set the outside parameters to zero except on a cube set \(A\), and let

\[
 Y=D\cup\bigcup_{\Delta\in A}\Delta.
\]

Every surviving term in (GM.13) has its full carrier contained in \(Y\). Because that carrier is connected and contains its matrix endpoints, it lies in one connected component of \(Y\). The reference covariance is block diagonal across the components of \(D\). Hence \(C_I(s)\) is block diagonal across the components of \(Y\), and each block depends only on raw retained variables in that same component. A component of \(A\) not joined to \(D\) changes no matrix entry.

This is the same factorization as an independently calculated component, not only a block-diagonal matrix with global geometric coefficients. Let \(Y_a\) be a component, \(I_a=I\cap Y_a\), and \(D_a=D(I_a)\). Additivity of the enlargement implies \(D_a=D\cap Y_a\). The baseline \(C^D\) restricted to that component is the corresponding baseline from \(K^{D_a}\), by (GM.3). Every surviving tag carrier \(X\subset Y_a\) sees identical restrictions \(D\cap X=D_a\cap X\), so (GM.8) makes its difference coefficient identical as well. The outside parameter monomial is also identical. Therefore the full component family is exactly the family constructed from \(I_a\).

The determinant branch in (GM.16) consequently factorizes, because its factors agree at the positive reference and remain analytic. If a Mayer integrand is a product of functions belonging to the separate components, its localized Gaussian integral is the product of the corresponding component integrals. This proves the factorization required before the polymer logarithm.

## 5. Gaussian majorants and the localized integral identity

For a function \(G_I\) of the coordinates \(\mathscr I\) and retained data in \(I\), define

\[
 \mathcal F_I(s;v)=\int G_I(z;v)\,d\mu_{I,s}(z).
                                                               \tag{GM.19}
\]

At \(s=1\), this is exactly the original full Gaussian expectation \(\mu_C(G_I)\), by the Gaussian marginal identity. No global determinant is discarded or estimated separately.

Suppose the Mayer/source estimates give

\[
 |G_I(z;v)|\le a_I e^{a|z|^2}
       \prod_{i\in P}{\bf1}_{\{|z_i|>P(g)\}}.        \tag{GM.20}
\]

The indicator may be absent. Choose fixed positive \(a,y\) and the buffer so that \(a+y+c\Lambda u_m<\sigma/4\). Bounding the failed cutoffs by \(\exp[-yP(g)^2|P|]\exp[y\sum_{i\in P}|z_i|^2]\) and integrating (GM.18) yields

\[
 |\mathcal F_I(s;v)|
 \le a_I\exp\{c[u_m+(a+y)/\sigma]r_I\}
             \exp\{-yP(g)^2|P|\}.                  \tag{GM.21}
\]

This is the exact role of the Gaussian reserve in CMP116 (2.18)–(2.26), now proved for the ambient Gram family through one marginal covariance. A local polynomial root is treated by the same finite-rank Gaussian insertion bound, or by the adaptive small linear/quadratic source species of LC.35–LC.40. Its trace cost is local. A polynomial factor on a failed-cutoff coordinate is absorbed by reducing the fixed positive tail exponent.

Apply the product fundamental theorem of calculus to (GM.19), integrating each differentiated outside parameter from zero to one. Cauchy on the spare polydisc supplies a factor \((R-1)^{-|A|}\). Sections 3–4 imply that the resulting coefficient has actual raw support in \(Y\), vanishes for components disjoint from \(D\), and factorizes over the other components. These are the exact localization and factorization identities used in the subsequent Mayer/failed-cutoff resummation. The majorants in (GM.7) and (GM.21) are before signed coefficient sums; Cauchy and all matrix-word sums can be dominated absolutely.

The block side and target carrier rate must be paid explicitly. The initial enlargement obeys (GM.10); a physical weight on it costs at most \(\exp[c_d\kappa m^d|I|]\). A noncircular parameter order is: first fix the positive primitive carrier rates and the desired Gaussian reserve; choose \(R>1\) above the fixed outside-cube counting entropy with a strict margin; next choose \(m\) large enough for (GM.15) and that reserve; then choose \(\kappa>0\) so \(c_d\kappa m^d\) fits both the primitive input decay and the remaining \(\log(R-1)\) margin after entropy. Fix the remaining source/Mayer smallness constants and finally take the original coupling small enough to meet them. The cutoff \(P(g)\to\infty\) supplies the failed-cutoff smallness. All choices are independent of total volume and of the root energy, though they can be quantitatively very conservative.

## 6. What is proved, and the remaining uses

Under the explicit positive supported Gram input (GM.1), the construction supplies an exact, analytic, component-factorizing localization of every finite-support Gaussian marginal. It has a raw-local positive reference and a tunably small quadratic/determinant error. Therefore the simultaneous \(\Gamma\)/square-root compatibility problem is avoided; a single covariance generates both its precision and normalizer exactly.

For the positive extension in [local extension kernel](local_extension_kernel.md), its Gram coefficient budget is precisely (GM.1). Its clipped interaction coefficients retain their original fluctuation analyticity and small absolute source-free bounds. Its clipped reconstruction retains the scalar's supported linear/quadratic defect estimates. These ingredients can therefore be inserted into the same rooted Mayer argument as LC.5. Smooth retained cutoff derivatives still require their explicit product rules. The Gaussian derivative at fixed geometry is the ordinary derivative of (GM.16), including both the determinant and inverse-covariance terms; it is not obtained by pretending the cutoffs are holomorphic in retained variables.

No history change is contained in this statement. A different free-coordinate rank, a completed residual-component law, or an inherited interaction without a full physical-carrier budget requires its own input verification. The theorem supplies the missing Gaussian construction for the fixed-geometry ambient Gram family; it is not by itself the complete M-04 theorem.

## 7. Continuous retained derivatives of the same marginal family

Let \(D_d\) denote one of the normalized retained link directions of M-03. Its physical link displacement is of order \((1+\beta_1)^{-1/2}\). In addition to (GM.1), suppose the primitive extended coefficients satisfy the explicit input derivative budget

\[
 \|B\|_{\nu;1}:=
 \max_{\rm rows,columns}\sum_X e^{\nu|X|}
        \sum_{d\in\operatorname{dirs}(X)}
        \sup_v |D_d B_X|\le b_1,                    \tag{GM.22}
\]

where the row/column sums include the matrix endpoint as in (GM.1). This is a coefficient input, not a bound for a normalized marked output. Every direction not in the full raw carrier has derivative zero.

### Lemma GM.3 — derivative version of the common expansion

After reducing \(\nu_1\) if necessary, the common expansion of Lemma GM.1 has deterministic derivative majorants satisfying

\[
 \sup_i\sum_\gamma\sum_j e^{\nu_1|X_\gamma|}
    \sum_d\sup_{H,v}|D_d C^H_\gamma(i,j;v)|
       \le c_{C,1},                                \tag{GM.23}
\]

and the column analogue. The derivative coefficient has the same carrier and the same restriction consistency. The constants depend on \(b_0,b_1,\sigma,\nu\) and the fixed geometry.

**Proof.** The Gram product gives the corresponding derivative budget for its primitive precision coefficients. Restriction to \(H\) deletes coefficients, so it does not enlarge this budget. In the common local parametrix, differentiate a principal inverse by

\[
 D_d R_Q^H=-R_Q^H(D_d K_{n,Q}^H)R_Q^H.              \tag{GM.24}
\]

Both inverse factors have the uniform local entry majorant used in Lemma GM.1. The differentiated input is supported in the same complete cube halo. The finite local cube size and (GM.22) bound the sum over all its retained directions. Differentiate the parametrix error and the two Neumann series by the product rule. A word of length \(k\) gives \(k\) possible differentiated positions; the corresponding scalar sum is bounded by \(\sum_{k\ge1}k r^{k-1}\) for the existing strict contraction \(r<1\). The differentiated factor need only have a finite input budget; it need not be divided by the value of its undifferentiated factor. A fixed polynomial carrier/direction cost is absorbed by reducing the rate. The resulting majorants are uniform in \(H\), just as in (GM.7). The local restriction identity and support persist term by term. \(\square\)

The set \(D(I)\), the common tags and all decoupling monomials are fixed geometrical choices when \(D_d\) is taken. Consequently (GM.13) can be differentiated term by term. Lemma GM.3 gives a finite uniform row/column derivative bound on the same spare polydisc. The difference part also has an exponentially small buffer tail by the proof of Lemma GM.2, though smallness of the derivative is not needed for differentiating once.

The normalized density has the exact derivative

\[
 D_d\log\rho_{I,s}(z)=
 -\tfrac12\operatorname{Tr}\{C_I(s)^{-1}D_dC_I(s)\}
 +\tfrac12 z^{\mathsf T}C_I(s)^{-1}
              D_dC_I(s)C_I(s)^{-1}z.               \tag{GM.25}
\]

Both the determinant response and the inverse-covariance response are present. Its integral against \(\mu_{I,s}\) is zero, since that measure is normalized for every retained datum. On the spare polydisc the inverse norm is uniformly bounded, so

\[
 |D_d\log\rho_{I,s}(z)|
 \le c\|D_dC_I(s)\|\,(r_I+|z|^2).                  \tag{GM.26}
\]

For sums over directions, a deliberately conservative finite-rank bound suffices. Restrict the row/column derivative sums to \(\mathscr I\), and use (GM.23) to obtain

\[
 \sum_d\|D_d C_I(s)\|\le C r_I c_{C,1}.
\]

Thus the summed derivative of the Gaussian integral costs at most a fixed polynomial in \(r_I\), multiplying the same Gaussian majorant (GM.21). The extra \(|z|^2\) is integrated with a spare positive precision reserve. No total-volume rank or total-volume determinant is involved. After external component localization, a derivative vanishes outside its full physical carrier; the fixed polynomial direction count is paid by another strict part of the spatial rate.

### The explicit cutoff terms in the actual first-step extension

For the coefficients constructed in [local extension kernel](local_extension_kernel.md), every derivative is taken by

\[
 D_d(\eta_X a_X)=\eta_XD_da_X+(D_d\eta_X)a_X.         \tag{GM.27}
\]

The first term uses the native coefficient's inner physical analytic tube. The second uses the fixed geometric collar of its retained cutoff. Its full carrier includes that collar's curvature and local spectral tests. There are only a fixed number of local tests incident to a raw coordinate, or a fixed polynomial number on a declared carrier; their normalized derivatives are bounded by a constant times \((1+\beta_1)^{-1/2}\). Repeated occurrences of a local inverse in a Neumann word are handled by the differentiated geometric series in Lemma GM.3, not by an unbounded unweighted word count.

The initial native precision, resolvent and Gram coefficients have the derivative budget by their fixed local analytic domains. Multiplying by the smooth cutoffs and using (GM.27) gives (GM.22), after spending a fixed rate. The interaction coefficients satisfy the analogous input derivative budget in their scalar/linear/quadratic Gaussian class. At the first step their value budgets are bounded by \(c[gP(g)^3+g^2P(g)^2]\); normalized retained differentiation and the cutoff terms keep a finite, and in this construction vanishing, budget of the same sufficient order. The constraint-curvature and coarea terms remain included. No assertion that \(\eta_X\) is holomorphic in raw retained variables is used.

## 8. A fixed-geometry ambient one-root theorem

The following statement includes the complete real retained product domain for this geometry. It does not include replacement by another history geometry.

Use the source-independent extension

\[
 q_v^{\rm ext}(dz)=
 \frac{\mu_{C(v)}(dz)\,\chi_P(z)e^{W_{\rm ext}(z;v)}}
      {\mu_{C(v)}(\chi_Pe^{W_{\rm ext}})},
 \quad C=(\sigma I+B_{\rm ext}^{\mathsf T}B_{\rm ext})^{-1},
                                                               \tag{GM.28}
\]

with its literal fixed product cutoff \(\chi_P\), and the single compact-link reconstruction

\[
 \chi^{\rm ext}_e(z,v)=
       e^{i\Theta^{\rm ext}_e(z,v)}(Q^fv)_e.         \tag{GM.29}
\]

These are exactly the constructions in (4.1) and (4.12) of [local extension kernel](local_extension_kernel.md). The same kernel and reconstruction are used for every mark. They agree with the actual conditional operation on the first-clean active set. The complete interaction contains its Haar, coarea, soft-gauge and constraint terms once.

Any factor depending only on retained data is canceled algebraically between the numerator and denominator of this conditional kernel before (GM.28) is written. In particular the extensive classical background action is not placed in the small interaction budget. Such a factor remains in its original outer marginal weight on active data; this conditional cancellation does not delete it from the source-free RG law.

Take the incoming primitive scalar with fixed normalization and centering,

\[
 F_h=\alpha\beta_0\sigma_h-c,
 \qquad b=|\alpha|+h^4|c|,                          \tag{GM.30}
\]

with fixed stencil and trace factors absorbed in the constants. Assume the exposed ratio \(\beta_0/\beta_1\) lies in a fixed compact interval of positive numbers. Let

\[
 E_Y(v)=1+\sum_{p\subset\operatorname{foot}Y}
                         \beta_0s(v_p).
\]

The local-lift force comparison and extended Hermitian reconstruction give an actual pre-integration expansion

\[
 h^4F_h(\chi^{\rm ext}(z,v))=\sum_{Y\ni x}f_Y(z,v),
 \qquad a_Y\le cb e^{-\nu_f|Y|},                    \tag{GM.31}
\]

with exact ray coefficients satisfying

\[
 |f_Y(0,v)|\le a_YE_Y(v),\qquad
 \|\ell_Y\|_1\le a_Y\operatorname{poly}(|Y|)\sqrt{E_Y(v)},
 \quad\sup\|v_Y(gz)\|_1\le a_Y\operatorname{poly}(|Y|).
                                                               \tag{GM.32}
\]

The derivatives of these same coefficients have an explicitly summed supported bound of energy grade at most one. A sufficient form, with a smaller \(\nu_f\), is

\[
 \sum_d\left[|D_df_Y(0,v)|+
       \|D_d\ell_Y\|_1+
       \sup\|D_dv_Y(gz)\|_1\right]
 \le cb e^{-\nu_f|Y|}\operatorname{poly}(|Y|)E_Y(v).
                                                               \tag{GM.33}
\]

Here derivatives outside the full raw footprint vanish. To verify (GM.33) for (GM.29), apply (GM.27) to its supported logarithm coefficients and differentiate the local compact plaquette product. A normalized retained derivative gives a physical factor of order \(g\), while a fluctuation derivative gives a factor \(g\). Their product cancels the scalar's \(\beta_0\). The remaining first trace derivative is controlled by the local coarse plaquette defect and the force bound; its growth is at most \(1+\sqrt{E_Y}\). A cutoff derivative contributes its fixed collar factor times the already bounded coefficient. Summing its incident directions costs a fixed polynomial. The weaker energy-one bound (GM.33) follows. The microscopic formula is differentiated; no separately extended marked output is used.

### Theorem GM.4 — ambient continuous records at the first clean step

Fix the geometric constants, a sufficiently large marginal buffer, and a sufficiently small positive output carrier rate as described after (GM.21). For all sufficiently small admitted first-step couplings, the exact transported scalar through (GM.28)–(GM.29) has a connected physical-carrier representation, retaining its individual tags, with compatible value, direct and normalized-kernel records. These obey

\[
 (Lh)^4\sum_a e^{\kappa(|Z_a|+t(Z_a))}
 \left[
  \sup_v\frac{|A_a(v)|}{\widehat R_{Z_a}(v)}
  +\sup_v\frac{\sum_d\sup_{0<|t|\le1}
          (|B_{a,d,t}(v)|+|J_{a,d,t}(v)|)}
                 {\widehat R_{Z_a}(v)^{3/2}}
 \right]
 \le cL^4b.                                        \tag{GM.34}
\]

The suprema are over the entire real compact retained product domain of this fixed geometry, including selector-inactive data. The regulator is the actual output-scale Wilson-energy regulator, with its M-03 shifted version. The coupling-ratio hypothesis compares it to \(E_Y\). The sum is before cancellation or aggregation of different activity tags.

#### Proof: exact value and absolute root sum

Use the exact identity (GM.28). Expand the localized interactions and the fixed cutoffs as in CMP116, keeping each union of interaction supports and failed-cutoff coordinates as the set \(I\). Integrate its local integrand against the exact Gaussian marginal of \(C\). Equations (GM.13)–(GM.21) supply the analytic localization, Gaussian reserve and component factorization. Thus the same finite Mayer summations and connected logarithm apply to this positive extended kernel, with the strict decay margins and smallness constants fixed in Section 5. This argument uses no native \(\Gamma\) identity for the clipped coefficients.

Insert one exact defect \(f_Y-f_Y(0)\) as a source species. Its ray coefficients (GM.32) admit the adaptive circle

\[
 \rho_Y\asymp
 \frac{e^{-\lambda|Y|}}
 {a_Y\operatorname{poly}(|Y|)(1+\sqrt{E_Y})}.
\]

The linear and quadratic species estimate of LC.40 pays a fixed part of the same positive reserve in (GM.21), without changing \(P(g)\). The source-containing logarithmic tags have uniform deterministic absolute majorants on that circle, by the same argument as LC.41a. Its nonzero analytic integral and logarithm are conclusions of the convergent expansion. Termwise source Cauchy costs only \(\rho_Y^{-1}\), and the scalar constant \(f_Y(0)\) is restored exactly. The input decay, initial buffer enlargement, outside-block entropy and polynomial coordinate counts are paid by the strict rate choices. This proves the value part of (GM.34) on the full real retained domain.

#### Proof: separate infinitesimal records

Introduce independent retained copies and keep their roles fixed:

\[
 H(v_{\rm ins},v_{\rm ker})
   =q^{\rm ext}_{v_{\rm ker}}
           [F_h(\chi^{\rm ext}(z,v_{\rm ins}))].     \tag{GM.35}
\]

The same source expansion is valid for these two copies. The root energy uses the insertion copy; all kernel coefficients use the kernel copy. On the real product domain, all their source-free budgets are uniform.

Differentiate the insertion copy termwise. This differentiates only the exact mark coefficients, producing (GM.33). Their derivatives are another permitted localized scalar species; alternatively differentiate the original root Mayer factor before its source derivative. The one-root majorant with (GM.33) bounds each direct record by energy grade one. This operation does not differentiate the normalized kernel.

Differentiate the kernel copy termwise. For a marginal tag, use precisely (GM.25), together with the derivatives of its complete interaction coefficients. These differentiate both its normalizer and its exponent. Equations (GM.23), (GM.26) and the interaction derivative budgets give local Gaussian polynomial insertions, with at most fixed polynomial carrier/rank losses. They are paid by the remaining reserve and spatial rate. A differentiated ordinary Mayer factor can also be treated as a distinguished derivative species with its own explicit input budget. It is not divided by the unmarked species' value or by its vanishing smallness parameter. Every term in the derivative of the source-containing logarithmic difference still contains the scalar source. Hence the same root factor persists in its absolute majorant.

After differentiating the source at zero, the two records are exactly

\[
 B_d=q^{\rm ext}_v\bigl(D_d[F_h(\chi^{\rm ext})]\bigr),\qquad
 J_d=\operatorname{Cov}_{q^{\rm ext}_v}
     (F_h\circ\chi^{\rm ext},D_d\log w_v),          \tag{GM.36}
\]

where \(w_v\) is the full unnormalized fixed-support density. Formula (GM.25) is its marginal Gaussian contribution. No estimate of the derivative of \(B_d+J_d\) replaces these separate bounds. Each localized derivative is zero outside its complete raw carrier. Summed direction and local-rank losses are polynomial and are absorbed by the spare rate. The bounds grow at most like one local energy, which is stronger than the required current grade \(3/2\).

#### Proof: exact finite differences on all ambient paths

For \(v_t=\tau_{d,t}v\), use the two-copy endpoint identities

\[
 B_{d,t}=\frac{H(v_t,v_t)-H(v,v_t)}t,
 \qquad
 J_{d,t}=\frac{H(v,v_t)-H(v,v)}t.                    \tag{GM.37}
\]

These are exactly the M.30 records for a microscopic input with zero previous current. Integrate the insertion derivative on its first rectangular path at fixed endpoint kernel, and the kernel derivative on its second path at fixed original insertion. Since the extended kernel and reconstruction are smooth on the full real retained product domain, these paths are allowed even when they cross the old selector boundary. The extra \(D\eta\) contributions were already included in (GM.27).

Apply this two-copy construction to each individual localized tag \(H_a\), with \(A_a(v)=H_a(v,v)\). Thus (GM.37) gives \(\delta A_a=B_a+J_a\) tag by tag, before any aggregation or cancellation, as required for the decorated carrier norm.

The compact link inequality

\[
 \beta_1s(e^{tT/\sqrt{1+\beta_1}}P)
 \le2\beta_1s(P)+ct^2,
 \qquad |t|\le1,
\]

compares every path energy to the shifted output regulator. It holds for arbitrary compact links, not merely inside a small chart. The resulting finite-difference records have the same supported majorants. Their sum is exactly the finite difference of the value coefficient by (GM.37). This completes (GM.34). \(\square\)

If an outer law has \(\|\sum_{p\subset Z}\beta_1s(v_p)\|_{L^p}\le c|Z|p\), the same positive majorants give the averaged M-03 value and continuous-current grades, after another fixed spatial-rate expenditure for \(|Z|\). At the actual first Wilson step the unnormalized clean restriction of the blocked law has this reserve; no division by its clean-event probability is involved.

The theorem chooses a recorded source-independent extension on the whole retained product for this geometry. It therefore repairs the continuous selector-interface obstruction for that extension. It does not change the original probability law on active data, and does not identify the extension with the old point-mass convention. It does not estimate a transition to a different active history or an inherited residual quotient.

## 9. Scalar and identity extraction on the proved domain

The fixed F-01 scalar is exactly \(\sigma_{h'}=2w_{h'}/\sqrt6\), with \(h'=Lh\). Put \(\varphi_{h'}=\beta_1\sigma_{h'}\). For each tag from Theorem GM.4 use the all-identity retained datum and the normalized single-link pulse of [scalar extraction](scalar_extraction.md), (SE.2)–(SE.4). Average the pulse evaluation over the finite signed coordinate-permutation group at the anchor. The denominator remains the fixed positive quantity \(d(\beta_1,t)\) of (SE.3), uniformly bounded below for \(\beta_1\ge1\).

Define

\[
 c_a=A_a(v_0),\qquad
 a_a=\frac{h'^4[\operatorname{Av}_{\rm pulse}A_a-A_a(v_0)]}
               {d(\beta_1,t)},\qquad
 \mathcal R_a=A_a-c_a-a_a\varphi_{h'}.               \tag{GM.38}
\]

Subtract \(a_a\delta\varphi_{h'}\) from the direct record and keep the kernel record unchanged. The scalar and identity coefficients are field-independent numbers, and the remainder records stay compatible tag by tag. Each carrier is enlarged by the fixed scalar stencil.

The two probe regulators are uniformly bounded: the identity and a normalized one-link pulse, even after one further elementary shift, excite only a fixed number of the independent coarse plaquette energies. Therefore (SE.9) holds with \(r=0\). The primitive scalar has its pointwise and continuous-difference budget by M.1, and its averaged budget under the same optional energy-moment reserve used after GM.34. The extraction theorem (SE.11) consequently gives the exact decomposition

\[
 Q^{\rm ext}F_h=a\varphi_{h'}+c_{\rm out}+\mathcal R,
 \qquad
 |a|+h'^4|c_{\rm out}|+
       \|\mathcal R\|_{\rm ambient,continuous,\kappa}
       \le C L^4 b.                                \tag{GM.39}
\]

The norm denotes precisely the fixed-geometry ambient value and continuous direct/current norm proved above, with the averaged terms included when their stated reserve holds. The decomposition acts on the actual transported scalar, not a newly inserted coarse scalar.

If the fixed incoming scalar normalization is \(z_S^{\rm in}\ne0\), express its scalar term in that unchanged basis by

\[
 a\varphi_{h'}=
   \left(a\frac{\beta_1}{z_S^{\rm in}}\right)
          z_S^{\rm in}\sigma_{h'}.                  \tag{GM.40}
\]

The given input normalization is thereby exposed; no final running normalization is assumed. A zero incoming scalar coefficient has only the constant input case here and requires no division. The specified M-04 statement fixes its incoming basis but does not require a unique projection for an arbitrary transported output. Thus (GM.38) supplies the requested scalar/identity extraction on the domain where the operator theorem has been proved. A later comparison with a coefficient prescription in a Gamma or physical-renormalization calculation is a distinct downstream statement.
