### Exercise 7. Limit at a Point and Canceling a Factor

**Statement:**  
Compute

$$
\lim_{x \to 3} \frac{x^2 - 4x + 3}{x - 3}.
$$

Explain why the value of the function at $x = 3$ is not needed to compute the limit.

> **Why this exercise:** separates the concept of a limit from the value of a function at a point.

---

### Solution

#### 1. Computation of the Limit
Directly substituting $x = 3$ into the expression yields:

$$
\frac{3^2 - 4(3) + 3}{3 - 3} = \frac{9 - 12 + 3}{0} = \frac{0}{0}
$$

This results in the indeterminate form $\frac{0}{0}$. To evaluate the limit, factor the numerator:

$$
x^2 - 4x + 3 = (x - 1)(x - 3)
$$

Substitute the factored form back into the limit expression:

$$
\lim_{x \to 3} \frac{(x - 1)(x - 3)}{x - 3}
$$

Since $x \to 3$, we consider values of $x$ arbitrarily close to $3$ but $x \neq 3$. Therefore, we can safely cancel the common factor $(x - 3)$:

$$
= \lim_{x \to 3} (x - 1) = 3 - 1 = 2
$$

---

#### 2. Why the Value of the Function at $x = 3$ Is Not Needed
* **Definition of a Limit:** A limit describes the behavior of a function as the independent variable gets closer and closer to a target value, but it **never evaluates the function at the target value itself**. 
* **Undefined Function Value:** In this specific function, $f(x) = \frac{x^2 - 4x + 3}{x - 3}$, the function is strictly undefined at $x = 3$ because division by zero occurs. 
* **Conclusion:** Because limits depend entirely on values *near* $3$ rather than *at* $3$, the hole or undefined nature of the function at $x = 3$ does not prevent us from finding the limit. Algebraic simplification reveals the consistent value that the function approaches as $x$ approaches $3$, which is $2$.
