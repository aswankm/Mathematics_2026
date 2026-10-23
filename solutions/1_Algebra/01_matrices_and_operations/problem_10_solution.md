# Exercise 10. Columns of a Matrix Product

### Statement & Solution Overview

Given:

$$
A = \begin{bmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{bmatrix}, \quad 
B = \begin{bmatrix} 1 & 2 \\ -1 & 0 \\ 3 & 1 \end{bmatrix}
$$

---

### 1. Identify Column Vectors of $B$
Let $b_1$ and $b_2$ be the columns of $B$:

$$
b_1 = \begin{bmatrix} 1 \\ -1 \\ 3 \end{bmatrix}, \quad 
b_2 = \begin{bmatrix} 2 \\ 0 \\ 1 \end{bmatrix}
$$

---

### 2. Compute $Ab_1$

$$
Ab_1 = \begin{bmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{bmatrix} \begin{bmatrix} 1 \\ -1 \\ 3 \end{bmatrix} = \begin{bmatrix} (1)(1) + (2)(-1) + (0)(3) \\ (0)(1) + (1)(-1) + (1)(3) \end{bmatrix} = \begin{bmatrix} 1 - 2 + 0 \\ 0 - 1 + 3 \end{bmatrix} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
$$

---

### 3. Compute $Ab_2$

$$
Ab_2 = \begin{bmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{bmatrix} \begin{bmatrix} 2 \\ 0 \\ 1 \end{bmatrix} = \begin{bmatrix} (1)(2) + (2)(0) + (0)(1) \\ (0)(2) + (1)(0) + (1)(1) \end{bmatrix} = \begin{bmatrix} 2 + 0 + 0 \\ 0 + 0 + 1 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

---

### 4. Compute Matrix $AB$

$$
AB = \begin{bmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{bmatrix} \begin{bmatrix} 1 & 2 \\ -1 & 0 \\ 3 & 1 \end{bmatrix} = \begin{bmatrix} (1)(1) + (2)(-1) + (0)(3) & (1)(2) + (2)(0) + (0)(1) \\ (0)(1) + (1)(-1) + (1)(3) & (0)(2) + (1)(0) + (1)(1) \end{bmatrix} = \begin{bmatrix} -1 & 2 \\ 2 & 1 \end{bmatrix}
$$

---

## 5. Comparison and Explanation
* The first column of $AB$ is $\begin{bmatrix} -1 \\\\ 2 \end{bmatrix}$, which matches $Ab_1$.
* The second column of $AB$ is $\begin{bmatrix} 2 \\\\ 1 \end{bmatrix}$, which matches $Ab_2$.
* **Conclusion:** The columns of the product matrix $AB$ are precisely the matrix-vector products of matrix $A$ with each respective column of matrix $B$, meaning $AB = \begin{bmatrix} Ab_1 & Ab_2 \end{bmatrix}$.
