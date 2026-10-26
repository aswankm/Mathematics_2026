### Exercise 2. A Line in Space

**Statement:**
Given

$$
L : (x, y, z) = (2, -1, 3) + t(1, 2, -2).
$$

State a point on the line and its direction vector, check whether $P = (4, 3, -1)$ lies on $L$, and find the point corresponding to $t = -1$.

---

### Solution

#### 1. Point on the Line and Direction Vector
From the vector equation of the line $L: (x, y, z) = (2, -1, 3) + t(1, 2, -2)$:
- **Point on the line:** $A = (2, -1, 3)$ (obtained by setting $t = 0$)
- **Direction vector:** $\vec{v} = (1, 2, -2)$

#### 2. Checking if $P = (4, 3, -1)$ Lies on $L$
To check whether $P$ lies on $L$, we substitute the coordinates of $P$ into the parametric equation $(x, y, z) = (2 + t, -1 + 2t, 3 - 2t)$ and check for a consistent scalar $t$:

1. $x$-component: $4 = 2 + t \implies t = 2$
2. $y$-component: $3 = -1 + 2t \implies 2t = 4 \implies t = 2$
3. $z$-component: $-1 = 3 - 2t \implies -2t = -4 \implies t = 2$

Since $t = 2$ satisfies all three coordinate equations, **$P = (4, 3, -1)$ lies on $L$**.

#### 3. Finding the Point Corresponding to $t = -1$
Substitute $t = -1$ into the equation of the line:

$$
(x, y, z) = (2, -1, 3) + (-1)(1, 2, -2)
$$

$$
(x, y, z) = (2 - 1, -1 - 2, 3 + 2) = (1, -3, 5)
$$

The point corresponding to $t = -1$ is **$(1, -3, 5)$**.
