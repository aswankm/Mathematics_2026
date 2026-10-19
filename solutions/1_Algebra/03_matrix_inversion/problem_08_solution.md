## Exercise 8. Inverse of a Transformation

### Compute:
The matrix 

$$
S = \begin{pmatrix} 2 & 0 \\ 0 & \frac{1}{2} \end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S, S^{-1}$ on one simple vector[cite: 9].

### Solution:

**1. Find $S^{-1}$:**
Using the diagonal inverse method ($\det(S) = 1$):

$$
S^{-1} = \begin{pmatrix} 0.5 & 0 \\ 0 & 2 \end{pmatrix}
$$

**2. Geometric Explanation:**
* $S$ stretches the horizontal $x$-axis by a factor of $2$ and shrinks the vertical $y$-axis by a factor of $0.5$[cite: 9].
* $S^{-1}$ undoes this by shrinking the $x$-axis by a factor of $0.5$ and stretching the $y$-axis by a factor of $2$[cite: 9].

**3. Check on a Vector:**
Let $v = \begin{pmatrix} 4 \\ 6 \end{pmatrix}$:

$$
Sv = \begin{pmatrix} 2 & 0 \\ 0 & 0.5 \end{pmatrix} \begin{pmatrix} 4 \\ 6 \end{pmatrix} = \begin{pmatrix} 8 \\ 3 \end{pmatrix}
$$

$$
S^{-1}(Sv) = \begin{pmatrix} 0.5 & 0 \\ 0 & 2 \end{pmatrix} \begin{pmatrix} 8 \\ 3 \end{pmatrix} = \begin{pmatrix} 4 \\ 6 \end{pmatrix} = v
$$

* **Conclusion:** Applying $S$ and then $S^{-1}$ fully restores the original vector[cite: 9].
