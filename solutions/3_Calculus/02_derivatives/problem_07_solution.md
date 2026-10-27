## Problem 7. A Trigonometric Composition

### Statement

For 

$$f(x) = \sin(x^2 + 1)$$

Compute the derivative. Explicitly identify the outer function, the inner function, and the derivative of the inner function. Finally, determine the sign of $f'(0)$[cite: 5].

* **Why this problem:** It reinforces the chain rule in a different type of composition[cite: 5].

---

### Solution

#### 1. Identify the layers
* **Outer function:** $g(u) = \sin u$ where $u = x^2 + 1$
* **Inner function:** $u(x) = x^2 + 1$[cite: 5]

#### 2. Derivatives of individual functions
* **Derivative of outer function:** $g'(u) = \cos u$
* **Derivative of inner function:** $u'(x) = 2x$

#### 3. Compute $f'(x)$ using the Chain Rule
According to the Chain Rule, $f'(x) = g'(u(x)) \cdot u'(x)$:

$$f'(x) = \cos(x^2 + 1) \cdot (2x) = 2x \cos(x^2 + 1)$$

#### 4. Determine the sign of $f'(0)$
Substitute $x = 0$ into the derivative:

$$f'(0) = 2(0) \cdot \cos(0^2 + 1) = 0 \cdot \cos(1) = 0$$

Since $f'(0) = 0$, the sign of $f'(0)$ is **neither positive nor negative** (it is equal to zero).
