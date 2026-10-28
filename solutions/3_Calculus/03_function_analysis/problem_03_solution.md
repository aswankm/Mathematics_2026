## Problem 3. A Rational Function

Analyze the domain, zeros, asymptotes, and monotonicity of

$$f(x) = \frac{x+1}{x-2}$$

Finally, sketch a graph consistent with all the information obtained.

> **Why this problem:** it teaches how to combine the domain, limits, and derivative in the analysis of a rational function.

---

## Solution

### 1. Domain
The function is a rational function, which is defined everywhere except where the denominator is zero:
$$x - 2 = 0 \implies x = 2$$
* **Domain:** $(-\infty, 2) \cup (2, \infty)$

### 2. Intercepts (Zeros and $y$-intercept)
* **$x$-intercept (Zero):** Set $f(x) = 0$:
  $$\frac{x+1}{x-2} = 0 \implies x + 1 = 0 \implies x = -1 \quad \text{point: } (-1, 0)$$
* **$y$-intercept:** Evaluate $f(0)$:
  $$f(0) = \frac{0+1}{0-2} = -\frac{1}{2} \quad \text{point: } \left(0, -\frac{1}{2}\right)$$

### 3. Asymptotes
* **Vertical Asymptote:** Occurs where the denominator is zero and the numerator is non-zero ($x = 2$):
  $$\lim_{x \to 2^-} \frac{x+1}{x-2} = -\infty \quad \text{and} \quad \lim_{x \to 2^+} \frac{x+1}{x-2} = +\infty$$
  Thus, **$x = 2$** is a vertical asymptote.

* **Horizontal Asymptote:** Examine the limits as $x \to \pm\infty$:
  $$\lim_{x \to \pm\infty} \frac{x+1}{x-2} = \lim_{x \to \pm\infty} \frac{1 + \frac{1}{x}}{1 - \frac{2}{x}} = 1$$
  Thus, **$y = 1$** is a horizontal asymptote.

### 4. Monotonicity (First Derivative)
To find the intervals of increase and decrease, compute the first derivative using the quotient rule:
$$f'(x) = \frac{d}{dx}\left(\frac{x+1}{x-2}\right) = \frac{(1)(x - 2) - (x + 1)(1)}{(x - 2)^2} = \frac{x - 2 - x - 1}{(x - 2)^2} = \frac{-3}{(x - 2)^2}$$

* Since the numerator is always $-3$ (negative) and the denominator $(x-2)^2$ is always positive for all $x \neq 2$, we have:
  $$f'(x) < 0 \quad \text{for all } x \in (-\infty, 2) \cup (2, \infty)$$
* **Conclusion on Monotonicity:** The function is **strictly decreasing** on the intervals $(-\infty, 2)$ and $(2, \infty)$. 

### 5. Extrema
* Since $f'(x) = \frac{-3}{(x-2)^2}$ is never zero and is undefined only at $x = 2$ (which is outside the domain), **there are no local extrema**.

### 6. Graph Sketch Summary
* **Left branch ($x < 2$):** Starts near the horizontal asymptote $y = 1$ as $x \to -\infty$, passes through $(-1, 0)$ and $(0, -0.5)$, and drops down toward $-\infty$ as $x \to 2^-$.
* **Right branch ($x > 2$):** Starts from $+\infty$ as $x \to 2^+$, and decreases asymptotically toward $y = 1$ as $x \to +\infty$.
