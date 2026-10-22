## Exercise 15. Classifying Three Systems

### Statement

For each of the following systems, perform only as much elimination as necessary to recognize its type:

## Exercise 15. Classifying Three Systems

### Statement
For each of the following systems, perform only as much elimination as necessary to recognize its type:

* **System 1:** 

  $$
  \begin{cases}
  x + y = 2, \\
  x - y = 0
  \end{cases}
  $$
  
* **System 2:** 

   $$
  \begin{cases}
  x + y = 2, \\
  2x + 2y = 4
  \end{cases}
  $$
  
* **System 3:** 

   $$
  \begin{cases}
  x + y = 2, \\
  2x + 2y = 5
  \end{cases}
  $$

For each, justify the classification: **one solution**, **infinitely many solutions**, or **no solution**.

### Solution

#### System 1

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
1 & -1 & \big| & 0
\end{bmatrix}
\xrightarrow{R_2 \leftarrow R_2 - R_1}
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & -2 & \big| & -2
\end{bmatrix}
$$

* **Classification:** **One solution**
* **Justification:** Pivots exist in every variable column ($x$ and $y$), so there are no free variables and no contradictions. The unique solution is $(x, y) = (1, 1)$.

#### System 2

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
2 & 2 & \big| & 4
\end{bmatrix}
\xrightarrow{R_2 \leftarrow R_2 - 2R_1}
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & 0 & \big| & 0
\end{bmatrix}
$$

* **Classification:** **Infinitely many solutions**
* **Justification:** Row 2 becomes $[0 \quad 0 \mid 0]$, leaving $y$ as a free variable without any contradiction.

#### System 3

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
2 & 2 & \big| & 5
\end{bmatrix}
\xrightarrow{R_2 \leftarrow R_2 - 2R_1}
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & 0 & \big| & 1
\end{bmatrix}
$$

* **Classification:** **No solution**
* **Justification:** Row 2 yields the impossible contradiction $0 = 1$.

For each, justify the classification: one solution, infinitely many solutions, or no solution.

### Solution

#### System 1

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
1 & -1 & \big| & 0
\end{bmatrix}
\xrightarrow{R_2 \leftarrow R_2 - R_1}
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & -2 & \big| & -2
\end{bmatrix}
$$

* **Classification:** **One solution**.
* **Justification:** Pivots exist in every variable column ($x$ and $y$), so no free variables exist and there are no contradictions.

#### System 2

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
2 & 2 & \big| & 4
\end{bmatrix}
\xrightarrow{R_2 \leftarrow R_2 - 2R_1}
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & 0 & \big| & 0
\end{bmatrix}
$$

* **Classification:** **Infinitely many solutions**.
* **Justification:** Row 2 becomes $[0 \quad 0 \mid 0]$, leaving $y$ as a free variable without any contradiction.

#### System 3

$$
\begin{bmatrix}
1 & 1 & \big| & 2 \\
2 & 2 & \big| & 5
\end{bmatrix}
\xrightarrow{R_2 \leftarrow R_2 - 2R_1}
\begin{bmatrix}
1 & 1 & \big| & 2 \\
0 & 0 & \big| & 1
\end{bmatrix}
$$
* **Classification:** **No solution**.
* **Justification:** Row 2 yields the impossible contradiction $0 = 1$.
