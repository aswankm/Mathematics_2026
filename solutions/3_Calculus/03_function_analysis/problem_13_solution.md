## Problem 13. A Logistic-Type Rational Function

Perform a complete analysis of

$$f(x) = \frac{e^x}{1 + e^x}$$

Determine the domain, range, asymptotes, monotonicity, extrema, concavity, and inflection points.

> **Why this problem:** it illustrates the analytical properties of the standard sigmoid/logistic curve, showing how exponential terms govern bounded behavior and smooth transition between asymptotes.

---

## Solution

### 1. Domain & Range
* **Domain:** The denominator $1 + e^x$ is strictly positive for all $x \in \mathbb{R}$ since $e^x > 0$.
  $$\text{Domain: } (-\infty, \infty)$$
* **Range:** Since $0 < e^x < 1 + e^x$ for all $x$:
  $$\text{Range: } (0, 1)$$

### 2. Intercepts & Symmetry
* **$y$-intercept:** Evaluate $f(0)$:
  $$f(0) = \frac{e^0}{1 + e^0} = \frac{1}{2} \implies \mathbf{\left(0, \frac{1}{2}\right)}$$
* **$x$-intercept:** Set $f(x) = 0 \implies e^x = 0$, which has no real solutions. There are no $x$-intercepts.
* **Symmetry:** Note that $f(-x) = \frac{e^{-x}}{1 + e^{-x}} = \frac{1}{e^x + 1} = 1 - f(x)$. 
  This implies point symmetry around $\left(0, \frac{1}{2}\right)$.

### 3. Asymptotes & End Behavior
* **Vertical Asymptotes:** None, as the denominator is never zero.
* **Horizontal Asymptotes:**
  * As $x \to -\infty$: 
    $$\lim_{x \to -\infty} \frac{e^x}{1 + e^x} = \frac{0}{1 + 0} = 0 \implies \mathbf{y = 0}$$
  * As $x \to +\infty$: 
    $$\lim_{x \to +\infty} \frac{e^x}{1 + e^x} = \lim_{x \to +\infty} \frac{1}{e^{-x} + 1} = \frac{1}{0 + 1} = 1 \implies \mathbf{y = 1}$$

### 4. Monotonicity & Extrema (First Derivative)
Compute $f'(x)$ using the quotient rule:
$$f'(x) = \frac{e^x(1 + e^x) - e^x(e^x)}{(1 + e^x)^2} = \frac{e^x + e^{2x} - e^{2x}}{(1 + e^x)^2} = \frac{e^x}{(1 + e^x)^2}$$

* Since $e^x > 0$ and $(1 + e^x)^2 > 0$ for all $x \in \mathbb{R}$:
  $$f'(x) > 0 \quad \text{for all } x \in (-\infty, \infty)$$
* **Monotonicity:** The function is **strictly increasing** on $(-\infty, \infty)$.
* **Extrema:** Because $f'(x)$ is never zero and undefined nowhere, there are **no local extrema**.

### 5. Concavity & Inflection Points (Second Derivative)
Compute $f''(x)$ using the quotient rule on $f'(x) = e^x(1 + e^x)^{-2}$:
$$f''(x) = \frac{e^x(1 + e^x)^2 - e^x \cdot 2(1 + e^x)e^x}{(1 + e^x)^4} = \frac{e^x(1 + e^x) - 2e^{2x}}{(1 + e^x)^3} = \frac{e^x(1 - e^x)}{(1 + e^x)^3}$$

Set $f''(x) = 0$:
$$e^x(1 - e^x) = 0 \implies 1 - e^x = 0 \implies e^x = 1 \implies x = 0$$

* **Intervals of Concavity:**
  * **For $x < 0$**: $e^x < 1 \implies 1 - e^x > 0 \implies f''(x) > 0 \implies$ **Concave Up**
  * **For $x > 0$**: $e^x > 1 \implies 1 - e^x < 0 \implies f''(x) < 0 \implies$ **Concave Down**

* **Inflection Point:** At $x = 0$, $f(0) = \frac{1}{2}$, yielding point $\mathbf{\left(0, \frac{1}{2}\right)}$.

### 6. Graph Sketch Summary
* The graph approaches the horizontal asymptote $y = 0$ as $x \to -\infty$.
* It increases monotonically, remaining concave up through the lower half of its range.
* At the point $\left(0, \frac{1}{2}\right)$, it passes through its inflection point, shifting from concave up to concave down.
* It continues increasing monotonically toward the upper horizontal asymptote $y = 1$ as $x \to +\infty$.
