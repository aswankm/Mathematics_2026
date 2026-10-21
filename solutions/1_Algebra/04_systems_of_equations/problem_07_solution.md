## Exercise 6. A System with a Parameter — Which Cases Actually Occur?

### Statement
Analyze, depending on the parameter $a$, the system:

$$
\begin{cases}
x + y = 2, \\
ax + ay = 4.
\end{cases}
$$

Among the three possibilities — **exactly one solution**, **infinitely many solutions**, **no solution** — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

### Solution

#### 1. Augmented Matrix Form and Reduction
$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
a & a & \big| & 4
\end{bmatrix}
$$

Apply $R_2 \leftarrow R_2 - aR_1$:

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & 0 & \big| & 4 - 2a
\end{bmatrix}
$$

#### 2. Analysis of Cases

* **Infinitely Many Solutions ($a = 2$):**
  When $a = 2$, $4 - 2a = 0$, making Row 2 $[0 \quad 0 \mid 0]$. This leaves $y$ as a free variable ($y = t$), giving solutions $(x, y) = (2 - t, t)$.

* **No Solution ($a \neq 2$):**
  When $a \neq 2$, $4 - 2a \neq 0$, resulting in $0x + 0y = \text{non-zero}$, which is a contradiction ($0 = \text{non-zero}$).

* **Exactly One Solution (Impossible):**
  This case **cannot occur** for any value of $a$. The coefficient matrix has identical rows up to scaling ($[a, a] = a[1, 1]$), meaning the determinant is always $0$ and the columns are linearly dependent. Geometrically, the lines are always parallel, so they can never intersect at a single point.
