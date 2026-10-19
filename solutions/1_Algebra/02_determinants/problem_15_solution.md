## Exercise 15. Combining Determinant Properties

### Compute:
Let $A$ and $B$ be invertible $2 \times 2$ matrices with 

$$
\det A = -2, \quad \det B = 3
$$

Without finding the entries of the matrices, compute 

$$
\det \left( B^{-1} A^T B \right)
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

### Solution:

**1. Apply Determinant Properties in Order:**

* **Multiplicative Property:** $\det(XY) = \det(X)\det(Y)$

$$
\det \left( B^{-1} A^T B \right) = \det(B^{-1}) \cdot \det(A^T) \cdot \det(B)
$$

* **Inverse Property:** $\det(B^{-1}) = \frac{1}{\det(B)}$
* **Transpose Property:** $\det(A^T) = \det(A)$

$$
\det \left( B^{-1} A^T B \right) = \frac{1}{\det(B)} \cdot \det(A) \cdot \det(B)
$$

**2. Why the Factors Involving $B$ Cancel:**
Determinants evaluate to scalar real numbers. Because multiplication of scalars is commutative and associative, $\frac{1}{\det(B)}$ and $\det(B)$ multiply to $1$ (since $\det(B) = 3 \neq 0$):

$$
\det \left( B^{-1} A^T B \right) = \left( \frac{1}{\det(B)} \cdot \det(B) \right) \cdot \det(A) = 1 \cdot \det(A) = \det(A)
$$

**3. Final Result:**

$$
\det \left( B^{-1} A^T B \right) = -2
$$
