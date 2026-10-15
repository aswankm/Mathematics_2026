# Linear Algebra Exercises

## Exercise 5. Matrix Times Vector

### Problem Statement
Let
$$A = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix}, \quad x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

### Solution
* **Computed Product ($Ax$):** $\begin{pmatrix} 6 \\ 10 \end{pmatrix}$
* **Linear Combination Form:** $4 \begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$

---

## Exercise 6. Transpose

### Problem Statement
For $A = \begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{pmatrix}$ and $B = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix}$, compute $A^T$, $B^T$, and $AB$. Verify that $(AB)^T = B^T A^T$.

### Solution
1. **Transposes:**
   $$A^T = \begin{pmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{pmatrix}, \quad B^T = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \end{pmatrix}$$
2. **Product and Transpose:**
   $$AB = \begin{pmatrix} 2 & 11 \\ 8 & 23 \end{pmatrix} \implies (AB)^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}$$
3. **Verification:**
   $$B^T A^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}$$
   Thus, $(AB)^T = B^T A^T$ holds true.
