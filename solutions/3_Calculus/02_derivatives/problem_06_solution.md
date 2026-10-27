## Problem 6. Product Rule and Trigonometry

### Statement

For 

$$f(x) = x\sin x + \cos x$$

Compute the derivative and simplify the result. Then compute $f'(0)$ and interpret the direction of the tangent line at that point[cite: 5].

* **Why this problem:** It combines the product rule with trigonometric derivatives and geometric interpretation[cite: 5].

---

### Solution

#### 1. Compute the derivative
Apply the Product Rule $\frac{d}{dx}[u \cdot v] = u'v + uv'$ to the first term $x\sin x$[cite: 5]:

* For $x\sin x$: 
  $$\frac{d}{dx}(x\sin x) = (1)\sin x + x(\cos x) = \sin x + x\cos x$$

* For $\cos x$: 
  $$\frac{d}{dx}(\cos x) = -\sin x$$

Combine both parts:
$$f'(x) = (\sin x + x\cos x) - \sin x$$

#### 2. Simplify the result
The $\sin x$ terms cancel out:
$$f'(x) = x\cos x$$

#### 3. Compute $f'(0)$
Substitute $x = 0$ into the simplified derivative[cite: 5]:
$$f'(0) = 0 \cdot \cos(0) = 0 \cdot 1 = 0$$

#### 4. Geometric interpretation of the direction of the tangent line
Since $f'(0) = 0$, the slope of the tangent line at $x = 0$ is zero[cite: 5]. This means the tangent line to the graph of $f(x)$ at $x = 0$ is **completely horizontal**[cite: 5].
