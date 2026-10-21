## Exercise 11. A Parameter in a System of Three Equations

### Statement
Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x + y + z = 1, \\
x + ty + z = 2, \\
x + y + tz = 3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

### Solution

#### 1. Augmented Matrix Form and Elimination

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 1 \\
1 & t & 1 & \big| & 2 \\
1 & 1 & t & \big| & 3
\end{bmatrix}
$$

Apply $R_2 \leftarrow R_2 - R_1$ and $R_3 \leftarrow R_3 - R_1$:

$$
\begin{bmatrix}
1 & 1 & 1 & \big| & 1 \\
0 & t-1 & 0 & \big| & 1 \\
0 & 0 & t-1 & \big| & 2
\end{bmatrix}
$$

#### 2. Parameter Analysis

* **Case 1: $t = 1$ (Standard step invalid)**
  Substituting $t = 1$ into the reduced matrix gives:

  $$
  \begin{bmatrix}
  1 & 1 & 1 & \big| & 1 \\
  0 & 0 & 0 & \big| & 1 \\
  0 & 0 & 0 & \big| & 2
  \end{bmatrix}
  $$
  
  Rows 2 and 3 yield $0 = 1$ and $0 = 2$, which are impossible contradictions.
  **Result:** **No solution**.

* **Case 2: $t \neq 1$**
  Dividing by $(t - 1) \neq 0$:
  * $y = \frac{1}{t-1}$
  * $z = \frac{2}{t-1}$
  * $x = 1 - y - z = 1 - \frac{3}{t-1} = \frac{t-4}{t-1}$

  **Result:** **Exactly one solution**:
  $$
  (x, y, z) = \left( \frac{t - 4}{t - 1},\, \frac{1}{t - 1},\, \frac{2}{t - 1} \right)
  $$
