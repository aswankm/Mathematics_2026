## Exercise 14. A System of Equations and the Determinant

### Compute:
Consider the system $Ax = b$, where 

$$
A = \begin{pmatrix} 1 & 2 \\ k & 4 \end{pmatrix}
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution[cite: 18].

### Solution:

**1. Compute the Determinant:**
$$
\det(A) = (1)(4) - (2)(k) = 4 - 2k
$$

**2. Unique Solution Condition:**
A linear system has a unique solution for every $b$ if and only if $\det(A) \neq 0$[cite: 18]:
$$
4 - 2k \neq 0 \implies k \neq 2
$$
* **Result:** For **$k \neq 2$**, the system has exactly one solution for every $b$[cite: 18].

**3. Exceptional Case ($k = 2$):**
For $k = 2$, reduce the augmented matrix $[A \mid b]$ via row operations ($R_2 \to R_2 - 2R_1$):

$$
\begin{pmatrix} 1 & 2 & \vline & b_1 \\ 0 & 0 & \vline & b_2 - 2b_1 \end{pmatrix}
$$

* **Infinitely Many Solutions:** Requires $b_2 - 2b_1 = 0$. 
  * *Example:* $b = \begin{pmatrix} 1 \\ 2 \end{pmatrix}$[cite: 18].
* **No Solution:** Requires $b_2 - 2b_1 \neq 0$. 
  * *Example:* $b = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$[cite: 18].
