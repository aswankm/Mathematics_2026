## Exercise 10. Inverse of a Diagonal Matrix

### Compute:
Given 

$$
D = \begin{pmatrix} 2 & 0 & 0 \\ 0 & -3 & 0 \\ 0 & 0 & 5 \end{pmatrix}, \quad E = \begin{pmatrix} 2 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 5 \end{pmatrix}
$$

Without using Gauss-Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication[cite: 8].

### Solution:

**1. Determine Invertibility:**
* **Matrix $D$:** All diagonal entries ($2, -3, 5$) are non-zero, so **$D$ is invertible**[cite: 8].
* **Matrix $E$:** Contains a zero on the diagonal ($0$), making its determinant zero, so **$E$ is not invertible**[cite: 8].

**2. Find $D^{-1}$:**
For a diagonal matrix, invert each non-zero entry on the main diagonal:

$$
D^{-1} = \begin{pmatrix} \frac{1}{2} & 0 & 0 \\ 0 & -\frac{1}{3} & 0 \\ 0 & 0 & \frac{1}{5} \end{pmatrix}
$$

**3. Check via Multiplication:**

$$
D D^{-1} = \begin{pmatrix} 2 & 0 & 0 \\ 0 & -3 & 0 \\ 0 & 0 & 5 \end{pmatrix} \begin{pmatrix} \frac{1}{2} & 0 & 0 \\ 0 & -\frac{1}{3} & 0 \\ 0 & 0 & \frac{1}{5} \end{pmatrix} = \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix} = I
$$

* **Conclusion:** $D D^{-1} = I$, verifying that the diagonal inverse formula is correct[cite: 8].
