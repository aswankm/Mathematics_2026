### Exercise 5. Relative Position of Two Lines[cite: 1]

**Statement:**[  
Analyze the position of:

$$
L_1: (x, y, z) = (1, 1, 0) + t(1, 2, 1)
$$

$$
L_2: (x, y, z) = (2, 0, 1) + s(0, 1, -1)
$$

If they intersect, give the intersection point. If not, determine whether they are parallel or skew. Justify the classification.
> **Why this exercise:** teaches how to distinguish qualitatively different relationships between lines in space.

---

### Solution

#### 1. Identify the Direction Vectors
We extract the direction vectors for both lines from their parametric forms:

$$
\vec{v}_1 = (1, 2, 1)
$$

$$
\vec{v}_2 = (0, 1, -1)
$$

#### 2. Check for Parallelism
Two lines are parallel if their direction vectors are scalar multiples of each other ($\vec{v}_1 = k \vec{v}_2$ for some scalar $k$):

$$
(1, 2, 1) = k(0, 1, -1) \implies \begin{cases} 1 = 0 \cdot k \\ 2 = 1 \cdot k \\ 1 = -1 \cdot k \end{cases}
$$

Since $1 = 0$ is impossible, there is no scalar $k$ that satisfies this system. Thus, **the lines are not parallel**.

#### 3. Check for Intersection
Equate the corresponding components of $L_1$ and $L_2$ to form a system of equations:

1. **$x$-component:**

$$
1 + t = 2 \implies t = 1
$$

2. **$y$-component:**

$$
1 + 2t = s
$$

Substitute $t = 1$:

$$
s = 1 + 2(1) = 3
$$

3. **$z$-component (Consistency Check):**

Substitute $t = 1$ into $L_1$'s $z$-component:

$$
z = 0 + 1(1) = 1
$$

Substitute $s = 3$ into $L_2$'s $z$-component:

$$
z = 1 - 1(3) = -2
$$

Since $1 \neq -2$, the system of equations has no solution, meaning **the lines do not intersect**.

#### 4. Conclusion
Because the lines $L_1$ and $L_2$ are neither parallel nor intersecting, they are **skew lines**.
