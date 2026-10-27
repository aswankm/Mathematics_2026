## Problem 13. A Multi-Layer Composition

### Statement

For 

$$f(x) = e^{\sin(x^2)}$$

compute the derivative. First write the layers:

$$x \longrightarrow x^2 \longrightarrow \sin(x^2) \longrightarrow e^{\sin(x^2)}$$

and explain why differentiation moves through them in the reverse order.

* **Why this problem:** It develops the chain rule as a method for working with multiple layers.

---

### Solution

#### 1. Identify the layers (Inner to Outer)
* **Layer 1 (Innermost):** $u = x^2$
* **Layer 2 (Middle):** $v = \sin(u) = \sin(x^2)$
* **Layer 3 (Outermost):** $f = e^v = e^{\sin(x^2)}$

---

#### 2. Compute the derivative using the Chain Rule
Work from the outermost layer to the innermost layer:

1. Differentiate the outer exponential layer: $\frac{d}{dv}[e^v] = e^v = e^{\sin(x^2)}$
2. Multiply by the derivative of the sine layer: $\frac{d}{du}[\sin(u)] = \cos(u) = \cos(x^2)$
3. Multiply by the derivative of the inner polynomial layer: $\frac{d}{dx}[x^2] = 2x$

Combining all factors according to the Chain Rule:

$$f'(x) = e^{\sin(x^2)} \cdot \cos(x^2) \cdot 2x$$

Rearranging the factors neatly:

$$f'(x) = 2x \cos(x^2) e^{\sin(x^2)}$$

---

#### 3. Explain why differentiation moves through layers in reverse order
* When evaluating $f(x)$ for a given input $x$, computation flows from the **inside out**: $x \to x^2 \to \sin(x^2) \to e^{\sin(x^2)}$.
* When differentiating, we measure how the **overall final output** changes relative to small changes in the original input $x$.
* By Leibniz notation for the chain rule:
  $$\frac{df}{dx} = \frac{df}{dv} \cdot \frac{dv}{du} \cdot \frac{du}{dx}$$
* Differentiation starts at the outermost output $f$ to see how it responds to the adjacent layer $v$, then sees how $v$ responds to $u$, and finally how $u$ responds to $x$. Thus, differentiation naturally unpacks the function from the **outside in** (reverse order).
