## Exercise 2. Formula for a 2x2 Matrix

### Compute:
Find the inverse of

$$
A = \begin{pmatrix} 3 & 2 \\ 5 & 4 \end{pmatrix}
$$

using the formula for a $2 \times 2$ matrix. At the end, check the result by computing one product with $A$.

### Solution:

**1. Calculate the Determinant:**
$$
\det(A) = (3)(4) - (2)(5) = 12 - 10 = 2
$$

**2. Apply the Inverse Formula:**
For a $2 \times 2$ matrix, swap the diagonal elements, negate the off-diagonal elements, and divide by the determinant:

$$
A^{-1} = \frac{1}{2} \begin{pmatrix} 4 & -2 \\ -5 & 3 \end{pmatrix} = \begin{pmatrix} 2 & -1 \\ -2.5 & 1.5 \end{pmatrix}
$$

**3. Check via Product with $A$:**

$$
A A^{-1} = \begin{pmatrix} 3 & 2 \\ 5 & 4 \end{pmatrix} \begin{pmatrix} 2 & -1 \\ -2.5 & 1.5 \end{pmatrix} = \begin{pmatrix} 6 - 5 & -3 + 3 \\ 10 - 10 & -5 + 6 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}
$$

* **Conclusion:** Since $A A^{-1} = I$, the calculated inverse is verified.
