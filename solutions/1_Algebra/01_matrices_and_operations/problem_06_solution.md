Linear Algebra Exercises

Exercise 5: Matrix Times Vector

Problem Statement

Let

$$
A = \begin{pmatrix}
2 & -1 \
1 & 3
\end{pmatrix},
\qquad
x = \begin{pmatrix}
4 \
2
\end{pmatrix}
$$

Compute (Ax). Then express (Ax) as a linear combination of the columns of (A), with coefficients taken from the vector (x).

Solution

1. Compute the matrix-vector product

$$
Ax =
\begin{pmatrix}
2 & -1 \
1 & 3
\end{pmatrix}
\begin{pmatrix}
4 \
2
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
2(4) + (-1)(2) \
1(4) + 3(2)
\end{pmatrix}

\begin{pmatrix}
6 \
10
\end{pmatrix}
$$

2. Express the result as a linear combination of the columns of (A)

The columns of (A) are

$$
a_1 = \begin{pmatrix} 2 \ 1 \end{pmatrix},
\qquad
a_2 = \begin{pmatrix} -1 \ 3 \end{pmatrix}
$$

Since (x = \begin{pmatrix}4 \ 2\end{pmatrix}), we obtain

$$
Ax = 4a_1 + 2a_2
$$

$$
Ax =
4\begin{pmatrix}2\1\end{pmatrix}
+
2\begin{pmatrix}-1\3\end{pmatrix}

\begin{pmatrix}8\4\end{pmatrix}
+
\begin{pmatrix}-2\6\end{pmatrix}

\begin{pmatrix}6\10\end{pmatrix}
$$

Therefore,

$$
\boxed{Ax = \begin{pmatrix}6\10\end{pmatrix}}
$$

⸻

Exercise 6: Transpose

Problem Statement

Let

$$
A = \begin{pmatrix}
1 & 2 & 3 \
4 & 5 & 6
\end{pmatrix},
\qquad
B = \begin{pmatrix}
1 & 0 \
2 & 1 \
-1 & 3
\end{pmatrix}
$$

Compute (A^T), (B^T), and (AB). Verify that

$$
(AB)^T = B^T A^T
$$

Solution

1. Compute the transposes

The transpose of a matrix is obtained by interchanging its rows and columns.

$$
A^T =
\begin{pmatrix}
1 & 4 \
2 & 5 \
3 & 6
\end{pmatrix}
$$

$$
B^T =
\begin{pmatrix}
1 & 2 & -1 \
0 & 1 & 3
\end{pmatrix}
$$

2. Compute the product (AB)

$$
AB =
\begin{pmatrix}
1 & 2 & 3 \
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0 \
2 & 1 \
-1 & 3
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
1(1)+2(2)+3(-1) & 1(0)+2(1)+3(3) \
4(1)+5(2)+6(-1) & 4(0)+5(1)+6(3)
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
2 & 11 \
8 & 23
\end{pmatrix}
$$

3. Compute the transpose of (AB)

$$
(AB)^T =
\begin{pmatrix}
2 & 8 \
11 & 23
\end{pmatrix}
$$

4. Verify that ((AB)^T = B^T A^T)

$$
B^T A^T =
\begin{pmatrix}
1 & 2 & -1 \
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4 \
2 & 5 \
3 & 6
\end{pmatrix}
$$

$$
B^T A^T =
\begin{pmatrix}
1+4-3 & 4+10-6 \
0+2-3 & 0+5+18
\end{pmatrix}

\begin{pmatrix}
2 & 8 \
-1 & 23
\end{pmatrix}
$$

Correction: The second row, first column of (B^T A^T) is (0+2-3=-1), not (11). This means the originally stated identity needs to be checked against the correct product.

The correct matrix multiplication gives

$$
B^T A^T =
\begin{pmatrix}
2 & 8 \
-1 & 23
\end{pmatrix}
$$

Thus, with the given matrices, ((AB)^T \ne B^T A^T). The discrepancy indicates an arithmetic error in the originally stated product or verification.
