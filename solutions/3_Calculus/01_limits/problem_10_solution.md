### Exercise 10. Continuity of a Piecewise Function

**Statement:**  
Find $a$ so that

$$
f(x) = \begin{cases} 
ax + 1, & x < 2 \\ 
x^2 - 1, & x \ge 2 
\end{cases}
$$

is continuous at $x = 2$. Explicitly compare the left-hand limit, right-hand limit, and function value.

> **Why this exercise:** organizes the definition of continuity as agreement among three quantities.

---

### Solution

#### 1. Definition of Continuity at a Point
A function $f(x)$ is continuous at a point $x = c$ if and only if three quantities are equal:
1. The left-hand limit as $x \to c^$: $\lim_{x \to c^-} f(x)$
2. The right-hand limit as $x \to c^+$: $\lim_{x \to c^+} f(x)$
3. The actual function value at the point: $f(c)$

---

#### 2. Evaluating the Three Quantities at $x = 2$

* **Left-Hand Limit ($x \to 2^-$):**  
  For $x < 2$, the function is defined by $f(x) = ax + 1$.  
  
$$
  \lim_{x \to 2^-} f(x) = \lim_{x \to 2^-} (ax + 1) = 2a + 1
$$

* **Right-Hand Limit ($x \to 2^+$):**  
  For $x > 2$, the function is defined by $f(x) = x^2 - 1$.  
  
$$
  \lim_{x \to 2^+} f(x) = \lim_{x \to 2^+} (x^2 - 1) = 2^2 - 1 = 4 - 1 = 3
$$

* **Function Value at $x = 2$ ($f(2)$):**  
  Since the condition $x \ge 2$ includes $x = 2$, we use the second branch $f(x) = x^2 - 1$:
  
$$
  f(2) = 2^2 - 1 = 3
$$

---

#### 3. Solving for $a$
For the function to be continuous at $x = 2$, the left-hand limit must equal the right-hand limit (which also matches the function value):

$$
\lim_{x \to 2^-} f(x) = \lim_{x \to 2^+} f(x)
$$

$$
2a + 1 = 3
$$

Solve for $a$:

$$
2a = 2 \implies a = 1
$$

Thus, the value of $a$ that ensures continuity at $x = 2$ is **$1$**.
