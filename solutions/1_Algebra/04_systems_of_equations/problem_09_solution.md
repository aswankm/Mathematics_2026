## Exercise 9. A System from a Sum Condition

### Statement
Find numbers $x, y$ satisfying

$$
x + y = 10, \quad 2x + 5y = 32.
$$

Solve the system and explain geometrically why the solution is unique.

### Solution

#### 1. Augmented Matrix Form

$$
\begin{bmatrix}
1 & 1 & \big| & 10 \\
2 & 5 & \big| & 32
\end{bmatrix}
$$

#### 2. Row Elimination
Apply $R_2 \leftarrow R_2 - 2R_1$:

$$
\begin{bmatrix}
1 & 1 & \big| & 10 \\
0 & 3 & \big| & 12
\end{bmatrix}
$$

#### 3. Solving for Variables
* From $R_2$: $3y = 12 \implies y = 4$
* From $R_1$: $x + 4 = 10 \implies x = 6$

**Solution:** $(x, y) = (6, 4)$

#### 4. Geometric Interpretation
* Line 1 ($x + y = 10$) has slope $m_1 = -1$.
* Line 2 ($2x + 5y = 32$) has slope $m_2 = -\frac{2}{5}$.
* Since $m_1 \neq m_2$, the two lines are not parallel and intersect at exactly **one single point**, $(6, 4)$. Thus, the solution is unique.
