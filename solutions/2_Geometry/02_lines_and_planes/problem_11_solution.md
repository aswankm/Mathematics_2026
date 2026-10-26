### Exercise 11. Plane Containing a Line and a Point[cite: 3]

**Statement:** 
Find the equation of the plane containing[cite: 3]

$$
(x, y, z) = (1, 0, 2) + t(1, 1, -1)
$$

and the point $P = (0, 2, 1)$. Check that both the entire line and the point lie in the plane you obtain.[cite: 3]

> **Why this exercise:** requires independently constructing two linearly independent directions in the plane.[cite: 3]

---

### Solution

#### 1. Identify Components from the Line
From the given parametric equation of the line, we extract:
- A point on the line: $P_0 = (1, 0, 2)$
- The first direction vector lying in the plane: $\mathbf{v}_1 = (1, 1, -1)$
#### 2. Construct a Second Vector in the Plane
We construct a second direction vector $\mathbf{v}_2$ using the point on the line $P_0$ and the given point $P = (0, 2, 1)$[cite: 3]:

$$
\mathbf{v}_2 = \vec{P_0P} = P - P_0 = (0 - 1, 2 - 0, 1 - 2) = (-1, 2, -1)
$$

#### 3. Find the Normal Vector ($\mathbf{n}$) Using the Cross Product
The normal vector to the plane must be orthogonal to both $\mathbf{v}_1$ and $\mathbf{v}_2$:

$$
\mathbf{n} = \mathbf{v}_1 \times \mathbf{v}_2 = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 1 & 1 & -1 \\ -1 & 2 & -1 \end{vmatrix}
$$

$$
\mathbf{n} = \mathbf{i}(1(-1) - (-1)(2)) - \mathbf{j}(1(-1) - (-1)(-1)) + \mathbf{k}(1(2) - 1(-1))
$$

$$
\mathbf{n} = \mathbf{i}(-1 + 2) - \mathbf{j}(-1 - 1) + \mathbf{k}(2 + 1) = (1, 2, 3)
$$

#### 4. Find the Equation of the Plane
Using the normal vector $\mathbf{n} = (1, 2, 3)$ and the point $P_0 = (1, 0, 2)$:

$$
1(x - 1) + 2(y - 0) + 3(z - 2) = 0
$$

$$
x - 1 + 2y + 3z - 6 = 0
$$

Rearranging into standard form gives:

$$
x + 2y + 3z - 7 = 0
$$

#### 5. Verification
1. **Check the point $P = (0, 2, 1)$:**

$$
0 + 2(2) + 3(1) - 7 = 4 + 3 - 7 = 0 \quad (\text{True})
$$

2. **Check the entire line:**
Substitute the parametric expressions of the line $(x = 1 + t, \, y = t, \, z = 2 - t)$ into the plane equation:

$$
(1 + t) + 2(t) + 3(2 - t) - 7 = 1 + t + 2t + 6 - 3t - 7 = (1 + 6 - 7) + (t + 2t - 3t) = 0 \quad (\text{True})
$$
