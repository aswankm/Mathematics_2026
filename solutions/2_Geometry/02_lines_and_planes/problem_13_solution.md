### Exercise 13. Closest Point on a Plane

**Statement:**  
Find the point on the plane $x + 2y + 2z = 4$ closest to $P = (3, 0, 0)$. Give the distance and check that the segment joining the two points is perpendicular to the plane.

> **Why this exercise:** combines projection, distance, and the normal direction in one problem.

---

### Solution

#### 1. Find the Closest Point (Orthogonal Projection $Q$)
The normal vector of the plane $\Pi: x + 2y + 2z = 4$ is:

$$
\mathbf{n} = (1, 2, 2)
$$

The line passing through $P = (3, 0, 0)$ perpendicular to the plane has the parametric form:

$$
(x, y, z) = (3 + t, 2t, 2t)
$$

Substitute these parametric equations into the plane equation $x + 2y + 2z = 4$:

$$
(3 + t) + 2(2t) + 2(2t) = 4
$$

$$
3 + t + 4t + 4t = 4 \implies 3 + 9t = 4 \implies 9t = 1 \implies t = \frac{1}{9}
$$

Substitute $t = \frac{1}{9}$ back into the line's parametric equations to get the closest point $Q$:

- $x = 3 + \frac{1}{9} = \frac{28}{9}$
- $y = 2 \left(\frac{1}{9}\right) = \frac{2}{9}$
- $z = 2 \left(\frac{1}{9}\right) = \frac{2}{9}$

Thus, the closest point on the plane is **$Q = \left(\frac{28}{9}, \frac{2}{9}, \frac{2}{9}\right)$**.

---

#### 2. Calculate the Distance
The distance $d$ between $P = (3, 0, 0)$ and $Q = \left(\frac{28}{9}, \frac{2}{9}, \frac{2}{9}\right)$ is:

$$
d = \|\vec{PQ}\| = \sqrt{\left(\frac{28}{9} - 3\right)^2 + \left(\frac{2}{9} - 0\right)^2 + \left(\frac{2}{9} - 0\right)^2}
$$

$$
d = \sqrt{\left(\frac{1}{9}\right)^2 + \left(\frac{2}{9}\right)^2 + \left(\frac{2}{9}\right)^2} = \sqrt{\frac{1 + 4 + 4}{81}} = \sqrt{\frac{9}{81}} = \frac{3}{9} = \frac{1}{3}
$$

Alternatively, using the point-to-plane distance formula:

$$
d = \frac{|1(3) + 2(0) + 2(0) - 4|}{\sqrt{1^2 + 2^2 + 2^2}} = \frac{|3 - 4|}{\sqrt{9}} = \frac{1}{3}
$$

Thus, the distance is **$\frac{1}{3}$**.

---

#### 3. Verification: Check Perpendicularity
The segment vector $\vec{PQ}$ joining the two points is:

$$
\vec{PQ} = Q - P = \left(\frac{28}{9} - 3, \frac{2}{9} - 0, \frac{2}{9} - 0\right) = \left(\frac{1}{9}, \frac{2}{9}, \frac{2}{9}\right) = \frac{1}{9}(1, 2, 2)
$$

Since $\vec{PQ} = \frac{1}{9}\mathbf{n}$, the segment vector is a scalar multiple of the normal vector $\mathbf{n} = (1, 2, 2)$, which proves that the segment joining $P$ and $Q$ is strictly **perpendicular to the plane**.
