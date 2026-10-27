## Problem 11. Derivative from the Definition

### Statement

Using only

$$f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$

find the derivative of $f(x) = x^2$. Compare the result with the power rule and indicate where the limit is used in the calculation.

* **Why this problem:** It shows the origin of the power rule and the direct connection between the derivative and a limit.

---

### Solution

#### 1. Set up the difference quotient
Substitute $f(x) = x^2$ into the limit definition of the derivative:

$$f'(x) = \lim_{h \to 0} \frac{(x + h)^2 - x^2}{h}$$

#### 2. Expand and simplify algebraically
Expand the term $(x + h)^2$:

$$f'(x) = \lim_{h \to 0} \frac{x^2 + 2xh + h^2 - x^2}{h}$$

Cancel $x^2 - x^2 = 0$ in the numerator:

$$f'(x) = \lim_{h \to 0} \frac{2xh + h^2}{h}$$

Factor out $h$ from the numerator:

$$f'(x) = \lim_{h \to 0} \frac{h(2x + h)}{h}$$

Divide by $h$ (valid since $h \to 0$ means $h \neq 0$):

$$f'(x) = \lim_{h \to 0} (2x + h)$$

#### 3. Evaluate the limit
Now apply the limit as $h \to 0$:

$$f'(x) = 2x + 0 = 2x$$

---

#### 4. Comparison and Explanation

* **Comparison with the Power Rule:**
  The Power Rule states that $\frac{d}{dx}[x^n] = n x^{n-1}$. For $n = 2$, this gives $\frac{d}{dx}[x^2] = 2x^{2-1} = 2x$. The result from the limit definition matches the Power Rule perfectly.

* **Where the limit is used in the calculation:**
  The limit operation is explicitly evaluated in the very last step when substituting $h = 0$ into the expression $(2x + h)$. Before evaluating the limit, we performed purely algebraic simplification to eliminate $h$ from the denominator, preventing division by zero.
