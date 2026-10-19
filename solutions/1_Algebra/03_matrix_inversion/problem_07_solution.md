## Exercise 7. Inverse of a Product

### Compute:
For 

$$
A = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}, \quad B = \begin{pmatrix} 2 & 0 \\ 0 & 3 \end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order[cite: 9].

### Solution:

**1. Compute $(AB)^{-1}$:**
* Find the product $AB$:
  
$$
AB = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 2 & 0 \\ 0 & 3 \end{pmatrix} = \begin{pmatrix} 2 & 3 \\ 0 & 3 \end{pmatrix}
$$

* Find the inverse of $AB$ ($\det(AB) = 6$):
  
$$
(AB)^{-1} = \frac{1}{6} \begin{pmatrix} 3 & -3 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} 0.5 & -0.5 \\ 0 & \frac{1}{3} \end{pmatrix}
$$

**2. Compute $B^{-1}A^{-1}$:**
* Find individual inverses:
  
$$
A^{-1} = \begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix}, \quad B^{-1} = \begin{pmatrix} 0.5 & 0 \\ 0 & \frac{1}{3} \end{pmatrix}
$$

* Multiply $B^{-1}A^{-1}$:
  
$$
B^{-1}A^{-1} = \begin{pmatrix} 0.5 & 0 \\ 0 & \frac{1}{3} \end{pmatrix} \begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 0.5 & -0.5 \\ 0 & \frac{1}{3} \end{pmatrix}
$$

**3. Verification & Interpretation:**
* The results match: $(AB)^{-1} = B^{-1}A^{-1}$[cite: 9].
* **Meaning of reversed order:** When reversing a sequence of linear transformations, you must undo the final action first, requiring the order of inverse operations to be flipped[cite: 9].
