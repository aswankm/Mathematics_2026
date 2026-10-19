## Exercise 13. Undoing a Composite Transformation

### Compute:
The matrices 

$$
S = \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}, \quad H = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
$$

describe nonuniform scaling and shear[cite: 7]. For $T = HS$, find $T^{-1}$ in two ways[cite: 7]:
1. First compute $T$, then its inverse[cite: 7].
2. Use $(HS)^{-1} = S^{-1}H^{-1}$[cite: 7].

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: "when undoing a composition of operations, we undo them from the end"[cite: 7].

### Solution:

**1. Method 1 (Compute $T$ then $T^{-1}$):**
* Find $T = HS$:
  
$$
T = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 1 \end{pmatrix}
$$

* Find $T^{-1}$ ($\det(T) = 2$):
  
$$
T^{-1} = \frac{1}{2} \begin{pmatrix} 1 & -1 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} 0.5 & -0.5 \\ 0 & 1 \end{pmatrix}
$$

**2. Method 2 (Use $(HS)^{-1} = S^{-1}H^{-1}$):**
* Compute individual inverses:
  
$$
S^{-1} = \begin{pmatrix} 0.5 & 0 \\ 0 & 1 \end{pmatrix}, \quad H^{-1} = \begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix}
$$

* Multiply in reverse order:
  
$$
S^{-1}H^{-1} = \begin{pmatrix} 0.5 & 0 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 0.5 & -0.5 \\ 0 & 1 \end{pmatrix}
$$

**3. Test Incorrect Order ($H^{-1}S^{-1}$):**
  
$$
H^{-1}S^{-1} = \begin{pmatrix} 1 & -1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 0.5 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 0.5 & -1 \\ 0 & 1 \end{pmatrix}
$$

* **Conclusion:** The incorrect order produces a different matrix[cite: 7]. The rule "undo them from the end" ensures that the final transformation applied is the first one reversed[cite: 7].
