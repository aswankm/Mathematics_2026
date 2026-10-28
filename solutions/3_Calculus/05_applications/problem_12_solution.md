## Problem 12. Complete Model and Computer Verification

A museum wants to create a rectangular exhibition room next to an existing straight wall. The side along the wall does not need to be built. The remaining three sides are to be constructed to two different standards: the two sides perpendicular to the wall cost 300 PLN/m each, while the side parallel to the wall costs 500 PLN/m. The budget is 30,000 PLN.

Build a model that maximizes the area of the room and prepare a complete analysis containing:
* definition of variables and units,
* mathematical model,
* domain resulting from the problem statement,
* computation of the derivative,
* determination and verification of the optimum,
* interpretation of the result,
* graph of the objective function,
* numerical verification of several values near the optimum found.

Finally, indicate which part of the solution required modeling the problem and which part was only the execution of the calculation. Produce the graph and computer calculations only after completing the mathematical solution, and treat them as verification.

> Why this problem: it checks full transfer to a new problem with unequal side costs and integrates the process from model construction to independent verification.

---

### Solution

#### 1. Definition of Variables and Units
* $x$: length of the side parallel to the wall $[\text{m}]$
* $y$: length of each of the two sides perpendicular to the wall $[\text{m}]$
* $A$: area of the rectangular exhibition room $[\text{m}^2]$
* $C$: total construction cost $[\text{PLN}]$

#### 2. Mathematical Model
* **Objective function (to maximize):**
  $$A(x, y) = x \cdot y$$

* **Cost constraint equation:**
  $$500x + 300y + 300y = 30\,000$$
  $$500x + 600y = 30\,000$$

  Expressing $y$ in terms of $x$:
  $$600y = 30\,000 - 500x \implies y = 50 - \frac{5}{6}x$$

* **Single-variable objective function:**
  $$A(x) = x\left(50 - \frac{5}{6}x\right) = 50x - \frac{5}{6}x^2$$

#### 3. Domain Resulting from the Problem Statement
Since the side lengths must be strictly positive:
* $x > 0$
* $y = 50 - \frac{5}{6}x > 0 \implies \frac{5}{6}x < 50 \implies x < 60$

Thus, the domain is:
$$x \in (0, 60)$$

#### 4. Computation of the Derivative
Taking the derivative of $A(x)$ with respect to $x$:

$$A'(x) = \frac{d}{dx}\left(50x - \frac{5}{6}x^2\right) = 50 - \frac{5}{3}x$$

#### 5. Determination and Verification of the Optimum
Set $A'(x) = 0$ to find the critical point:

$$50 - \frac{5}{3}x = 0 \implies \frac{5}{3}x = 50 \implies x = 30\text{ m}$$

Now calculate the corresponding value of $y$:

$$y = 50 - \frac{5}{6}(30) = 50 - 25 = 25\text{ m}$$

**Verification via Second Derivative Test:**
$$A''(x) = -\frac{5}{3} < 0$$

Since the second derivative is strictly negative everywhere on the domain, $x = 30\text{ m}$ is a strict local and global maximum.

The maximum area $A_{\text{max}}$ is:
$$A(30) = 30 \cdot 25 = 750\text{ m}^2$$

#### 6. Interpretation of the Result
To maximize the area given the non-uniform side costs, the museum should construct a room that is **$30\text{ m}$ wide** (parallel to the wall) and **$25\text{ m}$ deep** (perpendicular to the wall). Notice that the total budget is split equally: $500(30) = 15\,000\text{ PLN}$ for the parallel wall, and $600(25) = 15\,000\text{ PLN}$ for the two perpendicular walls combined.

---

### Computer Verification

#### 7. Numerical Verification Near the Optimum
Testing values of $x$ near $x = 30$ using $A(x) = 50x - \frac{5}{6}x^2$:

| Side $x$ (m) | Side $y = 50 - \frac{5}{6}x$ (m) | Total Cost (PLN) | Area $A(x)$ ($\text{m}^2$) | Status |
| :---: | :---: | :---: | :---: | :---: |
| $28.0$ | $26.67$ | $30\,000$ | $746.67$ | Below Optimum |
| $29.0$ | $25.83$ | $30\,000$ | $749.17$ | Below Optimum |
| **$30.0$** | **$25.00$** | **$30\,000$** | **$750.00$** | **OPTIMUM** |
| $31.0$ | $24.17$ | $30\,000$ | $749.17$ | Below Optimum |
| $32.0$ | $23.33$ | $30\,000$ | $746.67$ | Below Optimum |

The table confirms that any deviation from $x = 30\text{ m}$ reduces the enclosed area.

#### 8. Graph of the Objective Function
The area function $A(x) = -\frac{5}{6}x^2 + 50x$ represents a downward-opening parabola with roots at $x = 0$ and $x = 60$, and its peak (vertex) located at $(30, 750)$.
