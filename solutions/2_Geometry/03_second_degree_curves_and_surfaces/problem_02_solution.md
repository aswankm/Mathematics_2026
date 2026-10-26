### Exercise 2. Circle by Completing the Square

**Statement:**  
Reduce

$$
x^2 + y^2 - 6x + 4y - 3 = 0
$$

to canonical form. Find the center and radius, then substitute two simple points from the circle into both forms of the equation.

> **Why this exercise:** practices completing the square as a transition from a general equation to the geometry of the object.

---

### Solution

#### 1. Complete the Square to Find the Canonical Form
Group the $x$ and $y$ terms together and move the constant term to the right-hand side:

$$
(x^2 - 6x) + (y^2 + 4y) = 3
$$

Complete the square for both variables:
- For $x$: $\left(\frac{-6}{2}\right)^2 = (-3)^2 = 9$
- For $y$: $\left(\frac{4}{2}\right)^2 = 2^2 = 4$

Add $9$ and $4$ to both sides of the equation:

$$
(x^2 - 6x + 9) + (y^2 + 4y + 4) = 3 + 9 + 4
$$

Rewrite as squared binomials:

$$
(x - 3)^2 + (y + 2)^2 = 16
$$

This is the **canonical form** of the circle equation.

---

#### 2. Identify the Center and Radius
Comparing $(x - 3)^2 + (y + 2)^2 = 16$ with the standard circle equation $(x - h)^2 + (y - k)^2 = R^2$:

- **Center $(h, k)$:** $(3, -2)$
- **Radius $R$:** $\sqrt{16} = 4$

---

#### 3. Find Two Simple Points on the Circle
Using the center $(3, -2)$ and radius $R = 4$, we can easily pick two points along the principal axes:

1. **Point $P_1$ (move 4 units right from center):**  
   $(3 + 4, -2) = (7, -2)$

2. **Point $P_2$ (move 4 units up from center):**  
   $(3, -2 + 4) = (3, 2)$

---

#### 4. Substitute Points into Both Equations to Verify

##### **Verification for Point $P_1 = (7, -2)$:**
- **Canonical Form:**  
  
  $$
  (7 - 3)^2 + (-2 + 2)^2 = 4^2 + 0^2 = 16 \quad (\text{True})
  $$

- **General Form:**  
  
  $$
  7^2 + (-2)^2 - 6(7) + 4(-2) - 3 = 49 + 4 - 42 - 8 - 3 = 53 - 53 = 0 \quad (\text{True})
  $$

##### **Verification for Point $P_2 = (3, 2)$:**
- **Canonical Form:**  
  
  $$
  (3 - 3)^2 + (2 + 2)^2 = 0^2 + 4^2 = 16 \quad (\text{True})
  $$

- **General Form:**  
  
  $$
  3^2 + 2^2 - 6(3) + 4(2) - 3 = 9 + 4 - 18 + 8 - 3 = 21 - 21 = 0 \quad (\text{True})
  $$

Both forms yield consistent results for both points.
