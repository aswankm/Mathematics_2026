## Exercise: Limit of an Exponential Expression

**Compute[cite: 1]:**
$$\lim_{n \to \infty} \sqrt{5^n + 2^n}$$

* **Additional Question[cite: 1]:** Explain which term dominates and why the transformation looks different from the case of a quotient of polynomials.
* **Why this exercise[cite: 1]:** Extends the idea of dominance to exponential expressions.

---

### Solution

1. **Identify the dominant term:** 
   Inside the square root, $5^n$ grows exponentially faster than $2^n$ as $n \to \infty$ because $5 > 2$. Thus, $5^n$ is the dominant term.

2. **Factor out the dominant term:**
   $$\sqrt{5^n + 2^n} = \sqrt{5^n \left(1 + \left(\frac{2}{5}\right)^n\right)}$$

3. **Simplify using exponent and radical rules:**
   $$= \sqrt{5^n} \cdot \sqrt{1 + \left(\frac{2}{5}\right)^n} = 5^{n/2} \sqrt{1 + \left(\frac{2}{5}\right)^n}$$

4. **Evaluate the limit as $n \to \infty$:**
   * Since $0 < \frac{2}{5} < 1$, the ratio term vanishes: $\left(\frac{2}{5}\right)^n \to 0$.
   * The radical part approaches: $\sqrt{1 + 0} = 1$.
   * The outside exponential term grows without bound: $5^{n/2} = (\sqrt{5})^n \to \infty$.

$$\lim_{n \to \infty} 5^{n/2} \sqrt{1 + \left(\frac{2}{5}\right)^n} = \infty \cdot 1 = \infty$$

* **Why the transformation looks different from a quotient of polynomials:** In rational functions (quotients of polynomials), dividing by the highest power normalizes the expression into constants. Here, factoring out the dominant exponential term from underneath a square root leaves a fractional power ($5^{n/2}$) outside, which continues to diverge to infinity rather than reducing to a finite constant coefficient.
