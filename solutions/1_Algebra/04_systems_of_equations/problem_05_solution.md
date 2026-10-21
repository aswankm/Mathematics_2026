## Exercise 5. Row Echelon Form and Number of Solutions

### Statement
For the augmented matrix

$$
\begin{bmatrix}
1 & 2 & -1 & \big| & 3 \\
0 & 1 & 2 & \big| & 1 \\
0 & 0 & 0 & \big| & 0
\end{bmatrix}
$$
determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

### Solution

#### 1. Analysis of Pivots and Free Variables
* **Pivots:** Located in Column 1 ($x$) and Column 2 ($y$).
* **Free Variables:** Column 3 ($z$) has no pivot, so **$z$ is a free variable**.
* **Explanation:** The number of free variables equals total variables minus number of pivots ($3 - 2 = 1$). Thus, **1 variable** can be chosen freely.

#### 2. Number of Solutions
Because there is 1 free variable, the system has **infinitely many solutions**.

#### 3. Parametric Solution Form
Let $z = t$ where $t \in \mathbb{R}$:

* From Row 2: $y + 2t = 1 \implies y = 1 - 2t$
* From Row 1: $x + 2(1 - 2t) - t = 3 \implies x = 1 + 5t$

**Solution Vector:**
$$
(x, y, z) = (1 + 5t,\, 1 - 2t,\, t) \quad \text{where } t \in \mathbb{R}
$$
