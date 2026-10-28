## Problem 6. Average Value of a Function

Compute the average value of the function

$$f(x) = x^2$$

on the interval $[0, 3]$.

Find a point $c \in [0, 3]$ for which $f(c)$ is equal to this average value, and interpret the result geometrically.

> Why this problem: it gives the integral the interpretation of an average value and connects the numerical result with a level of the function on the graph.

---

### Solution

#### 1. Average Value Calculation
The average value $f_{\text{avg}}$ of a continuous function $f(x)$ on an interval $[a, b]$ is given by the formula:

$$f_{\text{avg}} = \frac{1}{b - a} \int_{a}^{b} f(x) \, dx$$

For $f(x) = x^2$ on the interval $[0, 3]$:
$$f_{\text{avg}} = \frac{1}{3 - 0} \int_{0}^{3} x^2 \, dx$$

Evaluating the integral:
$$\int_{0}^{3} x^2 \, dx = \left[ \frac{x^3}{3} \right]_{0}^{3} = \frac{3^3}{3} - 0 = \frac{27}{3} = 9$$

Multiplying by $\frac{1}{3}$:
$$f_{\text{avg}} = \frac{1}{3} \cdot 9 = 3$$

Thus, the average value of the function is **$3$**.

---

#### 2. Finding the Point $c$
We need to find a point $c \in [0, 3]$ such that $f(c) = f_{\text{avg}}$:
$$f(c) = c^2 = 3$$

Solving for $c$:
$$c = \pm\sqrt{3}$$

Since the interval is $[0, 3]$, we take the positive root:
$$c = \sqrt{3} \approx 1.732$$

---

#### 3. Geometric Interpretation
According to the **Mean Value Theorem for Integrals**, for a continuous function, there exists at least one number $c$ in the interval such that the function value at $c$ equals the average value. 

Geometrically, this means that the area under the curve $y = x^2$ from $x = 0$ to $x = 3$ is exactly equal to the area of a rectangle with a width of $3$ (the length of the interval) and a height of $3$ (the average value $f(c)$), giving a total area of $3 \times 3 = 9$.
