## Problem 4. A Quotient and Domain Control

### Statement

For 

$$f(x) = \frac{x^2 + 1}{x - 1}$$

Determine the domain, compute the derivative, simplify the result, and explain why the restriction $x \neq 1$ remains important[cite: 4].

* **Why this problem:** It practices the quotient rule together with domain control[cite: 4].

---

### Solution

#### 1. Determine the domain
The denominator cannot be zero[cite: 4]:
$$x - 1 \neq 0 \implies x \neq 1$$

$$\text{Domain of } f(x) = (-\infty, 1) \cup (1, \infty) \quad \text{or} \quad \{x \in \mathbb{R} \mid x \neq 1\}$$

#### 2. Compute the derivative using the Quotient Rule
Applying the Quotient Rule $\frac{d}{dx}\left[\frac{u}{v}\right] = \frac{u'v - uv'}{v^2}$[cite: 4]:

Let $u(x) = x^2 + 1 \implies u'(x) = 2x$  
Let $v(x) = x - 1 \implies v'(x) = 1$

$$f'(x) = \frac{(2x)(x - 1) - (x^2 + 1)(1)}{(x - 1)^2}$$

#### 3. Simplify the result
Expand and combine like terms in the numerator:

$$f'(x) = \frac{2x^2 - 2x - x^2 - 1}{(x - 1)^2}$$

$$f'(x) = \frac{x^2 - 2x - 1}{(x - 1)^2}$$

#### 4. Explain why the restriction $x \neq 1$ remains important
* The original function $f(x)$ is undefined at $x = 1$ because division by zero is impossible[cite: 4].
* A function cannot have a derivative at a point where it is not even defined[cite: 4].
* Even though $f'(x) = \frac{x^2 - 2x - 1}{(x - 1)^2}$ is an algebraic expression, substituting $x = 1$ gives $\frac{-2}{0}$, which is undefined[cite: 4]. Thus, the restriction $x \neq 1$ naturally persists into the domain of $f'(x)$[cite: 4].
