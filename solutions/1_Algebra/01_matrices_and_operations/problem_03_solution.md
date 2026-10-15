Exercise 3. When Can Matrices Be Multiplied?[cite: 4]

The matrix sizes are:
$A_{2 \times 3}, \quad B_{3 \times 4}, \quad C_{4 \times 2}, \quad D_{2 \times 2}$[cite: 4]

For the products:
$AB, \ BA, \ BC, \ CB, \ AC, \ CA, \ AD, \ DA$[cite: 4]

Determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition[cite: 4].

---

### **Theory: Dimension Compatibility Condition for Matrix Multiplication**
For a product of two matrices $M \cdot N$ to be defined, the **number of columns in the first matrix ($M$) must equal the number of rows in the second matrix ($N$)**. 
* If $M$ has size $m \times k$ and $N$ has size $k \times n$, the product is defined, and the resulting matrix has the size of the outer dimensions: **$m \times n$**.

---

### **Analysis of Each Product**

#### **1. $AB$**
* **Dimensions:** $A_{2 \times 3}$ and $B_{3 \times 4}$[cite: 4]
* **Check:** The inner dimensions match (columns of $A$ = 3, rows of $B$ = 3).
* **Answer:** **Defined.** Size of the result is **$2 \times 4$**.

#### **2. $BA$**
* **Dimensions:** $B_{3 \times 4}$ and $A_{2 \times 3}$[cite: 4]
* **Check:** The inner dimensions do not match (columns of $B$ = 4 $\neq$ rows of $A$ = 2).
* **Answer:** **Not defined.**

#### **3. $BC$**
* **Dimensions:** $B_{3 \times 4}$ and $C_{4 \times 2}$[cite: 4]
* **Check:** The inner dimensions match (columns of $B$ = 4, rows of $C$ = 4).
* **Answer:** **Defined.** Size of the result is **$3 \times 2$**.

#### **4. $CB$**
* **Dimensions:** $C_{4 \times 2}$ and $B_{3 \times 4}$[cite: 4]
* **Check:** The inner dimensions do not match (columns of $C$ = 2 $\neq$ rows of $B$ = 3).
* **Answer:** **Not defined.**

#### **5. $AC$**
* **Dimensions:** $A_{2 \times 3}$ and $C_{4 \times 2}$[cite: 4]
* **Check:** The inner dimensions do not match (columns of $A$ = 3 $\neq$ rows of $C$ = 4).
* **Answer:** **Not defined.**

#### **6. $CA$**
* **Dimensions:** $C_{4 \times 2}$ and $A_{2 \times 3}$[cite: 4]
* **Check:** The inner dimensions match (columns of $C$ = 2, rows of $A$ = 2).
* **Answer:** **Defined.** Size of the result is **$4 \times 3$**.

#### **7. $AD$**
* **Dimensions:** $A_{2 \times 3}$ and $D_{2 \times 2}$[cite: 4]
* **Check:** The inner dimensions do not match (columns of $A$ = 3 $\neq$ rows of $D$ = 2).
* **Answer:** **Not defined.**

#### **8. $DA$**
* **Dimensions:** $D_{2 \times 2}$ and $A_{2 \times 3}$[cite: 4]
* **Check:** The inner dimensions match (columns of $D$ = 2, rows of $A$ = 2).
* **Answer:** **Defined.** Size of the result is **$2 \times 3$**.
```[cite: 4]
