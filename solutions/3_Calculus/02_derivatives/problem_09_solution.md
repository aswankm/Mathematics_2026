## Problem 9. A Logarithm and the Chain Rule

### Statement

For 

$$f(x) = \ln(x^2 + 1)$$

Compute the derivative. Then determine the sign of $f'(x)$ for $x < 0$, $x = 0$, and $x > 0$, and describe qualitatively how the function behaves around zero

* **Why this problem:** It connects differentiation with sign analysis and the behavior of a function.

---

### Solution

#### 1. Compute the derivative
Apply the Chain Rule to $\ln(u)$ where $u(x) = x^2 + 1$:

* Outer function derivative: $\frac{d}{du}[\ln(u)] = \frac{1}{u}$
* Inner function derivative: $\frac{d}{dx}[x^2 + 1] = 2x$

$$f'(x) = \frac{1}{x^2 + 1} \cdot 2x = \frac{2x}{x^2 + 1}$$

#### 2. Determine the sign of $f'(x)$
Note that the denominator $x^2 + 1 \ge 1 > 0$ for all real numbers $x$, so the sign of $f'(x)$ is entirely determined by the numerator $2x$[cite: 6]:

* **For $x < 0$:** The numerator $2x < 0$, so $f'(x) < 0$ (Negative).
* **For $x = 0$:** $f'(0) = \frac{2(0)}{0^2 + 1} = 0$ (Zero).
* **For $x > 0$:** The numerator $2x > 0$, so $f'(x) > 0$ (Positive).

#### 3. Qualitative behavior around zero
* Since $f'(x) < 0$ for $x < 0$, the function $f(x)$ is **strictly decreasing** as it approaches zero from the left.
* At $x = 0$, the slope of the tangent line is zero ($f'(0) = 0$), indicating a **horizontal tangent**.
* Since $f'(x) > 0$ for $x > 0$, the function $f(x)$ is **strictly increasing** as $x$ moves to the right of zero.
* Consequently, the function $f(x)$ reaches a **local minimum** at $x = 0$.
