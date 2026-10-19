## Exercise 2. Determinant of a 3x3 Matrix

### Compute:
$$
For the matrix  
A = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 3 & 4 \\ 2 & 1 & 5 \end{pmatrix}
compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant[cite: 7].
$$
### Solution:

**1. Computation using Sarrus' Rule:**

$$
\det(A) = [(1 \cdot 3 \cdot 5) + (2 \cdot 4 \cdot 2) + (-1 \cdot 0 \cdot 1)] - [(2 \cdot 3 \cdot -1) + (1 \cdot 4 \cdot 1) + (5 \cdot 0 \cdot 2)]
$$

$$
\det(A) = [15 + 16 + 0] - [-6 + 4 + 0] = 31 - (-2) = 33
$$

**2. Check via Cofactor Expansion along Row 1:**

$$
\det(A) = 1 \begin{vmatrix} 3 & 4 \\ 1 & 5 \end{vmatrix} - 2 \begin{vmatrix} 0 & 4 \\ 2 & 5 \end{vmatrix} + (-1) \begin{vmatrix} 0 & 3 \\ 2 & 1 \end{vmatrix}
$$

$$
\det(A) = 1(15 - 4) - 2(0 - 8) - 1(0 - 6)
$$

$$
\det(A) = 11 + 16 + 6 = 33
$$

* **Conclusion:** Both methods yield **$33$**, confirming the result is correct.
