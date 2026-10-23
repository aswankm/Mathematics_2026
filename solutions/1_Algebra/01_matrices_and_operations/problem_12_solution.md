# Exercise 12. Formula for a Matrix Power

### Statement & Solution Overview

Let:

$$
A = \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix}
$$

---

### 1. Compute Successive Powers ($A^2, A^3, A^4$)

- **$A^2$:**

$$
  A^2 = \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} (1)(1) + (1)(0) & (1)(1) + (1)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{bmatrix} = \begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix}
$$

- **$A^3$ ($A^2 A$):**

$$
  A^3 = \begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} (1)(1) + (2)(0) & (1)(1) + (2)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{bmatrix} = \begin{bmatrix} 1 & 3 \\ 0 & 1 \end{bmatrix}
$$

- **$A^4$ ($A^3 A$):**

$$
  A^4 = \begin{bmatrix} 1 & 3 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} (1)(1) + (3)(0) & (1)(1) + (3)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{bmatrix} = \begin{bmatrix} 1 & 4 \\ 0 & 1 \end{bmatrix}
$$

---

### 2. Formulate Conjecture for $A^n$

- Observing that the top-right entry scales sequentially with the exponent $n$:

$$
  A^n = \begin{bmatrix} 1 & n \\ 0 & 1 \end{bmatrix}
$$

---

### 3. Inductive Step (Multiply by $A$ to show $n+1$)

- Assuming the formula holds for $n$, compute $A^{n+1} = A^n A$:

$$
  A^{n+1} = \begin{bmatrix} 1 & n \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} (1)(1) + (n)(0) & (1)(1) + (n)(1) \\ (0)(1) + (1)(0) & (0)(1) + (1)(1) \end{bmatrix} = \begin{bmatrix} 1 & n+1 \\ 0 & 1 \end{bmatrix}
$$

- **Explanation:** Multiplying the general power matrix $A^n$ by matrix $A$ adds $1$ to the top-right component, successfully preserving the diagonal structure and validating the formula for $n + 1$.
