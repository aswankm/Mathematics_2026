## Problem 9. An Oblique Asymptote[cite: 3]

Analyze the asymptotes of[cite: 3]

$$f(x) = \frac{x^2 + 1}{x - 1}[cite: 3]$$

Perform polynomial division and explain why the remainder term vanishes for large $|x|$[cite: 3].

> **Why this problem:** it teaches how to recognize an oblique asymptote and interpret the decomposition of a function[cite: 3].

---

## Solution

### 1. Polynomial Division[cite: 3]
To analyze the function and its behavior for large values, we perform polynomial division on $f(x) = \frac{x^2 + 1}{x - 1}$[cite: 3]:
$$f(x) = x + 1 + \frac{2}{x - 1}[cite: 3]$$

### 2. Asymptote Analysis[cite: 3]
* **Vertical Asymptote:** The denominator equals zero when $x - 1 = 0$, giving **$x = 1$**[cite: 3].
* **Oblique (Slant) Asymptote:** As $|x| \to \infty$, the remainder term $\frac{2}{x - 1}$ approaches zero[cite: 3]. 
  $$\lim_{|x| \to \infty} \frac{2}{x - 1} = 0[cite: 3]$$
  Therefore, the graph approaches the linear function described by the quotient[cite: 3].
  * **Oblique Asymptote:** **$y = x + 1$**[cite: 3]

### 3. Explanation of the Remainder Term[cite: 3]
The remainder term $\frac{2}{x - 1}$ vanishes for large $|x|$ because the denominator grows infinitely larger in magnitude than the constant numerator ($2$), driving the overall fraction to zero[cite: 3]. This demonstrates that the curve closely approximates the line $y = x + 1$ as $x$ moves toward positive or negative infinity[cite: 3].
