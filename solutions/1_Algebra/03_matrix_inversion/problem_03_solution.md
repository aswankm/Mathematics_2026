## Exercise 3. When Does the Inverse Not Exist?

### Compute:
For 

$$
A = \begin{pmatrix} 2 & 4 \\ 1 & 2 \end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

### Solution:

**1. Explanation Using the Determinant:**
* Calculate the determinant of $A$:
  
$$
\det(A) = (2)(2) - (4)(1) = 4 - 4 = 0
$$

* Since the determinant is $0$, the matrix is singular, and division by zero makes the inverse formula undefined.

**2. Explanation Using Row Dependence:**

$$
* Inspecting the rows: Row 1 is $\begin{pmatrix} 2 & 4 \end{pmatrix}$ and Row 2 is $\begin{pmatrix} 1 & 2 \end{pmatrix}$.
* Row 1 is a direct scalar multiple of Row 2 ($\text{Row } 1 = 2 \cdot \text{Row } 2$). This linear dependence prevents the matrix from being invertible.
$$
