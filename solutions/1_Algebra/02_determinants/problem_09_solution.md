## Exercise 9. Area and the Determinant

### Compute:
The vectors

$$
u = \begin{pmatrix} 3 \\ 1 \end{pmatrix}, \quad v = \begin{pmatrix} 1 \\ 4 \end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area[cite: 15].

### Solution:

**1. Area Computation with $(u, v)$:**

$$
\det \begin{pmatrix} 3 & 1 \\ 1 & 4 \end{pmatrix} = (3)(4) - (1)(1) = 12 - 1 = 11
$$

$$
\text{Area} = |\det| = |11| = 11
$$

**2. Computation with Reversed Order $(v, u)$:**

$$
\det \begin{pmatrix} 1 & 3 \\ 4 & 1 \end{pmatrix} = (1)(1) - (3)(4) = 1 - 12 = -11
$$

$$
\text{Area} = |\det| = |-11| = 11
$$

**3. Explanation:**
* **What changes in the determinant:** The sign of the determinant reverses (from $+11$ to $-11$) because swapping columns negates the determinant value, representing a flip in orientation[cite: 15].
* **What does not change in the area:** The geometric area remains $11$ because area is defined as the absolute value of the determinant ($|\det|$), which is always positive[cite: 15].
