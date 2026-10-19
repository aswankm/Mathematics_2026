## Exercise 8. Determinant of a Product

### Compute:
Let $A, B$ be square matrices such that $\det A = 3$ and $\det B = -5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB \neq BA$[cite: 15].

### Solution:

**1. Compute $\det(AB)$:**
Using the multiplicative property of determinants:

$$
\det(AB) = \det(A) \cdot \det(B) = (3) \cdot (-5) = -15
$$

**2. Compute $\det(BA)$:**

$$
\det(BA) = \det(B) \cdot \det(A) = (-5) \cdot (3) = -15
$$

**3. Why $\det(AB) = \det(BA)$ despite $AB \neq BA$:**
* Determinants compute to scalar numbers. Because scalar multiplication is commutative ($xy = yx$), $\det(A)\det(B) = \det(B)\det(A)$ holds true, even though matrix multiplication itself is not commutative ($AB \neq BA$).

**4. Compute $\det(A^{-1}B)$:**
Using the inverse and multiplicative properties:

$$
\det(A^{-1}B) = \det(A^{-1}) \cdot \det(B) = \frac{1}{\det(A)} \cdot \det(B) = \left(\frac{1}{3}\right) \cdot (-5) = -\frac{5}{3}
$$
