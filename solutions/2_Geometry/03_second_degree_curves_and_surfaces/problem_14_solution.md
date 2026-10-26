### Exercise 14. Cone and Cylinder

**Statement:**  
Compare

$$
x^2 + y^2 = z^2
$$

and

$$
x^2 + y^2 = 4.
$$

For each surface, describe the cross-sections $z = c$, $x = 0$, and $y = 0$, make a sketch, and explain why the radius of the cross-section depends on $z$ in the first case but is constant in the second.

> **Why this exercise:** teaches how to distinguish a cone from a cylinder by the behavior of their cross-sections.

---

### Solution

#### 1. Analysis of Surface 1: $x^2 + y^2 = z^2$ (Circular Cone)

* **Cross-Sections $z = c$ (horizontal planes):**  
  Substitute $z = c$ into the equation:

$$
  x^2 + y^2 = c^2
$$

  * For $c \neq 0$: A **circle** centered at $(0, 0, c)$ with radius $R(c) = |c|$.
  * For $c = 0$: A single **point**, the origin $(0, 0, 0)$ (the apex of the cone).

* **Cross-Section $x = 0$ ($yz$-plane):**  

$$
  y^2 = z^2 \implies y = \pm z
$$

  Two intersecting straight lines through the origin with slopes $+1$ and $-1$.

* **Cross-Section $y = 0$ ($xz$-plane):**  

$$
  x^2 = z^2 \implies x = \pm z
$$

  Two intersecting straight lines through the origin with slopes $+1$ and $-1$.

* **Qualitative Sketch Description:**  
  A double-napped circular cone with its apex at the origin $(0,0,0)$, opening infinitely upward along $+z$ and downward along $-z$.

---

#### 2. Analysis of Surface 2: $x^2 + y^2 = 4$ (Circular Cylinder)

* **Cross-Sections $z = c$ (horizontal planes):**  
  Substitute $z = c$ into the equation:

$$
  x^2 + y^2 = 4
$$

  For any constant height $z = c$, the cross-section is a **circle** centered at $(0, 0, c)$ with fixed radius $R = \sqrt{4} = 2$.

* **Cross-Section $x = 0$ ($yz$-plane):**  

$$
  y^2 = 4 \implies y = \pm 2
$$

  Two parallel vertical straight lines extending infinitely along the $z$-axis.

* **Cross-Section $y = 0$ ($xz$-plane):**  

$$
  x^2 = 4 \implies x = \pm 2
$$

  Two parallel vertical straight lines extending infinitely along the $z$-axis.

* **Qualitative Sketch Description:**  
  An infinitely long right circular cylinder extending vertically along the $z$-axis with a uniform circular radius of $2$.

---

#### 3. Why the Radius Depends on $z$ in the Cone but is Constant in the Cylinder

* **Cone ($x^2 + y^2 = z^2$):**  
  The horizontal radius is given by $R(z) = \sqrt{z^2} = |z|$. The variable $z$ appears directly inside the equation controlling the right-hand side. As height $|z|$ increases away from the origin, the circular radius grows proportionally to $|z|$.

* **Cylinder ($x^2 + y^2 = 4$):**  
  The variable $z$ is completely **absent** from the defining equation. This means the cross-sectional shape in the $xy$-plane ($x^2 + y^2 = 4$) is entirely independent of the height $z$. The same circular cross-section of constant radius $R = 2$ is simply extruded along the $z$-axis.
