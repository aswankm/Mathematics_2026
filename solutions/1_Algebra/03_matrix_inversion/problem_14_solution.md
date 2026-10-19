## Exercise 14. A Matrix That Is Its Own Inverse

### Compute:
Assume that a square matrix $A$ satisfies

$$
A^2 = I
$$

Show that

$$
A^{-1} = A
$$

Then give an example of a $2 \times 2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication[cite: 8].

### Solution:

**1. Proof that $A^{-1} = A$:**
* Start with the given equation:
  
$$
A \cdot A = I
$$

* By the definition of an inverse matrix, if multiplying $A$ by $A$ produces the identity matrix $I$, then $A$ is its own inverse, meaning $A^{-1} = A$[cite: 8].

**2. Example Matrix:**
Consider the $2 \times 2$ matrix:

$$
A = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}
$$

(Note that $A \neq I$ and $A \neq -I$)[cite: 8].

**3. Verification by Multiplication:**

$$
A^2 = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I
$$

* **Conclusion:** Since $A^2 = I$, the example successfully satisfies the condition and acts as its own inverse[cite: 8].
