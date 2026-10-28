## Problem 6. When Does a Logarithm Appear from an Integral?

**Statement:**
Compute 

$$\int \frac{2x}{x^2+5} \, dx$$

Identify the denominator as a candidate for substitution, compare the numerator with its derivative, and explain the source of the logarithm in the result[cite: 2].

> **Why this problem:** it teaches how to recognize the structure "derivative of the denominator over the denominator."[cite: 2]

---

### Solution

#### 1. Identify the Substitution Candidate
Let the denominator be our substitution variable $u$:
$$u = x^2 + 5$$

#### 2. Find the Differential
Compute the derivative of $u$ with respect to $x$:
$$\frac{du}{dx} = 2x \implies du = 2x \, dx$$
Notice that the numerator of our integrand is $2x \, dx$, which matches $du$ exactly.

#### 3. Rewrite and Evaluate the Integral
Substitute $u$ and $du$ into the integral:
$$\int \frac{2x}{x^2+5} \, dx = \int \frac{1}{u} \, du$$

Integrating with respect to $u$ gives:
$$\int \frac{1}{u} \, du = \ln|u| + C$$

#### 4. Substitute Back in Terms of $x$
Replace $u$ with $x^2 + 5$:
$$\ln|x^2 + 5| + C$$
Since $x^2 + 5 > 0$ for all real numbers $x$, the absolute value bars can be written as standard parentheses:
$$\ln(x^2 + 5) + C$$

#### 5. Verification by Differentiation
To verify the result, differentiate our antiderivative with respect to $x$ using the chain rule:
$$\frac{d}{dx} \left[ \ln(x^2 + 5) + C \right] = \frac{1}{x^2 + 5} \cdot \frac{d}{dx}(x^2 + 5) = \frac{2x}{x^2 + 5}$$
This matches the original integrand, verifying the result.

#### 6. Explanation of the Source of the Logarithm
The natural logarithm appears because the integral takes the form $\int \frac{1}{u} \, du$ after substitution. Whenever the numerator of a rational function is the exact derivative of its denominator (or a constant multiple of it), the substitution method leads directly to the standard integration rule $\int \frac{1}{u} \, du = \ln|u| + C$.
