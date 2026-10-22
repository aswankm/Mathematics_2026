## Exercise 13. Does Every Equation Add New Information?

### Statement
Consider the system

$$
x_1 + x_2 = 10, \quad x_2 + x_3 = 8, \quad x_1 - x_3 = 2.
$$
Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

### Solution

#### 1. Augmented Matrix Form and Elimination

$$
\begin{bmatrix}
1 & 1 & 0 & \big| & 10 \\
0 & 1 & 1 & \big| & 8 \\
1 & 0 & -1 & \big| & 2
\end{bmatrix}
$$

**Step 1:** Apply $R_3 \leftarrow R_3 - R_1$:

$$
\begin{bmatrix}
1 & 1 & 0 & \big| & 10 \\
0 & 1 & 1 & \big| & 8 \\
0 & -1 & -1 & \big| & -8
\end{bmatrix}
$$

**Step 2:** Apply $R_3 \leftarrow R_3 + R_2$:

$$
\begin{bmatrix}
1 & 1 & 0 & \big| & 10 \\
0 & 1 & 1 & \big| & 8 \\
0 & 0 & 0 & \big| & 0
\end{bmatrix}
$$

#### 2. Solution Set
* **Free Variable:** $x_3 = t$ where $t \in \mathbb{R}$.
* From Row 2: $x_2 = 8 - t$
* From Row 1: $x_1 = 10 - x_2 = 10 - (8 - t) = 2 + t$

**Solution Vector:**

$$
(x_1, x_2, x_3) = (2 + t,\, 8 - t,\, t) \quad \text{where } t \in \mathbb{R}
$$

#### 3. Redundancy Proof
Not all three equations are independently necessary. Equation 3 ($x_1 - x_3 = 2$) directly follows from subtracting Equation 2 from Equation 1:

$$
(x_1 + x_2) - (x_2 + x_3) = 10 - 8 \implies x_1 - x_3 = 2
$$

Therefore, Equation 3 adds no new restrictions/information to the system.
