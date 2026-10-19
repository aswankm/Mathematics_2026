## Exercise 6. Solving a System Using the Inverse

### Compute:
Solve

$$
Ax = b
$$

where

$$
A = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix}, \quad b = \begin{pmatrix} 5 \\ 7 \end{pmatrix}
$$

using $x = A^{-1}b$[cite: 10]. Then substitute the resulting vector back into the equation and check the result[cite: 10].

### Solution:

**1. Calculate $A^{-1}$:**
* Find $\det(A)$:

$$
\det(A) = (2)(3) - (1)(1) = 5
$$

* Apply the $2 \times 2$ inverse formula:

$$
A^{-1} = \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix}
$$

**2. Solve for $x = A^{-1}b$:**

$$
x = \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix} \begin{pmatrix} 5 \\ 7 \end{pmatrix} = \frac{1}{5} \begin{pmatrix} 15 - 7 \\ -5 + 14 \end{pmatrix} = \begin{pmatrix} 1.6 \\ 1.8 \end{pmatrix}
$$

**3. Check via Substitution ($Ax = b$):**

$$
Ax = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix} \begin{pmatrix} 1.6 \\ 1.8 \end{pmatrix} = \begin{pmatrix} 3.2 + 1.8 \\ 1.6 + 5.4 \end{pmatrix} = \begin{pmatrix} 5 \\ 7 \end{pmatrix} = b
$$

* **Conclusion:** The substitution matches $b$, verifying the solution[cite: 10].
