### Exercise 7. Classifying a Second-Degree Equation

**Statement:**  
Determine the type of object described by:

1. $4x^2 + 9y^2 = 36$,
2. $x^2 - y^2 = 1$,
3. $x^2 - 4y = 0$,
4. $x^2 + y^2 + 1 = 0$.

In the last case, explain why there are no real points.

> **Why this exercise:** develops quick recognition of the curve type and checking whether real solutions exist.

---

### Solution

#### 1. Classification of Each Equation

##### **Equation 1:** $4x^2 + 9y^2 = 36$
* **Reduction to Canonical Form:** Divide both sides by $36$:

  $$\frac{4x^2}{36} + \frac{9y^2}{36} = 1 \implies \frac{x^2}{9} + \frac{y^2}{4} = 1$$

* **Type of Object:** **Ellipse**
* **Features:** Centered at $(0,0)$ with horizontal semiaxis $a = 3$ and vertical semiaxis $b = 2$.

---

##### **Equation 2:** $x^2 - y^2 = 1$
* **Canonical Form:** $\frac{x^2}{1^2} - \frac{y^2}{1^2} = 1$
* **Type of Object:** **Equilateral (Rectangular) Hyperbola**
* **Features:** Centered at $(0,0)$, opens horizontally along the $x$-axis with vertices at $(\pm 1, 0)$ and asymptotes $y = \pm x$.

---

##### **Equation 3:** $x^2 - 4y = 0$
* **Reduction to Canonical Form:** Rearrange to isolate the squared term:

  $$x^2 = 4y$$

* **Type of Object:** **Parabola**
* **Features:** Vertex at $(0,0)$, opens upwards along the positive $y$-axis with focal parameter $2p = 4 \implies p = 2$ (focus at $(0, 1)$).

---

##### **Equation 4:** $x^2 + y^2 + 1 = 0$
* **Reduction:** Rearrange the terms:

  $$x^2 + y^2 = -1$$

* **Type of Object:** **Empty Set (Imaginary Circle / No Real Points)**

---

#### 2. Explanation of Why Equation 4 Has No Real Points

For any real numbers $x, y \in \mathbb{R}$:
- $x^2 \ge 0$ (the square of a real number is always non-negative),
- $y^2 \ge 0$.

Therefore, the sum of two real squares must also be non-negative:

$$x^2 + y^2 \ge 0$$

However, the equation requires $x^2 + y^2 = -1$. Since a non-negative number cannot equal a negative number ($-1$), there are **no pairs of real coordinates $(x, y)$** that satisfy the equation. Geometrically, this means the equation describes an empty set in the real Cartesian plane $\mathbb{R}^2$.
