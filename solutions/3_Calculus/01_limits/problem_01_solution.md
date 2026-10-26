### Exercise 1. Dominant Terms in a Sequence

**Statement:**  
Compute

$$
\lim_{n \to \infty} \frac{4n^2 - 3n + 1}{2n^2 + 5n - 7}.
$$

Explain why the highest-degree terms determine the result.

> **Why this exercise:** introduces the idea of a dominant term and teaches how to simplify the behavior of expressions for large arguments.

---

### Solution

#### 1. Computation of the Limit
Factor out the highest power of $n$ present in the expression ($n^2$) from both the numerator and the denominator:

$$
\lim_{n \to \infty} \frac{4n^2 - 3n + 1}{2n^2 + 5n - 7} = \lim_{n \to \infty} \frac{n^2 \left(4 - \frac{3}{n} + \frac{1}{n^2}\right)}{n^2 \left(2 + \frac{5}{n} - \frac{7}{n^2}\right)}
$$

Cancel $n^2$ from both the numerator and denominator:

$$
= \lim_{n \to \infty} \frac{4 - \frac{3}{n} + \frac{1}{n^2}}{2 + \frac{5}{n} - \frac{7}{n^2}}
$$

As $n \to \infty$, all terms divided by $n$ or $n^2$ tend to $0$:

$$
\lim_{n \to \infty} \frac{3}{n} = 0, \quad \lim_{n \to \infty} \frac{1}{n^2} = 0, \quad \lim_{n \to \infty} \frac{5}{n} = 0, \quad \lim_{n \to \infty} \frac{7}{n^2} = 0
$$

Applying limit laws:

$$
= \frac{4 - 0 + 0}{2 + 0 - 0} = \frac{4}{2} = 2
$$

---

#### 2. Why the Highest-Degree Terms Determine the Result
For very large values of $n$, the term with the highest power of $n$ grows significantly faster than lower-degree terms:

* In the numerator, $4n^2$ completely dominates $-3n + 1$.
* In the denominator, $2n^2$ completely dominates $5n - 7$.

When $n \to \infty$, the lower-order terms become negligible relative to the highest-power term, so the sequence behaves asymptotically like the ratio of its highest-degree terms:

$$
\frac{4n^2 - 3n + 1}{2n^2 + 5n - 7} \approx \frac{4n^2}{2n^2} = 2
$$

Rigorous algebraic factoring shows that these lower-order terms vanish when divided by the leading power $n^2$, leaving only the ratio of the leading coefficients $\frac{4}{2} = 2$.
