### Exercise 12. Recognizing a Surface from Cross-Sections

**Statement:**  
A certain surface has the following properties:

* the cross-section $z = 0$ is a point,
* for $z > 0$, the cross-sections $z = \text{const}$ are circles with increasing radius,
* vertical cross-sections through the $Oz$ axis are parabolas.

Propose a simple equation for such a surface and justify your choice.

> **Why this exercise:** reverses the usual reasoning: from geometry to an equation.

---

### Solution

#### 1. Proposed Equation
A simple equation representing this surface is:

$$
z = x^2 + y^2
$$

---

#### 2. Justification of the Properties

##### **Property 1: The cross-section $z = 0$ is a point**
Set $z = 0$ in the proposed equation:

$$
x^2 + y^2 = 0
$$

Since $x^2 \ge 0$ and $y^2 \ge 0$ for all real numbers $x, y \in \mathbb{R}$, the sum of two squares equals zero if and only if $x = 0$ and $y = 0$.  
Thus, the cross-section at $z = 0$ is the single point **$(0, 0, 0)$** (the origin).

---

##### **Property 2: For $z > 0$, horizontal cross-sections $z = c$ are circles with increasing radius**
Fix $z = c$ for any constant $c > 0$:

$$
x^2 + y^2 = c
$$

* This matches the canonical equation of a circle centered at $(0, 0, c)$ in the plane $z = c$.
* The radius of the circle is $R(c) = \sqrt{c}$.
* As $c$ increases ($z > 0$ increases), $R(c) = \sqrt{c}$ strictly increases, satisfying the condition that the radius grows as $z$ increases.

---

##### **Property 3: Vertical cross-sections through the $Oz$ axis are parabolas**
A vertical plane passing through the $z$-axis ($Oz$ axis) makes an angle $\theta$ with the $x$-axis. It can be defined parametrically by $x = r\cos\theta$ and $y = r\sin\theta$, where $r$ is the distance from the $z$-axis along that direction.

Substitute these into $z = x^2 + y^2$:

$$
z = (r\cos\theta)^2 + (r\sin\theta)^2 = r^2(\cos^2\theta + \sin^2\theta) = r^2
$$

* **In the $xz$-plane ($y = 0$):** $z = x^2$, which is an upward-opening parabola with vertex at $(0, 0, 0)$.
* **In the $yz$-plane ($x = 0$):** $z = y^2$, which is an upward-opening parabola with vertex at $(0, 0, 0)$.
* **In any arbitrary vertical plane through $Oz$:** The section is the parabola $z = r^2$.

---

#### 3. Conclusion
All three given properties uniquely characterize an **elliptic (circular) paraboloid** opening upward along the positive $z$-axis, which is described by the equation **$z = x^2 + y^2$**.
