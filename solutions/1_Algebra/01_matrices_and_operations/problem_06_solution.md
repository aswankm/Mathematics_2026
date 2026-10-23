# Verification of Transpose Property: $(AB)^T = B^T A^T$

## Given Matrices
Let:

$$
A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}, \quad B = \begin{bmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{bmatrix}
$$

---

## Step-by-Step Proof

### 1. Compute Transposes $A^T$ and $B^T$

$$
A^T = \begin{bmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{bmatrix}, \quad B^T = \begin{bmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \end{bmatrix}
$$

### 2. Compute Matrix Product $AB$

$$
AB = \begin{bmatrix} (1)(1)+(2)(2)+(3)(-1) & (1)(0)+(2)(1)+(3)(3) \\ (4)(1)+(5)(2)+(6)(-1) & (4)(0)+(5)(1)+(6)(3) \end{bmatrix}
$$

$$
AB = \begin{bmatrix} 1 + 4 - 3 & 0 + 2 + 9 \\ 4 + 10 - 6 & 0 + 5 + 18 \end{bmatrix}
$$

$$
AB = \begin{bmatrix} 2 & 11 \\ 8 & 23 \end{bmatrix}
$$

### 3. Compute Transpose of Product $(AB)^T$

$$
(AB)^T = \begin{bmatrix} 2 & 8 \\ 11 & 23 \end{bmatrix}
$$

### 4. Compute Product of Transposed Factors $B^T A^T$

$$
B^T A^T = \begin{bmatrix} (1)(1)+(2)(2)+(-1)(3) & (1)(4)+(2)(5)+(-1)(6) \\ (0)(1)+(1)(2)+(3)(3) & (0)(4)+(1)(5)+(3)(6) \end{bmatrix}
$$

$$
B^T A^T = \begin{bmatrix} 1 + 4 - 3 & 4 + 10 - 6 \\ 0 + 2 + 9 & 0 + 5 + 18 \end{bmatrix}
$$

$$B^T A^T = \begin{bmatrix} 2 & 8 \\ 11 & 23 \end{bmatrix}$$

### 5. Final Verification
Since $(AB)^T$ equals $B^T A^T$ (both resulting in $\begin{bmatrix} 2 & 8 \\ 11 & 23 \end{bmatrix}$), the property is verified:
$$(AB)^T = B^T A^T$$
