# Exercise 8. Row Operations and Their Reversibility

### Statement & Solution Overview

Given the matrix $A$:

$$
A = \begin{bmatrix} 
1 & 2 & -1 \\\\ 
2 & 4 & 1 \\\\ 
-1 & 1 & 3 
\end{bmatrix}
$$

---

### 1. Initial Matrix

$$
A = \begin{bmatrix} 
1 & 2 & -1 \\\\ 
2 & 4 & 1 \\\\ 
-1 & 1 & 3 
\end{bmatrix}
$$

---

### 2. Step 1 ($R_2 \leftarrow R_2 - 2R_1$)
* **Calculation:** 
 $$
  R_2 - 2R_1 = (2, 4, 1) - 2(1, 2, -1) = (2-2, 4-4, 1 - (-2)) = (0, 0, 3)
$$
* **Matrix after Step 1:**

   $$
  \begin{bmatrix} 
  1 & 2 & -1 \\\\ 
  0 & 0 & 3 \\\\ 
  -1 & 1 & 3 
  \end{bmatrix}
  $$
  
* **Reversing Operation:** $R_2 \leftarrow R_2 + 2R_1$

---

### 3. Step 2 ($R_3 \leftarrow R_3 + R_1$)
* **Calculation:** 

$$
  R_3 + R_1 = (-1, 1, 3) + (1, 2, -1) = (-1+1, 1+2, 3-1) = (0, 3, 2)
$$

* **Matrix after Step 2:**

$$
  \begin{bmatrix} 
  1 & 2 & -1 \\\\ 
  0 & 0 & 3 \\\\ 
  0 & 3 & 2 
  \end{bmatrix}
$$

* **Reversing Operation:** $R_3 \leftarrow R_3 - R_1$

---

### 4. Step 3 (Interchange $R_2$ and $R_3$)
* **Matrix after Step 3:**
  $$
  \begin{bmatrix} 
  1 & 2 & -1 \\\\ 
  0 & 3 & 2 \\\\ 
  0 & 0 & 3 
  \end{bmatrix}
  $$
* **Reversing Operation:** Interchange $R_2$ and $R_3$ again
