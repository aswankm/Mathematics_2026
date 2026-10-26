### Exercise 13. Intersection of a Sphere and a Plane

**Statement:**  
Given the sphere

$$
x^2 + y^2 + z^2 = 25
$$

and the plane $z = 3$, find the equation of the curve of intersection, state what kind of curve it is, and give its center and radius in 3D space.

---

### Solution

#### 1. Substitute the Plane Equation into the Sphere Equation
To find the intersection of the sphere $x^2 + y^2 + z^2 = 25$ and the plane $z = 3$, substitute $z = 3$ into the equation of the sphere:

$$
x^2 + y^2 + (3)^2 = 25
$$

$$
x^2 + y^2 + 9 = 25 \implies x^2 + y^2 = 16
$$

---

#### 2. Classify the Intersection Curve
The system of equations representing the intersection curve is:

$$
\begin{cases}
x^2 + y^2 = 16 \\
z = 3
\end{cases}
$$

* **Type of Curve:** A **circle** lying parallel to the $xy$-plane at height $z = 3$.

---

#### 3. Determine Center and Radius in 3D Space
From the canonical equation of the circle $x^2 + y^2 = R^2$ in the plane $z = 3$:

* **Center:** The $x$ and $y$ coordinates of the center are $(0, 0)$, and its height is $z = 3$.  
  Therefore, in 3D space, the center is **$(0, 0, 3)$**.
* **Radius:** $R = \sqrt{16} = 4$.

---

#### 4. Geometric Verification
We can verify the radius using the Pythagorean theorem on the cross-sectional right triangle formed by:
1. The sphere's center at the origin $(0, 0, 0)$,
2. The intersection circle's center at $(0, 0, 3)$,
3. Any point $P$ on the circle of intersection.

- Distance from origin to plane along $z$-axis: $d = 3$
- Sphere radius: $R_{\text{sphere}} = \sqrt{25} = 5$

Using the right triangle relation $R_{\text{sphere}}^2 = d^2 + R_{\text{circle}}^2$:

$$
5^2 = 3^2 + R_{\text{circle}}^2 \implies 25 = 9 + R_{\text{circle}}^2 \implies R_{\text{circle}}^2 = 16 \implies R_{\text{circle}} = 4
$$

This confirms the radius of the intersection circle is **$4$**.
