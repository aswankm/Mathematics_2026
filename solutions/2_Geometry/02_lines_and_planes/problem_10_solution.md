### Exercise 10. Projection of a Point onto a Plane[cite: 2]

**Statement:**[cite: 2]  
Find the orthogonal projection of $P = (2, 1, 3)$ onto the plane $x + y + z = 3$, and then find the reflection of $P$ across this plane. Check that the midpoint of the segment joining the point and its reflection lies on the plane.[cite: 2]

> **Why this exercise:** combines the normal, intersection, and distance into the construction of a projection and reflection.[cite: 2]

---

### Solution

#### 1. Construct a Line Through $P$ Perpendicular to the Plane
The normal vector of the plane $\Pi: x + y + z = 3$ is:
$$
\mathbf{n} = (1, 1, 1)
$$

The line $L$ passing through $P = (2, 1, 3)$ with direction vector $\mathbf{n}$ has the parametric form:
$$
(x, y, z) = (2, 1, 3) + t(1, 1, 1) = (2 + t, 1 + t, 3 + t)
$$

#### 2. Find the Orthogonal Projection ($P'$)
Substitute the parametric expressions into the plane equation $x + y + z = 3$:
$$
(2 + t) + (1 + t) + (3 + t) = 3
$$
$$
6 + 3t = 3 \implies 3t = -3 \implies t = -1
$$

Substitute $t = -1$ back into the line's parametric equations:
- $x = 2 + (-1) = 1$
- $y = 1 + (-1) = 0$
- $z = 3 + (-1) = 2$

Thus, the orthogonal projection is **$P' = (1, 0, 2)$**.

#### 3. Find the Reflection ($P''$) Across the Plane
Let $P''$ be the reflection of $P$ across the plane. The projection $P'$ acts as the midpoint between $P$ and $P''$:
$$
P' = \frac{P + P''}{2} \implies P'' = 2P' - P
$$

$$
P'' = 2(1, 0, 2) - (2, 1, 3) = (2, 0, 4) - (2, 1, 3) = (0, -1, 1)
$$

Thus, the reflection of $P$ is **$P'' = (0, -1, 1)$**.

#### 4. Verification
We check that the midpoint of the segment joining $P$ and $P''$ lies on the plane:
$$
\text{Midpoint} = \frac{P + P''}{2} = \frac{(2, 1, 3) + (0, -1, 1)}{2} = \frac{(2, 0, 4)}{2} = (1, 0, 2)
$$

Substitute the midpoint into the plane equation $x + y + z = 3$:
$$
1 + 0 + 2 = 3 \quad (\text{True})
$$
