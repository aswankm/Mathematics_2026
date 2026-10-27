## Problem 8. Two Exponential Functions

### Statement

For 

$$f(x) = e^{2x - 3} + 5^x$$

Compute the derivative. Explain why the factor 2 appears in the first term and why $\ln 5$ appears in the second[cite: 6].

* **Why this problem:** It organizes two different mechanisms that produce additional factors[cite: 6].

---

### Solution

#### 1. Compute the derivative
Differentiate each term separately[cite: 6]:

* **First term ($e^{2x - 3}$):** Apply the Chain Rule[cite: 6].
  $$\frac{d}{dx}\left[e^{2x - 3}\right] = e^{2x - 3} \cdot \frac{d}{dx}(2x - 3) = 2e^{2x - 3}$$

* **Second term ($5^x$):** Apply the General Exponential Rule $\frac{d}{dx}[a^x] = a^x \ln a$[cite: 6].
  $$\frac{d}{dx}\left[5^x\right] = 5^x \ln 5$$

Combining both parts gives[cite: 6]:
$$f'(x) = 2e^{2x - 3} + 5^x \ln 5$$

---

#### 2. Explanation of the additional factors

* **Why the factor 2 appears in the first term:**
  The term $e^{2x - 3}$ is a composite function where $u(x) = 2x - 3$ is the inner exponent[cite: 6]. By the **Chain Rule**, the derivative of $e^{u}$ with respect to $x$ requires multiplying by the derivative of the inner function $u'(x) = \frac{d}{dx}(2x - 3) = 2$[cite: 6].

* **Why $\ln 5$ appears in the second term:**
  The base of $5^x$ is $5$, not $e$[cite: 6]. Since natural logarithms are base $e$, converting $5^x$ to base $e$ gives $5^x = e^{x \ln 5}$[cite: 6]. Differentiating $e^{x \ln 5}$ with respect to $x$ brings down the constant factor $\ln 5$ from the exponent via the Chain Rule[cite: 6].
