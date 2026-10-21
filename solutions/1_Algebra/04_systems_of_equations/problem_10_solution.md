## Exercise 10. A Polynomial Through Three Points

### Statement
Find a polynomial $p(x) = ax^2 + bx + c$ whose graph passes through $(0, 1)$, $(1, 3)$, and $(2, 9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

### Solution

#### 1. System of Equations Formation
Substituting each point $(x, y)$ into $p(x) = ax^2 + bx + c$:
* **$(0, 1)$:** $c = 1$
* **$(1, 3)$:** $a + b + c = 3 \implies a + b = 2$
* **$(2, 9)$:** $4a + 2b + c = 9 \implies 4a + 2b = 8 \implies 2a + b = 4$

#### 2. Augmented Matrix Form and Solution

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
2 & 1 & \big| & 4
\end{bmatrix}
$$

Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & -1 & \big| & 0
\end{bmatrix}
$$

* From $R_2$: $-b = 0 \implies b = 0$
* From $R_1$: $a + 0 = 2 \implies a = 2$
* From initial condition: $c = 1$

**Polynomial:** $p(x) = 2x^2 + 1$

#### 3. Verification
* $p(0) = 2(0)^2 + 1 = 1 \quad (\text{Valid})$
* $p(1) = 2(1)^2 + 1 = 3 \quad (\text{Valid})$
* $p(2) = 2(2)^2 + 1 = 9 \quad (\text{Valid})$
