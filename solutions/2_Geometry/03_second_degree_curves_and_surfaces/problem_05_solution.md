### Exercise 5. Hyperbola and Asymptotes

**Statement:**  
For

$$
\frac{x^2}{16} - \frac{y^2}{9} = 1,
$$

find the intercepts with the $x$-axis, the asymptotes, and make a sketch. Explain why the asymptotes describe the behavior of the curve far from the center.

> **Why this exercise:** shows the role of asymptotes in understanding the global shape of a hyperbola.

---

### Solution

#### 1. Find Intercepts with the $x$-axis
To find the $x$-intercepts, set $y = 0$:

$$
\frac{x^2}{16} - 0 = 1 \implies x^2 = 16 \implies x = \pm 4
$$

Thus, the intercepts with the $x$-axis (the vertices of the hyperbola) are **$(-4, 0)$** and **$(4, 0)$**.

*(Note: Setting $x = 0$ gives $-\frac{y^2}{9} = 1 \implies y^2 = -9$, which has no real solutions, confirming there are no $y$-intercepts).*

---

#### 2. Find the Equations of the Asymptotes
For a canonical hyperbola $\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1$, the asymptotes are found by setting the right-hand side to $0$:

$$
\frac{x^2}{16} - \frac{y^2}{9} = 0 \implies \frac{y^2}{9} = \frac{x^2}{16} \implies y^2 = \frac{9}{16}x^2 \implies y = \pm \frac{3}{4}x
$$

The asymptotes are the straight lines **$y = \frac{3}{4}x$** and **$y = -\frac{3}{4}x$**.

---

#### 3. Why Asymptotes Describe the Behavior Far From the Center
Solve the original hyperbola equation for $y$:

$$
\frac{y^2}{9} = \frac{x^2}{16} - 1 \implies y^2 = \frac{9}{16}x^2 \left(1 - \frac{16}{x^2}\right) \implies y = \pm \frac{3}{4}x \sqrt{1 - \frac{16}{x^2}}
$$

As $x$ becomes extremely large ($x \to \pm\infty$):
- The term $\frac{16}{x^2}$ approaches $0$.
- The expression $\sqrt{1 - \frac{16}{x^2}}$ approaches $1$.

Therefore, for very large values of $|x|$, $y \approx \pm \frac{3}{4}x$. This proves mathematically that as you move far away from the center, the hyperbola gets arbitrarily close to its asymptote lines without ever touching them.

---

#### 4. Sketch Description
- **Center:** $(0, 0)$
- **Vertices:** $(-4, 0)$ and $(4, 0)$
- **Asymptote Lines:** Draw the diagonal guidelines $y = \frac{3}{4}x$ and $y = -\frac{3}{4}x$.
- **Shape:** Two symmetric smooth curves (left and right branches) opening horizontally from vertices $(-4, 0)$ and $(4, 0)$, approaching closer and closer to the diagonal asymptotes as they move outward.
