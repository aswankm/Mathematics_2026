## Exercise 12. Finding Inverses Without Starting from Scratch

### Compute:
It is known that

$$
A^{-1} = \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix}
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property[cite: 9].

### Solution:

**1. Compute $(3A)^{-1}$:**
* **Property:** For a scalar $k$, $(kA)^{-1} = \frac{1}{k}A^{-1}$[cite: 9].
* **Calculation:**
  
$$
(3A)^{-1} = \frac{1}{3} \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix} = \begin{pmatrix} \frac{2}{3} & -\frac{1}{3} \\ -1 & \frac{2}{3} \end{pmatrix}
$$

**2. Compute $(A^T)^{-1}$:**
* **Property:** The inverse of a transpose is the transpose of the inverse: $(A^T)^{-1} = (A^{-1})^T$[cite: 9].
* **Calculation:**
  
$$
(A^T)^{-1} = \begin{pmatrix} 2 & -3 \\ -1 & 2 \end{pmatrix}
$$

**3. Compute $(A^2)^{-1}$:**
* **Property:** $(A^2)^{-1} = (A^{-1})^2$[cite: 9].
* **Calculation:**
  
$$
(A^2)^{-1} = \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix} \begin{pmatrix} 2 & -1 \\ -3 & 2 \end{pmatrix} = \begin{pmatrix} 7 & -4 \\ -12 & 7 \end{pmatrix}
$$
