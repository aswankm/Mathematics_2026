## Exercise 8. Two Systems with the Same Coefficient Matrix

### Statement
Solve by elimination the two systems:
$$
\begin{cases}
2x + y = 5, \\
x - y = 1,
\end{cases}
\quad \text{and} \quad
\begin{cases}
2x + y = 1, \\
x - y = 4.
\end{cases}
$$
Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

### Solution

#### 1. Joint Augmented Matrix Elimination
$$
\left[\begin{array}{cc|c|c}
2 & 1 & 5 & 1 \\
1 & -1 & 1 & 4
\end{array}\right]
$$

**Step 1:** Swap $R_1 \leftrightarrow R_2$:
$$
\left[\begin{array}{cc|c|c}
1 & -1 & 1 & 4 \\
2 & 1 & 5 & 1
\end{array}\right]
$$

**Step 2:** Apply $R_2 \leftarrow R_2 - 2R_1$:
$$
\left[\begin{array}{cc|c|c}
1 & -1 & 1 & 4 \\
0 & 3 & 3 & -7
\end{array}\right]
$$

**Step 3:** Apply $R_2 \leftarrow \frac{1}{3}R_2$:
$$
\left[\begin{array}{cc|c|c}
1 & -1 & 1 & 4 \\
0 & 1 & 1 & -\frac{7}{3}
\end{array}\right]
$$

#### 2. Final Solutions
* **System 1:** $y = 1 \implies x - 1 = 1 \implies x = 2$.
  * Solution: $(x, y) = (2, 1)$

* **System 2:** $y = -\frac{7}{3} \implies x + \frac{7}{3} = 4 \implies x = \frac{5}{3}$.
  * Solution: $(x, y) = \left(\frac{5}{3}, -\frac{7}{3}\right)$

#### 3. Comparison
* **Identical Part:** All row operations performed on the $2 \times 2$ coefficient matrix $A$.
* **Reason:** The sequence of pivot choices and row multipliers is strictly determined by the coefficient matrix $A$. The right-hand side vectors $b_1$ and $b_2$ only passively track these operations.
