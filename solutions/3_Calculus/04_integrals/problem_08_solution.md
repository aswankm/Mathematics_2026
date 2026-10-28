## Problem 8. Choosing the Factors in Integration by Parts

**Statement:**
Compute 

$$\int x \cos x \, dx$$

Before calculating, justify why it is convenient to differentiate $x$ and integrate $\cos x$, rather than the other way around.

> **Why this problem:** it teaches that integration by parts requires a deliberate choice of factors.

---

### Solution

#### 1. Justification for the Choice of Factors
When using integration by parts ($\int u \, dv = uv - \int v \, du$), we want the new integral $\int v \, du$ to be simpler than the original.

* **Differentiating $x$ and integrating $\cos x$:**
  * Let $u = x \implies du = dx$ (the algebraic term simplifies to a constant).
  * Let $dv = \cos x \, dx \implies v = \sin x$ (the trigonometric term stays at the same level of complexity).
  * The resulting integral is $\int \sin x \, dx$, which is easy to evaluate directly.

* **Integrating $x$ and differentiating $\cos x$:**
  * Let $u = \cos x \implies du = -\sin x \, dx$.
  * Let $dv = x \, dx \implies v = \frac{1}{2}x^2$.
  * The resulting integral would be $\int -\frac{1}{2}x^2 \sin x \, dx$, which increases the power of $x$ and makes the integral more complicated than the original.

Therefore, it is convenient to choose $u = x$ to reduce the power of $x$ to $1$.

#### 2. Evaluate the Integral
Using our chosen factors:
$$\int x \cos x \, dx = x \sin x - \int \sin x \, dx$$

Evaluate the remaining integral:
$$\int x \cos x \, dx = x \sin x - (-\cos x) + C$$
$$\int x \cos x \, dx = x \sin x + \cos x + C$$

#### 3. Verification by Differentiation
Differentiate the result using the product rule to verify:
$$\frac{d}{dx} \left[ x \sin x + \cos x + C \right] = \left( 1 \cdot \sin x + x \cos x \right) - \sin x$$
$$= \sin x + x \cos x - \sin x$$
$$= x \cos x$$

The derivative matches the original integrand, confirming the solution.
