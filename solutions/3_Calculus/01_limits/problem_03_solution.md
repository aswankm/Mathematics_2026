### Exercise 3. A Square Root and Removing an Indeterminate Form

**Statement:**  
Compute

$$
\lim_{n \to \infty} \left(\sqrt{n^2 + 5n} - n\right).
$$

Use the conjugate expression and explain why this transformation removes the difficulty.

> **Why this exercise:** introduces conjugation as a deliberate technique for removing an indeterminate form.

---

### Solution

#### 1. Identification of Indeterminate Form
Directly evaluating the limit gives:

$$
\lim_{n \to \infty} \sqrt{n^2 + 5n} = \infty \quad \text{and} \quad \lim_{n \to \infty} n = \infty
$$

This results in the indeterminate form **$\infty - \infty$**, which cannot be evaluated directly.

---

#### 2. Computation Using the Conjugate Expression
Multiply and divide the expression by its algebraic conjugate $\left(\sqrt{n^2 + 5n} + n\right)$:

$$
\lim_{n \to \infty} \left(\sqrt{n^2 + 5n} - n\right) = \lim_{n \to \infty} \frac{\left(\sqrt{n^2 + 5n} - n\right)\left(\sqrt{n^2 + 5n} + n\right)}{\sqrt{n^2 + 5n} + n}
$$

Apply the difference of squares identity $(a - b)(a + b) = a^2 - b^2$ to the numerator:

$$
= \lim_{n \to \infty} \frac{(n^2 + 5n) - n^2}{\sqrt{n^2 + 5n} + n} = \lim_{n \to \infty} \frac{5n}{\sqrt{n^2 + 5n} + n}
$$

Factor out $n$ from the denominator:

$$
= \lim_{n \to \infty} \frac{5n}{\sqrt{n^2\left(1 + \frac{5}{n}\right)} + n} = \lim_{n \to \infty} \frac{5n}{n\sqrt{1 + \frac{5}{n}} + n}
$$

$$
= \lim_{n \to \infty} \frac{5n}{n \left(\sqrt{1 + \frac{5}{n}} + 1\right)}
$$

Cancel $n$ from both numerator and denominator:

$$
= \lim_{n \to \infty} \frac{5}{\sqrt{1 + \frac{5}{n}} + 1}
$$

As $n \to \infty$, $\frac{5}{n} \to 0$:

$$
= \frac{5}{\sqrt{1 + 0} + 1} = \frac{5}{1 + 1} = \frac{5}{2}
$$

---

#### 3. Why Transformation Removes the Difficulty
- The initial expression $\sqrt{n^2 + 5n} - n$ presented a subtraction between two infinitely large terms ($\infty - \infty$), masking how fast one grows relative to the other.
- Multiplying by the conjugate transforms the **subtraction ($\infty - \infty$)** into a **quotient of infinite terms ($\frac{\infty}{\infty}$)**.
- In this new rational form, the highest power of $n$ in both numerator and denominator can be factored out and canceled, resolving the indeterminate form and revealing the exact limit $\frac{5}{2}$.
