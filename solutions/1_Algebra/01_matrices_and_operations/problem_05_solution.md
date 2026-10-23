# Exercise 5: Matrix Times Vector

## Statement

Let $A = \begin{bmatrix} 2 & -1 \\ 1 & 3 \end{bmatrix}$ and $x = \begin{bmatrix} 4 \\ 2 \end{bmatrix}$. Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

---

## Theory
* **Matrix-Vector Multiplication:** Multiplying a matrix by a vector can be understood as taking the dot products of the rows of the matrix with the vector, or equivalently, as a linear combination of the columns of the matrix weighted by the entries of the vector.

---

## Solution

### 1. Compute $Ax$
Using the row-vector dot product method:

$$
Ax = \begin{bmatrix} 2 & -1 \\ 1 & 3 \end{bmatrix} \begin{bmatrix} 4 \\ 2 \end{bmatrix} = \begin{bmatrix} (2)(4) + (-1)(2) \\ (1)(4) + (3)(2) \end{bmatrix} = \begin{bmatrix} 8 - 2 \\ 4 + 6 \end{bmatrix} = \begin{bmatrix} 6 \\ 10 \end{bmatrix}
$$

---

### 2. Linear Combination of Columns
Using the columns of $A$ weighted by the entries of $x$:

$$
Ax = 4 \begin{bmatrix} 2 \\ 1 \end{bmatrix} + 2 \begin{bmatrix} -1 \\ 3 \end{bmatrix}
$$

$$= \begin{bmatrix} 8 \\ 4 \end{bmatrix} + \begin{bmatrix} -2 \\ 6 \end{bmatrix} = \begin{bmatrix} 8 - 2 \\ 4 + 6 \end{bmatrix} = \begin{bmatrix} 6 \\ 10 \end{bmatrix}$$
