## Problem 1. A Cubic Polynomial

Analyze the monotonicity and extrema of

$$f(x) = x^3 - 3x^2 + 2$$

Sketch the graph based on the results and mark the critical points.

> **Why this problem:** it teaches how to use the first derivative to describe the shape of a polynomial.

---

## Solution

### 1. Domain
Since $f(x)$ is a polynomial function, it is defined for all real numbers:
$$\text{Domain: } (-\infty, \infty)$$

### 2. First Derivative
To find the critical points and analyze monotonicity, we compute the first derivative of $f(x)$:
$$f'(x) = \frac{d}{dx}(x^3 - 3x^2 + 2) = 3x^2 - 6x = 3x(x - 2)$$

### 3. Critical Points
Set $f'(x) = 0$ to find the critical numbers:
$$3x(x - 2) = 0 \implies x = 0 \quad \text{or} \quad x = 2$$

Evaluate the function at these critical points:
* For $x = 0$: $f(0) = 0^3 - 3(0)^2 + 2 = 2 \implies \mathbf{(0, 2)}$ (Local Maximum)
* For $x = 2$: $f(2) = 2^3 - 3(2)^2 + 2 = 8 - 12 + 2 = -2 \implies \mathbf{(2, -2)}$ (Local Minimum)

### 4. Monotonicity (Intervals of Increase and Decrease)
We test the sign of $f'(x) = 3x(x - 2)$ across the intervals partitioned by the critical points:

| Interval | Test Value ($x$) | Sign of $f'(x)$ | Behavior of $f(x)$ |
| :--- | :---: | :---: | :--- |
| $(-\infty, 0)$ | $-1$ | $3(-1)(-1-2) = +9$ | Increasing |
| $(0, 2)$ | $1$ | $3(1)(1-2) = -3$ | Decreasing |
| $(2, \infty)$ | $3$ | $3(3)(3-2) = +9$ | Increasing |

* **Increasing on:** $(-\infty, 0) \cup (2, \infty)$
* **Decreasing on:** $(0, 2)$

### 5. Local Extrema
* **Local Maximum:** At $x = 0$, the derivative transitions from positive to negative. The local maximum value is $f(0) = 2$ at the point $(0, 2)$.
* **Local Minimum:** At $x = 2$, the derivative transitions from negative to positive. The local minimum value is $f(2) = -2$ at the point $(2, -2)$.

### 6. Additional Sketching Aids (Intercepts)
* **$y$-intercept:** $(0, 2)$
* **$x$-intercepts:** Solve $x^3 - 3x^2 + 2 = 0$. Since $f(1) = 0$, factoring yields:
  $$(x-1)(x^2 - 2x - 2) = 0$$
  The roots are $x = 1$ and $x = 1 \pm \sqrt{3}$ (approx. $-0.73$ and $2.73$).

### 7. Graph Sketch Summary
* The curve comes up from $-\infty$, increasing through the root at $1 - \sqrt{3}$.
* It peaks at the local maximum $(0, 2)$ (which also serves as the $y$-intercept).
* It then decreases down through the $x$-intercept at $x = 1$ to reach the local minimum at $(2, -2)$.
* Finally, it turns upward, increasing through the rightmost $x$-intercept at $1 + \sqrt{3}$ toward $+\infty$.
