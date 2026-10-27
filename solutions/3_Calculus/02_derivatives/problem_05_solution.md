## Problem 5. The Chain Rule as Working Through Layers

### Statement

For 

$$f(x) = (3x^2 - 2x + 1)^5$$

Identify the inner and outer functions, compute their derivatives, and combine the result according to the chain rule. Explain the origin of the additional factor[cite: 4, 5].

* **Why this problem:** It teaches how to recognize the structure of a composition instead of memorizing the rule as a meaningless pattern[cite: 5].

---

### Solution

#### 1. Identify the inner and outer functions
* **Outer function:** $g(u) = u^5$ where $u = 3x^2 - 2x + 1$
* **Inner function:** $u(x) = 3x^2 - 2x + 1$

#### 2. Compute their derivatives
* Derivative of the outer function with respect to $u$: 
  $$g'(u) = 5u^4$$
* Derivative of the inner function with respect to $x$: 
  $$u'(x) = 6x - 2$$

#### 3. Combine using the Chain Rule
According to the Chain Rule, $\frac{d}{dx}[g(u(x))] = g'(u(x)) \cdot u'(x)$[cite: 4, 5]:

$$f'(x) = 5(3x^2 - 2x + 1)^4 \cdot (6x - 2)$$

Factoring out $2$ from the second factor gives:

$$f'(x) = 10(3x^2 - 2x + 1)^4 (3x - 1)$$

#### 4. Explain the origin of the additional factor
The additional factor $(6x - 2)$ comes directly from taking the derivative of the **inner function** $u(x) = 3x^2 - 2x + 1$[cite: 4, 5]. 

When applying the chain rule, differentiating the outer layer $u^5$ only accounts for how the output changes relative to changes in $u$[cite: 5]. The inner derivative $(6x - 2)$ acts as a scaling multiplier that accounts for how rapidly the inner value $u$ itself changes as $x$ changes[cite: 5].
