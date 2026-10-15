# Exercise 5: Matrix Times Vector

## 📌 Problem Statement

Given the matrix

\[
A = \begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}
\]

and the vector

\[
x = \begin{pmatrix}
4 \\
2
\end{pmatrix}
\]

**Tasks:**
1. Compute the matrix-vector product \(Ax\).
2. Express \(Ax\) as a linear combination of the columns of \(A\), using the entries of \(x\) as coefficients.

---

## 📚 Theory

### Matrix-Vector Multiplication

Matrix-vector multiplication is performed by multiplying each row of the matrix by the corresponding entries of the vector and adding the results.

If \(A\) has columns \(c_1\) and \(c_2\), and

\[
x = \begin{pmatrix}x_1\\x_2\end{pmatrix},
\]

then the product can be expressed as:

\[
\boxed{Ax = x_1c_1+x_2c_2}
\]

This means that multiplying a matrix by a vector is equivalent to taking a linear combination of the matrix's columns, weighted by the entries of the vector.

---

## ✏️ Solution

### Step 1: Compute \(Ax\)

Substitute the given matrix and vector into the matrix multiplication formula:

\[
Ax =
\begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
\]

Multiply each row by the vector:

\[
Ax =
\begin{pmatrix}
(2)(4)+(-1)(2) \\
(1)(4)+(3)(2)
\end{pmatrix}
\]

Simplify:

\[
Ax =
\begin{pmatrix}
8-2 \\
4+6
\end{pmatrix}
=
\boxed{\begin{pmatrix}6\\10\end{pmatrix}}
\]

### Step 2: Express \(Ax\) as a Linear Combination of Columns

The columns of matrix \(A\) are:

\[
c_1 = \begin{pmatrix}2\\1\end{pmatrix},
\qquad
c_2 = \begin{pmatrix}-1\\3\end{pmatrix}
\]

The entries of vector \(x\) are \(x_1=4\) and \(x_2=2\).

Using the linear combination formula:

\[
Ax = x_1c_1+x_2c_2
\]

Substitute the values:

\[
Ax =
4\begin{pmatrix}2\\1\end{pmatrix}
+
2\begin{pmatrix}-1\\3\end{pmatrix}
\]

Multiply each column by its coefficient:

\[
Ax =
\begin{pmatrix}8\\4\end{pmatrix}
+
\begin{pmatrix}-2\\6\end{pmatrix}
\]

Add the vectors:

\[
Ax =
\begin{pmatrix}8-2\\4+6\end{pmatrix}
=
\boxed{\begin{pmatrix}6\\10\end{pmatrix}}
\]

---

## ✅ Final Answer

The matrix-vector product is:

\[
\boxed{Ax=\begin{pmatrix}6\\10\end{pmatrix}}
\]

Expressed as a linear combination of the columns of \(A\):

\[
\boxed{
Ax =
4\begin{pmatrix}2\\1\end{pmatrix}
+
2\begin{pmatrix}-1\\3\end{pmatrix}
}
\]

**Conclusion:** Both methods give the same result, confirming that matrix-vector multiplication is equivalent to a linear combination of the matrix's columns.

---

*Topic: Linear Algebra — Matrix-Vector Multiplication and Linear Combinations*
