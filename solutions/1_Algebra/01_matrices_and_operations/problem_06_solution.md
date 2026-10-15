## Exercise 6. Transpose

### Statement
For $A = \begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{pmatrix}$ and $B = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix}$, compute $A^T$, $B^T$, and $AB$. Verify that $(AB)^T = B^T A^T$.
[cite: 7]

### Theory
* **Transpose:** Swaps rows and columns.
* **Transpose of a Product:** $(AB)^T = B^T A^T$.
[cite: 7]

### Essential Steps & Solution
1. **Compute $A^T$ and $B^T$:**
   $$A^T = \begin{pmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{pmatrix}, \quad B^T = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \end{pmatrix}$$[cite: 7]
2. **Compute $AB$ and $(AB)^T$:**
   $$AB = \begin{pmatrix} (1)(1)+(2)(2)+(3)(-1) & (1)(0)+(2)(1)+(3)(3) \\ (4)(1)+(5)(2)+(6)(-1) & (4)(0)+(5)(1)+(6)(3) \end{pmatrix} = \begin{pmatrix} 1+4-3 & 0+2+9 \\ 4+10-6 & 0+5+18 \end{pmatrix} = \begin{pmatrix} 2 & 11 \\ 8 & 23 \end{pmatrix}$$[cite: 7]
   $$(AB)^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}$$[cite: 7]
3. **Compute $B^T A^T$:**
   $$B^T A^T = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \end{pmatrix} \begin{pmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{pmatrix} = \begin{pmatrix} (1)(1)+(2)(2)+(-1)(3) & (1)(4)+(2)(5)+(-1)(6) \\ (0)(1)+(1)(2)+(3)(3) & (0)(4)+(1)(5)+(3)(6) \end{pmatrix} = \begin{pmatrix} 1+4-3 & 4+10-6 \\ 0+2+9 & 0+5+18 \end{pmatrix} = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}$$[cite: 7]
4. **Verification:** $(AB)^T = B^T A^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}$ holds true[cite: 7].

---
