# Exercise. Closest Point on a Line via Projection

### Statement & Solution Overview

**Question:**  
For $P = (4, 1)$ and the line through the origin in direction $v = (1, 2)$, find the closest point and distance using projection, and verify the relevant perpendicularity.

---

### Solution

#### 1. Find the Closest Point ($Q$)
The closest point is the orthogonal projection of $P$ onto the line direction vector $v$:
$$
Q = \text{proj}_v P = \frac{P \cdot v}{v \cdot v} v = \frac{6}{5}(1, 2) = \left(\frac{6}{5}, \frac{12}{5}\right)
$$

#### 2. Compute the Distance
The displacement vector from the closest point $Q$ to $P$ is:
$$
P - Q = (4, 1) - \left(\frac{6}{5}, \frac{12}{5}\right) = \left(\frac{14}{5}, -\frac{7}{5}\right)
$$

Thus, the distance is:
$$
\|P - Q\| = \sqrt{\left(\frac{14}{5}\right)^2 + \left(-\frac{7}{5}\right)^2} = \sqrt{\frac{196 + 49}{25}} = \sqrt{\frac{245}{25}} = \sqrt{\frac{49}{5}} = \frac{7}{\sqrt{5}}
$$

#### 3. Verify Perpendicularity
The dot product between the displacement vector and the line direction vector $v$ is:
$$
(P - Q) \cdot v = \left(\frac{14}{5}, -\frac{7}{5}\right) \cdot (1, 2) = \frac{14}{5}(1) + \left(-\frac{7}{5}\right)(2) = \frac{14}{5} - \frac{14}{5} = 0
$$

#### 4. Geometric Explanation
Since $(P - Q) \cdot v = 0$, the displacement vector from $Q$ to $P$ is perpendicular to the line direction $v$. A perpendicular segment always provides the shortest possible distance from a point to a line, confirming that $Q$ is indeed the closest point on the line.
