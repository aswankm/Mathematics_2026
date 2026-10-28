## Problem 4. A Function with Two Vertical Asymptotes

Analyze

$$f(x) = \frac{1}{x^2 - 1}$$

Determine the domain, asymptotes, sign, and monotonicity on the intervals of the domain. Explain why each interval must be analyzed.

> **Why this problem:** it shows how vertical asymptotes partition the domain into separate intervals that must be analyzed individually.

---

## Solution

### 1. Domain
The function is defined everywhere except where the denominator equals zero:
$$x^2 - 1 = 0 \implies (x-1)(x+1) = 0 \implies x = \pm 1$$
* **Domain:** $(-\infty, -1) \cup (-1, 1) \cup (1, \infty)$

### 2. Asymptotes
* **Vertical Asymptotes:** Occur at $x = -1$ and $x = 1$.
  * At $x = -1$: $\lim_{x \to -1^-} f(x) = +\infty$, $\lim_{x \to -1^+} f(x) = -\infty$
  * At $x = 1$: $\lim_{x \to 1^-} f(x) = -\infty$, $\lim_{x \to 1^+} f(x) = +\infty$
* **Horizontal Asymptote:** 
  $$\lim_{x \to \pm\infty} \frac{1}{x^2 - 1} = 0 \implies \mathbf{y = 0}$$

### 3. Sign Analysis
Testing signs across the domain partitioned by $x = -1$ and $x = 1$:
* $(-\infty, -1)$: $f(x) > 0$
* $(-1, 1)$: $f(x) < 0$
* $(1, \infty)$: $f(x) > 0$

### 4. Monotonicity & Extrema
First derivative:
$$f'(x) = \frac{d}{dx}(x^2 - 1)^{-1} = -\frac{2x}{(x^2 - 1)^2}$$

Critical point occurs at $x = 0$.
* **Intervals of Monotonicity:**
  * $(-\infty, -1)$: $f'(x) > 0 \implies$ **Increasing**
  * $(-1, 0)$: $f'(x) > 0 \implies$ **Increasing**
  * $(0, 1)$: $f'(x) < 0 \implies$ **Decreasing**
  * $(1, \infty)$: $f'(x) < 0 \implies$ **Decreasing**
* **Local Extrema:** Local maximum at $x = 0$ with value $f(0) = -1$, yielding point **$(0, -1)$**.

> **Why each interval must be analyzed:** Vertical asymptotes create discontinuities. Features like monotonicity or sign cannot be assumed to transfer across asymptote boundaries without separate evaluation.
