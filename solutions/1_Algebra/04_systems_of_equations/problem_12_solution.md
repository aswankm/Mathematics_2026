## Exercise 12. Homogeneous System

### Statement
Solve:
$$
\begin{cases}
x + 2y - z = 0, \\
2x + 4y - 2z = 0, \\
x - y + 2z = 0.
\end{cases}
$$
Give all solutions in parametric form and explain why $(0, 0, 0)$ always satisfies a homogeneous system.

### Solution

#### 1. Augmented Matrix Form
$$
\begin{bmatrix}
1 & 2 & -1 & \big| & 0 \\
2 & 4 & -2 & \big| & 0 \\
1 & -1 & 2 & \big| & 0
\end{bmatrix}
$$

#### 2. Row Elimination

**Step 1:** Apply $R_2 \leftarrow R_2 - 2R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{bmatrix}
1 & 2 & -1 & \big| & 0 \\
0 & 0 & 0 & \big| & 0 \\
0 & -3 & 3 & \big| & 0
\end{bmatrix}
$$

**Step 2:** Swap $R_2 \leftrightarrow R_3$:

$$
\begin{bmatrix}
1 & 2 & -1 & \big| & 0 \\
0 & -3 & 3 & \big| & 0 \\
0 & 0 & 0 & \big| & 0
\end{bmatrix}
$$

**Step 3:** Apply $R_2 \leftarrow -\frac{1}{3}R_2$:

$$
\begin{bmatrix}
1 & 2 & -1 & \big| & 0 \\
0 & 1 & -1 & \big| & 0 \\
0 & 0 & 0 & \big| & 0
\end{bmatrix}
$$

#### 3. Parametric Solution
* **Free Variable:** $z = t$ where $t \in \mathbb{R}$.
* From Row 2: $y - t = 0 \implies y = t$.
* From Row 1: $x + 2(t) - t = 0 \implies x = -t$.

**Solution Vector:**
$$
(x, y, z) = (-t,\, t,\, t) = t(-1,\, 1,\, 1) \quad \text{where } t \in \mathbb{R}
$$

#### 4. Why $(0, 0, 0)$ Always Satisfies a Homogeneous System
A homogeneous system has the form $Ax = \mathbf{0}$. Replacing the variable vector $x$ with the zero vector $\mathbf{0}$ results in $A\mathbf{0} = \mathbf{0}$ because every matrix entry multiplied by $0$ sums to $0$. Thus, $(0, 0, 0)$ (the trivial solution) always satisfies every homogeneous system.
