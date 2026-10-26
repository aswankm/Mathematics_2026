### Exercise 10. Paraboloids

**Statement:**  
Compare

$$
z = x^2 + y^2
$$

and

$$
z = x^2 - y^2.
$$

For each surface, describe the cross-sections $x = 0$, $y = 0$, and $z = c$, then make a qualitative sketch.

> **Why this exercise:** teaches how to distinguish two basic types of paraboloids from their cross-sections.

---

### Solution

#### 1. Analysis of the First Surface: $z = x^2 + y^2$ (Elliptic / Circular Paraboloid)

* **Cross-Section $x = 0$ ($yz$-plane):**  

$$
  z = y^2
$$

  A parabola opening upwards along the positive $z$-axis with vertex at $(0, 0, 0)$.

* **Cross-Section $y = 0$ ($xz$-plane):**  

  $$
  z = x^2
  $$

  A parabola opening upwards along the positive $z$-axis with vertex at $(0, 0, 0)$.

* **Cross-Sections $z = c$ (horizontal planes):**  

$$
  x^2 + y^2 = c
$$

  * For $c > 0$: **Circles** centered at $(0, 0, c)$ with radius $R = \sqrt{c}$, expanding in size as $c$ increases.
  * For $c = 0$: A single **point**, the origin $(0, 0, 0)$.
  * For $c < 0$: **Empty set** (no real points, since $x^2 + y^2 \ge 0$).

* **Qualitative Sketch Description:**  
  A smooth bowl-shaped surface opening upwards, starting from its lowest point at the origin $(0, 0, 0)$ and symmetric about the $z$-axis.

---

#### 2. Analysis of the Second Surface: $z = x^2 - y^2$ (Hyperbolic Paraboloid)

* **Cross-Section $x = 0$ ($yz$-plane):**  

$$
  z = -y^2
$$

  A parabola opening downwards along the negative $z$-axis with vertex at $(0, 0, 0)$.

* **Cross-Section $y = 0$ ($xz$-plane):**  

$$
  z = x^2
$$

  A parabola opening upwards along the positive $z$-axis with vertex at $(0, 0, 0)$.

* **Cross-Sections $z = c$ (horizontal planes):**  

$$
  x^2 - y^2 = c
$$

  * For $c > 0$: **Hyperbolas** opening along the $x$-axis direction.
  * For $c = 0$: Two intersecting straight lines $x^2 - y^2 = 0 \implies y = \pm x$.
  * For $c < 0$: **Hyperbolas** opening along the $y$-axis direction.

* **Qualitative Sketch Description:**  
  A saddle-shaped surface passing through the origin $(0, 0, 0)$, curving upwards along the $x$-axis direction and downwards along the $y$-axis direction.

---

#### 3. Summary Comparison

| Surface | $x = 0$ | $y = 0$ | $z = c$ ($c > 0$) | Geometric Name |
| :--- | :--- | :--- | :--- | :--- |
| $z = x^2 + y^2$ | Parabola $z = y^2$ (upwards) | Parabola $z = x^2$ (upwards) | Circle $x^2 + y^2 = c$ | **Elliptic (Circular) Paraboloid** |
| $z = x^2 - y^2$ | Parabola $z = -y^2$ (downwards) | Parabola $z = x^2$ (upwards) | Hyperbola $x^2 - y^2 = c$ | **Hyperbolic Paraboloid** |
