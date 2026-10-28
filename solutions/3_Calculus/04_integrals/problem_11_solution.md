## Problem 11. Choose the Method First

**Statement:**
For each integral, first write which method you choose and how you recognize it, and then compute:

1. $\int \sin(3x) \, dx$
2. $\int x \ln x \, dx$
3. $\int \frac{x}{\sqrt{x^2+1}} \, dx$

> **Why this problem:** it tests the choice of method based on the structure of the problem.

---

### Solution

#### Part 1: $\int \sin(3x) \, dx$

* **Method Chosen:** Substitution (or direct reverse chain rule).
* **Recognition:** The integrand is a simple composite function where the inner function $u = 3x$ has a constant derivative ($3$), meaning its differential differs from $dx$ by only a scaling constant.

**Computation:**
Let $u = 3x \implies du = 3 \, dx \implies dx = \frac{du}{3}$.

$$\int \sin(3x) \, dx = \int \sin(u) \cdot \frac{du}{3} = \frac{1}{3} \int \sin(u) \, du$$
$$= -\frac{1}{3} \cos(u) + C = -\frac{1}{3} \cos(3x) + C$$

---

#### Part 2: $\int x \ln x \, dx$

* **Method Chosen:** Integration by Parts.
* **Recognition:** The integrand is a product of two different types of functions—an algebraic function ($x$) and a logarithmic function ($\ln x$)—with no derivative-pair relationship between them.

**Computation:**
Using $\int u \, dv = uv - \int v \, du$:
* Let $u = \ln x \implies du = \frac{1}{x} \, dx$ (logarithmic function is easy to differentiate).
* Let $dv = x \, dx \implies v = \frac{x^2}{2}$.

$$\int x \ln x \, dx = (\ln x)\left(\frac{x^2}{2}\right) - \int \left(\frac{x^2}{2}\right) \left(\frac{1}{x}\right) dx$$
$$= \frac{x^2 \ln x}{2} - \frac{1}{2} \int x \, dx$$
$$= \frac{x^2 \ln x}{2} - \frac{1}{2} \left( \frac{x^2}{2} \right) + C = \frac{x^2 \ln x}{2} - \frac{x^2}{4} + C$$

---

#### Part 3: $\int \frac{x}{\sqrt{x^2+1}} \, dx$

* **Method Chosen:** Substitution.
* **Recognition:** The numerator $x$ is (up to a constant multiplier) the exact derivative of the inner function inside the square root in the denominator, $x^2+1$.

**Computation:**
Let $u = x^2 + 1 \implies du = 2x \, dx \implies x \, dx = \frac{du}{2}$.

$$\int \frac{x}{\sqrt{x^2+1}} \, dx = \int \frac{\frac{1}{2} du}{\sqrt{u}} = \frac{1}{2} \int u^{-1/2} \, du$$
$$= \frac{1}{2} \left( \frac{u^{1/2}}{1/2} \right) + C = \sqrt{u} + C$$
$$= \sqrt{x^2 + 1} + C$$
