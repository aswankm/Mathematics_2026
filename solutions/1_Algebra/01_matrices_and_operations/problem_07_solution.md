# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Statement
Let $A = \begin{bmatrix} 2 & 1 \\ 0 & 2 \end{bmatrix}$. Compute the powers $A^2$ and $A^3$, and determine the general pattern for $A^k$.

---

## Solution

### 1. Compute $A^2$
Multiply matrix $A$ by itself:

$$
A^2 = A \cdot A = \begin{bmatrix} 2 & 1 \\ 0 & 2 \end{bmatrix} \begin{bmatrix} 2 & 1 \\ 0 & 2 \end{bmatrix}
$$

$$
A^2 = \begin{bmatrix} (2)(2) + (1)(0) & (2)(1) + (1)(2) \\ (0)(2) + (2)(0) & (0)(1) + (2)(2) \end{bmatrix}
$$

$$
A^2 = \begin{bmatrix} 4 & 4 \\ 0 & 4 \end{bmatrix}
$$

---

### 2. Compute $A^3$
Multiply $A^2$ by $A$:

$$
A^3 = A^2 \cdot A = \begin{bmatrix} 4 & 4 \\ 0 & 4 \end{bmatrix} \begin{bmatrix} 2 & 1 \\ 0 & 2 \end{bmatrix}
$$

$$
A^3 = \begin{bmatrix} (4)(2) + (4)(0) & (4)(1) + (4)(2) \\ (0)(2) + (4)(0) & (0)(1) + (4)(2) \end{bmatrix}
$$

$$
A^3 = \begin{bmatrix} 8 & 12 \\ 0 & 8 \end{bmatrix}
$$

---

### 3. General Pattern for $A^k$
Observing the pattern from $A^1$, $A^2$, and $A^3$:
- For $ A^1 = \begin{bmatrix} 2^1 & 1 \cdot 2^0 \\ 0 & 2^1 \end{bmatrix}$
- For $ A^2 = \begin{bmatrix} 2^2 & 2 \cdot 2^1 \\ 0 & 2^2 \end{bmatrix}$
- For $ A^3 = \begin{bmatrix} 2^3 & 3 \cdot 2^2 \\ 0 & 2^3 \end{bmatrix}$

The general formula for any integer $k \ge 1$ is:
$$
A^k = \begin{bmatrix} 2^k & k \cdot 2^{k-1} \\ 0 & 2^k \end{bmatrix}
$$
