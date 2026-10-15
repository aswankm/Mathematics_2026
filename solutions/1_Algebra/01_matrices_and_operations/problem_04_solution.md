Exercise 4. Matrix Multiplication and Noncommutativity[cite: 5]

For:
A = 
[ 1   2]
[ 0   1]

B = 
[ 2   0]
[ 3   1]

Compute AB and BA. Is AB = BA? Use this example to explain what noncommutativity of matrix multiplication means[cite: 5].

---

### **1. Compute $AB$**

* **Theory:** 
  Matrix multiplication of two matrices $A$ (size $m \times k$) and $B$ (size $k \times n$) produces a matrix $C$ of size $m \times n$, where each entry $c_{ij}$ is calculated by taking the dot product of the $i$-th row of $A$ and the $j$-th column of $B$.
* **Steps:**
  * Entry $(1,1)$: $(1 \times 2) + (2 \times 3) = 2 + 6 = 8$
  * Entry $(1,2)$: $(1 \times 0) + (2 \times 1) = 0 + 2 = 2$
  * Entry $(2,1)$: $(0 \times 2) + (1 \times 3) = 0 + 3 = 3$
  * Entry $(2,2)$: $(0 \times 0) + (1 \times 1) = 0 + 1 = 1$
* **Answer:**
  $$AB = \begin{pmatrix} 8 & 2 \\ 3 & 1 \end{pmatrix}$$

---

### **2. Compute $BA$**

* **Theory:** 
  Similarly, compute the product $BA$ by taking the dot products of the rows of $B$ and the columns of $A$.
* **Steps:**
  * Entry $(1,1)$: $(2 \times 1) + (0 \times 0) = 2 + 0 = 2$
  * Entry $(1,2)$: $(2 \times 2) + (0 \times 1) = 4 + 0 = 4$
  * Entry $(2,1)$: $(3 \times 1) + (1 \times 0) = 3 + 0 = 3$
  * Entry $(2,2)$: $(3 \times 2) + (1 \times 1) = 6 + 1 = 7$
* **Answer:**
  $$BA = \begin{pmatrix} 2 & 4 \\ 3 & 7 \end{pmatrix}$$

---

### **3. Is $AB = BA$?**

* **Answer:** 
  No, $AB \neq BA$ because $\begin{pmatrix} 8 & 2 \\ 3 & 1 \end{pmatrix} \neq \begin{pmatrix} 2 & 4 \\ 3 & 7 \end{pmatrix}$[cite: 5].

---

### **4. Explanation of Noncommutativity**

* **Theory & Explanation:**
  In standard real number arithmetic, multiplication is **commutative**, meaning that the order of multiplication does not change the result (e.g., $2 \times 3 = 3 \times 2$). 
  
  As demonstrated by this example, **matrix multiplication is non-commutative** in general[cite: 5]. This means that for two matrices $A$ and $B$, even when both products $AB$ and $BA$ are defined and result in matrices of the same dimensions, **$AB$ is not necessarily equal to $BA$**[cite: 5]. The order in which matrices are multiplied fundamentally alters the final product.
```[cite: 5]
