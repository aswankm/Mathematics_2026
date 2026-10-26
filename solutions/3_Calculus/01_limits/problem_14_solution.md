### Exercise 14. A 0/0 Limit with Trigonometry

**Statement:**  
Compute[cite: 5]

$$
\lim_{x \to 0} \frac{1 - \cos x}{x^2}.
$$

Justify the result without using L'Hôpital's rule, using a trigonometric identity and the fundamental limit[cite: 5].

> **Why this exercise:** requires combining two known tools in one argument[cite: 5].

---

### Solution

#### 1. Identification of Indeterminate Form
Directly substituting $x = 0$ into the expression yields:

$$
\frac{1 - \cos(0)}{0^2} = \frac{1 - 1}{0} = \frac{0}{0}
$$

This results in the indeterminate form $\frac{0}{0}$.

---

#### 2. Computation Using Trigonometric Identities
To evaluate the limit without L'Hôpital's rule, multiply both the numerator and the denominator by the conjugate expression $(1 + \cos x)$ or use the half-angle identity:

$$
1 - \cos x = 2 \sin^2\left(\frac{x}{2}\right)
$$

Alternatively, multiply by $(1 + \cos x)$ in the numerator and denominator:

$$
\lim_{x \to 0} \frac{1 - \cos x}{x^2} = \lim_{x \to 0} \frac{(1 - \cos x)(1 + \cos x)}{x^2(1 + \cos x)}
$$

Simplify the numerator using the Pythagorean identity $(1 - \cos^2 x = \sin^2 x)$:

$$
= \lim_{x \to 0} \frac{1 - \cos^2 x}{x^2(1 + \cos x)} = \lim_{x \to 0} \frac{\sin^2 x}{x^2 (1 + \cos x)}
$$

Rewrite the expression to isolate the fundamental limit $\lim_{x \to 0} \frac{\sin x}{x} = 1$:

$$
= \lim_{x \to 0} \left( \left(\frac{\sin x}{x}\right)^2 \cdot \frac{1}{1 + \cos x} \right)
$$

---

#### 3. Evaluation Using Limit Laws
Apply the product rule for limits:

$$
= \left( \lim_{x \to 0} \frac{\sin x}{x} \right)^2 \cdot \lim_{x \to 0} \frac{1}{1 + \cos x}
$$

* Since $\lim_{x \to 0} \frac{\sin x}{x} = 1$, the first term is $1^2 = 1$.
* For the second term, substitute $x = 0$:

$$
  \frac{1}{1 + \cos(0)} = \frac{1}{1 + 1} = \frac{1}{2}
$$

Combining these results:

$$
= 1^2 \cdot \frac{1}{2} = \frac{1}{2}
$$
