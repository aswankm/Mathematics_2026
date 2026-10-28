## Problem 12. Symmetry, Sign, and Absolute Value

**Statement:**
Compare 

$$\int_{-2}^{2} x \, dx$$

and

$$\int_{-2}^{2} |x| \, dx.$$

Before calculating, predict the results from symmetry and a sketch, then carry out the calculation and explain the difference.

> **Why this problem:** it teaches how to use symmetry and geometry before applying a computational procedure.

---

### Solution

#### 1. Prediction from Symmetry and Geometry

* **For $\int_{-2}^{2} x \, dx$:**
  * The integrand $f(x) = x$ is an **odd function** ($f(-x) = -f(x)$).
  * Its graph is symmetric about the origin. Over a symmetric interval $[-2, 2]$, the area below the $x$-axis on $[-2, 0]$ exactly cancels out the area above the $x$-axis on $[0, 2]$.
  * **Prediction:** The integral will equal **$0$**.

* **For $\int_{-2}^{2} |x| \, dx$:**
  * The integrand $g(x) = |x|$ is an **even function** ($g(-x) = g(x)$).
  * Its graph is symmetric about the $y$-axis and lies entirely on or above the $x$-axis (V-shape).
  * The integral represents the total geometric area of two identical triangles (one on $[-2, 0]$ and one on $[0, 2]$), each with base $2$ and height $2$.
  * **Prediction:** The integral will equal $2 \times \left( \frac{1}{2} \times 2 \times 2 \right) = \mathbf{4}$.

---

#### 2. Carry Out the Calculations

* **Integral 1: $\int_{-2}^{2} x \, dx$**
  $$\int_{-2}^{2} x \, dx = \left[ \frac{x^2}{2} \right]_{-2}^{2} = \frac{2^2}{2} - \frac{(-2)^2}{2} = \frac{4}{2} - \frac{4}{2} = 0$$

* **Integral 2: $\int_{-2}^{2} |x| \, dx$**
  Split the integral at $x = 0$ where the absolute value function changes definition ($|x| = -x$ for $x < 0$ and $|x| = x$ for $x \geq 0$):
  $$\int_{-2}^{2} |x| \, dx = \int_{-2}^{0} (-x) \, dx + \int_{0}^{2} x \, dx$$
  $$= \left[ -\frac{x^2}{2} \right]_{-2}^{0} + \left[ \frac{x^2}{2} \right]_{0}^{2}$$
  $$= \left( 0 - \left( -\frac{(-2)^2}{2} \right) \right) + \left( \frac{2^2}{2} - 0 \right)$$
  $$= \left( 0 - (-2) \right) + (2) = 2 + 2 = 4$$

---

#### 3. Explanation of the Difference

* **$\int_{-2}^{2} x \, dx = 0$** measures the **net signed area** (accumulated change). The negative accumulation on $[-2, 0]$ cancels out the positive accumulation on $[0, 2]$.
* **$\int_{-2}^{2} |x| \, dx = 4$** measures the **total geometric area** between the curve and the $x$-axis. Taking the absolute value flips the negative region above the $x$-axis so that both halves contribute positively to the total sum.
