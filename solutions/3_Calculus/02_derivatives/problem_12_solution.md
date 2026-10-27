## Problem 12. Several Rules at Once

### Statement

For 

$$f(x) = (x^2 + 1)^3 e^x$$

compute the derivative. Before calculating, write down a plan: which rule applies to the whole expression and which rule applies to one of its factors. Finally, organize the result by factoring out common factors.

* **Why this problem:** It practices the order of decisions when combining familiar differentiation rules.

---

### Solution

#### 1. Plan of attack
* **Main expression structure:** The function is a product of two terms, $u(x) = (x^2 + 1)^3$ and $v(x) = e^x$. Therefore, the **Product Rule** applies to the overall expression:
  $$f'(x) = u'(x)v(x) + u(x)v'(x)$$
* **Specific factor rule:** To differentiate the first factor $u(x) = (x^2 + 1)^3$, we must apply the **Chain Rule** (and Power Rule).

---

#### 2. Compute the derivatives of the individual factors
* **First factor:** $u(x) = (x^2 + 1)^3$
  $$u'(x) = 3(x^2 + 1)^2 \cdot \frac{d}{dx}(x^2 + 1) = 3(x^2 + 1)^2 \cdot (2x) = 6x(x^2 + 1)^2$$

* **Second factor:** $v(x) = e^x$
  $$v'(x) = e^x$$

---

#### 3. Apply the Product Rule
Substitute $u(x)$, $u'(x)$, $v(x)$, and $v'(x)$ into the Product Rule formula:

$$f'(x) = \left[6x(x^2 + 1)^2\right] e^x + (x^2 + 1)^3 e^x$$

---

#### 4. Organize by factoring out common factors
Identify the common factors in both terms: $(x^2 + 1)^2$ and $e^x$.

Factor them out:
$$f'(x) = (x^2 + 1)^2 e^x \cdot \left[ 6x + (x^2 + 1) \right]$$

Simplify the expression inside the brackets:
$$f'(x) = (x^2 + 1)^2 e^x (x^2 + 6x + 1)$$
