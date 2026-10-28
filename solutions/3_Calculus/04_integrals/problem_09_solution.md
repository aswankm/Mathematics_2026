## Problem 9. Definite Integral and Geometric Area

**Statement:**
Compute 

$$\int_{-1}^{2} x \, dx$$

Then separately compute the areas of the parts of the graph below and above the $x$-axis and explain the difference between the definite integral and geometric area.

> **Why this problem:** it clarifies the difference between signed accumulation and area.

---

### Solution

#### 1. Compute the Definite Integral
Using the Fundamental Theorem of Calculus:
$$\int_{-1}^{2} x \, dx = \left[ \frac{x^2}{2} \right]_{-1}^{2}$$
$$= \left( \frac{2^2}{2} \right) - \left( \frac{(-1)^2}{2} \right)$$
$$= \frac{4}{2} - \frac{1}{2} = 2 - 0.5 = 1.5$$

#### 2. Compute the Areas Separately (Below and Above the $x$-axis)
The function $f(x) = x$ crosses the $x$-axis at $x = 0$. This splits our interval $[-1, 2]$ into two regions:
* **Region 1 (Below the $x$-axis on $[-1, 0]$):**
  * Forms a triangle with a base of $1$ and a height of $1$.
  * Area = $\frac{1}{2} \times \text{base} \times \text{height} = \frac{1}{2}(1)(1) = 0.5$.
  * Because this region is below the $x$-axis, its contribution to the definite integral is negative: $-0.5$.

* **Region 2 (Above the $x$-axis on $[0, 2]$):**
  * Forms a triangle with a base of $2$ and a height of $2$.
  * Area = $\frac{1}{2} \times \text{base} \times \text{height} = \frac{1}{2}(2)(2) = 2$.
  * Because this region is above the $x$-axis, its contribution to the definite integral is positive: $+2$.

#### 3. Total Geometric Area vs. Definite Integral
* **Total Geometric Area:** Represents the total physical space between the curve and the $x$-axis, where all areas are treated as positive quantities.
  $$\text{Total Area} = 0.5 + 2 = 2.5$$

* **Definite Integral:** Represents the *signed* accumulation of area, meaning areas below the $x$-axis are subtracted and areas above the $x$-axis are added.
  $$\text{Definite Integral} = -0.5 + 2 = 1.5$$
