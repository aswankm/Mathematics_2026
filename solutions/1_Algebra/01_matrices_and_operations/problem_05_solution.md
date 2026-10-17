## Exercise 5. Matrix Times Vector

**Statement:**
Let 
$$A = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix}, \quad x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}.$$
Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

---

## Solution

### 1. Compute $Ax$
To compute the matrix-vector product $Ax$, we take the dot product of each row of matrix $A$ with vector $x$:

$$Ax = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix} \begin{pmatrix} 4 \\ 2 \end{pmatrix} = \begin{pmatrix} (2)(4) + (-1)(2) \\ (1)(4) + (3)(2) \end{pmatrix}$$

$$= \begin{pmatrix} 8 - 2 \\ 4 + 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$

### 2. Express $Ax$ as a Linear Combination of the Columns of $A$
A matrix-vector product can be viewed as a linear combination of the columns of $A$, where the weights are the entries of vector 
$$x = \begin{pmatrix} x_1 \\ x_2 \end{pmatrix} = \begin{pmatrix} 4 \\ 2 \end{pmatrix}:$$

$$Ax = x_1 \mathbf{a}_1 + x_2 \mathbf{a}_2$$

Substituting the columns of $A$ and entries of $x$:

$$Ax = 4 \begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \end{pmatrix}$$

Checking the calculation:

$$= \begin{pmatrix} 4 \times 2 \\ 4 \times 1 \end{pmatrix} + \begin{pmatrix} 2 \times (-1) \\ 2 \times 3 \end{pmatrix}$$

$$= \begin{pmatrix} 8 \\ 4 \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$
