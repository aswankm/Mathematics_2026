## Problem 12. Function with an Absolute Value

Perform a complete analysis of

$$f(x) = |x^2 - 4|$$

Determine the domain, symmetry, piecewise definition, derivative, critical points, non-differentiable points, monotonicity, and extrema.

> **Why this problem:** it demonstrates how absolute value functions create corner points (non-differentiable points) where the derivative fails to exist, requiring careful piecewise analysis.

---

## Solution

### 1. Domain & Symmetry
* **Domain:** The function is defined for all real numbers: $(-\infty, \infty)$
* **Symmetry:** Evaluate $f(-x)$:
  $$f(-x) = |(-x)^2 - 4| = |x^2 - 4| = f(x)$$
  The function is an **even function** (symmetric across the $y$-axis).

### 2. Piecewise Definition & Zeros
The inner expression $x^2 - 4$ changes sign at $x = \pm 2$:
* $x^2 - 4 \ge 0 \implies x \in (-\infty, -2] \cup [2, \infty)$
* $x^2 - 4 < 0 \implies x \in (-2, 2)$

Rewriting $f(x)$ piecewise:
$$f(x) = \begin{cases} x^2 - 4, & x \le -2 \text{ or } x \ge 2 \\ -(x^2 - 4) = 4 - x^2, & -2 < x < 2 \end{cases}$$

* **Zeros ($x$-intercepts):** Set $f(x) = 0 \implies x = -2$ and $x = 2$, giving points **$(-2, 0)$** and **$(2, 0)$**.
* **$y$-intercept:** $f(0) = |0^2 - 4| = 4$, giving point **$(0, 4)$**.

### 3. Derivative and Non-Differentiable Points
Differentiating each open interval:
$$f'(x) = \begin{cases} 2x, & x < -2 \text{ or } x > 2 \\ -2x, & -2 < x < 2 \end{cases}$$

Examine the one-sided derivatives at $x = \pm 2$:
* At $x = 2$: $\lim_{x \to 2^-} f'(x) = -4$, but $\lim_{x \to 2^+} f'(x) = 4$.
* At $x = -2$: $\lim_{x \to -2^-} f'(x) = -4$, but $\lim_{x \to -2^+} f'(x) = 4$.

Since left- and right-hand derivatives do not match, $f(x)$ is **not differentiable at $x = -2$ and $x = 2$** (these are sharp corner points).

### 4. Critical Points
Critical points occur where $f'(x) = 0$ or where $f'(x)$ does not exist:
* $f'(x) = 0 \implies x = 0$ (stationary point)
* $f'(x)$ undefined $\implies x = -2$ and $x = 2$

### 5. Monotonicity (Intervals of Increase and Decrease)
Testing the sign of $f'(x)$ across the four partitioned intervals:
* **For $x \in (-\infty, -2)$**: $f'(x) = 2x < 0 \implies$ **Decreasing**
* **For $x \in (-2, 0)$**: $f'(x) = -2x > 0 \implies$ **Increasing**
* **For $x \in (0, 2)$**: $f'(x) = -2x < 0 \implies$ **Decreasing**
* **For $x \in (2, \infty)$**: $f'(x) = 2x > 0 \implies$ **Increasing**

### 6. Extrema
* **Absolute (Local) Minima:** Occur at the corner points $x = -2$ and $x = 2$ where the function transitions from decreasing to increasing:
  $$\mathbf{(-2, 0)} \quad \text{and} \quad \mathbf{(2, 0)}$$
* **Local Maximum:** Occurs at the critical point $x = 0$ where the function transitions from increasing to decreasing:
  $$\mathbf{(0, 4)}$$

### 7. Graph Sketch Summary
* The graph starts from $+\infty$ as $x \to -\infty$, decreasing along a parabolic curve until it reaches a sharp point (cusp/corner) at the $x$-axis $(-2, 0)$.
* It bounces upward, reaching a smooth local maximum peak at $(0, 4)$.
* It turns downward until hitting another sharp corner at $(2, 0)$ on the $x$-axis.
* Finally, it bounces upward again, increasing without bound toward $+\infty$ as $x \to +\infty$.
