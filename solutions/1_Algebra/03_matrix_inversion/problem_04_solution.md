## Exercise 4. Gauss-Jordan

### Compute:
Find $A^{-1}$ using the Gauss-Jordan method for

$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 5 \end{pmatrix}
$$

Show the augmented matrix $[A \mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

### Solution:

**1. Set up the Augmented Matrix $[A \mid I]$:**
$$
\left(\begin{array}{cc|cc} 1 & 2 & 1 & 0 \\ 3 & 5 & 0 & 1 \end{array}\right)
$$

**2. Successive Row Operations:**
* Apply $R_2 \to R_2 - 3R_1$:
  
$$
\left(\begin{array}{cc|cc} 1 & 2 & 1 & 0 \\ 0 & -1 & -3 & 1 \end{array}\right)
$$

* Apply $R_2 \to -R_2$:
  
$$
\left(\begin{array}{cc|cc} 1 & 2 & 1 & 0 \\ 0 & 1 & 3 & -1 \end{array}\right)
$$

* Apply $R_1 \to R_1 - 2R_2$:
  
$$
\left(\begin{array}{cc|cc} 1 & 0 & -5 & 2 \\ 0 & 1 & 3 & -1 \end{array}\right)
$$

**3. Resulting Inverse:**
$$
A^{-1} = \begin{pmatrix} -5 & 2 \\ 3 & -1 \end{pmatrix}
$$

* **Explanation:** Row operations are equivalent to multiplying by elementary matrices ($E_k \cdots E_1 A = I$). Multiplying both sides by $A^{-1}$ shows that the accumulated operations transform $I$ into $A^{-1}$.
