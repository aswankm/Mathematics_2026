# Exercise 11. When Do Matrices Commute?

### Statement & Solution Overview

Given:

$$
A = \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix}, \quad 
B = \begin{bmatrix} a & b \\ c & d \end{bmatrix}
$$

---

### 1. Compute Product $AB$

$$
AB = \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} a & b \\ c & d \end{bmatrix} = \begin{bmatrix} (1)(a) + (1)(c) & (1)(b) + (1)(d) \\ (0)(a) + (1)(c) & (0)(b) + (1)(d) \end{bmatrix} = \begin{bmatrix} a+c & b+d \\ c & d \end{bmatrix}
$$

---

### 2. Compute Product $BA$

$$
BA = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} (a)(1) + (b)(0) & (a)(1) + (b)(1) \\ (c)(1) + (d)(0) & (c)(1) + (d)(1) \end{bmatrix} = \begin{bmatrix} a & a+b \\ c & c+d \end{bmatrix}
$$

---

### 3. Equate Entries ($AB = BA$)

Equating corresponding entries of $AB$ and $BA$:

- **Top-left:** 

$$
  a + c = a \implies c = 0
$$

- **Top-right:** 

$$
b + d = a + b \implies d = a
$$

- **Bottom-left:** 

$$
c = c \quad \text{(always true)}
$$

- **Bottom-right:** 

$$
d = c + d \implies c = 0 \quad \text{(consistent)}
$$

---

### 4. Conditions and General Form

- **Conditions:** $c = 0$ and $a = d$.
- **General Form of $B$:** Substituting these conditions gives:
  $$
  B = \begin{bmatrix} a & b \\ 0 & a \end{bmatrix}
  $$
