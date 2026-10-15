Given:
A = 
[ 2  -1   3]
[ 0   4   5]

B = 
[ 1   0]
[-2   3]
[ 4   1]

---

### **1. State the sizes of matrices A and B.**

* **Theory:** 
  The size (or dimension) of a matrix is expressed as $m \times n$, where $m$ represents the number of rows and $n$ represents the number of columns.
* **Steps:**
  1. Count the number of horizontal rows in matrix $A$ (there are 2 rows) and vertical columns (there are 3 columns).
  2. Count the number of horizontal rows in matrix $B$ (there are 3 rows) and vertical columns (there are 2 columns).
* **Answer:**
  * Matrix $A$ is of size $2 \times 3$.
  * Matrix $B$ is of size $3 \times 2$.

---

### **2. Read off the entries a12, a23, b21, and b32.**

* **Theory:** 
  An individual entry in a matrix is denoted by $a_{ij}$, where $i$ represents the row index and $j$ represents the column index.
* **Steps:**
  * For $a_{12}$, look at matrix $A$, row 1, column 2.
  * For $a_{23}$, look at matrix $A$, row 2, column 3.
  * For $b_{21}$, look at matrix $B$, row 2, column 1.
  * For $b_{32}$, look at matrix $B$, row 3, column 2.
* **Answer:**
  * $a_{12} = -1$
  * $a_{23} = 5$
  * $b_{21} = -2$
  * $b_{32} = 1$

---

### **3. Write the second row of A and the first column of B as vectors.**

* **Theory:** 
  A row or column extracted from a matrix can be represented as a row vector or a column vector containing those specific ordered elements.
* **Steps:**
  * Locate the second row of matrix $A$: elements are $0, 4, 5$.
  * Locate the first column of matrix $B$: elements are $1, -2, 4$.
* **Answer:**
  * Second row of $A$ as a vector: $[0, 4, 5]$
  * First column of $B$ as a vector: $[1, -2, 4]^T$ (or $\begin{pmatrix} 1 \\ -2 \\ 4 \end{pmatrix}$)
