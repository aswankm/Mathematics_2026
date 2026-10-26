### Exercise 13. Fundamental Trigonometric Limit

**Statement:**  
Using

$$
\lim_{x \to 0} \frac{\sin x}{x} = 1,
$$

compute

$$
\lim_{x \to 0} \frac{\sin 5x}{x}, \qquad \lim_{x \to 0} \frac{\sin 2x}{\sin 3x}.
$$

In each case, show how you reduce the expression to the fundamental limit
> **Why this exercise:** teaches how to reduce new limits to one known pattern

---

### Solution

#### 1. First Limit: $\lim_{x \to 0} \frac{\sin 5x}{x}$
To apply the fundamental limit $\lim_{u \to 0} \frac{\sin u}{u} = 1$, the argument inside the sine function must match the denominator. 

Multiply and divide the expression by $5$:

$$
\lim_{x \to 0} \frac{\sin 5x}{x} = \lim_{x \to 0} 5 \cdot \frac{\sin 5x}{5x}
$$

Let $u = 5x$. As $x \to 0$, $u \to 0$. Applying this substitution:

$$
= 5 \cdot \lim_{u \to 0} \frac{\sin u}{u}
$$

Since $\lim_{u \to 0} \frac{\sin u}{u} = 1$, we obtain:

$$
= 5 \cdot 1 = 5
$$

---

#### 2. Second Limit: $\lim_{x \to 0} \frac{\sin 2x}{\sin 3x}$
Divide both the numerator and the denominator by $x$ to introduce the fundamental limit pattern:

$$
\lim_{x \to 0} \frac{\sin 2x}{\sin 3x} = \lim_{x \to 0} \frac{\frac{\sin 2x}{x}}{\frac{\sin 3x}{x}}
$$

Adjust the numerator and denominator by introducing factors of $2$ and $3$:

$$
= \lim_{x \to 0} \frac{2 \cdot \frac{\sin 2x}{2x}}{3 \cdot \frac{\sin 3x}{3x}}
$$

Let $u = 2x$ and $v = 3x$. As $x \to 0$, both $u \to 0$ and $v \to 0$:

$$
= \frac{2 \cdot \lim_{u \to 0} \frac{\sin u}{u}}{3 \cdot \lim_{v \to 0} \frac{\sin v}{v}}
$$

Evaluating the fundamental limits gives:

$$
= \frac{2 \cdot 1}{3 \cdot 1} = \frac{2}{3}
$$
