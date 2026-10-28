## Problem 15. Recovering a Function from Its Derivative and a Condition

**Statement:**
The function $F$ satisfies

$$F'(x) = 2x e^{x^2}$$

and

$$F(0) = 3.$$

1. Recognize the method needed to find the function $F$.
2. Determine the entire family of functions with the given derivative.
3. Use the condition $F(0) = 3$ to determine the correct constant.
4. Verify the final result by differentiation and substitution of $x = 0$.

> **Why this problem:** it combines recognition of substitution, the meaning of the constant of integration, and an initial condition in one problem, using only mechanisms introduced earlier.

---

### Solution

#### 1. Recognize the Method
To find the function $F(x)$ from its derivative $F'(x)$, we need to integrate the derivative:
$$F(x) = \int F'(x) \, dx = \int 2x e^{x^2} \, dx$$
Looking at the structure of the integrand, the term $2x$ is the derivative of the exponent $x^2$. Therefore, we recognize this as requiring **substitution** (reversing the chain rule).

#### 2. Determine the Entire Family of Functions
Let $u = x^2$, which gives $du = 2x \, dx$. Substituting these into the integral:
$$\int 2x e^{x^2} \, dx = \int e^u \, du = e^u + C$$
Replacing $u$ back with $x^2$, the entire family of antiderivatives is:
$$F(x) = e^{x^2} + C$$

#### 3. Determine the Correct Constant Using the Initial Condition
We are given the initial condition $F(0) = 3$. Substitute $x = 0$ into our general expression for $F(x)$:
$$F(0) = e^{0^2} + C = 3$$
$$e^0 + C = 3$$
$$1 + C = 3 \implies C = 2$$

Thus, the specific function is:
$$F(x) = e^{x^2} + 2$$

#### 4. Verify the Final Result
* **Check the derivative:**
  $$\frac{d}{dx} \left[ e^{x^2} + 2 \right] = e^{x^2} \cdot \frac{d}{dx}(x^2) + 0 = 2x e^{x^2}$$
  This matches the given derivative $F'(x)$.

* **Check the initial condition:**
  $$F(0) = e^{0^2} + 2 = 1 + 2 = 3$$
  This matches the given condition $F(0) = 3$, completely verifying the result.
