# Literal narrow cutoffs: lower-bound analysis and exact Gaussian reference formula


This note retains the printed normalized radii. It does not correct a source typo, replace the original normalizers, or declare the later quiet masks to be high-probability events. The normalization issue is documented in [preparatory cutoff normalization analysis](preparatory_cutoff_normalization_analysis.md).

## 1. Analysis of the already proved first-family mass reserves

### 1.1 The first birth is unchanged

CMP119 (1.18) explicitly uses the normalized radius `delta_0/g_0`. RB, EC0 and the first-conditional theorem TM use this initial step. Their fixed-width first-coordinate boxes and the first Gaussian relative comparison do not use the ambiguous later radius. In particular LE §5's fixed small first balls concern only the initial `j=0` factor.

### 1.2 The conservative RT later box fits the smaller literal radii

The actual RT trial radius is

\[
 a_N=c g_k^{c_0}
       [C_0(1+R_k)^{c_1}]^{-c_2(N+1)}.
 \tag{NC.1}
\]

The chart/pullback loss was bounded there by a fixed power of `g_k^{-1}` times `[C(1+R_k)^c]^{C(N+1)}`. Take `c_0` larger than that fixed conversion power plus one, and `c_2` larger than its composition constant. Then the image of the box is smaller than a fixed fraction of each positive literal radius

\[
 \delta_j=g_jP_0(g_j),\qquad
 \delta'_j=g_jP_1(g_j),
 \tag{NC.2}
\]

as well as each broader radius `delta_j/g_j` or `delta'_j/g_j` where it is actually printed. Couplings on the waiting window are comparable. The required coordinate thickness cost remains

\[
 C D_{\rm tr}\big[(N+1)\log(1+R)+\log g_k^{-1}\big],
 \tag{NC.3}
\]

which was already present in RT.14 and LE's `D_late`. No new `P_0^2` term appears.

Thus the **explicit finite trial-box arithmetic** survives the smaller radii. It is wrong to justify it by saying all normalized later margins tend to infinity. The correct statement is that (NC.1), after the stated pullback loss, is smaller than the smallest actual radius, even when that radius tends to zero.

The optional claim that one can replace every later box by a fixed-radius normalized Gaussian box is also invalid for the literal radii (NC.2). A fixed-radius box is available for the broad initial factor and for any other factor whose actual radius has been verified. For a narrow `m`-dimensional factor, its volume cost includes `m log g_j^{-1}`. That cost is already allowed by (NC.3).


### 1.3 LE and ER

The direct upper estimates LE.9 and ER's canceled-energy upper only become smaller when a positive integration domain is restricted. Their fixed Gaussian gaps and positive energies are not derived from a cutoff-probability lower bound. Exact restoration ER.1–ER.2 retains the same smaller cutoffs, so its normalization identity is unchanged.

LE's lower estimate uses the broad initial all-P box and the conservative later RT box. At the level of those explicit boxes it retains the same logarithmic cost (NC.3). The unchanged denominator in ER is the original LE denominator; no new lower box is needed after restoration.

The failure-tail application is different. A literal narrow cutoff can fail at quadratic energy `O(g_j^2P_1(g_j)^2)`. Therefore it cannot be included in a catalog of implications `failure => E_* >= H_R`, with `H_R` of order `P_1(g)^2/R^9`. Only separately verified tests retain that implication.

### 1.4 Boundary-action source qualification

The preceding analysis is not a derivation of every published unmarked activity bound under the literal radius convention. A normalized Gaussian completion on a shrinking `m`-dimensional box can contain a scalar of size `m log g^{-1}`. It cannot automatically be assigned an `O(1)` bound merely by citing a broad-cutoff fluctuation theorem. On a **finite changed list** this cost can be charged by (NC.3). An extensive unchanged completion must remain in the common original baseline; it may not be discarded or counted again as a finite error.

Consequently the RT/LE/ER finite-volume arithmetic survives. Any use of a source completed-action bound whose proof depends on the unresolved radius convention still needs that convention or an exact retained-completion argument. This note does not manufacture a new cutoff-independent activity estimate.

## 2. Exact Gaussian small-box formula, with all ranks and normalizers

Let `mu` be one fixed nondegenerate centered Gaussian measure on a real physical quotient of dimension `D`, with precision `K`. Fix its normalized Lebesgue convention. A branch `s` uses an invertible linear coordinate chart

\[
 x=A_s y,\qquad K_s=A_s^T K A_s.
 \tag{NC.4}
\]

Partition `y` into blocks of dimensions `d_i`, and let `C_i` be fixed bounded, centrally symmetric sets of positive Lebesgue volume. Put

\[
 \mathcal C_s=\prod_i r_{s,i}C_i,\qquad
 V_s=\prod_i r_{s,i}^{d_i}|C_i|.
 \tag{NC.5}
\]

The exact branch Gaussian mass is

\[
 I_s=(2\pi)^{-D/2}(\det K_s)^{1/2}V_s\,
       \mathbb E_{\mathrm{Unif}(\mathcal C_s)}
              e^{-y^T K_s y/2}.
 \tag{NC.6}
\]

This formula contains both the linear chart Jacobian and the original Gaussian normalization: `(det K_s)^{1/2}=|det A_s|(det K)^{1/2}`. They are not optional normalization choices.

If every block `C_i` lies in a fixed Euclidean ball and

\[
 \epsilon_s=C D\|K_s\|_{\rm op}\max_i r_{s,i}^2,
 \tag{NC.7}
\]

then

\[
 \log I_s=
 -\tfrac D2\log(2\pi)+\tfrac12\log\det K_s
       +\sum_i d_i\log r_{s,i}+\sum_i\log|C_i|
       +e_s,\qquad -\epsilon_s\le e_s\le0.
 \tag{NC.8}
\]

**Proof.** Change variables by (NC.4), then factor out the volume (NC.5). On the product domain, `0<=y^T K_s y/2<=epsilon_s`. This proves both (NC.6) and (NC.8). No lower bound for a rare cutoff probability is used. ∎

For radii `r_{s,i}=g_{j(i)}P_{a(i)}(g_{j(i)})`, all powers of `g_j` occur explicitly in the sum in (NC.8). At a finite native rank polynomial in `R`, with a polynomial precision upper bound, `epsilon_s=g^2 poly(R,P)=o(1)`.

If the actual source includes a branch-dependent factor `c_s` outside this common Gaussian measure, the formula is for `c_s I_s`, and `log c_s` must be added. It cannot be removed separately in different branches. If the two branches have different dimensions, they must first be put on one legitimate common space with their exact auxiliary measures; (NC.8) alone does not invent that identification.

## 3. What would suffice for translated-history comparison

For two branches on the same physical Gaussian space, (NC.8) gives

\[
 \begin{split}
 \log\frac{c_sI_s}{c_tI_t}
 ={}&\log\frac{c_s}{c_t}
  +\frac12\log\frac{\det K_s}{\det K_t}\\
 &+\sum_i d_i\log r_{s,i}
      -\sum_i d_i\log r_{t,i}
      +\sum_i\log\frac{|C_{s,i}|}{|C_{t,i}|}
      +O(\epsilon_s+\epsilon_t).
 \end{split}
 \tag{NC.9}
\]

Hence a useful narrow-cutoff comparison needs the **combined** determinant, rank, radius and original-normalization ratio on the right. Matching ranks at each scale and cutoff type cancels all corresponding `g_j` and `P_a(g_j)` powers exactly. It does not by itself cancel the determinant/Jacobian or source vacuum factors.

There is no general comparison theorem from “both branches are Gaussian Schur factorizations” alone. Even in a fixed common Gaussian space, the coordinate change `A_t=2A_s` changes the leading small-box mass by `2^D` if the coordinate radii are held fixed. The energy error in (NC.8) still tends to zero. This is a finite-dimensional warning, not an actual-source counterexample: the source may have a special determinant identity, but that identity must be proved.

A promising exact geometric reduction is to match the complete per-level rectangular side-length profile among translated single-seed histories. Then the relevant native coordinate ranks and counts of each radius type agree. Because each quiet step pads by a fixed number of cells, there can be many inverse-cover phases with the same side lengths. Establishing their count and proving the remaining Gaussian determinant/source-factor comparison are separate tasks. No uniform actual history-weight conclusion is claimed here.

## 4. Marked moments on a branch-specific Gaussian reference

For a quadratic local root `F(y)=|L_s y+m_s|^2`, (NC.6) gives the elementary bound

\[
 \frac{\int_{\mathcal C_s}F(y)e^{-y^TK_sy/2}dy}
      {\int_{\mathcal C_s}e^{-y^TK_sy/2}dy}
 \le 2|m_s|^2+C\|L_s\|_{\rm op}^2
                        \sum_i d_i r_{s,i}^2.
 \tag{NC.10}
\]

For a bounded linear readout in the Gaussian energy metric, a stronger covariance estimate follows by keeping the centered convex cutoff in the Gaussian reference: its covariance is dominated by `K_s^{-1}`. This is the already proved convex-mask lemma, and does not require the mask to have high probability. A first birth innovation which is independent of the later Gaussian innovations can be treated separately, with its original event weight and original normalized first law.

Thus narrow later masks do not intrinsically create a local Gaussian-moment problem. The unresolved dilution problem is the branch weight in (NC.9), and the actual Wilson transfer still requires its exact common chart, original normalizers and perturbation bounds. Neither a rare-event division nor a redefinition of the baseline is justified by (NC.10).
