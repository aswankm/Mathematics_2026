## Exercise 3. Inconsistent System

### Statement
Solve or show that the system is inconsistent:

$$
begin{cases}
x + 2y = 3, \\
2x + 4y = 7.
\end{cases}
$$
Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

### Solution

#### 1. Augmented Matrix Form

$$
\begin{bmatrix}
1 & 2 & \big| & 3 \\
2 & 4 & \big| & 7
\end{bmatrix}
$$

#### 2. Row Elimination
Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{bmatrix}
1 & 2 & \big| & 3 \\
0 & 0 & \big| & 1
\end{bmatrix}
$$

#### 3. Interpretation of Contradiction
* **Matrix Level:** Row 2 translates to $0x + 0y = 1$, which simplifies to $0 = 1$ (an impossible contradiction).
* **Geometric Level:** The equations represent two distinct parallel lines ($y = -\frac{1}{2}x + \frac{3}{2}$ and $y = -\frac{1}{2}x + \frac{7}{2}$) that never intersect.

**Conclusion:** The system is **inconsistent** (no solution exists).
