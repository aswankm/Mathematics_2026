### Exercise 11. An n-th Root

**Statement:**  
Compute

$$
\lim_{n \to \infty} \sqrt[n]{5^n + 2^n}
$$

Explain which term dominates and why the transformation looks different from the case of a quotient of polynomials[cite: 4].

> **Why this exercise:** extends the idea of dominance to exponential expressions[cite: 4].

---

### Solution

#### 1. Computation of the Limit
To evaluate the limit of the $n$-th root of a sum of exponential terms, factor out the dominant exponential term ($5^n$) from inside the radical:

$$
\lim_{n \to \infty} \sqrt[n]{5^n + 2^n} = \lim_{n \to \infty} \sqrt[n]{5^n \left(1 + \left(\frac{2}{5}\right)^n\right)}
$$

Using the properties of radicals ($\sqrt[n]{a \cdot b} = \sqrt[n]{a} \cdot \sqrt[n]{b}$), separate the terms:

$$
= \lim_{n \to \infty} \left( 5 \cdot \sqrt[n]{1 + \left(\frac{2}{5}\right)^n} \right) = 5 \cdot \lim_{n \to \infty} \left(1 + \left(\frac{2}{5}\right)^n\right)^{\frac{1}{n}}
$$

As $n \to \infty$:
* The base fraction $\frac{2}{5} < 1$, so $\left(\frac{2}{5}\right)^n \to 0$.
* The exponent $\frac{1}{n} \to 0$.

Applying these limits:

$$
= 5 \cdot (1 + 0)^0 = 5 \cdot 1 = 5
$$

---

#### 2. Dominant Term and Comparison with Polynomial Quotients

* **Which Term Dominates:**  
  The exponential term $5^n$ grows exponentially faster than $2^n$. Therefore, $5^n$ dominates the expression inside the radical as $n \to \infty$.

* **Why the Transformation Looks Different from Polynomial Quotients:**  
  * In a polynomial quotient (like in Exercises 1 and 6), terms are added or subtracted as polynomials ($P(n)/Q(n)$), allowing us to factor out the highest power of $n$ and cancel terms directly.
  * In this expression involving an $n$-th root ($\sqrt[n]{5^n + 2^n}$), the entire sum is trapped beneath a fractional power $\frac{1}{n}$. Factoring out the dominant base $5^n$ allows us to extract it entirely from the radical (since $\sqrt[n]{5^n} = 5$), leaving a benign expression that collapses to $1$ under the limit, rather than relying on direct algebraic cancellation of numerator and denominator degrees.
