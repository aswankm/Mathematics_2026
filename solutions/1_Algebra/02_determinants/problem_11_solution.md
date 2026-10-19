## Exercise 11. Shortening the Calculation with Row Operations

### Compute:

$$

\det \begin{pmatrix} 1 & 2 & 3 \\ 1 & 3 & 4 \\ 1 & 4 & 6 \end{pmatrix}

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant[cite: 16].

$$

### Solution:

**1. Row Operations (Row Replacement):**
To introduce zeros below the first pivot, apply row replacement operations ($R_2 \to R_2 - R_1$ and $R_3 \to R_3 - R_1$):

$$
\begin{pmatrix} 1 & 2 & 3 \\ 0 & 1 & 1 \\ 0 & 2 & 3 \end{pmatrix}
$$

* **Property Note:** **Row replacement operations** (adding a multiple of one row to another) do not change the value of the determinant[cite: 16].

**2. Further Simplification:**
Next, apply $R_3 \to R_3 - 2R_2$ to eliminate the remaining entry below the diagonal:

$$
\begin{pmatrix} 1 & 2 & 3 \\ 0 & 1 & 1 \\ 0 & 0 & 1 \end{pmatrix}
$$

**3. Final Computation:**
Since the matrix is now in upper-triangular form, multiply the entries along the main diagonal:

$$
\det = (1) \cdot (1) \cdot (1) = 1
$$
