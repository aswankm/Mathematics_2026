## Problem 13. An Integral Depending on the Upper Limit

**Statement:**
Let 

$$F(x) = \int_{0}^{x} (t^2 + 1) \, dt.$$

Determine $F(x)$, compute $F'(x)$, and compare the result with the integrand. Explain in your own words why the height of the function describes the local rate of increase of the accumulated area.

> **Why this problem:** it connects differentiation and integration through the idea of accumulation.

---

### Solution

#### 1. Determine $F(x)$
Evaluate the definite integral using the Fundamental Theorem of Calculus:
$$F(x) = \int_{0}^{x} (t^2 + 1) \, dt = \left[ \frac{t^3}{3} + t \right]_{0}^{x}$$
$$F(x) = \left( \frac{x^3}{3} + x \right) - \left( \frac{0^3}{3} + 0 \right) = \frac{x^3}{3} + x$$

#### 2. Compute $F'(x)$ and Compare with the Integrand
Differentiate $F(x)$ with respect to $x$:
$$F'(x) = \frac{d}{dx} \left( \frac{x^3}{3} + x \right) = 3 \cdot \frac{x^2}{3} + 1 = x^2 + 1$$

* **Comparison:** $F'(x) = x^2 + 1$, which is identical to the original integrand $f(t) = t^2 + 1$ evaluated at $t = x$. This directly illustrates Part 1 of the Fundamental Theorem of Calculus: $\frac{d}{dx} \int_{a}^{x} f(t) \, dt = f(x)$.

#### 3. Explanation of the Rate of Accumulated Area
Imagine $F(x)$ as the total area under the curve $f(t)$ from $t = 0$ to a moving right-hand wall at $t = x$. 

When you extend the right boundary by a tiny distance $\Delta x$, the additional area gained is approximately a thin rectangle of width $\Delta x$ and height $f(x)$:
$$\Delta \text{Area} \approx f(x) \cdot \Delta x$$

Dividing both sides by $\Delta x$ gives:
$$\frac{\Delta \text{Area}}{\Delta x} \approx f(x)$$

Taking the limit as $\Delta x \to 0$ yields the instantaneous rate of change of the accumulated area:
$$F'(x) = f(x)$$

Thus, the height of the function $f(x)$ dictates how fast the total accumulated area grows at that exact location.
