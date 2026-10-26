### Exercise 8. A Square Root in a Function Limit

**Statement:**  
Compute

$$
\lim_{x \to 4} \frac{\sqrt{x} - 2}{x - 4}
$$

by rationalizing the numerator. Compare the idea with Exercise 3 involving a sequence.

> **Why this exercise:** reinforces transferring the same algebraic technique between two types of limits.

---

### Solution

#### 1. Identification of Indeterminate Form
Directly substituting $x = 4$ into the expression yields:

$$
\frac{\sqrt{4} - 2}{4 - 4} = \frac{2 - 2}{0} = \frac{0}{0}
$$

This results in the indeterminate form $\frac{0}{0}$.

---

#### 2. Computation Using Rationalization (Conjugate Expression)
Multiply and divide the expression by the conjugate of the numerator, $(\sqrt{x} + 2)$:

$$
\lim_{x \to 4} \frac{(\sqrt{x} - 2)}{x - 4} = \lim_{x \to 4} \frac{(\sqrt{x} - 2)(\sqrt{x} + 2)}{(x - 4)(\sqrt{x} + 2)}
$$

Apply the difference of squares identity in the numerator:

$$
= \lim_{x \to 4} \frac{x - 4}{(x - 4)(\sqrt{x} + 2)}
$$

Since $x \to 4$, we consider values of $x$ arbitrarily close to $4$ where $x \neq 4$. Cancel the common factor $(x - 4)$:

$$
= \lim_{x \to 4} \frac{1}{\sqrt{x} + 2}
$$

Evaluate the limit by direct substitution:

$$
= \frac{1}{\sqrt{4} + 2} = \frac{1}{2 + 2} = \frac{1}{4}
$$

---

#### 3. Comparison with Exercise 3

* **Common Algebraic Technique:** In both Exercise 3 (sequence limit with square roots) and this exercise (function limit with square roots), we apply the conjugate expression to eliminate square roots and clear out an indeterminate form.
* **Contextual Difference:** 
  * In Exercise 3, the conjugate eliminated an indeterminate difference of infinities ($\infty - \infty$) for a sequence as $n \to \infty$.
  * In this exercise, the conjugate eliminates an indeterminate quotient ($\frac{0}{0}$) for a function as $x$ approaches a finite point ($x \to 4$).
* **Underlying Principle:** Both problems highlight how a single core algebraic tool (multiplication by conjugates) bridges different domains (discrete sequences vs. continuous functions) to resolve limits involving radicals.
