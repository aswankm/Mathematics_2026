## Exercise 3. Swapping Two Rows

### Compute:
For 

$$
A = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 3 & 1 \\ 2 & 1 & 1 \end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$. First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

### Solution:

**1. Compute $\det A$:**

$$
\det(A) = (1 \cdot 3 \cdot 1) + (2 \cdot 1 \cdot 2) + (0 \cdot 0 \cdot 1) - [(2 \cdot 3 \cdot 0) + (1 \cdot 1 \cdot 1) + (1 \cdot 0 \cdot 2)]
$$

$$
\det(A) = (3 + 4 + 0) - (0 + 1 + 0) = 7 - 1 = 6
$$

**2. Form Matrix $B$ and Predict $\det B$:**

Matrix $B$ is formed by swapping rows 1 and 2 of $A$:

$$
B = \begin{pmatrix} 0 & 3 & 1 \\ 1 & 2 & 0 \\ 2 & 1 & 1 \end{pmatrix}
$$

* **Prediction:** By the row-swap property, swapping any two rows multiplies the determinant by $-1$. Therefore, $\det(B) = -\det(A) = -6$.

**3. Verify Prediction by Calculation:**

$$
\det(B) = 0 \begin{vmatrix} 2 & 0 \\ 1 & 1 \end{vmatrix} - 3 \begin{vmatrix} 1 & 0 \\ 2 & 1 \end{vmatrix} + 1 \begin{vmatrix} 1 & 2 \\ 2 & 1 \end{vmatrix}
$$

$$
\det(B) = 0 - 3(1 - 0) + 1(1 - 4) = -3 - 3 = -6
$$

* **Conclusion:** The calculated determinant matches the prediction ($\det(B) = -6$).
