## Problem 11. Volume of a Solid of Revolution

The region under the graph

$$y = \sqrt{x}, \quad x \in [0, 4],$$

is rotated about the $x$-axis.

1. Construct the integral describing the volume using the disk method.
2. Compute the volume.
3. Explain where the factor $\pi y^2$ in the integral comes from.

> Why this problem: it teaches how to construct an integral from the geometry of cross-sections instead of applying a volume formula without understanding its origin.

---

### Solution

#### 1. Constructing the Volume Integral
Using the disk method for rotation around the $x$-axis, each thin vertical slice at position $x$ with width $dx$ forms a circular disk upon rotation. 

The radius of each disk is given by the height of the curve $y = f(x) = \sqrt{x}$. The volume of an elemental disk is:

$$dV = \pi [f(x)]^2 \, dx = \pi (\sqrt{x})^2 \, dx = \pi x \, dx$$

Integrating over the interval $x \in [0, 4]$ yields the volume integral:

$$V = \int_{0}^{4} \pi (\sqrt{x})^2 \, dx = \pi \int_{0}^{4} x \, dx$$

---

#### 2. Computing the Volume
Evaluate the antiderivative of $x$:

$$\int_{0}^{4} x \, dx = \left[ \frac{x^2}{2} \right]_{0}^{4} = \frac{4^2}{2} - \frac{0^2}{2} = \frac{16}{2} = 8$$

Multiply by $\pi$:

$$V = \pi \cdot 8 = 8\pi$$

Thus, the volume of the solid of revolution is **$8\pi$** (or approximately $25.13$).

---

#### 3. Origin of the Factor $\pi y^2$
When a 2D region bounded by a function $y = f(x)$ is rotated around the $x$-axis:
* The cross-section perpendicular to the axis of rotation at any point $x$ forms a flat circular disk.
* The radius $r$ of this circular cross-section is the vertical distance from the $x$-axis to the curve, which is $r = y = f(x)$.
* The surface area of a circle with radius $r$ is given by $A = \pi r^2 = \pi y^2$.

Multiplying this cross-sectional area $\pi y^2$ by an infinitesimal thickness $dx$ gives the volume $dV = \pi y^2 \, dx$ of an individual disk, which is then summed (integrated) across the interval.
