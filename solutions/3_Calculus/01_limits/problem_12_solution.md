### Exercise 12. Exponential Function Limit

**Statement:**  
Compute

$$
\lim_{x \to 0} (1 + 3x)^{1/x}.
$$

Connect the result with the limit from Exercise 5 and show the appropriate transformation.

> **Why this exercise:** teaches how to recognize the classical pattern after a transformation.

---

### Solution

#### 1. Identification and Substitution
Direct substitution yields the indeterminate form $1^\infty$. 

To connect this with the fundamental limit $\lim_{t \to 0} (1 + t)^{1/t} = e$, substitute $t = 3x$.

- As $x \to 0$, $t \to 0$.
- Solving for $x$ gives $x = \frac{t}{3}$, so the exponent is:

$$
\frac{1}{x} = \frac{3}{t}
$$

Substitute these into the original limit expression:

$$
\lim_{x \to 0} (1 + 3x)^{1/x} = \lim_{t \to 0} (1 + t)^{3/t}
$$

---

#### 2. Computation Using Limit Laws
Use the power rule for exponents to isolate the standard limit:

$$
\lim_{t \to 0} (1 + t)^{3/t} = \lim_{t \to 0} \left( (1 + t)^{1/t} \right)^3
$$

Since the function $f(u) = u^3$ is continuous, bring the limit inside the power:

$$
= \left( \lim_{t \to 0} (1 + t)^{1/t} \right)^3
$$

Recall from Exercise 5 (adapted to continuous variables) that $\lim_{t \to 0} (1 + t)^{1/t} = e$:

$$
= e^3
$$

---

#### 3. Summary of Transformation
- **Pattern Recognition:** The expression $(1 + 3x)^{1/x}$ matches the classical base-e exponential form $(1 + \text{expression})^{1/\text{expression}}$.
- **Key Insight:** Substituting $t = 3x$ introduces a factor of $3$ into the exponent reciprocal, resulting in $e^3$ instead of $e^1$.
