## Problem 10. A Cable Through Water and Land

Point $A$ lies on one bank of a river of width $100\text{ m}$, and point $B$ lies on the other bank, $500\text{ m}$ along the bank from the point directly opposite $A$.

The cost per meter of cable underwater is twice the cost per meter of cable on land.

Build a cost function depending on the point where the cable comes out of the water, determine the domain, and find the solution that minimizes the cost.

> Why this problem: it checks whether the student can independently translate a spatial description and two different costs into a single function to be optimized.

---

### Solution

#### 1. Setting up the Cost Function
Let:
* The point directly opposite $A$ on the other bank be $A'$.
* The distance from $A'$ to $B$ along the bank be $500\text{ m}$.
* The point where the cable emerges from the water onto $B$'s bank be $C$, located at a distance $x$ from $A'$ towards $B$.

This gives two segments for the cable:
1. **Underwater segment ($AC$):** Forms the hypotenuse of a right triangle with legs $100\text{ m}$ (river width) and $x$ (distance along the opposite bank):
   $$\text{Length of } AC = \sqrt{100^2 + x^2} = \sqrt{10000 + x^2}$$

2. **Land segment ($CB$):** Lies along the bank from $C$ to $B$:
   $$\text{Length of } CB = 500 - x$$

Let $k$ be the unit cost per meter of cable on land ($k > 0$). Then the cost per meter underwater is $2k$.

The total cost function $C(x)$ is:
$$C(x) = 2k \cdot \sqrt{10000 + x^2} + k \cdot (500 - x)$$

---

#### 2. Domain of the Function
The cable comes out of the water at some point between directly opposite $A$ ($x = 0$) and the destination point $B$ ($x = 500$). 

Thus, the domain is:
$$x \in [0, 500]$$

---

#### 3. Minimizing the Cost Function
To minimize $C(x)$, factor out the constant $k$ and differentiate with respect to $x$:

$$C'(x) = k \cdot \left( 2 \cdot \frac{1}{2\sqrt{10000 + x^2}} \cdot 2x - 1 \right) = k \cdot \left( \frac{2x}{\sqrt{10000 + x^2}} - 1 \right)$$

Set $C'(x) = 0$ to find the critical point (since $k \neq 0$):

$$\frac{2x}{\sqrt{10000 + x^2}} - 1 = 0$$
$$2x = \sqrt{10000 + x^2}$$

Square both sides:
$$4x^2 = 10000 + x^2$$
$$3x^2 = 10000$$
$$x^2 = \frac{10000}{3}$$
$$x = \frac{100}{\sqrt{3}} \approx 57.74\text{ m}$$

---

#### 4. Verification
Evaluating the cost function at the critical point and domain boundaries:

* **At $x = 0$
