## Problem 2. A Parabola from the Perspective of the Derivative

For $f(x) = x^2 - 4x + 1$, find the minimum using the derivative. Compare the result with the vertex form and explain why both approaches lead to the same point.

> **Why this problem:** it connects a new tool with the familiar geometry of a parabola.

---

## Solution

### 1. Solution Using the Derivative
To find the minimum of the function using calculus, we find its first derivative and set it to zero to locate critical points:
$$f'(x) = \frac{d}{dx}(x^2 - 4x + 1) = 2x - 4$$

Set $f'(x) = 0$:
$$2x - 4 = 0 \implies x = 2$$

To confirm whether this critical point is a minimum, we can use the second derivative test:
$$f''(x) = \frac{d}{dx}(2x - 4) = 2$$
Since $f''(2) = 2 > 0$, the function is concave up at $x = 2$, meaning $x = 2$ yields a **local (and global) minimum**.

Now, evaluate the function at $x = 2$:
$$f(2) = (2)^2 - 4(2) + 1 = 4 - 8 + 1 = -3$$
* **Minimum Point via Derivative:** $(2, -3)$

---

### 2. Solution Using the Vertex Form (Completing the Square)
To convert the standard quadratic form $f(x) = ax^2 + bx + c$ into vertex form $f(x) = a(x - h)^2 + k$, we complete the square:
$$f(x) = (x^2 - 4x) + 1$$
Take half of the linear coefficient ($-\frac{4}{2} = -2$), square it ($(-2)^2 = 4$), and add/subtract it inside the expression:
$$f(x) = (x^2 - 4x + 4 - 4) + 1$$
$$f(x) = (x^2 - 4x + 4) - 4 + 1$$
$$f(x) = (x - 2)^2 - 3$$

From the vertex form $f(x) = a(x - h)^2 + k$, the vertex $(h, k)$ is:
* **Vertex / Minimum Point:** $(2, -3)$

---

### 3. Comparison and Explanation
* **Comparison:** Both approaches yield the exact same minimum point, **$(2, -3)$**.
* **Why they lead to the same point:** 
  1. **The Derivative Approach** looks for the point where the tangent line is horizontal ($f'(x) = 0$). For a parabola opening upwards ($a > 0$), the vertex is precisely the lowest point on the curve, which is also the unique point where the slope of the tangent line is zero.
  2. **The Vertex Form** algebraically shifts the parabola to isolate its turning point (vertex) by completing the square, exposing the minimum value directly as the constant $k$ when the squared term evaluates to zero. 
  Thus, finding where the derivative vanishes is the calculus equivalent of locating the vertex of a parabola.
