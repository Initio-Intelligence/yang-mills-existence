# Transfer normalization and the marked-insertion condition

The positive-trace comparison holds on intermediate rectangular Wilson tori. A thermal-to-vacuum comparison for polynomial insertions also requires the [marked-insertion condition](transfer_normalization.md). The Laplace estimate concerns $\beta\ge\beta_*m^{C_0}$ and gives no bound on a physically matched sequence with fixed terminal coupling.

## 1.1 The construction's definition of \(\Gamma_n\)

- **Operator.** Annex M (1.2): \(T_0=AKA\) on the full link space, with \(A=e^{-V_s/2}\), \(V_s=\beta\sum_{p\ \rm spatial}s(U_p)\), and \(K=\bigotimes_lC_\beta\) where \(C_\beta\) is convolution by \(Z_1(\beta)^{-1}e^{-\beta s}\). "The physical restriction \(T\) has the same simple positive largest eigenvalue \(\lambda_0\) as \(T_0\). Set \(H=-a^{-1}\log(T/\lambda_0)\ge0\)."
- **Trace.** Annex V after (E.2): "The trace below is the physical trace; representing the gauge-projected operator on the full link space gives the same trace". TS20 §1: "All traces below are physical traces."
- **Increment.** Annex M (4.2): \(\Gamma_n=\log[\mathcal Z_n(T_n/2)/\mathcal Z_n(T_n)]\ge0\), \(\mathcal Z_n(u)=\operatorname{Tr}e^{-uH_n}\), with \(T_n/a_n\) even. Annex V (E.1) and TS20.4 are the same quantity.

All traces are taken over the physical, gauge-invariant Hilbert space. 

*Normalization remark.* Annex M normalizes each link convolution by \(Z_1(\beta)\), so \(\operatorname{Tr}_{\rm phys}T^M=Z_1(\beta)^{-3N_n^3M}Z^W(M,N_n,N_n,N_n)\), whereas the unnormalized kernel gives \(\operatorname{Tr}P_n^M=Z^W\) for the unnormalized kernel. The factor is \(e^{\text{const}\cdot M}\), so it cancels in \(f_n\) and in the combination \(\log\operatorname{Tr}P^{N/L}-\frac1L\log\operatorname{Tr}P^N\) of Step 2. Nothing changes.

## 1.2 Theorem 2, step by step

**Step 1** (\(\Gamma_n\le\Gamma_{n,1/L}\)). \(f_n(u)=\log\sum_ie^{-uE_i}\) with \(E_i\ge0\) is nonincreasing, and \(T_n/L\le T_n/2\). 

**Step 2.** With \(\mu_i\) the eigenvalues of the (unnormalized or normalized) physical transfer operator,
\(\Gamma_{n,1/L}=\log\sum\mu_i^{N/L}-\log\sum\mu_i^N+(1-\frac1L)N\log\mu_0\), and \(\mu_0^N\le\sum\mu_i^N\). Correct; it uses only an upper bound on the top eigenvalue.

**Step 3, Euclidean identity.** Re-derived: the kernel of \(T_0\Pi\) (\(\Pi\) = gauge projection) is
\(\int\prod_xdg_x\,e^{-V_s(U)/2}\prod_{(x,i)}e^{-\beta s(U_{x,i}\,g_{x+i}U'^{-1}_{x,i}g_x^{-1})}e^{-V_s(U')/2}\).
The argument of \(s\) is the temporal plaquette with temporal links \(g_x\); the two half spatial weights of adjacent slices combine. Hence \(\operatorname{Tr}(T_0\Pi)^M=Z^W(M,N,N,N)\) with the isotropic weight \(e^{-\beta\sum_ps_p}\), for every \(M\ge1\) (for \(M=1,2\) the torus is the usual cell complex with repeated incidences). 

**Step 3, positivity in every direction.** The Wilson action is hypercubic invariant, so the same construction with any coordinate as "time" and any transverse torus \(M_1\times M_2\times M_3\) gives \(Z^W=\operatorname{Tr}Q^{M_\mu}\) with \(Q=\Pi AKA\Pi\). \(Q\ge0\) because \(K\ge0\): the class function \(e^{\beta\operatorname{Re}\operatorname{tr}g}=\sum_n\frac{\beta^n}{n!}(\operatorname{Re}\operatorname{tr}g)^n\) has nonnegative character coefficients, so convolution by it is a positive operator (Lüscher, CMP 54 (1977) 283; Osterwalder–Seiler, Ann. Phys. 110 (1978) 440; also the "positive Fourier coefficients" retained in Annex M §1). \(Q\) is trace class because its kernel is continuous on a compact space. Nothing in this uses equal side lengths. 

**Step 3, trace inequality.** For \(Q\ge0\) trace class with eigenvalues \(\mu_i\ge0\): \(\sum\mu_i^{kM}\le(\sum\mu_i^M)^k\). Applied in directions 1, 2, 3 with \(k=L\): \(Z^W(\tfrac NL,N,N,N)\le Z^W(\tfrac NL,\tfrac NL,N,N)^L\le\dots\le Z^W_{\rm cube}(\tfrac NL)^{L^3}\). Each intermediate torus is rectangular, which is allowed. 

**Step 4.** Combining gives \(\Gamma_{n,1/L}\le L^3\log Z_{\rm cube}(N/L)-L^{-1}\log Z_{\rm cube}(N)=\Phi_n/L\); four applications give \(\Phi_n\ge0\). 

## 1.3 Corollaries 2.1, 2.2 and the remarks of §2.3

- Corollary 2.2: \(\Phi_n(0)=0\) and \(\frac d{d\beta}\log Z_{\rm cube}(M)=-6M^4\langle s_p\rangle_M\). 
- "\(p_\infty\) exists by Step 3": \(M^{-4}\log Z_{\rm cube}(M)\) is nonincreasing along \(M\to LM\) and bounded below. 
- §2.4 is an identity about one factorization,. 

## 1.4 The reduction of (4.5) to (G)

**Lemma 1.1.** If \(q_n(0)\ge\eta\): \(q_n(t_n)/q_n(0)\le\exp\{\vartheta_n(\log^+q_n(S_n)+\log\eta^{-1})\}\to1\). If \(q_n(0)<\eta<1\): \(q_n(t_n)\le\eta^{1-\vartheta_n}e^{\vartheta_n\log^+q_n(S_n)}\le2\eta^{1/2}\) eventually.  So Annex M Lemma 4.1 and Theorem 4.2 need only \(\sup_np_n(F)^2<\infty\). 

**Endpoint bound.** \(q_{F,n}(S_n)=\operatorname{Tr}[X^*e^{-(T_n/2)H}X]/\mathcal Z_n(T_n)\le\lVert X\rVert^2e^{\Gamma_n}\) is Annex M (4.9). 

**Proposition 1.2.** The inequality \(\lVert X_{F,n}\rVert\le\lVert F_n\rVert_\infty\) is Annex M (4.19)–(4.20): a marked path kernel is dominated pointwise by \(\lVert F_n\rVert_\infty\) times the unmarked positive kernel, whose \(L^2\) norm over \(r/a\) steps is \(\lambda_0^{r/a}\). Then \(\lVert F_n\rVert_\infty\le\lVert f\rVert_{1,n}(\sup\lvert\Phi^R\rvert)^m\). Correct, for every degree \(m\), with a degree-dependent but \(n\)-independent prefactor. 

**The gap in the summary, and its repair.** Proposition 1.2 begins "Make the following assumptions", and those assumptions are structural, not growth conditions:

> **(S)** At each cutoff the renormalized one-field representatives are finite linear combinations \(\sum_\beta Z^{(n)}_{\alpha\beta}a_n^{-4}O_\beta+c^{(n)}_\alpha\) of **bounded functions of the link variables in a fixed finite stencil** (\(\lvert O_\beta\rvert\le C_O\)); product redefinitions are of the same kind; and each fixed \(F\) has a lattice kernel with bounded lattice \(L^1\) norm and time support in a fixed \([0,R_F]\).

(S) is what makes the transfer realization (4.3) exist with a bounded slab \(X_{F,n}\) and what gives the sup bound. The results table (T1, C1) and the "Conclusion of §1" mention only (G). The correct statement is:

> On a cubic sequence with **(S)** and **(G)**, Annex M (4.5) for every fixed \(F\) of every degree is equivalent to \(\Gamma_n=o(T_n)\).

This matters downstream. The M-07 criterion asks for "the resulting local fields, response kernels and terminal remainder"; if the fields that M-07 and F-05 finally deliver are not compact time-local stencils (for instance RG-transported marks), then (S) has to be re-proved in whatever form replaces (4.3), and (G) alone is not the full interface. Annex M itself flags this ("The finite-cutoff scheme must actually have these transfer realizations"). With (S) added, the claim "E-05's thermal route depends on later proposition only through coefficient growth" is right.

**Corollary 1.3 (arithmetic on B-02).** From `Finite Wilson family`: \(H_n=3n+O(1)\), \(K_n\le n\), \((\log Y_0)^r=L^{2n+s+1/2}\), \(r\ge2\). So \(\log(1/a_n)/T_n\to0\) and \(\log\beta_{W,n}\le L^{n+(s+1/2)/2}=o(L^{3n})\). 

A bound for a multiplication function need not be a matching lower bound for the operator norm of a slab containing that multiplication. In particular the growth of the sup norm of an insertion does not itself disprove a polynomial bound on the slab norm. The terminal-coupling sequence in which $\beta$ grows superpolynomially in the number of sites is distinct from the fixed-coupling continuum sequence.
