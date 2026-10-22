
## Exercise 2. Gaussian Elimination — One Solution

### Statement
Solve using Gaussian elimination:

$$
\begin{cases}
x + y + z = 6, \\
2x - y + z = 3, \\
x + 2y - z = 2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

### Solution

#### 1. Augmented Matrix Form

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 6 \\
2 & -1 & 1 & \big| & 3 \\
1 & 2 & -1 & \big| & 2
\end{bmatrix}
$$

#### 2. Row Elimination

**Step 1:** Apply $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 6 \\
0 & -3 & -1 & \big| & -9 \\
0 & 1 & -2 & \big| & -4
\end{bmatrix}
$$

**Step 2:** Swap $R_2 \leftrightarrow R_3$:

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 6 \\
0 & 1 & -2 & \big| & -4 \\
0 & -3 & -1 & \big| & -9
\end{bmatrix}
$$

**Step 3:** Apply $R_3 \leftarrow R_3 + 3R_2$:

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 6 \\
0 & 1 & -2 & \big| & -4 \\
0 & 0 & -7 & \big| & -21
\end{bmatrix}
$$

#### 3. Back-Substitution
* From $R_3$: $-7z = -21 \implies z = 3$
* From $R_2$: $y - 2(3) = -4 \implies y = 2$
* From $R_1$: $x + 2 + 3 = 6 \implies x = 1$

**Solution Vector:** $(x, y, z) = (1, 2, 3)$

#### 4. Consistency Check
* **Equation 1:** $1 + 2 + 3 = 6 \quad (\text{Valid})$
* **Equation 2:** $2(1) - 2 + 3 = 3 \quad (\text{Valid})$
* **Equation 3:** $1 + 2(2) - 3 = 2 \quad (\text{Valid})$
