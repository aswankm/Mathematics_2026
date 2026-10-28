## Problem 9. Minimizing the Material Used for a Can

A closed cylinder has fixed volume $V$.

1. Write the volume constraint.
2. Eliminate one of the variables.
3. Express the surface area as a function of the radius $r$.
4. Find the relation between the height $h$ and the radius $r$ for which the material usage is minimal.

Interpret the obtained relation geometrically.

> Why this problem: it requires independent reduction of a problem with two variables to one objective function and control of the geometric constraint.

---

### Solution

#### 1. Volume Constraint
Let $r$ be the radius of the base and $h$ be the height of the cylinder. The volume $V$ of a closed cylinder is:

$$V = \pi r^2 h$$

---

#### 2. Eliminating One Variable
We express height $h$ in terms of the fixed volume $V$ and radius $r$:

$$h = \frac{V}{\pi r^2}$$

---

#### 3. Surface Area as a Function of Radius $r$
The total surface area $A$ of a closed cylinder consists of two circular bases and the lateral surface area:

$$A = 2\pi r^2 + 2\pi r h$$

Substituting $h = \frac{V}{\pi r^2}$ into the area equation:

$$A(r) = 2\pi r^2 + 2\pi r \left( \frac{V}{\pi r^2} \right) = 2\pi r^2 + \frac{2V}{r}$$

---

#### 4. Height to Radius Relation for Minimal Material Usage
To find the radius $r$ that minimizes surface area, take the first derivative of $A(r)$ with respect to $r$ and set it to zero:

$$A'(r) = \frac{d}{dr}\left(2\pi r^2 + 2V r^{-1}\right) = 4\pi r - \frac{2V}{r^2}$$

Set $A'(r) = 0$:

$$4\pi r - \frac{2V}{r^2} = 0 \implies 4\pi r^3 = 2V \implies V = 2\pi r^3$$

Now, substitute $V = \pi r^2 h$ into $V = 2\pi r^3$:

$$\pi r^2 h = 2\pi r^3$$

Dividing both sides by $\pi r^2$ (since $r > 0$):

$$h = 2r$$

#### Geometric Interpretation:
Material usage is minimized when the height of the cylinder is equal to its diameter ($h = 2r$), meaning the cross-section passing through the central vertical axis forms a square.
