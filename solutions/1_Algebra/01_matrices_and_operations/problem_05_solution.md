## Exercise 5. Matrix Times Vector

### Statement
Let $A = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix}$ and $x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$. Compute $Ax$, then express $Ax$ as a linear combination of the columns of $A$ with coefficients from $x$.
**[cite: 6]

### Theory
* **Linear Combination of Columns:** Matrix-vector multiplication $Ax$ equals a linear combination of the columns of $A$ weighted by the entries of $x$: $x_1 c_1 + x_2 c_2$.
**[cite: 6]

### Essential Steps & Solution
1. **Compute $Ax$:**
   $$Ax = \begin{pmatrix} (2)(4) + (-1)(2) \\ (1)(4) + (3)(2) \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$[cite: 6]
2. **Linear Combination:**
   $$Ax = 4 \begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \end{pmatrix} = \begin{pmatrix} 8 \\ 4 \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$[cite: 6]
