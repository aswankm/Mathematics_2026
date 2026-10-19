## Exercise 11. Parameter and Invertibility

### Compute:
For 

$$
A(t) = \begin{pmatrix} 1 & t \\ t & 1 \end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values[cite: 8].

### Solution:

**1. Compute the Determinant:**
$$
\det(A(t)) = (1)(1) - (t)(t) = 1 - t^2
$$

**2. Condition for Invertibility:**
A $2 \times 2$ matrix is invertible if and only if its determinant is non-zero:
$$
1 - t^2 \neq 0 \implies t \neq 1 \text{ and } t \neq -1
$$
* **Result:** The matrix is invertible for all $t \in \mathbb{R}$ except $t = \pm 1$.

**3. Formula for $A(t)^{-1}$:**
Using the standard $2 \times 2$ inverse formula:

$$
A(t)^{-1} = \frac{1}{1 - t^2} \begin{pmatrix} 1 & -t \\ -t & 1 \end{pmatrix}
$$

**4. Behavior at Excluded Values:**
* At $t = 1$ or $t = -1$, the determinant $1 - t^2$ equals zero. 
* This causes division by zero in the inverse formula, reflecting the fact that the matrix loses its inverse and becomes singular.
