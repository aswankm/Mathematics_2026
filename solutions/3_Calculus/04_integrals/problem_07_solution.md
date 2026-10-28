## Problem 7. Integration by Parts as Reversing the Product Rule

**Statement:**
Compute 

$$\int x e^x \, dx$$

First write the product differentiation rule and, on that basis, explain the meaning of the integration-by-parts formula. Verify the result by differentiation.

> **Why this problem:** it connects a new technique with the familiar product rule.

---

### Solution

#### 1. Background: The Product Rule and Integration by Parts
The product rule for differentiation states:
$$\frac{d}{dx}[u(x)v(x)] = u'(x)v(x) + u(x)v'(x)$$

Integrating both sides with respect to $x$:
$$u(x)v(x) = \int v(x)u'(x) \, dx + \int u(x)v'(x) \, dx$$

Rearranging the terms gives the integration-by-parts formula:
$$\int u \, dv = uv - \int v \, du$$

This shows that integration by parts is simply the product rule of differentiation written in integral form to evaluate integrals of products.

#### 2. Choose $u$ and $dv$
Let:
- $u = x \implies du = dx$
- $dv = e^x dx \implies v = e^x$

#### 3. Evaluate the Integral
Apply the integration-by-parts formula:
$$\int x e^x \, dx = x e^x - \int e^x \, dx$$
$$\int x e^x \, dx = x e^x - e^x + C$$

Factor out $e^x$:
$$\int x e^x \, dx = e^x(x - 1) + C$$

#### 4. Verification by Differentiation
Differentiate the result using the product rule:
$$\frac{d}{dx} \left[ e^x(x - 1) + C \right] = \frac{d}{dx}(e^x) \cdot (x - 1) + e^x \cdot \frac{d}{dx}(x - 1)$$
$$= e^x(x - 1) + e^x(1)$$
$$= x e^x - e^x + e^x$$
$$= x e^x$$

The derivative matches the original integrand, verifying the calculation.
