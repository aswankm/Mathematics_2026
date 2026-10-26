### Exercise 12. Intersection Line of Two Planes

**Statement:**  
Find a parametric equation of the line that is the intersection of

$$
x + y + z = 3, \quad x - y + z = 1.
$$

Find its direction vector in two ways: from the system of equations and from the cross product of the normal vectors. Compare the results.

> **Why this exercise:** shows the equivalence of the algebraic and geometric approaches to constructing an intersection line.

---

### Solution

#### 1. Algebraic Method: Solving the System of Equations
Given the system of two plane equations:

$$
\begin{cases}
x + y + z = 3 \quad \text{--- (1)} \\
x - y + z = 1 \quad \text{--- (2)}
\end{cases}
$$

Subtract equation (2) from equation (1):

$$
(x + y + z) - (x - y + z) = 3 - 1
$$

$$
2y = 2 \implies y = 1
$$

Now substitute $y = 1$ back into equation (1):

$$
x + 1 + z = 3 \implies x + z = 2 \implies x = 2 - z
$$

Let $z = t$ be the free parameter. Then we obtain the parametric equations of the line:

$$
\begin{cases}
x = 2 - t \\
y = 1 \\
z = t
\end{cases}
\implies (x, y, z) = (2, 1, 0) + t(-1, 0, 1)
$$

From this system, the direction vector is **$\mathbf{v}_{\text{alg}} = (-1, 0, 1)$**.

---

#### 2. Geometric Method: Cross Product of Normal Vectors
Extract the normal vectors from the equations of the two planes:
- Normal vector of $\Pi_1$: $\mathbf{n}_1 = (1, 1, 1)$
- Normal vector of $\Pi_2$: $\mathbf{n}_2 = (1, -1, 1)$

The line of intersection lies in both planes, so its direction vector must be perpendicular to both normal vectors. We compute their cross product:

$$
\mathbf{v}_{\text{geom}} = \mathbf{n}_1 \times \mathbf{n}_2 = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 1 & 1 & 1 \\ 1 & -1 & 1 \end{vmatrix}
$$

$$
\mathbf{v}_{\text{geom}} = \mathbf{i}(1(1) - 1(-1)) - \mathbf{j}(1(1) - 1(1)) + \mathbf{k}(1(-1) - 1(1))
$$

$$
\mathbf{v}_{\text{geom}} = \mathbf{i}(1 + 1) - \mathbf{j}(1 - 1) + \mathbf{k}(-1 - 1) = (2, 0, -2)
$$

---

#### 3. Comparison of Results
Comparing the two direction vectors obtained:
- Algebraic method: $\mathbf{v}_{\text{alg}} = (-1, 0, 1)$
- Geometric method: $\mathbf{v}_{\text{geom}} = (2, 0, -2)$

Notice that:

$$
\mathbf{v}_{\text{geom}} = -2 \cdot \mathbf{v}_{\text{alg}}
$$

Both vectors are scalar multiples of each other, meaning they are parallel and point along the exact same line in space. This demonstrates the equivalence between the algebraic solution of the system of linear equations and the geometric construction using the cross product of normal vectors.
