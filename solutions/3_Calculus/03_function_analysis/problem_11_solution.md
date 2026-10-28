## Problem 11. Radical Function Analysis

Perform a complete analysis of

$$f(x) = x\sqrt{4 - x^2}$$

Determine the domain, symmetry, intercepts, local extrema, and intervals of increase and decrease.

> **Why this problem:** it demonstrates how to handle product rule derivatives and domain boundary conditions involving radical functions.

---

## Solution

### 1. Domain
The expression inside the square root must be non-negative:
$$4 - x^2 \ge 0 \implies x^2 \le 4 \implies -2 \le x \le 2$$
* **Domain:** $[-2, 2]$

### 2. Symmetry
Check $f(-x)$:
$$f(-x) = (-x)\sqrt{4 - (-x)^2} = -x\sqrt{4 - x^2} = -f(x)$$
* **Conclusion:** The function is an **odd function** (symmetric with respect to the origin).

### 3. Intercepts (Zeros)
Set $f(x) = 0$:
$$x\sqrt{4 - x^2} = 0 \implies x = 0 \quad \text{or} \quad 4 - x^2 = 0 \implies x = -2, 0, 2$$
* **Points:** $(-2, 0)$, $(0, 0)$, and $(2, 0)$

### 4. First Derivative and Critical Points
Using the product rule and chain rule on $f(x) = x(4 - x^2)^{1/2}$:
$$f'(x) = (1)\sqrt{4 - x^2} + x \cdot \frac{-2x}{2\sqrt{4 - x^2}} = \sqrt{4 - x^2} - \frac{x^2}{\sqrt{4 - x^2}} = \frac{(4 - x^2) - x^2}{\sqrt{4 - x^2}} = \frac{4 - 2x^2}{\sqrt{4 - x^2}}$$

Set $f'(x) = 0$ on the interior of the domain $(-2, 2)$:
$$4 - 2x^2 = 0 \implies x^2 = 2 \implies x = -\sqrt{2} \quad \text{and} \quad x = \sqrt{2}$$

### 5. Monotonicity (Intervals of Increase and Decrease)
Testing the sign of $f'(x) = \frac{4 - 2x^2}{\sqrt{4 - x^2}}$:
* **For $x \in (-2, -\sqrt{2})$**: $f'(x) < 0 \implies$ **Decreasing**
* **For $x \in (-\sqrt{2}, \sqrt{2})$**: $f'(x) > 0 \implies$ **Increasing**
* **For $x \in (\sqrt{2}, 2)$**: $f'(x) < 0 \implies$ **Decreasing**

### 6. Local and Absolute Extrema
Evaluating $f(x)$ at critical points and boundary endpoints:

* **Boundary Endpoints:**
  * $f(-2) = 0$
  * $f(2) = 0$

* **Critical Points:**
  * At $x = -\sqrt{2}$: $f(-\sqrt{2}) = -\sqrt{2}\sqrt{4 - 2} = -\sqrt{2}\sqrt{2} = -2$ $\implies \mathbf{(-\sqrt{2}, -2)}$ (**Absolute Minimum**)
  * At $x = \sqrt{2}$: $f(\sqrt{2}) = \sqrt{2}\sqrt{4 - 2} = \sqrt{2}\sqrt{2} = 2$ $\implies \mathbf{(\sqrt{2}, 2)}$ (**Absolute Maximum**)

### 7. Graph Sketch Summary
* The graph begins at the endpoint $(-2, 0)$ and decreases into an absolute minimum at $(-\sqrt{2}, -2)$.
* It turns upwards, passing through the origin $(0, 0)$, and reaches an absolute maximum at $(\sqrt{2}, 2)$.
* Finally, it decreases from $(\sqrt{2}, 2)$ back down to the right endpoint at $(2, 0)$.
