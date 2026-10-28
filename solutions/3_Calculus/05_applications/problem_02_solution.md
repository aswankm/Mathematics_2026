## Problem 2. Maximum Area of a Rectangle

A rectangle has perimeter 40.

1. Write its area as a function of the length of one side.
2. Determine the domain of this function resulting from the geometry of the problem.
3. Find the dimensions that give the maximum area.
4. Justify that the point found actually gives a maximum.

> Why this problem: it teaches the complete optimization scheme: model $\to$ domain $\to$ derivative $\to$ verification and interpretation of the maximum.

---

### Solution

#### 1. Area as a Function of One Side
Let the sides of the rectangle be $x$ and $y$. 

The perimeter formula is:
$$2x + 2y = 40 \implies x + y = 20 \implies y = 20 - x$$

The area $A$ of the rectangle is given by $A = x \cdot y$. Expressing area as a function of $x$:
$$A(x) = x(20 - x) = 20x - x^2$$

---

#### 2. Domain of the Function
Since side lengths must be strictly positive:
* $x > 0$
* $y = 20 - x > 0 \implies x < 20$

Thus, the geometrically meaningful domain is:
$$x \in (0, 20)$$

---

#### 3. Dimensions for Maximum Area
To find the critical points, take the first derivative of $A(x)$ with respect to $x$ and set it to zero:
$$A'(x) = \frac{d}{dx}(20x - x^2) = 20 - 2x$$

Setting $A'(x) = 0$:
$$20 - 2x = 0 \implies 2x = 20 \implies x = 10$$

Calculating the other side $y$:
$$y = 20 - 10 = 10$$

The dimensions that maximize the area are **$10 \times 10$** (a square).

---

#### 4. Justification of Maximum
Using the **Second Derivative Test**:
$$A''(x) = \frac{d}{dx}(20 - 2x) = -2$$

Since $A''(10) = -2 < 0$, the function is strictly concave down on its domain, which guarantees that $x = 10$ gives a **local and absolute maximum**.
