## Problem 6. A Logarithmic Function

Analyze the domain, zero, and monotonicity of

$$f(x) = \ln x - x + 1$$

Explain why the analysis must begin with the domain.

---

## Solution

### 1. Domain
Since the logarithmic function $\ln(x)$ is only defined for strictly positive real numbers, the domain is:
$$\text{Domain: } (0, \infty)$$

> **Why analysis must begin with the domain:** We must establish the domain first because any calculus operations (such as derivatives or limits) evaluated at or outside $(0, \infty)$ are undefined for $\ln(x)$.

### 2. Zeros
To find the zeros of the function, set $f(x) = 0$:
$$\ln x - x + 1 = 0 \implies \ln x = x - 1$$
By inspection, $x = 1$ satisfies the equation:
$$\ln(1) = 0 \quad \text{and} \quad 1 - 1 = 0$$
Thus, the zero is at **$x = 1$**.

### 3. Monotonicity & Extrema
Compute the first derivative of $f(x)$:
$$f'(x) = \frac{1}{x} - 1 = \frac{1 - x}{x}$$

Since the domain is restricted to $x > 0$, the denominator $x$ is always positive. The sign of $f'(x)$ depends entirely on the numerator $1 - x$:
* **For $0 < x < 1$**: $1 - x > 0 \implies f'(x) > 0$ (the function is **increasing**).
* **For $x > 1$**: $1 - x < 0 \implies f'(x) < 0$ (the function is **decreasing**).

### 4. Absolute Maximum
At $x = 1$, the derivative transitions from positive to negative. 
* Evaluating at $x = 1$: $f(1) = \ln(1) - 1 + 1 = 0$.
* Since the function increases up to $x = 1$ and decreases thereafter, $f(1) = 0$ is an **absolute maximum**, meaning $f(x) \le 0$ for all $x$ in the domain.
