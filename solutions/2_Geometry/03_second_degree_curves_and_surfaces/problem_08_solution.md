### Exercise 8. Sphere

**Statement:**  
Reduce

$$
x^2 + y^2 + z^2 - 4x + 2y - 6z - 2 = 0
$$

to canonical form. Find the center and radius. Give two points on the sphere and check them in the equation.

> **Why this exercise:** transfers the technique known from circles from two dimensions to three.

---

### Solution

#### 1. Complete the Square to Find the Canonical Form
Group the $x$, $y$, and $z$ terms together and move the constant term to the right-hand side:

$$
(x^2 - 4x) + (y^2 + 2y) + (z^2 - 6z) = 2
$$

Complete the square for each variable:
- For $x$: $\left(\frac{-4}{2}\right)^2 = 4$
- For $y$: $\left(\frac{2}{2}\right)^2 = 1$
- For $z$: $\left(\frac{-6}{2}\right)^2 = 9$

Add these values to both sides of the equation:

$$
(x^2 - 4x + 4) + (y^2 + 2y + 1) + (z^2 - 6z + 9) = 2 + 4 + 1 + 9
$$

Rewrite as squared binomials:

$$
(x - 2)^2 + (y + 1)^2 + (z - 3)^2 = 16
$$

This is the **canonical form** of the sphere equation.

---

#### 2. Identify Center and Radius
Comparing $(x - 2)^2 + (y + 1)^2 + (z - 3)^2 = 16$ with the standard sphere equation $(x - x_0)^2 + (y - y_0)^2 + (z - z_0)^2 = R^2$:

- **Center $(x_0, y_0, z_0)$:** $(2, -1, 3)$
- **Radius $R$:** $\sqrt{16} = 4$

---

#### 3. Find Two Points on the Sphere
Using the center $(2, -1, 3)$ and radius $R = 4$, we can easily pick two points along the principal coordinate directions:

1. **Point $P_1$ (move 4 units along the positive $x$-axis):**  
   $(2 + 4, -1, 3) = (6, -1, 3)$

2. **Point $P_2$ (move 4 units along the positive $z$-axis):**  
   $(2, -1, 3 + 4) = (2, -1, 7)$

---

#### 4. Verification

##### **Verification for Point $P_1 = (6, -1, 3)$:**
- **Canonical Form:**  
  
$$
  (6 - 2)^2 + (-1 + 1)^2 + (3 - 3)^2 = 4^2 + 0^2 + 0^2 = 16 \quad (\text{True})
$$

- **General Form:**  
  
$$
  6^2 + (-1)^2 + 3^2 - 4(6) + 2(-1) - 6(3) - 2
$$

$$
  = 36 + 1 + 9 - 24 - 2 - 18 - 2 = 46 - 46 = 0 \quad (\text{True})
$$

##### **Verification for Point $P_2 = (2, -1, 7)$:**
- **Canonical Form:**  

$$
  (2 - 2)^2 + (-1 + 1)^2 + (7 - 3)^2 = 0^2 + 0^2 + 4^2 = 16 \quad (\text{True})
$$

- **General Form:**  
  
$$
  2^2 + (-1)^2 + 7^2 - 4(2) + 2(-1) - 6(7) - 2
$$

  $$
  = 4 + 1 + 49 - 8 - 2 - 42 - 2 = 54 - 54 = 0 \quad (\text{True})
  $$

Both points satisfy both forms of the equation correctly.
