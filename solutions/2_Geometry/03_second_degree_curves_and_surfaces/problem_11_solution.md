### Exercise 11. Two Similar Surfaces

**Statement:**  
Compare

$$
x^2 + y^2 - z^2 = 1
$$

and

$$
x^2 + y^2 - z^2 = -1.
$$

For several values $z = c$, check whether the cross-section exists and what its radius is. Based on this, describe qualitatively the difference between the surfaces and make sketches.

> **Why this exercise:** teaches how to recognize the shape of a surface from cross-sections instead of from a memorized catalog of names.

---

### Solution

#### 1. Analysis of Surface 1: $x^2 + y^2 - z^2 = 1$

Substitute $z = c$ into the equation:

$$
x^2 + y^2 = 1 + c^2
$$

* **Existence:** Since $c^2 \ge 0$, the right-hand side $1 + c^2$ is always greater than or equal to $1$ for all real values of $c \in \mathbb{R}$. Thus, a horizontal cross-section exists for **every value of $c$**.
* **Cross-Section Geometry:** Each cross-section $z = c$ is a **circle** centered at $(0, 0, c)$ with radius:

  $$
  R(c) = \sqrt{1 + c^2}
  $$

* **Radius Behavior:**
  * Minimum radius occurs at $z = 0$: $R(0) = \sqrt{1} = 1$ (the "waist" or neck of the surface).
  * As $|c| \to \infty$, $R(c)$ increases without bound.
* **Qualitative Shape:** A connected, single-piece surface with a central waist that opens outward infinitely in both the positive and negative $z$-directions. This is a **Hyperboloid of One Sheet**.

---

#### 2. Analysis of Surface 2: $x^2 + y^2 - z^2 = -1$

Substitute $z = c$ into the equation and rearrange:

$$
x^2 + y^2 = c^2 - 1
$$

* **Existence and Cross-Section Geometry:**
  * **For $|c| < 1$** (i.e., $-1 < c < 1$): $c^2 - 1 < 0$. Since $x^2 + y^2 \ge 0$, **no real cross-section exists**. There is a gap between $z = -1$ and $z = 1$.
  * **For $|c| = 1$** ($z = \pm 1$): $c^2 - 1 = 0 \implies x^2 + y^2 = 0$. The cross-section degenerates to a single **point**: $(0, 0, 1)$ and $(0, 0, -1)$ (the vertices).
  * **For $|c| > 1$**: $c^2 - 1 > 0$. The cross-section is a **circle** with radius:

    $$
    R(c) = \sqrt{c^2 - 1}
    $$

* **Qualitative Shape:** Two completely separate, symmetric cup-like pieces (one opening upwards for $z \ge 1$ and one opening downwards for $z \le -1$). This is a **Hyperboloid of Two Sheets**.

---

#### 3. Quantitative Cross-Section Comparison

| $z = c$ | Surface 1 ($x^2 + y^2 - z^2 = 1$) | Surface 2 ($x^2 + y^2 - z^2 = -1$) |
| :--- | :--- | :--- |
| $c = 0$ | Circle with radius $R = 1$ | No real points (gap) |
| $c = \pm 1$ | Circle with radius $R = \sqrt{2}$ | Single Point at $(0,0,\pm 1)$ ($R = 0$) |
| $c = \pm 2$ | Circle with radius $R = \sqrt{5}$ | Circle with radius $R = \sqrt{3}$ |
| $c = \pm 3$ | Circle with radius $R = \sqrt{10}$ | Circle with radius $R = \sqrt{8}$ |

---

#### 4. Summary of Qualitative Differences

- **Connectivity:** $x^2 + y^2 - z^2 = 1$ forms a **continuous single surface** connected across the origin plane $z = 0$, whereas $x^2 + y^2 - z^2 = -1$ is split into **two disconnected components** separated by a clear spatial gap for $-1 < z < 1$.
- **Waist vs. Vertices:** Surface 1 has its tightest circular waist ($R = 1$) at $z = 0$, while Surface 2 starts from apex points at $z = \pm 1$ and grows outward as $|z|$ increases.
