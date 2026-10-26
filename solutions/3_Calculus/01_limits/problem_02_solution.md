### Exercise 2. Different Growth Rates

**Statement:**  
Compute

$$
\lim_{n \to \infty} \frac{3n + 1}{n^2 + 4}, \qquad \lim_{n \to \infty} \frac{2n^3 - n}{5n^2 + 1}.
$$

Compare the two cases and formulate a general observation about the degrees of the polynomials in the numerator and denominator.

> **Why this exercise:** teaches how to compare growth rates and recognize qualitatively different cases.

---

### Solution

#### 1. First Limit Computation
Compute $\lim_{n \to \infty} \frac{3n + 1}{n^2 + 4}$:

Factor out the highest power of $n$ in the denominator ($n^2$) from both the numerator and denominator:

$$
\lim_{n \to \infty} \frac{3n + 1}{n^2 + 4} = \lim_{n \to \infty} \frac{n^2 \left(\frac{3}{n} + \frac{1}{n^2}\right)}{n^2 \left(1 + \frac{4}{n^2}\right)} = \lim_{n \to \infty} \frac{\frac{3}{n} + \frac{1}{n^2}}{1 + \frac{4}{n^2}}
$$

As $n \to \infty$, terms with $n$ in the denominator vanish ($\frac{3}{n} \to 0$, $\frac{1}{n^2} \to 0$, $\frac{4}{n^2} \to 0$):

$$
= \frac{0 + 0}{1 + 0} = 0
$$

---

#### 2. Second Limit Computation
Compute $\lim_{n \to \infty} \frac{2n^3 - n}{5n^2 + 1}$:

Factor out the highest power of $n$ in the denominator ($n^2$) from both the numerator and denominator:

$$
\lim_{n \to \infty} \frac{2n^3 - n}{5n^2 + 1} = \lim_{n \to \infty} \frac{n^2 \left(2n - \frac{1}{n}\right)}{n^2 \left(5 + \frac{1}{n^2}\right)} = \lim_{n \to \infty} \frac{2n - \frac{1}{n}}{5 + \frac{1}{n^2}}
$$

As $n \to \infty$, $\frac{1}{n} \to 0$ and $\frac{1}{n^2} \to 0$, while $2n \to \infty$:

$$
= \frac{\infty}{5} = +\infty
$$

---

#### 3. Comparison and General Observation

Let $P(n)$ be a polynomial of degree $\deg(P)$ in the numerator and $Q(n)$ be a polynomial of degree $\deg(Q)$ in the denominator:

$$
L = \lim_{n \to \infty} \frac{P(n)}{Q(n)}
$$

* **Case 1: $\deg(P) < \deg(Q)$** (Numerator has lower degree than denominator)  
  The denominator grows much faster than the numerator. The limit is always **$0$**.  
  *(Example: $\frac{3n+1}{n^2+4}$ has degrees $1 < 2$, so limit is $0$).*

* **Case 2: $\deg(P) > \deg(Q)$** (Numerator has higher degree than denominator)  
  The numerator grows much faster than the denominator. The limit is always **infinite ($\pm\infty$)**.  
  *(Example: $\frac{2n^3-n}{5n^2+1}$ has degrees $3 > 2$, so limit is $+\infty$).*

* **Case 3: $\deg(P) = \deg(Q)$** (Numerator and denominator have equal degrees)  
  The limit is finite and equal to the **ratio of the leading coefficients**.
