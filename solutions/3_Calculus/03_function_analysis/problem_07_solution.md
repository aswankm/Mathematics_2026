## Problem 7. A Trigonometric Function[cite: 2]

On $[0, 2\pi]$, find the intervals of monotonicity and the extrema of[cite: 2]

$$f(x) = \sin x + \cos x.[cite: 2]$$

Include the endpoints of the interval and compare the function values at the critical points and at the endpoints[cite: 2].

> **Why this problem:** it practices the analysis of a periodic function on a bounded interval[cite: 2].

---

## Solution

### 1. Derivative and Critical Points
To find the critical points, compute the first derivative of $f(x)$:
$$f'(x) = \cos x - \sin x$$

Set $f'(x) = 0$ on the interval $[0, 2\pi]$:
$$\cos x - \sin x = 0 \implies \sin x = \cos x \implies \tan x = 1$$

The solutions in the interval $[0, 2\pi]$ are:
$$x = \frac{\pi}{4} \quad \text{and} \quad x = \frac{5\pi}{4}$$

### 2. Monotonicity (Intervals of Increase and Decrease)
We test the sign of $f'(x) = \cos x - \sin x$ across the intervals partitioned by the critical points:
* **For $\left(0, \frac{\pi}{4}\right)$** (e.g., $x = 0$): $f'(0) = \cos(0) - \sin(0) = 1 > 0$ (Increasing)
* **For $\left(\frac{\pi}{4}, \frac{5\pi}{4}\right)$** (e.g., $x = \pi$): $f'(\pi) = \cos(\pi) - \sin(\pi) = -1 - 0 = -1 < 0$ (Decreasing)
* **For $\left(\frac{5\pi}{4}, 2\pi\right)$** (e.g., $x = \frac{3\pi}{2}$): $f'\left(\frac{3\pi}{2}\right) = \cos\left(\frac{3\pi}{2}\right) - \sin\left(\frac{3\pi}{2}\right) = 0 - (-1) = 1 > 0$ (Increasing)

* **Increasing on:** $\left[0, \frac{\pi}{4}\right) \cup \left(\frac{5\pi}{4}, 2\pi\right]$
* **Decreasing on:** $\left(\frac{\pi}{4}, \frac{5\pi}{4}\right)$

### 3. Extremum Values and Endpoint Comparison
Evaluate the function $f(x) = \sin x + \cos x$ at the critical points and the boundary endpoints:

| Location $x$ | Calculation | Value of $f(x)$ | Classification |
| :---: | :--- | :---: | :--- |
| $x = 0$ | $\sin(0) + \cos(0)$ | $1$ | Left Endpoint |
| $x = \frac{\pi}{4}$ | $\sin\left(\frac{\pi}{4}\right) + \cos\left(\frac{\pi}{4}\right)$ | $\sqrt{2} \approx 1.414$ | **Absolute Maximum** |
| $x = \frac{5\pi}{4}$ | $\sin\left(\frac{5\pi}{4}\right) + \cos\left(\frac{5\pi}{4}\right)$ | $-\sqrt{2} \approx -1.414$ | **Absolute Minimum** |
| $x = 2\pi$ | $\sin(2\pi) + \cos(2\pi)$ | $1$ | Right Endpoint |

* **Absolute Maximum:** $\sqrt{2}$ at $x = \frac{\pi}{4}$[cite: 2]
* **Absolute Minimum:** $-\sqrt{2}$ at $x = \frac{5\pi}{4}$[cite: 2]
```[cite: 2]
