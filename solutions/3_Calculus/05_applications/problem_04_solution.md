## Problem 4. Area Between Curves

Find the area of the region bounded by the graphs

$$y = x$$

and

$$y = x^2.$$

First find the intersection points and justify which function is greater on the relevant interval.

> Why this problem: it teaches that before integrating, one must first determine the geometry of the region and the correct order of the functions.

---

### Solution

#### 1. Intersection Points
To find where the two curves intersect, set them equal to each other:
$$x = x^2$$
$$x^2 - x = 0$$
$$x(x - 1) = 0$$

This gives two intersection points:
* $x = 0 \implies y = 0 \implies (0, 0)$
* $x = 1 \implies y = 1 \implies (1, 1)$

The relevant interval of integration is therefore $[0, 1]$.

---

#### 2. Determining the Greater Function
To see which function is greater on the interval $(0, 1)$, we can test a value, such as $x = 0.5$:
* Upper curve candidate: $y = 0.5$
* Lower curve candidate: $y = (0.5)^2 = 0.25$

Since $0.5 > 0.25$, the linear function $f(x) = x$ is greater than the quadratic function $g(x) = x^2$ across the entire interval $(0, 1)$.

---

#### 3. Computing the Area
The area $A$ of the region is given by the integral of the upper function minus the lower function over the interval $[0, 1]$:

$$A = \int_{0}^{1} (x - x^2) \, dx$$

Evaluating the antiderivative:
$$\int (x - x^2) \, dx = \frac{x^2}{2} - \frac{x^3}{3}$$

Evaluating from $0$ to $1$:
$$A = \left( \frac{1^2}{2} - \frac{1^3}{3} \right) - \left( 0 - 0 \right)$$
$$A = \frac{1}{2} - \frac{1}{3} = \frac{3}{6} - \frac{2}{6} = \frac{1}{6}$$

Thus, the area of the region is **$\frac{1}{6}$**.
