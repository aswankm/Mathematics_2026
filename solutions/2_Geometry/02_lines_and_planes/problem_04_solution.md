### Exercise 4. Plane Through Three Points

**Statement:**
Find the equation of the plane through 

$$
A = (1, 0, 0), \quad B = (0, 1, 0), \quad C = (0, 0, 1).
$$

First construct two vectors lying in the plane, and then use the cross product. Check the resulting equation on all three points.

---

### Solution

#### 1. Construct Two Vectors in the Plane
We construct two vectors lying within the plane using the given points:

$$
\vec{u} = \vec{AB} = B - A = (0 - 1, 1 - 0, 0 - 0) = (-1, 1, 0)
$$

$$
\vec{v} = \vec{AC} = C - A = (0 - 1, 0 - 0, 1 - 0) = (-1, 0, 1)
$$

#### 2. Find the Normal Vector ($\vec{n}$) Using the Cross Product
The normal vector to the plane is orthogonal to both $\vec{u}$ and $\vec{v}$, so we calculate their cross product:

$$
\vec{n} = \vec{u} \times \vec{v} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ -1 & 1 & 0 \\ -1 & 0 & 1 \end{vmatrix}
$$

$$
\vec{n} = \mathbf{i}(1 \cdot 1 - 0 \cdot 0) - \mathbf{j}((-1) \cdot 1 - 0 \cdot (-1)) + \mathbf{k}((-1) \cdot 0 - 1 \cdot (-1))
$$

$$
\vec{n} = (1, 1, 1)
$$

#### 3. General Equation of the Plane
Using the normal vector $\vec{n} = (1, 1, 1)$ and point $A = (1, 0, 0)$:

$$
1(x - 1) + 1(y - 0) + 1(z - 0) = 0
$$

$$
x - 1 + y + z = 0
$$

Rearranging into standard form gives:

$$
x + y + z - 1 = 0
$$

*(Or equivalently, $x + y + z = 1$)*

#### 4. Verification
Let's check if all three points satisfy the equation $x + y + z - 1 = 0$:

- **For point $A = (1, 0, 0)$:**

$$
1 + 0 + 0 - 1 = 0 \quad (\text{True})
$$

- **For point $B = (0, 1, 0)$:**

$$
0 + 1 + 0 - 1 = 0 \quad (\text{True})
$$

- **For point $C = (0, 0, 1)$:**

$$
0 + 0 + 1 - 1 = 0 \quad (\text{True})
$$
