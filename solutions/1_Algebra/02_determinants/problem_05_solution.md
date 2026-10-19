## Exercise 5. Row Operations

### Compute:
For 

$$
A = \begin{pmatrix} 1 & 2 & 3 \\ 2 & 1 & 0 \\ -1 & 4 & 2 \end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes[cite: 13].

### Solution:

**1. Initial Matrix:**
$$
A = \begin{pmatrix} 1 & 2 & 3 \\ 2 & 1 & 0 \\ -1 & 4 & 2 \end{pmatrix}
$$

**2. Step 1 (Row Replacement):**
Apply $R_2 \to R_2 - 2R_1$ and $R_3 \to R_3 + R_1$:

$$
\begin{pmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \\ 0 & 6 & 5 \end{pmatrix}
$$

* **Effect:** Row replacement operations **do not change** the determinant.

**3. Step 2 (Row Replacement):**
Apply $R_3 \to R_3 + 2R_2$:

$$
\begin{pmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \\ 0 & 0 & -7 \end{pmatrix}
$$

* **Effect:** Row replacement operation **does not change** the determinant.

**4. Step 3 (Calculation):**
Multiply the main diagonal entries of the resulting upper triangular matrix:

$$
\det(A) = (1) \cdot (-3) \cdot (-7) = 21
$$


## Exercise 6. Parameter and Invertibility

### Compute:
For 

$$
A(t) = \begin{pmatrix} t & 1 \\ 2 & t \end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero[cite: 13].

### Solution:

**1. Calculate the Determinant:**

$$
\det(A(t)) = (t)(t) - (1)(2) = t^2 - 2
$$

**2. Condition for Non-Invertibility:**
A matrix is not invertible if and only if its determinant equals zero:

$$
t^2 - 2 = 0 \implies t^2 = 2 \implies t = \pm\sqrt{2}
$$

* **Conclusion:** The matrix $A(t)$ is **not invertible** when $t = \sqrt{2}$ or $t = -\sqrt{2}$ because its determinant evaluates to $0$ at these parameter values[cite: 13]..
