# Pressure and scalar contact terms

## 1. Outcome and the exact normalization problem

**Full R2 remains open.** This note adds an actual-model result and a more concrete finite-jet completion criterion. It does not replace a physical source by a conditional innovation, and it does not divide out any compulsory history mass.

The actual-model result is a uniform lower bound on the variance of a literal scalar source with a plateau. For every SU(N), all sufficiently large bare Wilson coefficients, and every finite periodic lattice, that variance is at least a constant times the number of fine links in the plateau divided by the square of the coefficient. Consequently a quadratic source counterterm is unavoidable in any cutoff-uniform two-jet or complex-pressure theorem. This conclusion is stronger than the previously established divergence of the first derivative.

The positive reduction proved here uses the *actual normalized connected covariance*, not an auxiliary Gaussian or a source-free activity bound. A short-distance dyadic annular bound of dimension eight, a separate macroscopic smeared bound that permits phase correlations, and matching of the prescribed local contact coefficients give a complete cutoff-uniform scalar two-jet estimate by an explicit Taylor subtraction through degree four. It does not require a fixed complex-source logarithm on each history or clustering before phase selection. These actual-model inputs are stated as open, rather than inferred from the new variance estimate. An optional stronger all-distance decay version is also proved as an implication.

Let the torus have n sites in each of four directions, n≥2, and put V=n⁴. With normalized Haar measure and G=SU(N), use the literal preamble action:

\[
 s_p=N-\operatorname{Re}\operatorname{Tr}U_p,\qquad
 S=\sum_p s_p,\qquad
 Z_n(\beta)=\int e^{-\beta S}\,dU,\qquad
 \mu_{n,\beta}(dU)=Z_n(\beta)^{-1}e^{-\beta S(U)}\,dU.
 \tag{CP.1; P: definitions}
\]

Write S_b for the sum of the six plaquette actions incident on a positive link b. There are 4V such links and 6V plaquettes, and each plaquette belongs to four stars. For a real scalar profile f, with the literal plaquette-source anchors fixed, set

\[
 F_f=\sum_p f(x_p)s_p,\qquad
 B_f(a)=\{b:\ f(x_p)=1\text{ for every }p\ni b\}.
 \tag{CP.2; P: definitions}
\]

The set B_f(a) is only used for the lower bound. A fixed C⁵ profile equal to one on an open physical cube and supported with margin in a cell has at least c_f a⁻⁴ links in B_f(a) for all sufficiently small a.

For any deterministic source subtraction C_a[j], the finite-cutoff normalized source function is

\[
 H_a(j)=e^{-C_a[j]}\,\mu_{n,\beta_a}(e^{F_j}),\qquad C_a[0]=0.
 \tag{CP.3; P: definition}
\]

Its logarithmic derivatives at zero are the actual connected moments minus the corresponding source derivatives of C_a. In particular, the second derivative contains a covariance of the original physical plaquette source. Performing positive marginalizations, adjoining normalized references, and retaining or integrating old fields does not change this identity.

The notation C_a does not authorize setting the counterterm equal to the full logarithm of the partition function. In the physical application it must be the deterministic local recipe of the construction. Section 4 displays an explicit local Taylor recipe at the level of the two-point kernel and then separates the still-unproved comparison with that prescribed recipe. Its coefficients can depend on the finite torus until this comparison has been established; no torus-independent conclusion is hidden in the notation.

Labels have the following meaning: P is proved here; L is an assertion checked on the cited primary page, within its stated hypotheses; C is a consequence with an explicitly unverified physical hypothesis; O is an unproved physical input. N2-F is the sole assumed interface. It is needed below only for its elementary upper bound β_a≤C(K+1), where a=L⁻ᴷℓ₀. The finite-lattice variance theorem does not use it.

## 2. An actual Wilson lower bound for the second scalar cumulant

### 2.1 A uniform elementary cold-region estimate

Put d_A=N²−1. Fix a sufficiently small identity chart in SU(N). Its Haar density is bounded above and below by positive constants in Lie-algebra coordinates. Requiring every one of the 4V links to lie in a ball of radius rβ⁻¹ᐟ², for β≥1 and a fixed small r, has Haar probability at least c_N^{4V}β^{-2d_AV}. On that event, the telescoping product inequality and unitarity give a plaquette Hilbert–Schmidt distance at most 4rβ⁻¹ᐟ² from the identity. Since s(U)=‖U−I‖²_HS/2, the action satisfies βS≤C_NV there. Hence

\[
 Z_n(\beta)\ge e^{-C_NV}\beta^{-2d_AV},
 \qquad \beta\ge1.
 \tag{CP.4; P}
\]

No gauge fixing or independent-plaquette assertion is used. The less sharp count 4V of original link variables is sufficient for the present purpose.

At finite volume, differentiating under the compact Haar integral gives −∂_β log Z_n=μ_{n,β}(S) and ∂_βμ_{n,β}(S)=−Var_{μ_{n,β}}S≤0. It follows that

\[
 \frac{\beta}{2}\mu_{n,\beta}(S)
 \le\log Z_n(\beta/2)-\log Z_n(\beta)
 \le-\log Z_n(\beta)
 \le C_NV+2d_AV\log\beta.
 \tag{CP.5; P}
\]

The middle inequality uses Z_n(β/2)≤1. Translation and coordinate-permutation invariance, together with Σ_bS_b=4S, therefore imply

\[
 \mu_{n,\beta}(S_b)=V^{-1}\mu_{n,\beta}(S)
 \le C_N\frac{\log(2+\beta)}{\beta}
 \quad\text{for every }b,\ n\ge2,\ \beta\ge1.
 \tag{CP.6; P}
\]

This estimate is weaker than the exponential-energy theorem already in the companion notes. Its advantage here is that its entire proof is the preceding elementary calculation, with no trajectory or reflection hypothesis.

### 2.2 Thermal variance of a near-flat conditional star

Fix the exterior of one link. Using cyclicity of the trace and Re Tr U⁻¹=Re Tr U, rewrite its six plaquette actions as s(UV_i), with fixed V_i∈SU(N). Define the conditional star potential and its minimum by

\[
 A_v(U)=\sum_{i=1}^{6}s(UV_i),\qquad
 W(v)=\min_{U\in SU(N)}A_v(U),\qquad
 \pi_{\beta,v}(dU)=
 \frac{e^{-\beta A_v(U)}\,dU}{\int e^{-\beta A_v}\,dU}.
 \tag{CP.7; P: definitions}
\]

**Lemma 2.1 (P).** There are δ_N>0, β_N<∞ and c_N>0 such that

\[
 W(v)\le\delta_N,\quad\beta\ge\beta_N
 \quad\Longrightarrow\quad
 \operatorname{Var}_{\pi_{\beta,v}} A_v\ge c_N\beta^{-2}.
 \tag{CP.8; P}
\]

**Proof.** Choose a minimizing U_* and put B_i=U_*V_i. Then Σ_i s(B_i)=W(v). Consequently ‖B_i−I‖_HS≤(2δ_N)¹ᐟ² for every i. With U=QU_*, Haar invariance gives

\[
 D_B(Q):=A_v(QU_*)-W(v)
  =\operatorname{Re}\operatorname{Tr}
       \left[(I-Q)\sum_iB_i\right]
  =6s(Q)+E_B(Q).
 \tag{CP.9; P}
\]

The C² norm of E_B, with respect to any fixed bi-invariant group metric, is at most C_Nδ_N¹ᐟ². Also E_B(I)=0 and DE_B(I)=0: the first identity is immediate, and the second follows because both D_B and s have a minimum at I. Taylor's formula along a minimizing geodesic gives |E_B(Q)|≤C_Nδ_N¹ᐟ² dist(I,Q)².

The two nonnegative functions dist(I,Q)² and s(Q) are comparable globally on SU(N). Near I this follows from the nonsingular exponential chart and the quadratic Taylor coefficient of s. Away from that chart it follows from compactness and the fact that s has its only zero at I. Decreasing δ_N therefore gives the uniform global comparison

\[
 3s(Q)\le D_B(Q)\le9s(Q),
 \qquad c_N\,\operatorname{dist}(I,Q)^2
       \le D_B(Q)\le C_N\,\operatorname{dist}(I,Q)^2 .
 \tag{CP.10; P}
\]

In particular I is the unique minimum in these centered coordinates. This conclusion was derived from small W; it was not assumed for arbitrary exteriors.

Let c and C be fixed lower and upper constants in the second comparison. Choose R>1 so that cR²>C+1. In a fixed identity chart consider the two sets dist(I,Q)≤β⁻¹ᐟ² and Rβ⁻¹ᐟ²≤dist(I,Q)≤(R+1)β⁻¹ᐟ². For all sufficiently large β they lie in that chart. The Haar volumes of both sets are at least a positive constant times β^{-d_A/2}. The density numerator on either set is at least exp[−C(R+1)²], while (CP.10), a Gaussian chart integral and a compact exterior bound give

\[
 \int e^{-\beta D_B(Q)}\,dQ\le C_N\beta^{-d_A/2}.
 \tag{CP.11; P}
\]

Thus each of the two sets has π_{β,v}-probability bounded below by a positive constant independent of β and v. The D_B values on the second set exceed those on the first by at least (cR²−C)/β. For independent samples Q,Q′, use Var D_B=½ E[(D_B(Q)−D_B(Q′))²] and the two opposite ordered events to obtain (CP.8). Adding W does not change a variance. This proves the lemma without differentiating a Laplace asymptotic. ∎

For the actual Wilson exterior law, W_b≤S_b pointwise. Markov's inequality and (CP.6), with β_N enlarged once, give

\[
 \mu_{n,\beta}(W_b\le\delta_N)\ge\tfrac12
 \qquad(\beta\ge\beta_N,\ n\ge2).
 \tag{CP.12; P}
\]

Thus the conditional-variance estimate is used on a set whose probability under the *actual normalized exterior law* is uniformly positive. It is not an estimate under a separately chosen reference.

### 2.3 Disjoint stars produce an extensive variance

**Theorem 2.2 (P).** For every SU(N), constants c_N>0 and β_N<∞ exist such that every finite four-dimensional periodic lattice with n≥2, every β≥β_N, and every real scalar profile f satisfy

\[
 \operatorname{Var}_{\mu_{n,\beta}}F_f
 \ge c_N\,\frac{|B_f(a)|}{\beta^2}.
 \tag{CP.13; P}
\]

**Proof.** Form the graph whose vertices are the links in B_f(a), with two links adjacent if they share a plaquette. A link belongs to six plaquettes, each with three other links, so its degree is at most 18. Greedy selection gives a subset I⊂B_f(a) with |I|≥|B_f(a)|/19 and no common plaquette between two of its links.

Condition on every link outside I. The original Wilson density factorizes exactly into a product of the one-link conditional laws (CP.7): every plaquette contains at most one link of I. The source also has the exact form F_f=F_ext+Σ_{b∈I}S_b, because all six source coefficients at a link in B_f(a) equal one and these six-plaquette sets are disjoint. Conditional independence therefore gives

\[
 \begin{aligned}
 \operatorname{Var}_{\mu_{n,\beta}}F_f
 &\ge
 \mu_{n,\beta}\!\left(
       \operatorname{Var}(F_f\mid U_{I^c})\right)\\
 &=\sum_{b\in I}\mu_{n,\beta}
          \left(\operatorname{Var}_{\pi_{\beta,v_b}}S_b\right)
 \ge \frac{c_N|I|}{2\beta^2}.
 \end{aligned}
 \tag{CP.14; P}
\]

The first inequality is the law of total variance; the last uses (CP.8) and (CP.12). Absorb 38 into c_N. No signs of covariances between distinct stars have been assumed. ∎

For a fixed cell-supported C⁵ plateau profile, |B_f(a)|≥c_fa⁻⁴ for small a. N2-F implies β_a→∞ and β_a≤C(K+1). Thus the theorem applies for all sufficiently large K, and

\[
 \operatorname{Var}_{\mu_{n,\beta_a}}F_f
 \ge c_f\frac{a^{-4}}{(K+1)^2}
 \longrightarrow\infty,\qquad a=L^{-K}\ell_0.
 \tag{CP.15; P from Theorem 2.2 and N2-F}
\]

A fixed rescaling of f to fit the prescribed source norm multiplies this lower bound by the square of that rescaling. The divergence persists. This is a lower bound for the bare scalar representative; applying a running multiplicative field normalization multiplies both sides by its square.

## 3. Necessary contact cancellation and the genuine separated-correlation requirement

### 3.1 A quadratic counterterm is compulsory

**Proposition 3.1 (P).** Suppose C_a(zf) is holomorphic for |z|<r, real for real z, and C_a(0)=0. If the actual normalized function (CP.3) satisfies |H_a(zf)|≤M on that disk, with r>0 and M independent of a, then

\[
 \left|
   \operatorname{Var}_{\mu_{n,\beta_a}}F_f
           -D^2C_a(0)[f,f]\right|
 \le\frac{2M+M^2}{r^2}.
 \tag{CP.16; P: necessary consequence of the displayed bound}
\]

**Proof.** H_a(0)=1. Cauchy's inequalities give |H_a′(0)|≤M/r and |H_a″(0)|≤2M/r², taking limits of smaller circles if necessary. A logarithm exists in some neighborhood of zero because H_a(0)=1; no uniform zero-free disk is needed for this calculation. Its second derivative is H_a″(0)−H_a′(0)². Differentiating the finite compact-group integral identifies this with Var F_f−D²C_a(0)[f,f]. The stated bound follows. ∎

Combining with Theorem 2.2 gives the actual necessary size

\[
 D^2C_a(0)[f,f]\ge
 c_N\frac{|B_f(a)|}{\beta_a^2}
             -\frac{2M+M^2}{r^2}.
 \tag{CP.17; P}
\]

The same conclusion follows directly if a cutoff-uniform renormalized two-jet, rather than a complex finite-source theorem, is assumed. A subtraction that removes only the mean cannot meet either requirement. The divergent second derivative is a deterministic source contact; it cannot be discarded as a small field-valued remainder.

This result does not prohibit renormalized Schwinger distributions. Their prescribed contact subtractions are precisely what can cancel this divergence. Nor does it assert that every extension across coincident points is positive as an ordinary Euclidean random-variable covariance. The reflection-positive reconstruction problem has its own support and contact requirements.

### 3.2 Separated supports expose an actual normalized correlation

For two source directions f,g, write F=F_f and G=F_g. At every finite cutoff one has the exact identity

\[
 D^2\log H_a(0)[f,g]
   =\operatorname{Cov}_{\mu_{n,\beta_a}}(F,G)
                         -D^2C_a(0)[f,g].
 \tag{CP.18; P}
\]

Suppose the counterterm has no mixed contribution for these supports. This is automatic for a strictly contact-local jet when the supports are disjoint with positive separation. For a merely cell-local functional it instead requires that no cell collar used by that functional meets both supports. Under precisely this condition the last term of (CP.18) is zero.

If |H_a(zf+wg)|≤M on |z|<r_f, |w|<r_g, then multivariable Cauchy inequalities applied to H_a itself give

\[
 \left|
 \operatorname{Cov}_{\mu_{n,\beta_a}}(F,G)
                  -D^2C_a(0)[f,g]\right|
 \le \frac{M+M^2}{r_fr_g}.
 \tag{CP.19; P: necessary consequence of the displayed bound}
\]

Indeed H_{zw}(0) is bounded by M/(r_fr_g), while H_z(0)H_w(0) is bounded by M²/(r_fr_g). Thus a physical R2 pressure theorem contains a genuine bound on the actual normalized separated covariance. It is not only a bound on local energy sizes or a cancellation of Gaussian dimensions.

### 3.3 Weighted energy control does not supply that covariance bound

Here is a precise logical counterexample to an inference from the existing weighted energy theorem alone. It is not a Wilson model. Let two disjoint blocks each have m labels, let η be one Bernoulli variable with probability one half, and set X_i=η/β at every label. For arbitrary weights 0≤w_i≤1,

\[
 \log\mathbb E\exp\!\left(\kappa\beta\sum_iw_iX_i\right)
 \le\kappa\sum_iw_i.
 \tag{CP.20; P}
\]

The variables are nonnegative and individually bounded. Nevertheless, if F_A and F_B are their sums over the two blocks, then

\[
 \operatorname{Cov}(F_A,F_B)
       =\frac{m^2}{4\beta^2}.
 \tag{CP.21; P}
\]

The first assertion follows from ½(1+e^t)≤e^t for t≥0; the second from Var η=¼. Choosing m of order a⁻⁴ and β of order log(a⁻¹) makes (CP.21) diverge. No counterterm whose mixed derivative vanishes between the two blocks can change it.

The example does not contradict the locality of the Wilson action. Rather, it demonstrates the additional information a proof must extract *from* that locality and the actual multiscale dynamics. Weighted energy moments, positivity, and exact retention of masses do not already contain it. An actual normalized connected-kernel estimate is a concrete way to supply the missing information, as the next section shows.

## 4. A positive finite-jet completion criterion using the actual covariance

This section gives a concrete alternative to a uniform complex finite-source theorem for the *scalar first and second jets*. The companion notes already prove Taylor contact estimates for admitted regular carrier kernels. The distinction here is that the kernel below is the connected covariance under the complete normalized Wilson measure, with all sectors already summed. No transfer from a regular carrier bound to this kernel is assumed.

### 4.1 A deterministic local subtraction identity

Use the preamble's anchored scalar representative O_a(x)=a⁻⁴Σ_{μ<ν}s_{p_{μν}(x)}, so F_f=a⁴Σ_xf(x)O_a(x). Define its actual normalized mean and connected kernel by

\[
 m_{a,T}(x)=\mu_{n,\beta_a}(O_a(x)),\qquad
 \kappa_{a,T}(x,y)=
       \operatorname{Cov}_{\mu_{n,\beta_a}}(O_a(x),O_a(y)).
 \tag{CP.22; P: definitions}
\]

At finite a,T these are finite real quantities. The kernel is symmetric and translation covariant. This last statement does not identify the lower-vertex scalar anchor with a point-scalar under every lattice reflection; that separate placement issue remains as recorded in the main manuscript.

Take ρ=ℓ₀/8 and a fixed smooth even cutoff 0≤χ(r)≤1, equal to one for |r|≤ρ/2 and zero for |r|≥ρ. The compatible tori obey T≥2ℓ₀, so every displacement in the support of χ has a unique lift r=y−x in the short coordinate cube. Use the supplied underlying C⁵ test functions, with the fixed scaled norm Σ_{|α|≤5}ℓ₀^{|α|}sup|∂^αf|. If a source is supplied only as an array, an extension convention must additionally be fixed before using source jets.

For a test function g, put P_x^4g(r)=Σ_{|α|≤4}r^α∂^αg(x)/α!. Define

\[
 \begin{aligned}
 q_{a,T}(f,g)
   &=
    \frac{a^8}{2}\sum_{x,y}\kappa_{a,T}(x,y)\chi(y-x)
       \left[f(x)P_x^4g(y-x)+g(x)P_x^4f(y-x)\right]\\
   &=\frac{a^4}{2}\sum_x\sum_{|\alpha|\le4}
       c_{a,T,\alpha}(x)
       \left[f(x)\partial^\alpha g(x)
                       +g(x)\partial^\alpha f(x)\right],\\
 c_{a,T,\alpha}(x)
   &=a^4\sum_y\kappa_{a,T}(x,y)\chi(y-x)
                            \frac{(y-x)^\alpha}{\alpha!}.
 \end{aligned}
 \tag{CP.23; P: explicit finite-cutoff contact recipe}
\]

It is a symmetric, strictly contact-local bilinear functional of the source jets through degree four. Its coefficients may depend on a and T. Translation invariance makes them independent of x in the present homogeneous Wilson law. Symmetry and translation invariance also make κ(x,x+r)=κ(x,x−r); hence coefficients with odd total |α| vanish for the even χ. No further rotation or reflection assertion is needed in the proof.

Direct symmetrization of the finite double sum gives the exact identity

\[
 \begin{aligned}
 &\operatorname{Cov}(F_f,F_g)-q_{a,T}(f,g)\\
 &\quad=\frac{a^8}{2}\sum_{x,y}\kappa_{a,T}(x,y)
 \left\{
 f(x)\left[g(y)-\chi(y-x)P_x^4g(y-x)\right]
 +g(x)\left[f(y)-\chi(y-x)P_x^4f(y-x)\right]
 \right\}.
 \end{aligned}
 \tag{CP.24; P}
\]

At x=y the expression in braces vanishes exactly. Thus the diagonal kernel, however large, has been explicitly subtracted; it has not been estimated by an off-diagonal bound.

### 4.2 An optional stronger all-distance normalized-kernel hypothesis

Let d_T be the shortest Euclidean torus distance. First formulate a stronger sufficient version with long-distance two-point decay. This is not required by YM-E before phase selection. Section 4.4 gives a variant that only asks for ultraviolet annuli and keeps an independent macroscopic covariance term. For dyadic lengths h=2^ja, j≥0, up to the torus diameter, consider the estimate

\[
 \sup_x a^4
   \sum_{\substack{y:\ h\le d_T(x,y)<2h}}
                |\kappa_{a,T}(x,y)|
 \le C_\kappa h^{-4}
       \left(1+\left|\log(h/\ell_0)\right|\right)^q,
 \qquad 0\le q<\infty\text{ fixed}.
 \tag{CP.25; O: optional all-distance annular covariance bound}
\]

The constants and the exponent q must be independent of a and T. A pointwise bound of order d_T(x,y)⁻⁸ with the same fixed logarithmic factor is a stronger sufficient condition. The annular formulation is the one used here. It allows fixed logarithmic corrections and does not require a mass gap, but it does impose a long-distance decay property not included in the program's existence target.

This is a statement about the normalized complete connected kernel (CP.22). It is not supplied by the existing energy estimate, by a fixed-background propagator bound, or by the source-free R-activity estimate. It is a usable sufficient input, not asserted to be logically necessary for every possible distributional two-point construction.

**Proposition 4.1 (C: finite-jet consequence of (CP.25)).** If the actual bound (CP.25) holds and the lattice supports of f and g lie in a union D of physical cells, then

\[
 \left|\operatorname{Cov}(F_f,F_g)-q_{a,T}(f,g)\right|
 \le C_q C_\kappa |D|\,
                \|f\|_{C^5,\ell_0}\|g\|_{C^5,\ell_0}.
 \tag{CP.26; C}
\]

**Proof under the displayed hypothesis.** Taylor's theorem on a short lifted segment gives, for |r|≤ρ/2,
|g(x+r)−P_x^4g(r)|≤C‖g‖_{C⁵,ℓ₀}(|r|/ℓ₀)⁵.
In the cutoff transition and outside its support, boundedness of g and of the finitely many Taylor terms gives the uniform bound C‖g‖_{C⁵,ℓ₀}. Therefore on an annulus h≤d_T(x,y)<2h the bracket involving g in (CP.24) is bounded by
C‖g‖_{C⁵,ℓ₀}min{(h/ℓ₀)⁵,1}; the fixed cutoff ratio only changes C. The same statement holds for f.

Multiplying this remainder by (CP.25), and summing over dyadic h, costs at most C_qC_κℓ₀⁻⁴. Indeed the fine shells contribute a geometric series with terms proportional to (h/ℓ₀)(1+|log(h/ℓ₀)|)^q, and the coarse shells contribute terms proportional to (ℓ₀/h)^4(1+|log(h/ℓ₀)|)^q. Both sums converge uniformly in their endpoints. Finally a⁴ times the number of root sites where f or g is nonzero is at most |D|ℓ₀⁴. Insert these facts in (CP.24). ∎

For separated supports at distance δ>0, the same annular summation, with no Taylor operation, gives

\[
 |\operatorname{Cov}(F_f,F_g)|
 \le C_q C_\kappa
       \min\{\operatorname{vol}_a(\operatorname{supp}f),
                      \operatorname{vol}_a(\operatorname{supp}g)\}
       \delta^{-4}
       \left(1+\left|\log(\delta/\ell_0)\right|\right)^q
       \|f\|_\infty\|g\|_\infty .
 \tag{CP.27; C}
\]

Here vol_a(A)=a⁴ times the number of sites in A. If δ<a, the right side can only become weaker than using the first nonempty lattice shell. This is the concrete normalized correlation information that is absent from (CP.20).

### 4.3 Matching the prescribed counterterm, rather than redefining it

Let c_{a,1} and c_{a,2} be the first two derivatives of the *prescribed* deterministic source counterterm C_a. The additional compatibility estimates required for this route are

\[
 \begin{aligned}
 \left|a^4\sum_xm_{a,T}(x)f(x)-c_{a,1}[f]\right|
   &\le A_1|D|\|f\|_{C^5,\ell_0},\\
 \left|q_{a,T}(f,g)-c_{a,2}[f,g]\right|
   &\le A_2|D|\|f\|_{C^5,\ell_0}\|g\|_{C^5,\ell_0},
 \end{aligned}
 \tag{CP.28; O: first- and second-contact matching}
\]

uniformly in a,T and the source directions. These estimates include the needed finite-volume copying comparison for the coefficients of (CP.23) if C_a is to be torus independent. Defining c_{a,1},c_{a,2} to be the expressions on the left would prove finite-volume locality of that newly defined two-jet, but would not verify the prescribed Balaban recipe or torus independence. That substitution is not made here.

**Theorem 4.2 (C: scalar two-jet bound under the stronger sufficient inputs).** If (CP.25) and (CP.28) hold for the complete normalized Wilson kernel and the prescribed counterterm, then

\[
 \begin{aligned}
 |D\log H_a(0)[f]|
   &\le A_1|D|\|f\|_{C^5,\ell_0},\\
 |D^2\log H_a(0)[f,g]|
   &\le (C_qC_\kappa+A_2)|D|\,
                     \|f\|_{C^5,\ell_0}\|g\|_{C^5,\ell_0}.
 \end{aligned}
 \tag{CP.29; C}
\]

**Proof under these inputs.** The first derivative of the finite-cutoff logarithm is its actual mean minus c_{a,1}. Apply the first line of (CP.28). For the second derivative, use (CP.18), add and subtract q_{a,T}, and apply (CP.26) and the second line of (CP.28). These identities use the original normalized measure, so no separate inverse survivor mass is needed. ∎

This theorem identifies a finite-jet route that can be pursued directly if a complex finite-source induction is unnecessarily strong. It completes the downstream normalization and contact-extension argument *once the two displayed actual-model inputs are proved*. It does not prove them, does not supply tensor mixing or higher collision forests, and does not imply a complex-pressure bound. The all-order hierarchy and its fixed growth exponent remain separate obligations.

### 4.4 A variant that permits non-clustering phase mixtures

The large-distance part of (CP.25) can be replaced by a bound on macroscopic *smeared* covariances. Define the far bilinear form by retaining the actual covariance kernel outside the short contact cutoff. The exact decomposition is

\[
 \begin{aligned}
 B^{\mathrm{far}}_{a,T}(f,g)
   &=a^8\sum_{x,y}(1-\chi(y-x))
                     \kappa_{a,T}(x,y)f(x)g(y),\\
 \operatorname{Cov}(F_f,F_g)-q_{a,T}(f,g)
   &=B^{\mathrm{far}}_{a,T}(f,g)\\
   &\quad+\frac{a^8}{2}\sum_{x,y}\chi(y-x)\kappa_{a,T}(x,y)
      \left[
       f(x)\bigl(g(y)-P_x^4g(y-x)\bigr)
       +g(x)\bigl(f(y)-P_x^4f(y-x)\bigr)
      \right].
 \end{aligned}
 \tag{CP.29a; P}
\]

Now suppose the annular estimate (CP.25) is known only for a≤h≤ℓ₀, and separately suppose that for supports in D_f,D_g physical cells,

\[
 |B^{\mathrm{far}}_{a,T}(f,g)|
 \le C_M |D_f||D_g|\,
                  \|f\|_{C^5,\ell_0}\|g\|_{C^5,\ell_0},
 \quad C_M\text{ independent of }a,T.
 \tag{CP.29b; O: macroscopic smeared covariance bound}
\]

This bound permits a nonzero constant covariance component: a kernel equal to a fixed constant times ℓ₀⁻⁸ contributes at most a constant times |D_f||D_g|‖f‖_∞‖g‖_∞. It therefore does not require clustering before pure-phase decomposition. Other fixed test-function seminorms can be used in place of the displayed support-volume bound if their contact estimate is stated.

**Theorem 4.3 (C: finite-jet completion without a clustering premise).** Under the ultraviolet part of (CP.25), (CP.29b), and the prescribed-contact matching (CP.28), the first estimate in (CP.29) still holds and the second is replaced by

\[
 |D^2\log H_a(0)[f,g]|
 \le
 \left[(C_qC_\kappa+A_2)|D_f\cup D_g|
                       +C_M|D_f||D_g|\right]
              \|f\|_{C^5,\ell_0}\|g\|_{C^5,\ell_0}.
 \tag{CP.29c; C}
\]

**Proof under the displayed inputs.** The near term in (CP.29a) uses only distances at most ρ=ℓ₀/8. Taylor's fifth-order remainder and the ultraviolet annuli give the same C_qC_κ|D_f∪D_g| bound as before. Bound the far term by (CP.29b) and add the second line of (CP.28). The first derivative is unchanged. ∎

The quadratic support-volume cost is intentional: it accommodates macroscopic phase correlations. For fixed supported tests this gives a uniform cutoff and torus bound on the first two renormalized derivatives. It is a sufficient finite-jet result for those orders, not the original finite-source R2 statement and not an all-order growth theorem. This variant is the one compatible with the absence of a clustering requirement in YM-E; the all-distance version is optional.

## 5. The precise failure of taking absolute values before vacuum cancellation

For a complex source j and a real-on-real analytic subtraction C_a, positivity of the source-zero Wilson measure gives the exact general comparison

\[
 |H_a(j)|
 \le
 \exp\!\left(C_a[\operatorname{Re}j]
                       -\operatorname{Re}C_a[j]\right)
                         H_a(\operatorname{Re}j).
 \tag{CP.30; P}
\]

It follows by applying the triangle inequality to the original integral. Thus even a uniform real-source estimate for H_a leaves a second factor to control on a complex domain. The source-local vacuum cannot be omitted from that factor.

For j=itf the real source is zero. At each fixed cutoff, real Taylor coefficients imply

\[
 -\operatorname{Re}C_a[itf]
     =\frac{t^2}{2}D^2C_a(0)[f,f]+O_a(t^4).
 \tag{CP.31; P: finite-cutoff Taylor identity}
\]

The remainder is deliberately written O_a. The lower bound (CP.17) does **not** by itself prove divergence at any fixed imaginary source: higher source terms could matter, and no uniform Taylor remainder for the actual counterterm has been proved here. What it does show is that the particular majorant produced by (CP.30) already has an ultraviolet-divergent quadratic coefficient when the contact cancellation required by R2 is made. A useful complex estimate must retain additional cancellation in the integrated numerator.

The fixed-imaginary-source loss can be seen exactly in a Gaussian energy factor. Let ξ_1,…,ξ_m be independent centered real Gaussians of variance one, and put F=(2β)⁻¹Σ_iξ_i². The nonsingular finite-dimensional Gaussian integral gives

\[
 M_{m,\beta}(z)=\mathbb E e^{zF}
       =(1-z/\beta)^{-m/2},\qquad
 C_{m,\beta}(z)=-\frac m2\log(1-z/\beta),
 \qquad |z|<\beta.
 \tag{CP.32; P}
\]

This is also the form of a constant scalar perturbation of a nonsingular Gaussian energy after diagonalizing its quadratic form. With this exact deterministic vacuum, the renormalized function is identically one. Yet applying the unsubtracted triangle inequality first gives only

\[
 |e^{-C_{m,\beta}(it)}M_{m,\beta}(it)|
       =1
       \ \le\
       e^{-\operatorname{Re}C_{m,\beta}(it)}
       =\left(1+\frac{t^2}{\beta^2}\right)^{m/4}.
 \tag{CP.33; P}
\]

If m is of order L^{4K}, β is of order K, and t≠0 is fixed, the right side diverges. The left side stays exactly one. The error is entirely the loss of Gaussian characteristic-function damping that cancels the imaginary-source vacuum. Real-source stability is perfect in this example, so improving its real bound cannot repair this particular complex estimate.

The lesson for the actual construction is an order of operations, not an impossibility theorem for R2. Perform the integrations responsible for each source-dependent local vacuum before estimating the remaining complex integrand in absolute value, or work directly with a finite-jet construction such as §4. The existing complete positive Lᵖ transport is useful for already represented raw densities, but it does not supply the missing local contact cancellations or normalized separated-correlation information.

## 6. What now has to be proved for R2

There are two distinct sufficient routes. The current note does not merge their unproved premises.

**Complex finite-source route (O).** Establish the same-vacuum complete marked-pressure estimate and torus-independent local vacuum comparison in the existing R2 contract. The source-zero lower bound can then supply the final denominator, and the established reflection argument can localize the resulting bound where its literal source placements are correct. The estimate must be obtained after the integrations and vacuum cancellations to which §5 applies. It cannot be obtained merely by replacing a complex source by its real part in the original unintegrated Wilson integral.

**Scalar two-jet route (O inputs, C completion theorem).** Establish the ultraviolet part of (CP.25) for the actual normalized connected kernel, the macroscopic smeared bound (CP.29b), and (CP.28) for the specified counterterm. Theorem 4.3 then completes the first and second scalar normalization bounds for fixed supported tests, allowing macroscopic phase correlations. This route avoids both a full complex-source disk and a pointwise logarithm on every retained history. The all-distance version in Theorem 4.2 is an optional stronger sufficient route, not a requirement of YM-E. Higher source orders, tensor transport, and the growth condition needed for the full field hierarchy remain separate.

The required checks in a proposed proof are as follows.

| Proposed input or step | What must be shown |
|---|---|
| The observable in the connected kernel | It is the same original physical insertion, with the chosen running field normalization, carried through every old integration. It is not a centered conditional replacement. |
| Complete normalization | The numerator and denominator contain the same actual old masses, cutoffs, constraints, selectors and future continuation. Neither a fresh normalized reference nor a source-free local upper bound performs this comparison. |
| Ultraviolet annuli and macroscopic covariance | The ultraviolet constant controls the full normalized covariance on short separation shells. The independent macroscopic smeared bound can retain non-clustering phase correlations. A fixed-background Gaussian covariance, or decay attached only to regular activities, supplies neither input until all mixed terms and histories are included. |
| Contact matching | The coefficients extracted by the actual E/R vacuum recipe agree with the Taylor-local coefficients up to the uniform bounds in (CP.28), including their finite-volume dependence. |
| Field-valued contacts | Any exterior-dependent curvature or tensor output is retained and projected as such. It cannot be counted as the deterministic identity coefficient in (CP.23). |
| Source placement and reflection | The original lattice anchors and tensor transformation are used, or their stated correction is proved quantitatively. Translation covariance alone does not resolve the anchor issue. |

Theorem 2.2 supplies a sharp qualitative test for the contact ledger: a claimed scalar two-jet construction with no divergent quadratic identity coefficient cannot be correct for a plateau source. Sections 3.2–3.3, namely (CP.18)–(CP.21), supply a separate test for the normalization ledger: a bound that contains only the local energy budget has not yet controlled separated connected insertions.

The non-clustering two-jet criterion requires neither a mass gap nor long-distance power decay. Its dimension-eight annular estimate is an ultraviolet requirement; its separate macroscopic bound allows a constant covariance component. Other distributional kernel norms could replace these inputs if their contact-extension argument is proved. The current version is deliberately concrete so that another researcher can try to establish its precise estimates from the actual mixed RG transition.

For a nontrivial continuum scalar field, its actual running multiplicative normalization must be fixed before applying this criterion. Multiplying the bare scalar by a scale-dependent factor changes the kernel in (CP.22) and the contact coefficients in (CP.23). The lower variance bound scales by the square of that factor. The present analysis does not select or prove the required field normalization.

No new interface is assumed. The choice of a finite-jet proof space is permitted by the proof strategy of [lattice_conventions.md](lattice_conventions.md) §5. What remains missing is a bound for an actual normalized interacting kernel and its prescribed contact recipe, not a missing definition of the finite-dimensional derivative.

## 7. Checked primary statements and their exact scope

The actual variance theorem and the deterministic identities in §§2–5 have independent proofs above; they do not use an unverified extension of a Balaban theorem.

| Primary source and printed page | Checked statement, labelled L in its printed scope | Consequence and limitation for this note |
|---|---|---|
| Bałaban, CMP119 (1988), 243–285, p.259, (2.24)–(2.28) | The inductive regular action has the localized field-independent subtraction and Wilson projection in (2.25). Its activities have the specified localization, analytic extension, gauge invariance and bounds. The displayed spatial coupling is generated by the construction's cutoff functions in (2.24). | This is a precise source-free extraction recipe. Its spatial cutoff dependence is not a theorem for an arbitrary external scalar or clover source. |
| Same paper, p.260, (2.30)–(2.31) | R terms receive a field-independent subtraction and satisfy the stronger small-coupling activity bound. The text explains why their resulting marginal terms can be summed over generations without another Wilson counterterm. | The bound concerns the activities actually constructed on their prescribed determining-field domains. A derivative with respect to an additional physical source must still be admitted and estimated. |
| Same paper, p.262, paragraph beginning with the constant E_k, and Theorem 1 | The initial vacuum constant is defined from whole-lattice small-field one-step vacuum expressions; local one-step terms are subsequently subtracted. Theorem 1 propagates the stated induction assumptions for the stipulated coupling sequence. The final remark describes a possible formulation on all densities satisfying the same assumptions. | Sourced admission is the missing issue. The remark does not drop localization, domains, covariance, or the identity and marginal subtractions. This note does not check the complete running-coordinate dictionary needed to apply the theorem on the N2-F physical trajectory. |
| Same paper, p.264, Corollary 3, (2.50) | Under Theorem 1's assumptions the full effective density has the printed ultraviolet upper bound and small-field lower bound, with constants independent of the fine spacing and torus in that construction. | Once corresponding uniform sourced assumptions have actually been established, this is the source-free pattern for the final normalization step. It does not provide (CP.25) for marked normalized correlations. |
| Bałaban, LFR II, CMP122 (1989), 355–392, p.380, (1.73)–(1.75) | A complex-background old operation is compared with a positive real-background operation using its small exponent σ. The real old mass is positive; the normalized quotient acts on an F whose supremum enters the estimate. | Positivity controls the displayed quotient on its admitted domain. It does not remove the need to estimate the actual old physical-source readout F, or make the old mass a constant. |
| Same paper, p.390, (1.98)–(1.100) | The convergent connected expansion exponentiates to local R′ activities, analytic in the determining variables (U,J), with the stated tree decay and additional large-field smallness for interior R terms. | Here J is Balaban's determining variable. It is not the external physical source of this program. A bound for the complete marked connected kernel is additional work. |
| Same paper, pp.391–392, (1.103)–(1.104) and the paragraph continuing on p.392 | The old masses T′_k(Y_i)1 are factored out of normalized operations and survive as multiplicative functions of the new field restricted to Y_i. Their dependence is explicitly retained in the alternative density representation. | The factors must remain in the actual normalized kernel used in (CP.22). Normalizing the operations in the bracket does not establish a normalized physical insertion estimate. |

These pages explain why the two remaining inputs in §4 are substantial. The source-free construction does contain local vacuum and marginal projections, and its complete density has stability bounds under the printed hypotheses. What has not been supplied is a proof that the additional physical-source derivatives satisfy those hypotheses through every mixed E/R/B step, or an independent proof of the complete normalized annular estimate.

The missing N0 dictionary is not filled in here. No formula beyond the cited pages is used. Nor is a source-free bound on a local activity restated as an L bound on the normalized covariance (CP.22).

## 8. Summary

R2 remains open for the complete Wilson construction. A new theorem identifies an unavoidable part of its source counterterm. For every SU(N), every finite periodic lattice with at least two sites per direction, and sufficiently large bare coefficient β, the variance of a literal scalar plateau insertion is bounded below by c times the number of fine plateau links divided by β². Along N2-F this diverges at least as a⁻⁴ divided by (K+1)².

The proof retains the actual normalized measure. An elementary low-temperature partition estimate makes near-flat exterior stars probable. Centering such a star at its minimum gives uniform quadratic confinement; two thermal annuli then give conditional variance. A bounded-degree packing selects conditionally independent stars. Total variance proves the full lower bound without discarding covariances or survivor masses.

Consequently a cutoff-uniform two-jet requires a divergent quadratic identity contact. For separated supports with vanishing mixed counterterm, the requested normalized bound is an actual connected covariance estimate. Weighted energy control alone cannot supply that information. A Gaussian calculation also shows exactly why taking absolute values before subtracting the integrated vacuum loses the damping needed at imaginary sources.

The positive reduction is a finite-jet route. Short-distance annular bounds for the complete normalized covariance, a separate macroscopic smeared bound, and matching of the prescribed local counterterm imply uniform first and second derivatives. Taylor subtraction through degree four leaves a fifth-order remainder, whose scale sum converges. The macroscopic bound permits constant phase correlations and therefore does not impose clustering. An all-distance decay version is only an optional stronger criterion.

The cited Balaban pages supply source-free local extraction and stability statements, not these additional marked estimates. Proving the actual ultraviolet covariance bound, macroscopic control, and contact matching remains open. Tensor mixing and all-order growth are separate. All estimates must use the unchanged physical source and trajectory.
