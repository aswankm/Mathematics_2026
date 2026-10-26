### Exercise 6. Angle Between Planes

**Statement:** 
Given

$$
\Pi_1: x + y + z = 1, \quad \Pi_2: x - y = 2.
$$

First use the normal vectors to decide whether the planes are parallel. If not, compute the angle between them and explain why the normal vectors alone are enough for this calculation.

> **Why this exercise:** focuses attention on one mechanism—using normals to analyze position and angle—without also introducing the construction of the intersection line.

---

### Solution

#### 1. Identify the Normal Vectors
The normal vectors $\vec{n}_1$ and $\vec{n}_2$ are extracted directly from the coefficients of the plane equations:

$$
\vec{n}_1 = (1, 1, 1)
$$

$$
\vec{n}_2 = (1, -1, 0)
$$

#### 2. Check for Parallelism
Two planes are parallel if and only if their normal vectors are proportional ($\vec{n}_1 = k \vec{n}_2$ for some scalar $k$):

- $1 = k \cdot 1 \implies k = 1$
- $1 = k \cdot (-1) \implies k = -1$

Since there is no single scalar $k$ satisfying the relationship, the normal vectors are not parallel. Therefore, **the planes $\Pi_1$ and $\Pi_2$ are not parallel**.

#### 3. Compute the Angle Between the Planes
The angle $\theta$ between two planes is defined as the acute angle between their normal vectors, calculated using the formula:

$$
\cos \theta = \frac{|\vec{n}_1 \cdot \vec{n}_2|}{\|\vec{n}_1\| \|\vec{n}_2\|}
$$

1. **Calculate the Dot Product ($\vec{n}_1 \cdot \vec{n}_2$):**

$$
\vec{n}_1 \cdot \vec{n}_2 = (1)(1) + (1)(-1) + (1)(0) = 1 - 1 + 0 = 0
$$

2. **Calculate the Magnitudes ($\|\vec{n}_1\|$ and $\|\vec{n}_2\|$):**

$$
\|\vec{n}_1\| = \sqrt{1^2 + 1^2 + 1^2} = \sqrt{3}
$$

$$
\|\vec{n}_2\| = \sqrt{1^2 + (-1)^2 + 0^2} = \sqrt{2}
$$

3. **Calculate $\cos \theta$ and $\theta$:**

$$
\cos \theta = \frac{|0|}{\sqrt{3} \cdot \sqrt{2}} = 0
$$

$$
\theta = \arccos(0) = \frac{\pi}{2} \text{ rad} \quad (90^\circ)
$$

The angle between the planes is **$90^\circ$** (the planes are perpendicular).

#### 4. Explanation: Why Normal Vectors are Sufficient
The angle between two planes is geometrically defined by how their respective orientations tilt relative to one another in 3D space. 

Since normal vectors are perpendicular to their corresponding planes, rotating the planes preserves the exact relative angular difference between the planes themselves and their normal vectors. Thus, measuring the angle between $\vec{n}_1$ and $\vec{n}_2$ directly yields the angle between $\Pi_1$ and $\Pi_2$ without needing to find or construct their line of intersection.
