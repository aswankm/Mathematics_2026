## Exercise 5. A 3x3 Matrix

### Compute:
Use Gauss-Jordan elimination to find the inverse of

$$
A = \begin{pmatrix} 1 & 1 & 0 \\ 0 & 1 & 1 \\ 1 & 0 & 1 \end{pmatrix}
$$

Check the result by multiplication[cite: 10].

### Solution:

**1. Set up the Augmented Matrix $[A \mid I]$:**
$$
\left(\begin{array}{ccc|ccc} 1 & 1 & 0 & 1 & 0 & 0 \\ 0 & 1 & 1 & 0 & 1 & 0 \\ 1 & 0 & 1 & 0 & 0 & 1 \end{array}\right)
$$

**2. Successive Row Operations:**
* $R_3 \to R_3 - R_1$:
  
$$
\left(\begin{array}{ccc|ccc} 1 & 1 & 0 & 1 & 0 & 0 \\ 0 & 1 & 1 & 0 & 1 & 0 \\ 0 & -1 & 1 & -1 & 0 & 1 \end{array}\right)
$$

* $R_3 \to R_3 + R_2$:
  
$$
\left(\begin{array}{ccc|ccc} 1 & 1 & 0 & 1 & 0 & 0 \\ 0 & 1 & 1 & 0 & 1 & 0 \\ 0 & 0 & 2 & -1 & 1 & 1 \end{array}\right)
$$

* $R_3 \to \frac{1}{2}R_3$, then back-substitute to clear above the diagonal:
  
$$
\left(\begin{array}{ccc|ccc} 1 & 0 & 0 & 0.5 & -0.5 & 0.5 \\ 0 & 1 & 0 & 0.5 & 0.5 & -0.5 \\ 0 & 0 & 1 & -0.5 & 0.5 & 0.5 \end{array}\right)
$$

**3. Resulting Inverse:**
$$
A^{-1} = \frac{1}{2}\begin{pmatrix} 1 & -1 & 1 \\ 1 & 1 & -1 \\ -1 & 1 & 1 \end{pmatrix}
$$

**4. Check via Multiplication:**
Multiplying $A$ by $A^{-1}$ yields the identity matrix $I$, confirming the calculation is correct[cite: 10].
