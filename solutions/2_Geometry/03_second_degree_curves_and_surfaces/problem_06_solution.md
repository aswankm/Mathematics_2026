### Exercise 6. Shifted Ellipse

**Statement:**  
Reduce

$$
4x^2 + 9y^2 - 16x + 18y - 11 = 0
$$

to canonical form. Give the center and semiaxis lengths. Check that substituting the coordinates of the center into the left-hand side gives a value consistent with the form you obtained.

> **Why this exercise:** reinforces completing the square and recognizing a shift of the coordinate system.

---

### Solution

#### 1. Complete the Square to Find the Canonical Form
Group the $x$ and $y$ terms together and move the constant term to the right-hand side:

$$
(4x^2 - 16x) + (9y^2 + 18y) = 11
$$

Factor out the leading coefficients from each group:

$$
4(x^2 - 4x) + 9(y^2 + 2y) = 11
$$

Complete the square inside each parenthesis:
- For $x$: $\left(\frac{-4}{2}\right)^2 = 4$
- For $y$: $\left(\frac{2}{2}\right)^2 = 1$

Add the corresponding weighted values to the right-hand side:

$$
4(x^2 - 4x + 4) + 9(y^2 + 2y + 1) = 11 + 4(4) + 9(1)
$$

$$
4(x - 2)^2 + 9(y + 1)^2 = 11 + 16 + 9
$$

$$
4(x - 2)^2 + 9(y + 1)^2 = 36
$$

Divide both sides by $36$ to obtain the canonical form equal to $1$:

$$
\frac{4(x - 2)^2}{36} + \frac{9(y + 1)^2}{36} = 1 \implies \frac{(x - 2)^2}{9} + \frac{(y + 1)^2}{4} = 1
$$

This is the **canonical form** of the shifted ellipse.

---

#### 2. Identify Center and Semiaxis Lengths
Comparing with the standard equation $\frac{(x - h)^2}{a^2} + \frac{(y - k)^2}{b^2} = 1$:

- **Center $(h, k)$:** $(2, -1)$
- **Semi-major axis $a$:** $\sqrt{9} = 3$ (along the horizontal direction)
- **Semi-minor axis $b$:** $\sqrt{4} = 2$ (along the vertical direction)

---

#### 3. Check Center Coordinates in the Equations

1. **Substitute $(2, -1)$ into the original left-hand side:**

$$
   4(2)^2 + 9(-1)^2 - 16(2) + 18(-1) - 11 = 4(4) + 9(1) - 32 - 18 - 11
$$

$$
   = 16 + 9 - 32 - 18 - 11 = 25 - 61 = -36
$$

2. **Consistency check with the completed square form:**  
   Before dividing by $36$, our equation was $4(x - 2)^2 + 9(y + 1)^2 - 36 = 0$.  
   Evaluating the un-shifted terms at $(2, -1)$ yields $0 + 0 - 36 = -36$. 

This confirms that at the center $(2, -1)$, the variable parts evaluate to $0$, leaving $-36$, which precisely balances the constant $+36$ required to equal $1$ in canonical form.
