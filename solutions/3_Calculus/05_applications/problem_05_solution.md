## Problem 5. Distance from Velocity

The velocity of a car during the first five seconds is described by the function

$$v(t) = 4t + 2 \quad [\text{m/s}].$$

Compute the distance traveled and explain why the integral of velocity gives the change in position.

Then answer what would have to be changed in the reasoning if the velocity also took negative values.

> Why this problem: it connects the integral with accumulation and distinguishes displacement from the actual distance traveled.

---

### Solution

#### 1. Distance Traveled Calculation
Since $v(t) = 4t + 2 > 0$ for all $t \in [0, 5]$, the car moves in a single direction without changing orientation. Therefore, the total distance traveled equals the displacement over the time interval $[0, 5]$:

$$s = \int_{0}^{5} (4t + 2) \, dt$$

Evaluating the antiderivative:
$$\int (4t + 2) \, dt = 2t^2 + 2t$$

Applying the limits from $0$ to $5$:
$$s = \left[ 2(5)^2 + 2(5) \right] - \left[ 2(0)^2 + 2(0) \right]$$
$$s = (2 \cdot 25 + 10) - 0 = 50 + 10 = 60\text{ meters}$$

Thus, the distance traveled is **$60\text{ meters}$**.

---

#### 2. Why the Integral of Velocity Gives Change in Position
The derivative of position $s(t)$ with respect to time is velocity, i.e., $s'(t) = v(t)$. 

By the **Fundamental Theorem of Calculus**, integrating a rate of change (velocity) over a time interval $[a, b]$ accumulates all the infinitesimal displacements $v(t)\,dt = \frac{ds}{dt}\,dt = ds$, yielding the net change in position (displacement):

$$\int_{a}^{b} v(t) \, dt = s(b) - s(a)$$

---

#### 3. Reasoning Adjustments if Velocity Takes Negative Values
If velocity takes negative values:
* **Displacement** (change in position) is still given directly by the integral of velocity:
  $$\text{Displacement} = \int_{a}^{b} v(t) \, dt$$
* **Total Distance Traveled** requires accumulating the magnitude of motion regardless of direction. To calculate total distance, one must integrate the absolute value of velocity (speed):
  $$\text{Total Distance} = \int_{a}^{b} |v(t)| \, dt$$

Practically, this means splitting the interval of integration at the points where $v(t) = 0$ and taking the absolute value of the integral on each sub-interval where $v(t) < 0$.
