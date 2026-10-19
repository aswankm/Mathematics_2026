## Exercise 9. Matrix Equation

### Compute:
Given 

$$
A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}, \quad B = \begin{pmatrix} 3 & 1 \\ 2 & 4 \end{pmatrix}
$$

Solve the equation $AX = B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$[cite: 9].

### Solution:

**1. Placement of $A^{-1}$:**

$$
Since $A$ is on the left of $X$ in the expression $AX = B$, we must apply $A^{-1}$ from the **left** on both sides:
A^{-1}(AX) = A^{-1}B \implies X = A^{-1}B
$$

**2. Compute $A^{-1}$:**
Using the $2 \times 2$ inverse formula ($\det(A) = 1$):

$$
A^{-1} = \begin{pmatrix} 1 & -2 \\ 0 & 1 \end{pmatrix}
$$

**3. Compute $X = A^{-1}B$:**

$$
X = \begin{pmatrix} 1 & -2 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 3 & 1 \\ 2 & 4 \end{pmatrix} = \begin{pmatrix} 3 - 4 & 1 - 8 \\ 0 + 2 & 0 + 4 \end{pmatrix} = \begin{pmatrix} -1 & -7 \\ 2 & 4 \end{pmatrix}
$$

**4. Check via $AX$:**

$$
AX = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} -1 & -7 \\ 2 & 4 \end{pmatrix} = \begin{pmatrix} -1 + 4 & -7 + 8 \\ 0 + 2 & 0 + 4 \end{pmatrix} = \begin{pmatrix} 3 & 1 \\ 2 & 4 \end{pmatrix} = B
$$

* **Conclusion:** The computed matrix $X = \begin{pmatrix} -1 & -7 \\ 2 & 4 \end{pmatrix}$ correctly satisfies $AX = B$[cite: 9].
