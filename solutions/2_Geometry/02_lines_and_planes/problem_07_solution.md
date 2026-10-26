### Exercise 7. A Line Relative to a Plane

**Statement:**
For

$$
L: (x, y, z) = (1, 1, 0) + t(1, -1, 0), \quad \Pi: x + y + z = 2
$$

determine whether the line intersects the plane at one point, is parallel to it, or lies in it. Explain the role of the dot product of the direction vector and the normal vector.

> **Why this exercise:** builds a universal test for the relative position of a line and a plane.

---

### Solution

#### 1. Identify the Direction Vector and Normal Vector
- **Direction vector of line $L$:** 

$$
\vec{v} = (1, -1, 0)
$$

- **Normal vector of plane $\Pi$:** 

$$
\vec{n} = (1, 1, 1)
$$

#### 2. Compute the Dot Product ($\vec{v} \cdot \vec{n}$)
To test the orientation between the line and the plane, we compute the dot product of the line's direction vector and the plane's normal vector:

$$
\vec{v} \cdot \vec{n} = (1)(1) + (-1)(1) + (0)(1) = 1 - 1 + 0 = 0
$$

Since $\vec{v} \cdot \vec{n} = 0$, the direction vector $\vec{v}$ is orthogonal to the normal vector $\vec{n}$. Geometrically, this means the line is either strictly parallel to the plane or lies entirely within it.

#### 3. Test a Point from the Line in the Plane Equation
To distinguish whether the line is parallel or lies within the plane, we take a point from the line ($t = 0$) and check if it satisfies the plane's equation:

- **Point from $L$ ($t = 0$):** $P_0 = (1, 1, 0)$
- **Substitute into $\Pi$ ($x + y + z = 2$):**

$$
1 + 1 + 0 = 2 \implies 2 = 2 \quad (\text{True})
$$

Since the point belongs to the plane and the line's direction is parallel to the plane, **the entire line lies in the plane**.

#### 4. Explanation: The Role of the Dot Product
The dot product $\vec{v} \cdot \vec{n}$ serves as a quick test for intersection:
- If $\vec{v} \cdot \vec{n} \neq 0$, the line is not perpendicular to the normal vector, meaning it cuts through the plane at **exactly one unique point**.
- If $\vec{v} \cdot \vec{n} = 0$, the line is parallel to the plane's surface, requiring a secondary point-check to determine whether it floats above the plane (parallel) or is embedded within it (lies in it).
