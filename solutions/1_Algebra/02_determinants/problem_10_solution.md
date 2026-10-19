## Exercise 10. Detecting Dependence

### Compute:
Without carrying out a full determinant calculation, explain why[cite: 15]:

$$
\det \begin{pmatrix} 1 & 2 & 3 \\ 2 & 4 & 6 \\ 0 & 1 & 5 \end{pmatrix} = 0
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix[cite: 15].

### Solution:

**1. Specific Row Dependence:**
* Comparing Row 1 ($R_1$) and Row 2 ($R_2$):

$$
R_2 = \begin{pmatrix} 2 & 4 & 6 \end{pmatrix} = 2 \cdot \begin{pmatrix} 1 & 2 & 3 \end{pmatrix} = 2 R_1
$$

* Row 2 is an exact scalar multiple of Row 1, making the rows **linearly dependent**[cite: 15].

**2. Why the Determinant equals 0:**
* Applying the row operation $R_2 \to R_2 - 2R_1$ produces a row filled entirely with zeros[cite: 15]. 
* Any matrix containing a row of zeros has a determinant equal to **$0$**[cite: 15].

**3. Connection to Non-invertibility:**
* A matrix is invertible if and only if its rows are linearly independent and its determinant is non-zero[cite: 15].
* Because the rows are linearly dependent, the matrix collapses volume to zero and is **not invertible**[cite: 15].
