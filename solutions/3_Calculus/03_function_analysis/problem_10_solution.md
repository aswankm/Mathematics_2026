## Problem 10. Complete Function Analysis

Perform a complete analysis of

$$f(x) = \frac{x}{x^2 + 1}$$

Include the domain, symmetry, zeros, limits, monotonicity, extrema, and convexity. Finally, produce a sketch based only on this information.

> **Why this problem:** it combines all the basic elements of function analysis into one organized process.

---

## Solution

### 1. Domain
Since the denominator $x^2 + 1$ is never zero for any real number $x$, the function is defined everywhere:
$$\text{Domain: } (-\infty, \infty)$$

### 2. Symmetry
Check for symmetry by evaluating $f(-x)$:
$$f(-x) = \frac{-x}{(-x)^2 + 1} = \frac{-x}{x^2 + 1} = -f(x)$$
* **Conclusion:** The function is an **odd function**, meaning its graph is symmetric with respect to the origin $(0, 0)$.

### 3. Zeros (Intercepts)
Set $f(x) = 0$:
$$\frac{x}{x^2 + 1} = 0 \implies x = 0$$
* **$x$-intercept and $y$-intercept:** Both occur at the origin **$(0, 0)$**.

### 4. Limits and End Behavior (Asymptotes)
Examine the limits as $x \to \pm\infty$:
$$\lim_{x \to \pm\infty} \frac{x}{x^2 + 1} = 0$$
* **Horizontal Asymptote:** **$y = 0$** (the $x$-axis) as $x \to \pm\infty$.
* **Vertical Asymptotes:** None, since the domain is all real numbers.

### 5. Monotonicity (First Derivative and Extrema)
Compute the first derivative using the quotient rule:
$$f'(x) = \frac{(1)(x^2 + 1) - x(2x)}{(x^2 + 1)^2} = \frac{x^2 + 1 - 2x^2}{(x^2 + 1)^2} = \frac{1 - x^2}{(x^2 + 1)^2} = \frac{(1 - x)(1 + x)}{(x^2 + 1)^2}$$

Set $f'(x) = 0$ to find critical points:
$$1 - x^2 = 0 \implies x = -1 \quad \text{or} \quad x = 1$$

* **Intervals of Monotonicity:**
  * **Decreasing on:** $(-\infty, -1)$ and $(1, \infty)$
  * **Increasing on:** $(-1, 1)$

* **Local Extrema:**
  * **Local Minimum:** At $x = -1$, with value $f(-1) = \frac{-1}{(-1)^2 + 1} = -\frac{1}{2} \implies \mathbf{\left(-1, -\frac{1}{2}\right)}$
  * **Local Maximum:** At $x = 1$, with value $f(1) = \frac{1}{1^2 + 1} = \frac{1}{2} \implies \mathbf{\left(1, \frac{1}{2}\right)}$

### 6. Convexity and Concavity (Second Derivative and Inflection Points)
Compute the second derivative:
$$f''(x) = \frac{d}{dx}\left(\frac{1 - x^2}{(x^2 + 1)^2}\right) = \frac{2x(x^2 - 3)}{(x^2 + 1)^3}$$

Set $f''(x) = 0$ to find inflection points:
$$2x(x^2 - 3) = 0 \implies x = 0, \, x = -\sqrt{3}, \, x = \sqrt{3}$$

* **Intervals of Concavity:**
  * **Concave Down ($f''(x) < 0$):** $\left(-\infty, -\sqrt{3}\right) \cup \left(0, \sqrt{3}\right)$
  * **Concave Up ($f''(x) > 0$):** $\left(-\sqrt{3}, 0\right) \cup \left(\sqrt{3}, \infty\right)$

* **Inflection Points:**
  * At $x = -\sqrt{3}$: $f(-\sqrt{3}) = -\frac{\sqrt{3}}{4} \implies \mathbf{\left(-\sqrt{3}, -\frac{\sqrt{3}}{4}\right)}$
  * At $x = 0$: $f(0) = 0 \implies \mathbf{(0, 0)}$
  * At $x = \sqrt{3}$: $f(\sqrt{3}) = \frac{\sqrt{3}}{4} \implies \mathbf{\left(\sqrt{3}, \frac{\sqrt{3}}{4}\right)}$

### 7. Graph Sketch Summary
* The graph approaches $y = 0$ from below as $x \to -\infty$.
* It is concave down until it reaches the inflection point at $\left(-\sqrt{3}, -\frac{\sqrt{3}}{4}\right)$, where it shifts to concave up.
* It hits its global minimum at $\left(-1, -\frac{1}{2}\right)$, turns upward, passes through the origin $(0, 0)$ (an inflection point), and reaches its global maximum at $\left(1, \frac{1}{2}\right)$.
* Past $x = 1$, it decreases, passes through an inflection point at $\left(\sqrt{3}, \frac{\sqrt{3}}{4}\right)$, and approaches $y = 0$ from above as $x \to +\infty$.
