## Problem 14. A Piecewise-Defined Function

**Statement:**
Let 

$$f(x) = \begin{cases} x + 1, & -1 \leq x < 1, \\ 2, & 1 \leq x \leq 3. \end{cases}$$

Sketch the graph, decide where to split the integral, compute 

$$\int_{-1}^{3} f(x) \, dx$$

and verify the result geometrically.

> **Why this problem:** it requires understanding the definition of the function before carrying out the calculation.

---

### Solution

#### 1. Splitting the Integral
Because the function $f(x)$ changes its definition at $x = 1$, we must split the domain of integration $[-1, 3]$ into two sub-intervals: $[-1, 1]$ and $[1, 3]$. 

$$\int_{-1}^{3} f(x) \, dx = \int_{-1}^{1} (x + 1) \, dx + \int_{1}^{3} 2 \, dx$$

#### 2. Compute the Integrals
* **First Sub-integral on $[-1, 1]$:**
  $$\int_{-1}^{1} (x + 1) \, dx = \left[ \frac{x^2}{2} + x \right]_{-1}^{1}$$
  $$= \left( \frac{1^2}{2} + 1 \right) - \left( \frac{(-1)^2}{2} + (-1) \right)$$
  $$= \left( \frac{1}{2} + 1 \right) - \left( \frac{1}{2} - 1 \right) = \frac{3}{2} - \left( -\frac{1}{2} \right) = \frac{3}{2} + \frac{1}{2} = 2$$

* **Second Sub-integral on $[1, 3]$:**
  $$\int_{1}^{3} 2 \, dx = \left[ 2x \right]_{1}^{3} = 2(3) - 2(1) = 6 - 2 = 4$$

* **Total Definite Integral:**
  $$\int_{-1}^{3} f(x) \, dx = 2 + 4 = 6$$

#### 3. Geometric Verification
We can find the total area under the graph by dividing the region into two geometric shapes above the $x$-axis:
* **Region 1 (on $[-1, 1]$):** Forms a trapezoid (or a triangle and a rectangle). 
  * At $x = -1$, height is $-1 + 1 = 0$. At $x = 1$, height is $1 + 1 = 2$.
  * Area = $\frac{\text{base}_1 + \text{base}_2}{2} \times \text{width} = \frac{0 + 2}{2} \times 2 = 2$.
* **Region 2 (on $[1, 3]$):** Forms a rectangle with a width of $3 - 1 = 2$ and a height of $2$.
  * Area = $\text{width} \times \text{height} = 2 \times 2 = 4$.

Summing the geometric areas:
$$\text{Total Area} = 2 + 4 = 6$$

This matches our calculated integral value.
