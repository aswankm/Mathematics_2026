## Problem 3. The Product Rule — Why Is It Needed?

### Statement

For 

$$f(x) = (x^2 + 1)e^x$$

Compute the derivative. Then compare the correct result with the incorrect idea 

$$f'(x) \stackrel{?}{=} (2x)e^x$$

and explain which term is missing.

* **Why this problem:** It teaches the product rule by analyzing a common mistake.

---

### Solution

#### 1. Compute the correct derivative
Using the Product Rule $\frac{d}{dx}[u \cdot v] = u'v + uv'$:

Let $u(x) = x^2 + 1 \implies u'(x) = 2x$  
Let $v(x) = e^x \implies v'(x) = e^x$

$$f'(x) = u'(x)v(x) + u(x)v'(x)$$

$$f'(x) = (2x)e^x + (x^2 + 1)e^x$$

Factoring out $e^x$:
$$f'(x) = (x^2 + 3x + 1)e^x \quad \text{or} \quad (x^2 + 2x + 1)e^x = (x + 1)^2 e^x$$

#### 2. Compare with the incorrect idea and explain the missing term
* **Incorrect idea:** $f'(x) \stackrel{?}{=} (2x)e^x$
* **Comparison:** The incorrect attempt only takes the derivative of the first factor $(x^2 + 1)' = 2x$ and multiplies it by the unchanged second factor $e^x$, treating the product as if differentiation distributes over multiplication like addition.

* **Missing term:** The term $u(x)v'(x) = (x^2 + 1)e^x$ is completely missing. By the Product Rule, differentiating a product requires two parts:
  1. The derivative of the first function times the second function ($u'v = 2x e^x$).
  2. **Plus** the first function times the derivative of the second function ($uv' = (x^2 + 1)e^x$).
