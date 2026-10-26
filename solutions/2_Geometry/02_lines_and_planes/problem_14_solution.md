### Exercise 14. Contrast: Intersection and Parallelism

**Statement:**  
From the point $P = (0, 0, 1)$, two lines are drawn with direction vectors

$$\mathbf{v}_1 = (2, 1, -1), \quad \mathbf{v}_2 = (2, 1, 0).$$

For each line, analyze its position relative to the plane $z = 0$.

For the line that intersects the plane, find the intersection point. For the other line, explain how you can recognize parallelism without solving an equation.

> **Why this exercise:** compares two very similar data sets that lead to different outcomes and forces recognition of the geometric condition before calculation.

---

### Solution

#### 1. Identify the Normal Vector of the Plane
The plane equation is $z = 0$ (the $xy$-plane), which can be written as $0x + 0y + 1z = 0$.  
Its normal vector is:

$$\mathbf{n} = (0, 0, 1)$$

---

#### 2. Line 1 (with direction vector $\mathbf{v}_1 = (2, 1, -1)$)

1. **Test for Parallelism:**  
   Compute the dot product of $\mathbf{v}_1$ and $\mathbf{n}$:

   $$\mathbf{v}_1 \cdot \mathbf{n} = (2)(0) + (1)(0) + (-1)(1) = -1 \neq 0$$

   Since $\mathbf{v}_1 \cdot \mathbf{n} \neq 0$, the line is **not parallel** to the plane and must **intersect** it at a single point.

2. **Find the Intersection Point:**  
   Parametric equations for Line 1 starting from $P = (0, 0, 1)$:

   $$(x, y, z) = (0, 0, 1) + t(2, 1, -1) = (2t, t, 1 - t)$$

   Set $z = 0$:

   $$1 - t = 0 \implies t = 1$$

   Substitute $t = 1$ back into the parametric equations:
   - $x = 2(1) = 2$
   - $y = 1$
   - $z = 1 - 1 = 0$

   Thus, the intersection point is **$(2, 1, 0)$**.

---

#### 3. Line 2 (with direction vector $\mathbf{v}_2 = (2, 1, 0)$)

1. **Test for Parallelism:**  
   Compute the dot product of $\mathbf{v}_2$ and $\mathbf{n}$:

   $$\mathbf{v}_2 \cdot \mathbf{n} = (2)(0) + (1)(0) + (0)(1) = 0$$

   Since $\mathbf{v}_2 \cdot \mathbf{n} = 0$, Line 2 is **parallel** to the plane $z = 0$.

2. **Check if it lies in the plane:**  
   The starting point $P = (0, 0, 1)$ has $z = 1 \neq 0$, so $P$ does not lie on the plane. Therefore, Line 2 is **strictly parallel** to the plane (no intersection points).

---

#### 4. Explanation: Recognizing Parallelism Without Solving Equations
We can recognize that Line 2 is parallel to the plane $z = 0$ immediately without setting up or solving any algebraic equations by examining its direction vector:

- The plane $z = 0$ consists of all points where the $z$-coordinate is constant ($0$). Any vector parallel to this plane must have a **$z$-component of $0$** (meaning zero change in height).
- Observing $\mathbf{v}_2 = (2, 1, 0)$, its $z$-component is explicitly $0$. This means movement along $\mathbf{v}_2$ maintains a constant $z$-level.
- Since the line starts at $P = (0, 0, 1)$ with $z = 1$, every point along Line 2 will always have $z = 1$, making it impossible to ever reach $z = 0$.
