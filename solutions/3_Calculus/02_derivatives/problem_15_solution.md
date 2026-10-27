## Problem 15. The Difference Quotient as a Check of the Derivative

### Statement

Choose one function from the problem set and a point $x_0$ at which the derivative exists. Compute $f'(x_0)$ exactly, and then calculate

$$\frac{f(x_0 + h) - f(x_0)}{h}$$

for $h = 1, 0.1$, and $0.01$. Compare the values with $f'(x_0)$ and explain why the difference quotient approaching a single number is consistent with the definition of the derivative, while a few computations do not replace a limit argument.

* **Why this problem:** It connects the definition of the derivative with concrete calculations and teaches the distinction between observation and proof.

---

### Solution (Demonstrated using $f(x) = x^2$ at $x_0 = 1$)

#### 1. Compute the exact derivative $f'(x_0)$
* Given $f(x) = x^2$, the derivative rule gives $f'(x) = 2x$.
* Evaluating at $x_0 = 1$:
  $$f'(1) = 2(1) = 2$$

#### 2. Calculate the difference quotient for $h = 1, 0.1,$ and $0.01$
Using the formula $\frac{f(1 + h) - f(1)}{h}$:
* For $f(x) = x^2$, the difference quotient simplifies algebraically to:
  $$\frac{(1 + h)^2 - 1^2}{h} = \frac{1 + 2h + h^2 - 1}{h} = \frac{2h + h^2}{h} = 2 + h$$

* **For $h = 1$:**
  $$2 + 1 = 3$$

* **For $h = 0.1$:**
  $$2 + 0.1 = 2.1$$

* **For $h = 0.01$:**
  $$2 + 0.01 = 2.01$$

#### 3. Compare the values with $f'(1)$
As $h$ decreases toward zero ($1 \to 0.1 \to 0.01$), the computed values ($3 \to 2.1 \to 2.01$) steadily approach the exact analytical derivative $f'(1) = 2$.

#### 4. Explanation: Observation versus Proof
* **Consistency with the Definition:** The derivative is formally defined as the limit of the difference quotient as $h \to 0$. Seeing the values close in on $2$ numerically demonstrates this exact concept.
* **Why computations do not replace a limit argument:** Testing a finite number of discrete values for $h$ only provides observations and approximations. It is impossible to test infinitely many numbers manually. A formal limit argument evaluates the behavior across the entire continuous neighborhood as $h$ approaches zero, providing absolute mathematical proof rather than just an empirical observation.
