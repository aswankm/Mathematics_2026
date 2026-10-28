## Problem 8. Number of Requests Handled by a Server

The rate at which requests arrive at a server during the first 5 minutes is described by the function

$$r(t) = 100 + 20t \quad [\text{requests/min}], \quad 0 \leq t \leq 5.$$

1. Compute the total number of requests that arrived during this time.
2. Compute the average rate of incoming requests over this interval.
3. Compare the average rate with the values $r(0)$ and $r(5)$.

> Why this problem: it shows the integral as summation of a varying rate in an example directly related to computer science.

---

### Solution

#### 1. Total Number of Requests
The total number of requests $R$ arriving between $t = 0$ and $t = 5$ minutes is the integral of the rate function $r(t)$:

$$R = \int_{0}^{5} r(t) \, dt = \int_{0}^{5} (100 + 20t) \, dt$$

Evaluating the antiderivative:
$$\int (100 + 20t) \, dt = 100t + 10t^2$$

Applying the integration bounds from $0$ to $5$:
$$R = \left[ 100(5) + 10(5)^2 \right] - \left[ 100(0) + 10(0)^2 \right]$$
$$R = (500 + 10 \cdot 25) - 0 = 500 + 250 = 750\text{ requests}$$

Thus, **750 requests** arrived during the first 5 minutes.

---

#### 2. Average Rate of Incoming Requests
The average rate $r_{\text{avg}}$ over the interval $[0, 5]$ is given by:

$$r_{\text{avg}} = \frac{1}{5 - 0} \int_{0}^{5} r(t) \, dt$$

Using the result $R = 750$ from part 1:
$$r_{\text{avg}} = \frac{750}{5} = 150\text{ requests/min}$$

---

#### 3. Comparison with $r(0)$ and $r(5)$
Evaluate $r(t)$ at the endpoints of the interval:
* $r(0) = 100 + 20(0) = 100\text{ requests/min}$
* $r(5) = 100 + 20(5) = 100 + 100 = 200\text{ requests/min}$

Calculating the arithmetic mean of $r(0)$ and $r(5)$:
$$\frac{r(0) + r(5)}{2} = \frac{100 + 200}{2} = 150\text{ requests/min}$$

**Comparison:** 
The average rate $r_{\text{avg}} = 150$ is exactly equal to the midpoint value and the arithmetic mean of the initial rate $r(0) = 100$ and final rate $r(5) = 200$. This occurs because $r(t)$ is a linear function.
