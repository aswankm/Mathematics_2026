## Problem 2. Powers, Roots, and the Domain

### Statement

For 

$$f(x) = 2\sqrt{x} - \frac{3}{x^2} + x^{3/2}$$

1. Rewrite the function using powers,
2. Determine the domain,
3. Compute the derivative,
4. Compare the domain of the function with the domain of its derivative.

* **Why this problem:** It teaches how to rewrite different forms so that the power rule can be applied and how to keep track of the domain.

---

### Solution

#### 1. Rewrite the function using powers
Convert radicals and reciprocals to fractional and negative exponents:
$$f(x) = 2x^{1/2} - 3x^{-2} + x^{3/2}$$

#### 2. Determine the domain
* $\sqrt{x} = x^{1/2}$ requires $x \ge 0$.
* $x^{3/2} = (\sqrt{x})^3$ also requires $x \ge 0$.
* $\frac{3}{x^2} = 3x^{-2}$ requires $x \neq 0$ (division by zero is undefined).

Combining these restrictions ($x \ge 0$ and $x \neq 0$):
$$\text{Domain of } f(x) = (0, \infty) \quad \text{or} \quad \{x \in \mathbb{R} \mid x > 0\}$$

#### 3. Compute the derivative
Apply the Power Rule $\frac{d}{dx}[x^n] = n x^{n-1}$ term-by-term:

$$f'(x) = 2 \cdot \left(\frac{1}{2}x^{-1/2}\right) - 3 \cdot \left(-2x^{-3}\right) + \frac{3}{2}x^{1/2}$$

$$f'(x) = x^{-1/2} + 6x^{-3} + \frac{3}{2}x^{1/2}$$

Converting back to radical/fractional form:
$$f'(x) = \frac{1}{\sqrt{x}} + \frac{6}{x^3} + \frac{3}{2}\sqrt{x}$$

#### 4. Compare the domains
* **Domain of $f(x)$:** $(0, \infty)$
* **Domain of $f'(x)$:** $(0, \infty)$

**Comparison:** 
In this case, the domain of the derivative $f'(x)$ is **identical** to the domain of the original function $f(x)$, which is $(0, \infty)$. The term $\sqrt{x}$ originally allowed $x=0$, but the term $\frac{3}{x^2}$ already excluded $x=0$ from the domain of $f(x)$. Thus, differentiating does not restrict the domain any further.
