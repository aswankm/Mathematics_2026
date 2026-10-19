## Exercise 7. Using Properties Instead of Recomputing

### Compute:
Suppose that for a $3 \times 3$ matrix, $\det A = -4$[cite: 14]. Compute:

1. $\det(2A)$
2. $\det(A^T)$
3. $\det(A^{-1})$
4. $\det(3A^{-1})$

### Solution:

**1. For $\det(2A)$:**
Since $A$ is a $3 \times 3$ matrix, scaling the matrix by $2$ scales its determinant by $2^3$:

$$
\det(2A) = 2^3 \cdot \det(A) = 8 \cdot (-4) = -32
$$

**2. For $\det(A^T)$:**
By the transpose property, swapping rows and columns does not change the determinant:

$$
\det(A^T) = \det(A) = -4
$$

**3. For $\det(A^{-1})$:**
The determinant of an inverse matrix is the reciprocal of the original determinant:

$$
\det(A^{-1}) = \frac{1}{\det(A)} = \frac{1}{-4} = -0.25
$$

**4. For $\det(3A^{-1})$:**
Combining the scalar multiple property for a $3 \times 3$ matrix with the inverse property:

$$
\det(3A^{-1}) = 3^3 \cdot \det(A^{-1}) = 27 \cdot \left(-\frac{1}{4}\right) = -\frac{27}{4}
$$
