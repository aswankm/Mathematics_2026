### Exercise 8. Intersection Point of a Line and a Plane

**Statement:**  
Find the intersection point of

$$
(x, y, z) = (1, 0, 2) + t(1, 2, -1)
$$

with the plane $x + y + z = 4$. Check the result by substituting it into both descriptions.

> **Why this exercise:** practices the most important computational case of the line–plane relationship.

---

### Solution

#### 1. Express the Line in Parametric Form
From the vector equation of the line, we write $x, y, z$ in terms of the parameter $t$:

$$
x = 1 + t
$$

$$
y = 2t
$$

$$
z = 2 - t
$$

#### 2. Find the Parameter $t$
Substitute the parametric expressions into the equation of the plane $x + y + z = 4$:

$$
(1 + t) + (2t) + (2 - t) = 4
$$

Simplify the equation:

$$
1 + 3 + 2t = 4 \implies 3 + 2t = 4 \implies 2t = 1 \implies t = \frac{1}{2}
$$

#### 3. Compute the Intersection Point
Substitute $t = \frac{1}{2}$ back into the parametric equations of the line:

- $x = 1 + \frac{1}{2} = \frac{3}{2}$
- $y = 2 \left(\frac{1}{2}\right) = 1$
- $z = 2 - \frac{1}{2} = \frac{3}{2}$

Thus, the point of intersection is $I = \left(\frac{3}{2}, 1, \frac{3}{2}\right)$.

#### 4. Verification

We verify that $I = \left(\frac{3}{2}, 1, \frac{3}{2}\right)$ lies on both the line and the plane:

1. **Check on the line:**

   For $t = \frac{1}{2}$:


   $$
   (1, 0, 2) + \frac{1}{2}(1, 2, -1) = \left(1 + \frac{1}{2}, 0 + 1, 2 - \frac{1}{2}\right) = \left(\frac{3}{2}, 1, \frac{3}{2}\right) \quad (\text{True})
   $$


3. **Check in the plane equation ($x + y + z = 4$):**

   $$
   \frac{3}{2} + 1 + \frac{3}{2} = 3 + 1 = 4 \quad (\text{True})
   $$

Since both descriptions are satisfied, the intersection point is **$\left(\frac{3}{2}, 1, \frac{3}{2}\right)$**.
