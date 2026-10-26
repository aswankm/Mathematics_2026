### Exercise 15. Complete Classification of a Line Relative to a Plane

**Statement:**  
Let

$$
L: \mathbf{p} + t\mathbf{v}, \quad \Pi: \mathbf{n} \cdot \mathbf{x} = d.
$$

State the conditions distinguishing the three cases: one intersection point, parallel with no common points, and the line contained in the plane. Then illustrate each case with your own simple numerical example.

> **Why this exercise:** requires formulating a general mathematical criterion instead of carrying out one isolated calculation.

---

### Solution

#### 1. General Mathematical Conditions

Given a line $L: \mathbf{x}(t) = \mathbf{p} + t\mathbf{v}$ and a plane $\Pi: \mathbf{n} \cdot \mathbf{x} = d$:

Substitute the equation of the line into the plane equation:

$$
\mathbf{n} \cdot (\mathbf{p} + t\mathbf{v}) = d \implies (\mathbf{n} \cdot \mathbf{p}) + t(\mathbf{n} \cdot \mathbf{v}) = d \implies t(\mathbf{n} \cdot \mathbf{v}) = d - \mathbf{n} \cdot \mathbf{p}
$$

The three possible geometric cases depend on the values of $\mathbf{n} \cdot \mathbf{v}$ and $d - \mathbf{n} \cdot \mathbf{p}$:

1. **Case 1: Exactly One Intersection Point**
   * **Condition:** $\mathbf{n} \cdot \mathbf{v} \neq 0$
   * **Geometric Meaning:** The direction vector of the line is not perpendicular to the normal vector of the plane, meaning the line penetrates the plane at a single point.
   * **Parameter:** $t = \frac{d - \mathbf{n} \cdot \mathbf{p}}{\mathbf{n} \cdot \mathbf{v}}$

2. **Case 2: Parallel with No Common Points (Strictly Parallel)**
   * **Condition:** $\mathbf{n} \cdot \mathbf{v} = 0$ AND $\mathbf{n} \cdot \mathbf{p} \neq d$
   * **Geometric Meaning:** The line's direction is parallel to the plane surface ($\mathbf{n} \cdot \mathbf{v} = 0$), but its base point $\mathbf{p}$ does not lie on the plane ($\mathbf{n} \cdot \mathbf{p} \neq d$). The equation $0 \cdot t = \text{nonzero}$ has no solutions.

3. **Case 3: Line Contained in the Plane**
   * **Condition:** $\mathbf{n} \cdot \mathbf{v} = 0$ AND $\mathbf{n} \cdot \mathbf{p} = d$
   * **Geometric Meaning:** The line is parallel to the plane surface ($\mathbf{n} \cdot \mathbf{v} = 0$), and its base point $\mathbf{p}$ lies on the plane ($\mathbf{n} \cdot \mathbf{p} = d$). The equation $0 \cdot t = 0$ is satisfied for all $t \in \mathbb{R}$.

---

#### 2. Numerical Examples

Consider the fixed plane $\Pi: x + y + z = 1$, which has normal vector $\mathbf{n} = (1, 1, 1)$ and constant $d = 1$.

* **Example for Case 1 (One Intersection Point):**
  * Let $L_1: (0, 0, 0) + t(1, 0, 0)$ with $\mathbf{p} = (0, 0, 0)$ and $\mathbf{v} = (1, 0, 0)$.
  * **Check:** $\mathbf{n} \cdot \mathbf{v} = (1, 1, 1) \cdot (1, 0, 0) = 1 \neq 0$.
  * **Result:** Solving $t(1) = 1 - 0 \implies t = 1$, giving the single intersection point $(1, 0, 0)$.

* **Example for Case 2 (Parallel with No Common Points):**
  * Let $L_2: (0, 0, 2) + t(1, -1, 0)$ with $\mathbf{p} = (0, 0, 2)$ and $\mathbf{v} = (1, -1, 0)$.
  * **Check:** 
    * $\mathbf{n} \cdot \mathbf{v} = (1, 1, 1) \cdot (1, -1, 0) = 1 - 1 + 0 = 0$.
    * $\mathbf{n} \cdot \mathbf{p} = (1, 1, 1) \cdot (0, 0, 2) = 2 \neq 1$.
  * **Result:** Substituting into the plane yields $0 + 2 = 1 \implies 2 = 1$ (contradiction, no common points).

* **Example for Case 3 (Line Contained in the Plane):**
  * Let $L_3: (1, 0, 0) + t(1, -1, 0)$ with $\mathbf{p} = (1, 0, 0)$ and $\mathbf{v} = (1, -1, 0)$.
  * **Check:** 
    * $\mathbf{n} \cdot \mathbf{v} = (1, 1, 1) \cdot (1, -1, 0) = 1 - 1 + 0 = 0$.
    * $\mathbf{n} \cdot \mathbf{p} = (1, 1, 1) \cdot (1, 0, 0) = 1 = d$.
  * **Result:** Substituting into the plane yields $(1 + t) + (-t) + 0 = 1 \implies 1 = 1$ (true for all $t$, the line lies in the plane).
  * 
