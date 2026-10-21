## Exercise 1. From a System to a Matrix

### Statement
Write the system

$$
\begin{cases}
2x - y + z = 4, \\
x + 3y - 2z = 1, \\
3x + y + z = 7.
\end{cases}
$$

in the form $Ax = b$.

Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

### Solution

#### 1. Matrix Equation Form ($Ax = b$)

$$
\begin{bmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix} =
\begin{bmatrix}
4 \\
1 \\
7
\end{bmatrix}
$$

#### 2. Identification of Components
* **Coefficient Matrix ($A$):** 

$$
A = \begin{bmatrix} 2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1 \end{bmatrix}$$

* **Vector of Unknowns ($x$):** 

   $$
  x = \begin{bmatrix} x \\ y \\ z \end{bmatrix}
  $$

* **Right-Hand Side Vector ($b$):** 

   $$
  b = \begin{bmatrix} 4 \\ 1 \\ 7 \end{bmatrix}
  $$

#### 3. Row-to-Equation Correspondence
* **Row 1:** $2(x) - 1(y) + 1(z) = 4
*
  $ corresponds to the first equation: $2x - y + z = 4$.
* **Row 2:** $1(x) + 3(y) - 2(z) = 1
* $ corresponds to the second equation: $x + 3y - 2z = 1$.
* **Row 3:** $3(x) + 1(y) + 1(z) = 7
* $ corresponds to the third equation: $3x + y + z = 7$.
