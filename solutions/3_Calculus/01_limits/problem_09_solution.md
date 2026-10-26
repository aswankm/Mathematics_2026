### Exercise 9. One-Sided Limits and an Asymptote

**Statement:**  
Analyze the left-hand and right-hand limits of[cite: 3]

$$
f(x) = \frac{1}{x - 2}
$$

as $x \to 2$[cite: 3]. Does the two-sided limit exist? Interpret the result on a sketch of the graph and identify the vertical asymptote[cite: 3].

> **Why this exercise:** teaches how to distinguish one-sided limits and connect them with the geometry of an asymptote[cite: 3].

---

### Solution

#### 1. Analysis of One-Sided Limits as $x \to 2$

* **Left-Hand Limit ($x \to 2^-$):**  
  As $x$ approaches $2$ from values strictly less than $2$ (e.g., $1.9, 1.99, 1.999$), the denominator $(x - 2)$ is a very small negative number, while the numerator is $1$. Therefore, the quotient grows negatively without bound:
  
$$
  \lim_{x \to 2^-} \frac{1}{x - 2} = -\infty
$$

* **Right-Hand Limit ($x \to 2^+$):**  
  As $x$ approaches $2$ from values strictly greater than $2$ (e.g., $2.1, 2.01, 2.001$), the denominator $(x - 2)$ is a very small positive number, while the numerator is $1$. Therefore, the quotient grows positively without bound:
  
$$
  \lim_{x \to 2^+} \frac{1}{x - 2} = +\infty
$$

---

#### 2. Existence of the Two-Sided Limit
For a two-sided limit $\lim_{x \to a} f(x)$ to exist, both the left-hand and right-hand limits must exist and be equal to the same finite real number. 

In this case:
- The left-hand limit is $-\infty$.
- The right-hand limit is $+\infty$.

Since these one-sided limits are unequal (and neither is a finite number), the **two-sided limit $\lim_{x \to 2} \frac{1}{x - 2}$ does not exist**.

---

#### 3. Vertical Asymptote and Graphical Interpretation
* **Vertical Asymptote:** Because the function values increase or decrease without bound as $x$ approaches $2$, the line **$x = 2$** is a **vertical asymptote** of the graph.
* **Graphical Interpretation:** On a sketch of the function $f(x) = \frac{1}{x - 2}$ (which is a standard hyperbola shifted 2 units to the right):
  * To the left of $x = 2$, the curve plummets downward toward $-\infty$.
  * To the right of $x = 2$, the curve shoots upward toward $+\infty$.
  * The graph never touches or crosses the vertical line $x = 2$.
