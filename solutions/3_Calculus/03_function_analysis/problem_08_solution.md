## Problem 8. The Second Derivative[cite: 3]

For[cite: 3]

$$f(x) = x^4 - 4x^2[cite: 3]$$

find the local extrema, intervals of convexity and concavity, and inflection points. Sketch the graph and mark all the identified features on it[cite: 3].

> **Why this problem:** it introduces the second derivative as a tool for describing the curvature of a graph[cite: 3].

---

## Solution

### 1. First Derivative & Extrema[cite: 3]
Compute the first derivative:[cite: 3]
$$f'(x) = 4x^3 - 8x = 4x(x^2 - 2)[cite: 3]$$

Set $f'(x) = 0$ to find critical points:[cite: 3]
$$4x(x^2 - 2) = 0 \implies x = 0, \, x = -\sqrt{2}, \, x = \sqrt{2}[cite: 3]$$

Evaluate the function at these critical points:[cite: 3]
* For $x = -\sqrt{2}$: $f(-\sqrt{2}) = (-\sqrt{2})^4 - 4(-\sqrt{2})^2 = 4 - 8 = -4 \implies \mathbf{(-\sqrt{2}, -4)}$ (Local Minimum)[cite: 3]
* For $x = 0$: $f(0) = 0^4 - 4(0)^2 = 0 \implies \mathbf{(0, 0)}$ (Local Maximum)[cite: 3]
* For $x = \sqrt{2}$: $f(\sqrt{2}) = (\sqrt{2})^4 - 4(\sqrt{2})^2 = 4 - 8 = -4 \implies \mathbf{(\sqrt{2}, -4)}$ (Local Minimum)[cite: 3]

### 2. Second Derivative & Concavity[cite: 3]
Compute the second derivative:[cite: 3]
$$f''(x) = \frac{d}{dx}(4x^3 - 8x) = 12x^2 - 8 = 4(3x^2 - 2)[cite: 3]$$

Set $f''(x) = 0$ to find potential inflection points:[cite: 3]
$$4(3x^2 - 2) = 0 \implies 3x^2 = 2 \implies x^2 = \frac{2}{3} \implies x = \pm\sqrt{\frac{2}{3}} = \pm\frac{\sqrt{6}}{3}[cite: 3]$$

Test concavity on intervals partitioned by $x = -\frac{\sqrt{6}}{3}$ and $x = \frac{\sqrt{6}}{3}$:[cite: 3]
* **Concave Up ($f''(x) > 0$):** $\left(-\infty, -\frac{\sqrt{6}}{3}\right) \cup \left(\frac{\sqrt{6}}{3}, \infty\right)$[cite: 3]
* **Concave Down ($f''(x) < 0$):** $\left(-\frac{\sqrt{6}}{3}, \frac{\sqrt{6}}{3}\right)$[cite: 3]

### 3. Inflection Points[cite: 3]
Evaluate $f(x)$ at the inflection coordinates:[cite: 3]
$$f\left(\pm\frac{\sqrt{6}}{3}\right) = \left(\pm\frac{\sqrt{6}}{3}\right)^4 - 4\left(\pm\frac{\sqrt{6}}{3}\right)^2 = \frac{36}{81} - 4\left(\frac{6}{9}\right) = \frac{4}{9} - \frac{8}{3} = -\frac{20}{9}$$

* **Inflection Points:** $\mathbf{\left(-\frac{\sqrt{6}}{3}, -\frac{20}{9}\right)}$ and $\mathbf{\left(\frac{\sqrt{6}}{3}, -\frac{20}{9}\right)}$[cite: 3]
