## Problem 15. A Logarithmic Rational Function

Perform a complete analysis of

$$f(x) = \frac{\ln x}{x}$$

Determine the domain, intercepts, asymptotes, monotonicity, local and global extrema, concavity, and inflection points.

> **Why this problem:** it highlights how the logarithmic rate of growth compares to linear growth, illustrating the classic maximum of $\frac{\ln x}{x}$ which plays a key role in comparing powers such as $a^b$ vs $b^a$.

---

## Solution

### 1. Domain & Intercepts
* **Domain:** Since $\ln x$ is defined only for strictly positive real numbers, the domain is:
  $$\text{Domain: } (0, \infty)$$
* **$x$-intercept:** Set $f(x) = 0 \implies \ln x = 0 \implies x = 1$. Point: **$(1, 0)$**
* **$y$-intercept:** None, since $x = 0$ is outside the domain.

### 2. Limits and Asymptotes
* **Vertical Asymptote at $x = 0^+$:**
  $$\lim_{x \to 0^+} \frac{\ln x}{x} = \frac{-\infty}{0^+} = -\infty \implies \mathbf{x = 0}$$
* **Horizontal Asymptote as $x \to \infty$:**
  Applying L'Hôpital's Rule:
  $$\lim_{x \to \infty} \frac{\ln x}{x} = \lim_{x \to \infty} \frac{1/x}{1} = 0 \implies \mathbf{y = 0}$$

### 3. Monotonicity & Extrema (First Derivative)
Compute $f'(x)$ using the quotient rule:
$$f'(x) = \frac{\left(\frac{1}{x}\right)(x) - (\ln x)(1)}{x^2} = \frac{1 - \ln x}{x^2}$$

Set $f'(x) = 0$ to find critical points:
$$1 - \ln x = 0 \implies \ln x = 1 \implies x = e$$

* **Intervals of Monotonicity:**
  * **For $0 < x < e$**: $1 - \ln x > 0 \implies f'(x) > 0$ (**Increasing**)
  * **For $x > e$**: $1 - \ln x < 0 \implies f'(x) < 0$ (**Decreasing**)

* **Extrema:**
  At $x = e$, the derivative transitions from positive to negative.
  $$f(e) = \frac{\ln e}{e} = \frac{1}{e}$$
  * **Absolute (and Local) Maximum:** $\mathbf{\left(e, \frac{1}{e}\right)}$

### 4. Concavity & Inflection Points (Second Derivative)
Compute $f''(x)$ using the quotient rule on $f'(x) = \frac{1 - \ln x}{x^2}$:
$$f''(x) = \frac{\left(-\frac{1}{x}\right)(x^2) - (1 - \ln x)(2x)}{(x^2)^2} = \frac{-x - 2x + 2x\ln x}{x^4} = \frac{x(2\ln x - 3)}{x^4} = \frac{2\ln x - 3}{x^3}$$

Set $f''(x) = 0$ to find inflection points:
$$2\ln x - 3 = 0 \implies \ln x = \frac{3}{2} \implies x = e^{3/2} = e\sqrt{e}$$

* **Intervals of Concavity:**
  * **For $0 < x < e^{3/2}$**: $2\ln x - 3 < 0 \implies f''(x) < 0$ (**Concave Down**)
  * **For $x > e^{3/2}$**: $2\ln x - 3 > 0 \implies f''(x) > 0$ (**Concave Up**)

* **Inflection Point:**
  $$f(e^{3/2}) = \frac{3/2}{e^{3/2}} = \frac{3}{2e\sqrt{e}}$$
  * Point: $\mathbf{\left(e^{3/2}, \frac{3}{2e^{3/2}}\right)}$

### 5. Graph Sketch Summary
* The graph enters from $-\infty$ moving up along the vertical asymptote $x = 0$.
* It crosses the $x$-axis at $(1, 0)$ while remaining concave down.
* It climbs to its global peak at $\left(e, \frac{1}{e}\right) \approx (2.718, 0.368)$.
* Past $x = e$, the curve descends, passing through the inflection point at $\left(e^{3/2}, \frac{3}{2e^{3/2}}\right) \approx (4.482, 0.335)$ where it transitions to concave up.
* It slowly approaches the horizontal asymptote $y = 0$ from above as $x \to \infty$.
