# Exercise 5. Matrix Times Vector

### Statement
Let $A = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix}$ and $x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$. Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

### Theory
* **Matrix-Vector Multiplication:** Multiplying a matrix by a vector can be understood as taking the dot products of the rows of the matrix with the vector, or equivalently, as a linear combination of the columns of the matrix weighted by the entries of the vector.

### Essential Steps & Solution
1. **Compute $Ax$:**
   $$Ax = \begin{pmatrix} (2)(4) + (-1)(2) \\ (1)(4) + (3)(2) \end{pmatrix} = \begin{pmatrix} 8 - 2 \\ 4 + 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$

2. **Express as a linear combination:**
   $$Ax = 4 \begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \end{pmatrix} = \begin{pmatrix} 8 \\ 4 \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$
