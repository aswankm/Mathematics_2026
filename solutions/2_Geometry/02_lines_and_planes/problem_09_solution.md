### Exercise 9. Distances

**Statement:**[cite: 2]  
Compute:[cite: 2]

1. the distance from $P = (2, 3)$ to the line $3x + 4y - 10 = 0$,[cite: 2]
2. the distance from $Q = (2, -1, 3)$ to the plane $2x - 2y + z - 4 = 0$.[cite: 2]

Compare the two formulas and explain their common connection with the normal direction.[cite: 2]

> **Why this exercise:** organizes two similar formulas through one geometric idea.[cite: 2]

---

### Solution

#### 1. Distance from Point $P$ to the Line
The formula for the distance $d$ from a 2D point $(x_0, y_0)$ to a line $Ax + By + C = 0$ is:

$$
d = \frac{|Ax_0 + By_0 + C|}{\sqrt{A^2 + B^2}}
$$

For point $P = (2, 3)$ and line $3x + 4y - 10 = 0$:
- $A = 3, B = 4, C = -10$
- $x_0 = 2, y_0 = 3$

$$
d_1 = \frac{|3(2) + 4(3) - 10|}{\sqrt{3^2 + 4^2}} = \frac{|6 + 12 - 10|}{\sqrt{9 + 16}} = \frac{|8|}{\sqrt{25}} = \frac{8}{5}
$$

Thus, the distance from $P$ to the line is **$\frac{8}{5}$** (or $1.6$).

---

#### 2. Distance from Point $Q$ to the Plane
The formula for the distance $d$ from a 3D point $(x_0, y_0, z_0)$ to a plane $Ax + By + Cz + D = 0$ is:

$$
d = \frac{|Ax_0 + By_0 + Cz_0 + D|}{\sqrt{A^2 + B^2 + C^2}}
$$

For point $Q = (2, -1, 3)$ and plane $2x - 2y + z - 4 = 0$:
- $A = 2, B = -2, C = 1, D = -4$
- $x_0 = 2, y_0 = -1, z_0 = 3$

$$
d_2 = \frac{|2(2) + (-2)(-1) + 1(3) - 4|}{\sqrt{2^2 + (-2)^2 + 1^2}} = \frac{|4 + 2 + 3 - 4|}{\sqrt{4 + 4 + 1}} = \frac{|5|}{\sqrt{9}} = \frac{5}{3}
$$

Thus, the distance from $Q$ to the plane is **$\frac{5}{3}$**.

---

#### 3. Comparison of Formulas and Connection to the Normal Direction

Both distance formulas follow the exact same structural template:

$$
d = \frac{|\text{Evaluate line/plane equation at the given point}|}{\|\mathbf{n}\|}
$$

**Geometric Connection:**
- In both cases, the coefficient vector $\mathbf{n}$—which is $\mathbf{n} = (A, B)$ in 2D and $\mathbf{n} = (A, B, C)$ in 3D—represents the **normal vector** (a vector perpendicular to the line or plane).
- The shortest distance from a point to a geometric object (line or plane) is always measured along the direction perpendicular to that object (the normal direction).
- Evaluating $Ax_0 + By_0 (+ Cz_0) + D$ computes the scalar projection of the displacement vector onto the normal direction $\mathbf{n}$, and dividing by $\|\mathbf{n}\|$ normalizes this value so that it measures the true perpendicular Euclidean distance.
