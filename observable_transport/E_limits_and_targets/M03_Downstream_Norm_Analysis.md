# Does the continuum hierarchy require the full pointwise M-03 norm?

This note does not alter the stated M-04/M-06/M-07 required conclusions or claim that any of them is proved.

## 1. Finding

The full ambient pointwise supremum and exponential **volume** carrier weight of M-03 are not logically necessary for the final Schwinger-hierarchy assembly theorem. Annex U, Theorems 4.2–4.3, uses actual connected shell distributions, endpoint-tree decay, current physical dimension, fixed source-order growth, terminal bounds and summable errors. It does not use an off-support conditional-kernel version or a volume weight on a hidden component.

There is a useful quantitative refinement: the larger spatial range R_j h_j already present in the H-03 reset theorem can be paid by a fixed additional factorial exponent after shell summation, provided R_j grows at most polynomially in shell depth and the shell weights have a fixed exponential reserve. Thus reducing the range from R_j h_j to h_j is not intrinsically necessary for that downstream assembly.

This does **not** currently supply a complete alternative proof. The actual current-scale moments, complete connected shell identity including outer means, physical retained-coordinate response bounds and all-order contact comparison are still missing. Replacing M-03 by an averaged norm without those inputs would merely relocate the gap.

## 2. Exact dependency map

| Catalogue item | Actual quantitative input | Does its final conclusion require M-03's ambient supremum/full-volume weight? |
|---|---|---|
| M-06 | Exact finite-jet algebra with compatible source orders and all generated responses; its catalogue statement expressly asks for the M-03 carrier-bound sum | Yes for the stated required conclusion. A different observable proof could use a different Banach space only with an explicit replacement theorem. |
| M-07 | Uniform iteration with summable irrelevant gains, current field budgets, all histories and outer responses | The specified interface is M-03. Conditional expectation contraction in an averaged moment norm alone does not establish its current-scale budget or spatial locality. |
| H-04 | Full normalized one-step estimate for regular, successful, residual and unreplaced histories, with fixed factorial growth | True-law averaged bounds can in principle suffice for final observables; actual sector probabilities, current moments and responses must all be controlled. |
| H-05/S-04 | Exact outer-mean and connected shell decomposition for the same physical fields | Essential independently of any norm choice. Averaging within-sector cumulants alone omits outer cumulants. |
| S-05/S-02 | A physical endpoint-tree kernel majorant, or a quantitatively sufficient substitute with a fixed-factorial summation theorem | No full-volume weight or off-support supremum occurs in the stated final premises. Section 4 below supplies one sufficient substitute. |
| F-07/S-06 | Inverse-running-product-weighted additive error budget in a joint-test distribution norm, including partial diagonals and connected/full conversion | No pointwise field-space norm is intrinsically required once that joint-test budget is actually proved. |
| F-06/P-01 | Compatible source contacts, locality and separated-half-space splitting of the actual realization | Averaged moment bounds alone do not establish these algebraic/support facts. |

The sources for this map are the catalogue statements M-06, M-07, H-04, H-05, S-04–S-06, F-06–F-07 and Annex U (S.27)–(S.40). None of their actual open model-specific estimates is inferred from the map.

## 3. What averaging the true branch masses proves immediately

Let μ be an actual joint probability law, π its output marginal, and Q conditional expectation under that same joint law. For d>0 define the existing graded moment seminorm

\[
 \mathfrak m_d(A;\mu)=\sup_{p\ge1}(dp)^{-d}\|A\|_{L^p(\mu)}.
\]

### Lemma DN.1 (averaged value algebra)

The following inequalities hold with no kernel supremum or inverse rare-sector mass:

\[
 \mathfrak m_d(QA;\pi)\le\mathfrak m_d(A;\mu),             \tag{DN.1}
\]

\[
 \mathfrak m_{d+e}(AB;\mu)
 \le\mathfrak m_d(A;\mu)\mathfrak m_e(B;\mu).             \tag{DN.2}
\]

For a compatible conditional cumulant of r inputs,

\[
 \|\kappa_Q(A_1,\ldots,A_r)\|_{L^p(\pi)}
 \le2^{r-1}r!\prod_{i=1}^r\|A_i\|_{L^{pr}(\mu)}.       \tag{DN.3}
\]

If ν_A(dy)=QA(y)π(dy) is the signed marked output measure, then

\[
 \|\nu_A\|_{\rm TV}\le\|A\|_{L^1(\mu)}.               \tag{DN.4}
\]

#### Proof

(DN.1) is conditional Jensen. (DN.2) is Hölder with exponents (d+e)/d and (d+e)/e, with the grade factors retained; it is already M.23. For (DN.3), expand the conditional cumulant by partitions, apply Hölder across blocks, conditional contraction inside each block and Hölder among its inputs. Each partition term is bounded by the displayed product. The total absolute partition coefficient is at most 2^{r-1}r!, by the permutation-and-cuts count. Finally the variation of the pushforward of Aμ is no larger than that of Aμ, proving (DN.4). QED.

These are genuine true-law statements, unchanged by any null-fiber continuation. They justify retaining the branch masses until after averaging. They do not by themselves prove that h^{4m} times the transported value has a uniform bound: a microscopic a^{-4m} bound remains a^{-4m} under contraction, with explicit loss (h/a)^{4m} in current units.

They also do not control the shifted-kernel term q_{τy} under the unshifted outer measure π(dy). That joint law need not equal the original input law. Consequently the direct/current estimates cannot be obtained by writing “conditional Jensen” after silently shifting the retained variable. A density ratio, a true coupling or a separately proved averaged response estimate is still required.

## 4. A rigorous shell theorem allowing the H-03 range

The next theorem is a sufficient substitute expressly permitted by the S-05 statement. It proves a downstream conversion, not the actual Wilson shell premise.

Let h_j=ℓ_0 L^{-j}, j≥0. Suppose an exact connected shell distribution has kernel t_{m,n,j} and satisfies, uniformly in cutoff n, source order m≥2 and component labels,

\[
 |t_{m,n,j}(x_1,\ldots,x_m)|
 \le A^{m+1}(m!)^{p_0}h_j^{-4m}w_j
 R_j^{a m+b}
 \exp\!\left[-\frac{c\tau(x_1,\ldots,x_m)}
                   {(m+d_0)R_jh_j}\right],               \tag{DN.5}
\]

where a,b≥0 and d0≥0 are fixed. The same assertion is sufficient if the right side bounds the **actual full-law expectation of the absolute random shell kernel** before its history average. No branchwise supremum is then used. Suppose

\[
 R_j\le C_R(1+j)^r,\qquad h_jw_j\le C_we^{-\lambda j},
 \quad \lambda>0.                                      \tag{DN.6}
\]

### Theorem DN.2 (polynomial range absorbed at fixed source-order cost)

On the coincidence-flat joint Schwartz space of Annex U,

\[
 \sum_j\|T_{m,n,j}\|_{6m,*}
 \le C^{m+1}(m!)^{p_0+5+r(4+a)}.                        \tag{DN.7}
\]

There is also a common shell-tail estimate

\[
 \sum_{j>J}\|T_{m,n,j}\|_{6m,*}
 \le e^{-\lambda J/2}
       C^{m+1}(m!)^{p_0+5+r(4+a)}.                       \tag{DN.8}
\]

Therefore, with the exact connected-shell identity, compatible one-point and terminal bounds, and their actual convergence/compactness premises, Annex U supplies the full hierarchy with

\[
 q=\max\{6,q_1,q_T\},\qquad
 p=\max\{1,p_T,p_0+5+r(4+a)\}.                         \tag{DN.9}
\]

Integer exponents can be obtained by rounding p upward. Constants are independent of m, cutoff, volume and shell depth.

#### Proof

Repeat the already proved physical shell argument of Annex U, Lemma 4.1, retaining the range ℓ_j=R_jh_j. Fifth-order Taylor remainder of a coincidence-flat test contributes ℓ_j^5. Successive tree leaf integrals/sums contribute ℓ_j^{4(m−1)}. The physical normalization is still h_j^{-4m}. Therefore the exact scale product is

\[
 h_j^{-4m}(R_jh_j)^5(R_jh_j)^{4(m-1)}
      =h_jR_j^{4m+1}.                                  \tag{DN.10}
\]

The factorial/tree/range-in-m counting remains the original additional power five; no field is renormalized to the longer range. Including the explicit prefactor in (DN.5),

\[
 \|T_{m,n,j}\|_{6m,*}
 \le C^{m+1}(m!)^{p_0+5}h_jw_j
        R_j^{(4+a)m+b+1}.                               \tag{DN.11}
\]

Put A0=r(4+a), B0=r(b+1). Under (DN.6), the remaining sum is bounded by

\[
 C^{m+1}\sum_{j\ge0}e^{-\lambda j}(1+j)^{A_0m+B_0}.
\]

Comparison with the gamma integral gives

\[
 \sum_{j\ge0}e^{-\lambda j}(1+j)^{A_0m+B_0}
 \le C^{m+1}\Gamma(A_0m+B_0+1)
 \le C'^{m+1}(m!)^{A_0}.                               \tag{DN.12}
\]

The second inequality follows from Stirling's bounds; the fixed polynomial power of m left after dividing by (m!)^{A0} is absorbed into C'^m. If A0=0 the sum is independent of m and the same conclusion holds.

For the tail, extract e^{-λJ/2} from e^{-λj/2} and apply the same bound with λ/2 to the remaining factor. This proves (DN.7)–(DN.8). The connected/full transformation and convergence theorem in Annex U preserve the resulting fixed exponent and linear distribution order, proving (DN.9). QED.

### Relation to the H-03 reset theorem

HS20.4 already has a spatial range proportional to (1+R_k)h and polynomial support factors when a physical insertion support is enlarged to a whole eligible component. If its inputs have the required true-law current-scale moment budget, those polynomial factors fit the fixed a,b in (DN.5). The difference between endpoint-tree distance and tree distance between component supports costs only an exponential constant: enlarging m supports by O(R_kh) changes the connecting length by at most O(mR_kh), which is divided by O(mR_kh) in the decay exponent.

This observation supplies a useful conversion for that reset sector. It does not identify the complete physical shell kernel: H-05 outer means, regular responses, collisions and unreplaced sectors must still be included. It also does not prove (DN.6) for the actual Wilson-normalized trajectory. Such a bound is expected from the intended logarithmic coupling flow but must follow from the actual admitted trajectory; choosing it as an unstated asymptotic-freedom assumption is not allowed.

## 5. Additive error and contact budgets need distributional control, not M-03 itself

For the actual inverse-running-product-weighted error distributions E_{m,n,j}, suppose one proves directly

\[
 \|E_{m,n,j}\|_{q_Em,*}
 \le a_{n,j}B^{m+1}(m!)^{p_E},\qquad
 \sum_j a_{n,j}\le\epsilon_n.                           \tag{DN.13}
\]

The triangle inequality immediately gives

\[
 \Big\|\sum_jE_{m,n,j}\Big\|_{q_Em,*}
 \le\epsilon_nB^{m+1}(m!)^{p_E}.                        \tag{DN.14}
\]

This is the F-07/S-06 budget if the errors are the actual ones, the running matrices are included before the estimate, ε_n vanishes or gives the stipulated summable comparison, and source/contact compatibility holds. If these are full-moment errors, S-01 inverse stability must first put them into connected form. M-03 is one sufficient way to prove (DN.13); it is not part of the final inequality.

There is likewise a direct averaged contact estimate. Suppose a derivative-of-measure representation of an actual error has order at most q0 m, total weighted variation M_m, and its tuples lie within physical radius ρ of a specified partial coincidence diagonal. A joint test flat on that diagonal has every finite Taylor jet there equal to zero. Taylor remainder of order ℓ≤q1 m gives a factor at most (C m ρ)^ℓ, and increases distribution order by at most q1 m. If the **actual averaged weighted variation moment** of ρ^ℓ is bounded by ε_n A^{m+1}(m!)^p, this yields a joint-test error with a fixed additional factorial exponent at most q1. The proof is Taylor's integral formula followed by total variation and expectation; the factor m^{q1m} is bounded by C^m(m!)^{q1}. Representatives of each collision block stay fixed along the Taylor path, so their Schwartz weight can be used for the variation integral.

This is useful only after locating the true contact supports and coefficients. It does not establish compatibility of lower-order contacts, the required inverse running weights, or reflection-half-space splitting. The fact that a random component has a large diameter cannot be erased by naming its coefficient a contact; its physical radius moment must actually enter the Taylor bound.

## 6. Why this is not yet an amended complete M-04 route

The valid downstream conversions above leave four precise missing inputs.

1. **Current-scale matching.** Averaged contraction preserves the microscopic a^{-4m} size. A real matching theorem must produce the h^{-4m} budget and summable irrelevant gains after local scalar/tensor/identity extraction.
2. **Spatial responses of actual transported marks.** The C-08 regular covariance theorem requires weighted gradients of the actual projected marks. Bare Lp bounds do not supply them. The shifted true-law response or a replacement coupling estimate must be proved, with normalized denominators retained.
3. **Complete shells and histories.** The full-law kernel must contain outer conditional means, all collisions and the unreplaced sector. The identity κ_total=Eκ_conditional is false in general. This remains H-04/H-05/S-04 work.
4. **Compatible contacts and additive normalization.** Direct averaged distribution estimates must be established for the exact F-06/F-07 objects with running inverses already applied, not for a differently normalized convenient field.

Until these are proved, dropping the pointwise/volume pieces would not close the downstream obligations and would not prove M-04. The genuinely established conclusion is narrower and constructive: an eventual proof may target true-law endpoint-tree kernels with polynomially enlarged range, and Theorem DN.2 supplies an exact fixed-factorial conversion to the existing OS assembly theorem. This removes an unnecessary geometric demand at the final distribution stage while leaving the actual marked analysis explicit.
