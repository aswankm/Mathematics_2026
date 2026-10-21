## Exercise 4. Infinitely Many Solutions

### Statement
Solve:
$$
\begin{cases}
x + y + z = 2, \\
2x + 2y + 2z = 4, \\
x - y + z = 0.
\end{cases}
$$
Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

### Solution

#### 1. Augmented Matrix Form
$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 2 \\
2 & 2 & 2 & \big| & 4 \\
1 & -1 & 1 & \big| & 0
\end{bmatrix}
$$

#### 2. Row Elimination

**Step 1:** Apply $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 2 \\
0 & 0 & 0 & \big| & 0 \\
0 & -2 & 0 & \big| & -2
\end{bmatrix}
$$

**Step 2:** Swap $R_2 \leftrightarrow R_3$:

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 2 \\
0 & -2 & 0 & \big| & -2 \\
0 & 0 & 0 & \big| & 0
\end{bmatrix}
$$

**Step 3:** Apply $R_2 \leftarrow -\frac{1}{2} R_2$:

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 2 \\
0 & 1 & 0 & \big| & 1 \\
0 & 0 & 0 & \big| & 0
\end{bmatrix}
$$

#### 3. Free Variable and Parametric Form
* **Free Variable:** $z$ (since column 3 lacks a pivot). Let $z = t$.
* From $R_2$: $y = 1$
* From $R_1$: $x + 1 + t = 2 \implies x = 1 - t$

**Parametric Solution:**
$$
(x, y, z) = (1 - t,\, 1,\, t) \quad \text{where } t \in \mathbb{R}
$$

#### 4. Verification for $t = 2$
Choosing parameter $t = 2$ gives the point $(-1, 1, 2)$:
* **Equation 1:** $-1 + 1 + 2 = 2 \quad (\text{Valid})$
* **Equation 2:** $2(-1) + 2(1) + 2(2) = 4 \quad (\text{Valid})$
* **Equation 3:** $-1 - 1 + 2 = 0 \quad (\text{Valid})$
