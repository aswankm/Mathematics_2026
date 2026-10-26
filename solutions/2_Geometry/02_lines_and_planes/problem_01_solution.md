### Exercise 1. Line Through Two Points

**Statement:**
Find the equation of the line through $A = (1, 2)$ and $B = (4, -1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

---

### Solution

#### 1. Direction Vector ($\vec{v}$)
The direction vector of the line passing through points $A$ and $B$ is given by the vector $\vec{AB}$:

$$
\vec{v} = \vec{AB} = B - A = (4 - 1, -1 - 2) = (3, -3)
$$

*(Note: This can also be simplified to $\vec{v} = (1, -1)$).*

#### 2. Parametric Form
Using the point $A = (1, 2)$ and the direction vector $\vec{v} = (3, -3)$, the parametric equations for the line are:

$$
x = 1 + 3t
$$

$$
y = 2 - 3t \quad (t \in \mathbb{R})
$$

#### 3. General Form

To find the general form ($Ax + By + C = 0$), we eliminate the parameter $t$ from the parametric equations:
From $x = 1 + 3t$, we solve for $t$:
$$t = \frac{x - 1}{3}$$
Substitute this into the $y$ equation:
$$y = 2 - 3\left(\frac{x - 1}{3}\right) = 2 - (x - 1) = 3 - x$$
Rearranging terms gives the general form:

$$
x + y - 3 = 0
$$

#### 4. Normal Vector ($\vec{n}$)
From the general form $1x + 1y - 3 = 0$, the normal vector is:

$$
\vec{n} = (1, 1)
$$

*(Verification: The dot product of the direction vector and normal vector must be zero: $\vec{v} \cdot \vec{n} = (3)(1) + (-3)(1) = 0$.)*

#### 5. Verification
Let's check if both points satisfy the general equation $x + y - 3 = 0$:
* **For point $A = (1, 2)$:**

$$
  1 + 2 - 3 = 0 \quad (\text{True})
$$

* **For point $B = (4, -1)$:**

$$
4 + (-1) - 3 = 0 \quad (\text{True})
$$
