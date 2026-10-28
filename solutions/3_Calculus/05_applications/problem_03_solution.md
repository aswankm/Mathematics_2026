## Problem 3. A Box Made from Cardboard

From a $30\text{ cm} \times 40\text{ cm}$ sheet, squares of side length $x$ are cut from the corners and the edges are folded up to form an open box.
Write the volume as a function of $x$, determine the physically meaningful domain, and find the value of $x$ for which the volume is greatest.

> Why this problem: it develops optimization modeling in a situation where the objective function is not given and must be built.

---

### Solution

#### 1. Volume as a Function of $x$
When squares of side length $x$ are cut from each of the four corners of the rectangular sheet:
* The new width of the box becomes: $30 - 2x$
* The new length of the box becomes: $40 - 2x$
* The height of the box is: $x$

The volume $V$ of the box is given by length $\times$ width $\times$ height:
$$V(x) = x(30 - 2x)(40 - 2x)$$

Expanding the expression:
$$V(x) = x(1200 - 60x - 80x + 4x^2) = x(1200 - 140x + 4x^2) = 4x^3 - 140x^2 + 1200x$$

---

#### 2. Physically Meaningful Domain
For the dimensions of the box to be physically positive:
1. $x > 0$
2. $30 - 2x > 0 \implies 2x < 30 \implies x < 15$
3. $40 - 2x > 0 \implies 2x < 40 \implies x < 20$

Taking the intersection of these conditions, the domain is:
$$x \in (0, 15)$$

---

#### 3. Value of $x$ for Maximum Volume
To find the critical points, take the first derivative of $V(x)$ with respect to $x$:
$$V'(x) = \frac{d}{dx}(4x^3 - 140x^2 + 1200x) = 12x^2 - 280x + 1200$$

Set $V'(x) = 0$ to find critical values:
$$12x^2 - 280x + 1200 = 0$$

Divide the entire equation by $4$:
$$3x^2 - 70x + 300 = 0$$

Using the quadratic formula $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$:
$$x = \frac{70 \pm \sqrt{(-70)^2 - 4(3)(300)}}{2(3)} = \frac{70 \pm \sqrt{4900 - 3600}}{6} = \frac{70 \pm \sqrt{1300}}{6}$$

$$\sqrt{1300} \approx 36.055$$

This gives two possible solutions:
* $x_1 = \frac{70 + 36.055}{6} = \frac{106.055}{6} \approx 17.68$ (Outside the domain $(0, 15)$)
* $x_2 = \frac{70 - 36.055}{6} = \frac{33.945}{6} \approx 5.66$ (Inside the domain)

Thus, the value of $x$ that maximizes the volume is approximately **$5.66\text{ cm}$** (or exactly $\frac{35 - \sqrt{325}}{3}\text{ cm}$).

---

#### 4. Justification of Maximum
Using the second derivative test:
$$V''(x) = \frac{d}{dx}(12x^2 - 280x + 1200) = 24x - 280$$

Evaluating at $x \approx 5.66$:
$$V''(5.66) = 24(5.66) - 280 = 135.84 - 280 = -144.16 < 0$$

Since the second derivative is negative at the critical point, the volume is maximized at **$x \approx 5.66\text{ cm}$**.
