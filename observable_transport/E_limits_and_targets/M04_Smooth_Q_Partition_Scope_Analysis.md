# What an exact smooth partition of a hard Q sector does and does not prove

This note examines one route for extending the construction to the nonlinear sector. Smooth sector weights can be introduced with an exact positive partition. Such a partition does not make the recombined hard-Q kernel smooth or holomorphic in its retained field. The useful smooth comparison in PJ/SC instead has fixed real integration domains, with the old hard-domain defects explicitly retained elsewhere.

## 1. A literal positive partition

On a finite native chart let a Q event be

\[
D(W)=\{z:\|A_\lambda(W,z)\|_{\rm op}<2gP
                 \text{ for every }\lambda\in\mathcal I\},
\]

where the A's are the actual real group-matrix differences occurring in its finite collection of tests. This notation does not discard their reference fields or determining inputs. Suppose a strict inner core has all these differences at most \(\gamma gP\), for a fixed \(\gamma<2\).

Choose an integer m and constants \(0<a<b<2\) such that
\(N^{1/(2m)}\gamma<a\). Let chi be a smooth scalar function with values in [0,1], equal to one below \(a^{2m}\) and zero above \(b^{2m}\). Define

\[
\psi(W,z)=\prod_{\lambda\in\mathcal I}
\chi\!\left(
 \frac{\operatorname{Tr}[(A_\lambda^*A_\lambda)^m]}
      {(gP)^{2m}}\right).
\]

The Schatten-norm inequalities
\(\|A\|_{\rm op}\le\{\operatorname{Tr}(A^*A)^m\}^{1/(2m)}
\le N^{1/(2m)}\|A\|_{\rm op}\)
show that psi is one on the strict inner core and has support inside D. It is gauge invariant whenever the complete Q test is transformed with its references, since the trace is invariant under unitary conjugation. It uses exactly the determining inputs of those tests.

For the literal hard weight \(\rho=1_D\),

\[
\rho=\psi+(\rho-\psi),\qquad
0\le\psi\le\rho,\qquad 0\le\rho-\psi.
\]

This is an exact positive partition **inside the Q sector**. Its residual is still supported on D and retains the hard outer boundary. It is not the replacement of the original complementary P/Q decomposition by a new whole-space partition.

For a positive density p, let \(Z_s=\int p\psi\), \(Z_r=\int p(\rho-\psi)\), and \(Z_Q=Z_s+Z_r\). The normalized conditional identity is

\[
q_Q f=\frac{Z_s}{Z_Q}\,q_s f+\frac{Z_r}{Z_Q}\,q_r f.
\]

Zero-mass terms may be omitted. A derivative of this identity includes the two varying masses and the residual domain response. Discarding any of those terms changes the original kernel.

## 2. A small residual can retain an actual cusp

The following is a comparison model, not an asserted nonzero cusp witness for the Yang--Mills source.

Let \(w(z)=e^{-z^2/2}\), \(P>0\), and

\[
D(t)=[-P,P]\cap[-P+t,P+t],\qquad
q_t f=\frac{\int_{D(t)}w(z)f(z)\,dz}
            {\int_{D(t)}w(z)\,dz}.
\]

For an even smooth f, let \(Z_0=\int_{-P}^P w\) and \(m_f=q_0f\).
Expanding the missing interval at the corresponding endpoint gives

\[
\int_{D(t)}w=Z_0-w(P)|t|+O(t^2),
\]

\[
\int_{D(t)}wf=Z_0m_f-w(P)f(P)|t|+O(t^2).
\]

Therefore

\[
q_t f=m_f-\frac{w(P)}{Z_0}(f(P)-m_f)|t|+O(t^2).
\]

For \(f(z)=z^2\), \(m_f<P^2\), so this coefficient is strictly nonzero. The right and left derivatives differ. Its coefficient is exponentially small at large P, but the exact normalized function still has a cusp.

Any exact partition of this conditional into a smooth interior and its residual must reproduce this same function after recombination. The small size of the residual is useful for a rare-error norm, but cannot make this cusp disappear. NP records the analogous geometric criterion for the actual Q family; the missing source-specific nonzero witness in that criterion is not supplied by this example.

## 3. A compactly supported analytic cutoff is unavailable

The weight constructed above is smooth as a real function. It is not a holomorphic cutoff in the retained raw field. More generally, a nonzero real-analytic function on a connected real chart cannot vanish on a nonempty open exterior region and remain nonzero in its interior: the real-analytic identity theorem would force it to vanish throughout that chart. The corresponding holomorphic statement is the same.

Thus an exact nontrivial cutoff supported inside a proper hard region cannot also be analytic across that region's boundary. Smooth regularity does not supply the complex Cauchy discs used in PJ, SC and OP.

There can still be a useful analytic integrand with a fixed real integration domain, including a fixed P cutoff independent of the retained field. That is precisely different from claiming analyticity of a moving hard-Q indicator.

## 4. Consequence for the nonlinear extension

This analysis preserves the exact original sector sum and identifies the remaining work. A smooth partition may help organize real boundary estimates, but it does not close the moving-core problem by itself. The present route keeps the analytic auxiliary P family, the real Q-defect payloads, their full denominators and their labelled boundary currents separate in the mathematical representation.

The elementary example above is not a new obstruction to Yang--Mills existence or to all augmented states. It rules out the proposed inference from an exact smooth interior partition to analytic regularity of the recombined hard-cutoff law.
