### Exercise 6. From a Sequence to a Function — Limit at Infinity

**Statement:**  
Compute

$$
\lim_{x \to \infty} \frac{3x^2 - x + 1}{5x^2 + 4x - 2}.
$$

Compare the method with Exercise 1. Explain what changes when moving from $n$ to a real variable $x$, and what stays the same.

> **Why this exercise:** deliberately transfers a technique from sequence limits to function limits.

---

### Solution

#### 1. Computation of the Limit
Factor out the highest power of $x$ present in the expression ($x^2$) from both the numerator and denominator:

$$
\lim_{x \to \infty} \frac{3x^2 - x + 1}{5x^2 + 4x - 2} = \lim_{x \to \infty} \frac{x^2 \left(3 - \frac{1}{x} + \frac{1}{x^2}\right)}{x^2 \left(5 + \frac{4}{x} - \frac{2}{x^2}\right)}
$$

Cancel $x^2$ from both the numerator and denominator:

$$
= \lim_{x \to \infty} \frac{3 - \frac{1}{x} + \frac{1}{x^2}}{5 + \frac{4}{x} - \frac{2}{x^2}}
$$

As $x \to \infty$, all terms divided by $x$ or $x^2$ approach $0$:

$$
\lim_{x \to \infty} \frac{1}{x} = 0, \quad \lim_{x \to \infty} \frac{1}{x^2} = 0, \quad \lim_{x \to \infty} \frac{4}{x} = 0, \quad \lim_{x \to \infty} \frac{2}{x^2} = 0
$$

Applying the limit laws:

$$
= \frac{3 - 0 + 0}{5 + 0 - 0} = \frac{3}{5}
$$

---

#### 2. Comparison with Exercise 1 and Analysis of Differences

##### **What Stays the Same:**
* **Algebraic Technique:** The procedure of factoring out the leading power (highest degree of the variable) in the numerator and denominator to simplify the expression remains identical.
* **Dominance Principle:** The highest-degree terms ($3x^2$ and $5x^2$) dominate the behavior of the expression as the variable grows large, making lower-order terms negligible. The result is determined by the ratio of their leading coefficients ($\frac{3}{5}$).

##### **What Changes:**
* **Domain of the Variable:**
  * In Exercise 1, $n \in \mathbb{N}$ (or positive integers), representing discrete values step-by-step ($n = 1, 2, 3, \dots$).
  * In this exercise, $x \in \mathbb{R}$, taking all continuous real values as $x \to \infty$.
* **Analytical Tools:** Because $x$ is a continuous variable, additional calculus tools like **L'Hôpital's Rule** can now be applied directly to evaluate the indeterminate form $\frac{\infty}{\infty}$ by taking derivatives with respect to $x$:

  $$
  \lim_{x \to \infty} \frac{3x^2 - x + 1}{5x^2 + 4x - 2} \stackrel{\text{H}}{=} \lim_{x \to \infty} \frac{6x - 1}{10x + 4} \stackrel{\text{H}}{=} \lim_{x \to \infty} \frac{6}{10} = \frac{3}{5}
  $$

  *(Note: L'Hôpital's Rule cannot be directly applied to discrete sequences $a_n$ without extending them to continuous functions).*
