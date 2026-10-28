## Problem 5. An Exponential Function with a Maximum


Analyze the monotonicity and extrema of

$$f(x) = xe^{-x}$$

Also examine the behavior as $x \to \infty$ and explain how the limit affects the shape of the graph on the right-hand side.

> **Why this problem:** it combines the derivative with a limit in the description of the global behavior of a function.

---

## Solution

### 1. Domain
The domain of the function is all real numbers:
$$\text{Domain: } (-\infty, \infty)$$

### 2. First Derivative and Critical Points
To find the intervals of monotonicity and extrema, we compute the first derivative using the product rule:
$$f'(x) = \frac{d}{dx}(x e^{-x}) = (1)e^{-x} + x(-e^{-x}) = e^{-x}(1 - x)$$

Set $f'(x) = 0$ to find critical points. Since $e^{-x} > 0$ for all real numbers $x$:
$$1 - x = 0 \implies x = 1$$

### 3. Monotonicity (Intervals of Increase and Decrease)
We test the sign of $f'(x) = e^{-x}(1 - x)$ around the critical point $x = 1$:
* **For $x < 1$** (e.g., $x = 0$): $f'(0) = e^{0}(1 - 0) = 1 > 0$ (Increasing)
* **For $x > 1$** (e.g., $x = 2$): $f'(2) = e^{-2}(1 - 2) = -e^{-2} < 0$ (Decreasing)

* **Increasing on:** $(-\infty, 1)$
* **Decreasing on:** $(1, \infty)$

### 4. Local Extrema
* **Local Maximum:** At $x = 1$, the derivative changes sign from positive to negative.
  $$f(1) = (1)e^{-1} = \frac{1}{e}$$
  * Local Maximum Point: $\mathbf{\left(1, \frac{1}{e}\right)}$

### 5. End Behavior and Limits as $x \to \infty$
* **As $x \to -\infty$:**
  $$\lim_{x \to -\infty} x e^{-x} = (-\infty)(\infty) = -\infty$$
* **As $x \to \infty$:**
  $$\lim_{x \to \infty} x e^{-x} = \lim_{x \to \infty} \frac{x}{e^x} = 0 \quad (\text{via L'Hôpital's Rule})
  $$
* **Effect on the Graph:** As $x$ increases toward $+\infty$, the function values decay to $0$, meaning the graph approaches the horizontal axis ($y = 0$) asymptotically from above on the right-hand side.
