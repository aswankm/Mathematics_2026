## Exercise 15. Two Methods for Solving the Same System

### Compute:
For 

$$
A = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix}, \quad b = \begin{pmatrix} 7 \\ 8 \end{pmatrix}
$$

solve $Ax = b$ in two ways[cite: 6]:
1. using $A^{-1}$[cite: 6],
2. using Gaussian elimination[cite: 6].

Compare both solutions, the number of essential steps, and state which method was simpler in this example[cite: 6].

### Solution:

**1. Method 1: Using $A^{-1}$**
* Calculate $A^{-1}$ ($\det(A) = 5$):
  
$$
A^{-1} = \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix}
$$

* Solve $x = A^{-1}b$:
  
$$
x = \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \end{pmatrix} \begin{pmatrix} 7 \\ 8 \end{pmatrix} = \frac{1}{5} \begin{pmatrix} 13 \\ 9 \end{pmatrix} = \begin{pmatrix} 2.6 \\ 1.8 \end{pmatrix}
$$

**2. Method 2: Using Gaussian Elimination**
* Augmented matrix $[A \mid b]$ and row reduction:
  
$$
\left(\begin{array}{cc|c} 1 & 3 & 8 \\ 0 & -5 & -9 \end{array}\right)
$$

* Back-substitution yields:
  
$$
x_2 = 1.8, \quad x_1 = 2.6 \implies x = \begin{pmatrix} 2.6 \\ 1.8 \end{pmatrix}
$$

**3. Comparison:**
* Both methods produce identical results[cite: 6]. 
* **Gaussian elimination** is simpler and more efficient here since it avoids intermediate fraction arithmetic required when computing $A^{-1}$[cite: 6].
