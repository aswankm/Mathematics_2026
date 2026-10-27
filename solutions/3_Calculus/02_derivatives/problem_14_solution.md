## Problem 14. Continuity and Differentiability of a Piecewise Function

### Statement

Investigate the behavior at $x = 0$ of

$$f(x) = \begin{cases} x^2, & x \ge 0, \\ ax, & x < 0. \end{cases}$$

For which values of $a$ is the function continuous? For which values do the one-sided derivatives exist and agree? For which value of $a$ is the function differentiable? Explain why continuity alone is not sufficient.

* **Why this problem:** It requires an organized argument and a clear distinction between two concepts.

---

### Solution

#### 1. Investigate Continuity at $x = 0$
A function is continuous at $x = 0$ if the limit from the left equals the limit from the right and equals the function value:
* **Right-hand limit:** 
  $$\lim_{x \to 0^+} f(x) = \lim_{x \to 0^+} x^2 = 0$$
* **Left-hand limit:** 
  $$\lim_{x \to 0^-} f(x) = \lim_{x \to 0^-} (ax) = a(0) = 0$$
* **Function value:** 
  $$f(0) = 0^2 = 0$$

Since the left-hand limit, right-hand limit, and function value all evaluate to $0$ regardless of the value of $a$, the function is **continuous for all real values of $a$**.

---

#### 2. Investigate One-Sided Derivatives at $x = 0$
Compute the limit definition of the derivative from both sides:
* **Right-hand derivative ($x > 0$):**
  $$\lim_{h \to 0^+} \frac{f(0 + h) - f(0)}{h} = \lim_{h \to 0^+} \frac{h^2 - 0}{h} = \lim_{h \to 0^+} h = 0$$

* **Left-hand derivative ($x < 0$):**
  $$\lim_{h \to 0^-} \frac{f(0 + h) - f(0)}{h} = \lim_{h \to 0^-} \frac{a(h) - 0}{h} = \lim_{h \to 0^-} a = a$$

For the one-sided derivatives to exist and agree, the left-hand derivative must equal the right-hand derivative:
$$a = 0$$

---

#### 3. Determine Differentiability
A function is differentiable at $x = 0$ if and only if its left-hand derivative and right-hand derivative both exist and are equal. 
* Based on the one-sided derivatives, this condition is satisfied **only when $a = 0$**.

---

#### 4. Why Continuity Alone Is Not Sufficient
* Continuity guarantees that the graph of the function has no gaps, jumps, or breaks at $x = 0$, meaning it can be drawn without lifting the pen.
* However, a continuous function can still possess a sharp corner, cusp, or vertical tangent at a point (where the left-hand slope abruptly differs from the right-hand slope). 
* Differentiability requires the stricter condition that the transition is smooth, meaning the instantaneous rates of change from both sides match precisely.
