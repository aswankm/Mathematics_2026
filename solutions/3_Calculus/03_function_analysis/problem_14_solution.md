## Problem 14. A Rational Function with Slant Asymptote & Extremum Analysis

Perform a complete analysis of

$$f(x) = \frac{x^3}{x^2 - 1}$$

Determine the domain, symmetry, intercepts, asymptotes (vertical and oblique), monotonicity, local extrema, concavity, and inflection points.

> **Why this problem:** it demonstrates how odd symmetry, vertical asymptotes, and an oblique asymptote interact with higher-degree numerators to govern global curve behavior.

---

## Solution

### 1. Domain & Symmetry
* **Domain:** Denominator equals zero when $x^2 - 1 = 0 \implies x = \pm 1$.
  $$\text{Domain: } (-\infty, -1) \cup (-1, 1) \cup (1, \infty)$$
* **Symmetry:** Evaluate $f(-x)$:
  $$f(-x) = \frac{(-x)^3}{(-x)^2 - 1} = \frac{-x^3}{x^2 - 1} = -f(x)$$
  The function is an **odd function** (symmetric with respect to the origin).

### 2. Intercepts
* Set $f(x) = 0 \implies x^3 = 0 \implies x = 0$.
* Both $x$-intercept and $y$-intercept are at the origin **$(0, 0)$**.

### 3. Asymptotes & Algebraic Restructuring
Perform polynomial division to decompose $f(x)$:
$$f(x) = x + \frac{x}{x^2 - 1}$$

* **Vertical Asymptotes:** Occur at $x = -1$ and $x = 1$.
  * At $x = 1$: $\lim_{x \to 1^-} f(x) = -\infty$, $\lim_{x \to 1^+} f(x) = +\infty$
  * At $x = -1$: $\lim_{x \to -1^-} f(x) = -\infty$, $\lim_{x \to -1^+} f(x) = +\infty$
* **Oblique (Slant) Asymptote:** As $|x| \to \infty$, the term $\frac{x}{x^2 - 1} \to 0$.
  * Oblique Asymptote: **$y = x$**

### 4. Monotonicity & Extrema (First Derivative)
Compute $f'(x)$ using the quotient rule:
$$f'(x) = \frac{3x^2(x^2 - 1) - x^3(2x)}{(x^2 - 1)^2} = \frac{3x^4 - 3x^2 - 2x^4}{(x^2 - 1)^2} = \frac{x^4 - 3x^2}{(x^2 - 1)^2} = \frac{x^2(x^2 - 3)}{(x^2 - 1)^2}$$

Set $f'(x) = 0$:
$$x^2(x^2 - 3) = 0 \implies x = 0 \quad \text{or} \quad x = \pm\sqrt{3}$$

* **Intervals of Monotonicity:**
  * **Increasing ($f'(x) > 0$):** $(-\infty, -\sqrt{3})$ and $(\sqrt{3}, \infty)$
  * **Decreasing ($f'(x) < 0$):** $(-\sqrt{3}, -1)$, $(-1, 0)$, $(0, 1)$, and $(1, \sqrt{3})$

* **Local Extrema:**
  * **Local Maximum:** At $x = -\sqrt{3}$, $f(-\sqrt{3}) = \frac{-3\sqrt{3}}{2} \implies \mathbf{\left(-\sqrt{3}, -\frac{3\sqrt{3}}{2}\right)}$
  * **Local Minimum:** At $x = \sqrt{3}$, $f(\sqrt{3}) = \frac{3\sqrt{3}}{2} \implies \mathbf{\left(\sqrt{3}, \frac{3\sqrt{3}}{2}\right)}$
  * At $x = 0$, $f'(0) = 0$, but the sign of $f'(x)$ does not change (stationary inflection point, not an extremum).

### 5. Concavity & Inflection Points (Second Derivative)
Compute $f''(x)$:
$$f''(x) = \frac{d}{dx}\left(\frac{x^4 - 3x^2}{(x^2 - 1)^2}\right) = \frac{2x(x^2 + 3)}{(x^2 - 1)^3}$$

Set $f''(x) = 0 \implies 2x(x^2 + 3) = 0 \implies x = 0$ (since $x^2 + 3 > 0$ for all real $x$).

* **Intervals of Concavity:**
  * **Concave Down ($f''(x) < 0$):** $(-\infty, -1)$ and $(0, 1)$
  * **Concave Up ($f''(x) > 0$):** $(-1, 0)$ and $(1, \infty)$

* **Inflection Point:** At $x = 0$, $f(0) = 0$, giving the inflection point at **$(0, 0)$**.

### 6. Graph Sketch Summary
* **Outer Branches ($|x| > 1$):** 
  * For $x < -\sqrt{3}$, the curve approaches $y = x$ from below, rises to a local maximum at $\left(-\sqrt{3}, -\frac{3\sqrt{3}}{2}\right)$, and falls toward $-\infty$ as $x \to -1^-$.
  * For $x > \sqrt{3}$, the curve comes from $+\infty$ at $x = 1^+$, falls to a local minimum at $\left(\sqrt{3}, \frac{3\sqrt{3}}{2}\right)$, and rises toward $y = x$ as $x \to +\infty$.
* **Central Branch ($-1 < x < 1$):**
  * The curve enters from $+\infty$ near $x = -1^+$, decreases while concave up toward the origin $(0, 0)$, passes through the inflection point at $(0, 0)$ to become concave down, and continues decreasing toward $-\infty$ as $x \to 1^-$.
