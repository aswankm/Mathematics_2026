## Problem 10. Definite Integral and Checking the Result

**Statement:**
Before carrying out the exact calculation, estimate the possible range of values of the integral

$$\int_{0}^{2} (x^2 + 1) \, dx$$

using

$$1 \leq x^2 + 1 \leq 5$$

on $[0, 2]$. Only then compute the integral exactly, compare the result with the earlier estimate, and explain what type of computational error such a check can detect.

> **Why this problem:** it teaches how to predict the possible range of a result and check the calculation.

---

### Solution

#### 1. Estimate the Range of the Integral
Using the property of bounds for definite integrals, if a function is bounded by $m \leq f(x) \leq M$ on an interval $[a, b]$, then:
$$m(b - a) \leq \int_{a}^{b} f(x) \, dx \leq M(b - a)$$

Here, the interval is $[0, 2]$, so $b - a = 2 - 0 = 2$.
Given that $1 \leq x^2 + 1 \leq 5$:
* **Lower Bound Estimate:** $1 \times (2 - 0) = 2$
* **Upper Bound Estimate:** $5 \times (2 - 0) = 10$

Thus, the value of the integral must lie between $2$ and $10$ ($2 \leq \int_{0}^{2} (x^2 + 1) \, dx \leq 10$).

#### 2. Compute the Integral Exactly
Using the Fundamental Theorem of Calculus:
$$\int_{0}^{2} (x^2 + 1) \, dx = \left[ \frac{x^3}{3} + x \right]_{0}^{2}$$
$$= \left( \frac{2^3}{3} + 2 \right) - \left( \frac{0^3}{3} + 0 \right)$$
$$= \left( \frac{8}{3} + 2 \right) - 0 = \frac{8}{3} + \frac{6}{3} = \frac{14}{3} \approx 4.67$$

#### 3. Compare with the Estimate
The exact value $\frac{14}{3}$ (or approximately $4.67$) falls comfortably within our estimated range of $[2, 10]$, which validates our calculation.

#### 4. Type of Computational Error Detected
Checking an integral against a rough bounds estimate can detect **gross arithmetic or algebraic errors** (such as sign mistakes, severe power-rule errors, or order-of-magnitude mistakes like getting $46.7$ or $-4.67$). It cannot detect small local errors, but it serves as a powerful sanity check against unreasonable answers.
