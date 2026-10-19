## Exercise 12. A Parameter Revealed by a Row Operation

### Compute:
For 

$$
A(t) = \begin{pmatrix} 1 & 2 & 3 \\ 2 & 4 & t \\ 0 & 1 & 1 \end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible. Before computing the determinant, perform the operation $R_2 \gets R_2 - 2R_1$ and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found[cite: 16].

### Solution:

**1. Apply Row Operation:**
Applying $R_2 \gets R_2 - 2R_1$ (which does not change the determinant)[cite: 16]:

$$
A' = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 0 & t - 6 \\ 0 & 1 & 1 \end{pmatrix}
$$

**2. Compute Determinant:**
Expanding along Row 2:

$$
\det A(t) = -(t - 6) \begin{vmatrix} 1 & 2 \\ 0 & 1 \end{vmatrix} = -(t - 6)(1) = 6 - t
$$

**3. Condition for Non-Invertibility:**
Set $\det A(t) = 0$[cite: 13, 16]:

$$
6 - t = 0 \implies t = 6
$$

**4. Structural Explanation:**
When $t = 6$, the original second row becomes 

$$
\begin{pmatrix} 2 & 4 & 6 \end{pmatrix}
$$

which is an exact scalar multiple ($2 \times$) of the first row 

$$
\begin{pmatrix} 1 & 2 & 3 \end{pmatrix}
$$

[cite: 16]. This creates linear dependence between the rows, making the determinant zero and rendering the matrix non-invertible[cite: 1, 16].
