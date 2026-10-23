# Exercise 9. Composing Transformations

### Statement & Solution Overview

Let:

$$
S = \begin{bmatrix} 2 & 0 \\ 0 & 1 \end{bmatrix}, \quad 
R = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}, \quad 
x = \begin{bmatrix} 1 \\ 2 \end{bmatrix}
$$

---

### 1. Compute $RSx$ (Scale first, then rotate)

* **Step A ($Sx$):**

$$
  Sx = \begin{bmatrix} 2 & 0 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 \\ 2 \end{bmatrix} = \begin{bmatrix} (2)(1) + (0)(2) \\ (0)(1) + (1)(2) \end{bmatrix} = \begin{bmatrix} 2 \\ 2 \end{bmatrix}
$$

* **Step B ($RSx$):**

$$
  RSx = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 2 \\ 2 \end{bmatrix} = \begin{bmatrix} (0)(2) + (-1)(2) \\ (1)(2) + (0)(2) \end{bmatrix} = \begin{bmatrix} -2 \\ 2 \end{bmatrix}
$$

---

### 2. Compute $SRx$ (Rotate first, then scale)

* **Step A ($Rx$):**

$$
  Rx = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 1 \\ 2 \end{bmatrix} = \begin{bmatrix} (0)(1) + (-1)(2) \\ (1)(1) + (0)(2) \end{bmatrix} = \begin{bmatrix} -2 \\ 1 \end{bmatrix}
$$

* **Step B ($SRx$):**

$$
  SRx = \begin{bmatrix} 2 & 0 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} -2 \\ 1 \end{bmatrix} = \begin{bmatrix} (2)(-2) + (0)(1) \\ (0)(-2) + (1)(1) \end{bmatrix} = \begin{bmatrix} -4 \\ 1 \end{bmatrix}
$$

---

### 3. Comparison and Geometric Explanation

$$
  RSx$ yields $\begin{bmatrix} -2 \\ 2 \end{bmatrix}$, while $SRx$ yields $\begin{bmatrix} -4 \\ 1 \end{bmatrix}$.
$$
* **Geometric Explanation:** Scaling an object first along the coordinate axes alters its dimensions relative to the original frame before it gets rotated. Conversely, rotating it first changes its spatial orientation before the scaling transformation is applied along the standard axes. Because matrix multiplication is non-commutative, the resulting final coordinates depend entirely on the sequence of transformations.
