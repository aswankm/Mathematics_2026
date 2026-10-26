### Exercise 9. Ellipsoid and Its Cross-Sections

**Statement:**  
Consider

$$
\frac{x^2}{9} + \frac{y^2}{4} + \frac{z^2}{16} = 1.
$$

Give the semiaxis lengths, describe the cross-section $z = 0$, and explain how the cross-sections $z = c$ change for $|c| < 4$.

> **Why this exercise:** teaches how to understand a 3D surface through a family of simpler 2D cross-sections.

---

### Solution

#### 1. Semiaxis Lengths
The canonical equation of a triaxial ellipsoid centered at the origin is:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} + \frac{z^2}{c_0^2} = 1
$$

Comparing the denominators:
- $a^2 = 9 \implies a = 3$ (semiaxis along the $x$-axis)
- $b^2 = 4 \implies b = 2$ (semiaxis along the $y$-axis)
- $c_0^2 = 16 \implies c_0 = 4$ (semiaxis along the $z$-axis)

---

#### 2. Cross-Section at $z = 0$
Substitute $z = 0$ into the original surface equation:

$$
\frac{x^2}{9} + \frac{y^2}{4} + \frac{0^2}{16} = 1 \implies \frac{x^2}{9} + \frac{y^2}{4} = 1
$$

- **Shape:** An **ellipse** in the $xy$-plane.
- **Features:** 
  - Centered at $(0,0,0)$.
  - Horizontal semiaxis along $x$: $a = 3$.
  - Vertical semiaxis along $y$: $b = 2$.

---

#### 3. Cross-Sections $z = c$ for $|c| < 4$
Substitute $z = c$ into the equation and rearrange:

$$
\frac{x^2}{9} + \frac{y^2}{4} + \frac{c^2}{16} = 1 \implies \frac{x^2}{9} + \frac{y^2}{4} = 1 - \frac{c^2}{16}
$$

Since $|c| < 4$, the factor $\left(1 - \frac{c^2}{16}\right)$ is strictly positive. Divide both sides by $\left(1 - \frac{c^2}{16}\right)$:

$$
\frac{x^2}{9\left(1 - \frac{c^2}{16}\right)} + \frac{y^2}{4\left(1 - \frac{c^2}{16}\right)} = 1
$$

**Description of Changes:**
- **Type of Curve:** For any constant plane $z = c$ with $|c| < 4$, the cross-section is an **ellipse**.
- **Behavior as $|c|$ increases from $0$ to $4$:**
  - At $c = 0$, the cross-section is the largest possible ellipse (the equatorial cross-section).
  - As $|c|$ increases toward $4$, the term $\left(1 - \frac{c^2}{16}\right)$ decreases toward $0$.
  - Consequently, both effective semiaxes $a(c) = 3\sqrt{1 - \frac{c^2}{16}}$ and $b(c) = 2\sqrt{1 - \frac{c^2}{16}}$ shrink continuously.
  - At the boundary $|c| = 4$, the cross-section degenerates to a single point: $(0,0,4)$ or $(0,0,-4)$ (the poles of the ellipsoid). For $|c| > 4$, no real cross-section exists.
