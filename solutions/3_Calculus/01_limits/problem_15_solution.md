### Exercise 15. Observation Versus Proof

**Statement:**  
Choose one sequence and one function from this set. For the sequence, compute several values for increasingly large $n$. For the function, prepare a table of values with arguments approaching the limit point from the left and right. Sketch the behavior of both objects.

Compare the observation with the analytical result and explain why a finite number of calculations or a sketch does not constitute a proof that the limit exists.

> **Why this exercise:** teaches how to distinguish intuition and observation from mathematical argument.

---

### Solution

#### 1. Chosen Examples

* **Sequence:** $a_n = \left(1 + \frac{1}{n}\right)^n$ (from Exercise 5)
* **Function:** $f(x) = \frac{\sin x}{x}$ (from Exercise 13)

---

#### 2. Sequence Observation (Increasing $n$)

Computing terms of $a_n = \left(1 + \frac{1}{n}\right)^n$ for large values of $n$:

| $n$ | $a_n = \left(1 + \frac{1}{n}\right)^n$ |
| :--- | :--- |
| $1$ | $2.000000$ |
| $10$ | $2.593742$ |
| $100$ | $2.704814$ |
| $1,000$ | $2.716924$ |
| $10,000$ | $2.718146$ |
| $100,000$ | $2.718268$ |

**Observation:** The sequence values monotonically increase and approach the constant $e \approx 2.71828$.

---

#### 3. Function Table of Values (Approaching $x = 0$)

Preparing a table of values for $f(x) = \frac{\sin x}{x}$ as $x$ approaches $0$ from both sides:

| Left Approach ($x \to 0^-$) | $f(x)$ | Right Approach ($x \to 0^+$) | $f(x)$ |
| :--- | :--- | :--- | :--- |
| $x = -0.1$ | $0.998334$ | $x = 0.1$ | $0.998334$ |
| $x = -0.01$ | $0.999983$ | $x = 0.01$ | $0.999983$ |
| $x = -0.001$ | $0.9999998$ | $x = 0.001$ | $0.9999998$ |
| $x = -0.0001$ | $0.99999999$ | $x = 0.0001$ | $0.99999999$ |

**Observation:** As $x \to 0$ from both directions, $f(x)$ approaches $1$.

---

#### 4. Sketch of Behavior

* **Sequence Sketch ($a_n$ vs $n$):** Plotting points $(1, 2), (2, 2.25), (3, 2.37), \dots$ shows discrete points rising rapidly at first, then flattening out asymptotically toward the horizontal asymptote $y = e$.
* **Function Sketch ($f(x)$ vs $x$):** The curve $y = \frac{\sin x}{x}$ forms a symmetric bell-like shape centered at $x = 0$ with a maximum height of $1$ at $(0, 1)$ (represented with an open circle at $x = 0$ as the function is undefined there).

---

#### 5. Comparison: Observation vs. Analytical Proof

While empirical calculations and visual sketches build strong mathematical intuition, **they do not constitute a formal proof** for several key reasons:

1. **Finite Sampling vs. Infinite Domain:**  
   Numerical tables test only a finite subset of points. A limit statement like $\lim_{n \to \infty} a_n = L$ requires the behavior to hold across all infinitely many terms past a certain point, which cannot be verified by calculation alone.

2. **Deceptive Functions:**  
   Functions can appear well-behaved at selected sample points but oscillate wildly or diverge between them (e.g., $g(x) = \sin\left(\frac{1}{x}\right)$ equals zero at $x = \frac{1}{\pi k}$, masking its infinite oscillation near zero).

3. **Limits of Graphical Precision:**  
   Sketches and numerical calculations suffer from finite machine precision and visual scaling limits, making it impossible to distinguish between a true limit and a very slow change or temporary plateau.

4. **Necessity of Analytical Proof:**  
   Only rigorous analytical methods (such as $\varepsilon$-$N$ or $\varepsilon$-$\delta$ limit definitions, squeezing arguments, or algebraic transformations) provide absolute guarantees about the existence and exact value of a limit.
